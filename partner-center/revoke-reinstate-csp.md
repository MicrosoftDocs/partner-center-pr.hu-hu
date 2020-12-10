---
title: Rendszergazdai jogosultságok visszaállítása az Azure CSP-hez
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy az ügyfelek hogyan állíthatják vissza a partner rendszergazdai jogosultságait, hogy a partner segítsen kezelni az ügyfelek Azure CSP-előfizetéseit.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 13fdeb01ecd73dc1a63d174a4ad5cb8e1bdc813a
ms.sourcegitcommit: 455894365fa488368f7572ac72312e84a267ef5e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/10/2020
ms.locfileid: "97011502"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="c4967-103">Rendszergazdai jogosultságok visszaállítása az ügyfél Azure CSP-előfizetései esetében</span><span class="sxs-lookup"><span data-stu-id="c4967-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="c4967-104">**Alkalmazható szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="c4967-104">**Applicable roles**</span></span>

- <span data-ttu-id="c4967-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="c4967-105">Global admin</span></span>
- <span data-ttu-id="c4967-106">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="c4967-106">Admin agent</span></span>

<span data-ttu-id="c4967-107">CSP-partnerként az ügyfelek gyakran elvárják, hogy az Azure-használatot és azok rendszereit is kezelni tudják.</span><span class="sxs-lookup"><span data-stu-id="c4967-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="c4967-108">Ehhez rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="c4967-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="c4967-109">Ezeket a jogosultságokat akkor kell megadnia, amikor a viszonteladói kapcsolat létrejött az ügyféllel.</span><span class="sxs-lookup"><span data-stu-id="c4967-109">Some privileges are granted these when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="c4967-110">Másokat az ügyfél biztosít Önnek.</span><span class="sxs-lookup"><span data-stu-id="c4967-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="c4967-111">Rendszergazdai jogosultságok az Azure-ban a CSP-ben</span><span class="sxs-lookup"><span data-stu-id="c4967-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="c4967-112">Az Azure-ban a CSP-ben két rendszergazdai jogosultsági szint van.</span><span class="sxs-lookup"><span data-stu-id="c4967-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="c4967-113">**Bérlői szintű rendszergazdai jogosultságok** (**delegált rendszergazdai jogosultságok**) – a CSP-partnerek megkapják ezeket a jogosultságokat a CSP viszonteladói kapcsolat ügyfelekkel való létrehozásakor.</span><span class="sxs-lookup"><span data-stu-id="c4967-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="c4967-114">Ez lehetővé teszi, hogy a CSP-partnerek hozzáférhessenek az ügyfelek bérlői számára, így olyan rendszergazdai feladatokat végezhetnek, mint például a felhasználók hozzáadása vagy kezelése, a jelszavak alaphelyzetbe állítása és a felhasználói licencek kezelése.</span><span class="sxs-lookup"><span data-stu-id="c4967-114">This gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="c4967-115">**Előfizetés szintű rendszergazdai jogosultságok** – a CSP-partnerek megkapják ezeket a jogosultságokat az Azure CSP-előfizetések létrehozásakor az ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="c4967-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="c4967-116">Ezek a jogosultságok lehetővé teszik a CSP-partnerek számára az Azure-erőforrások kiépítését és kezelését.</span><span class="sxs-lookup"><span data-stu-id="c4967-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="c4967-117">A CSP-partnerek rendszergazdai jogosultságának visszaállítása</span><span class="sxs-lookup"><span data-stu-id="c4967-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="c4967-118">A delegált rendszergazdai jogosultságok visszaszerzéséhez az ügyfelet kell használnia.</span><span class="sxs-lookup"><span data-stu-id="c4967-118">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="c4967-119">Jelentkezzen be a partner Center irányítópultra, és válassza a partner Center menü **ügyfelek** elemét.</span><span class="sxs-lookup"><span data-stu-id="c4967-119">Sign in to Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="c4967-120">Válassza ki azt az ügyfelet, aki dolgozik, és **kérjen egy viszonteladói kapcsolatot.**</span><span class="sxs-lookup"><span data-stu-id="c4967-120">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="c4967-121">Ez létrehoz egy hivatkozást arra a felhasználóra, aki bérlői rendszergazdai jogosultságokkal rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="c4967-121">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="c4967-122">A felhasználónak ki kell választania a hivatkozást, és jóvá kell hagynia a viszonteladói kapcsolat kérését.</span><span class="sxs-lookup"><span data-stu-id="c4967-122">That user needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="viszonteladói kapcsolat":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a><span data-ttu-id="c4967-124">A felügyeleti ügynökök csoport hozzáadása az Azure CSP-előfizetés tulajdonosaként</span><span class="sxs-lookup"><span data-stu-id="c4967-124">Adding the admin agents group as an owner for the Azure CSP subscription</span></span>

