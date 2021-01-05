---
title: Azure-előfizetés átvitele egy Azure-csomagból egy másik CSP-partnerbe
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan változtathatja meg egy Azure-csomag keretében az ügyfél Azure-előfizetéséhez társított felhőalapú megoldás-szolgáltatói partnert.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e792e4af2999924ba8be77ec0517ce56c1db7a27
ms.sourcegitcommit: ed5c873d19f0464cc986fe6e852383cd4280daf6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/05/2021
ms.locfileid: "97893206"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="29d8a-103">Ügyfél Azure-csomag-előfizetésének átvitele egy másik partnerre</span><span class="sxs-lookup"><span data-stu-id="29d8a-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="29d8a-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="29d8a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="29d8a-105">Partnerek a Cloud Solution Provider (CSP) programban</span><span class="sxs-lookup"><span data-stu-id="29d8a-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="29d8a-106">Ez a cikk azt ismerteti, hogy az ügyfél hogyan válthat az Azure-előfizetések között egy felhőalapú megoldás-szolgáltató (CSP) között egy másikra.</span><span class="sxs-lookup"><span data-stu-id="29d8a-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="29d8a-107">Az ügyfél Azure-előfizetésének egy másik partnertől való átváltásához kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="29d8a-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="29d8a-108">A partner és az ügyfél is elvégezheti a szükséges lépéseket.</span><span class="sxs-lookup"><span data-stu-id="29d8a-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="29d8a-109">Csak a Microsofttal közvetlen számlázási kapcsolattal rendelkező partnerek férhetnek hozzá az áttérési eszközökhöz.</span><span class="sxs-lookup"><span data-stu-id="29d8a-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="29d8a-110">A közvetett viszonteladóknak működniük kell a közvetett szolgáltatókkal az áttérési eszköz kihasználása érdekében.</span><span class="sxs-lookup"><span data-stu-id="29d8a-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="29d8a-111">Az ügyfélnek az eszköz kihasználása előtt mindkét partnerrel (aktuális és jövőbeli) kell kommunikálnia.</span><span class="sxs-lookup"><span data-stu-id="29d8a-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="29d8a-112">Az offline beszélgetéseknek el kell kerülniük a félreértések és a forgalom elkerülését.</span><span class="sxs-lookup"><span data-stu-id="29d8a-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="29d8a-113">Emellett a partnereknek és az ügyfeleknek meg kell érteniük ezeket a szempontokat és előfeltételeket az áttérés megkezdése előtt:</span><span class="sxs-lookup"><span data-stu-id="29d8a-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="29d8a-114">**Legfontosabb szempontok:**</span><span class="sxs-lookup"><span data-stu-id="29d8a-114">**Key considerations:**</span></span>

- <span data-ttu-id="29d8a-115">A Azure Reservations nem kerül át az előfizetésbe a jövőbeli partnernek</span><span class="sxs-lookup"><span data-stu-id="29d8a-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="29d8a-116">A jelenlegi partnernél az Azure-szolgáltatások CSP-díjszabása nem fog áttérni</span><span class="sxs-lookup"><span data-stu-id="29d8a-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="29d8a-117">Az ügyfél támogatási feladatai a jövőbeli partnernek lesznek áthelyezve</span><span class="sxs-lookup"><span data-stu-id="29d8a-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="29d8a-118">A számlázás és a számlázás a jövőbeli partnernek az átvitel időpontjában kerül át</span><span class="sxs-lookup"><span data-stu-id="29d8a-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="29d8a-119">Az átvitel nem érinti az Azure Role-Based Access Controlt (RBAC)</span><span class="sxs-lookup"><span data-stu-id="29d8a-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="29d8a-120">Alapértelmezés szerint a (z) (AOBO) rendszergazdai nevében nem adható meg a jövőbeli partner</span><span class="sxs-lookup"><span data-stu-id="29d8a-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="29d8a-121">A harmadik féltől származó Piactéri termékek addig lesznek továbbítva, amíg a termékek átadják a piactér jogosultsági ellenőrzését.</span><span class="sxs-lookup"><span data-stu-id="29d8a-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="29d8a-122">Nincsenek különleges kedvezmények vagy regionális korlátozások</span><span class="sxs-lookup"><span data-stu-id="29d8a-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="29d8a-123">A termékek nem előfizetésen alapulnak</span><span class="sxs-lookup"><span data-stu-id="29d8a-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="29d8a-124">A jövőbeli partnernek együtt kell működnie a közzétevővel annak ellenőrzéséhez, hogy az engedélyezési listán vannak-e a termék telepítéséhez</span><span class="sxs-lookup"><span data-stu-id="29d8a-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="29d8a-125">Ha a piactér-termékek átadásához nem teljesülnek az összes feltétel, akkor az Azure-előfizetések át lesznek adva, majd a piactér-termékek újravásárlása az új partnerrel</span><span class="sxs-lookup"><span data-stu-id="29d8a-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="29d8a-126">**Előfeltételek:**</span><span class="sxs-lookup"><span data-stu-id="29d8a-126">**Prerequisites:**</span></span>

