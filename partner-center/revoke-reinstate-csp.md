---
title: Rendszergazdai jogosultságok újbóli Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan segítheti az ügyfeleket a partner rendszergazdai jogosultságai visszaállításában, hogy a partner segítséget tudjon kérni az ügyfelek Azure CSP előfizetései kezeléséhez.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018187"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="6914b-103">Rendszergazdai jogosultságok visszahelyezése egy ügyfél Azure CSP előfizetéséhez</span><span class="sxs-lookup"><span data-stu-id="6914b-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="6914b-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="6914b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="6914b-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="6914b-105">Global admin</span></span>
- <span data-ttu-id="6914b-106">Rendszergazdai ügynök</span><span class="sxs-lookup"><span data-stu-id="6914b-106">Admin agent</span></span>

<span data-ttu-id="6914b-107">CSP-partnerként az ügyfelek gyakran elvárják, hogy Ön kezelje az Azure-használatot és azok rendszereit számukra.</span><span class="sxs-lookup"><span data-stu-id="6914b-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="6914b-108">Ehhez rendszergazdai jogosultság szükséges.</span><span class="sxs-lookup"><span data-stu-id="6914b-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="6914b-109">Bizonyos jogosultságok akkor kapnak, ha a viszonteladói kapcsolat létrejött az ügyféllel.</span><span class="sxs-lookup"><span data-stu-id="6914b-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="6914b-110">Az ügyfél másokat is ad Önnek.</span><span class="sxs-lookup"><span data-stu-id="6914b-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="6914b-111">Rendszergazdai jogosultságok a Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="6914b-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="6914b-112">A rendszergazdai jogosultságoknak két szintje van a Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="6914b-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="6914b-113">**Bérlői szintű rendszergazdai jogosultságok** (**Delegált** rendszergazdai jogosultságok ) – A CSP-partnerek a CSP-viszonteladói kapcsolat létrehozása közben kapják meg ezeket a jogosultságokat az ügyfelekkel.</span><span class="sxs-lookup"><span data-stu-id="6914b-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="6914b-114">A delegált rendszergazdai jogosultságok hozzáférést adnak a CSP-partnereknek az ügyfeleik bérlőihez, ami lehetővé teszi számukra olyan rendszergazdai funkciók elvégzését, mint a felhasználók hozzáadása/kezelése, a jelszavak visszaállítása és a felhasználói licencek kezelése.</span><span class="sxs-lookup"><span data-stu-id="6914b-114">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="6914b-115">**Előfizetési szintű rendszergazdai jogosultságok** – A CSP-partnerek ezeket a jogosultságokat az Azure CSP létrehozásakor kapják meg az ügyfeleik számára.</span><span class="sxs-lookup"><span data-stu-id="6914b-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="6914b-116">Ezek a jogosultságok teljes hozzáférést számukra biztosít a CSP-partnerek számára ezekhez az előfizetésekhez, ami lehetővé teszi számukra az Azure-erőforrások építését és kezelését.</span><span class="sxs-lookup"><span data-stu-id="6914b-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="6914b-117">CSP-partnerek rendszergazdai jogosultságának újbóli state</span><span class="sxs-lookup"><span data-stu-id="6914b-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="6914b-118">Az ügyfél újra létrehozhatja a CSP szerepkör-hozzárendelést, ha Ön az AdminAgents csoport objektumazonosítóját adja meg az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="6914b-118">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="6914b-119">A delegált rendszergazdai jogosultságok visszaszerzése előtt az ügyféllel kell dolgoznia.</span><span class="sxs-lookup"><span data-stu-id="6914b-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="6914b-120">Jelentkezzen be a Partnerközpont irányítópultra, és a Partnerközpont menüjében válassza az Ügyfelek **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6914b-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="6914b-121">Válassza ki azt az ügyfelet, akinél dolgozik, és **kérjen viszonteladói kapcsolatot.**</span><span class="sxs-lookup"><span data-stu-id="6914b-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="6914b-122">Ez a művelet létrehoz egy hivatkozást arra az ügyfélre, aki bérlői rendszergazdai jogosultságokkal rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="6914b-122">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="6914b-123">Az ügyfélnek ki kell választania a hivatkozást, és jóvá kell hagynia a viszonteladói kapcsolatkérést.</span><span class="sxs-lookup"><span data-stu-id="6914b-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Példa e-mailben viszonteladói kapcsolat létrehozására":::

4. <span data-ttu-id="6914b-125">Önnek, a partnernek csatlakoznia kell a partnerbérlőhöz, hogy le tudja szerezni az AdminAgents csoport objektumazonosítóját.</span><span class="sxs-lookup"><span data-stu-id="6914b-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="6914b-126">Az ügyfél, aki  tulajdonosi vagy felhasználói hozzáférés-rendszergazdai szerepkört tölt be, és jogosultsággal rendelkezik szerepkör-hozzárendelés létrehozására az előfizetés szintjén, a következőket teszi:</span><span class="sxs-lookup"><span data-stu-id="6914b-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="6914b-127">Csatlakozik ahhoz a bérlőhöz, ahol a CSP-előfizetés létezik.</span><span class="sxs-lookup"><span data-stu-id="6914b-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="6914b-128">Csatlakozik az előfizetéshez (csak akkor alkalmazható, ha a felhasználó több előfizetésre vonatkozó szerepkör-hozzárendelési engedélyekkel rendelkezik a bérlőben).</span><span class="sxs-lookup"><span data-stu-id="6914b-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="6914b-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"</span><span class="sxs-lookup"><span data-stu-id="6914b-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="6914b-130">Létrehozza a szerepkör-hozzárendelést</span><span class="sxs-lookup"><span data-stu-id="6914b-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="6914b-131">Ha az előfizetés hatóköre helyett erőforráscsoport- vagy erőforrásszinten szeretne tulajdonosi szerepköri engedélyt ad, a következő parancsok működnek:</span><span class="sxs-lookup"><span data-stu-id="6914b-131">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="6914b-132">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="6914b-132">Next steps</span></span>

- [<span data-ttu-id="6914b-133">Az Azure-csomagban foglalt előfizetések és erőforrások kezelése</span><span class="sxs-lookup"><span data-stu-id="6914b-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
