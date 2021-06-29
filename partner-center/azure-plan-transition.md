---
title: Ügyfelek áthelyezése a jelenlegi Azure-ajánlatokból Azure-csomagba
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogy a CSP-partnerek hogyan Partnerközpont ügyfeleket a meglévő CSP Azure-ajánlatokból az Azure-szolgáltatásokba az Azure-csomag keretében.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 770df3cff40b8cc51eab16fb95d0bd43967a5a69
ms.sourcegitcommit: 3ac88f7925bfe1df90e267ee5c1ee4d752ac92d4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/29/2021
ms.locfileid: "113013267"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a><span data-ttu-id="0b643-103">Ügyfelek váltása Azure-csomagra meglévő CSP Azure-ajánlatokból</span><span class="sxs-lookup"><span data-stu-id="0b643-103">Transition customers to Azure plan from existing CSP Azure offers</span></span>

<span data-ttu-id="0b643-104">**A következőkre vonatkozik:** Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="0b643-104">**Applies to**: Partner Center</span></span> 

<span data-ttu-id="0b643-105">**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Globális rendszergazdai | Az | Értékesítési ügynök | Felhasználókezelő rendszergazda</span><span class="sxs-lookup"><span data-stu-id="0b643-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent | User management admin</span></span>

<span data-ttu-id="0b643-106">Ez a cikk azt ismerteti, hogy a CSP-partnerek hogyan Partnerközpont az ügyfeleket a meglévő CSP Azure-ajánlatokból az Azure-szolgáltatásokba az Azure-csomag keretében.</span><span class="sxs-lookup"><span data-stu-id="0b643-106">This article explains how CSP partners can use Partner Center to move customers from existing CSP Azure offers to Azure services under the Azure plan.</span></span> <span data-ttu-id="0b643-107">A közvetett szolgáltatók és a közvetlen számlázási partnerek áttérnek az Azure-hoz elérhető Microsoft Cloud Service Provider Programban (CSP) elérhető új kereskedelmi élményre.</span><span class="sxs-lookup"><span data-stu-id="0b643-107">Indirect providers and direct bill partners can transition to the new commerce experience available in the Microsoft Cloud Service Provider Program (CSP) for Azure.</span></span> <span data-ttu-id="0b643-108">(A közvetett viszonteladóknak a közvetett szolgáltatóikon keresztül kell dolgozniuk.) Az ügyfelek zökkenőmentesen vásárolhatnak felhőszolgáltatásokat, akár partnerektől, akár Microsoft-értékesítőktől vagy közvetlenül a weben vásárolnak.</span><span class="sxs-lookup"><span data-stu-id="0b643-108">(Indirect resellers will need to work through their indirect providers.) Customers will have a streamlined way to buy cloud services, whether purchasing from partners, from Microsoft sellers, or directly on the web.</span></span>

<span data-ttu-id="0b643-109">Az áttérési képesség csak az azure-beli új kereskedelmi felhasználói élményre áttérő, és az előfizetést aláíró ügyfelek Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="0b643-109">The transition capability is only for customers transitioning to the new commerce experience for Azure and who have signed the Microsoft Customer Agreement.</span></span> <span data-ttu-id="0b643-110">Ez nem más CSP-ajánlatokhoz, például az Office 365-hez vagy a Dynamics 365-hez való.</span><span class="sxs-lookup"><span data-stu-id="0b643-110">It is not for other offers in CSP such as Office 365 or Dynamics 365.</span></span>

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a><span data-ttu-id="0b643-111">Meglévő CSP-ajánlatok váltása Azure-csomagra</span><span class="sxs-lookup"><span data-stu-id="0b643-111">Transition existing CSP offers to an Azure plan</span></span>

<span data-ttu-id="0b643-112">A CSP-program új kereskedelmi élményében az ügyfél meglévő CSP Azure-ajánlataiból az Azure-szolgáltatásokra az Azure-csomag keretében, a felhőszolgáltatói programon belül Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="0b643-112">You can transition a customer from their existing CSP Azure offers to Azure services under the Azure plan in the new commerce experience in the CSP program from within Partner Center.</span></span> <span data-ttu-id="0b643-113">Ehhez a partnernek és az ügyfélnek egy már létrehozott viszonteladói kapcsolattal kell Partnerközpont, és az ügyfélnek alá kell írnia a Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="0b643-113">To do this, the partner and customer must have an established reseller relationship through Partner Center, and the customer must have signed the Microsoft Customer Agreement.</span></span>

