---
title: Privát Azure Marketplace létrehozása és kezelése a Azure Portal
description: Ismerje meg, hogyan hozhat létre és kezelhet privát Azure Marketplace-t (előzetes verzió) a Azure Portal. A privát Azure Marketplace (előzetes verzió) lehetővé teszi, hogy a rendszergazdák szabályozzák, hogy a felhasználók mely harmadik féltől származó megoldásokat használhatják.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 73b9137728fba93704d9b0cb2bc93a3f6498bd90
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "101757069"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="7e0ff-104">Privát Azure Marketplace létrehozása és kezelése a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="7e0ff-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="7e0ff-105">A privát Azure piactér lehetővé teszi, hogy a rendszergazdák szabályozzák, hogy a felhasználók mely harmadik féltől származó megoldásokat használhatják.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="7e0ff-106">Ez a beállítás lehetővé teszi, hogy a felhasználó csak a rendszergazda által jóváhagyott ajánlatokat telepítsen, és megfeleljen a vállalat szabályzatának.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="7e0ff-107">A privát Azure piactéren a felhasználók megkereshetik és üzembe helyezhetik a megfelelő ajánlatokat az online áruházban.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="7e0ff-108">Piactéri rendszergazdaként (hozzárendelt szerepkör) egy letiltott és üres privát tárolóval kell kezdenie, ahol a jóváhagyott ajánlatokat és csomagokat is felveheti.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="7e0ff-109">Ez a cikk a szükséges szerepkör hozzárendelését, a privát tárolók létrehozását, az elemek kezelését, a felhasználói kérések jóváhagyását és a saját Azure Marketplace engedélyezését mutatja be a felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="7e0ff-110">A privát Azure piactér bérlői szinten található, így a bérlő összes felhasználója ugyanazokat a kurátori listát fogja látni.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="7e0ff-111">Az összes Microsoft-megoldás (beleértve a [támogatott Linux-disztribúciókat](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)is) automatikusan hozzá lesz adva a privát Azure Marketplace-hez.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-111">All Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="7e0ff-112">A piactér rendszergazdai szerepkörének kiosztása</span><span class="sxs-lookup"><span data-stu-id="7e0ff-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="7e0ff-113">A bérlői globális rendszergazdának hozzá kell rendelnie a **piactér rendszergazdai** szerepkörét a privát Azure Marketplace-rendszergazda számára, aki felügyelni fogja a saját tárolót.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="7e0ff-114">Az Azure Marketplace-en való hozzáférés csak a piactér rendszergazdai szerepkörrel rendelkező rendszergazdák számára érhető el.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="7e0ff-115">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="7e0ff-115">Prerequisites</span></span>

<span data-ttu-id="7e0ff-116">Ezek az előfeltételek akkor szükségesek, ha a piactér rendszergazdai szerepkört a bérlői hatókörben lévő felhasználóhoz rendeli hozzá:</span><span class="sxs-lookup"><span data-stu-id="7e0ff-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="7e0ff-117">**Globális rendszergazda** felhasználóhoz férhet hozzá.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="7e0ff-118">A bérlőnek legalább egy előfizetése van (bármilyen típus lehet).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="7e0ff-119">A kiválasztott előfizetéshez a globális rendszergazda felhasználó hozzá van rendelve a **közreműködő** szerepkörhöz vagy magasabbhoz.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="7e0ff-120">A piactér rendszergazdai szerepkörének kiosztása hozzáférés-vezérléssel (IAM)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="7e0ff-121">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="7e0ff-122">Válassza **a minden szolgáltatás** , majd a **piactér** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="7e0ff-123">Válassza a **privát piactér** lehetőséget a bal oldali menüben.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="7e0ff-124">[![Megjeleníti a piactér bal oldalán található privát piactér menüpontot.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="7e0ff-125">A piactér rendszergazdai szerepkörének hozzárendeléséhez válassza a **hozzáférés-vezérlés (iam)** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Megjeleníti az I M hozzáférés-vezérlési képernyőt.":::

1. <span data-ttu-id="7e0ff-127">Válassza a **+ Hozzáadás** > **Szerepkör-hozzárendelés hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="7e0ff-128">A **szerepkör** területen válassza a **piactér rendszergazdája** elemet.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="A szerepkör-hozzárendelés menüt jeleníti meg.":::

