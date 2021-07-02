---
title: Privát fiók létrehozása Azure Marketplace és kezelése a Azure Portal
description: Ismerje meg, hogyan lehet privát Azure Marketplace (előzetes verzió) létrehozni és Azure Portal. A Azure Marketplace (előzetes verzió) lehetővé teszi a rendszergazdák számára, hogy szabályozzák, mely külső megoldásokat használhatják a felhasználók.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173700"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="0283f-104">Privát fiók létrehozása Azure Marketplace és kezelése a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="0283f-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="0283f-105">A Azure Marketplace lehetővé teszi a rendszergazdák számára, hogy szabályozzák, mely külső megoldásokat használhatják a felhasználók.</span><span class="sxs-lookup"><span data-stu-id="0283f-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="0283f-106">Ezt úgy teszi lehetővé, hogy a felhasználó csak a rendszergazda által jóváhagyott ajánlatokat telepítsen, és megfeleljen a vállalat szabályzatának.</span><span class="sxs-lookup"><span data-stu-id="0283f-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="0283f-107">A Private Azure Marketplace lehetővé teszi, hogy a felhasználók az online áruházban megfelelő ajánlatokat keressenek a vásárláshoz és az üzembe helyezéshez.</span><span class="sxs-lookup"><span data-stu-id="0283f-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="0283f-108">Marketplace-rendszergazdaként (hozzárendelt szerepkör) egy letiltott és üres privát tárolóval fog kezdeni, ahol hozzáadhatja a jóváhagyott ajánlatokat és csomagokat.</span><span class="sxs-lookup"><span data-stu-id="0283f-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="0283f-109">Ez a cikk bemutatja, hogyan rendelheti hozzá a szükséges szerepkört, hogyan hozhat létre privát tárolót, hogyan kezelheti az elemeket, hogyan hagyja jóvá a felhasználói kéréseket, és hogyan engedélyezheti a Azure Marketplace privát tárolókat a felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="0283f-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="0283f-110">A privát Azure Marketplace bérlői szinten található, így a bérlő összes felhasználója ugyanazt az összeért listát fogja látni.</span><span class="sxs-lookup"><span data-stu-id="0283f-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="0283f-111">Minden Microsoft-megoldás (beleértve [a támogatott Linux-disztribúciókat](/azure/virtual-machines/linux/endorsed-distros)is) automatikusan hozzáadódik a privát Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0283f-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="0283f-112">A Marketplace rendszergazdai szerepkör hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="0283f-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="0283f-113">A bérlői globális rendszergazda **Marketplace** rendszergazdai szerepkört kell hozzárendelnie ahhoz a privát Azure Marketplace rendszergazdához, aki a privát tárolót fogja kezelni.</span><span class="sxs-lookup"><span data-stu-id="0283f-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="0283f-114">A privát Azure Marketplace kezeléséhez való hozzáférés csak a Marketplace rendszergazdai szerepkörével társított rendszergazdák számára érhető el.</span><span class="sxs-lookup"><span data-stu-id="0283f-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="0283f-115">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="0283f-115">Prerequisites</span></span>

<span data-ttu-id="0283f-116">Ezek az előfeltételek ahhoz szükségesek, hogy a Marketplace-rendszergazdai szerepkört hozzárendelje egy felhasználóhoz a bérlői hatókörben:</span><span class="sxs-lookup"><span data-stu-id="0283f-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="0283f-117">Hozzáféréssel rendelkezik **egy** globális rendszergazda felhasználóhoz.</span><span class="sxs-lookup"><span data-stu-id="0283f-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="0283f-118">A bérlő legalább egy előfizetéssel rendelkezik (bármilyen típusú lehet).</span><span class="sxs-lookup"><span data-stu-id="0283f-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="0283f-119">A globális rendszergazda felhasználóhoz a **választott** előfizetés közreműködői vagy magasabb szintű szerepköre van hozzárendelve.</span><span class="sxs-lookup"><span data-stu-id="0283f-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="0283f-120">A Marketplace rendszergazdai szerepkör hozzárendelése hozzáférés-vezérléssel (IAM)</span><span class="sxs-lookup"><span data-stu-id="0283f-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="0283f-121">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0283f-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="0283f-122">Válassza a **Minden szolgáltatás,** majd a **Marketplace lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0283f-122">Select **All services** and then **Marketplace**.</span></span>

