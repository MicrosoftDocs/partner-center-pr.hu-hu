---
title: Március 2021 közlemények
description: Március 2021 közlemények a Microsoft partner Centerben, beleértve az új képességeket, promóciókat, ajánlatokat, piacokat vagy a meglévő ajánlatok változásait.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 5b8c5f52207a7b9a49d07885a36b61486be45497
ms.sourcegitcommit: 60bbb8f4056120264b769f94431f84d86984c2e9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/03/2021
ms.locfileid: "106280870"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="c15ad-103">Március 2021 közlemények</span><span class="sxs-lookup"><span data-stu-id="c15ad-103">March 2021 announcements</span></span>

<span data-ttu-id="c15ad-104">Ez az oldal a Microsoft partner Center 2021. márciusi hirdetményeit tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="c15ad-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="c15ad-105">A frissített CSP-ügyfél címe ellenőrzési API már elérhető teszteléshez</span><span class="sxs-lookup"><span data-stu-id="c15ad-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-106">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-106">Categories</span></span>

- <span data-ttu-id="c15ad-107">Dátum: 2021-03-31</span><span class="sxs-lookup"><span data-stu-id="c15ad-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="c15ad-108">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-109">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-109">Summary</span></span>

<span data-ttu-id="c15ad-110">Elkötelezettségünk részeként, hogy a partnerek és az ügyfelek a bizalmi kapcsolaton alapuló üzleti tevékenységet futtassák, a globális partnereket a ValidateAddress API változásainak tesztelésére fogjuk meghívni.</span><span class="sxs-lookup"><span data-stu-id="c15ad-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-111">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-111">Impacted audience</span></span>

<span data-ttu-id="c15ad-112">Minden CSP közvetlen számlás partner és olyan közvetett szolgáltató, aki új vagy meglévő ügyfél-címzési adatokat hoz létre vagy frissít</span><span class="sxs-lookup"><span data-stu-id="c15ad-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-113">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-113">Details</span></span>

<span data-ttu-id="c15ad-114">A Microsoft megbízhatósági kapcsolaton fut.</span><span class="sxs-lookup"><span data-stu-id="c15ad-114">Microsoft runs on trust.</span></span> <span data-ttu-id="c15ad-115">Elkötelezettek vagyunk abban, hogy megfelelő, biztonságos és biztonságos módszert biztosítanak az ügyfél-címek ellenőrzésének elküldéséhez az ügyfél-előfizetések átadásához a CSP programban.</span><span class="sxs-lookup"><span data-stu-id="c15ad-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="c15ad-116">Ma, 2021. március 31-én bevezetjük a ValidateAddress API-t, amelyet szeretnénk meghívni a 2021 tesztelésre.</span><span class="sxs-lookup"><span data-stu-id="c15ad-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="c15ad-117">Vegye figyelembe, hogy ezek a módosítások csak a ValidateAddress API-t érintik.</span><span class="sxs-lookup"><span data-stu-id="c15ad-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="c15ad-118">A CreateCustomer és a UpdateBillingProfile API-kat nem érinti a rendszer.</span><span class="sxs-lookup"><span data-stu-id="c15ad-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="c15ad-119">A válasz a következő állapotüzenetek egyikét fogja visszaadni:</span><span class="sxs-lookup"><span data-stu-id="c15ad-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="c15ad-120">Állapot</span><span class="sxs-lookup"><span data-stu-id="c15ad-120">Status</span></span> | <span data-ttu-id="c15ad-121">Leírás</span><span class="sxs-lookup"><span data-stu-id="c15ad-121">Description</span></span> | <span data-ttu-id="c15ad-122">A visszaadott javasolt címek száma</span><span class="sxs-lookup"><span data-stu-id="c15ad-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="c15ad-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="c15ad-123">VerifiedShippable</span></span> | <span data-ttu-id="c15ad-124">A címek ellenőrzése megtörtént, és a következőre küldhető:.</span><span class="sxs-lookup"><span data-stu-id="c15ad-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="c15ad-125">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="c15ad-125">Single</span></span> |
| <span data-ttu-id="c15ad-126">Ellenőrzött</span><span class="sxs-lookup"><span data-stu-id="c15ad-126">Verified</span></span> | <span data-ttu-id="c15ad-127">A címnek ellenőrzése megtörtént.</span><span class="sxs-lookup"><span data-stu-id="c15ad-127">Address is verified.</span></span> | <span data-ttu-id="c15ad-128">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="c15ad-128">Single</span></span> |
| <span data-ttu-id="c15ad-129">InteractionRequired</span><span class="sxs-lookup"><span data-stu-id="c15ad-129">InteractionRequired</span></span> | <span data-ttu-id="c15ad-130">A javasolt címek jelentősen módosultak, és felhasználói megerősítést igényelnek.</span><span class="sxs-lookup"><span data-stu-id="c15ad-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="c15ad-131">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="c15ad-131">Single</span></span> |
| <span data-ttu-id="c15ad-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="c15ad-132">StreetPartial</span></span> | <span data-ttu-id="c15ad-133">A címben megadott utca részleges, és további információra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="c15ad-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="c15ad-134">Több – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="c15ad-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="c15ad-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="c15ad-135">PremisesPartial</span></span> | <span data-ttu-id="c15ad-136">A megadott hely (építési szám, csomag száma stb.) részleges, és további információra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="c15ad-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="c15ad-137">Több – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="c15ad-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="c15ad-138">Többszörös</span><span class="sxs-lookup"><span data-stu-id="c15ad-138">Multiple</span></span> | <span data-ttu-id="c15ad-139">Több mező is van, amelyek részben szerepelnek a címben (potenciálisan a StreetPartial és a PremisesPartial is beleértve).</span><span class="sxs-lookup"><span data-stu-id="c15ad-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="c15ad-140">Több – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="c15ad-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="c15ad-141">Nincsenek</span><span class="sxs-lookup"><span data-stu-id="c15ad-141">None</span></span> | <span data-ttu-id="c15ad-142">A címe helytelen.</span><span class="sxs-lookup"><span data-stu-id="c15ad-142">Address is incorrect.</span></span> | <span data-ttu-id="c15ad-143">Nincsenek</span><span class="sxs-lookup"><span data-stu-id="c15ad-143">None</span></span> |
| <span data-ttu-id="c15ad-144">NotValidated</span><span class="sxs-lookup"><span data-stu-id="c15ad-144">NotValidated</span></span> | <span data-ttu-id="c15ad-145">A címeket nem sikerült elküldeni az érvényesítési folyamaton keresztül.</span><span class="sxs-lookup"><span data-stu-id="c15ad-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="c15ad-146">Nincsenek</span><span class="sxs-lookup"><span data-stu-id="c15ad-146">None</span></span> |

<span data-ttu-id="c15ad-147">Miután elküldte a címet a ValidateAddress API-val való ellenőrzésre, a rendszer a következő választ adja vissza:</span><span class="sxs-lookup"><span data-stu-id="c15ad-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="c15ad-148">Tekintse meg ezt a választ.</span><span class="sxs-lookup"><span data-stu-id="c15ad-148">Take a look at this sample response.</span></span> <span data-ttu-id="c15ad-149">Vegye figyelembe, hogy az Egyesült Államokban a válasz egy további négyjegyű utótagot ad vissza az irányítószám sorához, ha csak öt számjegyet ír be a zip-kódra.</span><span class="sxs-lookup"><span data-stu-id="c15ad-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp
// IAggregatePartner partnerOperations;
// string customerId;
// s{
"suggested_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Microsoft Way",
    "postal_Code": "98052-8300"
},
"original_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Micro Way",
    "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="c15ad-150">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-150">Next steps</span></span>

- <span data-ttu-id="c15ad-151">Ossza meg a homokozó bérlői AZONOSÍTÓját a test Flight (kis-és nagyvállalati) szakértővel, Ali khaki-val, hogy a tesztelési célú repülésben is szerepeljen, így elkezdheti a frissítés előkészítését.</span><span class="sxs-lookup"><span data-stu-id="c15ad-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="c15ad-152">Ha Vezérlőpult-gyártói (CPV) megoldást használ, tekintse meg a CPV-t.</span><span class="sxs-lookup"><span data-stu-id="c15ad-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-153">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-153">Questions?</span></span>

<span data-ttu-id="c15ad-154">Ha bármilyen kérdése van, vagy támogatásra van szüksége a Microsoft által végzett műveletekhez, forduljon a partner támogatási Yammer csoportjához.</span><span class="sxs-lookup"><span data-stu-id="c15ad-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="c15ad-155">Az új Exchange felügyeleti központ (EAC) felülete</span><span class="sxs-lookup"><span data-stu-id="c15ad-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-156">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-156">Categories</span></span>

- <span data-ttu-id="c15ad-157">Dátum: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="c15ad-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="c15ad-158">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-159">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-159">Summary</span></span>

<span data-ttu-id="c15ad-160">2021. április 27-én az Exchange felügyeleti központ (EAC) új felhasználói élményt nyújt, amely javítani fogja a felhasználók napi hatékonyságát.</span><span class="sxs-lookup"><span data-stu-id="c15ad-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-161">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-161">Impacted audience</span></span>

<span data-ttu-id="c15ad-162">A partner centeren keresztül az Exchange-hez hozzáférő delegált rendszergazdák</span><span class="sxs-lookup"><span data-stu-id="c15ad-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-163">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-163">Details</span></span>

<span data-ttu-id="c15ad-164">2021. április 27-étől kezdve a partner centeren keresztül az Exchange-hez navigáló partnerek átirányítva lesznek az új EAC-ra.</span><span class="sxs-lookup"><span data-stu-id="c15ad-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="c15ad-165">Ez az új felhasználói felület jelenleg előzetes verzióként érhető el, és a rendszergazdák a klasszikus EAC jobb felső sarkában lévő váltógomb kiválasztásával aktiválhatja ezt a felhasználói élményt.</span><span class="sxs-lookup"><span data-stu-id="c15ad-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="c15ad-166">Az új EAC-t úgy is megnyithatja, hogy kijelöli az összes oldalon megjelenő "kipróbálás most" szalagcímet.</span><span class="sxs-lookup"><span data-stu-id="c15ad-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="c15ad-167">Az új EAC előnyei a következők:</span><span class="sxs-lookup"><span data-stu-id="c15ad-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="c15ad-168">További bepillantást, jelentéseket és riasztási mechanizmusokat a levelezés folyamatával kapcsolatos problémákhoz.</span><span class="sxs-lookup"><span data-stu-id="c15ad-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="c15ad-169">Személyre szabott irányítópultok a hatékonyság növelése érdekében.</span><span class="sxs-lookup"><span data-stu-id="c15ad-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="c15ad-170">Ha segítségre van szüksége az új felülettel való átálláshoz, a videók az új EAC-élmény **tanítás & útmutató** szakaszában találhatók.</span><span class="sxs-lookup"><span data-stu-id="c15ad-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="c15ad-171">Ezek áttekintést nyújtanak arról, hogyan használhatja a legjobban az új portált.</span><span class="sxs-lookup"><span data-stu-id="c15ad-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="c15ad-172">Ezzel a módosítással a klasszikus EAC-élmény nem lesz elavult.</span><span class="sxs-lookup"><span data-stu-id="c15ad-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="c15ad-173">A módosítások végrehajtása előtt a rendszer előzetes értesítést küld.</span><span class="sxs-lookup"><span data-stu-id="c15ad-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c15ad-174">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-174">Next steps</span></span>

