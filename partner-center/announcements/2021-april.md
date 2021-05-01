---
title: 2021. áprilisi bejelentések
description: A Microsoft 2021. áprilisi közleményei Partnerközpont új képességeket, promóciókat, ajánlatokat, piacokat vagy a meglévő ajánlatok változásait is beleértve.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: d26d1af994ae9a3f951ee9428ee6fd092b2c91d8
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328049"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="25140-103">2021. áprilisi bejelentések</span><span class="sxs-lookup"><span data-stu-id="25140-103">April 2021 announcements</span></span>

<span data-ttu-id="25140-104">Ez az oldal a Microsoft Partnerközpont 2021 áprilisára vonatkozó közleményeket tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="25140-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="25140-105">Készenlét: A frissített CSP-ügyfélcím-ellenőrzési API júniusban lesz elérhető; tesztelési képesség már elérhető</span><span class="sxs-lookup"><span data-stu-id="25140-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="25140-106">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="25140-106">Categories</span></span>

- <span data-ttu-id="25140-107">Dátum: 2021-04-30</span><span class="sxs-lookup"><span data-stu-id="25140-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="25140-108">Készenlét</span><span class="sxs-lookup"><span data-stu-id="25140-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="25140-109">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="25140-109">Summary</span></span>

<span data-ttu-id="25140-110">Annak érdekében, hogy a partnerek és az ügyfelek bizalom alapján futtassanak üzleti munkájukat, meghívjuk a partnereket, hogy teszteljék a Validate Address API módosításait a világ minden országában.</span><span class="sxs-lookup"><span data-stu-id="25140-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="25140-111">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="25140-111">Impacted audience</span></span>

<span data-ttu-id="25140-112">CsP – közvetlen számlázási partnerek és közvetett szolgáltatók, akik új ügyfelek címadatokat hoznak létre vagy frissítnek</span><span class="sxs-lookup"><span data-stu-id="25140-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="25140-113">Részletek</span><span class="sxs-lookup"><span data-stu-id="25140-113">Details</span></span>

<span data-ttu-id="25140-114">A Microsoft megbízhatósági kapcsolaton fut.</span><span class="sxs-lookup"><span data-stu-id="25140-114">Microsoft runs on trust.</span></span> <span data-ttu-id="25140-115">Elkötelezettek vagyunk amellett, hogy megfelelő, biztonságos és biztonságos módszert biztosítsunk az ügyfélcímek érvényesítéséhez az ügyfél-előfizetések tranzakciója során a CSP-programban.</span><span class="sxs-lookup"><span data-stu-id="25140-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="25140-116">2021. március 31-én bevezettük a Validate Address API módosításait.</span><span class="sxs-lookup"><span data-stu-id="25140-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="25140-117">Meghívjuk a partnereket, hogy teszteljék az API-t a 2021. június végi élő adás előtt.</span><span class="sxs-lookup"><span data-stu-id="25140-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="25140-118">Vegye figyelembe, hogy ezek a módosítások csak a Validate Address API-t érintik.</span><span class="sxs-lookup"><span data-stu-id="25140-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="25140-119">Az Ügyfél és a Számlázási profil API-k frissítése api-kat ez nem érinti.</span><span class="sxs-lookup"><span data-stu-id="25140-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="25140-120">Bár a javasolt címet jelenleg nem kell használni az Ügyfél létrehozása API-val, erősen ajánlott.</span><span class="sxs-lookup"><span data-stu-id="25140-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="25140-121">A válasz a következő állapotüzenetek egyikét adja vissza:</span><span class="sxs-lookup"><span data-stu-id="25140-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="25140-122">Állapot</span><span class="sxs-lookup"><span data-stu-id="25140-122">Status</span></span>     | <span data-ttu-id="25140-123">Leírás</span><span class="sxs-lookup"><span data-stu-id="25140-123">Description</span></span> |    <span data-ttu-id="25140-124">A visszaadott javasolt címek száma</span><span class="sxs-lookup"><span data-stu-id="25140-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="25140-125">Ellenőrzött szállításra használható</span><span class="sxs-lookup"><span data-stu-id="25140-125">Verified shippable</span></span> | <span data-ttu-id="25140-126">A cím ellenőrizve van, és szállítható a címre.</span><span class="sxs-lookup"><span data-stu-id="25140-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="25140-127">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="25140-127">Single</span></span> |
|<span data-ttu-id="25140-128">Ellenőrzött</span><span class="sxs-lookup"><span data-stu-id="25140-128">Verified</span></span> | <span data-ttu-id="25140-129">A cím ellenőrizve van.</span><span class="sxs-lookup"><span data-stu-id="25140-129">Address is verified.</span></span> | <span data-ttu-id="25140-130">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="25140-130">Single</span></span> |
|<span data-ttu-id="25140-131">Beavatkozás szükséges</span><span class="sxs-lookup"><span data-stu-id="25140-131">Interaction required</span></span> | <span data-ttu-id="25140-132">A javasolt cím jelentős mértékben módosult, és a felhasználó megerősítését kell kér.</span><span class="sxs-lookup"><span data-stu-id="25140-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="25140-133">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="25140-133">Single</span></span> |
|<span data-ttu-id="25140-134">Utca részleges</span><span class="sxs-lookup"><span data-stu-id="25140-134">Street partial</span></span> | <span data-ttu-id="25140-135">A címben megadott utca részleges, és további információra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="25140-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="25140-136">Multiple – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="25140-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="25140-137">Részleges helyszín</span><span class="sxs-lookup"><span data-stu-id="25140-137">Premises partial</span></span> | <span data-ttu-id="25140-138">Az adott helyszín (épületszám, csomagszám stb.) részleges, és további információra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="25140-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="25140-139">Multiple – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="25140-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="25140-140">Többszörös</span><span class="sxs-lookup"><span data-stu-id="25140-140">Multiple</span></span> | <span data-ttu-id="25140-141">Több mező is részleges a címben (beleértve az utca részleges és a helyszíni részleges mezőket is).</span><span class="sxs-lookup"><span data-stu-id="25140-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="25140-142">Multiple – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="25140-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="25140-143">Nincsenek</span><span class="sxs-lookup"><span data-stu-id="25140-143">None</span></span> | <span data-ttu-id="25140-144">A cím helytelen.</span><span class="sxs-lookup"><span data-stu-id="25140-144">Address is incorrect.</span></span> | <span data-ttu-id="25140-145">Nincsenek</span><span class="sxs-lookup"><span data-stu-id="25140-145">None</span></span> |
|<span data-ttu-id="25140-146">Nincs ellenőrizve.</span><span class="sxs-lookup"><span data-stu-id="25140-146">Not validated</span></span> | <span data-ttu-id="25140-147">A címet nem sikerült elküldeni az érvényesítési folyamaton keresztül.</span><span class="sxs-lookup"><span data-stu-id="25140-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="25140-148">Nincsenek</span><span class="sxs-lookup"><span data-stu-id="25140-148">None</span></span> |