1. <span data-ttu-id="0283f-123">A **bal oldali menüben** válassza a Privát piactér lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0283f-123">Select **Private Marketplace** from the menu on the left.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Megjeleníti a privát Marketplace menüpontot a Marketplace bal oldalán.":::

1. <span data-ttu-id="0283f-125">Válassza **a Hozzáférés-vezérlés (IAM) lehetőséget** a Marketplace rendszergazdai szerepkörének hozzárendeléshez.</span><span class="sxs-lookup"><span data-stu-id="0283f-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Megjeleníti az I A M hozzáférés-vezérlés képernyőjét.":::

1. <span data-ttu-id="0283f-127">Válassza a **+ Hozzáadás** > **Szerepkör-hozzárendelés hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0283f-127">Select **+ Add** > **Add role assignment**.</span></span>

1. <span data-ttu-id="0283f-128">A Szerepkör **alatt** válassza a **Marketplace-rendszergazda lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0283f-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Megjeleníti a Szerepkör-hozzárendelés menüt.":::

1. <span data-ttu-id="0283f-130">Válassza ki a kívánt felhasználót a legördülő listából, majd válassza a **Kész lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0283f-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="0283f-131">A Marketplace rendszergazdai szerepkör hozzárendelése a PowerShell használatával</span><span class="sxs-lookup"><span data-stu-id="0283f-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="0283f-132">Az alábbi PowerShell-szkript használatával rendelje hozzá a Marketplace rendszergazdai szerepkörét; ehhez a következő paraméterekre van szükség:</span><span class="sxs-lookup"><span data-stu-id="0283f-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="0283f-133">**TenantId (Bérlőazonosító):** A hatókörhöz tartozó bérlő azonosítója (a Marketplace rendszergazdai szerepkör hozzárendelhető a bérlői hatókörhöz).</span><span class="sxs-lookup"><span data-stu-id="0283f-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="0283f-134">**SubscriptionId (Előfizetés-azonosító):** Egy előfizetés, amelynek a globális rendszergazda Közreműködő **szerepköre** vagy magasabb szintű hozzárendelt szerepköre van.</span><span class="sxs-lookup"><span data-stu-id="0283f-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="0283f-135">**GlobalAdminUsername:** A globális rendszergazda felhasználóneve.</span><span class="sxs-lookup"><span data-stu-id="0283f-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="0283f-136">**UsernameToAssignRoleFor:** A felhasználónév, amelyhez a Marketplace rendszergazdai szerepkör hozzá lesz rendelve.</span><span class="sxs-lookup"><span data-stu-id="0283f-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="0283f-137">A bérlőbe meghívott vendégfelhasználók esetén akár 48 órát is igénybe vehet, amíg a fiókjuk elérhetővé válik a Marketplace-rendszergazdai szerepkör hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="0283f-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="0283f-138">További információ: [Egy B2B Azure Active Directory felhasználó tulajdonságai.](/azure/active-directory/b2b/user-properties)</span><span class="sxs-lookup"><span data-stu-id="0283f-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="0283f-139">További információ az Az.Portal PowerShell-modulban található parancsmagokkal kapcsolatban: [Microsoft Azure PowerShell: Portal Dashboard parancsmagok.](/powershell/module/az.portal/)</span><span class="sxs-lookup"><span data-stu-id="0283f-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="0283f-140">Privát Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0283f-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="0283f-141">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0283f-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="0283f-142">Válassza a **Minden szolgáltatás,** majd a **Marketplace lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0283f-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Megjeleníti Azure Portal fő ablakát.":::

