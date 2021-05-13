---
title: Azure-előfizetés átvitele Azure-csomag keretében egy másik CSP-partnernek
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan módosíthatja Felhőszolgáltató ügyfél Azure-előfizetéséhez társított programpartnert egy Azure-csomag keretében.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856049"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="9f5fc-103">Az ügyfél Azure-csomag előfizetésének átvitele egy másik partnernek</span><span class="sxs-lookup"><span data-stu-id="9f5fc-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="9f5fc-104">**Megfelelő szerepkörök:** Fiók-rendszergazdai | Értékesítési ügynök | Számlázási ügynök</span><span class="sxs-lookup"><span data-stu-id="9f5fc-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="9f5fc-105">Ez a cikk azt ismerteti, hogy az ügyfelek hogyan válthatnak Azure-előfizetéseik között egy Azure-Felhőszolgáltató (CSP) egy másikra.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="9f5fc-106">Ha egy ügyfél Azure-előfizetéseit egy másik partnerről is át kell váltania, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="9f5fc-107">A partnernek és az ügyfélnek is vannak lépései.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="9f5fc-108">Csak a Microsofttal közvetlen számlázási kapcsolatban áll partnerek férhetnek hozzá az átváltási eszközökhez.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="9f5fc-109">A közvetett viszonteladóknak a közvetett szolgáltatóikkal együtt kell használniuk ezt az átváltási eszközt.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="9f5fc-110">Az ügyfélnek az eszköz használata előtt mindkét partnerrel (aktuális és jövőbeli) párbeszédben kell lennie.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="9f5fc-111">A félreértések és adatváltozások elkerülése érdekében offline beszélgetésre van szükség.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="9f5fc-112">Emellett a partnereknek és az ügyfeleknek az átállás megkezdése előtt meg kell érteniük ezeket a szempontokat és előfeltételeket:</span><span class="sxs-lookup"><span data-stu-id="9f5fc-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="9f5fc-113">**Fő szempontok:**</span><span class="sxs-lookup"><span data-stu-id="9f5fc-113">**Key considerations:**</span></span>

- <span data-ttu-id="9f5fc-114">Az Azure Reservations nem lesz áthelyezve az előfizetéssel a jövőbeli partnerhez</span><span class="sxs-lookup"><span data-stu-id="9f5fc-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="9f5fc-115">Az aktuális partnerhez az Azure-szolgáltatások CSP-díjszabása nem fog áttérni</span><span class="sxs-lookup"><span data-stu-id="9f5fc-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="9f5fc-116">Az ügyfél támogatási feladatai a jövőbeli partnerhez fognak átköltözni</span><span class="sxs-lookup"><span data-stu-id="9f5fc-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="9f5fc-117">A számlázás és a számlázás az átadáskor át fog költözni a jövőbeli partnerhez</span><span class="sxs-lookup"><span data-stu-id="9f5fc-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="9f5fc-118">Az azure Role-Based Access Control (RBAC) nincs hatással az átvitelre</span><span class="sxs-lookup"><span data-stu-id="9f5fc-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="9f5fc-119">A következő partner alapértelmezés szerint nem kap rendszergazdai jogosultságot a nevében (AOBO).</span><span class="sxs-lookup"><span data-stu-id="9f5fc-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="9f5fc-120">A harmadik féltől származó Marketplace-termékek akkor lesznek áthozva, ha a termékek megfelelnek a Marketplace-jogosultságellenőrzésen.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="9f5fc-121">Nincsenek különleges kedvezmények vagy regionális korlátozások</span><span class="sxs-lookup"><span data-stu-id="9f5fc-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="9f5fc-122">A termékek nem előfizetésen alapulnak</span><span class="sxs-lookup"><span data-stu-id="9f5fc-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="9f5fc-123">A jövőbeli partnernek együtt kell működnie a közzétevővel, hogy biztosan fel legyen sorolva a termék üzembe helyezésének engedélyezései listájában</span><span class="sxs-lookup"><span data-stu-id="9f5fc-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="9f5fc-124">Ha nem teljesül az összes feltétel a Marketplace-termékek átviteléhez, az Azure-előfizetések átadása, majd a Marketplace-termékek újravásárlása az új partnerrel</span><span class="sxs-lookup"><span data-stu-id="9f5fc-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="9f5fc-125">**Előfeltételek:**</span><span class="sxs-lookup"><span data-stu-id="9f5fc-125">**Prerequisites:**</span></span>

