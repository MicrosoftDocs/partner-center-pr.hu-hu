---
title: Privát Azure Marketplace létrehozása és kezelése Azure Portal
description: Ismerje meg, hogyan hozhat létre és kezelhet privát Azure Marketplace-t (előzetes verzió) a Azure Portal.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: f62c9aef13b51ba2db42b267d7620f506bbdc1ec
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006939"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="20e6e-103">Privát Azure Marketplace létrehozása és kezelése (előzetes verzió) a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="20e6e-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="20e6e-104">A privát Azure Marketplace (előzetes verzió) lehetővé teszi, hogy a rendszergazdák szabályozzák, hogy a felhasználók mely harmadik féltől származó megoldásokat használhatják.</span><span class="sxs-lookup"><span data-stu-id="20e6e-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="20e6e-105">Ezzel lehetővé teszi, hogy csak az Ön által jóváhagyott és a vállalati szabályzatoknak megfelelő ajánlatokat telepítse.</span><span class="sxs-lookup"><span data-stu-id="20e6e-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="20e6e-106">A privát Azure piactéren a felhasználók az online áruházban kereshetik meg a megfelelő ajánlatokat a vásárláshoz és az üzembe helyezéshez.</span><span class="sxs-lookup"><span data-stu-id="20e6e-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="20e6e-107">Piactéri rendszergazdaként (hozzárendelt szerepkör) egy letiltott és üres privát tárolóval kell kezdenie, ahol a jóváhagyott ajánlatokat és csomagokat is felveheti.</span><span class="sxs-lookup"><span data-stu-id="20e6e-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="20e6e-108">Ez a cikk bemutatja, hogyan hozhat létre, kezelhet és engedélyezhet privát Azure Marketplace-t a felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="20e6e-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="20e6e-109">Megjegyzések:</span><span class="sxs-lookup"><span data-stu-id="20e6e-109">Notes:</span></span>

- <span data-ttu-id="20e6e-110">A privát Azure piactér bérlői szinten található, így a bérlő összes felhasználója ugyanazokat a kurátori listát fogja látni.</span><span class="sxs-lookup"><span data-stu-id="20e6e-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="20e6e-111">Az összes Microsoft-megoldás automatikusan hozzáadódik a privát Azure Marketplace-hez.</span><span class="sxs-lookup"><span data-stu-id="20e6e-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="20e6e-112">A piactér rendszergazdai szerepkörének kiosztása</span><span class="sxs-lookup"><span data-stu-id="20e6e-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="20e6e-113">A bérlői globális rendszergazdának hozzá kell rendelnie a **piactér rendszergazdai** szerepkörét a privát Azure Marketplace-rendszergazda számára, aki felügyelni fogja a saját tárolót.</span><span class="sxs-lookup"><span data-stu-id="20e6e-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="20e6e-114">Az Azure Marketplace-en való hozzáférés csak a piactér rendszergazdai szerepkörrel rendelkező rendszergazdák számára érhető el.</span><span class="sxs-lookup"><span data-stu-id="20e6e-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="20e6e-115">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="20e6e-115">Prerequisites</span></span>