3. <span data-ttu-id="0283f-144">A **bal oldali menüben** válassza a Privát piactér lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0283f-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="0283f-145">Válassza **Első lépések** lehetőséget a Privát Azure Marketplace létrehozásához (ezt csak egyszer kell megtennie).</span><span class="sxs-lookup"><span data-stu-id="0283f-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Bemutatja, hogyan választhatja ki Első lépések &quot;Azure Portal&quot; főablakban.":::

    <span data-ttu-id="0283f-147">Ha a Azure Marketplace már létezik privát előfizetés, a **Manage Marketplace (Piactér** kezelése) lehetőség alapértelmezés szerint ki van választva.</span><span class="sxs-lookup"><span data-stu-id="0283f-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="0283f-148">Ha elkészült, egy üres és letiltott Privát Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0283f-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Megjeleníti az üres Privát Azure Marketplace képernyőt.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="0283f-150">Elemek hozzáadása katalógusból</span><span class="sxs-lookup"><span data-stu-id="0283f-150">Add items from gallery</span></span>

<span data-ttu-id="0283f-151">Az elem egy ajánlat és egy csomag kombinációja.</span><span class="sxs-lookup"><span data-stu-id="0283f-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="0283f-152">A Marketplace kezelése oldalon kereshet és adhat hozzá elemeket.</span><span class="sxs-lookup"><span data-stu-id="0283f-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="0283f-153">Válassza **az Elemek hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0283f-153">Select **Add items**.</span></span>

2. <span data-ttu-id="0283f-154">Tallózással **keresse** meg a katalógust, vagy a keresőmezővel keresse meg a kívánt elemet.</span><span class="sxs-lookup"><span data-stu-id="0283f-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Bemutatja, hogyan tallózhat a katalógusban vagy használhatja a keresőmezőt.":::

3. <span data-ttu-id="0283f-156">Új ajánlat hozzáadásakor alapértelmezés szerint az összes jelenlegi csomag fel lesz sorolva a jóváhagyottak listájára.</span><span class="sxs-lookup"><span data-stu-id="0283f-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="0283f-157">Ha a kiválasztott elemek hozzáadása előtt módosítani szeretné a csomag kiválasztását, válassza ki a legördülő menüt az ajánlat csempéjéről, és frissítse a szükséges csomagokat.</span><span class="sxs-lookup"><span data-stu-id="0283f-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer's tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Bemutatja, hogyan frissítheti a szükséges csomagokat.":::

4. <span data-ttu-id="0283f-159">A **kiválasztás után** válassza a bal alsó sarokban található Kész lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0283f-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="0283f-160">**Az Elemek hozzáadása** a Marketplace-hez csak a nem Microsoft-ajánlatokhoz érhető el.</span><span class="sxs-lookup"><span data-stu-id="0283f-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="0283f-161">A Microsoft-megoldások (beleértve a támogatott Linux-disztribúciókat is) alapértelmezés szerint jóváhagyottként lesznek megjelölve, és nem kezelhetők a Privát Piactéren. [](/azure/virtual-machines/linux/endorsed-distros)</span><span class="sxs-lookup"><span data-stu-id="0283f-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as "Approved by default" and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="0283f-162">Elemtervek szerkesztése</span><span class="sxs-lookup"><span data-stu-id="0283f-162">Edit item's plans</span></span>

<span data-ttu-id="0283f-163">Egy elem csomagját a Marketplace kezelése oldalon szerkesztheti.</span><span class="sxs-lookup"><span data-stu-id="0283f-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="0283f-164">A **Plans (Csomagok)** oszlopban tekintse át az elemhez elérhető csomagokat a legördülő menüből.</span><span class="sxs-lookup"><span data-stu-id="0283f-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>

