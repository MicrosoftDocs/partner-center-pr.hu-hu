---
title: Azure-előfizetés átvitele Azure-csomag alá egy másik CSP-partnernek
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan módosíthatja Felhőszolgáltató ügyfél Azure-előfizetéséhez társított partnert egy Azure-csomag keretében.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: f0abfdfd2fbb242f7cdbe0ded04d387ea712cce5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702722"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="896e9-103">Ügyfél Azure-csomag előfizetésének átadása egy másik partnernek</span><span class="sxs-lookup"><span data-stu-id="896e9-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="896e9-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="896e9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="896e9-105">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="896e9-105">Account admin</span></span>
- <span data-ttu-id="896e9-106">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="896e9-106">Sales agent</span></span>
- <span data-ttu-id="896e9-107">Számlázási ügynök</span><span class="sxs-lookup"><span data-stu-id="896e9-107">Billing agent</span></span>

<span data-ttu-id="896e9-108">Ez a cikk azt ismerteti, hogy az ügyfelek hogyan válthatnak Azure-előfizetéseik között egy Azure-Felhőszolgáltató (CSP) egy másikra.</span><span class="sxs-lookup"><span data-stu-id="896e9-108">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="896e9-109">Ha egy ügyfél Azure-előfizetéseit egy másik partnerről is átkapcsolja, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="896e9-109">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="896e9-110">A partnernek és az ügyfélnek is vannak lépései.</span><span class="sxs-lookup"><span data-stu-id="896e9-110">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="896e9-111">Csak a Microsofttal közvetlen számlázási kapcsolatban áll partnerek férhetnek hozzá az átváltási eszközökhez.</span><span class="sxs-lookup"><span data-stu-id="896e9-111">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="896e9-112">A közvetett viszonteladóknak a közvetett szolgáltatóikkal együtt kell használniuk ezt az áttérési eszközt.</span><span class="sxs-lookup"><span data-stu-id="896e9-112">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="896e9-113">Az ügyfélnek mindkét partnerrel (aktuális és jövőbeli) kapcsolatban kell lennie az eszköz használata előtt.</span><span class="sxs-lookup"><span data-stu-id="896e9-113">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="896e9-114">A félreértések és adatváltozások elkerülése érdekében offline beszélgetést kell folytatni.</span><span class="sxs-lookup"><span data-stu-id="896e9-114">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="896e9-115">Emellett a partnereknek és az ügyfeleknek az átállás megkezdése előtt meg kell érteniük ezeket a szempontokat és előfeltételeket:</span><span class="sxs-lookup"><span data-stu-id="896e9-115">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="896e9-116">**Fő szempontok:**</span><span class="sxs-lookup"><span data-stu-id="896e9-116">**Key considerations:**</span></span>

- <span data-ttu-id="896e9-117">Az Azure Reservations nem lesz áthelyezve az előfizetéssel a jövőbeli partnerhez</span><span class="sxs-lookup"><span data-stu-id="896e9-117">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="896e9-118">Az aktuális partnerhez az Azure-szolgáltatások CSP-díjszabása nem fog áttérni</span><span class="sxs-lookup"><span data-stu-id="896e9-118">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="896e9-119">Az ügyfél támogatási feladatai a jövőbeli partnerhez fognak átköltözni</span><span class="sxs-lookup"><span data-stu-id="896e9-119">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="896e9-120">A számlázás és a számlázás az átadáskor át fog költözni a jövőbeli partnerhez</span><span class="sxs-lookup"><span data-stu-id="896e9-120">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="896e9-121">Az azure Role-Based Access Control (RBAC) nincs hatással az átvitelre</span><span class="sxs-lookup"><span data-stu-id="896e9-121">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="896e9-122">A következő partner alapértelmezés szerint nem kap rendszergazdai jogosultságot a nevében (AOBO).</span><span class="sxs-lookup"><span data-stu-id="896e9-122">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="896e9-123">A harmadik féltől származó Marketplace-termékek akkor lesznek áthozva, ha a termékek megfelelnek a Marketplace-jogosultságellenőrzésen.</span><span class="sxs-lookup"><span data-stu-id="896e9-123">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="896e9-124">Nincsenek különleges kedvezmények vagy regionális korlátozások</span><span class="sxs-lookup"><span data-stu-id="896e9-124">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="896e9-125">A termékek nem előfizetésen alapulnak</span><span class="sxs-lookup"><span data-stu-id="896e9-125">The products are non-subscription based</span></span>
    - <span data-ttu-id="896e9-126">A jövőbeli partnernek együtt kell működnie a közzétevővel, hogy biztosan fel legyen sorolva a termék üzembe helyezésének engedélyezése listában</span><span class="sxs-lookup"><span data-stu-id="896e9-126">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="896e9-127">Ha nem teljesül az összes feltétel a Marketplace-termékek átviteléhez, az Azure-előfizetések átadása, majd a Marketplace-termékek újravásárlása az új partnerrel</span><span class="sxs-lookup"><span data-stu-id="896e9-127">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="896e9-128">**Előfeltételek:**</span><span class="sxs-lookup"><span data-stu-id="896e9-128">**Prerequisites:**</span></span>