<span data-ttu-id="20e6e-116">Ezeket az előfeltételeket csak akkor kell teljesítenie, ha a piactér rendszergazdai szerepkört a bérlői hatókörben lévő felhasználóhoz rendeli hozzá:</span><span class="sxs-lookup"><span data-stu-id="20e6e-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="20e6e-117">**Globális rendszergazda** felhasználóhoz férhet hozzá.</span><span class="sxs-lookup"><span data-stu-id="20e6e-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="20e6e-118">A bérlőnek legalább egy előfizetése van (bármilyen típus lehet).</span><span class="sxs-lookup"><span data-stu-id="20e6e-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="20e6e-119">A kiválasztott előfizetéshez a globális rendszergazda felhasználó hozzá van rendelve a **közreműködő** szerepkörhöz vagy magasabbhoz.</span><span class="sxs-lookup"><span data-stu-id="20e6e-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>
- <span data-ttu-id="20e6e-120">A globális rendszergazda felhasználó emelt szintű hozzáféréssel rendelkezik az **Igen** értékre (lásd: [jogosultságszint-emelési hozzáférés az összes Azure-előfizetés és-felügyeleti csoport kezeléséhez](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="20e6e-120">The Global administrator user has elevated access set to **Yes** (see [Elevate access to manage all Azure subscriptions and management groups](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="20e6e-121">A piactér rendszergazdai szerepkörének kiosztása a PowerShell-lel</span><span class="sxs-lookup"><span data-stu-id="20e6e-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="20e6e-122">A piactér rendszergazdai szerepkörének hozzárendeléséhez használja a következő PowerShell-parancsfájlt: Ehhez a következő paramétereket kell megadni:</span><span class="sxs-lookup"><span data-stu-id="20e6e-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="20e6e-123">**TenantId:** A hatókörben lévő bérlő azonosítója (a piactér rendszergazdai szerepköre a bérlői hatókörben rendelhető hozzá).</span><span class="sxs-lookup"><span data-stu-id="20e6e-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="20e6e-124">**SubscriptionId:** Egy előfizetés, amelynek globális rendszergazdája **közreműködői** szerepkörrel rendelkezik vagy magasabban van hozzárendelve.</span><span class="sxs-lookup"><span data-stu-id="20e6e-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="20e6e-125">**GlobalAdminUsername:** A globális rendszergazda felhasználóneve.</span><span class="sxs-lookup"><span data-stu-id="20e6e-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="20e6e-126">**UsernameToAssignRoleFor:** Annak a felhasználónévnek a neve, amelyhez a piactér-rendszergazdai szerepkör hozzá lesz rendelve.</span><span class="sxs-lookup"><span data-stu-id="20e6e-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="20e6e-127">A bérlőnek meghívott vendég felhasználók esetében akár 48 óráig is eltarthat, amíg a fiók elérhetővé válik a piactér rendszergazdai szerepkörének hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="20e6e-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="20e6e-128">További információ: [Azure Active Directory B2B csoportmunka-felhasználó tulajdonságai](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="20e6e-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="20e6e-129">Az az. Portal PowerShell-modulban található parancsmagokkal kapcsolatos további információkért tekintse meg a [Microsoft Azure PowerShell: portál irányítópult-parancsmagokat](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="20e6e-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="20e6e-130">Privát Azure piactér létrehozása</span><span class="sxs-lookup"><span data-stu-id="20e6e-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="20e6e-131">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="20e6e-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="20e6e-132">Válassza **a minden szolgáltatás** , majd a **piactér** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="20e6e-132">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal fő ablak.":::

3. <span data-ttu-id="20e6e-134">Válassza a **privát piactér** lehetőséget a bal oldalon található beállítások közül.</span><span class="sxs-lookup"><span data-stu-id="20e6e-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Válassza ki a privát piactér elemet a Azure Portal főablakon.":::

4. <span data-ttu-id="20e6e-136">Válassza az első **lépések** lehetőséget a privát Azure Marketplace létrehozásához (ezt csak egyszer kell megtennie).</span><span class="sxs-lookup"><span data-stu-id="20e6e-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Válassza az első lépések lehetőséget a Azure Portal főablakban.":::

    <span data-ttu-id="20e6e-138">Ha a bérlőhöz már létezik privát Azure Marketplace, akkor a **piactér kezelése** alapértelmezés szerint ki lesz választva.</span><span class="sxs-lookup"><span data-stu-id="20e6e-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="20e6e-139">Ha elkészült, üres és letiltott privát Azure Marketplace-t fog tartalmazni.</span><span class="sxs-lookup"><span data-stu-id="20e6e-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Az üres privát Azure Marketplace-képernyő.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="20e6e-141">Elemek hozzáadása a gyűjteményből</span><span class="sxs-lookup"><span data-stu-id="20e6e-141">Add items from gallery</span></span>

<span data-ttu-id="20e6e-142">Az elemek egy ajánlat és egy csomag kombinációja.</span><span class="sxs-lookup"><span data-stu-id="20e6e-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="20e6e-143">A piactér kezelése oldalon megkeresheti és hozzáadhatja az elemeket.</span><span class="sxs-lookup"><span data-stu-id="20e6e-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="20e6e-144">Válassza az **elemek hozzáadása** elemet.</span><span class="sxs-lookup"><span data-stu-id="20e6e-144">Select **Add items**.</span></span>

2. <span data-ttu-id="20e6e-145">Tallózással keresse **meg a katalógust, vagy a** Keresés mező használatával keresse meg a kívánt elemeket.</span><span class="sxs-lookup"><span data-stu-id="20e6e-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Tallózással keresse meg a katalógust, vagy használja a keresőmezőt.":::

3. <span data-ttu-id="20e6e-147">Alapértelmezés szerint az új ajánlat hozzáadásakor az összes aktuális csomag hozzá lesz adva az engedélyezett listához.</span><span class="sxs-lookup"><span data-stu-id="20e6e-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="20e6e-148">Ha módosítani szeretné a csomag kijelölését a kijelölt elemek hozzáadása előtt, válassza a legördülő menüt az ajánlat csempén, és frissítse a szükséges terveket.</span><span class="sxs-lookup"><span data-stu-id="20e6e-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="A kötelező csomagok frissítése.":::

4. <span data-ttu-id="20e6e-150">Kattintson a **kész** gombra a bal alsó sarokban, miután elvégezte a beállításokat.</span><span class="sxs-lookup"><span data-stu-id="20e6e-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="20e6e-151">Az **elemek hozzáadása** a piactérhez csak a nem Microsoft-ajánlatok számára érhető el.</span><span class="sxs-lookup"><span data-stu-id="20e6e-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="20e6e-152">A Microsoft-ajánlatok alapértelmezés szerint engedélyezve vannak.</span><span class="sxs-lookup"><span data-stu-id="20e6e-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="20e6e-153">Elemszintű csomagok szerkesztése</span><span class="sxs-lookup"><span data-stu-id="20e6e-153">Edit item plans</span></span>

<span data-ttu-id="20e6e-154">A piactér kezelése oldalon szerkesztheti az elemek terveit.</span><span class="sxs-lookup"><span data-stu-id="20e6e-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="20e6e-155">A **csomagok** oszlopban tekintse át az elérhető csomagokat az adott elem legördülő menüjéből.</span><span class="sxs-lookup"><span data-stu-id="20e6e-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="20e6e-156">Jelölje be a jelölőnégyzeteket, vagy törölje a jelölést a felhasználók számára elérhetővé tenni kívánt csomagok kiválasztásához.</span><span class="sxs-lookup"><span data-stu-id="20e6e-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="A kötelező elemet tartalmazó jelölőnégyzet bejelölése vagy törlése.":::

> [!NOTE]
> <span data-ttu-id="20e6e-158">Minden ajánlatnak legalább egy tervet ki kell választania, hogy a frissítés megtörténjen.</span><span class="sxs-lookup"><span data-stu-id="20e6e-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="20e6e-159">Az ajánlattal kapcsolatos összes csomag eltávolításához törölje a teljes ajánlatot (lásd a következő szakaszt).</span><span class="sxs-lookup"><span data-stu-id="20e6e-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="20e6e-160">Ajánlatok törlése</span><span class="sxs-lookup"><span data-stu-id="20e6e-160">Delete offers</span></span>

<span data-ttu-id="20e6e-161">A piactér kezelése lapon jelölje be az ajánlat neve melletti jelölőnégyzetet (lásd a fenti képernyőt), és válassza az **elemek törlése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="20e6e-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="20e6e-162">Privát Azure Marketplace engedélyezése/letiltása</span><span class="sxs-lookup"><span data-stu-id="20e6e-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="20e6e-163">A piactér kezelése oldalon láthatja az alábbi szalagcímeket, amelyek a privát Azure Marketplace aktuális állapotát mutatják be:</span><span class="sxs-lookup"><span data-stu-id="20e6e-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Állapot szalagcímének letiltása":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Állapot szalagcímének engedélyezése":::

<span data-ttu-id="20e6e-166">Igény szerint engedélyezheti vagy letilthatja a privát Azure Marketplace-t.</span><span class="sxs-lookup"><span data-stu-id="20e6e-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="20e6e-167">Ha le van tiltva, válassza a **saját piactér** engedélyezése lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="20e6e-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="20e6e-168">Ha engedélyezve van, a letiltáshoz válassza a **privát piactér letiltása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="20e6e-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="20e6e-169">Privát Azure piactér tallózása</span><span class="sxs-lookup"><span data-stu-id="20e6e-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="20e6e-170">Ha a privát Azure Marketplace engedélyezve van, a felhasználók láthatják, hogy a piactér rendszergazdája milyen terveket engedélyezett.</span><span class="sxs-lookup"><span data-stu-id="20e6e-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="20e6e-171">A zöld **megengedett** értesítés egy olyan partner (nem Microsoft) ajánlatot jelöl, amely engedélyezett.</span><span class="sxs-lookup"><span data-stu-id="20e6e-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="20e6e-172">A kék **megengedett** értesítés egy engedélyezett Microsoft-ajánlatot jelez.</span><span class="sxs-lookup"><span data-stu-id="20e6e-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="20e6e-173">A felhasználók a (z) és a nem engedélyezett ajánlatok között szűrhetők:</span><span class="sxs-lookup"><span data-stu-id="20e6e-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Szűrési beállítás.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="20e6e-175">Vásárlás vagy üzembe helyezés a privát Azure piactéren</span><span class="sxs-lookup"><span data-stu-id="20e6e-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="20e6e-176">Míg a termék részletei lap a nyilvános Azure piactérhez hasonlóan működik, három privát Azure Marketplace-re vonatkozó forgatókönyv található.</span><span class="sxs-lookup"><span data-stu-id="20e6e-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="20e6e-177">Ha egy felhasználó egy engedélyezett csomagot választ, a **Létrehozás** gomb engedélyezve lesz:</span><span class="sxs-lookup"><span data-stu-id="20e6e-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Ajánlati szalagcím, amelyből egy terv hozható létre.":::

- <span data-ttu-id="20e6e-179">Ha a felhasználó egy nem engedélyezett csomagot választ ki, a szalagcím megjegyzi, hogy a csomag nem engedélyezett, és a **Létrehozás** gomb le van tiltva.</span><span class="sxs-lookup"><span data-stu-id="20e6e-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Ajánlati szalagcím – a terv nem hozható létre.":::

- <span data-ttu-id="20e6e-181">Ha a termékre vonatkozó csomag kiválasztása nem jelenik meg a termék részletei lapon, de a rendszergazda jóváhagyta egy vagy több csomagot, a szalagcím megállapítja, hogy mely csomagok engedélyezettek, és engedélyezve van a **Létrehozás** gomb:</span><span class="sxs-lookup"><span data-stu-id="20e6e-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Ajánlati szalagcím, amelyből az a terv is létrehozható, és megjeleníthető az elérhető csomagok.":::

## <a name="contact-support"></a><span data-ttu-id="20e6e-183">Kapcsolatfelvétel a támogatási szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="20e6e-183">Contact support</span></span>

<span data-ttu-id="20e6e-184">Az Azure Marketplace támogatásához látogasson el a [Microsoft Q&a](/answers/products/)-ra.</span><span class="sxs-lookup"><span data-stu-id="20e6e-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