2. <span data-ttu-id="0283f-165">Jelölje be vagy törölje a jelölőnégyzeteket a felhasználók számára elérhetővé tenni kívánt csomagok kiválasztásához.</span><span class="sxs-lookup"><span data-stu-id="0283f-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Bemutatja, hogyan jelölheti be vagy ürítheti ki a kötelező elem jelölőnégyzetét.":::

   > [!NOTE]
   > <span data-ttu-id="0283f-167">Minden ajánlathoz legalább egy kiválasztott csomag szükséges a frissítés következtéhez.</span><span class="sxs-lookup"><span data-stu-id="0283f-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="0283f-168">Egy ajánlathoz kapcsolódó összes csomag eltávolításához törölje a teljes ajánlatot (lásd a következő szakaszt).</span><span class="sxs-lookup"><span data-stu-id="0283f-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="0283f-169">Ajánlatok törlése</span><span class="sxs-lookup"><span data-stu-id="0283f-169">Delete offers</span></span>

<span data-ttu-id="0283f-170">A Marketplace kezelése oldalon jelölje be az ajánlat neve melletti jelölőnégyzetet (lásd a fenti képernyőt), majd válassza az **Elemek törlése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0283f-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="0283f-171">Privát kapcsolat engedélyezése/Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0283f-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="0283f-172">A Marketplace kezelése oldalon az alábbi szalagcímek egyike jelenik meg, amelyek a Privát előfizetések aktuális Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="0283f-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Megjeleníti az Állapot letiltása szalagcímet.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Megjeleníti az &quot;Állapot engedélyezése&quot; szalagcímet.":::

<span data-ttu-id="0283f-175">Szükség szerint engedélyezheti vagy letilthatja Azure Marketplace privát fiókokat.</span><span class="sxs-lookup"><span data-stu-id="0283f-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="0283f-176">Ha le van tiltva, válassza **a Privát piactér engedélyezése lehetőséget** az engedélyezéshez.</span><span class="sxs-lookup"><span data-stu-id="0283f-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="0283f-177">Ha engedélyezve van, a Privát **piactér letiltása lehetőség kiválasztásával** tiltsa le.</span><span class="sxs-lookup"><span data-stu-id="0283f-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="0283f-178">Privát Azure Marketplace értesítési központ</span><span class="sxs-lookup"><span data-stu-id="0283f-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="0283f-179">Az Értesítési központ háromféle értesítésből áll, és lehetővé teszi a Marketplace rendszergazdája számára, hogy az értesítés alapján műveleteket is végretessen:</span><span class="sxs-lookup"><span data-stu-id="0283f-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="0283f-180">Jóváhagyási kérelmek a felhasználóktól a jóváhagyott listán nem található elemekhez (lásd az ajánlatok vagy csomagok hozzáadásának kérését [alább).](#request-to-add-offers-or-plans)</span><span class="sxs-lookup"><span data-stu-id="0283f-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="0283f-181">Új csomagértesítések olyan ajánlatokhoz, amelyek már egy vagy több csomaggal vannak a jóváhagyott listában.</span><span class="sxs-lookup"><span data-stu-id="0283f-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="0283f-182">A jóváhagyott listában szereplő, de a globális listában szereplő elemekről eltávolított tervértesítések Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0283f-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="0283f-183">Az értesítési központ elérése:</span><span class="sxs-lookup"><span data-stu-id="0283f-183">To access the notification center:</span></span>

1. <span data-ttu-id="0283f-184">A **bal oldali menüben** válassza az Értesítések lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0283f-184">Select **Notifications** from the left-side menu.</span></span>

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Megjeleníti az Értesítések menüt.":::

1. <span data-ttu-id="0283f-186">További műveletekért válassza a három pont menüt.</span><span class="sxs-lookup"><span data-stu-id="0283f-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Megjeleníti a További beállítások menü eredményeit.":::