- <span data-ttu-id="896e9-129">Az ügyfél kapcsolatba fog lépjen a jelenlegi CSP-partnerrel az átállás szándéka alapján</span><span class="sxs-lookup"><span data-stu-id="896e9-129">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="896e9-130">A jövőbeli CSP-partner az ügyféllel együtt gondoskodik az ügyfelek igényeinek kielégítése érdekében</span><span class="sxs-lookup"><span data-stu-id="896e9-130">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="896e9-131">A jövőbeli CSP-partner kapcsolatot létesít az ügyféllel, és megvásárol egy Azure-tervet az átállás megkezdése előtt</span><span class="sxs-lookup"><span data-stu-id="896e9-131">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="896e9-132">Az ügyfélnek Microsoft Ügyfélszerződés CSP-partnerrel kell bejelentkeznie</span><span class="sxs-lookup"><span data-stu-id="896e9-132">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="896e9-133">A későbbi CSP-partnernek alá kell írnia a Microsoft Partnerszerződés az eszköz használatára</span><span class="sxs-lookup"><span data-stu-id="896e9-133">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="896e9-134">Teljesítenünk kell az ügyfélfeladatokat</span><span class="sxs-lookup"><span data-stu-id="896e9-134">Customer tasks to be completed</span></span>

<span data-ttu-id="896e9-135">Azure-előfizetés Azure-csomag keretében történő átviteléhez az ügyfélnek el kell kezdenie a folyamatot az aktuális partnerével való kapcsolatfelvétellel.</span><span class="sxs-lookup"><span data-stu-id="896e9-135">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="896e9-136">Össze kell gyűjteniük jelenlegi partnerük vállalatnevét és tartományát, hogy a jövőbeli partnerük a nevükben ki tudja egészlatni az átadási kérelem űrlapját.</span><span class="sxs-lookup"><span data-stu-id="896e9-136">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="896e9-137">Az ügyfélnek azonosítania kell azokat az előfizetéseket is, amelyek átadása az aktuális partnertől lehetséges.</span><span class="sxs-lookup"><span data-stu-id="896e9-137">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="896e9-138">Nem módosíthatja az Office 365-, Nagyvállalati mobilitási csomag- vagy Microsoft Dynamics CRM-előfizetések partnerét.</span><span class="sxs-lookup"><span data-stu-id="896e9-138">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="896e9-139">A jövőbeli partner felelőssége, hogy töltse ki az átadási kérelem űrlapját, amely elindítja az átadási folyamatot.</span><span class="sxs-lookup"><span data-stu-id="896e9-139">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="896e9-140">A Microsoft nem avatkozhat be az ügyfél vagy az aktuális partner nevében.</span><span class="sxs-lookup"><span data-stu-id="896e9-140">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="896e9-141">Az ügyfélnek szorosan együtt kell működnie a jövőbeli és a jelenlegi partnerrel, hogy zökkenőmentesen működjön az átállás.</span><span class="sxs-lookup"><span data-stu-id="896e9-141">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="896e9-142">A jövőbeli befejezendő partnerfeladatok</span><span class="sxs-lookup"><span data-stu-id="896e9-142">Future partner tasks to be completed</span></span>

<span data-ttu-id="896e9-143">Az előfizetés jövőbeli partnerének ki kell kitöltötte az átadási kérelem űrlapát a Partnerközpont az előfizetés átvitelének igényléséhez:</span><span class="sxs-lookup"><span data-stu-id="896e9-143">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="896e9-144">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, aki nevében el szeretné látni az átadási kérelem űrlapját.</span><span class="sxs-lookup"><span data-stu-id="896e9-144">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="896e9-145">Az Ügyfél menüben válassza az **Előfizetések lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="896e9-145">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="896e9-146">Válassza az **Átadási kérelem szakaszt.**</span><span class="sxs-lookup"><span data-stu-id="896e9-146">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="896e9-147">Az **Átadási kérelem szakaszban válassza** az **Új kérelem hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="896e9-147">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Átvitelek szakasz":::