- <span data-ttu-id="9f5fc-126">Az ügyfél kapcsolatba fog lépjen a jelenlegi CSP-partnerrel az áttérési szándéka miatt</span><span class="sxs-lookup"><span data-stu-id="9f5fc-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="9f5fc-127">A jövőbeli CSP-partner az ügyféllel együtt gondoskodik az ügyfelek igényeinek kielégítése érdekében</span><span class="sxs-lookup"><span data-stu-id="9f5fc-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="9f5fc-128">A jövőbeli CSP-partner kapcsolatot létesít az ügyféllel, és megvásárol egy Azure-tervet az átállás megkezdése előtt</span><span class="sxs-lookup"><span data-stu-id="9f5fc-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="9f5fc-129">Az ügyfélnek Microsoft Ügyfélszerződés CSP-partnerrel kell bejelentkeznie</span><span class="sxs-lookup"><span data-stu-id="9f5fc-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="9f5fc-130">A későbbi CSP-partnernek alá kell írnia a Microsoft Partnerszerződés az eszköz használatára</span><span class="sxs-lookup"><span data-stu-id="9f5fc-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="9f5fc-131">Teljesítenünk kell az ügyfélfeladatokat</span><span class="sxs-lookup"><span data-stu-id="9f5fc-131">Customer tasks to be completed</span></span>

<span data-ttu-id="9f5fc-132">Azure-előfizetés Azure-csomag keretében történő átviteléhez az ügyfélnek el kell kezdenie a folyamatot az aktuális partnerével való kapcsolatfelvétellel.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="9f5fc-133">Össze kell gyűjteniük az aktuális partnerük vállalatnevét és tartományát, hogy a jövőbeli partnerük befejezheti az átadási kérelem űrlapját a nevükben.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="9f5fc-134">Az ügyfélnek az aktuális partnertől átemelni kívánt előfizetéseket is azonosítania kell.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="9f5fc-135">Az Office 365, a Nagyvállalati mobilitási csomag vagy a Microsoft Dynamics CRM-előfizetések partnerét nem módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="9f5fc-136">A jövőbeli partner felelőssége, hogy töltse ki az átadási kérelem űrlapját, amely elindítja az átadási folyamatot.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="9f5fc-137">A Microsoft nem avatkozhat be az ügyfél vagy az aktuális partner nevében.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="9f5fc-138">Az ügyfélnek szorosan együtt kell működnie a jövőbeli és jelenlegi partnerével, hogy zökkenőmentesen működjön az átállás.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="9f5fc-139">A jövőben teljesítendő partnerfeladatok</span><span class="sxs-lookup"><span data-stu-id="9f5fc-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="9f5fc-140">Az előfizetés jövőbeli partnerének ki kell kitöltötte az átadási kérelem űrlapát a Partnerközpont az előfizetés átvitelének igényléséhez:</span><span class="sxs-lookup"><span data-stu-id="9f5fc-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="9f5fc-141">A Partnerközpont válassza a **Customers**(Ügyfelek) lehetőséget, majd válassza ki azt az ügyfelet, aki nevében el szeretné látni az átadási kérelem űrlapját.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="9f5fc-142">Az Ügyfél menüben válassza az **Előfizetések lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="9f5fc-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="9f5fc-143">Válassza az **Átadási kérelem szakaszt.**</span><span class="sxs-lookup"><span data-stu-id="9f5fc-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="9f5fc-144">Az **Átadási kérelem szakaszban válassza** az **Új kérelem hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="9f5fc-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Átvitelek szakasz":::

5.  <span data-ttu-id="9f5fc-146">Töltse ki **az Új átadási kérelem űrlapot.**</span><span class="sxs-lookup"><span data-stu-id="9f5fc-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="9f5fc-147">Válassza az **Átadási kérelem küldése**  >  **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="9f5fc-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Átadási kérelem kitöltése űrlap":::

7.  <span data-ttu-id="9f5fc-149">Az átadási kérelem megerősítésének áttekintése</span><span class="sxs-lookup"><span data-stu-id="9f5fc-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Függőben lévő átvitel áttekintése":::

    >[!Note]
    ><span data-ttu-id="9f5fc-151">A jövőbeli partner csak akkor  szakíthatja meg az átadási kérelmet, ha a jobb felső sarokban a Kérelem visszavonása gombra van kiválasztva, ha az átadási kérelem állapota "Függőben".</span><span class="sxs-lookup"><span data-stu-id="9f5fc-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="9f5fc-152">Ha az átadási kérelem állapota "folyamatban" vagy "kész", a megszakítások nem lesznek lehetségesek.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="9f5fc-153">Jelenleg befejezt partneri feladatok</span><span class="sxs-lookup"><span data-stu-id="9f5fc-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="9f5fc-154">Az ügyfél jelenlegi partnerének rendszergazdai ügynöke e-mailt fog kapni arról, hogy az ügyfél az előfizetések átvitelét kéri:</span><span class="sxs-lookup"><span data-stu-id="9f5fc-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Áttekintés":::

<span data-ttu-id="9f5fc-156">Tekintse át és fogadja el az átadási kérelem űrlapját a Partnerközpont az előfizetés átadásának befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="9f5fc-157">Ha az aktuális partner 30 napon belül nem hoz létre műveletet, a kérelem lejár, és a jövőbeli partnernek lesz egy művelete egy új átadási kérelem létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="9f5fc-158">Válassza **az Átadási kérelem áttekintése lehetőséget** az e-mailből VAGY</span><span class="sxs-lookup"><span data-stu-id="9f5fc-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="9f5fc-159">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, aki nevében átadási kérelem lett elküldve.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="9f5fc-160">Az Ügyfél menüben válassza az **Előfizetések lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="9f5fc-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="9f5fc-161">Válassza az **Átadási kérelem szakaszt.**</span><span class="sxs-lookup"><span data-stu-id="9f5fc-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="9f5fc-162">Bontsa ki az átadási adatokat a kiválasztott átadási kérelem **azonosítójának kiválasztásával** a **Fogadott kérelmek alatt**</span><span class="sxs-lookup"><span data-stu-id="9f5fc-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Forrás-felülvizsgálatok átadási kérése":::