### <a name="select-transition-to-azure-plan"></a><span data-ttu-id="0b643-114">Váltás Azure-csomagra kiválasztása</span><span class="sxs-lookup"><span data-stu-id="0b643-114">Select transition to Azure plan</span></span>

1. <span data-ttu-id="0b643-115">Válassza az Azure-csomag lehetőséget az ügyfél számára.</span><span class="sxs-lookup"><span data-stu-id="0b643-115">Select Azure plan for your customer.</span></span>

2. <span data-ttu-id="0b643-116">Válassza **a Számlázás váltása Azure-csomagra lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="0b643-116">Select **Transition billing to Azure plan**.</span></span>

   :::image type="content" source="images/azure/transition1.png" alt-text="Képernyőkép a használatalapú előfizetések jelentési adatairól egy kiválasztható lehetőséggel: Az Azure-előfizetés számlázásának váltása Azure-csomagra.":::

3. <span data-ttu-id="0b643-118">Válassza a **Folytatás** elemet</span><span class="sxs-lookup"><span data-stu-id="0b643-118">Select **Continue**</span></span>

   :::image type="content" source="images/azure/transition2.png" alt-text="Az Áttérés Az Azure-csomagra című párbeszédpanel, amely hatással van az átváltásra, valamint két választható lehetőség, a Folytatás vagy a Mégse elemre.":::

   <span data-ttu-id="0b643-120">Az ügyfél átvált az Azure-csomagra.</span><span class="sxs-lookup"><span data-stu-id="0b643-120">Your customer will be transitioned to the Azure plan.</span></span>

   <span data-ttu-id="0b643-121">**Az átváltási munkafolyamat automatizálja az előfeltételként szükséges lépéseket:**</span><span class="sxs-lookup"><span data-stu-id="0b643-121">**The transition workflow automates the pre-requisite steps**:</span></span>

   - <span data-ttu-id="0b643-122">Azure-csomag(ak) vásárlása</span><span class="sxs-lookup"><span data-stu-id="0b643-122">Purchase of Azure plan(s)</span></span>
   - <span data-ttu-id="0b643-123">Ügyfélenként egy csomag a közvetlen CSP-forgatókönyvekben</span><span class="sxs-lookup"><span data-stu-id="0b643-123">One plan per customer in Direct CSP scenarios</span></span>  
   - <span data-ttu-id="0b643-124">Viszonteladónként egy csomag</span><span class="sxs-lookup"><span data-stu-id="0b643-124">One plan per reseller</span></span>  

   <span data-ttu-id="0b643-125">Egy partner például megvásárolt két Microsoft Azure, és két különálló POR-t tartalmazott a vásárlásban.</span><span class="sxs-lookup"><span data-stu-id="0b643-125">For an example, a partner has purchased two Microsoft Azure offers and has included two distinct POR in the purchase.</span></span> <span data-ttu-id="0b643-126">Ebben az esetben az átváltási munkafolyamat két Azure-előfizetést vásárol (viszonteladónként egyet), és automatikusan leképezi a megfelelő Azure-előfizetéseket az Azure-csomagok alatt.</span><span class="sxs-lookup"><span data-stu-id="0b643-126">In this case, the transition    workflow will purchase two Azure plans (one per reseller) and map the respective Azure subscriptions under the Azure plans automatically.</span></span>  

   <span data-ttu-id="0b643-127">**Azure-előfizetés leképezése Azure-csomagra**</span><span class="sxs-lookup"><span data-stu-id="0b643-127">**Mapping Azure subscription to Azure plan**</span></span>

   <span data-ttu-id="0b643-128">Az Azure-csomagok megvásárlása után a rendszer leképezi a meglévő Azure-előfizetéseket az Azure-csomagokra.</span><span class="sxs-lookup"><span data-stu-id="0b643-128">After your purchase of Azure plan(s), our system will map the existing Azure subscriptions to the Azure plans.</span></span> <span data-ttu-id="0b643-129">Az előrehaladás megtekinthető a Azure Portal a Partnerközpontban is.</span><span class="sxs-lookup"><span data-stu-id="0b643-129">The progress can be viewed in Azure portal as well as in Partner center.</span></span>