1. <span data-ttu-id="0283f-188">A csomagkérések esetén a **Kérelmek megjelenítése megnyitja** a jóváhagyási kérelem űrlapját, ahol áttekintheti az adott ajánlatra vonatkozó összes felhasználói kérést.</span><span class="sxs-lookup"><span data-stu-id="0283f-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="0283f-189">Válassza a **Jóváhagyás vagy** az **Elutasítás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0283f-189">Select **Approve** or **Reject**.</span></span>

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="A jóváhagyó és elutasító beállításokat jeleníti meg.":::

1. <span data-ttu-id="0283f-191">Válassza ki a jóváhagyni kívánt tervet a legördülő menüből.</span><span class="sxs-lookup"><span data-stu-id="0283f-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="0283f-192">Megjegyzés hozzáadása után válassza a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0283f-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="0283f-193">Böngészés a privát Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0283f-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="0283f-194">Ha a privát Azure Marketplace engedélyezve van, a felhasználók látni fogják, hogy a Marketplace-rendszergazda mely csomagokat hagyta jóvá.</span><span class="sxs-lookup"><span data-stu-id="0283f-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="0283f-195">A zöld **Approved (Jóváhagyva)** értesítés egy jóváhagyott Partneri (nem Microsoft) ajánlatot jelez.</span><span class="sxs-lookup"><span data-stu-id="0283f-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="0283f-196">A kék **jóváhagyott** értesítés egy jóváhagyott Microsoft-ajánlatot (beleértve a támogatott Linux-disztribúciókat is) jelez. [](/azure/virtual-machines/linux/endorsed-distros)</span><span class="sxs-lookup"><span data-stu-id="0283f-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="0283f-197">A felhasználók szűrni tudnak a jóváhagyott és nem jóváhagyott ajánlatok között:</span><span class="sxs-lookup"><span data-stu-id="0283f-197">Users can filter between offers that are and are not approved:</span></span>

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Megjeleníti a szűrési lehetőséget.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="0283f-199">Vásárlás vagy üzembe helyezés privát Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0283f-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="0283f-200">Bár a termékadatokat tartalmazó oldal felhasználói élménye hasonló a globális Azure Marketplace, három privát Azure Marketplace forgatókönyv van.</span><span class="sxs-lookup"><span data-stu-id="0283f-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="0283f-201">Amikor egy felhasználó kiválaszt egy jóváhagyott tervet, a **Létrehozás** gomb engedélyezve lesz:</span><span class="sxs-lookup"><span data-stu-id="0283f-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Megjeleníti az ajánlat szalagcímét, amely jelzi, hogy létre lehet hozható csomag.":::

- <span data-ttu-id="0283f-203">Ha a termékterv kiválasztása nem jelenik meg a termékadatok oldalon, de a rendszergazda jóváhagyott egy vagy több tervet, egy szalagcímen szerepel, hogy mely csomagokat hagyja jóvá a rendszer, és a **Létrehozás** gomb engedélyezve van:</span><span class="sxs-lookup"><span data-stu-id="0283f-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Megjeleníti az ajánlat szalagcímét, amely azt jelzi, hogy a csomag létre lehet hozható, és megjeleníti az elérhető csomagokat.":::

- <span data-ttu-id="0283f-205">Amikor egy felhasználó nem jóváhagyott tervet választ, egy szalagcím nem jóváhagyottként veszi fel a tervet, és a **Létrehozás** gomb le van tiltva.</span><span class="sxs-lookup"><span data-stu-id="0283f-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="0283f-206">A felhasználó továbbra is kérheti a terv hozzáadását a jóváhagyott listához (lásd a következő szakaszt).</span><span class="sxs-lookup"><span data-stu-id="0283f-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="0283f-207">Ajánlatok vagy csomagok hozzáadásának kérése</span><span class="sxs-lookup"><span data-stu-id="0283f-207">Request to add offers or plans</span></span>