<span data-ttu-id="c4967-125">Az ügyfélnek hozzá kell adnia a felügyeleti ügynök csoportját az Azure CSP-előfizetés, egy erőforráscsoport vagy egy erőforrás tulajdonosaként.</span><span class="sxs-lookup"><span data-stu-id="c4967-125">Your customer will need to add your admin agent group as the owner of a Azure CSP subscription, a Resource group or a resource.</span></span> 

1. <span data-ttu-id="c4967-126">A PowerShell-konzol vagy a PowerShell integrált parancsfájlkezelési környezet (ISE) használata.</span><span class="sxs-lookup"><span data-stu-id="c4967-126">Use either PowerShell Console or PowerShell Integrated Scripting Environment(ISE).</span></span> <span data-ttu-id="c4967-127">Győződjön meg arról, hogy a AzureAD modulok telepítve vannak.</span><span class="sxs-lookup"><span data-stu-id="c4967-127">Ensure that AzureAD modules are installed.</span></span>

2. <span data-ttu-id="c4967-128">Kapcsolódjon az Azure AD-bérlőhöz.</span><span class="sxs-lookup"><span data-stu-id="c4967-128">Connect to your Azure AD Tenant.</span></span>

   ```powershell
   Connect-AzureAD
   ```

3. <span data-ttu-id="c4967-129">A felügyeleti ügynökök csoportjai ObjectId beolvasása.</span><span class="sxs-lookup"><span data-stu-id="c4967-129">Get ObjectId of the Admin Agents groups.</span></span>

   ```powershell
   Get-AzureADGroup
   ```
   <span data-ttu-id="c4967-130">A következő lépéseket az ügyfél azon vállalata végzi, aki tulajdonosi hozzáféréssel rendelkezik az Azure CSP-előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="c4967-130">The following steps are performed by the user in your customer's company who has owner access to the Azure CSP subscription.</span></span>

4. <span data-ttu-id="c4967-131">Az Azure CSP-előfizetéshez tulajdonosi hozzáféréssel rendelkező felhasználó hitelesítő adataival bejelentkezik az Azure-ba.</span><span class="sxs-lookup"><span data-stu-id="c4967-131">The user with owner access to the Azure CSP subscription, signs into Azure using her credentials.</span></span>

   ```powershell
   Connect-AzureRmAccount
   ```

5. <span data-ttu-id="c4967-132">Ezután hozzáadhatja a felügyeleti ügynök csoportját tulajdonosként a CSP Azure-előfizetéshez, az erőforráscsoporthoz vagy az erőforráshoz egy megfelelő erőforrás-URI alkalmazásával a hatókör-paraméterben.</span><span class="sxs-lookup"><span data-stu-id="c4967-132">She can then add your admin agent group as owner to the CSP Azure subscription, Resource group or Resource by applying a proper Resource Uri in Scope parameter.</span></span> 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a><span data-ttu-id="c4967-133">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c4967-133">Next steps</span></span>

[<span data-ttu-id="c4967-134">Az Azure-csomagban foglalt előfizetések és erőforrások kezelése</span><span class="sxs-lookup"><span data-stu-id="c4967-134">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