4. <span data-ttu-id="0b643-130">Térjen vissza az ügyfél Előfizetések Partnerközpont **oldalára,** és frissítse a költségkeretét a helyi pénznemük használatával.</span><span class="sxs-lookup"><span data-stu-id="0b643-130">Return to your customer's Partner Center **Subscriptions** page to update their budget limit using their local currency.</span></span>

   :::image type="content" source="images/azure/transition3.png" alt-text="Az Előfizetések Partnerközpont részleges nézete, amely a számlázási időszakra vonatkozó, helyi pénznemben beállított költségvetési korlátokkal rendelkezik.":::

   >[!NOTE]
   ><span data-ttu-id="0b643-132">Az ebben a Partnerközpont beállított költségvetés nem lesz áthozva a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="0b643-132">The budget you set in Partner Center doesn't carry over to the Azure portal.</span></span> <span data-ttu-id="0b643-133">A költségvetést és a riasztást a következő Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="0b643-133">You should also set the budget and alert in Azure portal.</span></span>

   <span data-ttu-id="0b643-134">Az Azure-csomagra való áttérve már nem vásárolhat Azure-előfizetéseket ehhez az ügyfélhez.</span><span class="sxs-lookup"><span data-stu-id="0b643-134">When you move to the Azure plan, you can no longer purchase Azure subscriptions for this customer.</span></span> <span data-ttu-id="0b643-135">Az előfizetéseket az Azure-csomag alatt hozhatja létre a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="0b643-135">You create the subscriptions under the Azure plan in the Azure portal.</span></span>

   >[!NOTE]
   > <span data-ttu-id="0b643-136">Az RBAC-n keresztül az Azure-csomag keretében vásárolt összes Azure-előfizetés díjszabása és számlázása helyi pénznemben történik.</span><span class="sxs-lookup"><span data-stu-id="0b643-136">All Azure subscriptions purchased through RBAC under the Azure plan will be    priced and billed in local currency.</span></span> <span data-ttu-id="0b643-137">Az FX-árfolyamok nem lesznek használva.</span><span class="sxs-lookup"><span data-stu-id="0b643-137">FX rates will not be used.</span></span>

### <a name="track-your-transition-details"></a><span data-ttu-id="0b643-138">Az átváltás részleteinek nyomon követése</span><span class="sxs-lookup"><span data-stu-id="0b643-138">Track your transition details</span></span>

<span data-ttu-id="0b643-139">Kövesse az áttérési előrehaladást a Azure Portal a következő Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="0b643-139">Follow the transition progress in Azure portal as well as in Partner Center.</span></span>

:::image type="content" source="images/azure/details1.png" alt-text="Képernyőkép az előfizetésenkénti áttűnés részleteinek listáját tartalmazó táblázatról – ide tartozik az előfizetésI D, az átváltás dátuma és az átváltás állapota.":::

### <a name="billing-impact-to-partners"></a><span data-ttu-id="0b643-141">A partnerek számlázásra gyakorolt hatása</span><span class="sxs-lookup"><span data-stu-id="0b643-141">Billing impact to partners</span></span>

<span data-ttu-id="0b643-142">Ha egy ügyfelet egy meglévő CSP Azure-ajánlatból hoz át, az a következő számlázási hatásokkal jár:</span><span class="sxs-lookup"><span data-stu-id="0b643-142">If you transition a customer from an existing CSP Azure offer, you will have the following billing impacts:</span></span>

- <span data-ttu-id="0b643-143">A meglévő CSP-számlán az összes használatért az eredeti CSP Azure-előfizetésből való kilépésig kell fizetni.</span><span class="sxs-lookup"><span data-stu-id="0b643-143">You will be billed on your existing CSP invoice for all usage up to the point of exiting the original CSP Azure subscription.</span></span>

- <span data-ttu-id="0b643-144">Ha rendszergazdai hozzáférési jogosultságokkal rendelkezik a meglévő CSP-előfizetéshez, az előfizetés migrálkor továbbra is hozzáférhet.</span><span class="sxs-lookup"><span data-stu-id="0b643-144">If you had admin access rights to the existing CSP subscription, you will continue to have access when that subscription is migrated.</span></span>

