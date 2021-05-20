---
title: 2021. áprilisi közlemények
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
ms.openlocfilehash: 13b8ec9ddd82b38a265606809b8c39c07436e548
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150131"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="f2b2c-103">2021. áprilisi közlemények</span><span class="sxs-lookup"><span data-stu-id="f2b2c-103">April 2021 announcements</span></span>

<span data-ttu-id="f2b2c-104">Ez az oldal a Microsoft 2021. áprilisi Partnerközpont bejelentését mutatja be.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="f2b2c-105">Készenlét: A CSP frissített ügyfélcím-ellenőrzési API-ja júniusban lesz elérhető; tesztelési képesség már elérhető</span><span class="sxs-lookup"><span data-stu-id="f2b2c-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="f2b2c-106">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="f2b2c-106">Categories</span></span>

- <span data-ttu-id="f2b2c-107">Dátum: 2021-04-30</span><span class="sxs-lookup"><span data-stu-id="f2b2c-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="f2b2c-108">Készenlét</span><span class="sxs-lookup"><span data-stu-id="f2b2c-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="f2b2c-109">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="f2b2c-109">Summary</span></span>

<span data-ttu-id="f2b2c-110">Annak érdekében, hogy a partnerek és az ügyfelek bizalom alapján futtassanak üzletüket, meghívjuk a partnereket, hogy teszteljék a Validate Address API módosításait az összes országban világszerte.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="f2b2c-111">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="f2b2c-111">Impacted audience</span></span>

<span data-ttu-id="f2b2c-112">CsP – közvetlen számlázási partnerek és közvetett szolgáltatók, akik új ügyfelek címének adatait hozják létre vagy frissítik</span><span class="sxs-lookup"><span data-stu-id="f2b2c-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="f2b2c-113">Részletek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-113">Details</span></span>

<span data-ttu-id="f2b2c-114">A Microsoft megbízhatósági kapcsolaton fut.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-114">Microsoft runs on trust.</span></span> <span data-ttu-id="f2b2c-115">Elkötelezettek vagyunk amellett, hogy megfelelő, biztonságos és biztonságos módszert biztosítsunk az ügyfélcímek érvényesítéséhez az ügyfél-előfizetések tranzakciója során a CSP-programban.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="f2b2c-116">2021. március 31-től bevezettük a Validate Address API módosításait.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="f2b2c-117">Meghívjuk a partnereket, hogy teszteljék az API-t a 2021. június végi élő adás előtt.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="f2b2c-118">Vegye figyelembe, hogy ezek a módosítások csak a Validate Address API-t érintik.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="f2b2c-119">A Create Customer and Update Billing Profile API-kat ez nem érinti.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="f2b2c-120">Bár a javasolt címet jelenleg nem kell használni az Ügyfél létrehozása API-val, erősen ajánlott.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="f2b2c-121">A válasz a következő állapotüzenetek egyikét adja vissza:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="f2b2c-122">Állapot</span><span class="sxs-lookup"><span data-stu-id="f2b2c-122">Status</span></span>     | <span data-ttu-id="f2b2c-123">Leírás</span><span class="sxs-lookup"><span data-stu-id="f2b2c-123">Description</span></span> |    <span data-ttu-id="f2b2c-124">A visszaadott javasolt címek száma</span><span class="sxs-lookup"><span data-stu-id="f2b2c-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="f2b2c-125">Ellenőrzött szállításra használható</span><span class="sxs-lookup"><span data-stu-id="f2b2c-125">Verified shippable</span></span> | <span data-ttu-id="f2b2c-126">A cím ellenőrizve van, és szállítható a címre.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="f2b2c-127">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="f2b2c-127">Single</span></span> |
|<span data-ttu-id="f2b2c-128">Ellenőrzött</span><span class="sxs-lookup"><span data-stu-id="f2b2c-128">Verified</span></span> | <span data-ttu-id="f2b2c-129">A cím ellenőrizve van.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-129">Address is verified.</span></span> | <span data-ttu-id="f2b2c-130">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="f2b2c-130">Single</span></span> |
|<span data-ttu-id="f2b2c-131">Beavatkozás szükséges</span><span class="sxs-lookup"><span data-stu-id="f2b2c-131">Interaction required</span></span> | <span data-ttu-id="f2b2c-132">A javasolt cím jelentős mértékben módosult, és a felhasználó megerősítését kell kér.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="f2b2c-133">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="f2b2c-133">Single</span></span> |
|<span data-ttu-id="f2b2c-134">Utca részleges</span><span class="sxs-lookup"><span data-stu-id="f2b2c-134">Street partial</span></span> | <span data-ttu-id="f2b2c-135">A címben megadott utca részleges, és további információra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="f2b2c-136">Többszörös – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="f2b2c-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="f2b2c-137">Részleges helyszín</span><span class="sxs-lookup"><span data-stu-id="f2b2c-137">Premises partial</span></span> | <span data-ttu-id="f2b2c-138">Az adott helyszín (épületszám, csomagszám stb.) részleges, és további információra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="f2b2c-139">Többszörös – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="f2b2c-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="f2b2c-140">Többszörös</span><span class="sxs-lookup"><span data-stu-id="f2b2c-140">Multiple</span></span> | <span data-ttu-id="f2b2c-141">Több mező is részleges a címben (beleértve az utca részleges és a helyszíni részleges mezőket is).</span><span class="sxs-lookup"><span data-stu-id="f2b2c-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="f2b2c-142">Többszörös – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="f2b2c-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="f2b2c-143">None</span><span class="sxs-lookup"><span data-stu-id="f2b2c-143">None</span></span> | <span data-ttu-id="f2b2c-144">A cím helytelen.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-144">Address is incorrect.</span></span> | <span data-ttu-id="f2b2c-145">None</span><span class="sxs-lookup"><span data-stu-id="f2b2c-145">None</span></span> |
|<span data-ttu-id="f2b2c-146">Nincs ellenőrizve.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-146">Not validated</span></span> | <span data-ttu-id="f2b2c-147">A cím nem lett elküldve az érvényesítési folyamaton keresztül.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="f2b2c-148">None</span><span class="sxs-lookup"><span data-stu-id="f2b2c-148">None</span></span> |

