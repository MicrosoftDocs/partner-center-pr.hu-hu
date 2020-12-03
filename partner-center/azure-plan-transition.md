---
title: Ügyfelek áthelyezése az aktuális Azure-ajánlatokból az Azure-csomagba
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy a CSP-partnerek hogyan használhatják a partner központot a meglévő CSP Azure-ajánlatokból az Azure-csomag keretében az Azure-szolgáltatásokhoz.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 4e22386dc8bddd9662a0d80020a5c90c464e9d39
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534811"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a><span data-ttu-id="5555c-103">Ügyfelek átváltása Azure-csomagra meglévő CSP Azure-ajánlatokból</span><span class="sxs-lookup"><span data-stu-id="5555c-103">Transition customers to Azure plan from existing CSP Azure offers</span></span>

<span data-ttu-id="5555c-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="5555c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5555c-105">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="5555c-105">Admin agent</span></span>
- <span data-ttu-id="5555c-106">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="5555c-106">Billing admin</span></span>
- <span data-ttu-id="5555c-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="5555c-107">Global admin</span></span>
- <span data-ttu-id="5555c-108">Segélyszolgálat ügynöke</span><span class="sxs-lookup"><span data-stu-id="5555c-108">Helpdesk agent</span></span>
- <span data-ttu-id="5555c-109">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="5555c-109">Sales agent</span></span>
- <span data-ttu-id="5555c-110">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="5555c-110">User management admin</span></span>

<span data-ttu-id="5555c-111">Ez a cikk azt ismerteti, hogy a CSP-partnerek hogyan használhatják a partner központot a meglévő CSP Azure-ajánlatokból az Azure-csomagba tartozó Azure-szolgáltatásokhoz.</span><span class="sxs-lookup"><span data-stu-id="5555c-111">This article explains how CSP partners can use Partner Center to move customers from existing CSP Azure offers to Azure services under the Azure plan.</span></span> <span data-ttu-id="5555c-112">A közvetett szolgáltatók és a közvetlen számlázási partnerek az Azure-beli Microsoft Cloud Service Provider program (CSP) szolgáltatásban elérhető új kereskedelmi élményre válthatnak.</span><span class="sxs-lookup"><span data-stu-id="5555c-112">Indirect providers and direct bill partners can transition to the new commerce experience available in the Microsoft Cloud Service Provider Program (CSP) for Azure.</span></span> <span data-ttu-id="5555c-113">(A közvetett viszonteladóknak a közvetett szolgáltatókon keresztül kell dolgozniuk.) Az ügyfelek zökkenőmentesen vehetik igénybe a felhőalapú szolgáltatásokat, akár a partnerektől, akár a Microsoft értékesítőtől, akár közvetlenül a világhálón vásárolnak.</span><span class="sxs-lookup"><span data-stu-id="5555c-113">(Indirect resellers will need to work through their indirect providers.) Customers will have a streamlined way to buy cloud services, whether purchasing from partners, from Microsoft sellers, or directly on the web.</span></span>

<span data-ttu-id="5555c-114">Az áttérési képesség csak olyan ügyfelek számára érhető el, akik az Azure-hoz készült új kereskedelmi tapasztalatra áttértek, és akik aláírták a Microsoft ügyfél-szerződést.</span><span class="sxs-lookup"><span data-stu-id="5555c-114">The transition capability is only for customers transitioning to the new commerce experience for Azure and who have signed the Microsoft Customer Agreement.</span></span> <span data-ttu-id="5555c-115">Nem a CSP egyéb ajánlatai, például az Office 365 vagy a Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="5555c-115">It is not for other offers in CSP such as Office 365 or Dynamics 365.</span></span>

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a><span data-ttu-id="5555c-116">Meglévő CSP-ajánlatok átváltása Azure-csomagra</span><span class="sxs-lookup"><span data-stu-id="5555c-116">Transition existing CSP offers to an Azure plan</span></span>

<span data-ttu-id="5555c-117">A meglévő CSP Azure-ajánlatait áthelyezheti az Azure-szolgáltatásokba az Azure-csomag keretében az új kereskedelmi környezet keretében a CSP programban a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="5555c-117">You can transition a customer from their existing CSP Azure offers to Azure services under the Azure plan in the new commerce experience in the CSP program from within Partner Center.</span></span> <span data-ttu-id="5555c-118">Ehhez a partnernek és az ügyfélnek rendelkeznie kell egy, a partner centeren keresztül létrehozott viszonteladói kapcsolattal, és az ügyfélnek alá kell írnia a Microsoft ügyfél-szerződést.</span><span class="sxs-lookup"><span data-stu-id="5555c-118">To do this, the partner and customer must have an established reseller relationship through Partner Center, and the customer must have signed the Microsoft Customer Agreement.</span></span>