- <span data-ttu-id="c15ad-175">Tekintse meg az [ebben a témakörben található forrásokat](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), ahol megtekintheti az új felület képernyőképeit.</span><span class="sxs-lookup"><span data-stu-id="c15ad-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="c15ad-176">Ossza meg ezeket az információkat a szervezete megfelelő szereplőivel.</span><span class="sxs-lookup"><span data-stu-id="c15ad-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="c15ad-177">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-177">Questions?</span></span>

<span data-ttu-id="c15ad-178">A változásokkal kapcsolatos bármilyen kérdés esetén keresse meg a megfelelő Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="c15ad-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="c15ad-179">Microsoft-műveletek: a termék indítási naptárának bemutatása</span><span class="sxs-lookup"><span data-stu-id="c15ad-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-180">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-180">Categories</span></span>

- <span data-ttu-id="c15ad-181">Dátum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="c15ad-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="c15ad-182">Ajánlatok | Modern munkahely</span><span class="sxs-lookup"><span data-stu-id="c15ad-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-183">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-183">Summary</span></span>

<span data-ttu-id="c15ad-184">A partneri visszajelzések megválaszolásával a Microsoft műveletei egyszerűbbé teszik a termékekkel kapcsolatos kommunikációt.</span><span class="sxs-lookup"><span data-stu-id="c15ad-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-185">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-185">Impacted audience</span></span>

<span data-ttu-id="c15ad-186">A Cloud Solution Provider (CSP) partnerei</span><span class="sxs-lookup"><span data-stu-id="c15ad-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-187">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-187">Details</span></span>

<span data-ttu-id="c15ad-188">A Microsoft elkötelezte magát a partneri élmény folyamatos javítására.</span><span class="sxs-lookup"><span data-stu-id="c15ad-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="c15ad-189">Visszajelzést kapott arról, hogy túl sok kommunikációt kapott a Microsofttól, beleértve a termék által indított ismétlődő hirdetményeket is.</span><span class="sxs-lookup"><span data-stu-id="c15ad-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="c15ad-190">Visszajelzése alapján a Microsoft egyszerűsítette a termékre vonatkozó készültségi tapasztalatot, amely új és meglévő ajánlatokat tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="c15ad-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="c15ad-191">Most az Operations Readiness Resource Galleryben közzétett, a termékre vonatkozó, egyetlen havi nézetet is biztosítunk.</span><span class="sxs-lookup"><span data-stu-id="c15ad-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="c15ad-192">Ez a havi [termék-indítási naptár nézet](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) az egyes termékek indításával kapcsolatos kommunikációt az Operations Readiness Resource Galleryben és a partner Center bejelentésekben fogja lecserélni.</span><span class="sxs-lookup"><span data-stu-id="c15ad-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="c15ad-193">A [termék elindítására vonatkozó naptárat](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) a [közösségi gyűjtemények](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), a [Naptár-nézetek](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)és a CSP- [hírlevelek](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)segítségével is elérheti.</span><span class="sxs-lookup"><span data-stu-id="c15ad-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="c15ad-194">Értesítjük Önt, ha minden hónap termék-indítási naptárát közzéteszik az Operations Readiness Resource Galleryben bejelentéssel.</span><span class="sxs-lookup"><span data-stu-id="c15ad-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="c15ad-195">Továbbra is megtalálhatja az új és meglévő ajánlatokkal kapcsolatos információkat a árlista előnézetében és a árlista változási naplóiban, valamint a Product blogs, a licencelési útmutatók és a termékek marketing oldalain.</span><span class="sxs-lookup"><span data-stu-id="c15ad-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="c15ad-196">A módosítás a következő termékek esetében érvényes lesz:</span><span class="sxs-lookup"><span data-stu-id="c15ad-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="c15ad-197">Helyszíni Dynamics</span><span class="sxs-lookup"><span data-stu-id="c15ad-197">Dynamics on-premises</span></span>
- <span data-ttu-id="c15ad-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c15ad-198">Microsoft 365</span></span>
- <span data-ttu-id="c15ad-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="c15ad-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="c15ad-200">Windows</span><span class="sxs-lookup"><span data-stu-id="c15ad-200">Windows</span></span>
- <span data-ttu-id="c15ad-201">Kiszolgáló</span><span class="sxs-lookup"><span data-stu-id="c15ad-201">Server</span></span>  
- <span data-ttu-id="c15ad-202">Eszközök</span><span class="sxs-lookup"><span data-stu-id="c15ad-202">Tools</span></span>
- <span data-ttu-id="c15ad-203">Csapatok és távközlési</span><span class="sxs-lookup"><span data-stu-id="c15ad-203">Teams and Telco</span></span>

<span data-ttu-id="c15ad-204">Továbbra is küldünk olyan, a termékre vonatkozó bejelentéseket, amelyek szükségesek az Operations Readiness részleteiről.</span><span class="sxs-lookup"><span data-stu-id="c15ad-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c15ad-205">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-205">Next steps</span></span>

<span data-ttu-id="c15ad-206">Tekintse át a témakör erőforrásait, és ossza meg ezeket az információkat a szervezete megfelelő szereplőivel.</span><span class="sxs-lookup"><span data-stu-id="c15ad-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-207">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-207">Questions?</span></span>

<span data-ttu-id="c15ad-208">Az ajánlatokkal kapcsolatos további kérdésekért keresse meg a megfelelő Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="c15ad-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="c15ad-209">A CSP-ügyfél bevezetési követelményeinek változásai</span><span class="sxs-lookup"><span data-stu-id="c15ad-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-210">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-210">Categories</span></span>

- <span data-ttu-id="c15ad-211">Dátum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="c15ad-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="c15ad-212">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-213">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-213">Summary</span></span>

<span data-ttu-id="c15ad-214">A partnereknek és az ügyfeleknek a bizalmi kapcsolaton alapuló elkötelezettségünk részeként további vásárlói adatokat fogunk kérni, amelyek 2021. március 25-én érvényesek.</span><span class="sxs-lookup"><span data-stu-id="c15ad-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-215">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-215">Impacted audience</span></span>

<span data-ttu-id="c15ad-216">Cloud Solution Provider (CSP) közvetlen számlázási partnerek és közvetett szolgáltatók, akik új vagy meglévő ügyfelekkel rendelkeznek a következő szakaszban felsorolt országokban</span><span class="sxs-lookup"><span data-stu-id="c15ad-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-217">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-217">Details</span></span>

<span data-ttu-id="c15ad-218">A Microsoft megbízhatósági kapcsolaton fut.</span><span class="sxs-lookup"><span data-stu-id="c15ad-218">Microsoft runs on trust.</span></span> <span data-ttu-id="c15ad-219">Elkötelezettek vagyunk abban, hogy megfelelő, biztonságos és biztonságos módszert biztosítanak az ügyfél-előfizetések lebonyolítására a CSP programban.</span><span class="sxs-lookup"><span data-stu-id="c15ad-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="c15ad-220">2021. március 25-én bevezetjük a partner Center API-t és a felhasználói felület (UI) fejlesztéseit, amelyek hatással lesznek a következő feltételeknek megfelelő partnerekre:</span><span class="sxs-lookup"><span data-stu-id="c15ad-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="c15ad-221">A partner közvetlen számlázási kapcsolatban áll a Microsofttal (ami azt jelenti, hogy a partner közvetlen számlás partner vagy közvetett szolgáltató).</span><span class="sxs-lookup"><span data-stu-id="c15ad-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="c15ad-222">A partner üzleti tevékenységet folytat az új vagy meglévő ügyfelekkel a következő országokban:</span><span class="sxs-lookup"><span data-stu-id="c15ad-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="c15ad-223">Thaiföld</span><span class="sxs-lookup"><span data-stu-id="c15ad-223">Thailand</span></span>
    - <span data-ttu-id="c15ad-224">Vietnam</span><span class="sxs-lookup"><span data-stu-id="c15ad-224">Vietnam</span></span>
    - <span data-ttu-id="c15ad-225">Törökország</span><span class="sxs-lookup"><span data-stu-id="c15ad-225">Turkey</span></span>
    - <span data-ttu-id="c15ad-226">Lengyelország</span><span class="sxs-lookup"><span data-stu-id="c15ad-226">Poland</span></span>
    - <span data-ttu-id="c15ad-227">Dél-afrikai Köztársaság</span><span class="sxs-lookup"><span data-stu-id="c15ad-227">South Africa</span></span>
    - <span data-ttu-id="c15ad-228">India</span><span class="sxs-lookup"><span data-stu-id="c15ad-228">India</span></span>
    - <span data-ttu-id="c15ad-229">Brazília</span><span class="sxs-lookup"><span data-stu-id="c15ad-229">Brazil</span></span>
    - <span data-ttu-id="c15ad-230">Irak</span><span class="sxs-lookup"><span data-stu-id="c15ad-230">Iraq</span></span>
    - <span data-ttu-id="c15ad-231">Mianmar</span><span class="sxs-lookup"><span data-stu-id="c15ad-231">Myanmar</span></span>
    - <span data-ttu-id="c15ad-232">Dél-Szudán</span><span class="sxs-lookup"><span data-stu-id="c15ad-232">South Sudan</span></span>
    - <span data-ttu-id="c15ad-233">Szaúd-Arábia</span><span class="sxs-lookup"><span data-stu-id="c15ad-233">Saudi Arabia</span></span>
    - <span data-ttu-id="c15ad-234">Egyesült Arab Emírségek</span><span class="sxs-lookup"><span data-stu-id="c15ad-234">United Arab Emirates</span></span>
    - <span data-ttu-id="c15ad-235">Venezuela</span><span class="sxs-lookup"><span data-stu-id="c15ad-235">Venezuela</span></span>

