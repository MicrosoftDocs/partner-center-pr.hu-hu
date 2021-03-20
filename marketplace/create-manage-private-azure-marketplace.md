---
title: Privát Azure Marketplace létrehozása és kezelése a Azure Portal
description: Ismerje meg, hogyan hozhat létre és kezelhet privát Azure Marketplace-t (előzetes verzió) a Azure Portal. A privát Azure Marketplace (előzetes verzió) lehetővé teszi, hogy a rendszergazdák szabályozzák, hogy a felhasználók mely harmadik féltől származó megoldásokat használhatják.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8cfe0e95d1655530c9bc9d24b1efe85e6432236b
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712766"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Privát Azure Marketplace létrehozása és kezelése a Azure Portal

A privát Azure piactér lehetővé teszi, hogy a rendszergazdák szabályozzák, hogy a felhasználók mely harmadik féltől származó megoldásokat használhatják. Ez a beállítás lehetővé teszi, hogy a felhasználó csak a rendszergazda által jóváhagyott ajánlatokat telepítsen, és megfeleljen a vállalat szabályzatának. A privát Azure piactéren a felhasználók megkereshetik és üzembe helyezhetik a megfelelő ajánlatokat az online áruházban.

Piactéri rendszergazdaként (hozzárendelt szerepkör) egy letiltott és üres privát tárolóval kell kezdenie, ahol a jóváhagyott ajánlatokat és csomagokat is felveheti. Ez a cikk a szükséges szerepkör hozzárendelését, a privát tárolók létrehozását, az elemek kezelését, a felhasználói kérések jóváhagyását és a saját Azure Marketplace engedélyezését mutatja be a felhasználók számára.

> [!NOTE]
> - A privát Azure piactér bérlői szinten található, így a bérlő összes felhasználója ugyanazokat a kurátori listát fogja látni.
> - Az összes Microsoft-megoldás (beleértve a [támogatott Linux-disztribúciókat](/azure/virtual-machines/linux/endorsed-distros)is) automatikusan hozzá lesz adva a privát Azure Marketplace-hez.

## <a name="assign-the-marketplace-admin-role"></a>A piactér rendszergazdai szerepkörének kiosztása

A bérlői globális rendszergazdának hozzá kell rendelnie a **piactér rendszergazdai** szerepkörét a privát Azure Marketplace-rendszergazda számára, aki felügyelni fogja a saját tárolót.

>[!IMPORTANT]
> Az Azure Marketplace-en való hozzáférés csak a piactér rendszergazdai szerepkörrel rendelkező rendszergazdák számára érhető el.

### <a name="prerequisites"></a>Előfeltételek

Ezek az előfeltételek akkor szükségesek, ha a piactér rendszergazdai szerepkört a bérlői hatókörben lévő felhasználóhoz rendeli hozzá:

- **Globális rendszergazda** felhasználóhoz férhet hozzá.
- A bérlőnek legalább egy előfizetése van (bármilyen típus lehet).
- A kiválasztott előfizetéshez a globális rendszergazda felhasználó hozzá van rendelve a **közreműködő** szerepkörhöz vagy magasabbhoz.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>A piactér rendszergazdai szerepkörének kiosztása hozzáférés-vezérléssel (IAM)

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).
1. Válassza **a minden szolgáltatás** , majd a **piactér** lehetőséget.
1. Válassza a **privát piactér** lehetőséget a bal oldali menüben.

    [![Megjeleníti a piactér bal oldalán található privát piactér menüpontot.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. A piactér rendszergazdai szerepkörének hozzárendeléséhez válassza a **hozzáférés-vezérlés (iam)** lehetőséget.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Megjeleníti az I M hozzáférés-vezérlési képernyőt.":::

1. Válassza a **+ Hozzáadás** > **Szerepkör-hozzárendelés hozzáadása** lehetőséget.
1. A **szerepkör** területen válassza a **piactér rendszergazdája** elemet.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="A szerepkör-hozzárendelés menüt jeleníti meg.":::

1. Válassza ki a kívánt felhasználót a legördülő listából, majd válassza a **kész** lehetőséget.

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

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

Az az. Portal PowerShell-modulban található parancsmagokkal kapcsolatos további információkért tekintse meg a [Microsoft Azure PowerShell: portál irányítópult-parancsmagokat](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Privát Azure piactér létrehozása

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).
2. Válassza **a minden szolgáltatás** , majd a **piactér** lehetőséget.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Megjeleníti a Azure Portal fő ablakát.":::

3. Válassza a **privát piactér** lehetőséget a bal oldali menüben.

4. Válassza az első **lépések** lehetőséget a privát Azure Marketplace létrehozásához (ezt csak egyszer kell megtennie).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Bemutatja, hogyan választható ki az &quot;első lépések a Azure Portal&quot; főablakban.":::

    Ha a bérlőhöz már létezik privát Azure Marketplace, akkor a **piactér kezelése** alapértelmezés szerint ki lesz választva.

5. Ha elkészült, üres és letiltott privát Azure Marketplace-t fog tartalmazni.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Megjeleníti az üres privát Azure Marketplace-képernyőt.":::

## <a name="add-items-from-gallery"></a>Elemek hozzáadása a gyűjteményből

Az elemek egy ajánlat és egy csomag kombinációja. A piactér kezelése oldalon kereshet és hozzáadhat elemeket.

1. Válassza az **elemek hozzáadása** elemet.

2. Tallózással keresse **meg a katalógust, vagy a** Keresés mező használatával keresse meg a kívánt elemeket.

    [![Bemutatja, hogyan böngészhet a katalógusban, vagy hogyan használhatja a keresési mezőt.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Alapértelmezés szerint új ajánlat hozzáadásakor a rendszer az összes aktuális csomagot hozzáadja a jóváhagyott listához. Ha módosítani szeretné a csomag kijelölését a kijelölt elemek hozzáadása előtt, válassza a legördülő menüt az ajánlat csempén, és frissítse a szükséges terveket.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Bemutatja a szükséges csomagok frissítésének módját.":::

4. Kattintson a **kész** gombra a bal alsó sarokban, miután elvégezte a beállításokat.

>[!Note]
> Az **elemek hozzáadása** a piactérhez csak a nem Microsoft-ajánlatok számára érhető el. A Microsoft-megoldások (beleértve a [támogatott Linux-disztribúciókat](/azure/virtual-machines/linux/endorsed-distros)) "alapértelmezés szerint jóváhagyva" néven lesznek megjelölve, és nem kezelhetők a privát piactéren.

## <a name="edit-items-plans"></a>Az elemek csomagjainak szerkesztése

A piactér kezelése lapon szerkesztheti az elemek terveit.

1. A **csomagok** oszlopban tekintse át az elérhető csomagokat az adott elem legördülő menüjéből.
2. Jelölje be a jelölőnégyzeteket, vagy törölje a jelölést a felhasználók számára elérhetővé tenni kívánt csomagok kiválasztásához.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Azt mutatja be, hogyan lehet kijelölni vagy törölni a kötelező elemhez tartozó jelölőnégyzetet.":::

> [!NOTE]
> Minden ajánlatnak legalább egy, a frissítéshez kiválasztott csomagra van szüksége. Az ajánlattal kapcsolatos összes csomag eltávolításához törölje a teljes ajánlatot (lásd a következő szakaszt).

## <a name="delete-offers"></a>Ajánlatok törlése

A piactér kezelése lapon jelölje be az ajánlat neve melletti jelölőnégyzetet (lásd a fenti képernyőt), és válassza az **elemek törlése** lehetőséget.

## <a name="enabledisable-private-azure-marketplace"></a>Privát Azure Marketplace engedélyezése/letiltása

A piactér kezelése oldalon láthatja az alábbi szalagcímeket, amelyek a privát Azure Marketplace aktuális állapotát mutatják be:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Az állapot letiltásának szalagcímét jeleníti meg.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Az &quot;állapot engedélyezése&quot; szalagcímet jeleníti meg.":::

Igény szerint engedélyezheti vagy letilthatja a privát Azure Marketplace-t.

- Ha le van tiltva, válassza a **saját piactér** engedélyezése lehetőséget.
- Ha engedélyezve van, a letiltáshoz válassza a **privát piactér letiltása** lehetőséget.

## <a name="private-azure-marketplace-notification-center"></a>Privát Azure Marketplace-értesítési központ

Az értesítési központ háromféle típusú értesítésből áll, és lehetővé teszi, hogy a piactér rendszergazdája a következő értesítés alapján tegyen lépéseket:

- A jóváhagyott listán nem szereplő elemekre vonatkozó jóváhagyási kérések a felhasználóktól (lásd [az ajánlatok vagy a csomagok hozzáadására vonatkozó kérést](#request-to-add-offers-or-plans) ).
- Új csomag-értesítések olyan ajánlatokhoz, amelyeken már van egy vagy több csomag a jóváhagyott listában.
- A rendszer eltávolította a jóváhagyott listán szereplő elemek megtervezésére vonatkozó értesítéseket, de eltávolították őket a globális Azure piactéren.

Az értesítési központ elérése:

1. Válassza az **értesítések** lehetőséget a bal oldali menüben.

    [![Az értesítések menüt jeleníti meg.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Válassza a három pont menüt a további műveletek elvégzéséhez.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="A további beállítások menü eredményét jeleníti meg.":::

1. A csomagra vonatkozó kérelmek esetében a **kérelmek megjelenítése** lehetőség megnyitja a jóváhagyási kérelem űrlapot, ahol áttekintheti az adott ajánlat összes felhasználói kérelmét.
1. Válassza a **jóváhagyás** vagy az **elutasítás** lehetőséget.

    [![Megjeleníti a jóváhagyás és az elutasítás lehetőséget.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Válassza ki a jóváhagyni kívánt tervet a legördülő menüből.
1. Adjon hozzá egy megjegyzést, és válassza a **Küldés** lehetőséget.

## <a name="browsing-private-azure-marketplace"></a>Privát Azure piactér tallózása

Ha a privát Azure Marketplace engedélyezve van, a felhasználók láthatják, hogy a piactér rendszergazdája mely terveket hagyta jóvá.

- A zöld **jóváhagyott** nyilatkozat egy jóváhagyott partner (nem Microsoft) ajánlatot jelöl.
- A kék **jóváhagyott** értesítés a jóváhagyott Microsoft-ajánlatokat (beleértve a [támogatott Linux-disztribúciókat](/azure/virtual-machines/linux/endorsed-distros)is) jelzi.

A felhasználók a nem jóváhagyott ajánlatok között szűrhetik a következőket:

[![Megjeleníti a szűrési lehetőséget.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Vásárlás vagy üzembe helyezés a privát Azure piactéren

Míg a termék részletei lap a globális Azure piactérhez hasonlóan működik, három privát Azure Marketplace-re vonatkozó forgatókönyv található.

- Ha egy felhasználó jóváhagyott csomagot választ, a **Létrehozás** gomb engedélyezve lesz:

    [![Megjeleníti az ajánlati szalagcímet, amelyből egy terv hozható létre.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Ha a termékre vonatkozó csomag kiválasztása nem jelenik meg a termék részletei lapon, de a rendszergazda jóváhagyta egy vagy több csomagot, a rendszer egy szalagcímet jelenít meg, amelyet jóváhagy, és engedélyezve van a **Létrehozás** gomb:

    [![Megjeleníti az ajánlati szalagcímet, amely szerint egy terv hozható létre, és megjeleníthető az elérhető csomagok.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Ha a felhasználó egy nem jóváhagyott csomagot választ, a szalagcím nem jóváhagyottként veszi fel a csomagot, és a **Létrehozás** gomb le lesz tiltva. A felhasználó továbbra is kérheti a terv hozzáadását a jóváhagyott listához (lásd a következő szakaszt).

## <a name="request-to-add-offers-or-plans"></a>Ajánlatok és csomagok hozzáadására vonatkozó kérelem

Kérheti, hogy olyan nyilvános ajánlatot vagy csomagot adjon hozzá, amely jelenleg nem lett jóváhagyva a privát Azure piactéren.

1. Válassza ki a szalagcímbe **felvenni kívánt kérelmet** a **hozzáférési kérelem űrlapjának** megnyitásához.

    [![Megjeleníti a "kérés a hozzáadáshoz" hivatkozást tartalmazó szalagcímet.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Az ajánlatok és csomagok hozzáférési kérelmi űrlapját jeleníti meg.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Válassza ki, hogy melyik csomagot kívánja hozzáadni a kérelemhez (**bármely csomag** azt jelzi, hogy a piactér rendszergazdája nem rendelkezik az ajánlaton belüli csomagokra vonatkozó beállításokkal).

1. Adjon meg egy **indoklást** , és válassza a **kérelem** lehetőséget a kérelem elküldéséhez.
  
    [![Az ajánlatok és csomagok hozzáférési kérelmi űrlapját jeleníti meg a minták bejegyzéseivel.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Egy függőben lévő kérés jelzése megjelenik a hozzáférési kérelem űrlapján a **kérelem visszavonására** szolgáló lehetőséggel.

    [![A visszavont kérelmek hivatkozással rendelkező jóváhagyott vagy függőben lévő csomagok listáját jeleníti meg.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> A jóváhagyást követően a rendszer elküldi a jóváhagyási kérelem űrlapját [a piactér](#private-azure-marketplace-notification-center) rendszergazdája számára a kérelem áttekintéséhez és a művelet elvégzéséhez.

## <a name="frequently-asked-questions-faqs"></a>Gyakori kérdések (GYIK)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Már blokkolja a Marketplace harmadik féltől származó alkalmazást a Azure Policyon keresztül. Miben különbözik?

A harmadik féltől származó szolgáltatásokat jelenleg két módon lehet korlátozni a piactéren:

1. Az EA portálon vagy a Azure Portalon tiltsa le a harmadik féltől származó szolgáltatásokat, vagy korlátozza az "ingyenes vagy BYOL SKU-ra".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Bemutatja, hogyan lehet korlátozni a szolgáltatásokat a Azure Portalban.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Bemutatja, hogyan lehet korlátozni a szolgáltatásokat az E-portálon.":::

2. Hozzon létre egy Azure-szabályzatot, hogy csak bizonyos virtuális gépeket engedélyezzen. A Windows rendszerű virtuális gépekre vonatkozó szabályzatok kikapcsolásával kapcsolatos további információkért lásd: [házirendek alkalmazása a Windows rendszerű virtuális gépekre Azure Resource Manager használatával](/azure/virtual-machines/windows/policy).

A privát Azure piactér nagyobb rugalmasságot tesz lehetővé az egyes ajánlatok és csomagok korlátozására és engedélyezésére. A végfelhasználók számára elérhetővé teszi a Piactéri katalógusban való üzembe helyezést, még mielőtt külső szolgáltatásokat próbálnak üzembe helyezni. A harmadik féltől származó szolgáltatások üzembe helyezésének engedélyezéséhez állítsa be az Azure Marketplace-t az EA Portálon és a Azure Portalon.

- A privát Azure Marketplace-en a partneri megoldások nem korlátozódnak a virtuális gépekre.
- A privát Azure Marketplace a csomag szintjén is megadható, és az "aktuális és jövőbeli terv" is megadható.
- A privát Azure piactér tájékoztathatja a végfelhasználókat arról, hogy mit lehet és nem lehet telepíteni.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Mi a különbség a privát ajánlat és a privát Azure Marketplace között?

A **privát ajánlat** lehetővé teszi, hogy a kiadók olyan csomagokat hozzanak létre, amelyek csak a célközönség számára láthatók. Ez lehetővé teszi, hogy a testreszabott megoldásokat megosszák az egyeztetett díjszabással, a privát feltételekkel és a speciális konfigurációkkal. Részletekért lásd: [privát ajánlatok a kereskedelmi piactéren](/azure/marketplace/private-offers).

A Azure Portal **privát Azure Marketplace** lehetővé teszi a rendszergazdák számára, hogy előzetesen hagyják el, hogy a felhasználók milyen külső megoldásokat telepíthetnek. A privát Azure piactéren a felhasználók a megfelelő ajánlatok megkeresésével, megvásárlásával és üzembe helyezésével élvezheti az Azure Marketplace előnyeit. Az előfizetés-alapú privát ajánlatok felügyeletéhez a piactér rendszergazdájának legalább "READ" szerepkörrel kell rendelkeznie az adott előfizetésben.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Felvettem egy privát ajánlatot a privát Azure Marketplace-re, miért nem jelenik meg a piactér kezelése lapon?

Az előfizetés-alapú privát ajánlatok csak a privát ajánlat beállításaiban felsorolt előfizetések esetében láthatók. A privát ajánlat megtekintéséhez győződjön meg arról, hogy a globális előfizetés-szűrő az összes előfizetést megjeleníti.

[![A privát piactér szűrőjét jeleníti meg.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Használhatunk egyéni lemezképeket a privát Azure piactéren?

Nem. A privát Azure Marketplace lehetővé teszi a rendszergazda számára, hogy a globális Azure piactéren felügyelje és betekintse harmadik féltől származó megoldásokat. Mivel az egyéni lemezképek nem a globális Azure Marketplace piactéren találhatók, a rendszergazda nem választhat ki és nem választhatja ki az egyéni lemezképeket. Ha egyéni rendszerképeket szeretne megosztani, használja a [megosztott képtárat](/azure/virtual-machines/shared-image-galleries).

1. Részletes útmutató a közös rendszerkép-katalógus ([parancssori](/azure/virtual-machines/shared-images-cli)felület, [PowerShell](/azure/virtual-machines/shared-images-powershell)) létrehozásához.
2. Rendszerkép-definíció létrehozása a SIG-ban. Az ügyfélnek az operációs rendszer állapot mezőjében **általánosított** elemet kell választania. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Felügyelt rendszerkép bekapcsolása a megosztott rendszerkép-katalógusba ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. A SIG VM-lemezképek egy előfizetésben találhatók. Ha más előfizetésekhez is elérhetővé kívánja tenni, használja az alkalmazás regisztrációját ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Miért jelenik meg, hogy egyes ajánlatok **alapértelmezés szerint jóvá vannak hagyva** , noha a közzétevő nem a Microsoft?

A Microsoft támogatja a Linux és a nyílt forráskódú technológiák használatát az Azure-ban. A támogatott [Linux-disztribúciók](/azure/virtual-machines/linux/endorsed-distros) az Azure-ban támogatottak, és az ár a virtuális gépeken van integrálva. Mivel az Azure Linux-ügynök már előre telepítve van az Azure Marketplace-en, a Microsoft-ajánlathoz hasonló módon kezelik. Mivel a Microsoft ajánlatait alapértelmezés szerint jóváhagyják, a támogatott Linux-disztribúciók nem kezelhetők a privát Azure piactéren, és alapértelmezés szerint jóváhagyjuk azokat.

## <a name="contact-support"></a>Kapcsolatfelvétel a támogatási szolgáltatással

- Az Azure Marketplace támogatásához látogasson el a [Microsoft Q&a](/answers/products/)-ra.