### <a name="select-transition-to-azure-plan"></a><span data-ttu-id="5555c-119">Az Azure-csomagra való áttérés kiválasztása</span><span class="sxs-lookup"><span data-stu-id="5555c-119">Select transition to Azure plan</span></span>

1. <span data-ttu-id="5555c-120">Válassza ki az Azure-csomagot az ügyfél számára.</span><span class="sxs-lookup"><span data-stu-id="5555c-120">Select Azure plan for your customer.</span></span>

2. <span data-ttu-id="5555c-121">Válassza **az áttérési számlázás az Azure-csomagra** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="5555c-121">Select **Transition billing to Azure plan**.</span></span>

   :::image type="content" source="images/azure/transition1.png" alt-text="Képernyőfelvétel: a használaton alapuló előfizetések jelentési információi az Azure-előfizetésre váltás Azure-csomagra való áttéréskor használt választható lehetőséggel.":::

3. <span data-ttu-id="5555c-123">Válassza a **Folytatás** elemet</span><span class="sxs-lookup"><span data-stu-id="5555c-123">Select **Continue**</span></span>

   :::image type="content" source="images/azure/transition2.png" alt-text="Az Azure-csomagra való áttérést ismertető párbeszédpanel, amely az áttéréssel kapcsolatos tudnivalókat és a kiválasztható, folytatott vagy megszakított két lehetőséget is érinti.":::

   <span data-ttu-id="5555c-125">Az ügyfelet az Azure-csomagra fogjuk áttérni.</span><span class="sxs-lookup"><span data-stu-id="5555c-125">Your customer will be transitioned to the Azure plan.</span></span>

   <span data-ttu-id="5555c-126">**Az áttérési munkafolyamat automatizálja az előfeltételként szükséges lépéseket**:</span><span class="sxs-lookup"><span data-stu-id="5555c-126">**The transition workflow automates the pre-requisite steps**:</span></span>

   - <span data-ttu-id="5555c-127">Azure-csomag (ok) vásárlása</span><span class="sxs-lookup"><span data-stu-id="5555c-127">Purchase of Azure plan(s)</span></span>
   - <span data-ttu-id="5555c-128">Egy csomag ügyfélként a közvetlen CSP-forgatókönyvek esetében</span><span class="sxs-lookup"><span data-stu-id="5555c-128">One plan per customer in Direct CSP scenarios</span></span>  
   - <span data-ttu-id="5555c-129">Egy csomag/viszonteladó</span><span class="sxs-lookup"><span data-stu-id="5555c-129">One plan per reseller</span></span>  

   <span data-ttu-id="5555c-130">Egy partner például két Microsoft Azure ajánlatot vásárolt, és két különböző POR szerepel a vásárlásban.</span><span class="sxs-lookup"><span data-stu-id="5555c-130">For an example, a partner has purchased two Microsoft Azure offers and has included two distinct POR in the purchase.</span></span> <span data-ttu-id="5555c-131">Ebben az esetben az áttérési munkafolyamat két Azure-csomagot (egy-egy viszonteladót) vásárol, és az Azure-csomagok megfelelő Azure-előfizetéseit automatikusan leképezi.</span><span class="sxs-lookup"><span data-stu-id="5555c-131">In this case, the transition    workflow will purchase two Azure plans (one per reseller) and map the respective Azure subscriptions under the Azure plans automatically.</span></span>  

   <span data-ttu-id="5555c-132">**Azure-előfizetés leképezése az Azure-csomagra**</span><span class="sxs-lookup"><span data-stu-id="5555c-132">**Mapping Azure subscription to Azure plan**</span></span>

   <span data-ttu-id="5555c-133">Az Azure-csomag (ok) megvásárlása után a rendszer leképezi a meglévő Azure-előfizetéseket az Azure-csomagokra.</span><span class="sxs-lookup"><span data-stu-id="5555c-133">After your purchase of Azure plan(s), our system will map the existing Azure subscriptions to the Azure plans.</span></span> <span data-ttu-id="5555c-134">A folyamat Azure Portal és a partner Centerben is megtekinthető.</span><span class="sxs-lookup"><span data-stu-id="5555c-134">The progress can be viewed in Azure portal as well as in Partner center.</span></span>

