---
title: 2021. márciusi bejelentések
description: A Microsoft 2021. márciusi közleményei Partnerközpont új képességeket, promóciókat, ajánlatokat, piacokat vagy a meglévő ajánlatok változásait is beleértve.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: b503e928b1491d5c2c70ac52460080f9e1ba91b8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150114"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="ad56e-103">2021. márciusi bejelentések</span><span class="sxs-lookup"><span data-stu-id="ad56e-103">March 2021 announcements</span></span>

<span data-ttu-id="ad56e-104">Ez az oldal a Microsoft 2021. márciusi Partnerközpont bejelentését mutatja be.</span><span class="sxs-lookup"><span data-stu-id="ad56e-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a><span data-ttu-id="ad56e-105">Készenlét: A Felhőszolgáltató (CSP) ügyfélcím-érvényesítési API-jának változásai júniusban érvénybe fognak tolni; tesztelési képesség már elérhető</span><span class="sxs-lookup"><span data-stu-id="ad56e-105">Readiness: Changes to the Cloud Solution Provider (CSP) customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-106">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-106">Categories</span></span>

- <span data-ttu-id="ad56e-107">Dátum: 2021-03-30</span><span class="sxs-lookup"><span data-stu-id="ad56e-107">Date: 2021-03-30</span></span>
- <span data-ttu-id="ad56e-108">Készenlét</span><span class="sxs-lookup"><span data-stu-id="ad56e-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-109">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-109">Summary</span></span>

<span data-ttu-id="ad56e-110">Annak érdekében, hogy a partnerek és az ügyfelek bizalom alapján futtassanak üzleti munkájukat, meghívjuk a partnereket, hogy teszteljék a Validate Address API módosításait a világ minden országában.</span><span class="sxs-lookup"><span data-stu-id="ad56e-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-111">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-111">Impacted audience</span></span>

<span data-ttu-id="ad56e-112">A CSP közvetlen számlázási partnerek és közvetett szolgáltatók, akik új ügyfelek címének részleteit hozják létre vagy frissítik.</span><span class="sxs-lookup"><span data-stu-id="ad56e-112">CSP direct bill partners and indirect providers who create new or update existing customers address details.</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-113">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-113">Details</span></span>

<span data-ttu-id="ad56e-114">A Microsoft megbízhatósági kapcsolaton fut.</span><span class="sxs-lookup"><span data-stu-id="ad56e-114">Microsoft runs on trust.</span></span> <span data-ttu-id="ad56e-115">Elkötelezettek vagyunk amellett, hogy megfelelő, biztonságos és biztonságos módszert biztosítsunk az ügyfélcímek érvényesítéséhez az ügyfél-előfizetések tranzakciója során a CSP-programban.</span><span class="sxs-lookup"><span data-stu-id="ad56e-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="ad56e-116">2021. március 31-én bevezettük a Validate Address API módosításait, amelyek tesztelésére hívtuk meg a partnereket, mielőtt a 2021. júniusi változásokat bevezettük volna.</span><span class="sxs-lookup"><span data-stu-id="ad56e-116">As of March 31, 2021, we’ve introduced changes to the Validate Address API that we invited partners to test, prior to going live with the changes in June 2021.</span></span>

<span data-ttu-id="ad56e-117">A módosítások csak a Validate Address API-t érintik.</span><span class="sxs-lookup"><span data-stu-id="ad56e-117">Changes affect the Validate Address API only.</span></span> <span data-ttu-id="ad56e-118">Az Ügyfél és a Számlázási profil API-k létrehozása nem lesz hatással.</span><span class="sxs-lookup"><span data-stu-id="ad56e-118">Create Customer and Update Billing Profile APIs aren’t impacted.</span></span>

<span data-ttu-id="ad56e-119">A válasz a következő állapotüzenetek egyikét adja vissza:</span><span class="sxs-lookup"><span data-stu-id="ad56e-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="ad56e-120">Állapot</span><span class="sxs-lookup"><span data-stu-id="ad56e-120">Status</span></span>     | <span data-ttu-id="ad56e-121">Leírás</span><span class="sxs-lookup"><span data-stu-id="ad56e-121">Description</span></span> |    <span data-ttu-id="ad56e-122">A visszaadott javasolt címek száma</span><span class="sxs-lookup"><span data-stu-id="ad56e-122">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="ad56e-123">Ellenőrzött szállításra használható</span><span class="sxs-lookup"><span data-stu-id="ad56e-123">Verified shippable</span></span> | <span data-ttu-id="ad56e-124">A cím ellenőrizve van, és szállítható a címre.</span><span class="sxs-lookup"><span data-stu-id="ad56e-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="ad56e-125">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="ad56e-125">Single</span></span> |
|<span data-ttu-id="ad56e-126">Ellenőrzött</span><span class="sxs-lookup"><span data-stu-id="ad56e-126">Verified</span></span> | <span data-ttu-id="ad56e-127">A cím ellenőrizve van.</span><span class="sxs-lookup"><span data-stu-id="ad56e-127">Address is verified.</span></span> | <span data-ttu-id="ad56e-128">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="ad56e-128">Single</span></span> |
|<span data-ttu-id="ad56e-129">Beavatkozás szükséges</span><span class="sxs-lookup"><span data-stu-id="ad56e-129">Interaction required</span></span> | <span data-ttu-id="ad56e-130">A javasolt cím jelentős mértékben módosult, és a felhasználó megerősítését kell kér.</span><span class="sxs-lookup"><span data-stu-id="ad56e-130">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="ad56e-131">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="ad56e-131">Single</span></span> |
|<span data-ttu-id="ad56e-132">Utca részleges</span><span class="sxs-lookup"><span data-stu-id="ad56e-132">Street partial</span></span> | <span data-ttu-id="ad56e-133">A címben megadott utca részleges, és további információra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="ad56e-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="ad56e-134">Multiple – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="ad56e-134">Multiple—maximum of three</span></span> |
|<span data-ttu-id="ad56e-135">Részleges helyszín</span><span class="sxs-lookup"><span data-stu-id="ad56e-135">Premises partial</span></span> | <span data-ttu-id="ad56e-136">Az adott helyszín (épületszám, csomagszám stb.) részleges, és további információra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="ad56e-136">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="ad56e-137">Multiple – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="ad56e-137">Multiple—maximum of three</span></span> |
|<span data-ttu-id="ad56e-138">Többszörös</span><span class="sxs-lookup"><span data-stu-id="ad56e-138">Multiple</span></span> | <span data-ttu-id="ad56e-139">Több mező is részleges a címben (beleértve az utca részleges és a helyszíni részleges mezőket is).</span><span class="sxs-lookup"><span data-stu-id="ad56e-139">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="ad56e-140">Multiple – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="ad56e-140">Multiple—maximum of three</span></span> |
|<span data-ttu-id="ad56e-141">None</span><span class="sxs-lookup"><span data-stu-id="ad56e-141">None</span></span> | <span data-ttu-id="ad56e-142">A cím helytelen.</span><span class="sxs-lookup"><span data-stu-id="ad56e-142">Address is incorrect.</span></span> | <span data-ttu-id="ad56e-143">None</span><span class="sxs-lookup"><span data-stu-id="ad56e-143">None</span></span> |
|<span data-ttu-id="ad56e-144">Nincs ellenőrizve.</span><span class="sxs-lookup"><span data-stu-id="ad56e-144">Not validated</span></span> | <span data-ttu-id="ad56e-145">A címet nem sikerült elküldeni az érvényesítési folyamaton keresztül.</span><span class="sxs-lookup"><span data-stu-id="ad56e-145">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="ad56e-146">None</span><span class="sxs-lookup"><span data-stu-id="ad56e-146">None</span></span> |

<span data-ttu-id="ad56e-147">Az USA-nak az utókódja további 4 számjegyet + kötőjelet ad vissza – például: 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="ad56e-147">US post codes will return an additional 4 digits + hyphen - for example, 12345-6789.</span></span>

<span data-ttu-id="ad56e-148">Miután a Validate Address API-val elküldött egy címet ellenőrzésre, a rendszer a következő válaszsémát fogja visszaadni:</span><span class="sxs-lookup"><span data-stu-id="ad56e-148">Once an address is submitted for validation via the Validate Address API, the following response schema will be returned:</span></span>

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

<span data-ttu-id="ad56e-149">Nézze meg ezt a mintaválaszt.</span><span class="sxs-lookup"><span data-stu-id="ad56e-149">Take a look at this sample response.</span></span> <span data-ttu-id="ad56e-150">Vegye figyelembe, hogy az Egyesült Államok esetén a válasz egy további négyjegyű utótagot ad vissza az irányítószám sorhoz, ha csak öt számjegyet ad meg az irányítószámhoz.</span><span class="sxs-lookup"><span data-stu-id="ad56e-150">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

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

### <a name="next-steps"></a><span data-ttu-id="ad56e-151">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-151">Next steps</span></span>

- <span data-ttu-id="ad56e-152">Ossza meg a tesztgép bérlőazonosítóját az érintett szakértővel (Ali Mertki), hogy felveje a tesztjáratba, hogy megkezdje a frissítés előkészítését.</span><span class="sxs-lookup"><span data-stu-id="ad56e-152">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="ad56e-153">Ha vezérlőpult-szállítói (CPV) megoldást használ, tekintse meg a CPV-t.</span><span class="sxs-lookup"><span data-stu-id="ad56e-153">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-154">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-154">Questions?</span></span>

<span data-ttu-id="ad56e-155">Ha támogatásra van szüksége a Microsofttal kapcsolatos műveleteihez, a partnertámogatási Yammer-csoporthoz kell segítséget nyújtanunk.</span><span class="sxs-lookup"><span data-stu-id="ad56e-155">If you need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

### <a name="change-log"></a><span data-ttu-id="ad56e-156">Változásnapló:</span><span class="sxs-lookup"><span data-stu-id="ad56e-156">Change log:</span></span>

- <span data-ttu-id="ad56e-157">2020. március 31. : Eredeti közzététel</span><span class="sxs-lookup"><span data-stu-id="ad56e-157">March 31, 2020: Original publication</span></span>

- <span data-ttu-id="ad56e-158">2021. április 30.: A mintaválasz és az irányítószám részleteinek frissítései</span><span class="sxs-lookup"><span data-stu-id="ad56e-158">April 30, 2021: Updates for sample response and Zip code details</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="ad56e-159">Új Exchange felügyeleti központ (EAC) felhasználói élmény</span><span class="sxs-lookup"><span data-stu-id="ad56e-159">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-160">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-160">Categories</span></span>

- <span data-ttu-id="ad56e-161">Dátum: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="ad56e-161">Date: 2021-03-29</span></span>
- <span data-ttu-id="ad56e-162">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-162">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-163">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-163">Summary</span></span>

<span data-ttu-id="ad56e-164">2021. április 27-től az Exchange felügyeleti központ (EAC) új felhasználói élményt nyújt, amely javítja a felhasználók napi hatékonyságát.</span><span class="sxs-lookup"><span data-stu-id="ad56e-164">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-165">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-165">Impacted audience</span></span>

