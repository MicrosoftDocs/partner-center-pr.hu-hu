---
title: Privát Azure Marketplace létrehozása és kezelése Azure Portal
description: Ismerje meg, hogyan hozhat létre és kezelhet privát Azure Marketplace-t (előzetes verzió) a Azure Portal.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/18/2020
ms.openlocfilehash: c0a395a7c5bfe926cdc56d7386aaaebb0305fb68
ms.sourcegitcommit: d31c06022624ca2d1db12b3c60ef1d0a3861f763
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/19/2020
ms.locfileid: "92528422"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Privát Azure Marketplace létrehozása és kezelése (előzetes verzió) a Azure Portal

A privát Azure Marketplace (előzetes verzió) lehetővé teszi, hogy a rendszergazdák szabályozzák, hogy a felhasználók mely harmadik féltől származó megoldásokat használhatják. Ezzel lehetővé teszi, hogy csak az Ön által jóváhagyott és a vállalati szabályzatoknak megfelelő ajánlatokat telepítse. A privát Azure piactéren a felhasználók az online áruházban kereshetik meg a megfelelő ajánlatokat a vásárláshoz és az üzembe helyezéshez. 

Piactéri rendszergazdaként (hozzárendelt szerepkör) egy letiltott és üres privát tárolóval kell kezdenie, ahol a jóváhagyott ajánlatokat és csomagokat is felveheti. Ez a cikk bemutatja, hogyan hozhat létre, kezelhet és engedélyezhet privát Azure Marketplace-t a felhasználók számára.

Megjegyzések:

- A privát Azure piactér bérlői szinten található, így a bérlő összes felhasználója ugyanazokat a kurátori listát fogja látni.
- Az összes Microsoft-megoldás automatikusan hozzáadódik a privát Azure Marketplace-hez.

## <a name="assign-the-marketplace-admin-role"></a>A piactér rendszergazdai szerepkörének kiosztása

A bérlői globális rendszergazdának hozzá kell rendelnie a **piactér rendszergazdai** szerepkörét a privát Azure Marketplace-rendszergazda számára, aki felügyelni fogja a saját tárolót.

>[!IMPORTANT]
> Az Azure Marketplace-en való hozzáférés csak a piactér rendszergazdai szerepkörrel rendelkező rendszergazdák számára érhető el.

### <a name="prerequisites"></a>Előfeltételek

Ezeket az előfeltételeket csak akkor kell teljesítenie, ha a piactér rendszergazdai szerepkört a bérlői hatókörben lévő felhasználóhoz rendeli hozzá:

- **Globális rendszergazda** felhasználóhoz férhet hozzá.
- A bérlőnek legalább egy előfizetése van (bármilyen típus lehet).
- A globális rendszergazda felhasználó a 2. lépésben kiválasztott előfizetéshez rendeli hozzá a **közreműködő** szerepkört vagy magasabb szintűt.
- A globális rendszergazda felhasználó emelt szintű hozzáféréssel rendelkezik az **Igen** értékre (lásd: [Jogosultságszint-emelés – hozzáférés-globális-rendszergazda](/azure/role-based-access-control/elevate-access-global-admin)).

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>A piactér rendszergazdai szerepkörének kiosztása a PowerShell-lel

A piactér rendszergazdai szerepkörének hozzárendeléséhez használja a következő PowerShell-parancsfájlt: Ehhez a következő paramétereket kell megadni:

- **TenantId:** A hatókörben lévő bérlő azonosítója (a piactér rendszergazdai szerepköre a bérlői hatókörben rendelhető hozzá).
- **SubscriptionId:** Egy előfizetés, amelynek globális rendszergazdája **közreműködői** szerepkörrel rendelkezik vagy magasabban van hozzárendelve.
- **GlobalAdminUsername:** A globális rendszergazda felhasználóneve.
- **UsernameToAssignRoleFor:** Annak a felhasználónévnek a neve, amelyhez a piactér-rendszergazdai szerepkör hozzá lesz rendelve.

> [!NOTE]
> A bérlőnek meghívott vendég felhasználók esetében akár 48 óráig is eltarthat, amíg a fiók elérhetővé válik a piactér rendszergazdai szerepkörének hozzárendeléséhez. További információ: [Azure Active Directory B2B csoportmunka-felhasználó tulajdonságai](/azure/active-directory/b2b/user-properties).