<span data-ttu-id="c15ad-236">A feltételeknek megfelelő partnereknek be kell nyújtaniuk az ügyfél **vállalati regisztrációs azonosítóját** (más néven az ügyfél **szervezeti** webhelyét) és a **telefonszámot** , amikor új ügyfeleket vesznek fel, vagy módosíthatják a meglévő ügyfelek adatait.</span><span class="sxs-lookup"><span data-stu-id="c15ad-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="c15ad-237">Ezek a partnerek **középső nevet** is megadhatnak az ügyfél számára.</span><span class="sxs-lookup"><span data-stu-id="c15ad-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="c15ad-238">Vegye figyelembe, hogy a vállalati regisztrációs azonosító hozzáadásakor az üzleti adó azonosítót kell használnia, nem pedig az ügyfél személyes AZONOSÍTÓját.</span><span class="sxs-lookup"><span data-stu-id="c15ad-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="c15ad-239">A következő országokban az új vagy meglévő ügyfelekkel folytatott üzleti partnerek már egy korábbi kiadásban, 2020 novemberében lettek bevezetve.</span><span class="sxs-lookup"><span data-stu-id="c15ad-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="c15ad-240">Örményország</span><span class="sxs-lookup"><span data-stu-id="c15ad-240">Armenia</span></span>
- <span data-ttu-id="c15ad-241">Azerbajdzsán</span><span class="sxs-lookup"><span data-stu-id="c15ad-241">Azerbaijan</span></span>
- <span data-ttu-id="c15ad-242">Belarusz</span><span class="sxs-lookup"><span data-stu-id="c15ad-242">Belarus</span></span>
- <span data-ttu-id="c15ad-243">Magyarország</span><span class="sxs-lookup"><span data-stu-id="c15ad-243">Hungary</span></span>
- <span data-ttu-id="c15ad-244">Kazahsztán</span><span class="sxs-lookup"><span data-stu-id="c15ad-244">Kazakhstan</span></span>
- <span data-ttu-id="c15ad-245">Kirgizisztán</span><span class="sxs-lookup"><span data-stu-id="c15ad-245">Kyrgyzstan</span></span>
- <span data-ttu-id="c15ad-246">Moldova</span><span class="sxs-lookup"><span data-stu-id="c15ad-246">Moldova</span></span>
- <span data-ttu-id="c15ad-247">Oroszország</span><span class="sxs-lookup"><span data-stu-id="c15ad-247">Russia</span></span>
- <span data-ttu-id="c15ad-248">Tádzsikisztán</span><span class="sxs-lookup"><span data-stu-id="c15ad-248">Tajikistan</span></span>
- <span data-ttu-id="c15ad-249">Ukrajna</span><span class="sxs-lookup"><span data-stu-id="c15ad-249">Ukraine</span></span>
- <span data-ttu-id="c15ad-250">Üzbegisztán</span><span class="sxs-lookup"><span data-stu-id="c15ad-250">Uzbekistan</span></span>

<span data-ttu-id="c15ad-251">A világ többi részén ügyfelekkel rendelkező partnerek a 2021. március 25-én megadhatják a **vállalati regisztrációs azonosítót**, a **telefonszámot** és a **középső nevet** az ügyfelek számára opcionális részletekként.</span><span class="sxs-lookup"><span data-stu-id="c15ad-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c15ad-252">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-252">Next steps</span></span>

- <span data-ttu-id="c15ad-253">Részletesebb útmutatásért tekintse át a technikai dokumentációt és a [dedikált partneri gyűjteményben](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) gyakran feltett kérdéseket.</span><span class="sxs-lookup"><span data-stu-id="c15ad-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="c15ad-254">Készítse elő a módosításokat a partner Center API és a webes felhasználói élmény használatával.</span><span class="sxs-lookup"><span data-stu-id="c15ad-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="c15ad-255">Az API-k és SDK-k tesztelésre lesznek elérhetők.</span><span class="sxs-lookup"><span data-stu-id="c15ad-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="c15ad-256">Ügyeljen arra, hogy új ügyfelek beléptetése vagy a meglévő ügyfél adatainak módosításakor küldje el a további adatokat.</span><span class="sxs-lookup"><span data-stu-id="c15ad-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="c15ad-257">Ha Vezérlőpult-gyártói (CPV) megoldást használ, tekintse meg a CPV-t.</span><span class="sxs-lookup"><span data-stu-id="c15ad-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-258">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-258">Questions?</span></span>