- <span data-ttu-id="29d8a-127">Az ügyfél az aktuális CSP-partnert az áttérés céljára irányítja</span><span class="sxs-lookup"><span data-stu-id="29d8a-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="29d8a-128">A jövőbeli CSP-partner az ügyféllel együttműködve biztosítja az ügyfelek igényeinek teljesítését</span><span class="sxs-lookup"><span data-stu-id="29d8a-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="29d8a-129">A jövőbeli CSP-partner kapcsolatot létesít az ügyféllel, és megvásárol egy Azure-csomagot az áttérés megkezdése előtt</span><span class="sxs-lookup"><span data-stu-id="29d8a-129">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="29d8a-130">Az ügyfélnek regisztrálnia kell a Microsoft ügyfél-szerződést a jövőbeli CSP-partnerrel</span><span class="sxs-lookup"><span data-stu-id="29d8a-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="29d8a-131">A jövőbeli CSP-partnernek alá kell írnia a Microsoft partneri szerződést az eszköz használatához</span><span class="sxs-lookup"><span data-stu-id="29d8a-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="29d8a-132">Elvégzendő felhasználói feladatok</span><span class="sxs-lookup"><span data-stu-id="29d8a-132">Customer tasks to be completed</span></span>

<span data-ttu-id="29d8a-133">Ha Azure-csomag keretében szeretne Azure-előfizetést továbbítani, az ügyfélnek a jelenlegi partnerével kell megindítania a folyamatot.</span><span class="sxs-lookup"><span data-stu-id="29d8a-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="29d8a-134">Össze kell gyűjteniük az aktuális partnere vállalatának nevét és tartományát, hogy a jövőbeli partnerük az adatátviteli kérelem űrlapját a nevében tudja befejezni.</span><span class="sxs-lookup"><span data-stu-id="29d8a-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="29d8a-135">Az ügyfélnek továbbá azonosítania kell az aktuális partnertől átvinni kívánt előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="29d8a-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="29d8a-136">Az Office 365, a nagyvállalati mobilitási csomag vagy a Microsoft Dynamics CRM-előfizetések partnerei nem változtathatók meg.</span><span class="sxs-lookup"><span data-stu-id="29d8a-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="29d8a-137">A jövőbeli partner feladata az adatátviteli kérelem űrlapjának elvégzése, amely elindítja az átvitel folyamatát.</span><span class="sxs-lookup"><span data-stu-id="29d8a-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="29d8a-138">A Microsoft nem tud beavatkozni az ügyfél vagy az aktuális partner nevében.</span><span class="sxs-lookup"><span data-stu-id="29d8a-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="29d8a-139">Az ügyfélnek meg kell terveznie, hogy a jövőben zökkenőmentesen működjön együtt a jövőbeli és a jelenlegi partnerével.</span><span class="sxs-lookup"><span data-stu-id="29d8a-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="29d8a-140">A jövőbeli partneri feladatok elvégzése</span><span class="sxs-lookup"><span data-stu-id="29d8a-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="29d8a-141">Az előfizetés jövőbeli partnerének el kell végeznie egy átadási kérelem űrlapját a partner Centertől az előfizetés átadásának igényléséhez:</span><span class="sxs-lookup"><span data-stu-id="29d8a-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="29d8a-142">A partner Center menüjében válassza az **ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, aki az átadási kérelem űrlapját a nevében szeretné végrehajtani.</span><span class="sxs-lookup"><span data-stu-id="29d8a-142">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="29d8a-143">Az ügyfél menüben válassza az **előfizetések** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="29d8a-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="29d8a-144">Válassza az **átviteli kérelem** szakaszt.</span><span class="sxs-lookup"><span data-stu-id="29d8a-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="29d8a-145">Az **átadási kérelem szakaszban** válassza az **új kérelem hozzáadása** elemet.</span><span class="sxs-lookup"><span data-stu-id="29d8a-145">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Átvitelek szakasz":::