```PowerShell
function Assign-MarketplaceAdminRole {
[CmdletBinding()]
param(
[Parameter(Mandatory)]
[string]$TenantId,

[Parameter(Mandatory)]
[string]$SubscriptionId,

[Parameter(Mandatory)]
[string]$GlobalAdminUsername,

[Parameter(Mandatory)]
[string]$UsernameToAssignRoleFor
)

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin"

Write-Output "TenantId = $TenantId"
Write-Output "SubscriptionId = $SubscriptionId"
Write-Output "GlobalAdminUsername = $GlobalAdminUsername"
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor"

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)"

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

if($profile -eq $null)
{
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop
}
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername)
{
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)"
}
else
{
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)"
}

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."

$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

Az az. Portal PowerShell-modulban található parancsmagokkal kapcsolatos további információkért tekintse meg a [Microsoft Azure PowerShell: portál irányítópult-parancsmagokat](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Privát Azure piactér létrehozása

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).
2. Válassza **a minden szolgáltatás** , majd a **piactér** lehetőséget.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal fő ablak.":::

3. Válassza a **privát piactér** lehetőséget a bal oldalon található beállítások közül.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Azure Portal fő ablak.":::

4. Válassza az első **lépések** lehetőséget a privát Azure Marketplace létrehozásához (ezt csak egyszer kell megtennie).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Azure Portal fő ablak.":::

    Ha a bérlőhöz már létezik privát Azure Marketplace, akkor a **piactér kezelése** alapértelmezés szerint ki lesz választva.

5. Ha elkészült, üres és letiltott privát Azure Marketplace-t fog tartalmazni.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Azure Portal fő ablak.":::

## <a name="add-items-from-gallery"></a>Elemek hozzáadása a gyűjteményből

Az elemek egy ajánlat és egy csomag kombinációja. A piactér kezelése oldalon megkeresheti és hozzáadhatja az elemeket.

1. Válassza az **elemek hozzáadása** elemet.

2. Tallózással keresse **meg a katalógust, vagy a** Keresés mező használatával keresse meg a kívánt elemeket.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Azure Portal fő ablak.":::

3. Alapértelmezés szerint az új ajánlat hozzáadásakor az összes aktuális csomag hozzá lesz adva az engedélyezett listához. Ha módosítani szeretné a csomag kijelölését a kijelölt elemek hozzáadása előtt, válassza a legördülő menüt az ajánlat csempén, és frissítse a szükséges terveket.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Azure Portal fő ablak.":::

4. Kattintson a **kész** gombra a bal alsó sarokban, miután elvégezte a beállításokat.

>[!Note]
> Az **elemek hozzáadása** a piactérhez csak a nem Microsoft-ajánlatok számára érhető el. A Microsoft-ajánlatok alapértelmezés szerint engedélyezve vannak.

## <a name="edit-item-plans"></a>Elemszintű csomagok szerkesztése

A piactér kezelése oldalon szerkesztheti az elemek terveit.

1. A **csomagok** oszlopban tekintse át az elérhető csomagokat az adott elem legördülő menüjéből.
2. Jelölje be a jelölőnégyzeteket, vagy törölje a jelölést a felhasználók számára elérhetővé tenni kívánt csomagok kiválasztásához.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Azure Portal fő ablak.":::

> [!NOTE]
> Minden ajánlatnak legalább egy tervet ki kell választania, hogy a frissítés megtörténjen. Az ajánlattal kapcsolatos összes csomag eltávolításához törölje a teljes ajánlatot (lásd a következő szakaszt).

## <a name="delete-offers"></a>Ajánlatok törlése

A piactér kezelése lapon jelölje be az ajánlat neve melletti jelölőnégyzetet (lásd a fenti képernyőt), és válassza az **elemek törlése** lehetőséget.

## <a name="enabledisable-private-azure-marketplace"></a>Privát Azure Marketplace engedélyezése/letiltása

A piactér kezelése oldalon láthatja az alábbi szalagcímeket, amelyek a privát Azure Marketplace aktuális állapotát mutatják be:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Azure Portal fő ablak.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Azure Portal fő ablak.":::

Igény szerint engedélyezheti vagy letilthatja a privát Azure Marketplace-t.

1. Ha le van tiltva, válassza a **saját piactér** engedélyezése lehetőséget.
2. Ha engedélyezve van, a letiltáshoz válassza a **privát piactér letiltása** lehetőséget.

## <a name="browsing-private-azure-marketplace"></a>Privát Azure piactér tallózása

Ha a privát Azure Marketplace engedélyezve van, a felhasználók láthatják, hogy a piactér rendszergazdája milyen terveket engedélyezett.

- A zöld **megengedett** értesítés egy olyan partner (nem Microsoft) ajánlatot jelöl, amely engedélyezett.
- A kék **megengedett** értesítés egy engedélyezett Microsoft-ajánlatot jelez.

A felhasználók a (z) és a nem engedélyezett ajánlatok között szűrhetők:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Azure Portal fő ablak.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Vásárlás vagy üzembe helyezés a privát Azure piactéren

Míg a termék részletei lap a nyilvános Azure piactérhez hasonlóan működik, három privát Azure Marketplace-re vonatkozó forgatókönyv található.

- Ha egy felhasználó egy engedélyezett csomagot választ, a **Létrehozás** gomb engedélyezve lesz:

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Azure Portal fő ablak.":::

- Ha a felhasználó egy nem engedélyezett csomagot választ ki, a szalagcím megjegyzi, hogy a csomag nem engedélyezett, és a **Létrehozás** gomb le van tiltva.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Azure Portal fő ablak.":::

- Ha a termékre vonatkozó csomag kiválasztása nem jelenik meg a termék részletei lapon, de a rendszergazda jóváhagyta egy vagy több csomagot, a szalagcím megállapítja, hogy mely csomagok engedélyezettek, és engedélyezve van a **Létrehozás** gomb:

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Azure Portal fő ablak.":::

## <a name="contact-support"></a>Kapcsolatfelvétel a támogatási szolgáltatással

Az Azure Marketplace támogatásához látogasson el a [Microsoft Q&a](/answers/products/)-ra. 