<span data-ttu-id="ad56e-166">Az Exchange-et a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ad56e-166">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-167">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-167">Details</span></span>

<span data-ttu-id="ad56e-168">2021. április 27-től az Exchange-hez Partnerközpont az új EAC-hoz lesznek átirányítva.</span><span class="sxs-lookup"><span data-stu-id="ad56e-168">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="ad56e-169">Ez az új felület jelenleg előzetes verzióként érhető el, és a rendszergazdák a klasszikus EAC jobb felső sarkában található váltógombot választva aktiválják ezt a felhasználói élményt.</span><span class="sxs-lookup"><span data-stu-id="ad56e-169">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="ad56e-170">Az összes oldalon megjelenő "Kipróbálom most" szalagcímre kattintva is navigálhat az új EAC-hoz.</span><span class="sxs-lookup"><span data-stu-id="ad56e-170">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="ad56e-171">Az új EAC előnyei többek között a következők:</span><span class="sxs-lookup"><span data-stu-id="ad56e-171">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="ad56e-172">Elemzések, jelentések és riasztási mechanizmusok hozzáadva a levélforgalomhoz kapcsolódó problémákhoz.</span><span class="sxs-lookup"><span data-stu-id="ad56e-172">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="ad56e-173">Személyre szabott irányítópultok a hatékonyság növelése érdekében.</span><span class="sxs-lookup"><span data-stu-id="ad56e-173">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="ad56e-174">Az új felhasználói élményben való eligazodás érdekében a videók az új EAC-& képzési útmutató szakaszában érhetők el. </span><span class="sxs-lookup"><span data-stu-id="ad56e-174">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="ad56e-175">Ezek áttekintést nyújtanak arról, hogyan használhatja a legjobban az új portált.</span><span class="sxs-lookup"><span data-stu-id="ad56e-175">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="ad56e-176">Ezzel a módosítással a klasszikus EAC-élmény nem lesz elavult.</span><span class="sxs-lookup"><span data-stu-id="ad56e-176">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="ad56e-177">A változások megvalósítása előtt értesítést kap.</span><span class="sxs-lookup"><span data-stu-id="ad56e-177">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ad56e-178">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-178">Next steps</span></span>

- <span data-ttu-id="ad56e-179">Tekintse meg az [ezzel a témakörvel](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)kapcsolatos forrásokat, ahol képernyőképeket készíthet az új felhasználói élményről.</span><span class="sxs-lookup"><span data-stu-id="ad56e-179">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="ad56e-180">Ossza meg ezt az információt a szervezet megfelelő érdekelt felével.</span><span class="sxs-lookup"><span data-stu-id="ad56e-180">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="ad56e-181">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-181">Questions?</span></span>

<span data-ttu-id="ad56e-182">A változásokkal kapcsolatos kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="ad56e-182">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="ad56e-183">Microsoft Operations: A termékindítási naptár bevezetése</span><span class="sxs-lookup"><span data-stu-id="ad56e-183">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-184">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-184">Categories</span></span>

- <span data-ttu-id="ad56e-185">Dátum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="ad56e-185">Date: 2021-03-25</span></span>
- <span data-ttu-id="ad56e-186">Ajánlatok | Modern munkahely</span><span class="sxs-lookup"><span data-stu-id="ad56e-186">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-187">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-187">Summary</span></span>

<span data-ttu-id="ad56e-188">A microsoftos visszajelzésekre reagálva a Microsoft Operations leegyszerűsíti a termékbeindítások kommunikációját.</span><span class="sxs-lookup"><span data-stu-id="ad56e-188">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-189">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-189">Impacted audience</span></span>

<span data-ttu-id="ad56e-190">Felhőszolgáltató (CSP) partnerek</span><span class="sxs-lookup"><span data-stu-id="ad56e-190">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-191">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-191">Details</span></span>

<span data-ttu-id="ad56e-192">A Microsoft elkötelezett amellett, hogy folyamatosan javítsa a partneri élményeket.</span><span class="sxs-lookup"><span data-stu-id="ad56e-192">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="ad56e-193">Visszajelzést kaptunk Öntől, hogy túl sok információt kapott a Microsofttól, beleértve a termékbeindítások duplikált bejelentéseit is.</span><span class="sxs-lookup"><span data-stu-id="ad56e-193">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="ad56e-194">Visszajelzésére válaszul a Microsoft leegyszerűsíti a termékindítások készenlétét az új és meglévő ajánlatokhoz.</span><span class="sxs-lookup"><span data-stu-id="ad56e-194">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="ad56e-195">Mostantól a termékindítások egyetlen havi nézetét biztosítjuk, amely az Operations readiness erőforrás-katalógusban van közzétéve.</span><span class="sxs-lookup"><span data-stu-id="ad56e-195">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="ad56e-196">Ez a [havi termékindítási naptárnézet](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) felváltja az egyes termékindítási kommunikációt az Üzemeltetési készenlét erőforrás-katalógusban és a Partnerközpont közlemények között.</span><span class="sxs-lookup"><span data-stu-id="ad56e-196">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="ad56e-197">A termékindítási [](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) naptárt közösségi gyűjtemények, [](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)naptárnézetek [és](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated) [CSP-hírlevelek segítségével is elérheti.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)</span><span class="sxs-lookup"><span data-stu-id="ad56e-197">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="ad56e-198">Az egyes hónap termékindítási naptárának közzétételekor értesítést adjuk meg az Operations readiness erőforrás-katalógusban található bejelentéssel.</span><span class="sxs-lookup"><span data-stu-id="ad56e-198">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="ad56e-199">Az új és meglévő ajánlatokkal kapcsolatos információkat az árlista előnézetében és az árlista változásnaplóiban, valamint a termék blogjaiban, licencelési útmutatóiban és termék marketingoldalán találja.</span><span class="sxs-lookup"><span data-stu-id="ad56e-199">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="ad56e-200">A módosítás a következő termékek indítására vonatkozik:</span><span class="sxs-lookup"><span data-stu-id="ad56e-200">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="ad56e-201">Helyszíni Dynamics</span><span class="sxs-lookup"><span data-stu-id="ad56e-201">Dynamics on-premises</span></span>
- <span data-ttu-id="ad56e-202">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ad56e-202">Microsoft 365</span></span>
- <span data-ttu-id="ad56e-203">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="ad56e-203">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="ad56e-204">Windows</span><span class="sxs-lookup"><span data-stu-id="ad56e-204">Windows</span></span>
- <span data-ttu-id="ad56e-205">Kiszolgáló</span><span class="sxs-lookup"><span data-stu-id="ad56e-205">Server</span></span>  
- <span data-ttu-id="ad56e-206">Eszközök</span><span class="sxs-lookup"><span data-stu-id="ad56e-206">Tools</span></span>
- <span data-ttu-id="ad56e-207">Teams és Telco</span><span class="sxs-lookup"><span data-stu-id="ad56e-207">Teams and Telco</span></span>

<span data-ttu-id="ad56e-208">Továbbra is küldünk olyan termékindításokkal kapcsolatos konkrét közleményeket, amelyekhez műveleti készenlétre vonatkozó részletekre van szükség.</span><span class="sxs-lookup"><span data-stu-id="ad56e-208">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ad56e-209">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-209">Next steps</span></span>

<span data-ttu-id="ad56e-210">Tekintse át a témakörre vonatkozó forrásokat, és ossza meg ezt az információt a szervezet megfelelő érdekelt felével.</span><span class="sxs-lookup"><span data-stu-id="ad56e-210">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-211">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-211">Questions?</span></span>

<span data-ttu-id="ad56e-212">Az ajánlatokkal kapcsolatos további kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="ad56e-212">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="ad56e-213">A CSP-ügyfelekre vonatkozó, az ügyfelekre vonatkozó beiratalozási követelmények változásai</span><span class="sxs-lookup"><span data-stu-id="ad56e-213">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-214">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-214">Categories</span></span>

- <span data-ttu-id="ad56e-215">Dátum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="ad56e-215">Date: 2021-03-25</span></span>
- <span data-ttu-id="ad56e-216">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-216">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-217">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-217">Summary</span></span>

<span data-ttu-id="ad56e-218">Elkötelezettségünk részeként, hogy segítsünk a partnereknek és az ügyfeleknek a bizalmi kapcsolaton alapuló üzleti tevékenységben, további ügyféladatokat kérünk 2021. március 25-ig.</span><span class="sxs-lookup"><span data-stu-id="ad56e-218">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-219">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-219">Impacted audience</span></span>

<span data-ttu-id="ad56e-220">Felhőszolgáltató (CSP) közvetlen számlázási partnerek és közvetett szolgáltatók, akik új vagy meglévő ügyfelekkel vannak a következő szakaszban felsorolt országokban</span><span class="sxs-lookup"><span data-stu-id="ad56e-220">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-221">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-221">Details</span></span>

<span data-ttu-id="ad56e-222">A Microsoft megbízhatósági kapcsolaton fut.</span><span class="sxs-lookup"><span data-stu-id="ad56e-222">Microsoft runs on trust.</span></span> <span data-ttu-id="ad56e-223">Elkötelezettek vagyunk amellett, hogy megfelelő, biztonságos és biztonságos ügyfél-ellenőrzési módszert biztosítsunk az ügyfél-előfizetések tranzakciós folyamatához a CSP-programban.</span><span class="sxs-lookup"><span data-stu-id="ad56e-223">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="ad56e-224">2021. március 25-én bevezetünk egy API- és felhasználói felületi (UI) fejlesztéseket Partnerközpont, amelyek hatással lesznek az alábbi két feltételnek megfelelő partnerekre:</span><span class="sxs-lookup"><span data-stu-id="ad56e-224">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="ad56e-225">A partner közvetlen számlázási kapcsolattal rendelkezik a Microsofttal (ami azt jelenti, hogy a partner közvetlen számlázási partner vagy közvetett szolgáltató).</span><span class="sxs-lookup"><span data-stu-id="ad56e-225">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="ad56e-226">A partner az alábbi országokban lévő új vagy meglévő ügyfelekkel működik együtt:</span><span class="sxs-lookup"><span data-stu-id="ad56e-226">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="ad56e-227">Thaiföld</span><span class="sxs-lookup"><span data-stu-id="ad56e-227">Thailand</span></span>
    - <span data-ttu-id="ad56e-228">Vietnam</span><span class="sxs-lookup"><span data-stu-id="ad56e-228">Vietnam</span></span>
    - <span data-ttu-id="ad56e-229">Törökország</span><span class="sxs-lookup"><span data-stu-id="ad56e-229">Turkey</span></span>
    - <span data-ttu-id="ad56e-230">Lengyelország</span><span class="sxs-lookup"><span data-stu-id="ad56e-230">Poland</span></span>
    - <span data-ttu-id="ad56e-231">Dél-afrikai Köztársaság</span><span class="sxs-lookup"><span data-stu-id="ad56e-231">South Africa</span></span>
    - <span data-ttu-id="ad56e-232">India</span><span class="sxs-lookup"><span data-stu-id="ad56e-232">India</span></span>
    - <span data-ttu-id="ad56e-233">Brazília</span><span class="sxs-lookup"><span data-stu-id="ad56e-233">Brazil</span></span>
    - <span data-ttu-id="ad56e-234">Irak</span><span class="sxs-lookup"><span data-stu-id="ad56e-234">Iraq</span></span>
    - <span data-ttu-id="ad56e-235">Mianmar</span><span class="sxs-lookup"><span data-stu-id="ad56e-235">Myanmar</span></span>
    - <span data-ttu-id="ad56e-236">Dél-Szudán</span><span class="sxs-lookup"><span data-stu-id="ad56e-236">South Sudan</span></span>
    - <span data-ttu-id="ad56e-237">Szaúd-Arábia</span><span class="sxs-lookup"><span data-stu-id="ad56e-237">Saudi Arabia</span></span>
    - <span data-ttu-id="ad56e-238">Egyesült Arab Emírségek</span><span class="sxs-lookup"><span data-stu-id="ad56e-238">United Arab Emirates</span></span>
    - <span data-ttu-id="ad56e-239">Venezuela</span><span class="sxs-lookup"><span data-stu-id="ad56e-239">Venezuela</span></span>