<span data-ttu-id="f2b2c-149">Az USA-nak az irányítószámai további négy számjegyet és kötőjelet fognak visszaadni, például: 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="f2b2c-150">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="f2b2c-150">Next steps</span></span>

- <span data-ttu-id="f2b2c-151">Részletesebb útmutatásért tekintse át a műszaki dokumentációt és a dedikált [partnergyűjtemény](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) gyakori kérdéseit.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="f2b2c-152">Készüljön fel arra, hogy a módosításokat a Partnerközpont API és a webes felhasználói felület használatával építse be.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="f2b2c-153">Ossza meg a tesztgép bérlőazonosítóját a témaszakértővel (Ali Sandki), aki szerepelni fog a tesztúton, hogy megkezdje a frissítés előkészítését.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="f2b2c-154">Ha vezérlőpult-szállító (CPV) megoldást használ, tekintse meg a CPV-t.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="f2b2c-155">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="f2b2c-155">Questions?</span></span>

<span data-ttu-id="f2b2c-156">Ha támogatásra van szüksége a Microsofttal kapcsolatos műveleteihez, kérje a partnertámogatási Yammer-csoportját, vagy nyisson meg egy [szolgáltatáskérést.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="f2b2c-157">Az API Swagger Partnerközpont dokumentációjának új helye</span><span class="sxs-lookup"><span data-stu-id="f2b2c-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="f2b2c-158">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="f2b2c-158">Categories</span></span>

- <span data-ttu-id="f2b2c-159">Dátum: 2021. 04. 26.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="f2b2c-160">Képességek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="f2b2c-161">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="f2b2c-161">Summary</span></span>

<span data-ttu-id="f2b2c-162">Partnerközpont API Swagger-dokumentumok migrálva vannak az előző [Swagger-dokumentációs webhelyről](https://apidocs.microsoft.com/services/partnercenter) egy új [Swagger-dokumentációs webhelyre.](/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="f2b2c-163">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="f2b2c-163">Impacted audience</span></span>

<span data-ttu-id="f2b2c-164">A Felhőszolgáltató (CSP) programban részt vevő közvetlen számlázási partnerek és közvetett szolgáltatók, akik az Partnerközpont API-kat</span><span class="sxs-lookup"><span data-stu-id="f2b2c-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="f2b2c-165">Részletek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-165">Details</span></span>

<span data-ttu-id="f2b2c-166">2021. április 26-tól az Partnerközpont API Swagger dokumentációja, beleértve a REST API-tartalmakat is, egy új [webhelyen található.](/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="f2b2c-167">A régi hely néhány hét után elérhetetlen lesz.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="f2b2c-168">Előnyök</span><span class="sxs-lookup"><span data-stu-id="f2b2c-168">Benefits</span></span>

<span data-ttu-id="f2b2c-169">A Partnerközpont API Swagger dokumentációja egy **Try It függvényt biztosít.**</span><span class="sxs-lookup"><span data-stu-id="f2b2c-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="f2b2c-170">A függvény csak akkor használható, ha rendelkezik egy Bearer Token jogkivonattal, amelyet a hitelesítést Partnerközpont követve hozhat [létre.](/partner-center/develop/partner-center-authentication#app--user-authentication)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="f2b2c-171">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="f2b2c-171">Next steps</span></span>

<span data-ttu-id="f2b2c-172">Ossza meg ezt az információt a szervezeten belül, hogy a megfelelő csapat áttekintheti és frissítheti a folyamatait.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="f2b2c-173">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="f2b2c-173">Questions?</span></span>

<span data-ttu-id="f2b2c-174">Az ajánlatokkal kapcsolatos kérdésekért tekintse meg a kapcsolódó Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="f2b2c-175">Felhőszolgáltató (CSP) szoftver visszaküldési időszakának szabályzata és letöltési hivatkozás lejárati értesítése</span><span class="sxs-lookup"><span data-stu-id="f2b2c-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="f2b2c-176">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="f2b2c-176">Categories</span></span>

- <span data-ttu-id="f2b2c-177">Dátum: 2021. 04. 21.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="f2b2c-178">Képességek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="f2b2c-179">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="f2b2c-179">Summary</span></span>

<span data-ttu-id="f2b2c-180">A CSP szoftver visszaküldési időszakra vonatkozó szabályzata és a letöltési hivatkozás lejárata módosult.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="f2b2c-181">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="f2b2c-181">Impacted audience</span></span>

<span data-ttu-id="f2b2c-182">Folyamatos szoftver- vagy szoftver-előfizetési ajánlatokat a CSP-ban tranzakciós partnerek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="f2b2c-183">Részletek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-183">Details</span></span>

<span data-ttu-id="f2b2c-184">Vegye figyelembe a következő fontos értesítéseket a szoftver- és szoftver-előfizetések folyamatos vásárlásával kapcsolatban a Partnerközpont:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="f2b2c-185">Szoftver visszaküldési időszakának szabályzata</span><span class="sxs-lookup"><span data-stu-id="f2b2c-185">Software return period policy</span></span>

<span data-ttu-id="f2b2c-186">2021. június 1-től a CSP-ben az Microsoft Partnerszerződés (MPA) által meghatározott szoftver ajánlatok visszatérési időtartama a megrendelés dátuma és 30 napja között 60 napra változik.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="f2b2c-187">A szoftverajánlatra vonatkozó megrendelés elküldése után a partnereknek a megrendelés dátumát követően 30 nap áll a 30 napra, hogy bármely változatot elküldje az adott rendelésre:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="f2b2c-188">A 30 napos visszatérési időszakban visszaadott minden állandó szoftverlicenc teljes jóváírást kap a fizetős vásárlási árról.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="f2b2c-189">A 30 napos visszatérési időszakban visszaadott szoftver-előfizetési termékek a fizetős vásárlási ár időkorreklott jóváírását kapják meg.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="f2b2c-190">Ez az üzenet a 2020. december és 2021. április között az összes CSP-partnernek küldött, az MPA visszaküldési időszakával és egyéb frissítéseivel kapcsolatos e-mail-üzenetek követő üzenete.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="f2b2c-191">Az MPA-t érintő változásokkal kapcsolatos részletekért tekintse meg ezeket a közleményeket.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="f2b2c-192">Szoftverletöltési hivatkozás lejárata</span><span class="sxs-lookup"><span data-stu-id="f2b2c-192">Software download link expiry</span></span>

<span data-ttu-id="f2b2c-193">2021. június 3-tól a szoftverletöltési hivatkozások folyamatos szoftver- és szoftver-előfizetési termékvásárláshoz Partnerközpont lejárati dátuma a kezdeti letöltéstől számított öt nap lesz.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="f2b2c-194">A lejárati időszak 2021. június 3., illetve 2021. június 3. előtt és után minden vásárlásra érvényes lesz.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="f2b2c-195">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="f2b2c-195">Next steps</span></span>

<span data-ttu-id="f2b2c-196">Tekintse át [a CSP visszaküldési időszakát,](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)és töltse le a hivatkozás lejáratával kapcsolatos gyakori kérdéseket, és tájékoztassa a szervezet összes megfelelő csapatát ezekről a változásokról:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="f2b2c-197">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="f2b2c-197">Questions?</span></span>

<span data-ttu-id="f2b2c-198">Az ajánlatokkal kapcsolatos kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="f2b2c-199">Nyílt licencprogram: Viszonteladók váltása a Felhőszolgáltató (CSP) programra</span><span class="sxs-lookup"><span data-stu-id="f2b2c-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="f2b2c-200">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="f2b2c-200">Categories</span></span>

- <span data-ttu-id="f2b2c-201">Dátum: 2021-04-19</span><span class="sxs-lookup"><span data-stu-id="f2b2c-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="f2b2c-202">Üzleti növekedés</span><span class="sxs-lookup"><span data-stu-id="f2b2c-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="f2b2c-203">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="f2b2c-203">Summary</span></span>

<span data-ttu-id="f2b2c-204">Ez a kommunikáció részletesen bemutatja, hogyan készül fel a hamarosan a nyílt licencelési program módosításaira.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="f2b2c-205">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="f2b2c-205">Impacted audience</span></span>

<span data-ttu-id="f2b2c-206">CSP- és open-licencpartnerek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="f2b2c-207">Részletek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-207">Details</span></span>

<span data-ttu-id="f2b2c-208">2020-ban a [Microsoft](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) bejelentette, hogy a folyamatos szoftverlicencek széles körben elérhetők lesznek a partnerek és az ügyfelek számára a Felhőszolgáltató (CSP) programon keresztül.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="f2b2c-209">Az első mérföldkövet 2021 januárban érte el, amikor a kereskedelmi célú folyamatos szoftveres ajánlatok elérhetővé váltak.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="f2b2c-210">A következő fontos mérföldkő 2021 júliusában lesz, amikor elérhetővé válnak a [közszférában](https://aka.ms/openlicensepublicsector) elérhető ajánlatok.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="f2b2c-211">Arról [is](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) tájékoztattunk, hogy 2022. január 1-től az Open License programon keresztül nem lehet új szoftverlicenc-vásárlásokat vagy Frissítési Garancia online szolgáltatások licenceket vásárolni vagy megújítni.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="f2b2c-212">Az új kereskedelmi élményben a folyamatos szoftver a CSP-programra való áttérése segít a partnereknek abban, hogy bővítsék a különböző megoldások és felügyelt szolgáltatások kínálta lehetőségeket.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="f2b2c-213">Ez felgyorsítja az ügyfelek felhőre való áttérését is.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="f2b2c-214">A partnerek és az ügyfelek zökkenőmentes átállásának biztosítása érdekében ezeket a módosításokat és anyagokat azért végeztünk, hogy felgyorsítsuk a digitális átalakítást:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="f2b2c-215">2021. április</span><span class="sxs-lookup"><span data-stu-id="f2b2c-215">April 2021</span></span>

<span data-ttu-id="f2b2c-216">[Mostantól elérhető:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Licencről CSP-re váltásra használható anyagok viszonteladók számára</span><span class="sxs-lookup"><span data-stu-id="f2b2c-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="f2b2c-217">2021. július</span><span class="sxs-lookup"><span data-stu-id="f2b2c-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="f2b2c-218">CSP</span><span class="sxs-lookup"><span data-stu-id="f2b2c-218">CSP</span></span>

- <span data-ttu-id="f2b2c-219">Július 1. : A közszférában dolgozó ügyfelek számára elérhető folyamatos szoftverlicencek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="f2b2c-220">Július 7. Visual Studio: a Pro és a Get Genuine Windows Agreement folyamatos szoftverlicencek, amelyek minden szegmensben elérhetők</span><span class="sxs-lookup"><span data-stu-id="f2b2c-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="f2b2c-221">Nyitott érték</span><span class="sxs-lookup"><span data-stu-id="f2b2c-221">Open Value</span></span>

- <span data-ttu-id="f2b2c-222">Július 1. : Az Open Value program oktatási és nonprofit programjában elérhető további termékkódok, amelyek az Open License programhoz hasonló ajánlatokat érhetők el</span><span class="sxs-lookup"><span data-stu-id="f2b2c-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="f2b2c-223">Open License</span><span class="sxs-lookup"><span data-stu-id="f2b2c-223">Open License</span></span>

- <span data-ttu-id="f2b2c-224">Július 1. : A Microsoft már nem indít új ajánlatokat az Open License programban.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="f2b2c-225">2022. január</span><span class="sxs-lookup"><span data-stu-id="f2b2c-225">January 2022</span></span>

- <span data-ttu-id="f2b2c-226">Január 1. : Az Open License programon keresztül nem lehet új vásárlásokat vagy megújításokat vásárolni</span><span class="sxs-lookup"><span data-stu-id="f2b2c-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="f2b2c-227">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="f2b2c-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="f2b2c-228">Közvetett CSP-szolgáltatók</span><span class="sxs-lookup"><span data-stu-id="f2b2c-228">CSP indirect providers</span></span>

<span data-ttu-id="f2b2c-229">Az elkövetkező hónapokban segítheti az Open License-viszonteladókat a CSP-programba való beteknésekben azáltal, hogy részt vesz a partnerközösségi eseményekben, és a viszonteladóknak készült Open License-to-CSP áttűnésanyagokat használja:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="f2b2c-230">Nyissa meg a viszonteladók számára készült [licenc–CSP](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)áttérési anyagokat – Testre szabható áttekintő bemutató, e-mail-sablon, közvetett CSP-viszonteladói útmutató és egyéb anyagok, amelyek segítenek a viszonteladók nagy léptékű bevezetésében.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="f2b2c-231">[A](https://globalpbocomm.eventbuilder.com/GlobalCSP) Microsoft Business Operations által üzemeltetett CSP-partnerközösségi események.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="f2b2c-232">Csatlakozzon a különböző munkamenetekhez, és ismerje meg a CSP alapjait (a CSP alapjait), vagy maradjon naprakész, és kérdéseket te fel a CSP-szoftverekkel (Q&A munkamenetek).</span><span class="sxs-lookup"><span data-stu-id="f2b2c-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="f2b2c-233">(Hamarosan érkezik) A Microsoft Business Operations által üzemeltetett közvetett CSP-viszonteladói képzési munkamenet.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="f2b2c-234">Open License resellers (Licenc-viszonteladók megnyitása)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-234">Open License resellers</span></span>

- <span data-ttu-id="f2b2c-235">Ha a szervezet jelenleg nincs regisztrálva a CSP-programban, az első lépésekről a forgalmazótól érdeklődik.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="f2b2c-236">Itt csatlakozhat egy közvetett [szolgáltatóhoz.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="f2b2c-237">Ha a szervezete már regisztrálva van a CSP-programban, itt olvashat bővebben a folyamatos szoftverről a [CSP-ban.](https://partner.microsoft.com/resources/collection/software-in-csp)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="f2b2c-238">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="f2b2c-238">Questions?</span></span>

<span data-ttu-id="f2b2c-239">Az ajánlatokkal kapcsolatos további kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="f2b2c-240">Most élő: Globális promóciós készenlét útmutató</span><span class="sxs-lookup"><span data-stu-id="f2b2c-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="f2b2c-241">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="f2b2c-241">Categories</span></span>

- <span data-ttu-id="f2b2c-242">Dátum: 2021.04. 16.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="f2b2c-243">Képességek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="f2b2c-244">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="f2b2c-244">Summary</span></span>

<span data-ttu-id="f2b2c-245">A Launch Readiness [](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) közzétett egy új globális promóciós készenlét-útmutatót az Operations Readiness erőforrás-katalógusban.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="f2b2c-246">Ez az útmutató az összes aktív globális promóció összevont [nézetét biztosítja.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="f2b2c-247">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="f2b2c-247">Impacted audience</span></span>

<span data-ttu-id="f2b2c-248">Minden mennyiségi licencelési (VL), Dynamics Price List- (DPL-) és Felhőszolgáltató (CSP-) partner</span><span class="sxs-lookup"><span data-stu-id="f2b2c-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="f2b2c-249">Részletek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-249">Details</span></span>

<span data-ttu-id="f2b2c-250">A Microsoft partnerei megosztották velünk, hogy az összes globális promócióról összevont nézetet kell biztosítani támogató részletekkel.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="f2b2c-251">Ezt az összevont útmutatót úgy szerette volna használni, hogy az előléptetések abban a biztosban legyenek, hogy az összes elérhető információ könnyen elérhető lesz egy központi és kényelmes helyen.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="f2b2c-252">2021 áprilisában a Microsoft havonta frissíti ezt az útmutatót, és elérhető lesz egy dedikált Global Promóciós készenlét útmutató gyűjteményben az Operations Readiness erőforrás-katalógusban.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="f2b2c-253">Az útmutatóra mutató hivatkozásokat a következő gyűjtemények is tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="f2b2c-254">[Indítsa el a naptárgyűjteményt,](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)amely központosított áttekintést nyújt a közelgő változásokról és indításról.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="f2b2c-255">[Közösségi gyűjtemények,](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)amelyek a havi partnerhívásainkhoz kapcsolódó anyagokat tartalmaznak, és kiemelik a közelgő változásokat és a fontos, időben esedékes témaköröket.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="f2b2c-256">[Partneri hírlevelek,](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)például a CSP havi frissítése</span><span class="sxs-lookup"><span data-stu-id="f2b2c-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="f2b2c-257">Havi emlékeztetőként közzé is teszünk egy Partnerközpont a globális promóciós készenlétre vonatkozó útmutató minden új kiadásával.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="f2b2c-258">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="f2b2c-258">Next steps</span></span>

<span data-ttu-id="f2b2c-259">Minden hónap elején megtalálja a legújabb [](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) globális promóciós készenléti útmutatót az [Operations Readiness erőforrás-katalógusban.](https://partner.microsoft.com/resources)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="f2b2c-260">Ossza meg ezt az információt a szervezet megfelelő kapcsolattartóival, és ossza meg velünk, mennyire hasznos az útmutató a "Hasznos volt ez az oldal?" című szakaszban.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="f2b2c-261">gombra az egyes oldalak végén.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="f2b2c-262">Áprilisi Felhőszolgáltató (CSP) közösségi frissítés és emlékeztetők</span><span class="sxs-lookup"><span data-stu-id="f2b2c-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="f2b2c-263">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="f2b2c-263">Categories</span></span>

- <span data-ttu-id="f2b2c-264">Dátum: 2021. 04. 16.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="f2b2c-265">Közösségi | Meghívók és emlékeztetők</span><span class="sxs-lookup"><span data-stu-id="f2b2c-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="f2b2c-266">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="f2b2c-266">Summary</span></span>

<span data-ttu-id="f2b2c-267">A CSP közösségi erőforrásai igény szerint és havonta frissítve érhetők el, hogy naprakészen és felkészülve legyen a CSP-program változási lehetőségére.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="f2b2c-268">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="f2b2c-268">Impacted audience</span></span>

<span data-ttu-id="f2b2c-269">CsP – közvetlen számlázási partnerek és közvetett szolgáltatók</span><span class="sxs-lookup"><span data-stu-id="f2b2c-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="f2b2c-270">Részletek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-270">Details</span></span>

<span data-ttu-id="f2b2c-271">Ebben a hónapban az erőforrások a következő fő témaköröket tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="f2b2c-272">Frissítés a CSP-program fejlődésére és az Open License program változásaira</span><span class="sxs-lookup"><span data-stu-id="f2b2c-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="f2b2c-273">A CSP-ügyfelekre vonatkozó, bizonyos régiókban való ügyfél-behozatás követelményeinek változásai</span><span class="sxs-lookup"><span data-stu-id="f2b2c-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="f2b2c-274">Az új kereskedelmi PDF-számla formátuma a CSP-programban</span><span class="sxs-lookup"><span data-stu-id="f2b2c-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="f2b2c-275">A [CSP-közösséggyűjteményben](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)a következőt találja:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="f2b2c-276">A letölthető [CSP Monthly Update hírlevele,](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)amely egy könnyen olvasható dokumentumban összesíti a legutóbbi CSP-közleményeket, frissítéseket, eseményeket és emlékeztetőket.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="f2b2c-277">A [CSP bejelentési naptára,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)amely idővonal-nézetet biztosít a programot érintő közelgő változásokról.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="f2b2c-278">Az új [termékindítási naptár,](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)amelyben megtekintheti a hamarosan megjelenő termékindításokat és -ajánlatokat.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="f2b2c-279">[A CSP elindítja a](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) frissítési erőforrásokat a legfontosabb üzemeltetési változásokon könnyen használható tartalommal.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="f2b2c-280">[Frissítők és emlékeztetők](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) az érdeklődést és lekérdezéseket fogadó főbb CSP-témakörökről.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="f2b2c-281">CSP Community Call Q&As</span><span class="sxs-lookup"><span data-stu-id="f2b2c-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="f2b2c-282">Community Call Q&Mint elérhető, amely segít a közelgő változásokkal kapcsolatos kérdésekben.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="f2b2c-283">Regisztráljon most a CSP community Call Q&Az áprilisban, májusban és júniusban sorra kerül.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="f2b2c-284">Ezek a legújabb indításokkal, fontos frissítésekkel és emlékeztetőkvel fognak összpontosítani.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="f2b2c-285">[Regisztráljon itt.](https://globalpbocomm.eventbuilder.com/GlobalCSP)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="f2b2c-286">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="f2b2c-286">Next steps</span></span>

<span data-ttu-id="f2b2c-287">Tekintse át a közösségi erőforrásokat, és regisztráljon a Community Call Q&A-re.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="f2b2c-288">Annak érdekében, hogy a lehető legtöbbet tudja kihozni a Community Call Q&A-ból, tekintse át az igény szerinti közösségi tartalmat, és küldje el kérdéseit a hívás előtt legfeljebb 48 órával.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="f2b2c-289">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="f2b2c-289">Questions?</span></span>

<span data-ttu-id="f2b2c-290">A CSP-közösség havi Call Q&A a legjobb hely a CSP-program változásaival kapcsolatos kérdésekhez.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="f2b2c-291">Minden hónapban tekintse át az anyagokat, és küldje el kérdéseit előre, hogy a munkamenetet az Ön számára legfontosabb témakörökre töltjük.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="f2b2c-292">További információért forduljon a támogatási [szolgálathoz.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a><span data-ttu-id="f2b2c-293">Utolsó emlékeztető: GET-minősítés elalasztása 2021. május 6-án</span><span class="sxs-lookup"><span data-stu-id="f2b2c-293">Final reminder: Deprecation of GET qualification on May 6, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="f2b2c-294">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="f2b2c-294">Categories</span></span>

- <span data-ttu-id="f2b2c-295">Dátum: 2021-05-04</span><span class="sxs-lookup"><span data-stu-id="f2b2c-295">Date: 2021-05-04</span></span>

- <span data-ttu-id="f2b2c-296">Képességek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="f2b2c-297">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="f2b2c-297">Impacted audience</span></span>

<span data-ttu-id="f2b2c-298">Academic, Nonprofit és Government Community Cloud (GCC) ajánlatokat értékesítő partnerek a Felhőszolgáltató programon keresztül az Partnerközpont API-val</span><span class="sxs-lookup"><span data-stu-id="f2b2c-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="f2b2c-299">Részletek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-299">Details</span></span>

<span data-ttu-id="f2b2c-300">Ez a közlemény a decemberben megjelent Partnerközpont [követő fejlesztéseket követi.](./2020-december.md#1)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-300">This announcement is a follow-up to the Partner Center [enhancements released in December](./2020-december.md#1).</span></span> <span data-ttu-id="f2b2c-301">Ennek a kiadásnak a részeként új GET és POST Qualifications API-kat helyezett üzembe, ezért a meglévő GET-minősítést **2021. május 6-án kivezetjük.**</span><span class="sxs-lookup"><span data-stu-id="f2b2c-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, **the existing GET qualification will be retired on May 6, 2021**.</span></span> <span data-ttu-id="f2b2c-302">Erre az időszakra át kell tért az új POST Partnerközpont API-kra.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-302">By that time, you will need to have transitioned to using the new POST Partner Center APIs.</span></span> <span data-ttu-id="f2b2c-303">Az új POST API-k lehetővé teszik az Oktatási ajánlatok megvásárlását, az új GET API-k pedig lehetővé teszik, hogy előre minősített nonprofit és GCC-ajánlatokat vásároljon.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-303">The new POST APIs will enable you to purchase Education offers, while the new GET APIs will enable you to purchase pre-qualified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="f2b2c-304">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="f2b2c-304">Next steps</span></span>

- <span data-ttu-id="f2b2c-305">**A sikeres és** időbeni átállás érdekében frissítsen az új API-kra.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-305">**Update to the new APIs** for a successful and timely transition.</span></span>

- <span data-ttu-id="f2b2c-306">**Tekintse át az Partnerközpont API új** módosításait és útmutatóját az Operations Readiness resources: Partnerközpont Education ügyfél-ellenőrzési folyamat [fejlesztései között.](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-306">**Review the new Partner Center API changes and Guide** in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="f2b2c-307">Ossza meg ezeket az információkat a szervezeten belüli megfelelő csapatokkal és a viszonteladóival, hogy felkészüljenek ezekre a változásokra.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-307">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="f2b2c-308">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="f2b2c-308">Questions?</span></span>

<span data-ttu-id="f2b2c-309">Az értesítéssel kapcsolatos kérdésekért lépjen kapcsolatba a [Partnerközpont ügyfélszolgálatával.](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-309">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="f2b2c-310">Változási napló</span><span class="sxs-lookup"><span data-stu-id="f2b2c-310">Change log</span></span>

- <span data-ttu-id="f2b2c-311">2021. május 4.: Utolsó emlékeztető a GET-minősítés hamarosan elalasztásról</span><span class="sxs-lookup"><span data-stu-id="f2b2c-311">May 4, 2021: Final reminder of upcoming deprecation of GET qualification</span></span>

- <span data-ttu-id="f2b2c-312">2021. április 9.: Emlékeztető a GET-minősítés hamarosan elalasztásról</span><span class="sxs-lookup"><span data-stu-id="f2b2c-312">April 9, 2021: Reminder of upcoming deprecation of GET qualification</span></span> 

- <span data-ttu-id="f2b2c-313">Február: Frissültek a GET és PUT minősítések & idővonalai</span><span class="sxs-lookup"><span data-stu-id="f2b2c-313">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>

- <span data-ttu-id="f2b2c-314">Január: Emlékeztető a GET és PUT minősítések & elalasztásról</span><span class="sxs-lookup"><span data-stu-id="f2b2c-314">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="f2b2c-315">Az új kereskedelmi PDF-számla formátuma a CSP-ben</span><span class="sxs-lookup"><span data-stu-id="f2b2c-315">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="f2b2c-316">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="f2b2c-316">Categories</span></span>

- <span data-ttu-id="f2b2c-317">Dátum: 2021-04-05</span><span class="sxs-lookup"><span data-stu-id="f2b2c-317">Date: 2021-04-05</span></span>
- <span data-ttu-id="f2b2c-318">Képességek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-318">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="f2b2c-319">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="f2b2c-319">Summary</span></span>

<span data-ttu-id="f2b2c-320">A Microsoft új formátumot vezet be az új kereskedelmi PDF-számlához a Felhőszolgáltató (CSP) programban, hogy a termékleírás helyett termékadatok szerint jelenítse meg a számlázási adatokat.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-320">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="f2b2c-321">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="f2b2c-321">Impacted audience</span></span>

<span data-ttu-id="f2b2c-322">CSP-programon keresztül tranzakciós partnerek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-322">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="f2b2c-323">Részletek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-323">Details</span></span>

<span data-ttu-id="f2b2c-324">2021 májusával kezdődően a Microsoft új formátumot vezet be az új kereskedelmi PDF-számlához a CSP-programban, hogy a termékleírás helyett termékadatok szerint jelenítse meg a számlázási adatokat.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-324">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="f2b2c-325">Ezzel az új frissítéssel a sorelemeket terméktípus szerint összesítődve jelenítjük meg az összes terméket egy külön sorban.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-325">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="f2b2c-326">A partnerek észrevehetnek egy ilyen változást a 2021. április 1. és 2021. április 30. közötti számlázási időszakra vonatkozó májusi számlán.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-326">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="f2b2c-327">Az érintett ajánlatok a Microsoft Azure, az Azure-előfizetések (Azure-csomag) és a Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-327">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="f2b2c-328">A számlaformátum frissítése után lekért jóváírási kérelmek az új formátumban jönnek létre.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-328">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="f2b2c-329">Partneri előnyök</span><span class="sxs-lookup"><span data-stu-id="f2b2c-329">Partner benefits</span></span>

<span data-ttu-id="f2b2c-330">Ez a frissítés a következő fejlesztéseket tartalmazza a partnerek számlázási élményében:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-330">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="f2b2c-331">Csökkentett számlaméret a kritikus adatok megőrzése közben</span><span class="sxs-lookup"><span data-stu-id="f2b2c-331">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="f2b2c-332">A formátum igazítása az iparági szabványokhoz a kompakt és felhasználóbarát számlákhoz</span><span class="sxs-lookup"><span data-stu-id="f2b2c-332">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="f2b2c-333">A következő elemekre ez nem lesz hatással:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-333">The following elements will not be affected:</span></span>

- <span data-ttu-id="f2b2c-334">Számlázási összefoglaló oldal a számla PDF-fájlján</span><span class="sxs-lookup"><span data-stu-id="f2b2c-334">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="f2b2c-335">Meglévő számlázási API-k</span><span class="sxs-lookup"><span data-stu-id="f2b2c-335">Existing invoicing APIs</span></span>

- <span data-ttu-id="f2b2c-336">Egyeztetési fájlok (a részletes adatok lekért Recon-fájlokkal is lekért fájlok.)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-336">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="f2b2c-337">Használati és licencalapú díjak számlái</span><span class="sxs-lookup"><span data-stu-id="f2b2c-337">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="f2b2c-338">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="f2b2c-338">Next steps</span></span>

<span data-ttu-id="f2b2c-339">Tekintse át a témakörrel kapcsolatos információkat a Microsoft partner [webhelyének Operations Readiness](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) erőforrás-katalógusában.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-339">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="f2b2c-340">A számlázási és adózási témakörökről , például a számlázási erőforrásokról, a [](../billing.md) számlákról, a CSP-számlázásról és az adókkal kapcsolatos további információkért látogasson el a Számlázás szakaszra a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-340">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](../billing.md) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="f2b2c-341">A Felhőszolgáltató (CSP) ügyfélbe való beiratalozási követelményeinek változásai</span><span class="sxs-lookup"><span data-stu-id="f2b2c-341">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="f2b2c-342">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="f2b2c-342">Categories</span></span>

- <span data-ttu-id="f2b2c-343">Dátum: 2021-04-02</span><span class="sxs-lookup"><span data-stu-id="f2b2c-343">Date: 2021-04-02</span></span>
- <span data-ttu-id="f2b2c-344">Ajánlatok/piacok</span><span class="sxs-lookup"><span data-stu-id="f2b2c-344">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="f2b2c-345">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="f2b2c-345">Summary</span></span>

<span data-ttu-id="f2b2c-346">Elkötelezettségünk részeként, hogy segítsünk a partnereknek és az ügyfeleknek a bizalmi kapcsolaton alapuló üzleti tevékenységben, további ügyféladatokat kérünk 2021. március 25-ig.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-346">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="f2b2c-347">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="f2b2c-347">Impacted audience</span></span>

<span data-ttu-id="f2b2c-348">CsP közvetlen számlázási partnerek és közvetett szolgáltatók, akik új vagy meglévő ügyfelekkel vannak a következő szakaszban felsorolt országokban</span><span class="sxs-lookup"><span data-stu-id="f2b2c-348">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="f2b2c-349">Részletek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-349">Details</span></span>

<span data-ttu-id="f2b2c-350">A Microsoft megbízhatósági kapcsolaton fut.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-350">Microsoft runs on trust.</span></span> <span data-ttu-id="f2b2c-351">Elkötelezettek vagyunk amellett, hogy megfelelő, biztonságos és biztonságos ügyfél-ellenőrzési módszert biztosítsunk az ügyfél-előfizetések tranzakciós folyamatához a CSP-programban.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-351">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="f2b2c-352">2021. március 25-én bevezetünk egy API- és felhasználói felületi (UI) fejlesztéseket Partnerközpont, amelyek hatással lesznek az alábbi két feltételnek megfelelő partnerekre:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-352">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="f2b2c-353">A partner közvetlen számlázási kapcsolattal rendelkezik a Microsofttal (ami azt jelenti, hogy a partner közvetlen számlázási partner vagy közvetett szolgáltató).</span><span class="sxs-lookup"><span data-stu-id="f2b2c-353">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="f2b2c-354">A partner az alábbi országokban lévő új vagy meglévő ügyfelekkel működik együtt:</span><span class="sxs-lookup"><span data-stu-id="f2b2c-354">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="f2b2c-355">Thaiföld</span><span class="sxs-lookup"><span data-stu-id="f2b2c-355">Thailand</span></span>
    - <span data-ttu-id="f2b2c-356">Vietnam</span><span class="sxs-lookup"><span data-stu-id="f2b2c-356">Vietnam</span></span>
    - <span data-ttu-id="f2b2c-357">Törökország</span><span class="sxs-lookup"><span data-stu-id="f2b2c-357">Turkey</span></span>
    - <span data-ttu-id="f2b2c-358">Lengyelország</span><span class="sxs-lookup"><span data-stu-id="f2b2c-358">Poland</span></span>
    - <span data-ttu-id="f2b2c-359">Dél-afrikai Köztársaság</span><span class="sxs-lookup"><span data-stu-id="f2b2c-359">South Africa</span></span>
    - <span data-ttu-id="f2b2c-360">India</span><span class="sxs-lookup"><span data-stu-id="f2b2c-360">India</span></span>
    - <span data-ttu-id="f2b2c-361">Brazília</span><span class="sxs-lookup"><span data-stu-id="f2b2c-361">Brazil</span></span>
    - <span data-ttu-id="f2b2c-362">Irak</span><span class="sxs-lookup"><span data-stu-id="f2b2c-362">Iraq</span></span>
    - <span data-ttu-id="f2b2c-363">Mianmar</span><span class="sxs-lookup"><span data-stu-id="f2b2c-363">Myanmar</span></span>
    - <span data-ttu-id="f2b2c-364">Dél-Szudán</span><span class="sxs-lookup"><span data-stu-id="f2b2c-364">South Sudan</span></span>
    - <span data-ttu-id="f2b2c-365">Szaúd-Arábia</span><span class="sxs-lookup"><span data-stu-id="f2b2c-365">Saudi Arabia</span></span>
    - <span data-ttu-id="f2b2c-366">Egyesült Arab Emírségek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-366">United Arab Emirates</span></span>
    - <span data-ttu-id="f2b2c-367">Venezuela</span><span class="sxs-lookup"><span data-stu-id="f2b2c-367">Venezuela</span></span>

<span data-ttu-id="f2b2c-368">A feltételeknek megfelelő partnereknek be kell majd nyújtaniuk az ügyfél céges regisztrációs azonosítóját (más néven az ügyfél szervezeti INN-ét) és telefonszámát, amikor legközelebb frissítik vagy létrehoznak egy előfizetést az adott ügyfél számára.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-368">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="f2b2c-369">Ezek a partnerek középső nevet is megadhatnak az ügyfél számára.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-369">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="f2b2c-370">Vegye figyelembe, hogy a céges regisztrációs azonosító hozzáadásakor az üzleti adóazonosítót kell használnia, nem az ügyfél személyes azonosítóját.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-370">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="f2b2c-371">Azok a partnerek, akik az alábbi országokban lévő új vagy meglévő ügyfelekkel üzleti partnereket hoznak létre, már elő vannak hozva egy korábbi kiadással 2020 novemberében.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-371">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="f2b2c-372">Örményország</span><span class="sxs-lookup"><span data-stu-id="f2b2c-372">Armenia</span></span>
- <span data-ttu-id="f2b2c-373">Azerbajdzsán</span><span class="sxs-lookup"><span data-stu-id="f2b2c-373">Azerbaijan</span></span>
- <span data-ttu-id="f2b2c-374">Belarusz</span><span class="sxs-lookup"><span data-stu-id="f2b2c-374">Belarus</span></span>
- <span data-ttu-id="f2b2c-375">Magyarország</span><span class="sxs-lookup"><span data-stu-id="f2b2c-375">Hungary</span></span>
- <span data-ttu-id="f2b2c-376">Kazahsztán</span><span class="sxs-lookup"><span data-stu-id="f2b2c-376">Kazakhstan</span></span>
- <span data-ttu-id="f2b2c-377">Kirgizisztán</span><span class="sxs-lookup"><span data-stu-id="f2b2c-377">Kyrgyzstan</span></span>
- <span data-ttu-id="f2b2c-378">Moldova</span><span class="sxs-lookup"><span data-stu-id="f2b2c-378">Moldova</span></span>
- <span data-ttu-id="f2b2c-379">Oroszország</span><span class="sxs-lookup"><span data-stu-id="f2b2c-379">Russia</span></span>
- <span data-ttu-id="f2b2c-380">Tádzsikisztán</span><span class="sxs-lookup"><span data-stu-id="f2b2c-380">Tajikistan</span></span>
- <span data-ttu-id="f2b2c-381">Ukrajna</span><span class="sxs-lookup"><span data-stu-id="f2b2c-381">Ukraine</span></span>
- <span data-ttu-id="f2b2c-382">Üzbegisztán</span><span class="sxs-lookup"><span data-stu-id="f2b2c-382">Uzbekistan</span></span>

<span data-ttu-id="f2b2c-383">A 2021. március végén az ügyfelekkel a világ többi részén partnerekkel is lehetősége lesz megadni a céges regisztrációs azonosítót, a telefonszámot és a középső nevet igény szerint.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-383">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="f2b2c-384">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="f2b2c-384">Next steps</span></span>

- <span data-ttu-id="f2b2c-385">Részletesebb útmutatásért tekintse át a műszaki dokumentációt és a dedikált [partnergyűjteményben](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) található gyakori kérdéseket.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-385">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="f2b2c-386">Készüljön fel arra, hogy a módosításokat az API Partnerközpont webes felhasználói felület használatával építse be.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-386">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="f2b2c-387">Az API/SDK-k elérhetők lesznek a teszteléshez.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-387">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="f2b2c-388">Az új ügyfelek be- vagy módosításakor küldje el a további adatokat.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-388">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="f2b2c-389">Ha vezérlőpult-szállítói (CPV) megoldást használ, tekintse meg a CPV-t.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-389">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="f2b2c-390">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="f2b2c-390">Questions?</span></span>

<span data-ttu-id="f2b2c-391">Ha bármilyen kérdése van a vállalat regisztrációs azonosítójával (más néven INN-rel vagy TIN-rel) kapcsolatban, lépjen kapcsolatba az adótanácsadójával vagy a helyi adóiroda segítségével.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-391">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="f2b2c-392">A Microsoft nem tud útmutatást nyújtani az adózási kérdésekkel kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-392">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="f2b2c-393">Ha támogatásra van szüksége a Microsofttal kapcsolatos műveleteihez, nyisson meg egy [szolgáltatáskérést.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="f2b2c-393">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="f2b2c-394">Az e havi termékbelövések és -ajánlatok megtekintése</span><span class="sxs-lookup"><span data-stu-id="f2b2c-394">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="f2b2c-395">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="f2b2c-395">Categories</span></span>

- <span data-ttu-id="f2b2c-396">Dátum: 2021.04. 01.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-396">Date: 2021-04-01</span></span>
- <span data-ttu-id="f2b2c-397">Képességek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-397">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="f2b2c-398">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="f2b2c-398">Summary</span></span>

<span data-ttu-id="f2b2c-399">Megjelent a 2021. áprilisi termékindítási naptár.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-399">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="f2b2c-400">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="f2b2c-400">Impacted audience</span></span>

<span data-ttu-id="f2b2c-401">Az összes partner, aki a Felhőszolgáltató (CSP) programon keresztül megy keresztül</span><span class="sxs-lookup"><span data-stu-id="f2b2c-401">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="f2b2c-402">Részletek</span><span class="sxs-lookup"><span data-stu-id="f2b2c-402">Details</span></span>

<span data-ttu-id="f2b2c-403">A 2021. áprilisi termékindítási [naptár](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) már elérhető az Operations Readiness erőforrás-katalógusban.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-403">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="f2b2c-404">A következő termékbelövéseket és -ajánlatokat itt megtekintheti.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-404">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="f2b2c-405">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="f2b2c-405">Next steps</span></span>

<span data-ttu-id="f2b2c-406">Tekintse át [a termékindítási naptárt,](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)és ossza meg az információkat a szervezet megfelelő érdekelt felével.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-406">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="f2b2c-407">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="f2b2c-407">Questions?</span></span>

<span data-ttu-id="f2b2c-408">Az ajánlatokkal kapcsolatos további kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="f2b2c-408">For any further questions about these offers, check your relevant Yammer communities.</span></span>