<span data-ttu-id="25140-149">Az USA-nak az utókódja egy további négy számjegyet + kötőjelet ad vissza, például: 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="25140-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="25140-150">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="25140-150">Next steps</span></span>

- <span data-ttu-id="25140-151">Részletesebb útmutatásért tekintse át a műszaki dokumentációt és a dedikált [partnergyűjteményben](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) található gyakori kérdéseket.</span><span class="sxs-lookup"><span data-stu-id="25140-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="25140-152">Készüljön fel arra, hogy a módosításokat a Partnerközpont API és a webes felhasználói felület használatával építse be.</span><span class="sxs-lookup"><span data-stu-id="25140-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="25140-153">Ossza meg a tesztgép bérlőazonosítóját az érintett szakértővel (Ali Mertki), hogy felveje a tesztjáratba, hogy megkezdje a frissítés előkészítését.</span><span class="sxs-lookup"><span data-stu-id="25140-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="25140-154">Ha vezérlőpult-szállítói (CPV) megoldást használ, tekintse meg a CPV-t.</span><span class="sxs-lookup"><span data-stu-id="25140-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="25140-155">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="25140-155">Questions?</span></span>

<span data-ttu-id="25140-156">Ha támogatásra van szüksége a Microsofttal kapcsolatos műveleteihez, kérje a partnertámogatási Yammer-csoportját, vagy nyisson meg egy [szolgáltatáskérést.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="25140-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="25140-157">Az API Swagger Partnerközpont dokumentáció új helye</span><span class="sxs-lookup"><span data-stu-id="25140-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="25140-158">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="25140-158">Categories</span></span>

- <span data-ttu-id="25140-159">Dátum: 2021-04-26</span><span class="sxs-lookup"><span data-stu-id="25140-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="25140-160">Képességek</span><span class="sxs-lookup"><span data-stu-id="25140-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="25140-161">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="25140-161">Summary</span></span>

<span data-ttu-id="25140-162">Partnerközpont API Swagger-dokumentumok migrálva vannak az előző [Swagger-dokumentációs webhelyről](https://apidocs.microsoft.com/services/partnercenter) egy új [Swagger-dokumentációs webhelyre.](https://docs.microsoft.com/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="25140-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="25140-163">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="25140-163">Impacted audience</span></span>

<span data-ttu-id="25140-164">A felhőszolgáltatói (CSP Felhőszolgáltató programban részt vevő közvetlen számlázási partnerek és közvetett szolgáltatók, akik az Partnerközpont API-kat</span><span class="sxs-lookup"><span data-stu-id="25140-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="25140-165">Részletek</span><span class="sxs-lookup"><span data-stu-id="25140-165">Details</span></span>

<span data-ttu-id="25140-166">2021. április 26-tól az Partnerközpont API Swagger dokumentációja, beleértve a Rest API-tartalmakat is, egy új [webhelyen található.](https://docs.microsoft.com/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="25140-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="25140-167">A régi hely néhány hét után elérhetetlen lesz.</span><span class="sxs-lookup"><span data-stu-id="25140-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="25140-168">Előnyök</span><span class="sxs-lookup"><span data-stu-id="25140-168">Benefits</span></span>

<span data-ttu-id="25140-169">A Partnerközpont API Swagger dokumentációja egy **Try It függvényt biztosít.**</span><span class="sxs-lookup"><span data-stu-id="25140-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="25140-170">A függvény csak akkor használható, ha rendelkezik egy Bearer Token jogkivonattal, amelyet a Hitelesítés (Hitelesítés) Partnerközpont [követ.](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication)</span><span class="sxs-lookup"><span data-stu-id="25140-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="25140-171">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="25140-171">Next steps</span></span>

<span data-ttu-id="25140-172">Ossza meg ezt az információt a szervezeten belül, hogy a megfelelő csapat áttekintheti és frissítheti a folyamatait.</span><span class="sxs-lookup"><span data-stu-id="25140-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="25140-173">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="25140-173">Questions?</span></span>

<span data-ttu-id="25140-174">Az ajánlatokkal kapcsolatos kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="25140-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="25140-175">Felhőszolgáltató (CSP) szoftver visszaküldési időszakának szabályzata és letöltési hivatkozás lejárati értesítése</span><span class="sxs-lookup"><span data-stu-id="25140-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="25140-176">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="25140-176">Categories</span></span>

- <span data-ttu-id="25140-177">Dátum: 2021-04-21</span><span class="sxs-lookup"><span data-stu-id="25140-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="25140-178">Képességek</span><span class="sxs-lookup"><span data-stu-id="25140-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="25140-179">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="25140-179">Summary</span></span>

<span data-ttu-id="25140-180">A CSP szoftver visszaküldési időszakra vonatkozó szabályzata és a letöltési hivatkozás lejárata módosult.</span><span class="sxs-lookup"><span data-stu-id="25140-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="25140-181">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="25140-181">Impacted audience</span></span>

<span data-ttu-id="25140-182">Folyamatos szoftver- vagy szoftver-előfizetési ajánlatokat a CSP-ban tranzakciós partnerek</span><span class="sxs-lookup"><span data-stu-id="25140-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="25140-183">Részletek</span><span class="sxs-lookup"><span data-stu-id="25140-183">Details</span></span>

<span data-ttu-id="25140-184">Vegye figyelembe a következő fontos értesítéseket a szoftver- és szoftver-előfizetések előfizetésen keresztüli folyamatos vásárlásával Partnerközpont:</span><span class="sxs-lookup"><span data-stu-id="25140-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="25140-185">Szoftver visszaküldési időszakának szabályzata</span><span class="sxs-lookup"><span data-stu-id="25140-185">Software return period policy</span></span>

<span data-ttu-id="25140-186">2021. június 1-től a CSP-ben az Microsoft Partnerszerződés (MPA) által meghatározott szoftveres ajánlatok visszatérési időtartama a megrendelés dátuma után 60 napról 30 napra változik.</span><span class="sxs-lookup"><span data-stu-id="25140-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="25140-187">A szoftverajánlatra vonatkozó megrendelés elküldése után a partnereknek a megrendelés dátuma után 30 nap áll a 30 napjuk arra, hogy bármely változatot elküldje az adott rendelésre:</span><span class="sxs-lookup"><span data-stu-id="25140-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="25140-188">A 30 napos visszatérési időszakban visszaadott állandó szoftverlicencek a fizetős vásárlási ár teljes jóváírását megkapják.</span><span class="sxs-lookup"><span data-stu-id="25140-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="25140-189">A 30 napos visszatérési időszakban visszaadott szoftver-előfizetési termékek a fizetős vásárlási ár időkorreklését kapják meg.</span><span class="sxs-lookup"><span data-stu-id="25140-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="25140-190">Ez az üzenet a 2020. december és 2021. április között az összes CSP-partnernek küldött, az MPA visszaküldési időszakával és egyéb frissítéseivel kapcsolatos e-mail-kommunikációnk követő üzenete.</span><span class="sxs-lookup"><span data-stu-id="25140-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="25140-191">Az MPA-t érintő változásokkal kapcsolatos részletekért tekintse meg ezeket a közleményeket.</span><span class="sxs-lookup"><span data-stu-id="25140-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="25140-192">Szoftverletöltési hivatkozás lejárata</span><span class="sxs-lookup"><span data-stu-id="25140-192">Software download link expiry</span></span>

<span data-ttu-id="25140-193">2021. június 3-tól a szoftverletöltési hivatkozások az Partnerközpont-ig tartó végleges szoftver- és szoftver-előfizetési termékvásárlások lejárati dátuma a kezdeti letöltéstől számított öt nap lesz.</span><span class="sxs-lookup"><span data-stu-id="25140-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="25140-194">A lejárati időszak 2021. június 3. előtt minden vásárlásra vonatkozik, valamint 2021. június 3-án és után is.</span><span class="sxs-lookup"><span data-stu-id="25140-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="25140-195">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="25140-195">Next steps</span></span>

<span data-ttu-id="25140-196">Tekintse át a CSP visszaküldési [időszakát,](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)és töltse le a hivatkozás lejáratával kapcsolatos gyakori kérdéseket, és tájékoztassa a szervezet összes megfelelő csapatát a változásokról:</span><span class="sxs-lookup"><span data-stu-id="25140-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="25140-197">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="25140-197">Questions?</span></span>

<span data-ttu-id="25140-198">Az ajánlatokkal kapcsolatos kérdésekért tekintse meg a kapcsolódó Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="25140-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="25140-199">Nyílt licencprogram: Viszonteladók váltása a Felhőszolgáltató (CSP) programra</span><span class="sxs-lookup"><span data-stu-id="25140-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="25140-200">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="25140-200">Categories</span></span>

- <span data-ttu-id="25140-201">Dátum: 2021. 04. 19.</span><span class="sxs-lookup"><span data-stu-id="25140-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="25140-202">Üzleti növekedés</span><span class="sxs-lookup"><span data-stu-id="25140-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="25140-203">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="25140-203">Summary</span></span>

<span data-ttu-id="25140-204">Ez a kommunikáció részletesen bemutatja, hogyan készül fel a hamarosan az Open Licensing Program módosításaira.</span><span class="sxs-lookup"><span data-stu-id="25140-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="25140-205">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="25140-205">Impacted audience</span></span>

<span data-ttu-id="25140-206">CSP- és Open-licencpartnerek</span><span class="sxs-lookup"><span data-stu-id="25140-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="25140-207">Részletek</span><span class="sxs-lookup"><span data-stu-id="25140-207">Details</span></span>

<span data-ttu-id="25140-208">2020-ban a [Microsoft](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) bejelentette, hogy a folyamatos szoftverlicencek széles körben elérhetők lesznek a partnerek és az ügyfelek számára a Felhőszolgáltató (CSP) programon keresztül.</span><span class="sxs-lookup"><span data-stu-id="25140-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="25140-209">Az első mérföldkövet 2021 januárban érte el, amikor elérhetővé váltak a kereskedelmi célú folyamatos szoftveres ajánlatok.</span><span class="sxs-lookup"><span data-stu-id="25140-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="25140-210">A következő fontos mérföldkő 2021 júliusában következik be, amikor [elérhetővé](https://aka.ms/openlicensepublicsector) válnak a közszférában elérhető ajánlatok.</span><span class="sxs-lookup"><span data-stu-id="25140-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="25140-211">Arról [is](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) tájékoztattunk, hogy 2022. január 1-től az Open License programon keresztül nem lehet új szoftverlicenc-vásárlásokat vagy Frissítési Garancia online szolgáltatások-licenceket vásárolni vagy megújítni.</span><span class="sxs-lookup"><span data-stu-id="25140-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="25140-212">A folyamatos szoftvernek a CSP-programra való átállása az új kereskedelmi élményben segít a partnereknek abban, hogy bővítsék a lehetőségeket, hogy változatos megoldásokat és felügyelt szolgáltatásokat kínálnak.</span><span class="sxs-lookup"><span data-stu-id="25140-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="25140-213">Ez felgyorsítja az ügyfelek felhőre való áttérését is.</span><span class="sxs-lookup"><span data-stu-id="25140-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="25140-214">A partnerek és az ügyfelek zökkenőmentes átállásának biztosítása érdekében a következő módosításokat és anyagokat végeztünk el a digitális átalakítás felgyorsítása érdekében:</span><span class="sxs-lookup"><span data-stu-id="25140-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="25140-215">2021. április</span><span class="sxs-lookup"><span data-stu-id="25140-215">April 2021</span></span>

<span data-ttu-id="25140-216">[Mostantól elérhető:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Licencek közötti váltás a CSP-be viszonteladók számára</span><span class="sxs-lookup"><span data-stu-id="25140-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="25140-217">2021. július</span><span class="sxs-lookup"><span data-stu-id="25140-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="25140-218">CSP</span><span class="sxs-lookup"><span data-stu-id="25140-218">CSP</span></span>

- <span data-ttu-id="25140-219">Július 1. : A közszférában dolgozó ügyfelek számára elérhető folyamatos szoftverlicencek</span><span class="sxs-lookup"><span data-stu-id="25140-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="25140-220">Július 7.: Visual Studio Pro és a Get Genuine Windows Agreement folyamatos szoftverlicencek, amelyek minden szegmensben elérhetők</span><span class="sxs-lookup"><span data-stu-id="25140-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="25140-221">Open Value</span><span class="sxs-lookup"><span data-stu-id="25140-221">Open Value</span></span>

- <span data-ttu-id="25140-222">Július 1. : Az Open Value program oktatási és nonprofit programjában elérhető további termékkódok, amelyek az Open License programhoz hasonló ajánlatokat érhetők el</span><span class="sxs-lookup"><span data-stu-id="25140-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="25140-223">Nyílt licenc</span><span class="sxs-lookup"><span data-stu-id="25140-223">Open License</span></span>

- <span data-ttu-id="25140-224">Július 1.: A Microsoft már nem indít új ajánlatokat az Open License programban.</span><span class="sxs-lookup"><span data-stu-id="25140-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="25140-225">2022. január</span><span class="sxs-lookup"><span data-stu-id="25140-225">January 2022</span></span>

- <span data-ttu-id="25140-226">Január 1. : Az Open License programon keresztül nem lehet új vásárlást vagy megújítást vásárolni</span><span class="sxs-lookup"><span data-stu-id="25140-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="25140-227">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="25140-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="25140-228">Közvetett CSP-szolgáltatók</span><span class="sxs-lookup"><span data-stu-id="25140-228">CSP indirect providers</span></span>

<span data-ttu-id="25140-229">Az elkövetkező hónapokban segítheti az Open License-viszonteladókat a CSP-programban való részvételben azáltal, hogy részt vesz a partnerek közösségi eseményeiben, és felhasználja az Open License-to-CSP váltási anyagokat a viszonteladók számára:</span><span class="sxs-lookup"><span data-stu-id="25140-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="25140-230">Nyissa meg a viszonteladóknak készült [Licenc–CSP](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)váltási anyagokat – Testreszabható áttekintő bemutató, e-mail-sablon, közvetett CSP-viszonteladói útmutató és egyéb anyagok, amelyek segítenek a viszonteladók nagy léptékű bevezetésében.</span><span class="sxs-lookup"><span data-stu-id="25140-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="25140-231">[A](https://globalpbocomm.eventbuilder.com/GlobalCSP) Microsoft Business Operations által üzemeltetett CSP-partnerközösségi események.</span><span class="sxs-lookup"><span data-stu-id="25140-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="25140-232">Csatlakozzon a különböző munkamenetekhez a CSP alapjainak elsajátításért (A CSP alapjai), vagy maradjon naprakész, és kérdéseket tudjon feltenni a CSP-szoftverekkel (Q&A munkamenetekkel).</span><span class="sxs-lookup"><span data-stu-id="25140-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="25140-233">(Hamarosan érkezik) A Microsoft Business Operations által üzemeltetett közvetett CSP-viszonteladói képzés.</span><span class="sxs-lookup"><span data-stu-id="25140-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="25140-234">Open License resellers (Licenc-viszonteladók megnyitása)</span><span class="sxs-lookup"><span data-stu-id="25140-234">Open License resellers</span></span>

- <span data-ttu-id="25140-235">Ha a szervezet jelenleg nincs regisztrálva a CSP-programban, az első lépésekről a terjesztőjéhez forduljon.</span><span class="sxs-lookup"><span data-stu-id="25140-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="25140-236">Itt csatlakozhat egy közvetett [szolgáltatóhoz.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)</span><span class="sxs-lookup"><span data-stu-id="25140-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="25140-237">Ha a szervezete már regisztrálva van a CSP-programban, itt olvashat a folyamatos szoftverről a [CSP-ban.](https://partner.microsoft.com/resources/collection/software-in-csp)</span><span class="sxs-lookup"><span data-stu-id="25140-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="25140-238">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="25140-238">Questions?</span></span>

<span data-ttu-id="25140-239">Az ajánlatokkal kapcsolatos további kérdésekért tekintse meg a kapcsolódó Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="25140-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="25140-240">Most élő: Globális promóciós készenlét-útmutató</span><span class="sxs-lookup"><span data-stu-id="25140-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="25140-241">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="25140-241">Categories</span></span>

- <span data-ttu-id="25140-242">Dátum: 2021. 04. 16.</span><span class="sxs-lookup"><span data-stu-id="25140-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="25140-243">Képességek</span><span class="sxs-lookup"><span data-stu-id="25140-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="25140-244">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="25140-244">Summary</span></span>

<span data-ttu-id="25140-245">A Launch Readiness közzétett egy új globális [promóciós](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) készenlét-útmutatót az Operations Readiness erőforrás-katalógusban.</span><span class="sxs-lookup"><span data-stu-id="25140-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="25140-246">Ez az útmutató az összes aktív globális promóció összevont [nézetét biztosítja.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)</span><span class="sxs-lookup"><span data-stu-id="25140-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="25140-247">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="25140-247">Impacted audience</span></span>

<span data-ttu-id="25140-248">Minden mennyiségi licencelési (VL- és Dynamics Price List-, DPL-) és Felhőszolgáltató (CSP-) partner</span><span class="sxs-lookup"><span data-stu-id="25140-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="25140-249">Részletek</span><span class="sxs-lookup"><span data-stu-id="25140-249">Details</span></span>

<span data-ttu-id="25140-250">A Microsoft partnerei megosztották velünk, hogy az összes globális promócióról összevont nézetet kell biztosítani támogató részletekkel.</span><span class="sxs-lookup"><span data-stu-id="25140-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="25140-251">Ezt az összevont útmutatót úgy szerette volna használni az promóciókban, hogy az összes rendelkezésre álló információ könnyen elérhető lesz egy központi és kényelmes helyen.</span><span class="sxs-lookup"><span data-stu-id="25140-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="25140-252">2021 áprilisában a Microsoft havonta frissíti ezt az útmutatót, és elérhető lesz az Operations Readiness erőforrás-katalógus egy dedikált Global Promóciós készenlét-útmutató gyűjteményében.</span><span class="sxs-lookup"><span data-stu-id="25140-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="25140-253">Az útmutatóra mutató hivatkozásokat a következő gyűjtemények is tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="25140-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="25140-254">[Indítsa el a naptárgyűjteményt,](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)amely központosított áttekintést nyújt a közelgő változásokról és indításról.</span><span class="sxs-lookup"><span data-stu-id="25140-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="25140-255">[Közösségi gyűjtemények,](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)amelyek a havi partnerhívásainkhoz kapcsolódó anyagokat tartalmaznak, és a közelgő változásokat és az aktuálisan fontos témaköröket emelik ki.</span><span class="sxs-lookup"><span data-stu-id="25140-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="25140-256">[Partneri hírlevelek,](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)például a CSP havi frissítése</span><span class="sxs-lookup"><span data-stu-id="25140-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="25140-257">Havi emlékeztetőként egy új bejelentést is Partnerközpont a globális promóciós készenlétre vonatkozó útmutató minden új kiadásával együtt.</span><span class="sxs-lookup"><span data-stu-id="25140-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="25140-258">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="25140-258">Next steps</span></span>

<span data-ttu-id="25140-259">Minden hónap elején megtalálja a legújabb [](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) globális promóciós készenlét-útmutatót az [Operations Readiness erőforrás-katalógusban.](https://partner.microsoft.com/resources)</span><span class="sxs-lookup"><span data-stu-id="25140-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="25140-260">Ossza meg ezt az információt a szervezet megfelelő kapcsolattartóival, és ossza meg velünk, mennyire hasznos ez az útmutató a "Hasznos volt ez az oldal?" című szakaszban.</span><span class="sxs-lookup"><span data-stu-id="25140-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="25140-261">gombra az egyes oldalak végén.</span><span class="sxs-lookup"><span data-stu-id="25140-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="25140-262">Áprilisi Felhőszolgáltató (CSP) közösségi frissítés és emlékeztetők</span><span class="sxs-lookup"><span data-stu-id="25140-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="25140-263">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="25140-263">Categories</span></span>

- <span data-ttu-id="25140-264">Dátum: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="25140-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="25140-265">Közösségi | Meghívók és emlékeztetők</span><span class="sxs-lookup"><span data-stu-id="25140-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="25140-266">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="25140-266">Summary</span></span>

<span data-ttu-id="25140-267">A CSP közösségi erőforrásai igény szerint és havonta frissítve érhetők el, hogy naprakész és felkészült legyen a CSP-programban való változásra.</span><span class="sxs-lookup"><span data-stu-id="25140-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="25140-268">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="25140-268">Impacted audience</span></span>

<span data-ttu-id="25140-269">CSP – közvetlen számlázási partnerek és közvetett szolgáltatók</span><span class="sxs-lookup"><span data-stu-id="25140-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="25140-270">Részletek</span><span class="sxs-lookup"><span data-stu-id="25140-270">Details</span></span>

<span data-ttu-id="25140-271">Ebben a hónapban az erőforrások a következő fő témaköröket tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="25140-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="25140-272">Frissítés a CSP-program fejlődésére és az Open License program változásaira</span><span class="sxs-lookup"><span data-stu-id="25140-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="25140-273">A CSP-ügyfelek egyes régiókban való felhasználói be- és beiratásai követelményeinek változásai</span><span class="sxs-lookup"><span data-stu-id="25140-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="25140-274">Az új kereskedelmi PDF-számla új formátuma a CSP-programban</span><span class="sxs-lookup"><span data-stu-id="25140-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="25140-275">A [CSP-közösséggyűjteményben](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)a következőt találja:</span><span class="sxs-lookup"><span data-stu-id="25140-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="25140-276">A letölthető [CSP Monthly Update](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)hírlevele, amely egy könnyen olvasható dokumentumban összesíti a legutóbbi CSP-közleményeket, frissítéseket, eseményeket és emlékeztetőket.</span><span class="sxs-lookup"><span data-stu-id="25140-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="25140-277">A [CSP bejelentési naptára,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)amely idővonal-nézetet biztosít a programot érintő közelgő változásokról.</span><span class="sxs-lookup"><span data-stu-id="25140-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="25140-278">Az új [termékindítási naptár,](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)ahol megtekintheti a hamarosan megjelenő termékindításokat és -ajánlatokat.</span><span class="sxs-lookup"><span data-stu-id="25140-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="25140-279">[A CSP elindítja a](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) frissítési erőforrásokat a legfontosabb üzemeltetési változásokon könnyen használható tartalommal.</span><span class="sxs-lookup"><span data-stu-id="25140-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="25140-280">[Frissítők és emlékeztetők](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) a fontos CSP-témakörökről, amelyek érdeklődést és lekérdezéseket kapnak.</span><span class="sxs-lookup"><span data-stu-id="25140-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="25140-281">CSP Community Call Q&As</span><span class="sxs-lookup"><span data-stu-id="25140-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="25140-282">Community Call Q&Mint érhetők el, amelyek segíthetnek a közelgő változásokkal kapcsolatos kérdésekben.</span><span class="sxs-lookup"><span data-stu-id="25140-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="25140-283">Regisztráljon most a CSP Community Call Q&Mivel ez áprilisban, májusban és júniusban zajlik.</span><span class="sxs-lookup"><span data-stu-id="25140-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="25140-284">Ezek a legújabb indításokkal, fontos frissítésekkel és emlékeztetőkvel fognak összpontosítani.</span><span class="sxs-lookup"><span data-stu-id="25140-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="25140-285">[Regisztráljon itt.](https://globalpbocomm.eventbuilder.com/GlobalCSP)</span><span class="sxs-lookup"><span data-stu-id="25140-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="25140-286">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="25140-286">Next steps</span></span>

<span data-ttu-id="25140-287">Tekintse át a közösségi erőforrásokat, és regisztráljon a Community Call Q&A-re.</span><span class="sxs-lookup"><span data-stu-id="25140-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="25140-288">Annak érdekében, hogy a lehető legtöbbet tudja kihozni a Community Call Q&A-ból, tekintse át az igény szerinti közösségi tartalmakat, és küldje el kérdéseit a hívás előtt legfeljebb 48 órával.</span><span class="sxs-lookup"><span data-stu-id="25140-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="25140-289">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="25140-289">Questions?</span></span>

<span data-ttu-id="25140-290">A HAVI CSP Community Call Q&A a legjobb hely a CSP-program változásaival kapcsolatos kérdésekhez.</span><span class="sxs-lookup"><span data-stu-id="25140-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="25140-291">Minden hónapban tekintse át az anyagokat, és küldje el előre a kérdéseit, hogy a munkamenetet az Ön számára legfontosabb témakörökre töltjük.</span><span class="sxs-lookup"><span data-stu-id="25140-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="25140-292">További információért forduljon a támogatási [szolgálathoz.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)</span><span class="sxs-lookup"><span data-stu-id="25140-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="reminder-deprecation-of-get-qualification-on-may-4-2021"></a><a name="4"></a><span data-ttu-id="25140-293">Emlékeztető: A GET-minősítés elalasztása 2021. május 4-én</span><span class="sxs-lookup"><span data-stu-id="25140-293">Reminder: Deprecation of GET qualification on May 4, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="25140-294">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="25140-294">Categories</span></span>

- <span data-ttu-id="25140-295">Dátum: 2021-04-09</span><span class="sxs-lookup"><span data-stu-id="25140-295">Date: 2021-04-09</span></span>
- <span data-ttu-id="25140-296">Képességek</span><span class="sxs-lookup"><span data-stu-id="25140-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="25140-297">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="25140-297">Impacted audience</span></span>

<span data-ttu-id="25140-298">Academic, Nonprofit és Government Community Cloud (GCC) ajánlatokat értékesítő partnerek a Felhőszolgáltató programon keresztül az Partnerközpont API-val</span><span class="sxs-lookup"><span data-stu-id="25140-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="25140-299">Részletek</span><span class="sxs-lookup"><span data-stu-id="25140-299">Details</span></span>

<span data-ttu-id="25140-300">Ez a bejelentés a decemberben megjelent Partnerközpont [továbbfejlesztéseit követi.](https://docs.microsoft.com/partner-center/announcements/2020-december#1)</span><span class="sxs-lookup"><span data-stu-id="25140-300">This announcement is a follow-up to the Partner Center [enhancements released in December](https://docs.microsoft.com/partner-center/announcements/2020-december#1).</span></span> <span data-ttu-id="25140-301">Ennek a kiadásnak a részeként új GET és POST Minősítési API-kat helyezett üzembe, ezért a meglévő GET-minősítést 2021. május 4-ig kivezetjük.</span><span class="sxs-lookup"><span data-stu-id="25140-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, the existing GET qualification will be retired by May 4, 2021.</span></span> <span data-ttu-id="25140-302">Erre az időszakra át kell tért az új POST Partnerközpont API-k használatára az Oktatási ajánlatok vásárlása során, valamint az új GET minősítési API-ra az előre minősített Nonprofit és GCC-ajánlatok megvásárlásához.</span><span class="sxs-lookup"><span data-stu-id="25140-302">By that time, you’ll need to have transitioned to using the new POST Partner Center APIs in purchase Education offers, and the new GET qualifications API to purchase prequalified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="25140-303">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="25140-303">Next steps</span></span>

- <span data-ttu-id="25140-304">A sikeres és időbeni átállás érdekében frissítsen az új API-kra.</span><span class="sxs-lookup"><span data-stu-id="25140-304">Update to the new APIs for a successful and timely transition.</span></span>

- <span data-ttu-id="25140-305">Tekintse át az Partnerközpont API új módosításait és útmutatóját az Operations Readiness resources: Partnerközpont Education ügyfélérvényesítési [folyamatának fejlesztései között.](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)</span><span class="sxs-lookup"><span data-stu-id="25140-305">Review the new Partner Center API changes and Guide in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="25140-306">Ossza meg ezeket az információkat a szervezet megfelelő csapatával és a viszonteladóival, hogy felkészüljenek ezekre a változásokra.</span><span class="sxs-lookup"><span data-stu-id="25140-306">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="25140-307">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="25140-307">Questions?</span></span>

<span data-ttu-id="25140-308">Az értesítéssel kapcsolatos kérdéseit a támogatási Partnerközpont [meg.](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)</span><span class="sxs-lookup"><span data-stu-id="25140-308">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="25140-309">Változási napló</span><span class="sxs-lookup"><span data-stu-id="25140-309">Change log</span></span>

- <span data-ttu-id="25140-310">Április: Emlékeztető a GET-minősítés hamarosan elalasztásról</span><span class="sxs-lookup"><span data-stu-id="25140-310">April: Reminder of upcoming deprecation of GET qualification</span></span> 
- <span data-ttu-id="25140-311">Február: Frissültek a GET és PUT-minősítések & idővonalai</span><span class="sxs-lookup"><span data-stu-id="25140-311">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>
- <span data-ttu-id="25140-312">Január: Emlékeztető a GET és PUT minősítések & elalasztásról</span><span class="sxs-lookup"><span data-stu-id="25140-312">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="25140-313">Az új kereskedelmi PDF-számla új formátuma a CSP-ben</span><span class="sxs-lookup"><span data-stu-id="25140-313">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="25140-314">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="25140-314">Categories</span></span>

- <span data-ttu-id="25140-315">Dátum: 2021-04-05</span><span class="sxs-lookup"><span data-stu-id="25140-315">Date: 2021-04-05</span></span>
- <span data-ttu-id="25140-316">Képességek</span><span class="sxs-lookup"><span data-stu-id="25140-316">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="25140-317">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="25140-317">Summary</span></span>

<span data-ttu-id="25140-318">A Microsoft új formátumot vezet be az új kereskedelmi PDF-számlához a Felhőszolgáltató -program (CSP) programjában, hogy a termékleírás helyett termékadatok szerint jelenítse meg a számlázási adatokat.</span><span class="sxs-lookup"><span data-stu-id="25140-318">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="25140-319">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="25140-319">Impacted audience</span></span>

<span data-ttu-id="25140-320">CSP-programon keresztül tranzakciós partnerek</span><span class="sxs-lookup"><span data-stu-id="25140-320">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="25140-321">Részletek</span><span class="sxs-lookup"><span data-stu-id="25140-321">Details</span></span>

<span data-ttu-id="25140-322">2021 májusával kezdődően a Microsoft új formátumot vezet be az új kereskedelmi PDF-számlához a CSP-programban, hogy termékleírás helyett termékadatok szerint jelenítse meg a számlázási adatokat.</span><span class="sxs-lookup"><span data-stu-id="25140-322">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="25140-323">Ezzel az új frissítéssel a sorelemeket terméktípus szerint összesítődve jelenítjük meg az összes terméket egy adott sorban.</span><span class="sxs-lookup"><span data-stu-id="25140-323">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="25140-324">A partnerek észrevehetnek egy ilyen változást a 2021. április 1. és 2021. április 30. közötti számlázási időszakra vonatkozó májusi számlán.</span><span class="sxs-lookup"><span data-stu-id="25140-324">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="25140-325">Az érintett ajánlatok a fenntartott Microsoft Azure, az Azure-előfizetések (Azure-csomag) és a Marketplace.</span><span class="sxs-lookup"><span data-stu-id="25140-325">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="25140-326">A számlaformátum frissítése után lekért jóváírási kérelmek az új formátumban jönnek létre.</span><span class="sxs-lookup"><span data-stu-id="25140-326">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="25140-327">Partneri előnyök</span><span class="sxs-lookup"><span data-stu-id="25140-327">Partner benefits</span></span>

<span data-ttu-id="25140-328">Ez a frissítés a következő fejlesztéseket tartalmazza a partnerek számlázási élményében:</span><span class="sxs-lookup"><span data-stu-id="25140-328">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="25140-329">Csökkentett számlaméret a kritikus adatok megőrzése közben</span><span class="sxs-lookup"><span data-stu-id="25140-329">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="25140-330">A formátum igazítása az iparági szabványokhoz a kompakt és felhasználóbarát számlákhoz</span><span class="sxs-lookup"><span data-stu-id="25140-330">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="25140-331">A következő elemekre ez nem lesz hatással:</span><span class="sxs-lookup"><span data-stu-id="25140-331">The following elements will not be affected:</span></span>

- <span data-ttu-id="25140-332">Számlázási összefoglaló oldal a számla PDF-fájlján</span><span class="sxs-lookup"><span data-stu-id="25140-332">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="25140-333">Meglévő számlázási API-k</span><span class="sxs-lookup"><span data-stu-id="25140-333">Existing invoicing APIs</span></span>

- <span data-ttu-id="25140-334">Egyeztetési fájlok (a részletes adatok lekért Recon-fájlokkal is lekért fájlok.)</span><span class="sxs-lookup"><span data-stu-id="25140-334">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="25140-335">Használati és licencalapú díjak számlái</span><span class="sxs-lookup"><span data-stu-id="25140-335">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="25140-336">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="25140-336">Next steps</span></span>

<span data-ttu-id="25140-337">Tekintse át a témakörrel kapcsolatos információkat a Microsoft partner [webhelyének Operations Readiness erőforrás-katalógusában.](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)</span><span class="sxs-lookup"><span data-stu-id="25140-337">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="25140-338">A számlázási és adózási témakörökről, például a számlázási erőforrásokról, a [](https://docs.microsoft.com/partner-center/billing) számlákról, a CSP-számlázásról és az adókról további információt a számlázással kapcsolatos szakaszban Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="25140-338">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](https://docs.microsoft.com/partner-center/billing) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="25140-339">A Felhőszolgáltató (CSP) ügyfélbehozatali követelményeinek változásai</span><span class="sxs-lookup"><span data-stu-id="25140-339">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="25140-340">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="25140-340">Categories</span></span>

- <span data-ttu-id="25140-341">Dátum: 2021-04-02</span><span class="sxs-lookup"><span data-stu-id="25140-341">Date: 2021-04-02</span></span>
- <span data-ttu-id="25140-342">Ajánlatok/piacok</span><span class="sxs-lookup"><span data-stu-id="25140-342">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="25140-343">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="25140-343">Summary</span></span>

<span data-ttu-id="25140-344">Elkötelezettségünk részeként, hogy segítsünk a partnereknek és az ügyfeleknek a bizalmi kapcsolaton alapuló üzleti tevékenységben, további ügyféladatokat kérünk 2021. március 25-ig.</span><span class="sxs-lookup"><span data-stu-id="25140-344">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="25140-345">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="25140-345">Impacted audience</span></span>

<span data-ttu-id="25140-346">A CSP közvetlen számlázási partnerek és közvetett szolgáltatók, akik új vagy meglévő ügyfelekkel vannak a következő szakaszban felsorolt országokban</span><span class="sxs-lookup"><span data-stu-id="25140-346">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="25140-347">Részletek</span><span class="sxs-lookup"><span data-stu-id="25140-347">Details</span></span>

<span data-ttu-id="25140-348">A Microsoft megbízhatósági kapcsolaton fut.</span><span class="sxs-lookup"><span data-stu-id="25140-348">Microsoft runs on trust.</span></span> <span data-ttu-id="25140-349">Elkötelezettek vagyunk amellett, hogy megfelelő, biztonságos és biztonságos ügyfél-ellenőrzési módszert biztosítsunk az ügyfél-előfizetések tranzakciója során a CSP-programban.</span><span class="sxs-lookup"><span data-stu-id="25140-349">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="25140-350">2021. március 25-én bevezetünk egy API- és felhasználói felületi (UI) fejlesztéseket Partnerközpont, amelyek hatással lesznek az alábbi két feltételnek megfelelő partnerekre:</span><span class="sxs-lookup"><span data-stu-id="25140-350">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="25140-351">A partner közvetlen számlázási kapcsolattal rendelkezik a Microsofttal (ami azt jelenti, hogy a partner közvetlen számlázási partner vagy közvetett szolgáltató).</span><span class="sxs-lookup"><span data-stu-id="25140-351">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="25140-352">A partner az alábbi országokban lévő új vagy meglévő ügyfelekkel működik együtt:</span><span class="sxs-lookup"><span data-stu-id="25140-352">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="25140-353">Thaiföld</span><span class="sxs-lookup"><span data-stu-id="25140-353">Thailand</span></span>
    - <span data-ttu-id="25140-354">Vietnam</span><span class="sxs-lookup"><span data-stu-id="25140-354">Vietnam</span></span>
    - <span data-ttu-id="25140-355">Törökország</span><span class="sxs-lookup"><span data-stu-id="25140-355">Turkey</span></span>
    - <span data-ttu-id="25140-356">Lengyelország</span><span class="sxs-lookup"><span data-stu-id="25140-356">Poland</span></span>
    - <span data-ttu-id="25140-357">Dél-afrikai Köztársaság</span><span class="sxs-lookup"><span data-stu-id="25140-357">South Africa</span></span>
    - <span data-ttu-id="25140-358">India</span><span class="sxs-lookup"><span data-stu-id="25140-358">India</span></span>
    - <span data-ttu-id="25140-359">Brazília</span><span class="sxs-lookup"><span data-stu-id="25140-359">Brazil</span></span>
    - <span data-ttu-id="25140-360">Irak</span><span class="sxs-lookup"><span data-stu-id="25140-360">Iraq</span></span>
    - <span data-ttu-id="25140-361">Mianmar</span><span class="sxs-lookup"><span data-stu-id="25140-361">Myanmar</span></span>
    - <span data-ttu-id="25140-362">Dél-Szudán</span><span class="sxs-lookup"><span data-stu-id="25140-362">South Sudan</span></span>
    - <span data-ttu-id="25140-363">Szaúd-Arábia</span><span class="sxs-lookup"><span data-stu-id="25140-363">Saudi Arabia</span></span>
    - <span data-ttu-id="25140-364">Egyesült Arab Emírségek</span><span class="sxs-lookup"><span data-stu-id="25140-364">United Arab Emirates</span></span>
    - <span data-ttu-id="25140-365">Venezuela</span><span class="sxs-lookup"><span data-stu-id="25140-365">Venezuela</span></span>

<span data-ttu-id="25140-366">A feltételeknek megfelelő partnereknek be kell majd nyújtaniuk az ügyfél céges regisztrációs azonosítóját (más néven az ügyfél szervezeti INN-ét) és telefonszámát, amikor legközelebb frissítik vagy létrehoznak egy előfizetést az adott ügyfél számára.</span><span class="sxs-lookup"><span data-stu-id="25140-366">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="25140-367">Ezek a partnerek középső nevet is megadhatnak az ügyfél számára.</span><span class="sxs-lookup"><span data-stu-id="25140-367">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="25140-368">Vegye figyelembe, hogy a céges regisztrációs azonosító hozzáadásakor az üzleti adóazonosítót kell használnia, nem az ügyfél személyes azonosítóját.</span><span class="sxs-lookup"><span data-stu-id="25140-368">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="25140-369">Azok a partnerek, akik az alábbi országokban lévő új vagy meglévő ügyfelekkel üzleti partnereket hoznak létre, már elő vannak útjára 2020 novemberében egy korábbi kiadással.</span><span class="sxs-lookup"><span data-stu-id="25140-369">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="25140-370">Örményország</span><span class="sxs-lookup"><span data-stu-id="25140-370">Armenia</span></span>
- <span data-ttu-id="25140-371">Azerbajdzsán</span><span class="sxs-lookup"><span data-stu-id="25140-371">Azerbaijan</span></span>
- <span data-ttu-id="25140-372">Belarusz</span><span class="sxs-lookup"><span data-stu-id="25140-372">Belarus</span></span>
- <span data-ttu-id="25140-373">Magyarország</span><span class="sxs-lookup"><span data-stu-id="25140-373">Hungary</span></span>
- <span data-ttu-id="25140-374">Kazahsztán</span><span class="sxs-lookup"><span data-stu-id="25140-374">Kazakhstan</span></span>
- <span data-ttu-id="25140-375">Kirgizisztán</span><span class="sxs-lookup"><span data-stu-id="25140-375">Kyrgyzstan</span></span>
- <span data-ttu-id="25140-376">Moldova</span><span class="sxs-lookup"><span data-stu-id="25140-376">Moldova</span></span>
- <span data-ttu-id="25140-377">Oroszország</span><span class="sxs-lookup"><span data-stu-id="25140-377">Russia</span></span>
- <span data-ttu-id="25140-378">Tádzsikisztán</span><span class="sxs-lookup"><span data-stu-id="25140-378">Tajikistan</span></span>
- <span data-ttu-id="25140-379">Ukrajna</span><span class="sxs-lookup"><span data-stu-id="25140-379">Ukraine</span></span>
- <span data-ttu-id="25140-380">Üzbegisztán</span><span class="sxs-lookup"><span data-stu-id="25140-380">Uzbekistan</span></span>

<span data-ttu-id="25140-381">A 2021. március végén az ügyfelekkel a világ többi részén partnerekkel is lehetősége lesz megadni a céges regisztrációs azonosítót, a telefonszámot és a középső nevet igény szerint.</span><span class="sxs-lookup"><span data-stu-id="25140-381">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="25140-382">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="25140-382">Next steps</span></span>

- <span data-ttu-id="25140-383">Részletesebb útmutatásért tekintse át a műszaki dokumentációt és a dedikált [partnergyűjtemény](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) gyakori kérdéseit.</span><span class="sxs-lookup"><span data-stu-id="25140-383">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="25140-384">Készüljön fel arra, hogy a módosításokat az API Partnerközpont webes felhasználói felület használatával építse be.</span><span class="sxs-lookup"><span data-stu-id="25140-384">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="25140-385">Az API/SDK-k elérhetők lesznek a teszteléshez.</span><span class="sxs-lookup"><span data-stu-id="25140-385">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="25140-386">A további adatokat mindenképpen el kell küldenünk az új ügyfelek előtt, vagy a meglévő ügyféladatok módosításakor.</span><span class="sxs-lookup"><span data-stu-id="25140-386">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="25140-387">Ha vezérlőpult-szállító (CPV) megoldást használ, tekintse meg a CPV-t.</span><span class="sxs-lookup"><span data-stu-id="25140-387">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="25140-388">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="25140-388">Questions?</span></span>

<span data-ttu-id="25140-389">Ha kérdése van a vállalat regisztrációs azonosítójával (más néven INN vagy TIN) kapcsolatban, lépjen kapcsolatba az adótanácsadóval vagy a helyi adóhivatalsal.</span><span class="sxs-lookup"><span data-stu-id="25140-389">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="25140-390">A Microsoft nem tud útmutatást nyújtani az adózási kérdésekkel kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="25140-390">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="25140-391">Ha támogatásra van szüksége a Microsofttal kapcsolatos műveleteihez, nyisson meg egy [szolgáltatáskérést.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="25140-391">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="25140-392">Az e havi termékbelövések és -ajánlatok megtekintése</span><span class="sxs-lookup"><span data-stu-id="25140-392">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="25140-393">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="25140-393">Categories</span></span>

- <span data-ttu-id="25140-394">Dátum: 2021-04-01</span><span class="sxs-lookup"><span data-stu-id="25140-394">Date: 2021-04-01</span></span>
- <span data-ttu-id="25140-395">Képességek</span><span class="sxs-lookup"><span data-stu-id="25140-395">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="25140-396">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="25140-396">Summary</span></span>

<span data-ttu-id="25140-397">Közzétették a 2021. áprilisi termékindítási naptárt.</span><span class="sxs-lookup"><span data-stu-id="25140-397">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="25140-398">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="25140-398">Impacted audience</span></span>

<span data-ttu-id="25140-399">Az összes partner, aki a Felhőszolgáltató (CSP) programon keresztül megy keresztül</span><span class="sxs-lookup"><span data-stu-id="25140-399">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="25140-400">Részletek</span><span class="sxs-lookup"><span data-stu-id="25140-400">Details</span></span>

<span data-ttu-id="25140-401">A 2021. [áprilisi](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) termékindítási naptár már elérhető az Üzemeltetési készenlét erőforrás-katalógusban.</span><span class="sxs-lookup"><span data-stu-id="25140-401">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="25140-402">A közelgő termékindításokat és -ajánlatokat itt megtekintheti.</span><span class="sxs-lookup"><span data-stu-id="25140-402">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="25140-403">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="25140-403">Next steps</span></span>

<span data-ttu-id="25140-404">Tekintse át [a termékindítási naptárt,](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)és ossza meg az információkat a szervezet megfelelő érdekelt felével.</span><span class="sxs-lookup"><span data-stu-id="25140-404">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="25140-405">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="25140-405">Questions?</span></span>

<span data-ttu-id="25140-406">Az ajánlatokkal kapcsolatos további kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="25140-406">For any further questions about these offers, check your relevant Yammer communities.</span></span>
