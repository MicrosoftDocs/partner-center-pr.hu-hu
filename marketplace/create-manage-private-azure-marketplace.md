---
title: Privát fiók létrehozása Azure Marketplace és kezelése a Azure Portal
description: Ismerje meg, hogyan lehet privát Azure Marketplace (előzetes verzió) létrehozni és Azure Portal. A Azure Marketplace (előzetes verzió) lehetővé teszi a rendszergazdák számára, hogy szabályozzák, mely külső megoldásokat használhatják a felhasználók.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 9da9eb4944508e815d1664fb44b13bce52f37150
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431671"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Privát fiók létrehozása Azure Marketplace és kezelése a Azure Portal

A Azure Marketplace lehetővé teszi a rendszergazdák számára, hogy szabályozzák, mely külső megoldásokat használhatják a felhasználók. Ezt úgy teszi lehetővé, hogy a felhasználó csak a rendszergazda által jóváhagyott ajánlatokat telepítsen, és megfeleljen a vállalat szabályzatának. A Private Azure Marketplace lehetővé teszi, hogy a felhasználók az online áruházban megfelelő ajánlatokat keressenek a vásárláshoz és az üzembe helyezéshez.

Marketplace-rendszergazdaként (hozzárendelt szerepkör) egy letiltott és üres privát tárolóval fog kezdeni, ahol hozzáadhatja a jóváhagyott ajánlatokat és csomagokat. Ez a cikk bemutatja, hogyan rendelheti hozzá a szükséges szerepkört, hogyan hozhat létre privát tárolót, hogyan kezelheti az elemeket, hogyan hagyja jóvá a felhasználói kéréseket, és hogyan engedélyezheti a Azure Marketplace privát tárolókat a felhasználók számára.

> [!NOTE]
> - A privát Azure Marketplace bérlői szinten található, így a bérlő összes felhasználója ugyanazt az összeért listát fogja látni.
> - Minden Microsoft-megoldás (beleértve [a támogatott Linux-disztribúciókat](/azure/virtual-machines/linux/endorsed-distros)is) automatikusan hozzáadódik a privát Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>A Marketplace rendszergazdai szerepkör hozzárendelése

A bérlői globális rendszergazda **Marketplace** rendszergazdai szerepkört kell hozzárendelnie ahhoz a privát Azure Marketplace rendszergazdához, aki a privát tárolót fogja kezelni.

>[!IMPORTANT]
> A privát Azure Marketplace kezeléséhez való hozzáférés csak a Marketplace rendszergazdai szerepkörével társított rendszergazdák számára érhető el.

### <a name="prerequisites"></a>Előfeltételek

Ezek az előfeltételek ahhoz szükségesek, hogy a Marketplace-rendszergazdai szerepkört hozzárendelje egy felhasználóhoz a bérlői hatókörben:

- Hozzáféréssel rendelkezik **egy** globális rendszergazda felhasználóhoz.
- A bérlő legalább egy előfizetéssel rendelkezik (bármilyen típusú lehet).
- A globális rendszergazda felhasználóhoz a **választott** előfizetés közreműködői vagy magasabb szintű szerepköre van hozzárendelve.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>A Marketplace rendszergazdai szerepkör hozzárendelése hozzáférés-vezérléssel (IAM)

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).
1. Válassza a **Minden szolgáltatás,** majd a **Marketplace lehetőséget.**
1. A **bal oldali menüben** válassza a Privát piactér lehetőséget.

    [![Megjeleníti a privát Marketplace menüpontot a Marketplace bal oldalán.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Válassza **a Hozzáférés-vezérlés (IAM) lehetőséget** a Marketplace rendszergazdai szerepkörének hozzárendeléshez.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Megjeleníti az I A M hozzáférés-vezérlés képernyőjét.":::

1. Válassza a **+ Hozzáadás** > **Szerepkör-hozzárendelés hozzáadása** lehetőséget.
1. A Szerepkör **alatt** válassza a **Marketplace-rendszergazda lehetőséget.**

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Megjeleníti a Szerepkör-hozzárendelés menüt.":::

1. Válassza ki a kívánt felhasználót a legördülő listából, majd válassza a **Kész lehetőséget.**

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>A Marketplace rendszergazdai szerepkör hozzárendelése a PowerShell-sel

Az alábbi PowerShell-szkript használatával rendelje hozzá a Marketplace rendszergazdai szerepkörét; A használatához a következő paraméterekre van szükség:

- **TenantId (Bérlőazonosító):** A hatókörhöz tartozó bérlő azonosítója (a Marketplace rendszergazdai szerepkör hozzárendelhető a bérlői hatókörhöz).
- **SubscriptionId (Előfizetés-azonosító):** Egy előfizetés, amelynek a globális rendszergazda Közreműködő **szerepköre** vagy magasabb szintű hozzárendelt szerepköre van.
- **GlobalAdminUsername:** A globális rendszergazda felhasználóneve.
- **UsernameToAssignRoleFor:** A felhasználónév, amelyhez a Marketplace rendszergazdai szerepkör hozzá lesz rendelve.

> [!NOTE]
> A bérlőbe meghívott vendégfelhasználók esetén akár 48 órát is igénybe vehet, amíg a fiókjuk elérhetővé válik a Marketplace-rendszergazdai szerepkör hozzárendeléséhez. További információ: [Egy B2B Azure Active Directory felhasználó tulajdonságai.](/azure/active-directory/b2b/user-properties)

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

További információ az Az.Portal PowerShell-modulban található parancsmagokkal kapcsolatban: [Microsoft Azure PowerShell: Portal Dashboard parancsmagok](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Privát Azure Marketplace

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).
2. Válassza a **Minden szolgáltatás,** majd a **Marketplace lehetőséget.**

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Megjeleníti Azure Portal fő ablakát.":::

3. A **bal oldali menüben** válassza a Privát piactér lehetőséget.

4. Válassza **az Első lépések** lehetőséget a Azure Marketplace létrehozásához (ezt csak egyszer kell megtennie).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Bemutatja, hogyan választhatja ki az &quot;Első lépések a Azure Portal&quot; főablakot.":::

    Ha a Azure Marketplace már létezik privát fiók, alapértelmezés szerint a **Manage Marketplace (Piactér** kezelése) lehetőség van kiválasztva.

5. Ha elkészült, egy üres és letiltott Privát Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Megjeleníti az üres Privát Azure Marketplace képernyőt.":::

## <a name="add-items-from-gallery"></a>Elemek hozzáadása katalógusból

Az elem egy ajánlat és egy csomag kombinációja. A Marketplace kezelése oldalon kereshet és adhat hozzá elemeket.

1. Válassza **az Elemek hozzáadása lehetőséget.**

2. Tallózással **keresse** meg a katalógust, vagy a keresőmezővel keresse meg a kívánt elemet.

    [![Bemutatja, hogyan tallózhat a katalógusban vagy használhatja a keresőmezőt.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Új ajánlat hozzáadásakor alapértelmezés szerint az összes jelenlegi csomag fel lesz sorolva a jóváhagyottak listájára. Ha a kiválasztott elemek hozzáadása előtt módosítani szeretné a csomag kiválasztását, válassza ki a legördülő menüt az ajánlat csempéjéről, és frissítse a szükséges csomagokat.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Bemutatja, hogyan frissítheti a szükséges csomagokat.":::

4. A **kiválasztás után** válassza a bal alsó sarokban található Kész lehetőséget.

>[!Note]
> **Az Elemek hozzáadása** a Marketplace-hez csak a nem Microsoft-ajánlatokhoz lesz elérhető. A Microsoft-megoldások (beleértve a támogatott Linux-disztribúciókat is) alapértelmezés szerint jóváhagyottként lesznek megjelölve, és nem kezelhetők a privát Piactéren. [](/azure/virtual-machines/linux/endorsed-distros)

## <a name="edit-items-plans"></a>Elemtervek szerkesztése

Egy elem csomagját a Marketplace kezelése oldalon szerkesztheti.

1. A **Plans (Csomagok)** oszlopban tekintse át az elemhez elérhető csomagokat a legördülő menüből.
2. Jelölje be vagy törölje a jelölőnégyzeteket a felhasználók számára elérhetővé tenni kívánt csomagok kiválasztásához.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Bemutatja, hogyan jelölheti be vagy ürítheti ki a kötelező elem jelölőnégyzetét.":::

> [!NOTE]
> Minden ajánlatnak legalább egy kiválasztott csomagra van szüksége a frissítés következtéhez. Egy ajánlathoz kapcsolódó összes csomag eltávolításához törölje a teljes ajánlatot (lásd a következő szakaszt).

## <a name="delete-offers"></a>Ajánlatok törlése

A Marketplace kezelése oldalon jelölje be az ajánlat neve melletti jelölőnégyzetet (lásd a fenti képernyőt), majd válassza az **Elemek törlése lehetőséget.**

## <a name="enabledisable-private-azure-marketplace"></a>Privát kapcsolat engedélyezése/Azure Marketplace

A Marketplace kezelése oldalon az alábbi szalagcímek egyike jelenik meg, amelyek a Privát előfizetések aktuális Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Megjeleníti az Állapot letiltása szalagcímet.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Megjeleníti az &quot;Állapot engedélyezése&quot; szalagcímet.":::

Szükség szerint engedélyezheti vagy letilthatja Azure Marketplace privát fiókokat.

- Ha le van tiltva, válassza **a Privát piactér engedélyezése lehetőséget** az engedélyezéshez.
- Ha engedélyezve van, a Privát **piactér letiltása lehetőség kiválasztásával** tiltsa le.

## <a name="private-azure-marketplace-notification-center"></a>Privát Azure Marketplace értesítési központ

Az Értesítési központ három típusú értesítésből áll, és lehetővé teszi a Marketplace rendszergazdája számára, hogy az értesítés alapján műveleteket is végretessen:

- Jóváhagyási kérelmek a felhasználóktól a jóváhagyott listán nem található elemekhez (lásd az ajánlatok vagy csomagok hozzáadásának kérését [alább).](#request-to-add-offers-or-plans)
- Új csomagértesítések olyan ajánlatokhoz, amelyek már egy vagy több csomaggal vannak a jóváhagyott listában.
- A jóváhagyott listában szereplő, de a globális listában szereplő elemekről eltávolított tervértesítések Azure Marketplace.

Az értesítési központ elérése:

1. A **bal oldali menüben** válassza az Értesítések lehetőséget.

    [![Megjeleníti az Értesítések menüt.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. További műveletekért válassza a három pont menüt.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Megjeleníti a További beállítások menü eredményeit.":::

1. A csomagkérések esetén a **Kérelmek megjelenítése megnyitja** a jóváhagyási kérelem űrlapját, ahol áttekintheti az adott ajánlatra vonatkozó összes felhasználói kérést.
1. Válassza a **Jóváhagyás vagy** az **Elutasítás lehetőséget.**

    [![A jóváhagyó és elutasító beállításokat jeleníti meg.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Válassza ki a jóváhagyni kívánt tervet a legördülő menüből.
1. Adjon hozzá egy megjegyzést, és válassza a **Küldés lehetőséget.**

## <a name="browsing-private-azure-marketplace"></a>Böngészés a privát Azure Marketplace

Ha a privát Azure Marketplace engedélyezve van, a felhasználók látni fogják, hogy a Marketplace-rendszergazda mely csomagokat hagyta jóvá.

- A zöld **Approved (Jóváhagyva)** értesítés egy jóváhagyott partneri (nem Microsoft) ajánlatot jelez.
- A kék **jóváhagyott** értesítés egy jóváhagyott Microsoft-ajánlatot (beleértve a támogatott Linux-disztribúciókat is) jelez. [](/azure/virtual-machines/linux/endorsed-distros)

A felhasználók szűrni tudnak a jóváhagyott és nem jóváhagyott ajánlatok között:

[![Megjeleníti a szűrési lehetőséget.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Vásárlás vagy üzembe helyezés privát Azure Marketplace

Bár a termékadatok lap felhasználói élménye hasonló a globális Azure Marketplace, három privát Azure Marketplace forgatókönyv van.

- Amikor egy felhasználó kiválaszt egy jóváhagyott tervet, a **Létrehozás** gomb engedélyezve lesz:

    [![Megjeleníti az ajánlat szalagcímét, amely jelzi, hogy a csomag létre lehet hozható.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Ha a termékterv kiválasztása nem jelenik meg a termékadatok oldalon, de a rendszergazda jóváhagyott egy vagy több tervet, egy szalagcímen szerepel, hogy mely csomagokat hagyja jóvá a rendszer, és a **Létrehozás** gomb engedélyezve van:

    [![Megjeleníti az ajánlat szalagcímét, amely azt jelzi, hogy a csomag létre lehet hozható, és megjeleníti az elérhető csomagokat.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Amikor egy felhasználó nem jóváhagyott tervet választ, egy szalagcím nem jóváhagyottként veszi fel a tervet, és a **Létrehozás** gomb le van tiltva. A felhasználó továbbra is kérheti a terv hozzáadását a jóváhagyott listához (lásd a következő szakaszt).

## <a name="request-to-add-offers-or-plans"></a>Ajánlatok vagy csomagok hozzáadásának kérése

Kérheti egy olyan nyilvános ajánlat vagy csomag hozzáadását, amely jelenleg nincs jóváhagyva a Privát Azure Marketplace.

1. Válassza **a Kérelem lehetőséget, hogy** hozzáadja a szalagcímhez a Hozzáférési kérelem űrlap **megnyitásához.**

    [![Megjeleníti a szalagcímet a "Hozzáadási kérelem" hivatkozással.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Megjeleníti az ajánlatok vagy csomagok hozzáférési kérelem űrlapját.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Válassza ki, hogy mely csomagokat adja hozzá a kéréshez **(** Bármely csomag jelzi a Marketplace rendszergazdának, hogy nem előnyben részesíti az ajánlaton belüli csomagokat).

1. Adjon hozzá egy **indoklást,** **és válassza a Kérelem lehetőséget** a kérés elküldését.
  
    [![Megjeleníti az ajánlatok vagy csomagok hozzáférési kérelem űrlapját mintabejegyzésekkel.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Egy függőben lévő kérelemre utaló jel jelenik meg a Hozzáférési kérelem űrlapon, és a **Kérés visszavonása lehetőséggel.**

    [![A jóváhagyott vagy függőben lévő tervek listáját jeleníti meg a Kérések hivatkozással.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> Az elküldés után a jóváhagyási kérelem [](#private-azure-marketplace-notification-center) űrlapja el lesz küldve az Értesítési központba, hogy a Marketplace rendszergazdája áttekintse a kérést, és megteje a szükséges lépéseket.

> [!CAUTION]
> A privát piactérre való jóváhagyás nem jelenti a megoldás beszerzését.

## <a name="frequently-asked-questions-faqs"></a>Gyakori kérdések (GYIK)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Már blokkoljam a Marketplace harmadik féltől származó alkalmazást a Azure Policy. Miben különbözik ez?

A marketplace-en jelenleg kétféleképpen korlátozhatja a külső szolgáltatásokat:

1. Az EA Portalon vagy a Azure Portal tiltsa le a külső szolgáltatásokat, vagy korlátozza az "Ingyenes vagy CSAK BYOL SKUs" korlátozást.

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Bemutatja, hogyan korlátozhatja a szolgáltatások Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Bemutatja, hogyan korlátozhatja a szolgáltatásokat az E A portálon.":::

2. Hozzon létre egy Azure-szabályzatot, amely csak bizonyos virtuális gépeket engedélyez. A házirendek Windows rendszerű virtuális gépekre való kényszerítésének részleteiért lásd: Házirendek alkalmazása Windows rendszerű virtuális gépekre a [Azure Resource Manager.](/azure/virtual-machines/windows/policy)

A Azure Marketplace nagyobb rugalmasságot biztosít bizonyos ajánlatok és csomagok korlátozásában és engedélyezésében. Még azelőtt tájékoztatja a végfelhasználókat a Marketplace-katalógusban való üzembe helyezés rendelkezésre állására, hogy harmadik féltől származó szolgáltatásokat próbálnak üzembe helyezni. A külső szolgáltatások üzembe helyezésének engedélyezése érdekében állítsa a Azure Marketplace On/Enabled (Be/engedélyezve) EA Portal és a Azure Portal.

- A Azure Marketplace a partnermegoldásokat nem csak a virtuális gépekhez lehet társozni.
- A Azure Marketplace a terv szintjén egyesedhet, és beállíthatja a "Jelenlegi és jövőbeli terv" beállítását is.
- A Azure Marketplace előre tájékoztathatja a végfelhasználókat arról, hogy mit lehet és mit nem lehet üzembe helyezni.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Mi a különbség a privát ajánlat és a privát Azure Marketplace?

A **privát ajánlatokkal** a közzétevők olyan csomagokat hozhatnak létre, amelyek csak a megcélzott ügyfelek számára láthatók. Ez lehetővé teszi, hogy privát módon osszanak meg testreszabott megoldásokat egyeztetett díjszabással, privát feltételekkel és speciális konfigurációval. Részletekért lásd: [Privát ajánlatok a kereskedelmi piactéren.](/azure/marketplace/private-offers)

**A Azure Marketplace** a Azure Portal lehetővé teszi a rendszergazdák számára, hogy előzetesen jóváhagyják, mely külső megoldásokat telepítheti a felhasználók. A privát Azure Marketplace a felhasználók a megfelelő ajánlatok megkeresés, Azure Marketplace vásárlása és üzembe helyezése által élvezhetik a felhasználók által nyújtott előnyöket. Az előfizetés-alapú privát ajánlatok privát Marketplace-en való kezeléséhez a Marketplace-rendszergazdának legalább olvasási szerepkört kell látnia az adott előfizetésben.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Hozzáadtam egy privát ajánlatot a privát Azure Marketplace, miért nem jelenik meg a Piactér kezelése lapon?

Az előfizetés-alapú privát ajánlatok csak a privát ajánlat beállításaiban felsorolt előfizetések számára láthatók. A privát ajánlat megtekintéséhez győződjön meg arról, hogy a globális előfizetés szűrője az összes előfizetést mutatja.

[![Megjeleníti a privát piactér szűrőt.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Tartalmazhatunk egyéni rendszerképeket a Private Azure Marketplace?

Nem. A Azure Marketplace lehetővé teszi, hogy bármely rendszergazda külső megoldásokat kezeljen és kezeljen a globális Azure Marketplace. Mivel az egyéni rendszerképek nincsenek globálisan Azure Marketplace, a rendszergazda nem választhatja ki és nem választhatja ki az egyéni rendszerképeket. Ha egyéni rendszerképeket szeretne megosztani, használja a [Shared Image Gallery.](/azure/virtual-machines/shared-image-galleries)

1. Részletes útmutató: Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. Képdefiníció létrehozása egy SIG-fájlban. Az ügyfélnek az **Operációs rendszer állapota** mezőben az Általánosított lehetőséget kell választania. ([PARANCSSORI FELÜLET,](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Felügyelt rendszerkép behozása a Shared Image Gallery ([parancssori felület](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. A SIG virtuálisgép-rendszerképek egy előfizetésben találhatók. Ha más előfizetések számára is elérhetővé tenni, használjon alkalmazásregisztrációt[(CLI,](/azure/virtual-machines/linux/share-images-across-tenants) [PowerShell).](/azure/virtual-machines/windows/share-images-across-tenants)

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Miért látok egyes  alapértelmezés szerint jóváhagyott ajánlatokat annak ellenére, hogy a közzétevő nem a Microsoft?

A Microsoft támogatja a Linux és a nyílt forráskódú technológiákat az Azure-ban. [A támogatott Linux-disztribúciók](/azure/virtual-machines/linux/endorsed-distros) támogatottak az Azure-ban, és az ár a virtuális gépekbe van integrálva. Mivel az Azure Linux-ügynök már előre telepítve van a Azure Marketplace, microsoftos ajánlatként kezeli. Mivel a Microsoft-ajánlatok alapértelmezés szerint jóvá vannak hagyva, a támogatott Linux-disztribúciók nem kezelhetők privát Azure Marketplace és alapértelmezés szerint jóvá vannak hagyva.

## <a name="contact-support"></a>Kapcsolatfelvétel a támogatási szolgáltatással

- A Azure Marketplace támogatásért látogasson el a [Microsoft Q&A webhelyre.](/answers/products/)