<span data-ttu-id="0283f-208">Kérheti egy olyan nyilvános ajánlat vagy csomag hozzáadását, amely jelenleg nincs jóváhagyva a Privát Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0283f-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="0283f-209">Válassza **a Kérés lehetőséget a** szalagcímen a Hozzáférési kérelem űrlap **megnyitásához.**</span><span class="sxs-lookup"><span data-stu-id="0283f-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Megjeleníti a szalagcímet a &quot;Hozzáadási kérelem&quot; hivatkozással.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Megjeleníti az ajánlatok vagy csomagok hozzáférési kérelem űrlapját.":::

1. <span data-ttu-id="0283f-212">Válassza ki, hogy mely csomagokat adja hozzá a kéréshez **(** Bármely csomag jelzi a Marketplace rendszergazdának, hogy nem előnyben részesíti az ajánlaton belüli csomagokat).</span><span class="sxs-lookup"><span data-stu-id="0283f-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="0283f-213">Adjon hozzá egy **indoklást,** **és válassza a Kérelem lehetőséget** a kérés elküldését.</span><span class="sxs-lookup"><span data-stu-id="0283f-213">Add a **Justification** and select **Request** to submit your request.</span></span>

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Megjeleníti az ajánlatok vagy csomagok hozzáférési kérelem űrlapját mintabejegyzésekkel.":::

1. <span data-ttu-id="0283f-215">Egy függőben lévő kérelemre utaló jel jelenik meg a Hozzáférési kérelem űrlapon, és a **Kérelem visszavonása lehetőséggel.**</span><span class="sxs-lookup"><span data-stu-id="0283f-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="A jóváhagyott vagy függőben lévő tervek listáját jeleníti meg a Kérések hivatkozással.":::

