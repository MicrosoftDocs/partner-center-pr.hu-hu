---
title: Rendszergazdai jogosultságok újbóli Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan segítheti az ügyfeleket a partner rendszergazdai jogosultságai visszaállításában, hogy a partner segítséget tudjon kérni az ügyfelek Azure CSP kezeléséhez.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ca4c8323562e6c6f1d762465cad86e7ae113eb19
ms.sourcegitcommit: beba696954b62ab5396a893d050d0c2c211aeafc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/28/2021
ms.locfileid: "110601426"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="e6fb5-103">Rendszergazdai jogosultságok visszahelyezése egy ügyfél Azure CSP előfizetéséhez</span><span class="sxs-lookup"><span data-stu-id="e6fb5-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="e6fb5-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök</span><span class="sxs-lookup"><span data-stu-id="e6fb5-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="e6fb5-105">CSP-partnerként az ügyfelek gyakran elvárják, hogy Ön kezelje az Azure-használatot és azok rendszereit a számukra.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-105">As a CSP partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="e6fb5-106">Erre rendszergazdai jogosultsággal kell rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="e6fb5-107">Bizonyos jogosultságok akkor kapnak, ha a viszonteladói kapcsolat létrejött az ügyféllel.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="e6fb5-108">Az ügyfél másokat is ad Önnek.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="e6fb5-109">Rendszergazdai jogosultságok a Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="e6fb5-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="e6fb5-110">A rendszergazdai jogosultságoknak két szintje van a Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="e6fb5-111">**Bérlői szintű rendszergazdai jogosultságok (Delegált** rendszergazdai jogosultságok): A CSP-partnerek ezeket a jogosultságokat kapják meg, amikor CSP-viszonteladói kapcsolatot hoznak létre az ügyfelekkel.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="e6fb5-112">A delegált rendszergazdai jogosultságok hozzáférést adnak a CSP-partnereknek az ügyfeleik bérlőihez.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="e6fb5-113">Ez a hozzáférés lehetővé teszi, hogy olyan rendszergazdai feladatokat is el tudjanak látni, mint a felhasználók hozzáadása/kezelése, a jelszavak visszaállítása és a felhasználói licencek kezelése.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="e6fb5-114">**Előfizetési szintű rendszergazdai jogosultságok:** A CSP-partnerek ezeket a jogosultságokat a Azure CSP létrehozásakor kapják meg az ügyfeleik számára.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="e6fb5-115">Ezen jogosultságok révén a CSP-partnerek teljes hozzáférést számukra az előfizetésekhez, így ők is kiépítik és kezelhetik az Azure-erőforrásokat.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="e6fb5-116">A CSP-k visszaállításához a partner rendszergazdai jogosultságai</span><span class="sxs-lookup"><span data-stu-id="e6fb5-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="e6fb5-117">Az ügyfél újra létrehozhatja a CSP szerepkör-hozzárendelést, ha az AdminAgents csoport tagjait adja `object ID` meg az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="e6fb5-118">A delegált rendszergazdai jogosultságok visszaszerzése érdekében az alábbi lépésekkel együtt kell működnie az ügyféllel.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="e6fb5-119">Jelentkezzen be az Partnerközpont irányítópultjára.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="e6fb5-120">A Partnerközpont válassza az Ügyfelek **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e6fb5-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="e6fb5-121">Válassza ki azt az ügyfelet, akinél dolgozik, és kérjen **viszonteladói kapcsolatot.**</span><span class="sxs-lookup"><span data-stu-id="e6fb5-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="e6fb5-122">Ez a művelet létrehoz egy hivatkozást arra az ügyfélre, aki bérlői rendszergazdai jogosultságokkal rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="e6fb5-123">Az ügyfélnek ki kell választania a hivatkozást, és jóvá kell hagynia a viszonteladói kapcsolatkérést.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-mailes példa viszonteladói kapcsolat létrehozására":::

5. <span data-ttu-id="e6fb5-125">Önnek, a partnernek csatlakoznia kell a partnerbérlőhöz, hogy le tudja szerezni az AdminAgents csoport objektumazonosítóját.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="e6fb5-126">Az ügyfélnek ezután a következő lépéseket kell megtennie a PowerShell vagy az Azure CLI használatával.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="e6fb5-127">Az ügyfélnek a következővel kell lennie:</span><span class="sxs-lookup"><span data-stu-id="e6fb5-127">Your customer must have:</span></span>

- <span data-ttu-id="e6fb5-128">A tulajdonosi **vagy felhasználói** hozzáférés **rendszergazdájának szerepköre**</span><span class="sxs-lookup"><span data-stu-id="e6fb5-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="e6fb5-129">Szerepkör-hozzárendelések előfizetési szinten való létrehozásához szükséges engedélyek</span><span class="sxs-lookup"><span data-stu-id="e6fb5-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="e6fb5-130">a.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-130">a.</span></span> <span data-ttu-id="e6fb5-131">Csak PowerShell esetén az ügyfélnek frissítenie kell a `Az.Resources` modult.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="e6fb5-132">b.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-132">b.</span></span> <span data-ttu-id="e6fb5-133">Az ügyfél ahhoz a bérlőhöz csatlakozik, ahol a CSP-előfizetés létezik.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="e6fb5-134">c.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-134">c.</span></span> <span data-ttu-id="e6fb5-135">Az ügyfél csatlakozik az előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-135">The customer connects to the subscription.</span></span> <span data-ttu-id="e6fb5-136">Ez csak *akkor érvényes,* ha a felhasználó több előfizetésre vonatkozó szerepkör-hozzárendelési engedélyekkel rendelkezik a bérlőben.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="e6fb5-137">d.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-137">d.</span></span> <span data-ttu-id="e6fb5-138">Az ügyfél ezután létrehozza a szerepkör-hozzárendelést.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="e6fb5-139">Ahelyett, hogy tulajdonosi engedélyeket ad meg az előfizetés hatókörében, az erőforráscsoport vagy az erőforrás szintjén is adhat.</span><span class="sxs-lookup"><span data-stu-id="e6fb5-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="e6fb5-140">Az erőforráscsoport szintjén</span><span class="sxs-lookup"><span data-stu-id="e6fb5-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="e6fb5-141">Az erőforrás szintjén</span><span class="sxs-lookup"><span data-stu-id="e6fb5-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

## <a name="next-steps"></a><span data-ttu-id="e6fb5-142">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="e6fb5-142">Next steps</span></span>

- [<span data-ttu-id="e6fb5-143">Az Azure-csomagban foglalt előfizetések és erőforrások kezelése</span><span class="sxs-lookup"><span data-stu-id="e6fb5-143">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