<span data-ttu-id="c15ad-259">Ha bármilyen kérdése van a jogi azonosítóval (más néven INN vagy TIN) kapcsolatban, forduljon az adó-tanácsadóhoz vagy a helyi adóhivatal-irodához.</span><span class="sxs-lookup"><span data-stu-id="c15ad-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="c15ad-260">A Microsoft nem tud útmutatást nyújtani adózási kérdésekben.</span><span class="sxs-lookup"><span data-stu-id="c15ad-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="c15ad-261">Ha támogatásra van szüksége a Microsoft által végzett műveletekhez, [Nyisson meg egy szolgáltatási kérelmet](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="c15ad-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="c15ad-262">Helyesbítések a 2021-es végleges szoftverek árlista</span><span class="sxs-lookup"><span data-stu-id="c15ad-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-263">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-263">Categories</span></span>

- <span data-ttu-id="c15ad-264">Dátum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="c15ad-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="c15ad-265">Ajánlatok/piacok</span><span class="sxs-lookup"><span data-stu-id="c15ad-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-266">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-266">Impacted audience</span></span>

<span data-ttu-id="c15ad-267">A közvetett szolgáltatók és a közvetlen számlázási partnerek örökös szoftvereket mutatnak a felhőalapú megoldás-szolgáltató programban</span><span class="sxs-lookup"><span data-stu-id="c15ad-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="c15ad-268">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-268">Details</span></span>

<span data-ttu-id="c15ad-269">A 2021. március 1-én közzétett, Perpetual szoftverekhez tartozó árlista olyan piacokat foglal magában, amelyek nem voltak ott.</span><span class="sxs-lookup"><span data-stu-id="c15ad-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="c15ad-270">A végleges szoftverhasználat-árlista 2021. március 17-én frissült a megfelelő értékekkel.</span><span class="sxs-lookup"><span data-stu-id="c15ad-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="c15ad-271">Ezek a javítások csak a következőre voltak érvényesek:</span><span class="sxs-lookup"><span data-stu-id="c15ad-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="c15ad-272">Termék azonosítója: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="c15ad-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="c15ad-273">Terméknév: Windows 10 Home to Pro verziófrissítés Microsoft 365 Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="c15ad-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="c15ad-274">Eltávolított vagy nem támogatott piacok: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, az LB, az LK, a MU, a NA, a NG , NI, NP, OM, PA, PE, PH, PK, PR, UY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG,, UZ, VE, VN, YE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="c15ad-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="c15ad-275">Ezek a módosítások csak a fenti termékre vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="c15ad-275">These changes only apply to the above product.</span></span> <span data-ttu-id="c15ad-276">Más termékek nem voltak kijavítani.</span><span class="sxs-lookup"><span data-stu-id="c15ad-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="c15ad-277">Következő lépések és erőforrások</span><span class="sxs-lookup"><span data-stu-id="c15ad-277">Next steps and resources</span></span>

- <span data-ttu-id="c15ad-278">Az örökös szoftvereket futtató partnereknek le kell tölteniük a legfrissebb végleges szoftverek árlista listáját.</span><span class="sxs-lookup"><span data-stu-id="c15ad-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="c15ad-279">A [régióbeli országkód](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) alapján a két betűs rövidítések országokra való rövid hozzárendelését lehet megkeresni.</span><span class="sxs-lookup"><span data-stu-id="c15ad-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="c15ad-280">SDK-kiadás a .NET standardban (v 1.17.0)</span><span class="sxs-lookup"><span data-stu-id="c15ad-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-281">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-281">Categories</span></span>

- <span data-ttu-id="c15ad-282">Dátum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="c15ad-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="c15ad-283">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="c15ad-284">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-284">Impacted audience</span></span>

<span data-ttu-id="c15ad-285">A partner Center .NET SDK-t használó CSP programban részt vevő közvetlen számlázási partnerek és közvetett szolgáltatók.</span><span class="sxs-lookup"><span data-stu-id="c15ad-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-286">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-286">Details</span></span>

<span data-ttu-id="c15ad-287">Március 23 2020-én a partnerek megkezdhetik a [MicrosoftPartnerCenter. NETSDK (NuGet Gallery) verziójának letöltését. Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), valamint a frissített Public partner Center SDK [GitHub-mintákat](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span><span class="sxs-lookup"><span data-stu-id="c15ad-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="c15ad-288">Ez a verzió a következő módszerek frissítéseit tartalmazza:</span><span class="sxs-lookup"><span data-stu-id="c15ad-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="c15ad-289">Naplózás frissítve: új műveleti típusok</span><span class="sxs-lookup"><span data-stu-id="c15ad-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="c15ad-290">Új [műveleti típusok](https://docs.microsoft.com/partner-center/develop/auditing-resources) lettek hozzáadva, amelyekből megtudhatja, mikor hagyta jóvá és szakítja meg a DAP szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="c15ad-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="c15ad-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="c15ad-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="c15ad-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="c15ad-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="c15ad-293">Napló frissítve: új erőforrás-és műveleti típusok</span><span class="sxs-lookup"><span data-stu-id="c15ad-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="c15ad-294">Új [erőforrás-és műveleti típusok](https://docs.microsoft.com/partner-center/develop/auditing-resources) lettek hozzáadva az ügyfél-címtár szerepkör-forgatókönyv támogatásához.</span><span class="sxs-lookup"><span data-stu-id="c15ad-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="c15ad-295">Új erőforrástípus: "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="c15ad-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="c15ad-296">A "AddUserMember" és a "RemoveUserMember" típusú műveletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="c15ad-297">Ügyfél-fiókok SDK-frissítései</span><span class="sxs-lookup"><span data-stu-id="c15ad-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="c15ad-298">Támogatás a/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus beolvasásához</span><span class="sxs-lookup"><span data-stu-id="c15ad-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="c15ad-299">/Customers/{Customer-Tenant-ID}/Qualifications beolvasása</span><span class="sxs-lookup"><span data-stu-id="c15ad-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="c15ad-300">POST/Customers/{customer_id}/Qualifications? Code = {validationCode}</span><span class="sxs-lookup"><span data-stu-id="c15ad-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="c15ad-301">További módosítások</span><span class="sxs-lookup"><span data-stu-id="c15ad-301">Additional changes</span></span>

<span data-ttu-id="c15ad-302">A következő változások az új kereskedelmi szolgáltatás részeként jelennek meg, és a meghívással jelenleg csak olyan partnereink számára érhetők el, akik a M365/D365 új kereskedelmi élményhez tartoznak.</span><span class="sxs-lookup"><span data-stu-id="c15ad-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="c15ad-303">Azok a partnerek, akik nem részei az új kereskedelmi technikai előzetes verziónak, nem észlelik a hatásokat, és visszamenőlegesen kompatibilisnek kell lenniük.</span><span class="sxs-lookup"><span data-stu-id="c15ad-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="c15ad-304">Katalógus változásai:</span><span class="sxs-lookup"><span data-stu-id="c15ad-304">Catalog Changes:</span></span>

  - <span data-ttu-id="c15ad-305">/Products/{Product-ID}/SKUs/{SKU-ID} beolvasása</span><span class="sxs-lookup"><span data-stu-id="c15ad-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="c15ad-306">Vásárlás és kezelés:</span><span class="sxs-lookup"><span data-stu-id="c15ad-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="c15ad-307">/Customers/{customerId}/subscriptions beolvasása</span><span class="sxs-lookup"><span data-stu-id="c15ad-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="c15ad-308">/Customers/{customerId}/subscriptions/{subscriptionId} beolvasása</span><span class="sxs-lookup"><span data-stu-id="c15ad-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="c15ad-309">/Customers/{customerId}/subscriptions/{subscriptionId} javítása</span><span class="sxs-lookup"><span data-stu-id="c15ad-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="c15ad-310">/Customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities beolvasása</span><span class="sxs-lookup"><span data-stu-id="c15ad-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="c15ad-311">/Customers/{customerId}/subscriptions/{subscriptionId}/transitions beolvasása</span><span class="sxs-lookup"><span data-stu-id="c15ad-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="c15ad-312">/Customers/{customerId}/subscriptions/{subscriptionId}/transitions közzététele</span><span class="sxs-lookup"><span data-stu-id="c15ad-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="c15ad-313">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-313">Next Steps</span></span>

- <span data-ttu-id="c15ad-314">Töltse le a legújabb verziót: [MicrosoftPartnerCenter. NETSDK (NuGet Gallery | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="c15ad-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="c15ad-315">A [GitHub-minták](https://github.com/Microsoft/Partner-Center-DotNet-Samples) letöltése és áttekintése</span><span class="sxs-lookup"><span data-stu-id="c15ad-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="c15ad-316">CSP kereskedelmi Marketplace ajánlat és FY21 CSP-ösztönzők a jogosult ajánlatok számára</span><span class="sxs-lookup"><span data-stu-id="c15ad-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-317">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-317">Categories</span></span>

- <span data-ttu-id="c15ad-318">Dátum: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="c15ad-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="c15ad-319">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-320">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-320">Impacted audience</span></span>

<span data-ttu-id="c15ad-321">Közvetett szolgáltatók és közvetlen számlázási partnerek a Cloud Solution Provider programban</span><span class="sxs-lookup"><span data-stu-id="c15ad-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="c15ad-322">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-322">Details</span></span>

<span data-ttu-id="c15ad-323">A közvetett szolgáltatók és a közvetlen számlázási partnerek a felhőalapú megoldás-szolgáltatói programban harmadik féltől származó ajánlatokat is értékesíthetik, és kedvezményeket szerezhetnek a partner Centerben vagy a Azure Portalban lebonyolított, jogosult harmadik féltől származó ajánlatokra vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="c15ad-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="c15ad-324">Az ösztönzés a jogosult ajánlatok esetében a számlázott értékesítések esetében engedmény formájában történik, és **2021. június 30-ig érhető el**.</span><span class="sxs-lookup"><span data-stu-id="c15ad-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="c15ad-325">Folytassa a jelen CSP kereskedelmi Marketplace ajánlatának megismerését, és lépjen kapcsolatba az ügyfelekkel a megfelelő ajánlatok azonosításához, hogy azok továbbra is sikeresek és digitális átalakítást nyújtsanak.</span><span class="sxs-lookup"><span data-stu-id="c15ad-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="c15ad-326">Független szoftvergyártók (ISV-ket) partnereink, hogy a legújabb IaaS és SaaS-megoldásokat a Microsoft ügyfelei számára is piacra hozzák.</span><span class="sxs-lookup"><span data-stu-id="c15ad-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="c15ad-327">Az ISV-közzétevők lehetővé teszik, hogy a Microsoft partneri csatornán keresztül engedélyezzék az ajánlatok értékesítését.</span><span class="sxs-lookup"><span data-stu-id="c15ad-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="c15ad-328">Az ösztönzőre jogosult ajánlatok két kategóriába sorolhatók:</span><span class="sxs-lookup"><span data-stu-id="c15ad-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="c15ad-329">Válassza ki a SaaS-és IaaS külső ajánlatokat az Azure IP-címek közös értékesítésének incentivized állapotával.</span><span class="sxs-lookup"><span data-stu-id="c15ad-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="c15ad-330">Csapatokkal vagy legalább két Microsoft 365 hatékonyságnövelő alkalmazásokkal integrált SaaS-alkalmazások, mint például a PowerPoint, a Word, az Excel, az Outlook vagy a SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c15ad-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="c15ad-331">Következő lépések és erőforrások</span><span class="sxs-lookup"><span data-stu-id="c15ad-331">Next steps and resources</span></span>

- <span data-ttu-id="c15ad-332">Ismerje meg, hogyan szerezhet [partneri ösztönzőket](https://partner.microsoft.com/membership/partner-incentives) a jogosult Marketplace-alkalmazások értékesítésére az ösztönző jogosult alkalmazások számára.</span><span class="sxs-lookup"><span data-stu-id="c15ad-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="c15ad-333">Az új ajánlatok havonta lesznek hozzáadva.</span><span class="sxs-lookup"><span data-stu-id="c15ad-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="c15ad-334">Felhőalapú megoldás-szolgáltató közvetlen számlázási partneri ösztönző erőforrásai</span><span class="sxs-lookup"><span data-stu-id="c15ad-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="c15ad-335">Felhőalapú megoldás szolgáltatójának közvetett szolgáltatói ösztönző erőforrásai</span><span class="sxs-lookup"><span data-stu-id="c15ad-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="c15ad-336">Tekintse át ezt a [bemutatót](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) , ha többet szeretne megtudni a kereskedelmi piactéren elérhető alkalmazások értékesítéséről.</span><span class="sxs-lookup"><span data-stu-id="c15ad-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="c15ad-337">További forrásokat [itt találhat](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span><span class="sxs-lookup"><span data-stu-id="c15ad-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="c15ad-338">Fedezze fel a kereskedelmi piactér katalógusát a [partner Centerben](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) vagy [Azure Portal](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="c15ad-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="c15ad-339">[API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) -k használata az alkalmazások vállalati piactéren való integrálásához</span><span class="sxs-lookup"><span data-stu-id="c15ad-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="c15ad-340">Tegye elérhetővé az olyan ISV-ket, akik érdeklődnek a</span><span class="sxs-lookup"><span data-stu-id="c15ad-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="c15ad-341">A közvetett szolgáltatóknak integrálnia kell az API-k és az útmutató viszonteladók használatával</span><span class="sxs-lookup"><span data-stu-id="c15ad-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-342">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-342">Questions?</span></span>  

<span data-ttu-id="c15ad-343">Tekintse át [ezt a cikket](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) a partner Center kereskedelmi piactérének áttekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="c15ad-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="c15ad-344">Ha további segítségre van szüksége, létrehozhat egy támogatási kérést a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="c15ad-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="c15ad-345">További információ: [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="c15ad-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="c15ad-346">Power BI Premium ajánlat elnevezési és előfeltétel-frissítése</span><span class="sxs-lookup"><span data-stu-id="c15ad-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-347">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-347">Categories</span></span>

- <span data-ttu-id="c15ad-348">Dátum: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="c15ad-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="c15ad-349">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-350">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-350">Summary</span></span>

<span data-ttu-id="c15ad-351">Az 2021-as április 1-től a végső árlista frissül, hogy egyértelművé tegye a felhasználók által kínált Power BI Premium elnevezési és/vagy előfeltétel-információit.</span><span class="sxs-lookup"><span data-stu-id="c15ad-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-352">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-352">Impacted audience</span></span>

<span data-ttu-id="c15ad-353">Cloud Solution Provider (CSP) közvetlen és közvetett partnerek</span><span class="sxs-lookup"><span data-stu-id="c15ad-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-354">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-354">Details</span></span>

<span data-ttu-id="c15ad-355">Az 2021-as április 1-től a végső árlista frissül, hogy egyértelművé tegye a felhasználók által kínált Power BI Premium elnevezési és/vagy előfeltétel-információit.</span><span class="sxs-lookup"><span data-stu-id="c15ad-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="c15ad-356">A végleges árlista frissítése előtt használja az ebben a szakaszban található információkat a megfelelő termék megrendelésének biztosításához.</span><span class="sxs-lookup"><span data-stu-id="c15ad-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="c15ad-357">Az alábbi részletek az érintett SKU-t és az előfeltételek részleteit mutatják be.</span><span class="sxs-lookup"><span data-stu-id="c15ad-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="c15ad-358">Ajánlat megjelenítendő neve március 1-től árlista</span><span class="sxs-lookup"><span data-stu-id="c15ad-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="c15ad-359">Frissített ajánlat megjelenítendő neve április 1-től végleges árlista</span><span class="sxs-lookup"><span data-stu-id="c15ad-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="c15ad-360">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="c15ad-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="c15ad-361">Felhasználónkénti Add-On Power BI Premium (nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="c15ad-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="c15ad-362">Power BI Premium felhasználónkénti Add-On **(Office)** (nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="c15ad-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="c15ad-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="c15ad-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="c15ad-364">Az ajánlat megvásárlásához az ügyfélnek az alábbi előfeltételek valamelyikét kell megadnia:</span><span class="sxs-lookup"><span data-stu-id="c15ad-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="c15ad-365">Ajánlat megjelenítendő neve</span><span class="sxs-lookup"><span data-stu-id="c15ad-365">Offer display name</span></span> | <span data-ttu-id="c15ad-366">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="c15ad-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="c15ad-367">Microsoft 365 E5 (nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="c15ad-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="c15ad-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="c15ad-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="c15ad-369">Microsoft 365 E5 hangkonferencia nélkül (nonprofit munkatársak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="c15ad-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="c15ad-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="c15ad-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="c15ad-371">Office 365 E5 (nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="c15ad-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="c15ad-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="c15ad-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="c15ad-373">Office 365 E5 (nonprofit alkalmazottak díjszabása) próbaverzió</span><span class="sxs-lookup"><span data-stu-id="c15ad-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="c15ad-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="c15ad-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="c15ad-375">Office 365 E5 hangkonferencia nélkül (nonprofit munkatársak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="c15ad-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="c15ad-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="c15ad-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="c15ad-377">Az alábbi Power BI Premium ajánlat előfeltétele a vásárláshoz szükséges:</span><span class="sxs-lookup"><span data-stu-id="c15ad-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="c15ad-378">Ajánlat megjelenítendő neve</span><span class="sxs-lookup"><span data-stu-id="c15ad-378">Offer display name</span></span> | <span data-ttu-id="c15ad-379">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="c15ad-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="c15ad-380">Felhasználónkénti Add-On Power BI Premium (nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="c15ad-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="c15ad-381">ef0b895b-681B-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="c15ad-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="c15ad-382">Az ajánlat megvásárlásához az ügyfeleknek meg kell követelniük az alábbi előfeltételeket:</span><span class="sxs-lookup"><span data-stu-id="c15ad-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="c15ad-383">Ajánlat megjelenítendő neve</span><span class="sxs-lookup"><span data-stu-id="c15ad-383">Offer display name</span></span> | <span data-ttu-id="c15ad-384">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="c15ad-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="c15ad-385">Power BI Pro (nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="c15ad-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="c15ad-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="c15ad-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="c15ad-387">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-387">Next steps</span></span>

<span data-ttu-id="c15ad-388">Tekintse át a témakör erőforrásait, és ossza meg ezeket az információkat a szervezete megfelelő szereplőivel.</span><span class="sxs-lookup"><span data-stu-id="c15ad-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="c15ad-389">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-389">Questions?</span></span>

<span data-ttu-id="c15ad-390">Az ajánlatokkal kapcsolatos bármilyen kérdés esetén keresse meg a megfelelő Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="c15ad-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="c15ad-391">A Microsoft 365 F3 díjszabási frissítései</span><span class="sxs-lookup"><span data-stu-id="c15ad-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-392">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-392">Categories</span></span>

- <span data-ttu-id="c15ad-393">Dátum: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="c15ad-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="c15ad-394">Ajánlatok/piacok</span><span class="sxs-lookup"><span data-stu-id="c15ad-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-395">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-395">Summary</span></span>

<span data-ttu-id="c15ad-396">Helytelen a március 2021 díjszabása kijavítva a Microsoft 365 F3 angol font (GBP) és az euro (EUR) esetében.</span><span class="sxs-lookup"><span data-stu-id="c15ad-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-397">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-397">Impacted audience</span></span>

<span data-ttu-id="c15ad-398">A partnerek a Cloud Solution Provider (CSP) program keretében a 2021. március 1. és március 17. között megvásárolt Microsoft 365 F3-at.</span><span class="sxs-lookup"><span data-stu-id="c15ad-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-399">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-399">Details</span></span>

<span data-ttu-id="c15ad-400">A Microsoft a Microsoft 365 F3 helytelen díjszabását oldotta meg.</span><span class="sxs-lookup"><span data-stu-id="c15ad-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="c15ad-401">A helytelen árak a GBP és az EUR, és csak a 2021. március 1. és március 17. között megvásárolt ajánlatokra érvényesek.</span><span class="sxs-lookup"><span data-stu-id="c15ad-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="c15ad-402">Az érintett ajánlatok és pénznemek az alábbiakban láthatók.</span><span class="sxs-lookup"><span data-stu-id="c15ad-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="c15ad-403">Ajánlat neve</span><span class="sxs-lookup"><span data-stu-id="c15ad-403">Offer name</span></span> | <span data-ttu-id="c15ad-404">Pénznem</span><span class="sxs-lookup"><span data-stu-id="c15ad-404">Currency</span></span> | <span data-ttu-id="c15ad-405">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="c15ad-405">Offer ID</span></span> | <span data-ttu-id="c15ad-406">Anyag azonosítója</span><span class="sxs-lookup"><span data-stu-id="c15ad-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="c15ad-407">Microsoft 365 F3 (jótékonysági)</span><span class="sxs-lookup"><span data-stu-id="c15ad-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="c15ad-408">GBP</span><span class="sxs-lookup"><span data-stu-id="c15ad-408">GBP</span></span> | <span data-ttu-id="c15ad-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="c15ad-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="c15ad-410">HRE-11626</span><span class="sxs-lookup"><span data-stu-id="c15ad-410">AAD-11626</span></span> |
| <span data-ttu-id="c15ad-411">Microsoft 365 F3 (kereskedelmi)</span><span class="sxs-lookup"><span data-stu-id="c15ad-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="c15ad-412">EUR</span><span class="sxs-lookup"><span data-stu-id="c15ad-412">EUR</span></span>| <span data-ttu-id="c15ad-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="c15ad-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="c15ad-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="c15ad-414">AAA-89898</span></span> |
 
<span data-ttu-id="c15ad-415">A márciusi és áprilisi előzetes verzióra vonatkozó alapszintű árlista a csendes-óceáni téli idő szerint 15. március 16-án frissült.</span><span class="sxs-lookup"><span data-stu-id="c15ad-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c15ad-416">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-416">Next steps</span></span>

- <span data-ttu-id="c15ad-417">Ha szükséges, a partnereknek újra le kell tölteniük az aktuális licenccel-alapú árlistát, valamint a márciusi és az áprilisi előzetes verziót is.</span><span class="sxs-lookup"><span data-stu-id="c15ad-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="c15ad-418">A Microsoft e-mailben kapcsolatba lép a kapcsolódó partnerekkel az elkövetkező hetekben, hogy tájékoztassa őket az érintett tranzakciók kijavítására vonatkozó következő lépésekről.</span><span class="sxs-lookup"><span data-stu-id="c15ad-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-419">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-419">Questions?</span></span>

<span data-ttu-id="c15ad-420">További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeit.</span><span class="sxs-lookup"><span data-stu-id="c15ad-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="c15ad-421">Jogi cég nevének frissítése a partner centeren keresztül</span><span class="sxs-lookup"><span data-stu-id="c15ad-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-422">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-422">Categories</span></span>

- <span data-ttu-id="c15ad-423">Dátum: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="c15ad-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="c15ad-424">A meghajtó hatékonyságának & skálázása</span><span class="sxs-lookup"><span data-stu-id="c15ad-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-425">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-425">Summary</span></span>

<span data-ttu-id="c15ad-426">Március 2021, Microsoft Partner Network (MPN) partnerek és a felhőalapú megoldás-szolgáltató (CSP) közvetett viszonteladók a partner centeren keresztül frissíthetik a vállalatuk nevét.</span><span class="sxs-lookup"><span data-stu-id="c15ad-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-427">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-427">Impacted audience</span></span>

<span data-ttu-id="c15ad-428">MPN-partnerek és CSP közvetett viszonteladók (nem alkalmazható a CSP Direct Bill-partnereknek)</span><span class="sxs-lookup"><span data-stu-id="c15ad-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-429">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-429">Details</span></span>

<span data-ttu-id="c15ad-430">A március 2021-től kezdődően az MPN-partnerek és a CSP közvetett viszonteladók megfelelő, önkiszolgáló módon frissíthetik a vállalatuk nevét a partner centeren keresztül.</span><span class="sxs-lookup"><span data-stu-id="c15ad-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="c15ad-431">Ezzel az új funkcióval a partnereknek többé nem kell beküldeniük a partner Center támogatási jegyét a vállalat nevének frissítéséhez.</span><span class="sxs-lookup"><span data-stu-id="c15ad-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="c15ad-432">Így jelentős mennyiségű időt takaríthat meg a partnerek számára ezen tevékenységek végrehajtásakor.</span><span class="sxs-lookup"><span data-stu-id="c15ad-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="c15ad-433">További információ: [a jogi üzleti profil frissítése](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="c15ad-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="c15ad-434">Győződjön meg arról, hogy a vállalat neve a jogi üzleti profilban nem tartalmaz helyesírási hibákat és rövidítéseket, és pontosan megfelel a vállalati üzleti regisztrációs rekordoknak.</span><span class="sxs-lookup"><span data-stu-id="c15ad-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="c15ad-435">A szervezeti profil frissítésével kapcsolatos további információkért tekintse meg a [szervezet profiljának ellenőrzése](../update-your-partner-profile.md#update-your-legal-business-profile)című témakört.</span><span class="sxs-lookup"><span data-stu-id="c15ad-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="c15ad-436">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-436">Next steps</span></span>

<span data-ttu-id="c15ad-437">Ossza meg ezt az információt a szervezeten belül, hogy a megfelelő csapat áttekintse és frissítse a folyamatait.</span><span class="sxs-lookup"><span data-stu-id="c15ad-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-438">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-438">Questions?</span></span>

<span data-ttu-id="c15ad-439">További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeit.</span><span class="sxs-lookup"><span data-stu-id="c15ad-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="c15ad-440">Frissítés a Cloud Solution Provider (CSP) program fejleményeire és a licencelési program megnyitására</span><span class="sxs-lookup"><span data-stu-id="c15ad-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-441">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-441">Categories</span></span>

- <span data-ttu-id="c15ad-442">Dátum: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="c15ad-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="c15ad-443">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-444">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-444">Summary</span></span>

<span data-ttu-id="c15ad-445">Az új kereskedelmi és közszektorbeli örökös szoftverek a Cloud Solution Provider (CSP) programba kerülnek, valamint az Open licencelési program módosításait.</span><span class="sxs-lookup"><span data-stu-id="c15ad-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-446">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-446">Impacted audience</span></span>

<span data-ttu-id="c15ad-447">A nyílt licencelési programon keresztül árusító kereskedelmi terjesztők és felügyelt viszonteladók, valamint az örökös szoftvereket lebonyolító CSP-partnerek</span><span class="sxs-lookup"><span data-stu-id="c15ad-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-448">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-448">Details</span></span>

<span data-ttu-id="c15ad-449">A Microsoft szeptember 2020-án [bejelentette](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a digitális átalakulás lépéseinek egy sorozatát, amely kibővíti a partnereinkkel kapcsolatos lehetőségeket a CSP programban, beleértve a helyszíni szoftverek rendelkezésre állását a partnerek számára.</span><span class="sxs-lookup"><span data-stu-id="c15ad-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="c15ad-450">Ezek a változások lehetővé teszik, hogy a partnerek a CSP-ben a szoftver licenceit kihasználva növeljék üzleti tevékenységüket</span><span class="sxs-lookup"><span data-stu-id="c15ad-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="c15ad-451">Emellett képessé teszik az ügyfeleket a felhőre való áttérésre, és lehetővé teszik a partnerek számára a hibrid felhőalapú környezetekhez szükséges rugalmasságot.</span><span class="sxs-lookup"><span data-stu-id="c15ad-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="c15ad-452">A digitális átalakítás folytatásakor a következő módosításokat tesszük közzé:</span><span class="sxs-lookup"><span data-stu-id="c15ad-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="c15ad-453">2021. július 1-jén: a program nem ad hozzá új SKU-t, terméket vagy előléptetést az Open szoftverlicenc-árlista listájához.</span><span class="sxs-lookup"><span data-stu-id="c15ad-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="c15ad-454">Július 7., 2021: két kereskedelmi ajánlat, valódi Windows-és Visual Studio Professional-és nyilvános szektor-ajánlatok (kormányzati, oktatási és nonprofit – lásd a [bejelentést](./2020-december.md#9)) a CSP Perpetual Software Prices listához lesznek hozzáadva.</span><span class="sxs-lookup"><span data-stu-id="c15ad-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="c15ad-455">Az árlista a partner Center [értékesítési > díjszabása & ajánlatok](https://partnercenter.microsoft.com/pcv/sales) oldalának szoftver szakaszában található, és ezen a napon újra közzé lesz téve.</span><span class="sxs-lookup"><span data-stu-id="c15ad-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="c15ad-456">A CSP-program evolúciójának és a licencelési program változásának részletes ismertetését az alábbi, **következő lépésekben** találhatja meg.</span><span class="sxs-lookup"><span data-stu-id="c15ad-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c15ad-457">További lépések:</span><span class="sxs-lookup"><span data-stu-id="c15ad-457">Next Steps:</span></span>

- <span data-ttu-id="c15ad-458">CSP-program evolúciója: Tekintse át az [örökös szoftvereket a Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) készenléti anyagaiban.</span><span class="sxs-lookup"><span data-stu-id="c15ad-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="c15ad-459">Ezzel a [készültségi térképsel](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) gyorsan megtalálhatja a szerepkörének megfelelő információkat.</span><span class="sxs-lookup"><span data-stu-id="c15ad-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="c15ad-460">A licencelési program módosításainak megnyitása: Tekintse át a [CSP-program evolúcióját, és nyissa meg a licencelési program változásait](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) .</span><span class="sxs-lookup"><span data-stu-id="c15ad-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="c15ad-461">Ezzel a [készültségi térképsel](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) gyorsan megtalálhatja a szerepkörének megfelelő információkat.</span><span class="sxs-lookup"><span data-stu-id="c15ad-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-462">Kérdések</span><span class="sxs-lookup"><span data-stu-id="c15ad-462">Questions</span></span>

<span data-ttu-id="c15ad-463">További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeit.</span><span class="sxs-lookup"><span data-stu-id="c15ad-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="c15ad-464">Frissítés korábbi bejelentésre: prémium szintű felmérések, a megfelelőségi vezető bővítménye</span><span class="sxs-lookup"><span data-stu-id="c15ad-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-465">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-465">Categories</span></span>

- <span data-ttu-id="c15ad-466">Dátum: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="c15ad-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="c15ad-467">Vállalkozás fejlesztése</span><span class="sxs-lookup"><span data-stu-id="c15ad-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-468">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-468">Summary</span></span>

<span data-ttu-id="c15ad-469">A próbaverziós ajánlatokat nem lehet listázni az árlista alapján, és el lesznek távolítva.</span><span class="sxs-lookup"><span data-stu-id="c15ad-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-470">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-470">Impacted audience</span></span>

<span data-ttu-id="c15ad-471">Felhőalapú megoldás-szolgáltatón keresztül lebonyolított partnerek</span><span class="sxs-lookup"><span data-stu-id="c15ad-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-472">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-472">Details</span></span>

<span data-ttu-id="c15ad-473">A próbaverziós ajánlatokat nem tartalmazza az árlista.</span><span class="sxs-lookup"><span data-stu-id="c15ad-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="c15ad-474">Ezeket a rendszer eltávolítja a 2021-es árlista-listából.</span><span class="sxs-lookup"><span data-stu-id="c15ad-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="c15ad-475">Az eredeti hirdetmény [itt](./2021-february.md#4)található.</span><span class="sxs-lookup"><span data-stu-id="c15ad-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="c15ad-476">További források</span><span class="sxs-lookup"><span data-stu-id="c15ad-476">Additional resources</span></span>

- [<span data-ttu-id="c15ad-477">Az E5 biztonsági és megfelelőségi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c15ad-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="c15ad-478">Értékelések készítése és kezelése a Microsoft megfelelőségi kezelőjében – Microsoft 365 megfelelőség</span><span class="sxs-lookup"><span data-stu-id="c15ad-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="c15ad-479">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-479">Next steps</span></span>

<span data-ttu-id="c15ad-480">Tekintse át a témakör erőforrásait, és ossza meg ezeket az információkat a szervezete megfelelő szereplőivel.</span><span class="sxs-lookup"><span data-stu-id="c15ad-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-481">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-481">Questions?</span></span>

<span data-ttu-id="c15ad-482">Az ajánlatokkal kapcsolatos kérdésekben keresse meg a megfelelő Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="c15ad-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="c15ad-483">Megoldásait áttelepítheti egy kereskedelmi partnertől (OCP) a Microsoft kereskedelmi Marketplace-re (GTM)</span><span class="sxs-lookup"><span data-stu-id="c15ad-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-484">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-484">Categories</span></span>

- <span data-ttu-id="c15ad-485">Dátum: 2021-03-12</span><span class="sxs-lookup"><span data-stu-id="c15ad-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="c15ad-486">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-487">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-487">Summary</span></span>

<span data-ttu-id="c15ad-488">2021. március 29-én elkezdjük korlátozni a kereskedelmi partneri (OCP) piacra lépéseit (GTM).</span><span class="sxs-lookup"><span data-stu-id="c15ad-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="c15ad-489">Javasoljuk, hogy telepítse át megoldásait a kereskedelmi piactérre a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="c15ad-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-490">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-490">Impacted audience</span></span>

<span data-ttu-id="c15ad-491">OCP GTM-megoldásokkal közösen értékesítő szervezetek</span><span class="sxs-lookup"><span data-stu-id="c15ad-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-492">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-492">Details</span></span>

<span data-ttu-id="c15ad-493">2020 decemberében kezdtük el utunkat a Microsoft OCP GTM eszközről a Microsoft kereskedelmi piactérről a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="c15ad-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="c15ad-494">Ez az áttérés kibővíti a kereskedelmi piactér képességeit, ahol több millió ügyfél számára is kiterjesztheti megoldásait, és kétirányú módon megoszthatja a lehetőségeket más Microsoft-és partner-értékesítővel, és közösen értékesítheti az innovatív megoldásokat.</span><span class="sxs-lookup"><span data-stu-id="c15ad-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="c15ad-495">Az áttérés következő mérföldköve a 2021. március 29-én kerül megadásra.</span><span class="sxs-lookup"><span data-stu-id="c15ad-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="c15ad-496">Ez az, amikor elkezdi megtapasztalni a korlátozott OCP GTM képességeket, és egyes mezők csak olvashatók lesznek.</span><span class="sxs-lookup"><span data-stu-id="c15ad-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="c15ad-497">Ha jelenleg a OCP GTM-megoldásokkal együtt értékesíti a megoldásokat, javasoljuk, hogy a megoldásait a kereskedelmi piactérre telepítse át, hogy kiaknázza a képességeit, és egyszerűsítse a közzétételi élményt.</span><span class="sxs-lookup"><span data-stu-id="c15ad-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="c15ad-498">A kereskedelmi piactérre való áttéréssel a partneri központ az elsődleges cél a közös értékesítésű közzétételi élmény.</span><span class="sxs-lookup"><span data-stu-id="c15ad-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="c15ad-499">Így tovább bővítheti üzleti tevékenységét úgy, hogy a Microsoft-termékekhez hasonló csatornákkal és a termékkel kapcsolatos felhasználói élményekkel összeköti megoldásait közös ügyfeleinkkel.</span><span class="sxs-lookup"><span data-stu-id="c15ad-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="c15ad-500">[További információ a kereskedelmi piactérről](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="c15ad-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="c15ad-501">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-501">Next steps</span></span>

- <span data-ttu-id="c15ad-502">Ha még nem helyezte át a megoldásait, kövesse az [áttérési útmutatóban](/azure/marketplace/co-sell-solution-migration) részletezett utasításokat, vagy tekintse meg az összes áttelepítési tevékenység befejezéséhez szükséges [útmutatót, és](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) kezdje el közzétenni a megoldás (oka) t a kereskedelmi piactéren.</span><span class="sxs-lookup"><span data-stu-id="c15ad-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="c15ad-503">A OCP-GTM korlátozott képességekkel kapcsolatos kérdéseivel kapcsolatban tekintse meg a [Microsoft kereskedelmi piactéren feltett gyakori kérdések című szakaszban közzétett közös értékesítésre vonatkozó követelményeket](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span><span class="sxs-lookup"><span data-stu-id="c15ad-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="c15ad-504">(Lásd a "OCP GTM korlátozott képességek" című szakaszt, amely 2021. március 29-én kezdődik. ")</span><span class="sxs-lookup"><span data-stu-id="c15ad-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-505">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-505">Questions?</span></span>

<span data-ttu-id="c15ad-506">Ha bármilyen kérdése van, vagy további információra van szüksége, forduljon az [ügyfélszolgálathoz](https://partner.microsoft.com/support/?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="c15ad-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="c15ad-507">Az új kereskedelmi élmény kibővítése az Azure-beli Cloud Solution Provider (CSP) program keretében</span><span class="sxs-lookup"><span data-stu-id="c15ad-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-508">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-508">Categories</span></span>

- <span data-ttu-id="c15ad-509">Dátum: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="c15ad-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="c15ad-510">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-511">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-511">Impacted audience</span></span>

<span data-ttu-id="c15ad-512">Az Oroszországban lévő összes partner a Cloud Solution Provider (CSP) programon keresztül lebonyolítja a tranzakciót.</span><span class="sxs-lookup"><span data-stu-id="c15ad-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-513">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-513">Details</span></span>

<span data-ttu-id="c15ad-514">A 10 2021. március 1-től örömmel jelentjük be, hogy elérhetővé tettük az **új kereskedelmi élményt az Azure-beli CSP-ben Oroszországban**.</span><span class="sxs-lookup"><span data-stu-id="c15ad-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="c15ad-515">Ez a tapasztalat egyszerűsíti és javítja az Azure-szolgáltatások vásárlásának és felhasználásának módját.</span><span class="sxs-lookup"><span data-stu-id="c15ad-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="c15ad-516">Emellett a CSP program partnereinek is egységes áttekintést nyújt az Azure díjszabásáról az értékesítési mozgások során, a globális konzisztencia, a számlázási dátum-igazítás és a Azure Cost Management elérésének USD-díja.</span><span class="sxs-lookup"><span data-stu-id="c15ad-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c15ad-517">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-517">Next steps</span></span>

<span data-ttu-id="c15ad-518">Számos erőforrás érhető el az új Azure-beli kereskedelmi élmény bevezetéséhez és további információk biztosításához.</span><span class="sxs-lookup"><span data-stu-id="c15ad-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="c15ad-519">A legújabb gyakori kérdések, a paklik, a videók és egyebek a [CSP program frissítésének erőforrás-gyűjteményében](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)találhatók.</span><span class="sxs-lookup"><span data-stu-id="c15ad-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="c15ad-520">A partner Center szoftverlicenc-kulcsa és a letöltés teljesítése</span><span class="sxs-lookup"><span data-stu-id="c15ad-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-521">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-521">Categories</span></span>

- <span data-ttu-id="c15ad-522">Dátum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="c15ad-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="c15ad-523">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-524">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-524">Summary</span></span>

<span data-ttu-id="c15ad-525">A partner Center szoftver letöltése és a licencek kulcsának teljesítésére szolgáló képesség vissza lett állítani.</span><span class="sxs-lookup"><span data-stu-id="c15ad-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-526">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-526">Impacted audience</span></span>

<span data-ttu-id="c15ad-527">Minden olyan felhőalapú megoldás-szolgáltatói (CSP) partner, amely az örökös és a kiszolgálói előfizetési szoftverek rendeléseit a partner centeren keresztül</span><span class="sxs-lookup"><span data-stu-id="c15ad-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-528">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-528">Details</span></span>

<span data-ttu-id="c15ad-529">A partneri visszajelzések megválaszolásával a visszaállítja teljesítjük a szoftver-és licenckulcs beszerzését az örökös és a kiszolgálói előfizetési szoftverek rendeléseihez.</span><span class="sxs-lookup"><span data-stu-id="c15ad-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="c15ad-530">A rendszer a korábbi állapotába állítja vissza, mielőtt a 2021. január 19-én megszűnik.</span><span class="sxs-lookup"><span data-stu-id="c15ad-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="c15ad-531">(Lásd a [közleményt](2020-september.md#17).)</span><span class="sxs-lookup"><span data-stu-id="c15ad-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="c15ad-532">Vegye figyelembe, hogy a szoftverlicenc-kulcsok és a letöltési hivatkozások értékesek és rendkívül keresettek a szellemi tulajdonban lévő eszközök után.</span><span class="sxs-lookup"><span data-stu-id="c15ad-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="c15ad-533">Ha kiszivárgott, gyorsan kimerítheti az aktiválási korlátokat, és negatív ügyfél-és partneri élményt eredményezhet.</span><span class="sxs-lookup"><span data-stu-id="c15ad-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c15ad-534">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-534">Next steps</span></span>

<span data-ttu-id="c15ad-535">Tekintse át a következő forrásokat a használati utasításokhoz, valamint a szoftveres kulcs terjesztésével kapcsolatos fontos útmutatást:</span><span class="sxs-lookup"><span data-stu-id="c15ad-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="c15ad-536">Helyszíni szoftverek értékesítése a CSP programon keresztül</span><span class="sxs-lookup"><span data-stu-id="c15ad-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="c15ad-537">A [partner Center új kereskedelmi üzemeltetési útmutatója](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (lásd: **útmutató a szoftveres kulcs terjesztéséhez** .)</span><span class="sxs-lookup"><span data-stu-id="c15ad-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-538">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-538">Questions?</span></span>

<span data-ttu-id="c15ad-539">Ha további kérdése van a nyilatkozattal kapcsolatban, tekintse meg a megfelelő Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="c15ad-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="c15ad-540">A partner értékesítési összekötő (PSC) és a partner Center közötti ajánlatok áttelepíthetők</span><span class="sxs-lookup"><span data-stu-id="c15ad-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-541">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-541">Categories</span></span>

- <span data-ttu-id="c15ad-542">Dátum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="c15ad-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="c15ad-543">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-544">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-544">Summary</span></span>

<span data-ttu-id="c15ad-545">A partner Sales-kapcsolódás (PSC) a 2021-as naptól kezdődő írásvédett hozzáférésre vált, ezért javasoljuk, hogy kezdje el áttelepíteni az ajánlatokat a PSC-ből a partneri központba.</span><span class="sxs-lookup"><span data-stu-id="c15ad-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-546">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-546">Impacted audience</span></span>

<span data-ttu-id="c15ad-547">Partnerek a PSC-ben található ügyletekkel</span><span class="sxs-lookup"><span data-stu-id="c15ad-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-548">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-548">Details</span></span>

<span data-ttu-id="c15ad-549">A növekedés iránti közös elkötelezettségünk részeként a **Microsofttal közösen értékesítjük** a **felderített, szakértelmét, és kiterjesztjük** az ügyfél-lábnyomot a pozitív ügyfelek eredményeire.</span><span class="sxs-lookup"><span data-stu-id="c15ad-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="c15ad-550">Ha átlagosan **3,5-szor gyorsabb** , mint a normál, a partner Center közös értékesítésű felhasználói élményének kezelése lehetővé teszi a közvetlen ügyfél-, partner-és Microsoft-értékesítői csatornák értékesítését, és egy helyen kezelheti a teljes átirányítási folyamatot.</span><span class="sxs-lookup"><span data-stu-id="c15ad-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="c15ad-551">A **PSC** a **2021**-as naptól kezdve **csak olvasási hozzáférésre** kerül át, ezért javasoljuk, hogy indítsa el a partneri központba való áttérést</span><span class="sxs-lookup"><span data-stu-id="c15ad-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="c15ad-552">A Microsoft és a megfelelő eladó közötti megosztások **pontosabb irányítása** a szükséges segítségnyújtási típus alapján.</span><span class="sxs-lookup"><span data-stu-id="c15ad-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="c15ad-553">**Előzetes támogatási jogosultságok érvényesítése** az ösztönzőre jogosult megoldások esetében, valamint az ISV kapcsolódási program feltételeinek teljesítése, a jóváhagyási folyamat és a végrehajtás végleges igazolása (PoE) igazolása.</span><span class="sxs-lookup"><span data-stu-id="c15ad-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="c15ad-554">**Zökkenőmentes felhasználói élmény** , amellyel egyetlen helyen kezelheti az összes közös értékesítéssel kapcsolatos lehetőséget és értékesítési minősítéssel rendelkező érdeklődőket.</span><span class="sxs-lookup"><span data-stu-id="c15ad-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="c15ad-555">Nemrégiben új funkciókat is hozzáadott a partner Centerben, hogy segítséget nyújtson az áthelyezéshez:</span><span class="sxs-lookup"><span data-stu-id="c15ad-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="c15ad-556">Tömeges műveletek közös értékesítési lehetőségekhez</span><span class="sxs-lookup"><span data-stu-id="c15ad-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="c15ad-557">Az [ügylet áttelepítési funkciója](../psc-to-pc.md) (lásd: a **PSC-ajánlatok áttelepítése** szakasz)</span><span class="sxs-lookup"><span data-stu-id="c15ad-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="c15ad-558">Az értékesítési csapatoknak több idő áll rendelkezésére a partner Center közös értékesítéssel kapcsolatos tapasztalataira, így az érdeklődők és a lehetőségek kiépítésére, az ajánlatok bezárására és a tartós ügyfélkapcsolatok létrehozására összpontosítanak.</span><span class="sxs-lookup"><span data-stu-id="c15ad-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c15ad-559">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-559">Next steps</span></span>

<span data-ttu-id="c15ad-560">A partneri központ [áttérési útmutatója](../psc-to-pc.md) végigvezeti Önt az ajánlatok PSC-ből a partneri központba való átirányításának lépésein.</span><span class="sxs-lookup"><span data-stu-id="c15ad-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-561">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-561">Questions?</span></span>

<span data-ttu-id="c15ad-562">További kérdésekért forduljon az [ügyfélszolgálathoz](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="c15ad-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="c15ad-563">Új Microsoft Dynamics 365-termékek és-ajánlatok, amelyek az 2021. április 1-jén érhetők el</span><span class="sxs-lookup"><span data-stu-id="c15ad-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-564">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-564">Categories</span></span>

- <span data-ttu-id="c15ad-565">Dátum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="c15ad-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="c15ad-566">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-567">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-567">Summary</span></span>

<span data-ttu-id="c15ad-568">2021. április 1-jén a Microsoft számos új terméket és ajánlatot indít el a Cloud Solution Provider (CSP) programhoz.</span><span class="sxs-lookup"><span data-stu-id="c15ad-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-569">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-569">Impacted audience</span></span>

<span data-ttu-id="c15ad-570">Minden partner a Cloud Solution Provider (CSP) programon keresztül lebonyolít</span><span class="sxs-lookup"><span data-stu-id="c15ad-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-571">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-571">Details</span></span>

<span data-ttu-id="c15ad-572">2021. április 1-jén a Microsoft a következő új termékeket és ajánlatokat fogja elindítani:</span><span class="sxs-lookup"><span data-stu-id="c15ad-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="c15ad-573">Felhasználónként Power BI Premium</span><span class="sxs-lookup"><span data-stu-id="c15ad-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="c15ad-574">Az ügyfelek hang-és marketing-felhasználói előfizetési licenc földrajzi és szegmensek bővítése</span><span class="sxs-lookup"><span data-stu-id="c15ad-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="c15ad-575">**Felhasználónként Power BI Premium**</span><span class="sxs-lookup"><span data-stu-id="c15ad-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="c15ad-576">A Microsoft az első felhasználónkénti Power BI Premium ajánlatokat fogja bevezetni.</span><span class="sxs-lookup"><span data-stu-id="c15ad-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="c15ad-577">A Power BI Premium jelenleg csak egy kapacitás-konstrukcióban értékesíti.</span><span class="sxs-lookup"><span data-stu-id="c15ad-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="c15ad-578">A felhasználónként Power BI Premium hozzáférést biztosít a vállalati üzleti intelligencia (BI) és az elemzési funkciókhoz.</span><span class="sxs-lookup"><span data-stu-id="c15ad-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="c15ad-579">A rugalmas egyéni munkaállomás-licencelés kis-és közepes méretű vállalkozások számára is elérhető.</span><span class="sxs-lookup"><span data-stu-id="c15ad-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="c15ad-580">Tekintse át a [Power bi kiadásának részleteit](/power-platform-release-plan/2020wave2/power-bi/planned-features) , és tudjon meg többet az ajánlatról.</span><span class="sxs-lookup"><span data-stu-id="c15ad-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="c15ad-581">**Ajánlat részletei**</span><span class="sxs-lookup"><span data-stu-id="c15ad-581">**Offer details**</span></span>

<span data-ttu-id="c15ad-582">Vegye figyelembe, hogy az ajánlat neve kis mértékben eltér a árlista előzetes verziójától.</span><span class="sxs-lookup"><span data-stu-id="c15ad-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="c15ad-583">Ajánlat neve</span><span class="sxs-lookup"><span data-stu-id="c15ad-583">Offer name</span></span> | <span data-ttu-id="c15ad-584">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="c15ad-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="c15ad-585">Felhasználónként Power BI Premium</span><span class="sxs-lookup"><span data-stu-id="c15ad-585">Power BI Premium Per User</span></span> | <span data-ttu-id="c15ad-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="c15ad-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="c15ad-587">Felhasználónként Power BI Premium oktatóknak</span><span class="sxs-lookup"><span data-stu-id="c15ad-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="c15ad-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="c15ad-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="c15ad-589">Felhasználónként Power BI Premium tanulók számára</span><span class="sxs-lookup"><span data-stu-id="c15ad-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="c15ad-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="c15ad-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="c15ad-591">Felhasználónkénti Power BI Premium (nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="c15ad-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="c15ad-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="c15ad-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="c15ad-593">Felhasználónként Power BI Premium Add-On</span><span class="sxs-lookup"><span data-stu-id="c15ad-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="c15ad-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="c15ad-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="c15ad-595">Power BI Premium felhasználói Add-On oktatóknak</span><span class="sxs-lookup"><span data-stu-id="c15ad-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="c15ad-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="c15ad-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="c15ad-597">Power BI Premium felhasználónként Add-On diákoknak</span><span class="sxs-lookup"><span data-stu-id="c15ad-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="c15ad-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="c15ad-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="c15ad-599">Felhasználónkénti Add-On Power BI Premium (nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="c15ad-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="c15ad-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="c15ad-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="c15ad-601">**Az ügyfelek hang-és marketing-felhasználói előfizetési licenc földrajzi és szegmensek bővítése**</span><span class="sxs-lookup"><span data-stu-id="c15ad-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="c15ad-602">A decemberi 2020-es indítás után a Dynamics 365-ügyfelek hang-és marketing-felhasználói előfizetési licenc ajánlatai új országok és több nonprofit és oktatási SKU hozzáadására lettek kialakítva.</span><span class="sxs-lookup"><span data-stu-id="c15ad-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="c15ad-603">Ajánlat neve</span><span class="sxs-lookup"><span data-stu-id="c15ad-603">Offer name</span></span> | <span data-ttu-id="c15ad-604">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="c15ad-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="c15ad-605">Dynamics 365-ügyfél hangalapú felhasználói előfizetési licenc (nonprofit személyzet díjszabása)</span><span class="sxs-lookup"><span data-stu-id="c15ad-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="c15ad-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="c15ad-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="c15ad-607">Dynamics 365-ügyfelek hang-felhasználói előfizetési licenc az oktatók számára</span><span class="sxs-lookup"><span data-stu-id="c15ad-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="c15ad-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="c15ad-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="c15ad-609">A következő lapokon további információkat talál az ajánlatokról:</span><span class="sxs-lookup"><span data-stu-id="c15ad-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="c15ad-610">Dynamics 365 ügyfél-szolgáltatás hangpostájának kezdőlapja</span><span class="sxs-lookup"><span data-stu-id="c15ad-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="c15ad-611">Dynamics 365 marketing Kezdőlap</span><span class="sxs-lookup"><span data-stu-id="c15ad-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="c15ad-612">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-612">Next steps</span></span>

<span data-ttu-id="c15ad-613">Tekintse át a témakör erőforrásait, és ossza meg ezeket az információkat a szervezete megfelelő szereplőivel.</span><span class="sxs-lookup"><span data-stu-id="c15ad-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="c15ad-614">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-614">Questions?</span></span>

<span data-ttu-id="c15ad-615">Az ajánlatokkal kapcsolatos bármilyen kérdés esetén keresse meg a megfelelő Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="c15ad-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="c15ad-616">A Microsoft Universal Print már elérhető néhány lakosztályban</span><span class="sxs-lookup"><span data-stu-id="c15ad-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="c15ad-617">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="c15ad-617">Categories</span></span>

- <span data-ttu-id="c15ad-618">Dátum: 2021-03-33</span><span class="sxs-lookup"><span data-stu-id="c15ad-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="c15ad-619">Képességek</span><span class="sxs-lookup"><span data-stu-id="c15ad-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c15ad-620">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="c15ad-620">Summary</span></span>

<span data-ttu-id="c15ad-621">A Microsoft Universal Print elérhető lesz a Select Microsoft 365 Suite-ban, valamint önálló bővítményként, 2021. március 1-től.</span><span class="sxs-lookup"><span data-stu-id="c15ad-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c15ad-622">Érintett közönség</span><span class="sxs-lookup"><span data-stu-id="c15ad-622">Impacted audience</span></span>

<span data-ttu-id="c15ad-623">Minden partner a Cloud Solution Provider (CSP) programon keresztül lebonyolít</span><span class="sxs-lookup"><span data-stu-id="c15ad-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="c15ad-624">Részletek</span><span class="sxs-lookup"><span data-stu-id="c15ad-624">Details</span></span>

<span data-ttu-id="c15ad-625">Az [univerzális nyomtatás](https://aka.ms/universalprint) egy Microsoft 365 nyomtatási szolgáltatás, amely eltávolítja a helyszíni nyomtatókiszolgálók szükségességét, és lehetővé teszi a Windows-eszközök számára az Azure-ban regisztrált nyomtatókhoz való nyomtatást.</span><span class="sxs-lookup"><span data-stu-id="c15ad-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="c15ad-626">A tranzakció 2021. március 1-től lesz elérhető.</span><span class="sxs-lookup"><span data-stu-id="c15ad-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="c15ad-627">A feldolgozók kihasználhatják az illesztőprogram nélküli nyomtatást, a egyszerűsített helymeghatározást, valamint az intuitív nyomtatási élményt tanulási görbe nélkül.</span><span class="sxs-lookup"><span data-stu-id="c15ad-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="c15ad-628">A Azure Active Directoryhoz (Azure AD) csatlakoztatott eszközök a meglévő Azure AD-beli hitelesítő adatokat használják a biztonságos nyomtatáshoz.</span><span class="sxs-lookup"><span data-stu-id="c15ad-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="c15ad-629">A rendszergazdák a Azure Portal használatával kezelhetik a nyomtatást, és könnyen csatlakoztathatók a nyomtatók az univerzális nyomtatás natív támogatásával.</span><span class="sxs-lookup"><span data-stu-id="c15ad-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="c15ad-630">Az univerzális nyomtatás a nem kompatibilis nyomtatókra is telepíthető univerzális nyomtatási összekötő szoftver használatával.</span><span class="sxs-lookup"><span data-stu-id="c15ad-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="c15ad-631">Az univerzális nyomtatás a Windows E3, a3, E5 és a5 nyelven, valamint Microsoft 365 a BP, az F3, az E3, az a3, az E5 és az A5 nyelven is visszatöltötte.</span><span class="sxs-lookup"><span data-stu-id="c15ad-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="c15ad-632">**Ajánlat részletei**</span><span class="sxs-lookup"><span data-stu-id="c15ad-632">**Offer details**</span></span>

<span data-ttu-id="c15ad-633">Vegye figyelembe, hogy az ajánlat neve kis mértékben eltér a árlista előzetes verziójától.</span><span class="sxs-lookup"><span data-stu-id="c15ad-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="c15ad-634">Ajánlat neve</span><span class="sxs-lookup"><span data-stu-id="c15ad-634">Offer name</span></span> | <span data-ttu-id="c15ad-635">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="c15ad-635">Offer ID</span></span> | <span data-ttu-id="c15ad-636">Anyag azonosítója</span><span class="sxs-lookup"><span data-stu-id="c15ad-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="c15ad-637">Univerzális nyomtatási kötet bővítmény (500 feladat) – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c15ad-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="c15ad-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="c15ad-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="c15ad-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="c15ad-639">9BI-00004</span></span>   |
| <span data-ttu-id="c15ad-640">Univerzális nyomtatási hangerő bővítmény (500-es feladat) az oktatók számára – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c15ad-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="c15ad-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="c15ad-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="c15ad-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="c15ad-642">9BK-00004</span></span>   |
| <span data-ttu-id="c15ad-643">Univerzális nyomtatási kötet bővítmény (500 feladat) – Windows</span><span class="sxs-lookup"><span data-stu-id="c15ad-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="c15ad-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="c15ad-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="c15ad-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="c15ad-645">9BI-00002</span></span>   |
| <span data-ttu-id="c15ad-646">Univerzális nyomtatási hangerő bővítmény (500 feladat) a kari-Windows rendszerhez</span><span class="sxs-lookup"><span data-stu-id="c15ad-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="c15ad-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="c15ad-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="c15ad-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="c15ad-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="c15ad-649">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c15ad-649">Next steps</span></span>

<span data-ttu-id="c15ad-650">Ismerkedjen meg az árlista és az [univerzális nyomtatás áttekintése](/universal-print/fundamentals/universal-print-whatis)szolgáltatással.</span><span class="sxs-lookup"><span data-stu-id="c15ad-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="c15ad-651">Ossza meg ezeket az információkat a szervezet összes megfelelő ügyfelével.</span><span class="sxs-lookup"><span data-stu-id="c15ad-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="c15ad-652">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="c15ad-652">Questions?</span></span>

<span data-ttu-id="c15ad-653">Az ajánlatokkal kapcsolatos bármilyen kérdés esetén keresse meg a megfelelő Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="c15ad-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