5.  <span data-ttu-id="896e9-149">Töltse ki **az Új átadási kérelem űrlapot.**</span><span class="sxs-lookup"><span data-stu-id="896e9-149">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="896e9-150">Válassza az **Átadási kérelem küldése**  >  **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="896e9-150">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Átadási kérelem kitöltése űrlap":::

7.  <span data-ttu-id="896e9-152">Átadási kérelem megerősítésének áttekintése</span><span class="sxs-lookup"><span data-stu-id="896e9-152">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Függőben lévő átvitel áttekintése":::

    >[!Note]
    ><span data-ttu-id="896e9-154">A jövőbeli partner csak akkor  szakíthatja meg az átadási kérelmet, ha a jobb felső sarokban a Kérelem visszavonása gombra választ, ha az átadási kérelem állapota "Függőben".</span><span class="sxs-lookup"><span data-stu-id="896e9-154">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="896e9-155">Ha az átadási kérelem állapota "folyamatban" vagy "kész", a megszakítások nem lesznek lehetségesek.</span><span class="sxs-lookup"><span data-stu-id="896e9-155">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="896e9-156">Jelenleg teljesítenünk kell a partneri feladatokat</span><span class="sxs-lookup"><span data-stu-id="896e9-156">Current partner tasks to be completed</span></span>

<span data-ttu-id="896e9-157">Az ügyfél aktuális partnerének rendszergazdai ügynöke e-mailt fog kapni arról, hogy az ügyfél az előfizetések átvitelét kéri:</span><span class="sxs-lookup"><span data-stu-id="896e9-157">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Áttekintés":::

<span data-ttu-id="896e9-159">Tekintse át és fogadja el az átadási kérelem űrlapját Partnerközpont előfizetés átvitelének befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="896e9-159">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="896e9-160">Ha az aktuális partner 30 napon belül nem hoz létre semmilyen műveletet, a kérelem lejár, és a jövőbeli partnernek lesz egy új átadási kérése.</span><span class="sxs-lookup"><span data-stu-id="896e9-160">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="896e9-161">Válassza **az Átadási kérelem áttekintése lehetőséget** az e-mailből VAGY</span><span class="sxs-lookup"><span data-stu-id="896e9-161">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="896e9-162">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, aki nevében elküldött egy átadási kérelmet.</span><span class="sxs-lookup"><span data-stu-id="896e9-162">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="896e9-163">Az Ügyfél menüben válassza az **Előfizetések lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="896e9-163">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="896e9-164">Válassza az **Átadási kérelem szakaszt.**</span><span class="sxs-lookup"><span data-stu-id="896e9-164">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="896e9-165">Bontsa ki az átadási adatokat a kiválasztott **átadási kérelem azonosítójának kiválasztásával a** **Fogadott kérések alatt**</span><span class="sxs-lookup"><span data-stu-id="896e9-165">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Forrás-felülvizsgálatok átadási kérése":::

5.  <span data-ttu-id="896e9-167">Tekintse át az átadási kérelmet.</span><span class="sxs-lookup"><span data-stu-id="896e9-167">Review transfer request.</span></span> <span data-ttu-id="896e9-168">Válassza ki az átvitelhez kért Azure-előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="896e9-168">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="896e9-169">Mielőtt továbblépne, vegye figyelembe, hogy a továbbiakban nem fog hozzáférni a kiválasztott előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="896e9-169">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="896e9-170">A további használatért nem lesz számlázva.</span><span class="sxs-lookup"><span data-stu-id="896e9-170">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="896e9-171">Az Azure-foglalások nem átvitele az előfizetésekkel együtt.</span><span class="sxs-lookup"><span data-stu-id="896e9-171">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="896e9-172">Ezután válassza **az Elfogadás és átvitel lehetőséget** az átviteli folyamat befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="896e9-172">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Válassza ki az Azure-csomagokban átvihető előfizetéseket":::