> [!NOTE]
> <span data-ttu-id="0283f-217">Az elküldés után a jóváhagyási kérelem [](#private-azure-marketplace-notification-center) űrlapja el lesz küldve az Értesítési központba, hogy a Marketplace rendszergazdája áttekintse a kérést, és megteje a szükséges lépéseket.</span><span class="sxs-lookup"><span data-stu-id="0283f-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="0283f-218">A privát piactérre való jóváhagyás nem jelenti a megoldás beszerzését.</span><span class="sxs-lookup"><span data-stu-id="0283f-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="0283f-219">Gyakori kérdések (GYIK)</span><span class="sxs-lookup"><span data-stu-id="0283f-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="0283f-220">Már blokkoljam a Marketplace harmadik féltől származó alkalmazást a Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="0283f-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="0283f-221">Miben különbözik ez?</span><span class="sxs-lookup"><span data-stu-id="0283f-221">How is this different?</span></span>

<span data-ttu-id="0283f-222">A marketplace-en jelenleg kétféleképpen korlátozhatja a külső szolgáltatásokat:</span><span class="sxs-lookup"><span data-stu-id="0283f-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="0283f-223">Az EA Portalon vagy a Azure Portal tiltsa le a külső szolgáltatásokat, vagy korlátozza az "Ingyenes vagy CSAK BYOL SKUs" korlátozást.</span><span class="sxs-lookup"><span data-stu-id="0283f-223">Through EA portal or the Azure portal, disable third-party services or restrict to "Free or BYOL SKUs only".</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Bemutatja, hogyan korlátozhatja a szolgáltatások Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Bemutatja, hogyan korlátozhatja a szolgáltatásokat az E A portálon.":::

2. <span data-ttu-id="0283f-226">Hozzon létre egy Azure-szabályzatot, amely csak bizonyos virtuális gépeket engedélyez.</span><span class="sxs-lookup"><span data-stu-id="0283f-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="0283f-227">A szabályzatok virtuális gépekre való kényszerítésének Windows részleteiért lásd: Szabályzatok alkalmazása virtuális Windows virtuális gépekre [Azure Resource Manager.](/azure/virtual-machines/windows/policy)</span><span class="sxs-lookup"><span data-stu-id="0283f-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="0283f-228">A Azure Marketplace nagyobb rugalmasságot tesz lehetővé bizonyos ajánlatok és csomagok korlátozásában és engedélyezésében.</span><span class="sxs-lookup"><span data-stu-id="0283f-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="0283f-229">Még azelőtt tájékoztatja a végfelhasználókat a Marketplace-katalógusban való üzembe helyezés rendelkezésre állására, hogy harmadik féltől származó szolgáltatásokat próbálnak üzembe helyezni.</span><span class="sxs-lookup"><span data-stu-id="0283f-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="0283f-230">A külső szolgáltatások üzembe helyezésének engedélyezése érdekében állítsa a Azure Marketplace On/Enabled (Be/engedélyezve) EA Portal és a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="0283f-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="0283f-231">A Azure Marketplace a partnermegoldásokat nem csak a virtuális gépekhez lehet társozni.</span><span class="sxs-lookup"><span data-stu-id="0283f-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="0283f-232">A Azure Marketplace a terv szintjén egyesedhet, és beállíthatja az "Aktuális és jövőbeli terv" beállítását is.</span><span class="sxs-lookup"><span data-stu-id="0283f-232">Private Azure Marketplace can curate at the plan level and can also set "Current and future plan".</span></span>
- <span data-ttu-id="0283f-233">A Azure Marketplace előre tájékoztathatja a végfelhasználókat arról, hogy mit lehet és mit nem lehet üzembe helyezni.</span><span class="sxs-lookup"><span data-stu-id="0283f-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="0283f-234">Mi a különbség a privát ajánlat és a privát Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="0283f-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="0283f-235">A **privát ajánlatokkal** a közzétevők olyan csomagokat hozhatnak létre, amelyek csak a megcélzott ügyfelek számára láthatók.</span><span class="sxs-lookup"><span data-stu-id="0283f-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="0283f-236">Ez lehetővé teszi, hogy privát módon osszanak meg testreszabott megoldásokat egyeztetett díjszabással, privát feltételekkel és speciális konfigurációval.</span><span class="sxs-lookup"><span data-stu-id="0283f-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="0283f-237">Részletekért lásd: [Privát ajánlatok a kereskedelmi piactéren.](/azure/marketplace/private-offers)</span><span class="sxs-lookup"><span data-stu-id="0283f-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="0283f-238">**A Azure Marketplace** a Azure Portal lehetővé teszi a rendszergazdák számára, hogy előzetesen jóváhagyják, mely külső megoldásokat helyezhetik üzembe a felhasználók.</span><span class="sxs-lookup"><span data-stu-id="0283f-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="0283f-239">A privát Azure Marketplace a felhasználók a megfelelő ajánlatok megkeresés, Azure Marketplace vásárlása és üzembe helyezése által élvezhetik a felhasználók által nyújtott előnyöket.</span><span class="sxs-lookup"><span data-stu-id="0283f-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="0283f-240">Az előfizetés-alapú privát ajánlatok privát Marketplace-en való kezeléséhez a Marketplace-rendszergazdának legalább olvasási szerepkört kell látnia az adott előfizetésben.</span><span class="sxs-lookup"><span data-stu-id="0283f-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of "read" role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="0283f-241">Hozzáadtam egy privát ajánlatot a privát Azure Marketplace, miért nem jelenik meg a Piactér kezelése lapon?</span><span class="sxs-lookup"><span data-stu-id="0283f-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="0283f-242">Az előfizetés-alapú privát ajánlatok csak a privát ajánlat beállításaiban felsorolt előfizetések számára láthatók.</span><span class="sxs-lookup"><span data-stu-id="0283f-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="0283f-243">A privát ajánlat megtekintéséhez győződjön meg arról, hogy a globális előfizetés szűrője az összes előfizetést mutatja.</span><span class="sxs-lookup"><span data-stu-id="0283f-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Megjeleníti a privát piactér szűrőt.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="0283f-245">Tartalmazhatunk egyéni rendszerképeket a Private Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="0283f-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="0283f-246">Nem.</span><span class="sxs-lookup"><span data-stu-id="0283f-246">No.</span></span> <span data-ttu-id="0283f-247">A Azure Marketplace lehetővé teszi, hogy a rendszergazdák külső megoldásokat kezeljenek és kezeljenek a globális Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0283f-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="0283f-248">Mivel az egyéni rendszerképek nincsenek globálisan Azure Marketplace, a rendszergazda nem választhatja ki és nem választhatja ki az egyéni rendszerképeket.</span><span class="sxs-lookup"><span data-stu-id="0283f-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="0283f-249">Ha egyéni rendszerképeket szeretne megosztani, használja a [Shared Image Gallery.](/azure/virtual-machines/shared-image-galleries)</span><span class="sxs-lookup"><span data-stu-id="0283f-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="0283f-250">Részletes útmutató: Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="0283f-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="0283f-251">Képdefiníció létrehozása egy SIG-fájlban.</span><span class="sxs-lookup"><span data-stu-id="0283f-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="0283f-252">Az ügyfélnek az **Operációs rendszer állapota** mezőben az Általánosított lehetőséget kell választania.</span><span class="sxs-lookup"><span data-stu-id="0283f-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="0283f-253">([PARANCSSORI FELÜLET,](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="0283f-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="0283f-254">Felügyelt rendszerképet a Shared Image Gallery ([parancssori felület](/azure/virtual-machines/image-version-managed-image-cli), PowerShell ) [használatával.](/azure/virtual-machines/image-version-managed-image-powershell)</span><span class="sxs-lookup"><span data-stu-id="0283f-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="0283f-255">A SIG virtuálisgép-rendszerképek egy előfizetésben találhatók.</span><span class="sxs-lookup"><span data-stu-id="0283f-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="0283f-256">Ha más előfizetések számára is elérhetővé tenni, használjon alkalmazásregisztrációt[(CLI,](/azure/virtual-machines/linux/share-images-across-tenants) [PowerShell).](/azure/virtual-machines/windows/share-images-across-tenants)</span><span class="sxs-lookup"><span data-stu-id="0283f-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="0283f-257">Miért látok néhány  alapértelmezés szerint jóváhagyott ajánlatot annak ellenére, hogy a közzétevő nem a Microsoft?</span><span class="sxs-lookup"><span data-stu-id="0283f-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="0283f-258">A Microsoft támogatja a Linux és a nyílt forráskódú technológiákat az Azure-ban.</span><span class="sxs-lookup"><span data-stu-id="0283f-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="0283f-259">[A támogatott Linux-disztribúciók](/azure/virtual-machines/linux/endorsed-distros) támogatottak az Azure-ban, és az ár a virtuális gépekbe van integrálva.</span><span class="sxs-lookup"><span data-stu-id="0283f-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="0283f-260">Mivel az Azure Linux-ügynök már előre telepítve van a Azure Marketplace, microsoftos ajánlatként kezeli.</span><span class="sxs-lookup"><span data-stu-id="0283f-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="0283f-261">Mivel a Microsoft-ajánlatok alapértelmezés szerint jóvá vannak hagyva, a támogatott Linux-disztribúciók nem kezelhetők privát Azure Marketplace és alapértelmezés szerint jóvá vannak hagyva.</span><span class="sxs-lookup"><span data-stu-id="0283f-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="0283f-262">Kapcsolatfelvétel a támogatási szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="0283f-262">Contact support</span></span>

- <span data-ttu-id="0283f-263">A Azure Marketplace támogatásért látogasson el a [Microsoft Q&A webhelyre.](/answers/products/)</span><span class="sxs-lookup"><span data-stu-id="0283f-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>