5.  <span data-ttu-id="29d8a-147">Fejezze be az **új adatátviteli kérés** űrlapot.</span><span class="sxs-lookup"><span data-stu-id="29d8a-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="29d8a-148">Válassza az **átvitel küldése kérelem**  >  **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="29d8a-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Adatátviteli kérelem űrlapjának befejezése":::

7.  <span data-ttu-id="29d8a-150">Átmozgatási kérelem megerősítése</span><span class="sxs-lookup"><span data-stu-id="29d8a-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Ellenőrzés függőben":::

    >[!Note]
    ><span data-ttu-id="29d8a-152">A jövőbeli partner megszakíthatja az adatátviteli kérést a jobb felső sarokban lévő **kérelem megszakítása** lehetőség kiválasztásával, ha az átadási kérelem állapota "függőben van".</span><span class="sxs-lookup"><span data-stu-id="29d8a-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="29d8a-153">Ha az átviteli kérelem állapota "folyamatban" vagy "kész", a lemondások nem lesznek lehetségesek.</span><span class="sxs-lookup"><span data-stu-id="29d8a-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="29d8a-154">Az aktuálisan elvégzendő partneri feladatok</span><span class="sxs-lookup"><span data-stu-id="29d8a-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="29d8a-155">Az ügyfél a jelenlegi partner rendszergazdai ügynöke egy e-mailt kap arról, hogy az ügyfél az előfizetésük átvitelét kéri:</span><span class="sxs-lookup"><span data-stu-id="29d8a-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Áttekintés":::

<span data-ttu-id="29d8a-157">Tekintse át és fogadja el az adatátviteli kérés űrlapot a partner Centertől az előfizetés átvitelének befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="29d8a-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="29d8a-158">Ha a jelenlegi partner semmilyen műveletet nem végez a kérés érvényességét követő 30 napon belül, és a jövőbeli partner egy új adatátviteli kérést fog létrehozni.</span><span class="sxs-lookup"><span data-stu-id="29d8a-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="29d8a-159">Válassza az **átadási kérelem megtekintése** az e-mailben vagy a</span><span class="sxs-lookup"><span data-stu-id="29d8a-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="29d8a-160">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, akinek a nevében elküldte az átadási kérelmet.</span><span class="sxs-lookup"><span data-stu-id="29d8a-160">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="29d8a-161">Az ügyfél menüben válassza az **előfizetések** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="29d8a-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="29d8a-162">Válassza az **átviteli kérelem** szakaszt.</span><span class="sxs-lookup"><span data-stu-id="29d8a-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="29d8a-163">Az átadási adatok kibontása a kiválasztott **átadási kérelem azonosítójának** kiválasztásával a **fogadott kérelmek** között</span><span class="sxs-lookup"><span data-stu-id="29d8a-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Forrás-felülvizsgálati kérelem átvitele":::

5.  <span data-ttu-id="29d8a-165">Átmozgatási kérelem áttekintése.</span><span class="sxs-lookup"><span data-stu-id="29d8a-165">Review transfer request.</span></span> <span data-ttu-id="29d8a-166">Válassza ki az átvinni kívánt Azure-előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="29d8a-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="29d8a-167">A továbblépés előtt vegye figyelembe, hogy a továbbiakban nem fog tudni hozzáférni a kijelölt előfizetésekhez.</span><span class="sxs-lookup"><span data-stu-id="29d8a-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="29d8a-168">A további használatra nem lesz számlázva.</span><span class="sxs-lookup"><span data-stu-id="29d8a-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="29d8a-169">Az Azure-foglalások nem vihetők át az előfizetésekre.</span><span class="sxs-lookup"><span data-stu-id="29d8a-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="29d8a-170">Ezután válassza az **elfogadás és az átvitel** lehetőséget az adatátviteli folyamat befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="29d8a-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Válassza ki az Azure-csomagok alá továbbítandó előfizetéseket":::