4. <span data-ttu-id="5555c-135">Térjen vissza az ügyfél partneri központ- **előfizetések** lapjára, hogy a helyi pénznem alapján frissítse a költségvetési korlátot.</span><span class="sxs-lookup"><span data-stu-id="5555c-135">Return to your customer's Partner Center **Subscriptions** page to update their budget limit using their local currency.</span></span>

   :::image type="content" source="images/azure/transition3.png" alt-text="A partner Center-előfizetések oldalának részleges megtekintése a helyi pénznemben beállított költségvetési korlátokkal egy számlázási időszakra vonatkozóan.":::

   >[!NOTE]
   ><span data-ttu-id="5555c-137">A partner Centerben megadott költségkeret nem veszi át a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="5555c-137">The budget you set in Partner Center doesn't carry over to the Azure portal.</span></span> <span data-ttu-id="5555c-138">A költségvetést és a riasztást is be kell állítania Azure Portalban.</span><span class="sxs-lookup"><span data-stu-id="5555c-138">You should also set the budget and alert in Azure portal.</span></span>

   <span data-ttu-id="5555c-139">Az Azure-csomagra való áttérés után már nem vásárolhat Azure-előfizetéseket ehhez az ügyfélhez.</span><span class="sxs-lookup"><span data-stu-id="5555c-139">When you move to the Azure plan, you can no longer purchase Azure subscriptions for this customer.</span></span> <span data-ttu-id="5555c-140">Az előfizetéseket az Azure Portal Azure-csomagjában hozza létre.</span><span class="sxs-lookup"><span data-stu-id="5555c-140">You create the subscriptions under the Azure plan in the Azure portal.</span></span>

   >[!NOTE]
   > <span data-ttu-id="5555c-141">Az Azure-RBAC keresztül vásárolt Azure-előfizetések díjszabása és számlázása helyi pénznemben történik.</span><span class="sxs-lookup"><span data-stu-id="5555c-141">All Azure subscriptions purchased through RBAC under the Azure plan will be    priced and billed in local currency.</span></span> <span data-ttu-id="5555c-142">Az FX díjszabása nem lesz használatban.</span><span class="sxs-lookup"><span data-stu-id="5555c-142">FX rates will not be used.</span></span>

### <a name="track-your-transition-details"></a><span data-ttu-id="5555c-143">Az áttérés részleteinek nyomon követése</span><span class="sxs-lookup"><span data-stu-id="5555c-143">Track your transition details</span></span>

<span data-ttu-id="5555c-144">Kövesse az áttérési folyamatot Azure Portal és a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="5555c-144">Follow the transition progress in Azure portal as well as in Partner Center.</span></span>

:::image type="content" source="images/azure/details1.png" alt-text="Képernyőfelvétel: az előfizetésre vonatkozó átmeneti részletek listáját tartalmazó táblázat, amely tartalmazza az előfizetés I D, az áttérési dátumot és az áttérési állapotot.":::

### <a name="billing-impact-to-partners"></a><span data-ttu-id="5555c-146">A partnerek felé irányuló számlázási hatás</span><span class="sxs-lookup"><span data-stu-id="5555c-146">Billing impact to partners</span></span>

<span data-ttu-id="5555c-147">Ha egy meglévő CSP Azure-ajánlatból átvált egy ügyfelet, a következő számlázási hatások lesznek:</span><span class="sxs-lookup"><span data-stu-id="5555c-147">If you transition a customer from an existing CSP Azure offer, you will have the following billing impacts:</span></span>

- <span data-ttu-id="5555c-148">A meglévő CSP-számlán minden használat után az eredeti CSP Azure-előfizetés kilépési pontjáig kell fizetnie.</span><span class="sxs-lookup"><span data-stu-id="5555c-148">You will be billed on your existing CSP invoice for all usage up to the point of exiting the original CSP Azure subscription.</span></span>

- <span data-ttu-id="5555c-149">Ha rendszergazdai hozzáférési jogosultságokkal rendelkezik a meglévő CSP-előfizetéshez, akkor továbbra is hozzáférhet az előfizetés áttelepítésekor.</span><span class="sxs-lookup"><span data-stu-id="5555c-149">If you had admin access rights to the existing CSP subscription, you will continue to have access when that subscription is migrated.</span></span>