7.  <span data-ttu-id="896e9-174">Az átadás elfogadásának megerősítésének megtekintése.</span><span class="sxs-lookup"><span data-stu-id="896e9-174">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="896e9-175">Ezen a ponton a jövőbeli partner, az ügyfél és az aktuális partner e-mailben értesítést kap az elfogadott átadási kérelemről.</span><span class="sxs-lookup"><span data-stu-id="896e9-175">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="896e9-176">Az átváltás elfogadott állapota akár 15 percig is függőben maradhat a rendszer frissítése közben.</span><span class="sxs-lookup"><span data-stu-id="896e9-176">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="896e9-177">Ha ez hosszabb időt vesz igénybe, a rendszer három napig próbálkozik.</span><span class="sxs-lookup"><span data-stu-id="896e9-177">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="896e9-178">Ha az átvitel állapota továbbra is Függőben marad, a partnernek be kell nyújtania egy szolgáltatáskérést.</span><span class="sxs-lookup"><span data-stu-id="896e9-178">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="896e9-179">Az átvitel befejezése után a kérésben szereplő előfizetések megjelennek a jövőbeli partner Azure-csomagja alatt, és a továbbiakban nem lesznek felsorolva.</span><span class="sxs-lookup"><span data-stu-id="896e9-179">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="896e9-180">Közvetett szolgáltatók esetén: Tájékoztassa a közvetett viszonteladót arról, hogy az átadási kérelem el lett fogadva.</span><span class="sxs-lookup"><span data-stu-id="896e9-180">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="896e9-181">Az átvitt ügyfél-előfizetések kezelése</span><span class="sxs-lookup"><span data-stu-id="896e9-181">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="896e9-182">A meglévő felhasználók, csoportok vagy szolgáltatásnevek hozzáféréseire, amelyek az Azure szerepköralapú hozzáférés-vezérlés (RBAC) segítségével lettek hozzárendelve, a váltás nincs hatással.</span><span class="sxs-lookup"><span data-stu-id="896e9-182">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="896e9-183">Az Azure szerepköralapú hozzáférés-vezérlés [(Azure RBAC)](/azure/role-based-access-control/overview) segítségével az ügyfelek kezelhetik, hogy ki férhet hozzá az Azure-erőforrásokhoz, mire használhatja őket, és milyen területekhez férhetnek hozzá.</span><span class="sxs-lookup"><span data-stu-id="896e9-183">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="896e9-184">Új partnerként nem kap RBAC-hozzáférést az ügyfél erőforrásaihoz az előfizetés átvitele után.</span><span class="sxs-lookup"><span data-stu-id="896e9-184">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="896e9-185">Az ügyfél korábbi partnere megtartja RBAC-hozzáférését.</span><span class="sxs-lookup"><span data-stu-id="896e9-185">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="896e9-186">Az ügyféllel együtt értse meg, hogy ki kaphat betekintést az előfizetéseibe, és hogyan lehet bármilyen módosítást tenni.</span><span class="sxs-lookup"><span data-stu-id="896e9-186">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="896e9-187">Ezért fontos, hogy az ügyfél eltávolítsa az Azure RBAC-hozzáférést a korábbi partnertől, és hozzáférést adjon hozzá az új partnerhez.</span><span class="sxs-lookup"><span data-stu-id="896e9-187">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="896e9-188">Az új hozzáférést adó ügyféllel kapcsolatos további információkért lásd: [Mi az az Azure szerepköralapú hozzáférés-vezérlés (Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="896e9-188">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="896e9-189">Az előző partner RBAC-hozzáférésének eltávolításával kapcsolatos további információkért [lásd: Szerepkör-hozzárendelés eltávolítása.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)</span><span class="sxs-lookup"><span data-stu-id="896e9-189">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="896e9-190">Emellett nem kap automatikusan rendszergazdai hozzáférést az előfizetései [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) nevében.</span><span class="sxs-lookup"><span data-stu-id="896e9-190">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="896e9-191">Az AOBO szükséges ahhoz, hogy a partnerek a nevükben kezelték az ügyfél Azure-előfizetését.</span><span class="sxs-lookup"><span data-stu-id="896e9-191">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="896e9-192">Az Azure-jogosultságokkal kapcsolatos további információkért lásd: Ügyfél szolgáltatásának vagy előfizetésének kezeléséhez szükséges [engedélyek beszerzése.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="896e9-192">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="896e9-193">Következő lépések:</span><span class="sxs-lookup"><span data-stu-id="896e9-193">Next steps:</span></span>

- [<span data-ttu-id="896e9-194">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="896e9-194">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="896e9-195">Engedélyek beszerzése egy ügyfél szolgáltatásának vagy előfizetésének kezeléséhez.</span><span class="sxs-lookup"><span data-stu-id="896e9-195">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