1. <span data-ttu-id="7e0ff-130">Válassza ki a kívánt felhasználót a legördülő listából, majd válassza a **kész** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="7e0ff-131">A piactér rendszergazdai szerepkörének kiosztása a PowerShell-lel</span><span class="sxs-lookup"><span data-stu-id="7e0ff-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="7e0ff-132">A piactér rendszergazdai szerepkörének hozzárendeléséhez használja a következő PowerShell-parancsfájlt: Ehhez a következő paramétereket kell megadni:</span><span class="sxs-lookup"><span data-stu-id="7e0ff-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="7e0ff-133">**TenantId:** A hatókörben lévő bérlő azonosítója (a piactér rendszergazdai szerepköre a bérlői hatókörben rendelhető hozzá).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="7e0ff-134">**SubscriptionId:** Egy előfizetés, amelynek globális rendszergazdája **közreműködői** szerepkörrel rendelkezik vagy magasabban van hozzárendelve.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="7e0ff-135">**GlobalAdminUsername:** A globális rendszergazda felhasználóneve.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="7e0ff-136">**UsernameToAssignRoleFor:** Annak a felhasználónévnek a neve, amelyhez a piactér-rendszergazdai szerepkör hozzá lesz rendelve.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="7e0ff-137">A bérlőnek meghívott vendég felhasználók esetében akár 48 óráig is eltarthat, amíg a fiók elérhetővé válik a piactér rendszergazdai szerepkörének hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="7e0ff-138">További információ: [Azure Active Directory B2B csoportmunka-felhasználó tulajdonságai](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="7e0ff-139">Az az. Portal PowerShell-modulban található parancsmagokkal kapcsolatos további információkért tekintse meg a [Microsoft Azure PowerShell: portál irányítópult-parancsmagokat](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="7e0ff-140">Privát Azure piactér létrehozása</span><span class="sxs-lookup"><span data-stu-id="7e0ff-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="7e0ff-141">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="7e0ff-142">Válassza **a minden szolgáltatás** , majd a **piactér** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Megjeleníti a Azure Portal fő ablakát.":::

3. <span data-ttu-id="7e0ff-144">Válassza a **privát piactér** lehetőséget a bal oldali menüben.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="7e0ff-145">Válassza az első **lépések** lehetőséget a privát Azure Marketplace létrehozásához (ezt csak egyszer kell megtennie).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Bemutatja, hogyan választható ki az &quot;első lépések a Azure Portal&quot; főablakban.":::

    <span data-ttu-id="7e0ff-147">Ha a bérlőhöz már létezik privát Azure Marketplace, akkor a **piactér kezelése** alapértelmezés szerint ki lesz választva.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="7e0ff-148">Ha elkészült, üres és letiltott privát Azure Marketplace-t fog tartalmazni.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Megjeleníti az üres privát Azure Marketplace-képernyőt.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="7e0ff-150">Elemek hozzáadása a gyűjteményből</span><span class="sxs-lookup"><span data-stu-id="7e0ff-150">Add items from gallery</span></span>

<span data-ttu-id="7e0ff-151">Az elemek egy ajánlat és egy csomag kombinációja.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="7e0ff-152">A piactér kezelése oldalon kereshet és hozzáadhat elemeket.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="7e0ff-153">Válassza az **elemek hozzáadása** elemet.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-153">Select **Add items**.</span></span>

2. <span data-ttu-id="7e0ff-154">Tallózással keresse **meg a katalógust, vagy a** Keresés mező használatával keresse meg a kívánt elemeket.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="7e0ff-155">[![Bemutatja, hogyan böngészhet a katalógusban, vagy hogyan használhatja a keresési mezőt.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="7e0ff-156">Alapértelmezés szerint új ajánlat hozzáadásakor a rendszer az összes aktuális csomagot hozzáadja a jóváhagyott listához.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="7e0ff-157">Ha módosítani szeretné a csomag kijelölését a kijelölt elemek hozzáadása előtt, válassza a legördülő menüt az ajánlat csempén, és frissítse a szükséges terveket.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Bemutatja a szükséges csomagok frissítésének módját.":::

4. <span data-ttu-id="7e0ff-159">Kattintson a **kész** gombra a bal alsó sarokban, miután elvégezte a beállításokat.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="7e0ff-160">Az **elemek hozzáadása** a piactérhez csak a nem Microsoft-ajánlatok számára érhető el.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="7e0ff-161">A Microsoft-megoldások (beleértve a [támogatott Linux-disztribúciókat](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) "alapértelmezés szerint jóváhagyva" néven lesznek megjelölve, és nem kezelhetők a privát piactéren.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-161">Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="7e0ff-162">Az elemek csomagjainak szerkesztése</span><span class="sxs-lookup"><span data-stu-id="7e0ff-162">Edit item's plans</span></span>

<span data-ttu-id="7e0ff-163">A piactér kezelése lapon szerkesztheti az elemek terveit.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="7e0ff-164">A **csomagok** oszlopban tekintse át az elérhető csomagokat az adott elem legördülő menüjéből.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="7e0ff-165">Jelölje be a jelölőnégyzeteket, vagy törölje a jelölést a felhasználók számára elérhetővé tenni kívánt csomagok kiválasztásához.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Azt mutatja be, hogyan lehet kijelölni vagy törölni a kötelező elemhez tartozó jelölőnégyzetet.":::

> [!NOTE]
> <span data-ttu-id="7e0ff-167">Minden ajánlatnak legalább egy, a frissítéshez kiválasztott csomagra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="7e0ff-168">Az ajánlattal kapcsolatos összes csomag eltávolításához törölje a teljes ajánlatot (lásd a következő szakaszt).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="7e0ff-169">Ajánlatok törlése</span><span class="sxs-lookup"><span data-stu-id="7e0ff-169">Delete offers</span></span>

<span data-ttu-id="7e0ff-170">A piactér kezelése lapon jelölje be az ajánlat neve melletti jelölőnégyzetet (lásd a fenti képernyőt), és válassza az **elemek törlése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="7e0ff-171">Privát Azure Marketplace engedélyezése/letiltása</span><span class="sxs-lookup"><span data-stu-id="7e0ff-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="7e0ff-172">A piactér kezelése oldalon láthatja az alábbi szalagcímeket, amelyek a privát Azure Marketplace aktuális állapotát mutatják be:</span><span class="sxs-lookup"><span data-stu-id="7e0ff-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Az állapot letiltásának szalagcímét jeleníti meg.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Az &quot;állapot engedélyezése&quot; szalagcímet jeleníti meg.":::

<span data-ttu-id="7e0ff-175">Igény szerint engedélyezheti vagy letilthatja a privát Azure Marketplace-t.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="7e0ff-176">Ha le van tiltva, válassza a **saját piactér** engedélyezése lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="7e0ff-177">Ha engedélyezve van, a letiltáshoz válassza a **privát piactér letiltása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="7e0ff-178">Privát Azure Marketplace-értesítési központ</span><span class="sxs-lookup"><span data-stu-id="7e0ff-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="7e0ff-179">Az értesítési központ háromféle típusú értesítésből áll, és lehetővé teszi, hogy a piactér rendszergazdája a következő értesítés alapján tegyen lépéseket:</span><span class="sxs-lookup"><span data-stu-id="7e0ff-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="7e0ff-180">A jóváhagyott listán nem szereplő elemekre vonatkozó jóváhagyási kérések a felhasználóktól (lásd [az ajánlatok vagy a csomagok hozzáadására vonatkozó kérést](#request-to-add-offers-or-plans) ).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="7e0ff-181">Új csomag-értesítések olyan ajánlatokhoz, amelyeken már van egy vagy több csomag a jóváhagyott listában.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="7e0ff-182">A rendszer eltávolította a jóváhagyott listán szereplő elemek megtervezésére vonatkozó értesítéseket, de eltávolították őket a globális Azure piactéren.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="7e0ff-183">Az értesítési központ elérése:</span><span class="sxs-lookup"><span data-stu-id="7e0ff-183">To access the notification center:</span></span>

1. <span data-ttu-id="7e0ff-184">Válassza az **értesítések** lehetőséget a bal oldali menüben.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="7e0ff-185">[![Az értesítések menüt jeleníti meg.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="7e0ff-186">Válassza a három pont menüt a további műveletek elvégzéséhez.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="A további beállítások menü eredményét jeleníti meg.":::

1. <span data-ttu-id="7e0ff-188">A csomagra vonatkozó kérelmek esetében a **kérelmek megjelenítése** lehetőség megnyitja a jóváhagyási kérelem űrlapot, ahol áttekintheti az adott ajánlat összes felhasználói kérelmét.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="7e0ff-189">Válassza a **jóváhagyás** vagy az **elutasítás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="7e0ff-190">[![Megjeleníti a jóváhagyás és az elutasítás lehetőséget.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="7e0ff-191">Válassza ki a jóváhagyni kívánt tervet a legördülő menüből.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="7e0ff-192">Adjon hozzá egy megjegyzést, és válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="7e0ff-193">Privát Azure piactér tallózása</span><span class="sxs-lookup"><span data-stu-id="7e0ff-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="7e0ff-194">Ha a privát Azure Marketplace engedélyezve van, a felhasználók láthatják, hogy a piactér rendszergazdája mely terveket hagyta jóvá.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="7e0ff-195">A zöld **jóváhagyott** nyilatkozat egy jóváhagyott partner (nem Microsoft) ajánlatot jelöl.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="7e0ff-196">A kék **jóváhagyott** értesítés a jóváhagyott Microsoft-ajánlatokat (beleértve a [támogatott Linux-disztribúciókat](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)is) jelzi.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="7e0ff-197">A felhasználók a nem jóváhagyott ajánlatok között szűrhetik a következőket:</span><span class="sxs-lookup"><span data-stu-id="7e0ff-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="7e0ff-198">[![Megjeleníti a szűrési lehetőséget.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="7e0ff-199">Vásárlás vagy üzembe helyezés a privát Azure piactéren</span><span class="sxs-lookup"><span data-stu-id="7e0ff-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="7e0ff-200">Míg a termék részletei lap a globális Azure piactérhez hasonlóan működik, három privát Azure Marketplace-re vonatkozó forgatókönyv található.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="7e0ff-201">Ha egy felhasználó jóváhagyott csomagot választ, a **Létrehozás** gomb engedélyezve lesz:</span><span class="sxs-lookup"><span data-stu-id="7e0ff-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="7e0ff-202">[![Megjeleníti az ajánlati szalagcímet, amelyből egy terv hozható létre.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="7e0ff-203">Ha a termékre vonatkozó csomag kiválasztása nem jelenik meg a termék részletei lapon, de a rendszergazda jóváhagyta egy vagy több csomagot, a rendszer egy szalagcímet jelenít meg, amelyet jóváhagy, és engedélyezve van a **Létrehozás** gomb:</span><span class="sxs-lookup"><span data-stu-id="7e0ff-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="7e0ff-204">[![Megjeleníti az ajánlati szalagcímet, amely szerint egy terv hozható létre, és megjeleníthető az elérhető csomagok.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="7e0ff-205">Ha a felhasználó egy nem jóváhagyott csomagot választ, a szalagcím nem jóváhagyottként veszi fel a csomagot, és a **Létrehozás** gomb le lesz tiltva.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="7e0ff-206">A felhasználó továbbra is kérheti a terv hozzáadását a jóváhagyott listához (lásd a következő szakaszt).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="7e0ff-207">Ajánlatok és csomagok hozzáadására vonatkozó kérelem</span><span class="sxs-lookup"><span data-stu-id="7e0ff-207">Request to add offers or plans</span></span>

<span data-ttu-id="7e0ff-208">Kérheti, hogy olyan nyilvános ajánlatot vagy csomagot adjon hozzá, amely jelenleg nem lett jóváhagyva a privát Azure piactéren.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="7e0ff-209">Válassza ki a szalagcímbe **felvenni kívánt kérelmet** a **hozzáférési kérelem űrlapjának** megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="7e0ff-210">[![Megjeleníti a "kérés a hozzáadáshoz" hivatkozást tartalmazó szalagcímet.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="7e0ff-211">[![Az ajánlatok és csomagok hozzáférési kérelmi űrlapját jeleníti meg.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="7e0ff-212">Válassza ki, hogy melyik csomagot kívánja hozzáadni a kérelemhez (**bármely csomag** azt jelzi, hogy a piactér rendszergazdája nem rendelkezik az ajánlaton belüli csomagokra vonatkozó beállításokkal).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="7e0ff-213">Adjon meg egy **indoklást** , és válassza a **kérelem** lehetőséget a kérelem elküldéséhez.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="7e0ff-214">[![Az ajánlatok és csomagok hozzáférési kérelmi űrlapját jeleníti meg a minták bejegyzéseivel.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="7e0ff-215">Egy függőben lévő kérés jelzése megjelenik a hozzáférési kérelem űrlapján a **kérelem visszavonására** szolgáló lehetőséggel.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="7e0ff-216">[![A visszavont kérelmek hivatkozással rendelkező jóváhagyott vagy függőben lévő csomagok listáját jeleníti meg.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="7e0ff-217">A jóváhagyást követően a rendszer elküldi a jóváhagyási kérelem űrlapját [a piactér](#private-azure-marketplace-notification-center) rendszergazdája számára a kérelem áttekintéséhez és a művelet elvégzéséhez.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="7e0ff-218">Gyakori kérdések (GYIK)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="7e0ff-219">Már blokkolja a Marketplace harmadik féltől származó alkalmazást a Azure Policyon keresztül.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="7e0ff-220">Miben különbözik?</span><span class="sxs-lookup"><span data-stu-id="7e0ff-220">How is this different?</span></span>

<span data-ttu-id="7e0ff-221">A harmadik féltől származó szolgáltatásokat jelenleg két módon lehet korlátozni a piactéren:</span><span class="sxs-lookup"><span data-stu-id="7e0ff-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="7e0ff-222">Az EA portálon vagy a Azure Portalon tiltsa le a harmadik féltől származó szolgáltatásokat, vagy korlátozza az "ingyenes vagy BYOL SKU-ra".</span><span class="sxs-lookup"><span data-stu-id="7e0ff-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Bemutatja, hogyan lehet korlátozni a szolgáltatásokat a Azure Portalban.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Bemutatja, hogyan lehet korlátozni a szolgáltatásokat az E-portálon.":::

2. <span data-ttu-id="7e0ff-225">Hozzon létre egy Azure-szabályzatot, hogy csak bizonyos virtuális gépeket engedélyezzen.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="7e0ff-226">A Windows rendszerű virtuális gépekre vonatkozó szabályzatok kikapcsolásával kapcsolatos további információkért lásd: [házirendek alkalmazása a Windows rendszerű virtuális gépekre Azure Resource Manager használatával](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="7e0ff-227">A privát Azure piactér nagyobb rugalmasságot tesz lehetővé az egyes ajánlatok és csomagok korlátozására és engedélyezésére.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="7e0ff-228">A végfelhasználók számára elérhetővé teszi a Piactéri katalógusban való üzembe helyezést, még mielőtt külső szolgáltatásokat próbálnak üzembe helyezni.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="7e0ff-229">A harmadik féltől származó szolgáltatások üzembe helyezésének engedélyezéséhez állítsa be az Azure Marketplace-t az EA Portálon és a Azure Portalon.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="7e0ff-230">A privát Azure Marketplace-en a partneri megoldások nem korlátozódnak a virtuális gépekre.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="7e0ff-231">A privát Azure Marketplace a csomag szintjén is megadható, és az "aktuális és jövőbeli terv" is megadható.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="7e0ff-232">A privát Azure piactér tájékoztathatja a végfelhasználókat arról, hogy mit lehet és nem lehet telepíteni.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="7e0ff-233">Mi a különbség a privát ajánlat és a privát Azure Marketplace között?</span><span class="sxs-lookup"><span data-stu-id="7e0ff-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="7e0ff-234">A **privát ajánlat** lehetővé teszi, hogy a kiadók olyan csomagokat hozzanak létre, amelyek csak a célközönség számára láthatók.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="7e0ff-235">Ez lehetővé teszi, hogy a testreszabott megoldásokat megosszák az egyeztetett díjszabással, a privát feltételekkel és a speciális konfigurációkkal.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="7e0ff-236">Részletekért lásd: [privát ajánlatok a kereskedelmi piactéren](https://docs.microsoft.com/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-236">For details, see [Private offers in the commercial marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="7e0ff-237">A Azure Portal **privát Azure Marketplace** lehetővé teszi a rendszergazdák számára, hogy előzetesen hagyják el, hogy a felhasználók milyen külső megoldásokat telepíthetnek.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="7e0ff-238">A privát Azure piactéren a felhasználók a megfelelő ajánlatok megkeresésével, megvásárlásával és üzembe helyezésével élvezheti az Azure Marketplace előnyeit.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="7e0ff-239">Az előfizetés-alapú privát ajánlatok felügyeletéhez a piactér rendszergazdájának legalább "READ" szerepkörrel kell rendelkeznie az adott előfizetésben.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="7e0ff-240">Felvettem egy privát ajánlatot a privát Azure Marketplace-re, miért nem jelenik meg a piactér kezelése lapon?</span><span class="sxs-lookup"><span data-stu-id="7e0ff-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="7e0ff-241">Az előfizetés-alapú privát ajánlatok csak a privát ajánlat beállításaiban felsorolt előfizetések esetében láthatók.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="7e0ff-242">A privát ajánlat megtekintéséhez győződjön meg arról, hogy a globális előfizetés-szűrő az összes előfizetést megjeleníti.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="7e0ff-243">[![A privát piactér szűrőjét jeleníti meg.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7e0ff-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="7e0ff-244">Használhatunk egyéni lemezképeket a privát Azure piactéren?</span><span class="sxs-lookup"><span data-stu-id="7e0ff-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="7e0ff-245">Nem.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-245">No.</span></span> <span data-ttu-id="7e0ff-246">A privát Azure Marketplace lehetővé teszi a rendszergazda számára, hogy a globális Azure piactéren felügyelje és betekintse harmadik féltől származó megoldásokat.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="7e0ff-247">Mivel az egyéni lemezképek nem a globális Azure Marketplace piactéren találhatók, a rendszergazda nem választhat ki és nem választhatja ki az egyéni lemezképeket.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="7e0ff-248">Ha egyéni rendszerképeket szeretne megosztani, használja a [megosztott képtárat](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-248">If you would like to share custom images, use [Shared Image Gallery](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="7e0ff-249">Részletes útmutató a közös rendszerkép-katalógus ([parancssori](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli)felület, [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)) létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="7e0ff-250">Rendszerkép-definíció létrehozása a SIG-ban.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="7e0ff-251">Az ügyfélnek az operációs rendszer állapot mezőjében **általánosított** elemet kell választania.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="7e0ff-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="7e0ff-253">Felügyelt rendszerkép bekapcsolása a megosztott rendszerkép-katalógusba ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-253">Bring managed image into the Shared Image Gallery ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="7e0ff-254">A SIG VM-lemezképek egy előfizetésben találhatók.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="7e0ff-255">Ha más előfizetésekhez is elérhetővé kívánja tenni, használja az alkalmazás regisztrációját ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="7e0ff-255">To make it available to other subscriptions, use an app registration ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="7e0ff-256">Miért jelenik meg, hogy egyes ajánlatok **alapértelmezés szerint jóvá vannak hagyva** , noha a közzétevő nem a Microsoft?</span><span class="sxs-lookup"><span data-stu-id="7e0ff-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="7e0ff-257">A Microsoft támogatja a Linux és a nyílt forráskódú technológiák használatát az Azure-ban.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="7e0ff-258">A támogatott [Linux-disztribúciók](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) az Azure-ban támogatottak, és az ár a virtuális gépeken van integrálva.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-258">[Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="7e0ff-259">Mivel az Azure Linux-ügynök már előre telepítve van az Azure Marketplace-en, a Microsoft-ajánlathoz hasonló módon kezelik.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="7e0ff-260">Mivel a Microsoft ajánlatait alapértelmezés szerint jóváhagyják, a támogatott Linux-disztribúciók nem kezelhetők a privát Azure piactéren, és alapértelmezés szerint jóváhagyjuk azokat.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="7e0ff-261">Kapcsolatfelvétel a támogatási szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="7e0ff-261">Contact support</span></span>

- <span data-ttu-id="7e0ff-262">Az Azure Marketplace támogatásához látogasson el a [Microsoft Q&a](/answers/products/)-ra.</span><span class="sxs-lookup"><span data-stu-id="7e0ff-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>