<span data-ttu-id="5555c-150">A közvetlen nagyvállalati szerződések a CSP-re, valamint a kiszolgáló-és Felhőbeli regisztrációra az Azure-szolgáltatásokra való áttéréshez olvassa el az [Azure-előfizetések számlázásának beszerzése](/azure/billing/mpa-request-ownership)</span><span class="sxs-lookup"><span data-stu-id="5555c-150">To transition direct Enterprise Agreements to CSP and Server and Cloud enrollments to Azure services, read [Get billing ownership of Azure subscriptions for Microsoft Partner Agreement](/azure/billing/mpa-request-ownership)</span></span>

### <a name="audit-log"></a><span data-ttu-id="5555c-151">Az auditnaplóban</span><span class="sxs-lookup"><span data-stu-id="5555c-151">Audit log</span></span>

<span data-ttu-id="5555c-152">A számlázás egyeztetéséhez tekintse meg a "Microsoft Azure" (0145P) előfizetések előzményeit az **előfizetések** lapon.</span><span class="sxs-lookup"><span data-stu-id="5555c-152">To reconcile billing, view your history of "Microsoft Azure" (0145P) subscriptions on the **Subscriptions** page.</span></span>

<span data-ttu-id="5555c-153">A "Microsoft Azure" (0145P) előfizetés két részből áll:</span><span class="sxs-lookup"><span data-stu-id="5555c-153">"Microsoft Azure" (0145P) subscription is comprised of two parts:</span></span>

1. <span data-ttu-id="5555c-154">Kereskedelmi előfizetés</span><span class="sxs-lookup"><span data-stu-id="5555c-154">Commerce subscription</span></span>
2. <span data-ttu-id="5555c-155">Azure-előfizetés (jogosultság)</span><span class="sxs-lookup"><span data-stu-id="5555c-155">Azure subscription (entitlement)</span></span>

<span data-ttu-id="5555c-156">Az áttérés befejezésekor az Azure-előfizetést új Azure-csomagba helyezi át, és a kereskedelmi előfizetés fel van függesztve, hogy ne jelentsen további használati adatokat.</span><span class="sxs-lookup"><span data-stu-id="5555c-156">When the transition is complete, the Azure subscription is moved under new Azure plan and the commerce subscription is suspended so that no further usage is reported.</span></span>  

>[!NOTE]
><span data-ttu-id="5555c-157">Ha Microsoft Azure (0145P) előfizetést vásárol a CSP-ben, akkor a kereskedelmi előfizetés és az Azure-előfizetés (jogosultság) is azonos értékű.</span><span class="sxs-lookup"><span data-stu-id="5555c-157">When Microsoft Azure (0145P) subscription is purchased in CSP, both the commerce subscription and the Azure subscription (entitlement) have the same value.</span></span> <span data-ttu-id="5555c-158">Csak a számlázási tulajdonosi változások esetén, vagy az értékek eltérőek.</span><span class="sxs-lookup"><span data-stu-id="5555c-158">It is only in the case of billing ownership changes or transfers do the values differ.</span></span>

### <a name="transition-issues"></a><span data-ttu-id="5555c-159">Átmeneti problémák</span><span class="sxs-lookup"><span data-stu-id="5555c-159">Transition issues</span></span>

<span data-ttu-id="5555c-160">A váltás során nem számítunk fel problémákat.</span><span class="sxs-lookup"><span data-stu-id="5555c-160">We don't anticipate any issues during transitions.</span></span> <span data-ttu-id="5555c-161">Ha ez történik, az áttérési munkafolyamatban is frissítjük Önt.</span><span class="sxs-lookup"><span data-stu-id="5555c-161">If one occurs, we will update you in the transition workflow itself.</span></span> <span data-ttu-id="5555c-162">Nem zavarja az Azure-használatot.</span><span class="sxs-lookup"><span data-stu-id="5555c-162">There won't be disturbances to Azure usage.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="5555c-163">További lépések</span><span class="sxs-lookup"><span data-stu-id="5555c-163">Next steps</span></span>

- [<span data-ttu-id="5555c-164">Az Azure-csomagban foglalt előfizetések és erőforrások kezelése</span><span class="sxs-lookup"><span data-stu-id="5555c-164">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="5555c-165">Partner által létrehozott kredit – áttekintés</span><span class="sxs-lookup"><span data-stu-id="5555c-165">Partner earned credit - overview</span></span>](partner-earned-credit.md)