<span data-ttu-id="0b643-145">Ha közvetlen Nagyvállalati Szerződéseket a CSP- és kiszolgáló- és felhőalapú regisztrációkról azure-szolgáltatásokra is át kell irányítania, olvassa el a következőt: [Azure-előfizetések](/azure/billing/mpa-request-ownership) számlázási tulajdonjogának Microsoft Partnerszerződés</span><span class="sxs-lookup"><span data-stu-id="0b643-145">To transition direct Enterprise Agreements to CSP and Server and Cloud enrollments to Azure services, read [Get billing ownership of Azure subscriptions for Microsoft Partner Agreement](/azure/billing/mpa-request-ownership)</span></span>

### <a name="audit-log"></a><span data-ttu-id="0b643-146">Az auditnaplóban</span><span class="sxs-lookup"><span data-stu-id="0b643-146">Audit log</span></span>

<span data-ttu-id="0b643-147">A számlázás egyeztetéséhez tekintse meg a "Microsoft Azure" (0145P) előfizetések előzményeit az **Előfizetések** lapon.</span><span class="sxs-lookup"><span data-stu-id="0b643-147">To reconcile billing, view your history of "Microsoft Azure" (0145P) subscriptions on the **Subscriptions** page.</span></span>

<span data-ttu-id="0b643-148">A "Microsoft Azure" (0145P) előfizetés két részből áll:</span><span class="sxs-lookup"><span data-stu-id="0b643-148">"Microsoft Azure" (0145P) subscription is comprised of two parts:</span></span>

1. <span data-ttu-id="0b643-149">Kereskedelmi előfizetés</span><span class="sxs-lookup"><span data-stu-id="0b643-149">Commerce subscription</span></span>
2. <span data-ttu-id="0b643-150">Azure-előfizetés (jogosultság)</span><span class="sxs-lookup"><span data-stu-id="0b643-150">Azure subscription (entitlement)</span></span>

<span data-ttu-id="0b643-151">Ha az átállás befejeződött, az Azure-előfizetés az új Azure-csomag alá kerül, és a kereskedelmi előfizetés fel lesz függesztve, hogy a rendszer ne jelentsen további használatot.</span><span class="sxs-lookup"><span data-stu-id="0b643-151">When the transition is complete, the Azure subscription is moved under new Azure plan and the commerce subscription is suspended so that no further usage is reported.</span></span>  

>[!NOTE]
><span data-ttu-id="0b643-152">Amikor Microsoft Azure (0145P) előfizetést vásárolnak a CSP-ben, a kereskedelmi előfizetés és az Azure-előfizetés (jogosultság) ugyanazokkal az értékkel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="0b643-152">When Microsoft Azure (0145P) subscription is purchased in CSP, both the commerce subscription and the Azure subscription (entitlement) have the same value.</span></span> <span data-ttu-id="0b643-153">Ez csak abban az esetben változik, ha a számlázási tulajdonjog megváltozik vagy az átadások eltérnek az értékektől.</span><span class="sxs-lookup"><span data-stu-id="0b643-153">It is only in the case of billing ownership changes or transfers do the values differ.</span></span>

### <a name="transition-issues"></a><span data-ttu-id="0b643-154">Áttűnésekkel kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="0b643-154">Transition issues</span></span>

<span data-ttu-id="0b643-155">Az átváltások során nem számítunk problémákra.</span><span class="sxs-lookup"><span data-stu-id="0b643-155">We don't anticipate any issues during transitions.</span></span> <span data-ttu-id="0b643-156">Ha van ilyen, magát az átváltási munkafolyamatot fogjuk frissíteni.</span><span class="sxs-lookup"><span data-stu-id="0b643-156">If one occurs, we will update you in the transition workflow itself.</span></span> <span data-ttu-id="0b643-157">Az Azure-használatot nem fogják zavarni.</span><span class="sxs-lookup"><span data-stu-id="0b643-157">There won't be disturbances to Azure usage.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="0b643-158">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="0b643-158">Next steps</span></span>

- [<span data-ttu-id="0b643-159">Az Azure-csomagban foglalt előfizetések és erőforrások kezelése</span><span class="sxs-lookup"><span data-stu-id="0b643-159">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="0b643-160">Partneri jóváírás – áttekintés</span><span class="sxs-lookup"><span data-stu-id="0b643-160">Partner earned credit - overview</span></span>](partner-earned-credit.md)