5.  <span data-ttu-id="9f5fc-164">Tekintse át az átadási kérelmet.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-164">Review transfer request.</span></span> <span data-ttu-id="9f5fc-165">Válassza ki a kért Azure-előfizetéseket az átvitelhez.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="9f5fc-166">Mielőtt továbblépne, vegye figyelembe, hogy a továbbiakban nem fog hozzáférni a kiválasztott előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="9f5fc-167">További használatra nem lesz kiszámlázva.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="9f5fc-168">Az Azure-foglalások nem átvitele az előfizetésekkel együtt.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="9f5fc-169">Ezután válassza **az Elfogadás és átvitel lehetőséget** az átviteli folyamat befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Válassza ki az Azure-csomagokban átvitt előfizetéseket":::

7.  <span data-ttu-id="9f5fc-171">Az átadás elfogadásának megerősítésének megtekintése.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="9f5fc-172">Ezen a ponton a jövőbeli partner, az ügyfél és az aktuális partner e-mailben értesítést kap az elfogadott átadási kérelemről.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="9f5fc-173">Az átváltás elfogadott állapota akár 15 percig is függőben maradhat a rendszer frissítése közben.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="9f5fc-174">Ha ez tovább tart, a rendszer három napig próbálkozik.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="9f5fc-175">Ha az átvitel állapota továbbra is Függőben marad, a partnernek be kell nyújtania egy szolgáltatáskérést.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="9f5fc-176">Az átvitel befejezése után a kérelemben foglalt előfizetések a jövőbeli partner Azure-csomagja alatt jelennek meg, és a továbbiakban nem lesznek felsorolva.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="9f5fc-177">Közvetett szolgáltatók esetén: Tájékoztassa közvetett viszonteladóját arról, hogy az átadási kérelem el lett fogadva.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="9f5fc-178">Az átvitt ügyfél-előfizetések kezelése</span><span class="sxs-lookup"><span data-stu-id="9f5fc-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="9f5fc-179">A meglévő felhasználók, csoportok vagy szolgáltatásnevek hozzáféréseire, amelyek az Azure szerepköralapú hozzáférés-vezérlés (RBAC) segítségével lettek hozzárendelve, a váltás nincs hatással.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="9f5fc-180">Az Azure szerepköralapú hozzáférés-vezérlés [(Azure RBAC)](/azure/role-based-access-control/overview) segítségével az ügyfelek kezelhetik, hogy ki férhet hozzá az Azure-erőforrásokhoz, mire használhatja őket, és milyen területekhez férhetnek hozzá.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="9f5fc-181">Új partnerként nem kap RBAC-hozzáférést az ügyfél erőforrásaihoz az előfizetés átvitele után.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="9f5fc-182">Az ügyfél korábbi partnere megtartja RBAC-hozzáférését.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="9f5fc-183">Az ügyféllel együtt értse meg, hogy ki kaphat betekintést az előfizetéseibe, és hogyan lehet bármilyen módosítást tenni.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="9f5fc-184">Ezért fontos, hogy az ügyfél eltávolítsa az Azure RBAC-hozzáférést a korábbi partnertől, és hozzáférést adjon hozzá az új partnerhez.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="9f5fc-185">Az új hozzáférést adó ügyféllel kapcsolatos további információkért lásd: Mi az [az Azure szerepköralapú hozzáférés-vezérlés (Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="9f5fc-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="9f5fc-186">Az előző partner RBAC-hozzáférésének eltávolításával kapcsolatos további információkért [lásd: Szerepkör-hozzárendelés eltávolítása.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)</span><span class="sxs-lookup"><span data-stu-id="9f5fc-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="9f5fc-187">Emellett nem kap automatikusan rendszergazdai hozzáférést [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) az előfizetéseihez.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="9f5fc-188">Az AOBO azért szükséges, hogy a partner az ügyfél Azure-előfizetését a nevükben kezelje.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="9f5fc-189">Az Azure-jogosultságokkal kapcsolatos további információkért lásd: Ügyfél szolgáltatásának vagy előfizetésének kezeléséhez szükséges [engedélyek beszerzése.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="9f5fc-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="9f5fc-190">Következő lépések:</span><span class="sxs-lookup"><span data-stu-id="9f5fc-190">Next steps:</span></span>

- [<span data-ttu-id="9f5fc-191">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="9f5fc-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="9f5fc-192">Szerezze be az ügyfél szolgáltatásának vagy előfizetésének kezeléséhez szükséges engedélyeket.</span><span class="sxs-lookup"><span data-stu-id="9f5fc-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