<span data-ttu-id="ad56e-240">A feltételeknek megfelelő partnereknek be kell majd nyújtaniuk az ügyfél céges regisztrációs azonosítóját **(más** néven az ügyfél szervezeti **INN-ét)** és telefonszámát, amikor új ügyfeleket regisztrálnak vagy módosítják a meglévő ügyféladatokat. </span><span class="sxs-lookup"><span data-stu-id="ad56e-240">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="ad56e-241">Ezek a partnerek **középső nevet** is megadhatnak az ügyfél számára.</span><span class="sxs-lookup"><span data-stu-id="ad56e-241">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="ad56e-242">Vegye figyelembe, hogy a céges regisztrációs azonosító hozzáadásakor az üzleti adóazonosítót kell használnia, nem az ügyfél személyes azonosítóját.</span><span class="sxs-lookup"><span data-stu-id="ad56e-242">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="ad56e-243">Azok a partnerek, akik az alábbi országokban lévő új vagy meglévő ügyfelekkel üzleti partnereket hoznak létre, már elő vannak hozva egy korábbi kiadással 2020 novemberében.</span><span class="sxs-lookup"><span data-stu-id="ad56e-243">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="ad56e-244">Örményország</span><span class="sxs-lookup"><span data-stu-id="ad56e-244">Armenia</span></span>
- <span data-ttu-id="ad56e-245">Azerbajdzsán</span><span class="sxs-lookup"><span data-stu-id="ad56e-245">Azerbaijan</span></span>
- <span data-ttu-id="ad56e-246">Belarusz</span><span class="sxs-lookup"><span data-stu-id="ad56e-246">Belarus</span></span>
- <span data-ttu-id="ad56e-247">Magyarország</span><span class="sxs-lookup"><span data-stu-id="ad56e-247">Hungary</span></span>
- <span data-ttu-id="ad56e-248">Kazahsztán</span><span class="sxs-lookup"><span data-stu-id="ad56e-248">Kazakhstan</span></span>
- <span data-ttu-id="ad56e-249">Kirgizisztán</span><span class="sxs-lookup"><span data-stu-id="ad56e-249">Kyrgyzstan</span></span>
- <span data-ttu-id="ad56e-250">Moldova</span><span class="sxs-lookup"><span data-stu-id="ad56e-250">Moldova</span></span>
- <span data-ttu-id="ad56e-251">Oroszország</span><span class="sxs-lookup"><span data-stu-id="ad56e-251">Russia</span></span>
- <span data-ttu-id="ad56e-252">Tádzsikisztán</span><span class="sxs-lookup"><span data-stu-id="ad56e-252">Tajikistan</span></span>
- <span data-ttu-id="ad56e-253">Ukrajna</span><span class="sxs-lookup"><span data-stu-id="ad56e-253">Ukraine</span></span>
- <span data-ttu-id="ad56e-254">Üzbegisztán</span><span class="sxs-lookup"><span data-stu-id="ad56e-254">Uzbekistan</span></span>

<span data-ttu-id="ad56e-255">A világ többi részén az ügyfelekkel partneri együttműködésben 2021. március 25-én opcionálisan megadhatja az ügyfelek céges regisztrációs azonosítóját, telefonszámát és középső nevét.   </span><span class="sxs-lookup"><span data-stu-id="ad56e-255">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ad56e-256">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-256">Next steps</span></span>

- <span data-ttu-id="ad56e-257">Részletesebb útmutatásért tekintse át a műszaki dokumentációt és a dedikált [partnergyűjtemény](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) gyakori kérdéseit.</span><span class="sxs-lookup"><span data-stu-id="ad56e-257">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="ad56e-258">Készüljön fel arra, hogy a módosításokat a Partnerközpont API és a webes felhasználói felület használatával építse be.</span><span class="sxs-lookup"><span data-stu-id="ad56e-258">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="ad56e-259">Az API/SDK-k elérhetők lesznek a teszteléshez.</span><span class="sxs-lookup"><span data-stu-id="ad56e-259">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="ad56e-260">Az új ügyfelek be- és módosításakor küldje el a további adatokat.</span><span class="sxs-lookup"><span data-stu-id="ad56e-260">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="ad56e-261">Ha vezérlőpult-szállító (CPV) megoldást használ, tekintse meg a CPV-t.</span><span class="sxs-lookup"><span data-stu-id="ad56e-261">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-262">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-262">Questions?</span></span>