7.  <span data-ttu-id="29d8a-172">Az átvitel elfogadási megerősítésének megtekintése.</span><span class="sxs-lookup"><span data-stu-id="29d8a-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="29d8a-173">Ezen a ponton a jövőbeli partner, az ügyfél és a jelenlegi partner értesítést kap az elfogadott átküldési kérelemről e-mailben.</span><span class="sxs-lookup"><span data-stu-id="29d8a-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="29d8a-174">Az áttérés elfogadását követően az átvitel állapota akár 15 percet is igénybe vehet, amíg a rendszer frissül.</span><span class="sxs-lookup"><span data-stu-id="29d8a-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="29d8a-175">Ha a rendszer továbbra is tart, a rendszer három napig próbálkozik.</span><span class="sxs-lookup"><span data-stu-id="29d8a-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="29d8a-176">Ha az átvitel állapota továbbra is függőben van, a partnernek be kell küldenie egy szolgáltatási kérelmet.</span><span class="sxs-lookup"><span data-stu-id="29d8a-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="29d8a-177">Az átvitel befejezése után a kérelemben foglalt előfizetések megjelennek a jövőbeli partner Azure-tervében, és már nem jelennek meg Önnel.</span><span class="sxs-lookup"><span data-stu-id="29d8a-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="29d8a-178">Közvetett szolgáltatók esetén: Kérjük, tájékoztassa a közvetett viszonteladót arról, hogy az átadási kérelem el lett fogadva.</span><span class="sxs-lookup"><span data-stu-id="29d8a-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="29d8a-179">Az átvitt ügyfél-előfizetések kezelése</span><span class="sxs-lookup"><span data-stu-id="29d8a-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="29d8a-180">A meglévő felhasználók, csoportok vagy szolgáltatásnevek hozzáféréseire, amelyek az Azure szerepköralapú hozzáférés-vezérlés (RBAC) segítségével lettek hozzárendelve, a váltás nincs hatással.</span><span class="sxs-lookup"><span data-stu-id="29d8a-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="29d8a-181">Az Azure szerepköralapú hozzáférés-vezérlés [(Azure RBAC)](/azure/role-based-access-control/overview) segítségével az ügyfelek felügyelhetik, hogy ki férhet hozzá az Azure-erőforrásokhoz, mit tehetnek ezekkel az erőforrásokkal, és milyen területekhez férnek hozzá.</span><span class="sxs-lookup"><span data-stu-id="29d8a-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="29d8a-182">Az új partnerként nem kap RBAC hozzáférést az ügyfél erőforrásaihoz az előfizetés átvitele után.</span><span class="sxs-lookup"><span data-stu-id="29d8a-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="29d8a-183">Az ügyfél korábbi partnere megtartja a RBAC-hozzáférését.</span><span class="sxs-lookup"><span data-stu-id="29d8a-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="29d8a-184">Az ügyféllel együttműködve megismerheti, hogy kik betekintést nyújtanak az előfizetésbe, és hogyan teheti meg a kívánt módosításokat.</span><span class="sxs-lookup"><span data-stu-id="29d8a-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="29d8a-185">Ezért fontos, hogy az ügyfél eltávolítsa az Azure RBAC-hozzáférést az előző partnerhez, és hozzá lehessen férni az új partnerhez.</span><span class="sxs-lookup"><span data-stu-id="29d8a-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="29d8a-186">További információ az ügyfél új hozzáféréséről: [Mi az az Azure szerepköralapú hozzáférés-vezérlés (Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="29d8a-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="29d8a-187">További információ az előző partner RBAC-hozzáférésének eltávolításáról: [szerepkör-hozzárendelés eltávolítása](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="29d8a-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="29d8a-188">Emellett nem kap automatikusan rendszergazdai jogosultságot az előfizetések nevében [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) .</span><span class="sxs-lookup"><span data-stu-id="29d8a-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="29d8a-189">Ahhoz, hogy a partner felügyelje ügyfele Azure-előfizetéseit az Ön nevében, az AOBO szükséges.</span><span class="sxs-lookup"><span data-stu-id="29d8a-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="29d8a-190">További információ az Azure-jogosultságokról: az [ügyfél szolgáltatásának vagy előfizetésének kezeléséhez szükséges engedélyek beszerzése.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="29d8a-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="29d8a-191">Következő lépések:</span><span class="sxs-lookup"><span data-stu-id="29d8a-191">Next steps:</span></span>

- [<span data-ttu-id="29d8a-192">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="29d8a-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="29d8a-193">Az ügyfél szolgáltatásának vagy előfizetésének kezeléséhez szükséges engedélyek beszerzése.</span><span class="sxs-lookup"><span data-stu-id="29d8a-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
