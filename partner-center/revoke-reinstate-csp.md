---
title: Rendszergazdai jogosultságok visszaállítása az Azure CSP-hez
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy az ügyfelek hogyan állíthatják vissza a partner rendszergazdai jogosultságait, hogy a partner segítsen kezelni az ügyfelek Azure CSP-előfizetéseit.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315847"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="e0344-103">Rendszergazdai jogosultságok visszaállítása az ügyfél Azure CSP-előfizetései esetében</span><span class="sxs-lookup"><span data-stu-id="e0344-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="e0344-104">**Alkalmazható szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="e0344-104">**Applicable roles**</span></span>

- <span data-ttu-id="e0344-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="e0344-105">Global admin</span></span>
- <span data-ttu-id="e0344-106">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="e0344-106">Admin agent</span></span>

<span data-ttu-id="e0344-107">CSP-partnerként az ügyfelek gyakran elvárják, hogy az Azure-használatot és azok rendszereit is kezelni tudják.</span><span class="sxs-lookup"><span data-stu-id="e0344-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="e0344-108">Ehhez rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="e0344-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="e0344-109">Bizonyos jogosultságokat akkor kell megadni, ha a viszonteladói kapcsolat létrejött az ügyféllel.</span><span class="sxs-lookup"><span data-stu-id="e0344-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="e0344-110">Másokat az ügyfél biztosít Önnek.</span><span class="sxs-lookup"><span data-stu-id="e0344-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="e0344-111">Rendszergazdai jogosultságok az Azure-ban a CSP-ben</span><span class="sxs-lookup"><span data-stu-id="e0344-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="e0344-112">Az Azure-ban a CSP-ben két rendszergazdai jogosultsági szint van.</span><span class="sxs-lookup"><span data-stu-id="e0344-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="e0344-113">**Bérlői szintű rendszergazdai jogosultságok** (**delegált rendszergazdai jogosultságok**) – a CSP-partnerek megkapják ezeket a jogosultságokat a CSP viszonteladói kapcsolat ügyfelekkel való létrehozásakor.</span><span class="sxs-lookup"><span data-stu-id="e0344-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="e0344-114">A delegált rendszergazdai jogosultságok lehetővé teszik a CSP-partnerek számára, hogy hozzáférjenek az ügyfelek bérlői számára, így olyan rendszergazdai feladatokat hajthatnak végre, mint például felhasználók hozzáadása/kezelése, jelszavak alaphelyzetbe állítása és felhasználói licencek kezelése.</span><span class="sxs-lookup"><span data-stu-id="e0344-114">Delegated admin privileges gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="e0344-115">**Előfizetés szintű rendszergazdai jogosultságok** – a CSP-partnerek megkapják ezeket a jogosultságokat az Azure CSP-előfizetések létrehozásakor az ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="e0344-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="e0344-116">Ezek a jogosultságok lehetővé teszik a CSP-partnerek számára az Azure-erőforrások kiépítését és kezelését.</span><span class="sxs-lookup"><span data-stu-id="e0344-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="e0344-117">A CSP-partnerek rendszergazdai jogosultságának visszaállítása</span><span class="sxs-lookup"><span data-stu-id="e0344-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="e0344-118">Az ügyfél újra létrehozhatja a CSP szerepkör-hozzárendelést, ha megadja az ügyfélnek az AdminAgents-csoport objektumazonosítót.</span><span class="sxs-lookup"><span data-stu-id="e0344-118">Your customer is able to re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="e0344-119">A delegált rendszergazdai jogosultságok visszaszerzéséhez az ügyfelet kell használnia.</span><span class="sxs-lookup"><span data-stu-id="e0344-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="e0344-120">Jelentkezzen be a partner Center irányítópultra, és válassza a partner Center menü **ügyfelek** elemét.</span><span class="sxs-lookup"><span data-stu-id="e0344-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="e0344-121">Válassza ki azt az ügyfelet, aki dolgozik, és **kérjen egy viszonteladói kapcsolatot.**</span><span class="sxs-lookup"><span data-stu-id="e0344-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="e0344-122">Ez létrehoz egy hivatkozást arra a felhasználóra, aki bérlői rendszergazdai jogosultságokkal rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="e0344-122">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="e0344-123">Az ügyfélnek ki kell választania a hivatkozást, és jóvá kell hagynia a viszonteladói kapcsolat kérését.</span><span class="sxs-lookup"><span data-stu-id="e0344-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-mail-példa viszonteladói kapcsolat létrehozására":::

4. <span data-ttu-id="e0344-125">Önnek, a partnernek csatlakoznia kell a partner bérlőhöz a AdminAgents-csoport objektumazonosító beszerzéséhez.</span><span class="sxs-lookup"><span data-stu-id="e0344-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="e0344-126">Az a felhasználó, aki rendelkezik a **tulajdonosi vagy a felhasználói hozzáférés-adminisztrátor** szerepkörrel, és jogosult szerepkör-hozzárendelés létrehozására az előfizetési szinten, a következő műveleteket végzi el:</span><span class="sxs-lookup"><span data-stu-id="e0344-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="e0344-127">Csatlakozik ahhoz a bérlőhöz, ahol a CSP-előfizetés létezik.</span><span class="sxs-lookup"><span data-stu-id="e0344-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="e0344-128">Csatlakozás az előfizetéshez (csak akkor alkalmazható, ha a felhasználó szerepkör-hozzárendelési engedéllyel rendelkezik több előfizetéshez a bérlőn).</span><span class="sxs-lookup"><span data-stu-id="e0344-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="e0344-129">PS CWindowsSystem32> Set-AzContext-SubscriptionID "CSP előfizetés azonosítója" "</span><span class="sxs-lookup"><span data-stu-id="e0344-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="e0344-130">Létrehozza a szerepkör-hozzárendelést.</span><span class="sxs-lookup"><span data-stu-id="e0344-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="e0344-131">Ha azt szeretné, hogy az erőforrás-csoport szintjén vagy az erőforrás szintjén adja meg a tulajdonosi szerepkör engedélyt az előfizetés hatóköre helyett, a következő parancsok működhetnek:</span><span class="sxs-lookup"><span data-stu-id="e0344-131">If the desire is to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="e0344-132">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="e0344-132">Next steps</span></span>

- [<span data-ttu-id="e0344-133">Az Azure-csomagban foglalt előfizetések és erőforrások kezelése</span><span class="sxs-lookup"><span data-stu-id="e0344-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