<span data-ttu-id="ad56e-263">Ha bármilyen kérdése van a jogi azonosítóval (más néven INN-rel vagy TIN-sel) kapcsolatban, forduljon az adótanácshoz vagy a helyi adóhivatalhoz.</span><span class="sxs-lookup"><span data-stu-id="ad56e-263">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="ad56e-264">A Microsoft nem tud útmutatást nyújtani az adózási kérdésekkel kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="ad56e-264">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="ad56e-265">Ha támogatásra van szüksége a Microsofttal kapcsolatos műveleteihez, [nyisson meg egy szolgáltatáskérést.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="ad56e-265">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="ad56e-266">A 2021. március 1-jén végleges szoftverárlistán tett javítások</span><span class="sxs-lookup"><span data-stu-id="ad56e-266">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-267">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-267">Categories</span></span>

- <span data-ttu-id="ad56e-268">Dátum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="ad56e-268">Date: 2021-03-23</span></span>
- <span data-ttu-id="ad56e-269">Ajánlatok/piacok</span><span class="sxs-lookup"><span data-stu-id="ad56e-269">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-270">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-270">Impacted audience</span></span>

<span data-ttu-id="ad56e-271">Közvetlen szolgáltatók és közvetlen számlázási partnerek, akik állandó szoftvereket tranzakcióznak a Felhőszolgáltató programjában</span><span class="sxs-lookup"><span data-stu-id="ad56e-271">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="ad56e-272">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-272">Details</span></span>

<span data-ttu-id="ad56e-273">A 2021. március 1-jén közzétett végleges szoftverek árlistja olyan piacokat is tartalmazott, amelyekre nem kellett volna.</span><span class="sxs-lookup"><span data-stu-id="ad56e-273">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="ad56e-274">A végleges szoftverárak listája 2021. március 17-én frissült a javításokkal.</span><span class="sxs-lookup"><span data-stu-id="ad56e-274">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="ad56e-275">Ezek a javítások csak a következőre voltak alkalmazhatók:</span><span class="sxs-lookup"><span data-stu-id="ad56e-275">These corrections were only applicable to:</span></span>

- <span data-ttu-id="ad56e-276">Termékazonosító: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="ad56e-276">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="ad56e-277">Terméknév: Windows 10 Home termék pro verziófrissítése a Microsoft 365 business termékhez</span><span class="sxs-lookup"><span data-stu-id="ad56e-277">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="ad56e-278">Eltávolított vagy nem támogatott piacok: AE, AF, AL, AM, AO, BA,ZŐ, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="ad56e-278">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="ad56e-279">Ezek a módosítások csak a fenti termékre vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="ad56e-279">These changes only apply to the above product.</span></span> <span data-ttu-id="ad56e-280">Más termékeknél nem voltak javítások.</span><span class="sxs-lookup"><span data-stu-id="ad56e-280">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="ad56e-281">Következő lépések és erőforrások</span><span class="sxs-lookup"><span data-stu-id="ad56e-281">Next steps and resources</span></span>

- <span data-ttu-id="ad56e-282">A folyamatos szoftvereket tranzakció partnereknek le kell töltenie a legújabb végleges szoftverárlistát.</span><span class="sxs-lookup"><span data-stu-id="ad56e-282">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="ad56e-283">A [kétbetűs](/azure/marketplace/commercial-marketplace-co-sell-countries) rövidítés országokra való rövidítésének felhasználóbarát leképezéséhez tekintse meg a régió országkódját.</span><span class="sxs-lookup"><span data-stu-id="ad56e-283">Consult the [region country codes](/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="ad56e-284">SDK-kiadás a .NET Standardon (1.17.0-s verzió)</span><span class="sxs-lookup"><span data-stu-id="ad56e-284">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-285">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-285">Categories</span></span>

- <span data-ttu-id="ad56e-286">Dátum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="ad56e-286">Date: 2021-03-23</span></span>

- <span data-ttu-id="ad56e-287">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-287">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="ad56e-288">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-288">Impacted audience</span></span>

<span data-ttu-id="ad56e-289">A CSP programban részt vevő közvetlen számlázási partnerek és közvetett szolgáltatók, akik az Partnerközpont .NET SDK-t használják.</span><span class="sxs-lookup"><span data-stu-id="ad56e-289">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-290">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-290">Details</span></span>

<span data-ttu-id="ad56e-291">2020. március 23-án a partnerek elkezdik letölteni a [MicrosoftPartnerCenter.NETSDK (NuGet Gallery Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), valamint frissített nyilvános Partnerközpont SDK [GitHub-minták.](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="ad56e-291">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="ad56e-292">Ez a verzió a következő módszerek frissítéseit tartalmazza:</span><span class="sxs-lookup"><span data-stu-id="ad56e-292">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="ad56e-293">Audit frissítve: Új művelettípusok</span><span class="sxs-lookup"><span data-stu-id="ad56e-293">Audit Updated: New operation types</span></span>

<span data-ttu-id="ad56e-294">Új [művelettípusok hozzáadva annak](/partner-center/develop/auditing-resources) tudatában, hogy az ügyfél mikor hagyta jóvá és szüntette meg a DAP-t.</span><span class="sxs-lookup"><span data-stu-id="ad56e-294">Added new [operation types](/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="ad56e-295">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="ad56e-295">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="ad56e-296">DapAdminRelationshipTerminated (DapAdminRelationshipTerminated)</span><span class="sxs-lookup"><span data-stu-id="ad56e-296">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="ad56e-297">Napló frissítve: Új erőforrás- és művelettípusok</span><span class="sxs-lookup"><span data-stu-id="ad56e-297">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="ad56e-298">Új [erőforrás- és művelettípusok hozzáadva](/partner-center/develop/auditing-resources) az ügyfél címtárszerepkör-forgatókönyvének támogatásához.</span><span class="sxs-lookup"><span data-stu-id="ad56e-298">Added new [resource and operation types](/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="ad56e-299">Új erőforrástípus: "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="ad56e-299">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="ad56e-300">Az "AddUserMember" és a "RemoveUserMember" művelettípusok</span><span class="sxs-lookup"><span data-stu-id="ad56e-300">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="ad56e-301">Az ügyfélfiókok SDK-frissítései</span><span class="sxs-lookup"><span data-stu-id="ad56e-301">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="ad56e-302">GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus támogatása</span><span class="sxs-lookup"><span data-stu-id="ad56e-302">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="ad56e-303">GET /customers/{customer-tenant-id}/qualifications</span><span class="sxs-lookup"><span data-stu-id="ad56e-303">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="ad56e-304">POST /customers/{customer_id}/qualifications?code={validationCode}</span><span class="sxs-lookup"><span data-stu-id="ad56e-304">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="ad56e-305">További módosítások</span><span class="sxs-lookup"><span data-stu-id="ad56e-305">Additional changes</span></span>

<span data-ttu-id="ad56e-306">A következő változások az Új kereskedelem részeként vannak bevezetve, és jelenleg csak az M365/D365 Új kereskedelmi felhasználói élmény technikai előzetes verzióban részt vesz partnerek számára érhetők el meghívással.</span><span class="sxs-lookup"><span data-stu-id="ad56e-306">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="ad56e-307">Azok a partnerek, akik nem részei az Új kereskedelmi technikai előzetes verziónak, nem láthatják a hatásokat, és visszamenőlegesen kompatibilisnek kell lenniük.</span><span class="sxs-lookup"><span data-stu-id="ad56e-307">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="ad56e-308">Katalógusváltozások:</span><span class="sxs-lookup"><span data-stu-id="ad56e-308">Catalog Changes:</span></span>

  - <span data-ttu-id="ad56e-309">GET /products/{termékazonosító}/skus/{sku-id}</span><span class="sxs-lookup"><span data-stu-id="ad56e-309">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="ad56e-310">Vásárlás és kezelés:</span><span class="sxs-lookup"><span data-stu-id="ad56e-310">Purchase and Manage:</span></span>
  - <span data-ttu-id="ad56e-311">GET /customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="ad56e-311">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="ad56e-312">GET /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="ad56e-312">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="ad56e-313">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="ad56e-313">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="ad56e-314">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="ad56e-314">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="ad56e-315">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="ad56e-315">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="ad56e-316">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="ad56e-316">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="ad56e-317">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-317">Next Steps</span></span>

- <span data-ttu-id="ad56e-318">Töltse le a [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="ad56e-318">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="ad56e-319">A [GitHub-minták letöltése és áttekintése](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="ad56e-319">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="ad56e-320">CSP kereskedelmi piactéri ajánlat és FY21 CSP-ösztönzők a jogosult ajánlatokhoz</span><span class="sxs-lookup"><span data-stu-id="ad56e-320">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-321">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-321">Categories</span></span>

- <span data-ttu-id="ad56e-322">Dátum: 2021. 03. 18.</span><span class="sxs-lookup"><span data-stu-id="ad56e-322">Date: 2021-03-18</span></span>
- <span data-ttu-id="ad56e-323">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-323">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-324">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-324">Impacted audience</span></span>

<span data-ttu-id="ad56e-325">Közvetett szolgáltatók és közvetlen számlázási partnerek a Felhőszolgáltató programjában</span><span class="sxs-lookup"><span data-stu-id="ad56e-325">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="ad56e-326">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-326">Details</span></span>

<span data-ttu-id="ad56e-327">A közvetett szolgáltatók és a Felhőszolgáltató-programban részt vevő közvetlen számlázási partnerek értékesíthet harmadik féltől származó ajánlatokat, és ösztönzőleg ösztönözheti a Partnerközpont vagy a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ad56e-327">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="ad56e-328">Az ösztönző a jogosult ajánlatok kiszámlázott értékesítésének formában lesz elérhető **2021.** június 30-ig.</span><span class="sxs-lookup"><span data-stu-id="ad56e-328">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="ad56e-329">Folytassa az alábbi, CSP kereskedelmi piactéri ajánlatra vonatkozó ösztönzővel kapcsolatos további tanulást, és vegye fel a kapcsolatot az ügyfelekkel még ma, hogy azonosítsa a sikeres és digitális átalakuláshoz szükséges megfelelő ajánlatokat.</span><span class="sxs-lookup"><span data-stu-id="ad56e-329">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="ad56e-330">A független szoftverszállítók (ISV-k) segítségével a legújabb IaaS- és SaaS-megoldásokat kínáljuk a Microsoft ügyfeleinek.</span><span class="sxs-lookup"><span data-stu-id="ad56e-330">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="ad56e-331">Az ISV-közzétevők számára lehetősége van engedélyezni az ajánlataik értékesítését a Microsoft partnercsatornáján keresztül.</span><span class="sxs-lookup"><span data-stu-id="ad56e-331">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="ad56e-332">Az ösztönzőre jogosult ajánlataink két kategóriába sorolhatók:</span><span class="sxs-lookup"><span data-stu-id="ad56e-332">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="ad56e-333">Válassza ki az Azure IP-alapú közös értékesítéscentrizált állapotú saaS- és IaaS-ajánlatokat.</span><span class="sxs-lookup"><span data-stu-id="ad56e-333">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="ad56e-334">A Teamsbe integrált SaaS-alkalmazások vagy legalább Microsoft 365 alkalmazások, például a PowerPoint, a Word, az Excel, az Outlook vagy a SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ad56e-334">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="ad56e-335">Következő lépések és erőforrások</span><span class="sxs-lookup"><span data-stu-id="ad56e-335">Next steps and resources</span></span>

- <span data-ttu-id="ad56e-336">Ismerje meg, hogyan lehet [partneri ösztönzőket keresni](https://partner.microsoft.com/membership/partner-incentives) jogosult Marketplace-alkalmazások értékesítéséhez az ösztönző jogosult alkalmazásokkal.</span><span class="sxs-lookup"><span data-stu-id="ad56e-336">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="ad56e-337">Az új ajánlatok hozzáadása havonta történik.</span><span class="sxs-lookup"><span data-stu-id="ad56e-337">New offers are added monthly.</span></span>  
- [<span data-ttu-id="ad56e-338">Felhőszolgáltató partneri ösztönzőerőforrások közvetlen számlázása</span><span class="sxs-lookup"><span data-stu-id="ad56e-338">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="ad56e-339">Felhőszolgáltató közvetett szolgáltatói ösztönző erőforrások</span><span class="sxs-lookup"><span data-stu-id="ad56e-339">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="ad56e-340">Tekintse át [ezt a bemutatót,](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) ha többet szeretne megtudni a kereskedelmi piactéren elérhető alkalmazások értékesítésről.</span><span class="sxs-lookup"><span data-stu-id="ad56e-340">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="ad56e-341">A további forrásokkal itt [is rendelkezik.](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)</span><span class="sxs-lookup"><span data-stu-id="ad56e-341">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="ad56e-342">Ismerkedés a kereskedelmi piactér-katalógussal [Partnerközpont](../csp-commercial-marketplace-discover.md) vagy [Azure Portal](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="ad56e-342">Explore the commercial marketplace catalog in [Partner Center](../csp-commercial-marketplace-discover.md) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="ad56e-343">Alkalmazások [integrálása](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) a vállalat piacterébe API-k használatával</span><span class="sxs-lookup"><span data-stu-id="ad56e-343">Use [APIs](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="ad56e-344">Érdeklődjön azokkal az ISV-ket, amelyek érdeklik az üzletben</span><span class="sxs-lookup"><span data-stu-id="ad56e-344">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="ad56e-345">A közvetett szolgáltatóknak API-k használatával kell integrálni az integrációt, és útmutatást kell adni az értékesíthető alkalmazások viszonteladói számára</span><span class="sxs-lookup"><span data-stu-id="ad56e-345">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-346">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-346">Questions?</span></span>  

<span data-ttu-id="ad56e-347">Ebben [a cikkben áttekintheti](../csp-commercial-marketplace-overview.md) a kereskedelmi piacteret a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ad56e-347">Refer to [this article](../csp-commercial-marketplace-overview.md) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="ad56e-348">Ha további segítségre van szüksége, hozzon létre egy támogatási kérést a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ad56e-348">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="ad56e-349">További információ: [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="ad56e-349">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="ad56e-350">Power BI Premium ajánlat elnevezése és előfeltétel-frissítése</span><span class="sxs-lookup"><span data-stu-id="ad56e-350">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-351">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-351">Categories</span></span>

- <span data-ttu-id="ad56e-352">Dátum: 2021.03. 18.</span><span class="sxs-lookup"><span data-stu-id="ad56e-352">Date: 2021-03-18</span></span>
- <span data-ttu-id="ad56e-353">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-353">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-354">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-354">Summary</span></span>

<span data-ttu-id="ad56e-355">A 2021. április 1- és 2021-es végleges árlista frissül, hogy egyértelműbb legyen a felhasználónkénti ajánlatokra vonatkozó Power BI Premium és/vagy előfeltétel-információk.</span><span class="sxs-lookup"><span data-stu-id="ad56e-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-356">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-356">Impacted audience</span></span>

<span data-ttu-id="ad56e-357">Felhőszolgáltató (CSP) közvetlen és közvetett partnerek</span><span class="sxs-lookup"><span data-stu-id="ad56e-357">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-358">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-358">Details</span></span>

<span data-ttu-id="ad56e-359">A 2021. április 1-i végleges árlista frissülni fog, hogy érthetőbb legyen az egyes Power BI Premium ajánlatokkal kapcsolatos elnevezési és/vagy előfeltétel-információk.</span><span class="sxs-lookup"><span data-stu-id="ad56e-359">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="ad56e-360">A végleges árlista frissítésig az ebben a szakaszban található információk alapján győződjön meg arról, hogy a megfelelő terméket rendelte meg.</span><span class="sxs-lookup"><span data-stu-id="ad56e-360">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="ad56e-361">Az alábbi részletek az érintett termékváltozatot és előfeltétel-részleteket mutatják be.</span><span class="sxs-lookup"><span data-stu-id="ad56e-361">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="ad56e-362">Ajánlat megjelenítendő neve a március 1-i árlista előzetes kiadásában</span><span class="sxs-lookup"><span data-stu-id="ad56e-362">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="ad56e-363">Frissített ajánlat megjelenítendő neve a április 1-i végleges árlistán</span><span class="sxs-lookup"><span data-stu-id="ad56e-363">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="ad56e-364">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="ad56e-364">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="ad56e-365">Power BI Premium felhasználónkénti Add-On (nonprofit személyzet díjszabása)</span><span class="sxs-lookup"><span data-stu-id="ad56e-365">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="ad56e-366">Power BI Premium felhasználónkénti Add-On **(Office) (Nonprofit** személyzet díjszabása)</span><span class="sxs-lookup"><span data-stu-id="ad56e-366">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="ad56e-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="ad56e-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="ad56e-368">Az ügyfeleknek az alábbi előfeltételek bármelyikével kell megfeleleni az ajánlat megvásárlásához:</span><span class="sxs-lookup"><span data-stu-id="ad56e-368">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="ad56e-369">Ajánlat megjelenítendő neve</span><span class="sxs-lookup"><span data-stu-id="ad56e-369">Offer display name</span></span> | <span data-ttu-id="ad56e-370">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="ad56e-370">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="ad56e-371">Microsoft 365 E5 (Nonprofit személyzet díjszabása)</span><span class="sxs-lookup"><span data-stu-id="ad56e-371">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="ad56e-372">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="ad56e-372">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="ad56e-373">Microsoft 365 E5 beállítása hangkonferencia nélkül (nonprofit személyzet díjszabása)</span><span class="sxs-lookup"><span data-stu-id="ad56e-373">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="ad56e-374">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="ad56e-374">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="ad56e-375">Office 365 E5 (Nonprofit személyzet díjszabása)</span><span class="sxs-lookup"><span data-stu-id="ad56e-375">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="ad56e-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="ad56e-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="ad56e-377">Office 365 E5 (Nonprofit személyzet díjszabása) próbaverzió</span><span class="sxs-lookup"><span data-stu-id="ad56e-377">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="ad56e-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="ad56e-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="ad56e-379">Hangkonferencia nélküli Office 365 E5 (nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="ad56e-379">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="ad56e-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="ad56e-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="ad56e-381">A következő Power BI Premium ajánlathoz előfeltétel szükséges a vásárláshoz:</span><span class="sxs-lookup"><span data-stu-id="ad56e-381">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="ad56e-382">Ajánlat megjelenítendő neve</span><span class="sxs-lookup"><span data-stu-id="ad56e-382">Offer display name</span></span> | <span data-ttu-id="ad56e-383">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="ad56e-383">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="ad56e-384">Power BI Premium felhasználónkénti Add-On (nonprofit személyzet díjszabása)</span><span class="sxs-lookup"><span data-stu-id="ad56e-384">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="ad56e-385">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="ad56e-385">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="ad56e-386">Az ügyfeleknek a következő előfeltételre van szüksége az ajánlat megvásárlásához:</span><span class="sxs-lookup"><span data-stu-id="ad56e-386">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="ad56e-387">Ajánlat megjelenítendő neve</span><span class="sxs-lookup"><span data-stu-id="ad56e-387">Offer display name</span></span> | <span data-ttu-id="ad56e-388">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="ad56e-388">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="ad56e-389">Power BI Pro (nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="ad56e-389">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="ad56e-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="ad56e-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="ad56e-391">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-391">Next steps</span></span>

<span data-ttu-id="ad56e-392">Tekintse át a témakörre vonatkozó forrásokat, és ossza meg ezt az információt a szervezet megfelelő érdekelt felével.</span><span class="sxs-lookup"><span data-stu-id="ad56e-392">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="ad56e-393">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-393">Questions?</span></span>

<span data-ttu-id="ad56e-394">Az ajánlatokkal kapcsolatos kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="ad56e-394">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="ad56e-395">Az F3 Microsoft 365 márciusi árának frissítései</span><span class="sxs-lookup"><span data-stu-id="ad56e-395">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-396">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-396">Categories</span></span>

- <span data-ttu-id="ad56e-397">Dátum: 2021.03. 16.</span><span class="sxs-lookup"><span data-stu-id="ad56e-397">Date: 2021-03-16</span></span>
- <span data-ttu-id="ad56e-398">Ajánlatok/piacok</span><span class="sxs-lookup"><span data-stu-id="ad56e-398">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-399">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-399">Summary</span></span>

<span data-ttu-id="ad56e-400">A 2021. márciusi díjszabás helytelenül lett kijavítva Microsoft 365 F3 font (GBP) és az európa (EUR) esetében.</span><span class="sxs-lookup"><span data-stu-id="ad56e-400">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-401">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-401">Impacted audience</span></span>

<span data-ttu-id="ad56e-402">Az F3 Microsoft 365 GB/s vagy EUR értékben vásárolt partnerek 2021. március 1. és 2021. március 17. között a Felhőszolgáltató (CSP) program keretében.</span><span class="sxs-lookup"><span data-stu-id="ad56e-402">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-403">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-403">Details</span></span>

<span data-ttu-id="ad56e-404">A Microsoft megoldotta az F3 Microsoft 365 díjszabását.</span><span class="sxs-lookup"><span data-stu-id="ad56e-404">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="ad56e-405">A helytelen árak a GBP és az EUR esetében voltak, és csak a 2021. március 1. és 2021. március 17. között vásárolt ajánlatok esetében.</span><span class="sxs-lookup"><span data-stu-id="ad56e-405">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="ad56e-406">Az érintett ajánlatok és pénznemek listája alább látható.</span><span class="sxs-lookup"><span data-stu-id="ad56e-406">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="ad56e-407">Ajánlat neve</span><span class="sxs-lookup"><span data-stu-id="ad56e-407">Offer name</span></span> | <span data-ttu-id="ad56e-408">Pénznem</span><span class="sxs-lookup"><span data-stu-id="ad56e-408">Currency</span></span> | <span data-ttu-id="ad56e-409">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="ad56e-409">Offer ID</span></span> | <span data-ttu-id="ad56e-410">Anyagazonosító</span><span class="sxs-lookup"><span data-stu-id="ad56e-410">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="ad56e-411">Microsoft 365 F3 (Majd)</span><span class="sxs-lookup"><span data-stu-id="ad56e-411">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="ad56e-412">GBP</span><span class="sxs-lookup"><span data-stu-id="ad56e-412">GBP</span></span> | <span data-ttu-id="ad56e-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="ad56e-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="ad56e-414">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="ad56e-414">AAD-11626</span></span> |
| <span data-ttu-id="ad56e-415">Microsoft 365 F3 (Kereskedelmi)</span><span class="sxs-lookup"><span data-stu-id="ad56e-415">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="ad56e-416">EUR</span><span class="sxs-lookup"><span data-stu-id="ad56e-416">EUR</span></span>| <span data-ttu-id="ad56e-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="ad56e-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="ad56e-418">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="ad56e-418">AAA-89898</span></span> |
 
<span data-ttu-id="ad56e-419">A márciusi és áprilisi licenc-alapárak listája március 16-án, 17:00-kor frissült a csendes-óceáni téli idő szerint.</span><span class="sxs-lookup"><span data-stu-id="ad56e-419">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ad56e-420">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-420">Next steps</span></span>

- <span data-ttu-id="ad56e-421">A partnereknek újra le kell töltenie az aktuális licencalapú árlistát márciusban és áprilisban is, ezekkel az árkorrekcióval, ha van ilyen.</span><span class="sxs-lookup"><span data-stu-id="ad56e-421">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="ad56e-422">A Microsoft az elkövetkező hetekben e-mailben kapcsolatba lép az érintett partnerekkel, hogy tájékoztassa őket az érintett tranzakciók kijavítása során szükséges további lépésekről.</span><span class="sxs-lookup"><span data-stu-id="ad56e-422">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-423">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-423">Questions?</span></span>

<span data-ttu-id="ad56e-424">További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="ad56e-424">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="ad56e-425">Jogi vállalat nevének frissítése a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ad56e-425">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-426">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-426">Categories</span></span>

- <span data-ttu-id="ad56e-427">Dátum: 2021. 03. 16.</span><span class="sxs-lookup"><span data-stu-id="ad56e-427">Date: 2021-03-16</span></span>
- <span data-ttu-id="ad56e-428">Drive Efficiency & Scale</span><span class="sxs-lookup"><span data-stu-id="ad56e-428">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-429">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-429">Summary</span></span>

<span data-ttu-id="ad56e-430">2021 márciusában Microsoft Partner Network (MPN) partnerek és Felhőszolgáltató (CSP) közvetett viszonteladók frissítheti jogi vállalatuk nevét a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ad56e-430">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-431">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-431">Impacted audience</span></span>

<span data-ttu-id="ad56e-432">MPN-partnerek és közvetett CSP-viszonteladók (nem vonatkoznak a közvetlen számlázási CSP-partnerekre)</span><span class="sxs-lookup"><span data-stu-id="ad56e-432">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-433">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-433">Details</span></span>

<span data-ttu-id="ad56e-434">2021 márciusánaktól az MPN-partnerek és a közvetett CSP-viszonteladók frissítheti jogi vállalatuk nevét a Partnerközpont megfelelő, önkiszolgáló módon.</span><span class="sxs-lookup"><span data-stu-id="ad56e-434">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="ad56e-435">Ezzel az új funkcióval a partnereknek többé nem kell támogatási jegyet Partnerközpont a vállalatuk nevének frissítéséhez.</span><span class="sxs-lookup"><span data-stu-id="ad56e-435">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="ad56e-436">Ez jelentős időt takarít meg a partnerek számára ezen tevékenységek végrehajtása során.</span><span class="sxs-lookup"><span data-stu-id="ad56e-436">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="ad56e-437">További információ: [A jogi üzleti profil frissítése.](../update-your-partner-profile.md#update-your-legal-business-profile)</span><span class="sxs-lookup"><span data-stu-id="ad56e-437">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="ad56e-438">Győződjön meg arról, hogy a jogi üzleti profiljában a vállalat neve nem tartalmaz helyesírási hibákat és rövidítéseket, és pontosan megegyezik a hivatalos vállalati üzleti regisztrációs rekordokkal.</span><span class="sxs-lookup"><span data-stu-id="ad56e-438">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="ad56e-439">A szervezeti profil frissítésével kapcsolatos további információkért lásd: [A szervezeti profil ellenőrzése.](../update-your-partner-profile.md#update-your-legal-business-profile)</span><span class="sxs-lookup"><span data-stu-id="ad56e-439">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="ad56e-440">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-440">Next steps</span></span>

<span data-ttu-id="ad56e-441">Ossza meg ezt az információt a szervezeten belül, hogy a megfelelő csapat áttekintheti és frissítheti a folyamatait.</span><span class="sxs-lookup"><span data-stu-id="ad56e-441">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-442">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-442">Questions?</span></span>

<span data-ttu-id="ad56e-443">További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="ad56e-443">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="ad56e-444">Frissítés a Felhőszolgáltató (CSP) program fejlődése és az Open License program változásai</span><span class="sxs-lookup"><span data-stu-id="ad56e-444">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-445">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-445">Categories</span></span>

- <span data-ttu-id="ad56e-446">Dátum: 2021. 03. 15.</span><span class="sxs-lookup"><span data-stu-id="ad56e-446">Date: 2021-03-15</span></span>
- <span data-ttu-id="ad56e-447">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-447">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-448">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-448">Summary</span></span>

<span data-ttu-id="ad56e-449">Az új kereskedelmi és közszférában elérhető folyamatos szoftveres ajánlatok a Felhőszolgáltató (CSP) programba, az Open Licensing Program változásaival együtt stb.</span><span class="sxs-lookup"><span data-stu-id="ad56e-449">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-450">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-450">Impacted audience</span></span>

<span data-ttu-id="ad56e-451">A kereskedelmi terjesztők és a felügyelt viszonteladók, akik az Open License programon keresztül értékesítik őket, valamint minden CSP-partner, amely állandó szoftvereket értékesít</span><span class="sxs-lookup"><span data-stu-id="ad56e-451">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-452">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-452">Details</span></span>

<span data-ttu-id="ad56e-453">2020 szeptemberében [a](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) Microsoft bejelentette a digitális átalakulási folyamat lépéseit, hogy bővítse a CSP-program partnereinek lehetőségeit, beleértve a helyszíni szoftverek elérhetőségét a partnerek számára.</span><span class="sxs-lookup"><span data-stu-id="ad56e-453">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="ad56e-454">Ezek a változások lehetővé teszik a partnerek számára, hogy a felhőszolgáltató szoftverlicenceinek segítségével bővíthétsék a munkájukat, és sikerre jutnak napjaink felhőalapú világában.</span><span class="sxs-lookup"><span data-stu-id="ad56e-454">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="ad56e-455">Emellett lehetővé teszi az ügyfelek felhőre való áttérését is, és a partnerek számára a hibrid felhőalapú ügyfélkörnyezetekhez szükséges rugalmasságot biztosítják.</span><span class="sxs-lookup"><span data-stu-id="ad56e-455">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="ad56e-456">A digitális átalakítás folytatásaként bejelentjük a következő változásokat:</span><span class="sxs-lookup"><span data-stu-id="ad56e-456">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="ad56e-457">2021. július 1.: Az Open License program árlistába nem kerülnek új termékkódok, termékek vagy promóciók.</span><span class="sxs-lookup"><span data-stu-id="ad56e-457">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="ad56e-458">2021. július 7.: Két kereskedelmi ajánlat, a Get Genuine Windows és az Visual Studio Professional, valamint a közszférában elérhető ajánlatok (kormányzati, oktatási és nonprofit – lásd a [bejelentést)](./2020-december.md#9)bekerülnek a CSP folyamatos szoftverár-listájára.</span><span class="sxs-lookup"><span data-stu-id="ad56e-458">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="ad56e-459">Az árlista a Partnerközpont Értékesítés > Díjszabási ajánlatok [& oldalának](https://partnercenter.microsoft.com/pcv/sales) Szoftver szakaszában található, és ezen a napon lesz újból közzétenve.</span><span class="sxs-lookup"><span data-stu-id="ad56e-459">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="ad56e-460">A CSP-program fejlődésével és az Open License program változásaival kapcsolatos részletekért tekintse meg az alábbi **Következő lépéseket.**</span><span class="sxs-lookup"><span data-stu-id="ad56e-460">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ad56e-461">További lépések:</span><span class="sxs-lookup"><span data-stu-id="ad56e-461">Next Steps:</span></span>

- <span data-ttu-id="ad56e-462">CSP-program fejlődése: Tekintse át a folyamatos szoftvert a Felhőszolgáltató [készültségi](https://partner.microsoft.com/resources/collection/software-in-csp#/) anyagokban.</span><span class="sxs-lookup"><span data-stu-id="ad56e-462">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="ad56e-463">Ezzel a [készenlét-leképezéspel](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) gyorsan megkeresheti a szerepkörének megfelelő információkat.</span><span class="sxs-lookup"><span data-stu-id="ad56e-463">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="ad56e-464">Open License program módosításai: Tekintse át a [CSP-program](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) fejlődését és az Open License program módosításainak készültségi anyagát.</span><span class="sxs-lookup"><span data-stu-id="ad56e-464">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="ad56e-465">Ezzel a [készenlét-leképezéspel](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) gyorsan megkeresheti a szerepkörének megfelelő információkat.</span><span class="sxs-lookup"><span data-stu-id="ad56e-465">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-466">Kérdések</span><span class="sxs-lookup"><span data-stu-id="ad56e-466">Questions</span></span>

<span data-ttu-id="ad56e-467">További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="ad56e-467">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="ad56e-468">Frissítés egy korábbi bejelentésre: Premium Assessments, a Compliance Manager bővítménye</span><span class="sxs-lookup"><span data-stu-id="ad56e-468">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-469">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-469">Categories</span></span>

- <span data-ttu-id="ad56e-470">Dátum: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="ad56e-470">Date: 2021-03-15</span></span>
- <span data-ttu-id="ad56e-471">Vállalkozás fejlesztése</span><span class="sxs-lookup"><span data-stu-id="ad56e-471">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-472">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-472">Summary</span></span>

<span data-ttu-id="ad56e-473">A próbaverziós ajánlatoknak nem kellett volna szerepelve az árlistában, és el lesznek távolítva.</span><span class="sxs-lookup"><span data-stu-id="ad56e-473">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-474">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-474">Impacted audience</span></span>

<span data-ttu-id="ad56e-475">A partnerek tranzakciós Felhőszolgáltató</span><span class="sxs-lookup"><span data-stu-id="ad56e-475">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-476">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-476">Details</span></span>

<span data-ttu-id="ad56e-477">A próbaverziós ajánlatoknak nem kellett volna szerepelniük az árlistában.</span><span class="sxs-lookup"><span data-stu-id="ad56e-477">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="ad56e-478">Ezek el lesznek távolítva a 2021. május 1-i árlistáról.</span><span class="sxs-lookup"><span data-stu-id="ad56e-478">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="ad56e-479">Az eredeti bejelentés itt [van.](./2021-february.md#4)</span><span class="sxs-lookup"><span data-stu-id="ad56e-479">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="ad56e-480">További források</span><span class="sxs-lookup"><span data-stu-id="ad56e-480">Additional resources</span></span>

- [<span data-ttu-id="ad56e-481">Microsoft 365 E5 biztonság és megfelelőség</span><span class="sxs-lookup"><span data-stu-id="ad56e-481">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="ad56e-482">Értékelések összeállítása és kezelése a Microsoft Compliance Managerben – Microsoft 365 megfelelőség</span><span class="sxs-lookup"><span data-stu-id="ad56e-482">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="ad56e-483">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-483">Next steps</span></span>

<span data-ttu-id="ad56e-484">Tekintse át a témakörre vonatkozó forrásokat, és ossza meg ezt az információt a szervezet megfelelő érdekelt felével.</span><span class="sxs-lookup"><span data-stu-id="ad56e-484">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-485">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-485">Questions?</span></span>

<span data-ttu-id="ad56e-486">Az ajánlatokkal kapcsolatos kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="ad56e-486">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="ad56e-487">Megoldások miminálása egy kereskedelmi partnertől (OCP) piaci útjára (GTM) a Microsoft kereskedelmi piacterére</span><span class="sxs-lookup"><span data-stu-id="ad56e-487">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-488">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-488">Categories</span></span>

- <span data-ttu-id="ad56e-489">Dátum: 2021. 03. 12.</span><span class="sxs-lookup"><span data-stu-id="ad56e-489">Date: 2021-03-12</span></span>
- <span data-ttu-id="ad56e-490">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-490">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-491">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-491">Summary</span></span>

<span data-ttu-id="ad56e-492">2021. március 29-től korlátozott, piacra piacra ható (GTM) One Commercial Partner (OCP) képességeket fog tapasztalni.</span><span class="sxs-lookup"><span data-stu-id="ad56e-492">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="ad56e-493">Javasoljuk, hogy megoldásait a kereskedelmi piactérre mi célra Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ad56e-493">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-494">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-494">Impacted audience</span></span>

<span data-ttu-id="ad56e-495">Megoldások közös értékesítése az OCP GTM-megoldásokkal</span><span class="sxs-lookup"><span data-stu-id="ad56e-495">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-496">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-496">Details</span></span>

<span data-ttu-id="ad56e-497">2020 decemberével kezdtük meg a Microsoft OCP GTM eszközével és a Microsoft kereskedelmi piacterével való Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ad56e-497">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="ad56e-498">Ez az átállás kibővíti a kereskedelmi piactér képességeit, ahol megoldásait ügyfelek milliói számára mutathatja be, kétirányúan oszthatja meg a lehetőségeket más Microsoft- és partner értékesítőkkel, és közösen innovatív megoldásokat értékesíthet.</span><span class="sxs-lookup"><span data-stu-id="ad56e-498">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="ad56e-499">Az átváltás következő mérföldköve 2021. március 29-én lesz.</span><span class="sxs-lookup"><span data-stu-id="ad56e-499">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="ad56e-500">Ez az, amikor korlátozott OCP GTM-képességeket fog tapasztalni, és egyes mezők írásra válnak.</span><span class="sxs-lookup"><span data-stu-id="ad56e-500">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="ad56e-501">Ha jelenleg együtt értékesít az OCP GTM megoldásaival, javasoljuk, hogy megoldásait a kereskedelmi piactérre miminálja, hogy kihasználja annak képességeit, és egyszerűsítse a közzétételi élményt.</span><span class="sxs-lookup"><span data-stu-id="ad56e-501">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="ad56e-502">A kereskedelmi piactérre való Partnerközpont az értékesítések közzétételi folyamatának elsődleges célhelyét.</span><span class="sxs-lookup"><span data-stu-id="ad56e-502">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="ad56e-503">A microsoftos termékekhez használt csatornákon és termékeken keresztül a megoldásokat a megosztott ügyfelekkel összekapcsolva tovább tudja növekedni vállalkozását.</span><span class="sxs-lookup"><span data-stu-id="ad56e-503">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="ad56e-504">[További információ a kereskedelmi piactérről.](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)</span><span class="sxs-lookup"><span data-stu-id="ad56e-504">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="ad56e-505">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-505">Next steps</span></span>

- <span data-ttu-id="ad56e-506">Ha még nem költözte át a megoldásait, kövesse az [](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) átváltási útmutató utasításait, vagy tekintse meg a részletes videó oktatóanyagot az összes migrálási tevékenység befejezéséhez és a megoldás(ok) kereskedelmi piactéren való közzétételének elkezdéséért. [](/azure/marketplace/co-sell-solution-migration)</span><span class="sxs-lookup"><span data-stu-id="ad56e-506">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="ad56e-507">Az OCP GTM korlátozott képességeivel kapcsolatos kérdésekért tekintse meg a Microsoft kereskedelmi piactéren való közzétételre vonatkozó, közös értékesítésre [vonatkozó követelményeket](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span><span class="sxs-lookup"><span data-stu-id="ad56e-507">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="ad56e-508">(Lásd az "OCP GTM korlátozott képességei 2021. március 29-től kezdődően" című szakaszt.)</span><span class="sxs-lookup"><span data-stu-id="ad56e-508">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-509">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-509">Questions?</span></span>

<span data-ttu-id="ad56e-510">Ha [kérdése](https://partner.microsoft.com/support/?stage=1) van, vagy további információra van szüksége, forduljon az ügyfélszolgálathoz.</span><span class="sxs-lookup"><span data-stu-id="ad56e-510">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="ad56e-511">Az új kereskedelmi élmény bővítése az Azure-Felhőszolgáltató (CSP) programjában Az Azure és Oroszország között</span><span class="sxs-lookup"><span data-stu-id="ad56e-511">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-512">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-512">Categories</span></span>

- <span data-ttu-id="ad56e-513">Dátum: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="ad56e-513">Date: 2021-03-10</span></span>
- <span data-ttu-id="ad56e-514">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-514">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-515">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-515">Impacted audience</span></span>

<span data-ttu-id="ad56e-516">Az összes olyan partner, aki a Felhőszolgáltató (CSP) programon keresztül megy keresztül.</span><span class="sxs-lookup"><span data-stu-id="ad56e-516">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-517">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-517">Details</span></span>

<span data-ttu-id="ad56e-518">2021. március 10-től kezdve nagy izgatottan jelentjük be, hogy a CSP új kereskedelmi élménye elérhető az **Azure-ban Oroszországban.**</span><span class="sxs-lookup"><span data-stu-id="ad56e-518">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="ad56e-519">Ez a felhasználói élmény leegyszerűsíti és javítja az ügyfelek Azure-szolgáltatások vásárlásának és használatának módját.</span><span class="sxs-lookup"><span data-stu-id="ad56e-519">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="ad56e-520">Emellett konzisztens nézetet biztosít a CSP-programban szereplő partnereknek az Azure-díjszabásról az értékesítési mozgások stb., a globális konzisztencia amerikai dollárban elérhető díjszabása, a számlázási dátum igazítása és a hozzáférés Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="ad56e-520">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ad56e-521">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-521">Next steps</span></span>

<span data-ttu-id="ad56e-522">Számos forrás áll rendelkezésre, amelyek bemutatják az Azure új kereskedelmi élményét, és további információkat érhetők el.</span><span class="sxs-lookup"><span data-stu-id="ad56e-522">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="ad56e-523">Keresse meg a legújabb gyakori kérdések, bemutatók, videók és egyéb részleteket a [CSP programfrissítési erőforrás-katalógusában.](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)</span><span class="sxs-lookup"><span data-stu-id="ad56e-523">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="ad56e-524">Partnerközpont szoftverlicenc-kulcs használata és a fulfillment letöltése</span><span class="sxs-lookup"><span data-stu-id="ad56e-524">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-525">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-525">Categories</span></span>

- <span data-ttu-id="ad56e-526">Dátum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="ad56e-526">Date: 2021-03-04</span></span>
- <span data-ttu-id="ad56e-527">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-527">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-528">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-528">Summary</span></span>

<span data-ttu-id="ad56e-529">A Partnerközpont szoftverletöltési és -licenckulcs-teljesítési képesség vissza lett helyezték.</span><span class="sxs-lookup"><span data-stu-id="ad56e-529">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-530">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-530">Impacted audience</span></span>

<span data-ttu-id="ad56e-531">Minden Felhőszolgáltató (CSP) partner, amely folyamatos és kiszolgáló-előfizetési szoftverrendeléseket teljesít a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ad56e-531">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-532">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-532">Details</span></span>

<span data-ttu-id="ad56e-533">A partneri visszajelzésekre válaszul visszaállítjuk a Partnerközpont-teljesítési képességet, hogy szoftvereket és licenckulcsokat szerezzünk be a folyamatos és kiszolgálói előfizetési szoftverrendelések esetén.</span><span class="sxs-lookup"><span data-stu-id="ad56e-533">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="ad56e-534">A rendszer a 2021. január 19-i eltávolítás előtt visszaállítja az előző állapotába.</span><span class="sxs-lookup"><span data-stu-id="ad56e-534">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="ad56e-535">(Lásd [a bejelentést.)](2020-september.md#17)</span><span class="sxs-lookup"><span data-stu-id="ad56e-535">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="ad56e-536">Vegye figyelembe, hogy a szoftverlicenc-kulcsok és a letöltési hivatkozások értékesek és nagy rákeresettségnek vannak kivetve a szellemi tulajdont hasznos eszközökként.</span><span class="sxs-lookup"><span data-stu-id="ad56e-536">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="ad56e-537">Kiszivárogtatás esetén gyorsan kimerülhet az aktiválási korlátaik, ami negatív ügyfél- és partnerélményt okozhat.</span><span class="sxs-lookup"><span data-stu-id="ad56e-537">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ad56e-538">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-538">Next steps</span></span>

<span data-ttu-id="ad56e-539">Tekintse át a következő forrásokat a használati utasításokért és a szoftverkulcsok terjesztésével kapcsolatos fontos útmutatásért:</span><span class="sxs-lookup"><span data-stu-id="ad56e-539">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="ad56e-540">Helyszíni szoftverek eladása a CSP-programon keresztül</span><span class="sxs-lookup"><span data-stu-id="ad56e-540">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="ad56e-541">[Partnerközpont a New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (Útmutató a **szoftverkulcsok terjesztéséhez)** című szakaszban.)</span><span class="sxs-lookup"><span data-stu-id="ad56e-541">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-542">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-542">Questions?</span></span>

<span data-ttu-id="ad56e-543">Ha további kérdései vannak ezzel a közleményrel kapcsolatban, tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="ad56e-543">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="ad56e-544">Az ügyletek mi áttelepítése a Partner Sales Connectből (PSC) a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ad56e-544">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-545">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-545">Categories</span></span>

- <span data-ttu-id="ad56e-546">Dátum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="ad56e-546">Date: 2021-03-04</span></span>
- <span data-ttu-id="ad56e-547">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-547">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-548">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-548">Summary</span></span>

<span data-ttu-id="ad56e-549">A Partner Sales Connect (PSC) 2021. március 31-től csak olvasási hozzáférésre lesz áttűnve, ezért arra kérjük, hogy kezdje meg az ügyletek PSC-ről Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ad56e-549">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-550">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-550">Impacted audience</span></span>

<span data-ttu-id="ad56e-551">PSC-ügyleteket kötött partnerek</span><span class="sxs-lookup"><span data-stu-id="ad56e-551">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-552">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-552">Details</span></span>

<span data-ttu-id="ad56e-553">A növekedés iránti közös elkötelezettségünk részeként a **Microsofttal** való közös értékesítéssel felfedezheti, biztosíthatja szakértelmét, és megnövelheti az ügyféligényét a pozitív ügyfél-eredmények érdekében. </span><span class="sxs-lookup"><span data-stu-id="ad56e-553">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="ad56e-554">Az átlagos üzlet a szokásosnál **3,5-szer** gyorsabb, így az Partnerközpont-ban történő közös értékesítési élmény kezelése lehetővé teszi, hogy a közvetlen ügyfél-, partner- és Microsoft-értékesítői csatornákon keresztül értékesítsen, és a teljes ajánlási folyamatot egyetlen helyen kezelje.</span><span class="sxs-lookup"><span data-stu-id="ad56e-554">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="ad56e-555">A **PSC** **2021. március 31-től** csak olvasási hozzáférésre fog áttűnni, ezért arra kérjük, hogy kezdje el a Partnerközpont-ra való áthelyezést, és hozzáférjen a következő képességbeli fejlesztésekhez: </span><span class="sxs-lookup"><span data-stu-id="ad56e-555">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="ad56e-556">**Pontosabb útválasztást** nyújt a Microsofttal a megfelelő értékesítőnek a szükséges segítség típusa alapján.</span><span class="sxs-lookup"><span data-stu-id="ad56e-556">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="ad56e-557">**Előzetes ajánlat jogosultságának** ellenőrzése az ösztönzőre jogosult megoldásokhoz és az ISV Connect program feltételeinek való megfeleléshez, leegyszerűsítve a jóváhagyási folyamatot és a végső végrehajtási igazolást (POE).</span><span class="sxs-lookup"><span data-stu-id="ad56e-557">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="ad56e-558">**Zökkenőmentes felhasználói élmény** az összes közös értékesítési lehetőség és az értékesítésre jogosult érdeklődők egyetlen helyen való kezeléséhez.</span><span class="sxs-lookup"><span data-stu-id="ad56e-558">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="ad56e-559">Nemrég új funkciókat is hozzáadtunk a Partnerközpont az áthelyezéshez:</span><span class="sxs-lookup"><span data-stu-id="ad56e-559">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="ad56e-560">Tömeges műveletek az együttműködési lehetőségekhez</span><span class="sxs-lookup"><span data-stu-id="ad56e-560">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="ad56e-561">[Az ügylet migrálási funkciója](../psc-to-pc.md) (lásd **a PSC-ügyletek migrálási** szakaszát.)</span><span class="sxs-lookup"><span data-stu-id="ad56e-561">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="ad56e-562">A Partnerközpont értékesítési élményének használatával az értékesítési csapatoknak több ideje lesz arra, hogy az érdeklődők és lehetőségek árnyalásaira, az üzletek lezárására és a tartós ügyfélkapcsolatok létrehozására összpontosítsanak.</span><span class="sxs-lookup"><span data-stu-id="ad56e-562">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ad56e-563">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-563">Next steps</span></span>

<span data-ttu-id="ad56e-564">A Partnerközpont [útmutató](../psc-to-pc.md) segítségével végigvezetheti az ügylet PSC-ről Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ad56e-564">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-565">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-565">Questions?</span></span>

<span data-ttu-id="ad56e-566">Ha további kérdései vannak, forduljon a [támogatási szolgálathoz.](https://partner.microsoft.com/support/?stage=1)</span><span class="sxs-lookup"><span data-stu-id="ad56e-566">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="ad56e-567">Új Microsoft Dynamics 365-termékek és -ajánlatok, amelyek 2021. április 1-én érhetők el</span><span class="sxs-lookup"><span data-stu-id="ad56e-567">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-568">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-568">Categories</span></span>

- <span data-ttu-id="ad56e-569">Dátum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="ad56e-569">Date: 2021-03-04</span></span>
- <span data-ttu-id="ad56e-570">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-570">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-571">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-571">Summary</span></span>

<span data-ttu-id="ad56e-572">2021. április 1-ével a Microsoft számos új terméket és ajánlatot bocsát ki a Felhőszolgáltató (CSP) programhoz.</span><span class="sxs-lookup"><span data-stu-id="ad56e-572">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-573">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-573">Impacted audience</span></span>

<span data-ttu-id="ad56e-574">Az összes partner, aki a Felhőszolgáltató (CSP) programon keresztül megy keresztül</span><span class="sxs-lookup"><span data-stu-id="ad56e-574">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-575">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-575">Details</span></span>

<span data-ttu-id="ad56e-576">2021. április 1-ével a Microsoft a következő új termékeket és ajánlatokat bocsátja ki:</span><span class="sxs-lookup"><span data-stu-id="ad56e-576">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="ad56e-577">Power BI Premium felhasználónként</span><span class="sxs-lookup"><span data-stu-id="ad56e-577">Power BI Premium Per User</span></span>
- <span data-ttu-id="ad56e-578">Customer Voice and Marketing USL geo- és szegmensbővítés</span><span class="sxs-lookup"><span data-stu-id="ad56e-578">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="ad56e-579">**Power BI Premium felhasználónként**</span><span class="sxs-lookup"><span data-stu-id="ad56e-579">**Power BI Premium Per User**</span></span>

<span data-ttu-id="ad56e-580">A Microsoft bemutatja az első felhasználónkénti Power BI Premium ajánlatát.</span><span class="sxs-lookup"><span data-stu-id="ad56e-580">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="ad56e-581">Power BI Premium jelenleg csak kapacitási szerkezetben értékesítik.</span><span class="sxs-lookup"><span data-stu-id="ad56e-581">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="ad56e-582">Power BI Premium felhasználónkénti hozzáférés a vállalati üzletiintelligencia- (BI-) és elemzési képességekhez.</span><span class="sxs-lookup"><span data-stu-id="ad56e-582">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="ad56e-583">A rugalmas egyéni helylicencek kis- és középvállalatok számára is használhatók.</span><span class="sxs-lookup"><span data-stu-id="ad56e-583">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="ad56e-584">Az [ajánlatról Power BI tekintse](/power-platform-release-plan/2020wave2/power-bi/planned-features) át a következő kiadási részleteket: .</span><span class="sxs-lookup"><span data-stu-id="ad56e-584">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="ad56e-585">**Ajánlat részletei**</span><span class="sxs-lookup"><span data-stu-id="ad56e-585">**Offer details**</span></span>

<span data-ttu-id="ad56e-586">Vegye figyelembe, hogy az ajánlat neve kis mértékben eltér az árlista előnézetének nevétől.</span><span class="sxs-lookup"><span data-stu-id="ad56e-586">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="ad56e-587">Ajánlat neve</span><span class="sxs-lookup"><span data-stu-id="ad56e-587">Offer name</span></span> | <span data-ttu-id="ad56e-588">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="ad56e-588">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="ad56e-589">Power BI Premium felhasználónként</span><span class="sxs-lookup"><span data-stu-id="ad56e-589">Power BI Premium Per User</span></span> | <span data-ttu-id="ad56e-590">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="ad56e-590">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="ad56e-591">Power BI Premium oktatók felhasználónkénti száma</span><span class="sxs-lookup"><span data-stu-id="ad56e-591">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="ad56e-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="ad56e-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="ad56e-593">Power BI Premium felhasználónkénti diákoknak</span><span class="sxs-lookup"><span data-stu-id="ad56e-593">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="ad56e-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="ad56e-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="ad56e-595">Power BI Premium felhasználónkénti (nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="ad56e-595">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="ad56e-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="ad56e-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="ad56e-597">Power BI Premium felhasználónkénti Add-On</span><span class="sxs-lookup"><span data-stu-id="ad56e-597">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="ad56e-598">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="ad56e-598">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="ad56e-599">Power BI Premium felhasználónkénti Add-On oktatóknak</span><span class="sxs-lookup"><span data-stu-id="ad56e-599">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="ad56e-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="ad56e-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="ad56e-601">Power BI Premium felhasználónkénti Add-On diákoknak</span><span class="sxs-lookup"><span data-stu-id="ad56e-601">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="ad56e-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="ad56e-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="ad56e-603">Power BI Premium felhasználónkénti Add-On (nonprofit személyzet díjszabása)</span><span class="sxs-lookup"><span data-stu-id="ad56e-603">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="ad56e-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="ad56e-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="ad56e-605">**Customer Voice and Marketing USL geo- és szegmensbővítés**</span><span class="sxs-lookup"><span data-stu-id="ad56e-605">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="ad56e-606">A 2020. decemberi bevezetés után a Dynamics 365 Customer Voice and Marketing USL-ajánlatok módosultak, hogy új országokat, valamint további nonprofit és oktatási termékkódokat adjanak hozzá.</span><span class="sxs-lookup"><span data-stu-id="ad56e-606">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="ad56e-607">Ajánlat neve</span><span class="sxs-lookup"><span data-stu-id="ad56e-607">Offer name</span></span> | <span data-ttu-id="ad56e-608">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="ad56e-608">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="ad56e-609">Dynamics 365 Customer Voice USL (Nonprofit alkalmazottak díjszabása)</span><span class="sxs-lookup"><span data-stu-id="ad56e-609">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="ad56e-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="ad56e-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="ad56e-611">Dynamics 365 Customer Voice USL oktatóknak</span><span class="sxs-lookup"><span data-stu-id="ad56e-611">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="ad56e-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="ad56e-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="ad56e-613">Ezekről az ajánlatokról az alábbi oldalakon talál további információt:</span><span class="sxs-lookup"><span data-stu-id="ad56e-613">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="ad56e-614">A Dynamics 365 Customer Service Voice kezdőlapja</span><span class="sxs-lookup"><span data-stu-id="ad56e-614">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="ad56e-615">A Dynamics 365 Marketing kezdőlapja</span><span class="sxs-lookup"><span data-stu-id="ad56e-615">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="ad56e-616">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-616">Next steps</span></span>

<span data-ttu-id="ad56e-617">Tekintse át az ebben a témakörben található forrásokat, és ossza meg ezt az információt a szervezet megfelelő érdekelt felével.</span><span class="sxs-lookup"><span data-stu-id="ad56e-617">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="ad56e-618">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-618">Questions?</span></span>

<span data-ttu-id="ad56e-619">Ha kérdései vannak ezekkel az ajánlatokkal kapcsolatban, tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="ad56e-619">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="ad56e-620">A Microsoft Univerzális nyomtatás egyes csomagokban már elérhető</span><span class="sxs-lookup"><span data-stu-id="ad56e-620">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="ad56e-621">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="ad56e-621">Categories</span></span>

- <span data-ttu-id="ad56e-622">Dátum: 2021-03-03</span><span class="sxs-lookup"><span data-stu-id="ad56e-622">Date: 2021-03-03</span></span>
- <span data-ttu-id="ad56e-623">Képességek</span><span class="sxs-lookup"><span data-stu-id="ad56e-623">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ad56e-624">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="ad56e-624">Summary</span></span>

<span data-ttu-id="ad56e-625">A Microsoft Univerzális nyomtatás 2021. március 1-től elérhető lesz a kiválasztott Microsoft 365 csomagokban és önálló bővítményként.</span><span class="sxs-lookup"><span data-stu-id="ad56e-625">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ad56e-626">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="ad56e-626">Impacted audience</span></span>

<span data-ttu-id="ad56e-627">Az összes partner, aki a Felhőszolgáltató (CSP) programon keresztül megy keresztül</span><span class="sxs-lookup"><span data-stu-id="ad56e-627">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="ad56e-628">Részletek</span><span class="sxs-lookup"><span data-stu-id="ad56e-628">Details</span></span>

<span data-ttu-id="ad56e-629">[Univerzális nyomtatás](https://aka.ms/universalprint) egy Microsoft 365 nyomtatószolgáltatás, amely feleslegessé teszi a helyszíni nyomtatókiszolgálókat, és lehetővé teszi a Windows-eszközök számára az Azure-ban regisztrált nyomtatókra való nyomtatást.</span><span class="sxs-lookup"><span data-stu-id="ad56e-629">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="ad56e-630">A tranzakció 2021. március 1-től lesz elérhető.</span><span class="sxs-lookup"><span data-stu-id="ad56e-630">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="ad56e-631">A dolgozóknak előnyére válik az illesztőprogram nélküli nyomtatás, az egyszerűsített helyalapú nyomtatófelderítés, valamint az intuitív, tanuláshoz nem használható nyomtatási élmény.</span><span class="sxs-lookup"><span data-stu-id="ad56e-631">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="ad56e-632">A Azure Active Directory (Azure AD) szolgáltatáshoz Azure Active Directory eszközök meglévő Azure AD-beli hitelesítő adatokat használják a biztonságos nyomtatáshoz.</span><span class="sxs-lookup"><span data-stu-id="ad56e-632">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="ad56e-633">A rendszergazdák a nyomtatást a Azure Portal kezelhetik, és könnyedén csatlakoztathatják a nyomtatókat a Univerzális nyomtatás.</span><span class="sxs-lookup"><span data-stu-id="ad56e-633">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="ad56e-634">Univerzális nyomtatás szoftverrel a nem kompatibilis nyomtatókkal Univerzális nyomtatás összekötője telepíthetők.</span><span class="sxs-lookup"><span data-stu-id="ad56e-634">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="ad56e-635">Univerzális nyomtatás a Windows E3, A3, E5 és A5 rendszerekre való indításkor, valamint az Microsoft 365 BP, F3, E3, A3, E5 és A5 rendszerekre.</span><span class="sxs-lookup"><span data-stu-id="ad56e-635">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="ad56e-636">**Ajánlat részletei**</span><span class="sxs-lookup"><span data-stu-id="ad56e-636">**Offer details**</span></span>

<span data-ttu-id="ad56e-637">Vegye figyelembe, hogy az ajánlat neve kis mértékben eltér az árlista előnézetének nevétől.</span><span class="sxs-lookup"><span data-stu-id="ad56e-637">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="ad56e-638">Ajánlat neve</span><span class="sxs-lookup"><span data-stu-id="ad56e-638">Offer name</span></span> | <span data-ttu-id="ad56e-639">Ajánlat azonosítója</span><span class="sxs-lookup"><span data-stu-id="ad56e-639">Offer ID</span></span> | <span data-ttu-id="ad56e-640">Anyagazonosító</span><span class="sxs-lookup"><span data-stu-id="ad56e-640">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="ad56e-641">Univerzális nyomtatás bővítmény (500 feladat) – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ad56e-641">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="ad56e-642">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="ad56e-642">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="ad56e-643">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="ad56e-643">9BI-00004</span></span>   |
| <span data-ttu-id="ad56e-644">Univerzális nyomtatás mennyiségi bővítmény (500 feladat) oktatók számára – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ad56e-644">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="ad56e-645">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="ad56e-645">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="ad56e-646">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="ad56e-646">9BK-00004</span></span>   |
| <span data-ttu-id="ad56e-647">Univerzális nyomtatás bővítmény (500 feladat) – Windows</span><span class="sxs-lookup"><span data-stu-id="ad56e-647">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="ad56e-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="ad56e-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="ad56e-649">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="ad56e-649">9BI-00002</span></span>   |
| <span data-ttu-id="ad56e-650">Univerzális nyomtatás kötet bővítménye (500 feladat) oktatók számára – Windows</span><span class="sxs-lookup"><span data-stu-id="ad56e-650">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="ad56e-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="ad56e-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="ad56e-652">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="ad56e-652">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="ad56e-653">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad56e-653">Next steps</span></span>

<span data-ttu-id="ad56e-654">Ismerkedjen meg az árlistával és a Univerzális nyomtatás [áttekintésével.](/universal-print/fundamentals/universal-print-whatis)</span><span class="sxs-lookup"><span data-stu-id="ad56e-654">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="ad56e-655">Ossza meg ezt az információt a szervezet összes megfelelő kapcsolattartóval.</span><span class="sxs-lookup"><span data-stu-id="ad56e-655">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="ad56e-656">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="ad56e-656">Questions?</span></span>

<span data-ttu-id="ad56e-657">Az ajánlatokkal kapcsolatos kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="ad56e-657">For any questions about these offers, check your relevant Yammer communities.</span></span>