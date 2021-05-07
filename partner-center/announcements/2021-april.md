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
ms.openlocfilehash: 798dcb1570a0f6dfc94c7b45fc3c2e152f55cbe5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702824"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="32aec-103">2021. áprilisi közlemények</span><span class="sxs-lookup"><span data-stu-id="32aec-103">April 2021 announcements</span></span>

<span data-ttu-id="32aec-104">Ez az oldal a Microsoft 2021. áprilisi Partnerközpont bejelentését mutatja be.</span><span class="sxs-lookup"><span data-stu-id="32aec-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="32aec-105">Készenlét: A CSP frissített ügyfélcím-ellenőrzési API-ja júniusban lesz elérhető; tesztelési képesség már elérhető</span><span class="sxs-lookup"><span data-stu-id="32aec-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="32aec-106">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="32aec-106">Categories</span></span>

- <span data-ttu-id="32aec-107">Dátum: 2021-04-30</span><span class="sxs-lookup"><span data-stu-id="32aec-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="32aec-108">Készenlét</span><span class="sxs-lookup"><span data-stu-id="32aec-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="32aec-109">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="32aec-109">Summary</span></span>

<span data-ttu-id="32aec-110">Annak érdekében, hogy a partnerek és az ügyfelek bizalom alapján futtassanak üzletüket, meghívjuk a partnereket, hogy teszteljék a Validate Address API módosításait az összes országban világszerte.</span><span class="sxs-lookup"><span data-stu-id="32aec-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="32aec-111">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="32aec-111">Impacted audience</span></span>

<span data-ttu-id="32aec-112">CsP – közvetlen számlázási partnerek és közvetett szolgáltatók, akik új ügyfelek címének adatait hozják létre vagy frissítik</span><span class="sxs-lookup"><span data-stu-id="32aec-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="32aec-113">Részletek</span><span class="sxs-lookup"><span data-stu-id="32aec-113">Details</span></span>

<span data-ttu-id="32aec-114">A Microsoft megbízhatósági kapcsolaton fut.</span><span class="sxs-lookup"><span data-stu-id="32aec-114">Microsoft runs on trust.</span></span> <span data-ttu-id="32aec-115">Elkötelezettek vagyunk amellett, hogy megfelelő, biztonságos és biztonságos módszert biztosítsunk az ügyfélcímek érvényesítéséhez az ügyfél-előfizetések tranzakciója során a CSP-programban.</span><span class="sxs-lookup"><span data-stu-id="32aec-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="32aec-116">2021. március 31-től bevezettük a Validate Address API módosításait.</span><span class="sxs-lookup"><span data-stu-id="32aec-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="32aec-117">Meghívjuk a partnereket, hogy teszteljék az API-t a 2021. június végi élő adás előtt.</span><span class="sxs-lookup"><span data-stu-id="32aec-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="32aec-118">Vegye figyelembe, hogy ezek a módosítások csak a Validate Address API-t érintik.</span><span class="sxs-lookup"><span data-stu-id="32aec-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="32aec-119">A Create Customer and Update Billing Profile API-kat ez nem érinti.</span><span class="sxs-lookup"><span data-stu-id="32aec-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="32aec-120">Bár a javasolt címet jelenleg nem kell használni az Ügyfél létrehozása API-val, erősen ajánlott.</span><span class="sxs-lookup"><span data-stu-id="32aec-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="32aec-121">A válasz a következő állapotüzenetek egyikét adja vissza:</span><span class="sxs-lookup"><span data-stu-id="32aec-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="32aec-122">Állapot</span><span class="sxs-lookup"><span data-stu-id="32aec-122">Status</span></span>     | <span data-ttu-id="32aec-123">Leírás</span><span class="sxs-lookup"><span data-stu-id="32aec-123">Description</span></span> |    <span data-ttu-id="32aec-124">A visszaadott javasolt címek száma</span><span class="sxs-lookup"><span data-stu-id="32aec-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="32aec-125">Ellenőrzött szállításra használható</span><span class="sxs-lookup"><span data-stu-id="32aec-125">Verified shippable</span></span> | <span data-ttu-id="32aec-126">A cím ellenőrizve van, és szállítható a címre.</span><span class="sxs-lookup"><span data-stu-id="32aec-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="32aec-127">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="32aec-127">Single</span></span> |
|<span data-ttu-id="32aec-128">Ellenőrzött</span><span class="sxs-lookup"><span data-stu-id="32aec-128">Verified</span></span> | <span data-ttu-id="32aec-129">A cím ellenőrizve van.</span><span class="sxs-lookup"><span data-stu-id="32aec-129">Address is verified.</span></span> | <span data-ttu-id="32aec-130">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="32aec-130">Single</span></span> |
|<span data-ttu-id="32aec-131">Beavatkozás szükséges</span><span class="sxs-lookup"><span data-stu-id="32aec-131">Interaction required</span></span> | <span data-ttu-id="32aec-132">A javasolt cím jelentős mértékben módosult, és felhasználói megerősítést kér.</span><span class="sxs-lookup"><span data-stu-id="32aec-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="32aec-133">Egyirányú</span><span class="sxs-lookup"><span data-stu-id="32aec-133">Single</span></span> |
|<span data-ttu-id="32aec-134">Utca részleges</span><span class="sxs-lookup"><span data-stu-id="32aec-134">Street partial</span></span> | <span data-ttu-id="32aec-135">A címben megadott utca részleges, és további információra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="32aec-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="32aec-136">Többszörös – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="32aec-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="32aec-137">Részleges helyszín</span><span class="sxs-lookup"><span data-stu-id="32aec-137">Premises partial</span></span> | <span data-ttu-id="32aec-138">Az adott helyszín (épületszám, csomagszám stb.) részleges, és további információra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="32aec-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="32aec-139">Többszörös – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="32aec-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="32aec-140">Többszörös</span><span class="sxs-lookup"><span data-stu-id="32aec-140">Multiple</span></span> | <span data-ttu-id="32aec-141">Több mező is részleges a címben (beleértve az utca részleges és a helyszíni részleges mezőket is).</span><span class="sxs-lookup"><span data-stu-id="32aec-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="32aec-142">Többszörös – legfeljebb három</span><span class="sxs-lookup"><span data-stu-id="32aec-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="32aec-143">Nincsenek</span><span class="sxs-lookup"><span data-stu-id="32aec-143">None</span></span> | <span data-ttu-id="32aec-144">A cím helytelen.</span><span class="sxs-lookup"><span data-stu-id="32aec-144">Address is incorrect.</span></span> | <span data-ttu-id="32aec-145">Nincsenek</span><span class="sxs-lookup"><span data-stu-id="32aec-145">None</span></span> |
|<span data-ttu-id="32aec-146">Nincs ellenőrizve.</span><span class="sxs-lookup"><span data-stu-id="32aec-146">Not validated</span></span> | <span data-ttu-id="32aec-147">A cím nem lett elküldve az érvényesítési folyamaton keresztül.</span><span class="sxs-lookup"><span data-stu-id="32aec-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="32aec-148">Nincsenek</span><span class="sxs-lookup"><span data-stu-id="32aec-148">None</span></span> |

<span data-ttu-id="32aec-149">Az USA-nak az irányítószámai további négy számjegyet és kötőjelet fognak visszaadni, például: 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="32aec-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="32aec-150">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="32aec-150">Next steps</span></span>

- <span data-ttu-id="32aec-151">Részletesebb útmutatásért tekintse át a műszaki dokumentációt és a dedikált [partnergyűjtemény](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) gyakori kérdéseit.</span><span class="sxs-lookup"><span data-stu-id="32aec-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="32aec-152">Készüljön fel arra, hogy a módosításokat a Partnerközpont API és a webes felhasználói felület használatával építse be.</span><span class="sxs-lookup"><span data-stu-id="32aec-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="32aec-153">Ossza meg a tesztgép bérlőazonosítóját a témaszakértővel (Ali Sandki), aki szerepelni fog a tesztúton, hogy megkezdje a frissítés előkészítését.</span><span class="sxs-lookup"><span data-stu-id="32aec-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="32aec-154">Ha vezérlőpult-szállító (CPV) megoldást használ, tekintse meg a CPV-t.</span><span class="sxs-lookup"><span data-stu-id="32aec-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="32aec-155">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="32aec-155">Questions?</span></span>

<span data-ttu-id="32aec-156">Ha támogatásra van szüksége a Microsofttal kapcsolatos műveleteihez, kérje a partnertámogatási Yammer-csoportját, vagy nyisson meg egy [szolgáltatáskérést.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="32aec-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="32aec-157">Az API Swagger Partnerközpont dokumentációjának új helye</span><span class="sxs-lookup"><span data-stu-id="32aec-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="32aec-158">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="32aec-158">Categories</span></span>

- <span data-ttu-id="32aec-159">Dátum: 2021. 04. 26.</span><span class="sxs-lookup"><span data-stu-id="32aec-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="32aec-160">Képességek</span><span class="sxs-lookup"><span data-stu-id="32aec-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="32aec-161">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="32aec-161">Summary</span></span>

<span data-ttu-id="32aec-162">Partnerközpont API Swagger-dokumentumok migrálva vannak az előző [Swagger-dokumentációs webhelyről](https://apidocs.microsoft.com/services/partnercenter) egy új [Swagger-dokumentációs webhelyre.](https://docs.microsoft.com/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="32aec-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="32aec-163">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="32aec-163">Impacted audience</span></span>

<span data-ttu-id="32aec-164">Az Felhőszolgáltató (CSP) programban részt vevő közvetlen számlázási partnerek és közvetett szolgáltatók, akik az Partnerközpont API-kat</span><span class="sxs-lookup"><span data-stu-id="32aec-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="32aec-165">Részletek</span><span class="sxs-lookup"><span data-stu-id="32aec-165">Details</span></span>

<span data-ttu-id="32aec-166">2021. április 26-tól az Partnerközpont API Swagger dokumentációja, beleértve a REST API-tartalmakat, egy új [webhelyen található.](https://docs.microsoft.com/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="32aec-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="32aec-167">A régi hely néhány hét után elérhetetlen lesz.</span><span class="sxs-lookup"><span data-stu-id="32aec-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="32aec-168">Előnyök</span><span class="sxs-lookup"><span data-stu-id="32aec-168">Benefits</span></span>

<span data-ttu-id="32aec-169">A Partnerközpont API Swagger dokumentációja egy **Try It függvényt biztosít.**</span><span class="sxs-lookup"><span data-stu-id="32aec-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="32aec-170">A függvény csak akkor használható, ha rendelkezik egy Bearer Token jogkivonattal, amelyet a hitelesítést Partnerközpont követve hozhat [létre.](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication)</span><span class="sxs-lookup"><span data-stu-id="32aec-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="32aec-171">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="32aec-171">Next steps</span></span>

<span data-ttu-id="32aec-172">Ossza meg ezt az információt a szervezeten belül, hogy a megfelelő csapat áttekintheti és frissítheti a folyamatait.</span><span class="sxs-lookup"><span data-stu-id="32aec-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="32aec-173">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="32aec-173">Questions?</span></span>

<span data-ttu-id="32aec-174">Az ajánlatokkal kapcsolatos kérdésekért tekintse meg a kapcsolódó Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="32aec-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="32aec-175">Felhőszolgáltató (CSP) szoftver visszaküldési időszakának szabályzata és letöltési hivatkozás lejárati értesítése</span><span class="sxs-lookup"><span data-stu-id="32aec-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="32aec-176">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="32aec-176">Categories</span></span>

- <span data-ttu-id="32aec-177">Dátum: 2021. 04. 21.</span><span class="sxs-lookup"><span data-stu-id="32aec-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="32aec-178">Képességek</span><span class="sxs-lookup"><span data-stu-id="32aec-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="32aec-179">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="32aec-179">Summary</span></span>

<span data-ttu-id="32aec-180">A CSP szoftver visszaküldési időszakra vonatkozó szabályzata és a letöltési hivatkozás lejárata módosult.</span><span class="sxs-lookup"><span data-stu-id="32aec-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="32aec-181">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="32aec-181">Impacted audience</span></span>

<span data-ttu-id="32aec-182">Folyamatos szoftver- vagy szoftver-előfizetési ajánlatokat a CSP-ban tranzakciós partnerek</span><span class="sxs-lookup"><span data-stu-id="32aec-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="32aec-183">Részletek</span><span class="sxs-lookup"><span data-stu-id="32aec-183">Details</span></span>

<span data-ttu-id="32aec-184">Vegye figyelembe a következő fontos értesítéseket a szoftver- és szoftver-előfizetések folyamatos vásárlásával kapcsolatban a Partnerközpont:</span><span class="sxs-lookup"><span data-stu-id="32aec-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="32aec-185">Szoftver visszaküldési időszakának szabályzata</span><span class="sxs-lookup"><span data-stu-id="32aec-185">Software return period policy</span></span>

<span data-ttu-id="32aec-186">2021. június 1-től a CSP-ben az Microsoft Partnerszerződés (MPA) által meghatározott szoftver ajánlatok visszatérési időtartama a megrendelés dátuma és 30 napja között 60 napra változik.</span><span class="sxs-lookup"><span data-stu-id="32aec-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="32aec-187">A szoftverajánlatra vonatkozó megrendelés elküldése után a partnereknek a megrendelés dátumát követően 30 nap áll a 30 napra, hogy bármely változatot elküldje az adott rendelésre:</span><span class="sxs-lookup"><span data-stu-id="32aec-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="32aec-188">A 30 napos visszatérési időszakon belül visszaadott minden állandó szoftverlicenc a fizetős vásárlási ár teljes jóváírását kapja meg.</span><span class="sxs-lookup"><span data-stu-id="32aec-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="32aec-189">A 30 napos visszatérési időszakban visszaadott szoftver-előfizetési termékek a fizetős vásárlási ár időkorreklott jóváírását kapják meg.</span><span class="sxs-lookup"><span data-stu-id="32aec-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="32aec-190">Ez az üzenet a 2020. december és 2021. április között az összes CSP-partnernek küldött, az MPA visszaküldési időszakával és egyéb frissítéseivel kapcsolatos e-mail-üzenetek követő üzenete.</span><span class="sxs-lookup"><span data-stu-id="32aec-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="32aec-191">Az MPA-t érintő változásokkal kapcsolatos részletekért tekintse meg ezeket a közleményeket.</span><span class="sxs-lookup"><span data-stu-id="32aec-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="32aec-192">Szoftverletöltési hivatkozás lejárata</span><span class="sxs-lookup"><span data-stu-id="32aec-192">Software download link expiry</span></span>

<span data-ttu-id="32aec-193">2021. június 3-tól a szoftverletöltési hivatkozások folyamatos szoftver- és szoftver-előfizetési termékvásárláshoz Partnerközpont lejárati dátuma a kezdeti letöltéstől számított öt nap lesz.</span><span class="sxs-lookup"><span data-stu-id="32aec-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="32aec-194">A lejárati időszak 2021. június 3., illetve 2021. június 3. előtt és után minden vásárlásra érvényes lesz.</span><span class="sxs-lookup"><span data-stu-id="32aec-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="32aec-195">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="32aec-195">Next steps</span></span>

<span data-ttu-id="32aec-196">Tekintse át [a CSP visszaküldési időszakát,](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)és töltse le a hivatkozás lejáratával kapcsolatos gyakori kérdéseket, és tájékoztassa a szervezet összes megfelelő csapatát ezekről a változásokról:</span><span class="sxs-lookup"><span data-stu-id="32aec-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="32aec-197">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="32aec-197">Questions?</span></span>

<span data-ttu-id="32aec-198">Az ajánlatokkal kapcsolatos kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="32aec-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="32aec-199">Nyílt licencprogram: Viszonteladók váltása a Felhőszolgáltató (CSP) programra</span><span class="sxs-lookup"><span data-stu-id="32aec-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="32aec-200">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="32aec-200">Categories</span></span>

- <span data-ttu-id="32aec-201">Dátum: 2021-04-19</span><span class="sxs-lookup"><span data-stu-id="32aec-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="32aec-202">Üzleti növekedés</span><span class="sxs-lookup"><span data-stu-id="32aec-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="32aec-203">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="32aec-203">Summary</span></span>

<span data-ttu-id="32aec-204">Ez a kommunikáció részletesen bemutatja, hogyan készül fel a hamarosan a nyílt licencelési programba érkező változásokra.</span><span class="sxs-lookup"><span data-stu-id="32aec-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="32aec-205">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="32aec-205">Impacted audience</span></span>

<span data-ttu-id="32aec-206">CSP- és open-licencpartnerek</span><span class="sxs-lookup"><span data-stu-id="32aec-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="32aec-207">Részletek</span><span class="sxs-lookup"><span data-stu-id="32aec-207">Details</span></span>

<span data-ttu-id="32aec-208">2020-ban a [Microsoft](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) bejelentette, hogy a folyamatos szoftverlicencek széles körben elérhetők lesznek a partnerek és az ügyfelek számára a Felhőszolgáltató (CSP) programon keresztül.</span><span class="sxs-lookup"><span data-stu-id="32aec-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="32aec-209">Az első mérföldkövet 2021 januárban érte el, amikor a kereskedelmi célú folyamatos szoftveres ajánlatok elérhetővé váltak.</span><span class="sxs-lookup"><span data-stu-id="32aec-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="32aec-210">A következő fontos mérföldkő 2021 júliusában lesz, amikor elérhetővé válnak a [közszférában](https://aka.ms/openlicensepublicsector) elérhető ajánlatok.</span><span class="sxs-lookup"><span data-stu-id="32aec-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="32aec-211">Arról [is](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) tájékoztattunk, hogy 2022. január 1-től az Open License programon keresztül nem lehet új szoftverlicenc-vásárlásokat vagy Frissítési Garancia online szolgáltatások licenceket vásárolni vagy megújítni.</span><span class="sxs-lookup"><span data-stu-id="32aec-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="32aec-212">Az új kereskedelmi élményben a folyamatos szoftver a CSP-programra való áttérése segít a partnereknek abban, hogy bővítsék a különböző megoldások és felügyelt szolgáltatások kínálta lehetőségeket.</span><span class="sxs-lookup"><span data-stu-id="32aec-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="32aec-213">Ez felgyorsítja az ügyfelek felhőre való áttérését is.</span><span class="sxs-lookup"><span data-stu-id="32aec-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="32aec-214">A partnerek és az ügyfelek zökkenőmentes átállásának biztosítása érdekében ezeket a módosításokat és anyagokat azért végeztünk, hogy felgyorsítsuk a digitális átalakítást:</span><span class="sxs-lookup"><span data-stu-id="32aec-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="32aec-215">2021. április</span><span class="sxs-lookup"><span data-stu-id="32aec-215">April 2021</span></span>

<span data-ttu-id="32aec-216">[Mostantól elérhető:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Licencről CSP-re váltásra használható anyagok viszonteladók számára</span><span class="sxs-lookup"><span data-stu-id="32aec-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="32aec-217">2021. július</span><span class="sxs-lookup"><span data-stu-id="32aec-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="32aec-218">CSP</span><span class="sxs-lookup"><span data-stu-id="32aec-218">CSP</span></span>

- <span data-ttu-id="32aec-219">Július 1. : A közszférában dolgozó ügyfelek számára elérhető folyamatos szoftverlicencek</span><span class="sxs-lookup"><span data-stu-id="32aec-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="32aec-220">Július 7. Visual Studio: a Pro és a Get Genuine Windows Agreement folyamatos szoftverlicencek, amelyek minden szegmensben elérhetők</span><span class="sxs-lookup"><span data-stu-id="32aec-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="32aec-221">Nyitott érték</span><span class="sxs-lookup"><span data-stu-id="32aec-221">Open Value</span></span>

- <span data-ttu-id="32aec-222">Július 1. : Az Open Value program oktatási és nonprofit programjában elérhető további termékkódok, amelyek az Open License programhoz hasonló ajánlatokat érhetők el</span><span class="sxs-lookup"><span data-stu-id="32aec-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="32aec-223">Open License</span><span class="sxs-lookup"><span data-stu-id="32aec-223">Open License</span></span>

- <span data-ttu-id="32aec-224">Július 1. : A Microsoft már nem indít új ajánlatokat az Open License programban.</span><span class="sxs-lookup"><span data-stu-id="32aec-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="32aec-225">2022. január</span><span class="sxs-lookup"><span data-stu-id="32aec-225">January 2022</span></span>

- <span data-ttu-id="32aec-226">Január 1. : Az Open License programon keresztül nem lehet új vásárlásokat vagy megújításokat vásárolni</span><span class="sxs-lookup"><span data-stu-id="32aec-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="32aec-227">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="32aec-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="32aec-228">Közvetett CSP-szolgáltatók</span><span class="sxs-lookup"><span data-stu-id="32aec-228">CSP indirect providers</span></span>

<span data-ttu-id="32aec-229">Az elkövetkező hónapokban segítheti az Open License-viszonteladókat a CSP-programba való beteknésekben azáltal, hogy részt vesz a partnerközösségi eseményekben, és a viszonteladóknak készült Open License-to-CSP áttűnésanyagokat használja:</span><span class="sxs-lookup"><span data-stu-id="32aec-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="32aec-230">Nyissa meg a viszonteladók számára készült [licenc–CSP](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)áttérési anyagokat – Testre szabható áttekintő bemutató, e-mail-sablon, közvetett CSP-viszonteladói útmutató és egyéb anyagok, amelyek segítenek a viszonteladók nagy léptékű bevezetésében.</span><span class="sxs-lookup"><span data-stu-id="32aec-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="32aec-231">[A](https://globalpbocomm.eventbuilder.com/GlobalCSP) Microsoft Business Operations által üzemeltetett CSP-partnerközösségi események.</span><span class="sxs-lookup"><span data-stu-id="32aec-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="32aec-232">Csatlakozzon a különböző munkamenetekhez, és ismerje meg a CSP alapjait (a CSP alapjait), vagy maradjon naprakész, és kérdéseket te fel a CSP-szoftverekkel (Q&A munkamenetek).</span><span class="sxs-lookup"><span data-stu-id="32aec-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="32aec-233">(Hamarosan érkezik) A Microsoft Business Operations által üzemeltetett közvetett CSP-viszonteladói képzési munkamenet.</span><span class="sxs-lookup"><span data-stu-id="32aec-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="32aec-234">Open License resellers (Licenc-viszonteladók megnyitása)</span><span class="sxs-lookup"><span data-stu-id="32aec-234">Open License resellers</span></span>

- <span data-ttu-id="32aec-235">Ha a szervezet jelenleg nincs regisztrálva a CSP-programban, az első lépésekről a forgalmazótól érdeklődik.</span><span class="sxs-lookup"><span data-stu-id="32aec-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="32aec-236">Itt csatlakozhat egy közvetett [szolgáltatóhoz.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)</span><span class="sxs-lookup"><span data-stu-id="32aec-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="32aec-237">Ha a szervezete már regisztrálva van a CSP-programban, itt olvashat bővebben a folyamatos szoftverről a [CSP-ban.](https://partner.microsoft.com/resources/collection/software-in-csp)</span><span class="sxs-lookup"><span data-stu-id="32aec-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="32aec-238">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="32aec-238">Questions?</span></span>

<span data-ttu-id="32aec-239">Az ajánlatokkal kapcsolatos további kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="32aec-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="32aec-240">Most élő: Globális promóciós készenlét útmutató</span><span class="sxs-lookup"><span data-stu-id="32aec-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="32aec-241">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="32aec-241">Categories</span></span>

- <span data-ttu-id="32aec-242">Dátum: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="32aec-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="32aec-243">Képességek</span><span class="sxs-lookup"><span data-stu-id="32aec-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="32aec-244">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="32aec-244">Summary</span></span>

<span data-ttu-id="32aec-245">A Launch Readiness [](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) közzétett egy új globális promóciós készenlét-útmutatót az Operations Readiness erőforrás-katalógusban.</span><span class="sxs-lookup"><span data-stu-id="32aec-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="32aec-246">Ez az útmutató az összes aktív globális promóció összevont [nézetét biztosítja.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)</span><span class="sxs-lookup"><span data-stu-id="32aec-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="32aec-247">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="32aec-247">Impacted audience</span></span>

<span data-ttu-id="32aec-248">Minden mennyiségi licencelési (VL), Dynamics Price List- (DPL-) és Felhőszolgáltató (CSP-) partner</span><span class="sxs-lookup"><span data-stu-id="32aec-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="32aec-249">Részletek</span><span class="sxs-lookup"><span data-stu-id="32aec-249">Details</span></span>

<span data-ttu-id="32aec-250">A Microsoft partnerei megosztották velünk, hogy az összes globális promócióról összevont nézetet kell biztosítani támogató részletekkel.</span><span class="sxs-lookup"><span data-stu-id="32aec-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="32aec-251">Ezt az összevont útmutatót úgy szerette volna használni, hogy az előléptetések abban a biztos tudatában legyenek, hogy az összes elérhető információ könnyen elérhető lesz egy központi és kényelmes helyen.</span><span class="sxs-lookup"><span data-stu-id="32aec-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="32aec-252">2021 áprilisában a Microsoft havonta frissíti ezt az útmutatót, és elérhető lesz egy dedikált Global Promóciós készenlét útmutató gyűjteményben az Operations Readiness erőforrás-katalógusban.</span><span class="sxs-lookup"><span data-stu-id="32aec-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="32aec-253">Az útmutatóra mutató hivatkozásokat a következő gyűjtemények is tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="32aec-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="32aec-254">[Indítsa el a naptárgyűjteményt,](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)amely központosított áttekintést nyújt a közelgő változásokról és indításról.</span><span class="sxs-lookup"><span data-stu-id="32aec-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="32aec-255">[Közösségi gyűjtemények,](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)amelyek a havi partnerhívásainkhoz kapcsolódó anyagokat tartalmaznak, és kiemelik a közelgő változásokat és a fontos, időben esedékes témaköröket.</span><span class="sxs-lookup"><span data-stu-id="32aec-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="32aec-256">[Partneri hírlevelek,](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)például a CSP havi frissítése</span><span class="sxs-lookup"><span data-stu-id="32aec-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="32aec-257">Havi emlékeztetőként közzé is teszünk egy Partnerközpont a globális promóciós készenlétre vonatkozó útmutató minden új kiadásával.</span><span class="sxs-lookup"><span data-stu-id="32aec-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="32aec-258">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="32aec-258">Next steps</span></span>

<span data-ttu-id="32aec-259">Minden hónap elején megtalálja a legújabb [](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) globális promóciós készenléti útmutatót az [Operations Readiness erőforrás-katalógusban.](https://partner.microsoft.com/resources)</span><span class="sxs-lookup"><span data-stu-id="32aec-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="32aec-260">Ossza meg ezt az információt a szervezet megfelelő kapcsolattartóival, és ossza meg velünk, mennyire hasznos az útmutató a "Hasznos volt ez az oldal?" című szakaszban.</span><span class="sxs-lookup"><span data-stu-id="32aec-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="32aec-261">gombra az egyes oldalak végén.</span><span class="sxs-lookup"><span data-stu-id="32aec-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="32aec-262">Áprilisi Felhőszolgáltató (CSP) közösségi frissítés és emlékeztetők</span><span class="sxs-lookup"><span data-stu-id="32aec-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="32aec-263">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="32aec-263">Categories</span></span>

- <span data-ttu-id="32aec-264">Dátum: 2021. 04. 16.</span><span class="sxs-lookup"><span data-stu-id="32aec-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="32aec-265">Közösségi | Meghívók és emlékeztetők</span><span class="sxs-lookup"><span data-stu-id="32aec-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="32aec-266">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="32aec-266">Summary</span></span>

<span data-ttu-id="32aec-267">A CSP közösségi erőforrásai igény szerint és havonta frissítve érhetők el, hogy naprakész és felkészült legyen a CSP-programban való változásra.</span><span class="sxs-lookup"><span data-stu-id="32aec-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="32aec-268">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="32aec-268">Impacted audience</span></span>

<span data-ttu-id="32aec-269">CsP – közvetlen számlázási partnerek és közvetett szolgáltatók</span><span class="sxs-lookup"><span data-stu-id="32aec-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="32aec-270">Részletek</span><span class="sxs-lookup"><span data-stu-id="32aec-270">Details</span></span>

<span data-ttu-id="32aec-271">Ebben a hónapban az erőforrások a következő fő témaköröket tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="32aec-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="32aec-272">Frissítés a CSP-program fejlődésére és az Open License program változásaira</span><span class="sxs-lookup"><span data-stu-id="32aec-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="32aec-273">A CSP-ügyfelekre vonatkozó, bizonyos régiókban való ügyfél-behozatás követelményeinek változásai</span><span class="sxs-lookup"><span data-stu-id="32aec-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="32aec-274">Az új kereskedelmi PDF-számla formátuma a CSP-programban</span><span class="sxs-lookup"><span data-stu-id="32aec-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="32aec-275">A [CSP-közösséggyűjteményben](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)a következőt találja:</span><span class="sxs-lookup"><span data-stu-id="32aec-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="32aec-276">A letölthető [CSP Monthly Update hírlevele,](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)amely egy könnyen olvasható dokumentumban összesíti a legutóbbi CSP-közleményeket, frissítéseket, eseményeket és emlékeztetőket.</span><span class="sxs-lookup"><span data-stu-id="32aec-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="32aec-277">A [CSP bejelentési naptára,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)amely idővonal-nézetet biztosít a programot érintő közelgő változásokról.</span><span class="sxs-lookup"><span data-stu-id="32aec-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="32aec-278">Az új [termékindítási naptár,](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)amelyben megtekintheti a hamarosan megjelenő termékindításokat és -ajánlatokat.</span><span class="sxs-lookup"><span data-stu-id="32aec-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="32aec-279">[A CSP elindítja a](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) frissítési erőforrásokat a legfontosabb üzemeltetési változásokon könnyen használható tartalommal.</span><span class="sxs-lookup"><span data-stu-id="32aec-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="32aec-280">[Frissítők és emlékeztetők](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) az érdeklődést és lekérdezéseket fogadó főbb CSP-témakörökről.</span><span class="sxs-lookup"><span data-stu-id="32aec-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="32aec-281">CSP Community Call Q&As</span><span class="sxs-lookup"><span data-stu-id="32aec-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="32aec-282">Community Call Q&Mint elérhető, amely segít a közelgő változásokkal kapcsolatos kérdésekben.</span><span class="sxs-lookup"><span data-stu-id="32aec-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="32aec-283">Regisztráljon most a CSP Community Call Q&Az áprilisban, májusban és júniusban sorra kerül.</span><span class="sxs-lookup"><span data-stu-id="32aec-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="32aec-284">Ezek a legújabb indításokkal, fontos frissítésekkel és emlékeztetőkvel fognak összpontosítani.</span><span class="sxs-lookup"><span data-stu-id="32aec-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="32aec-285">[Regisztráljon itt.](https://globalpbocomm.eventbuilder.com/GlobalCSP)</span><span class="sxs-lookup"><span data-stu-id="32aec-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="32aec-286">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="32aec-286">Next steps</span></span>

<span data-ttu-id="32aec-287">Tekintse át a közösségi erőforrásokat, és regisztráljon a Community Call Q&A-re.</span><span class="sxs-lookup"><span data-stu-id="32aec-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="32aec-288">Annak érdekében, hogy a lehető legtöbbet hozhatja ki a Community Call Q&A-ból, tekintse át az igény szerinti közösségi tartalmat, és küldje el kérdéseit a hívás előtt legfeljebb 48 órával.</span><span class="sxs-lookup"><span data-stu-id="32aec-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="32aec-289">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="32aec-289">Questions?</span></span>

<span data-ttu-id="32aec-290">A CSP-közösség havi Call Q&A a legjobb hely a CSP-program változásaival kapcsolatos kérdésekhez.</span><span class="sxs-lookup"><span data-stu-id="32aec-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="32aec-291">Minden hónapban tekintse át az anyagokat, és küldje el kérdéseit előre, hogy a munkamenetet az Ön számára legfontosabb témakörökre töltjük.</span><span class="sxs-lookup"><span data-stu-id="32aec-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="32aec-292">További információért forduljon a támogatási [szolgálathoz.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)</span><span class="sxs-lookup"><span data-stu-id="32aec-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a><span data-ttu-id="32aec-293">Utolsó emlékeztető: A GET minősítés elalasztása 2021. május 6-án</span><span class="sxs-lookup"><span data-stu-id="32aec-293">Final reminder: Deprecation of GET qualification on May 6, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="32aec-294">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="32aec-294">Categories</span></span>

- <span data-ttu-id="32aec-295">Dátum: 2021-05-04</span><span class="sxs-lookup"><span data-stu-id="32aec-295">Date: 2021-05-04</span></span>

- <span data-ttu-id="32aec-296">Képességek</span><span class="sxs-lookup"><span data-stu-id="32aec-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="32aec-297">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="32aec-297">Impacted audience</span></span>

<span data-ttu-id="32aec-298">Academic, Nonprofit és Government Community Cloud (GCC) ajánlatokat értékesítő partnerek a Felhőszolgáltató programon keresztül az Partnerközpont API-val</span><span class="sxs-lookup"><span data-stu-id="32aec-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="32aec-299">Részletek</span><span class="sxs-lookup"><span data-stu-id="32aec-299">Details</span></span>

<span data-ttu-id="32aec-300">Ez a közlemény a decemberben megjelent Partnerközpont [követő fejlesztéseket követi.](https://docs.microsoft.com/partner-center/announcements/2020-december#1)</span><span class="sxs-lookup"><span data-stu-id="32aec-300">This announcement is a follow-up to the Partner Center [enhancements released in December](https://docs.microsoft.com/partner-center/announcements/2020-december#1).</span></span> <span data-ttu-id="32aec-301">Ennek a kiadásnak a részeként új GET és POST Minősítési API-kat helyezett üzembe, ezért a meglévő GET-minősítést **2021. május 6-án kivezetjük.**</span><span class="sxs-lookup"><span data-stu-id="32aec-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, **the existing GET qualification will be retired on May 6, 2021**.</span></span> <span data-ttu-id="32aec-302">Erre az időszakra át kell tért az új POST Partnerközpont API-kra.</span><span class="sxs-lookup"><span data-stu-id="32aec-302">By that time, you will need to have transitioned to using the new POST Partner Center APIs.</span></span> <span data-ttu-id="32aec-303">Az új POST API-k lehetővé teszik oktatási ajánlatok vásárlását, az új GET API-k pedig lehetővé teszik, hogy előre minősített Nonprofit és GCC-ajánlatokat vásároljon.</span><span class="sxs-lookup"><span data-stu-id="32aec-303">The new POST APIs will enable you to purchase Education offers, while the new GET APIs will enable you to purchase pre-qualified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="32aec-304">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="32aec-304">Next steps</span></span>

- <span data-ttu-id="32aec-305">**A sikeres és** időbeni átállás érdekében frissítsen az új API-kra.</span><span class="sxs-lookup"><span data-stu-id="32aec-305">**Update to the new APIs** for a successful and timely transition.</span></span>

- <span data-ttu-id="32aec-306">**Tekintse át az Partnerközpont API új** módosításait és útmutatóját az Operations Readiness resources: Partnerközpont Education ügyfél-ellenőrzési folyamat [fejlesztései között.](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)</span><span class="sxs-lookup"><span data-stu-id="32aec-306">**Review the new Partner Center API changes and Guide** in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="32aec-307">Ossza meg ezeket az információkat a szervezeten belüli megfelelő csapatokkal és a viszonteladóival, hogy felkészüljenek ezekre a változásokra.</span><span class="sxs-lookup"><span data-stu-id="32aec-307">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="32aec-308">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="32aec-308">Questions?</span></span>

<span data-ttu-id="32aec-309">Az értesítéssel kapcsolatos kérdéseit a támogatási [Partnerközpont meg.](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)</span><span class="sxs-lookup"><span data-stu-id="32aec-309">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="32aec-310">Változási napló</span><span class="sxs-lookup"><span data-stu-id="32aec-310">Change log</span></span>

- <span data-ttu-id="32aec-311">2021. május 4.: A GET-minősítés hamarosan elalasztott változatának végleges emlékeztetője</span><span class="sxs-lookup"><span data-stu-id="32aec-311">May 4, 2021: Final reminder of upcoming deprecation of GET qualification</span></span>

- <span data-ttu-id="32aec-312">2021. április 9.: Emlékeztető a GET-minősítés hamarosan elalasztásról</span><span class="sxs-lookup"><span data-stu-id="32aec-312">April 9, 2021: Reminder of upcoming deprecation of GET qualification</span></span> 

- <span data-ttu-id="32aec-313">Február: Frissültek a GET és PUT minősítések & idővonalai</span><span class="sxs-lookup"><span data-stu-id="32aec-313">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>

- <span data-ttu-id="32aec-314">Január: Emlékeztető a GET és PUT minősítések & elalasztásról</span><span class="sxs-lookup"><span data-stu-id="32aec-314">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="32aec-315">Az új kereskedelmi PDF-számla formátuma a CSP-ben</span><span class="sxs-lookup"><span data-stu-id="32aec-315">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="32aec-316">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="32aec-316">Categories</span></span>

- <span data-ttu-id="32aec-317">Dátum: 2021-04-05</span><span class="sxs-lookup"><span data-stu-id="32aec-317">Date: 2021-04-05</span></span>
- <span data-ttu-id="32aec-318">Képességek</span><span class="sxs-lookup"><span data-stu-id="32aec-318">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="32aec-319">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="32aec-319">Summary</span></span>

<span data-ttu-id="32aec-320">A Microsoft új formátumot vezet be az új kereskedelmi PDF-számlához a Felhőszolgáltató (CSP) programban, hogy a termékleírás helyett termékadatok szerint jelenítse meg a számlázási adatokat.</span><span class="sxs-lookup"><span data-stu-id="32aec-320">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="32aec-321">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="32aec-321">Impacted audience</span></span>

<span data-ttu-id="32aec-322">CSP-programon keresztül tranzakciós partnerek</span><span class="sxs-lookup"><span data-stu-id="32aec-322">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="32aec-323">Részletek</span><span class="sxs-lookup"><span data-stu-id="32aec-323">Details</span></span>

<span data-ttu-id="32aec-324">2021 májusával kezdődően a Microsoft új formátumot vezet be az új kereskedelmi PDF-számlához a CSP-programban, hogy a termékleírás helyett termékadatok szerint jelenítse meg a számlázási adatokat.</span><span class="sxs-lookup"><span data-stu-id="32aec-324">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="32aec-325">Ezzel az új frissítéssel a sorelemeket terméktípus szerint összesítődve jelenítjük meg az összes terméket egy külön sorban.</span><span class="sxs-lookup"><span data-stu-id="32aec-325">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="32aec-326">A partnerek észrevehetnek egy ilyen változást a 2021. április 1. és 2021. április 30. közötti számlázási időszakra vonatkozó májusi számlán.</span><span class="sxs-lookup"><span data-stu-id="32aec-326">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="32aec-327">Az érintett ajánlatok a Microsoft Azure, az Azure-előfizetések (Azure-csomag) és a Marketplace.</span><span class="sxs-lookup"><span data-stu-id="32aec-327">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="32aec-328">A számlaformátum frissítése után lekért jóváírási kérelmek az új formátumban jönnek létre.</span><span class="sxs-lookup"><span data-stu-id="32aec-328">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="32aec-329">Partneri előnyök</span><span class="sxs-lookup"><span data-stu-id="32aec-329">Partner benefits</span></span>

<span data-ttu-id="32aec-330">Ez a frissítés a következő fejlesztéseket tartalmazza a partnerek számlázási élményében:</span><span class="sxs-lookup"><span data-stu-id="32aec-330">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="32aec-331">Csökkentett számlaméret a kritikus adatok megőrzése közben</span><span class="sxs-lookup"><span data-stu-id="32aec-331">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="32aec-332">A formátum igazítása az iparági szabványokhoz a kompakt és felhasználóbarát számlákhoz</span><span class="sxs-lookup"><span data-stu-id="32aec-332">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="32aec-333">A következő elemekre ez nem lesz hatással:</span><span class="sxs-lookup"><span data-stu-id="32aec-333">The following elements will not be affected:</span></span>

- <span data-ttu-id="32aec-334">Számlázási összefoglaló oldal a számla PDF-fájlján</span><span class="sxs-lookup"><span data-stu-id="32aec-334">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="32aec-335">Meglévő számlázási API-k</span><span class="sxs-lookup"><span data-stu-id="32aec-335">Existing invoicing APIs</span></span>

- <span data-ttu-id="32aec-336">Egyeztetési fájlok (a recon-fájlok a részletes adatok leolvasására használhatók.)</span><span class="sxs-lookup"><span data-stu-id="32aec-336">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="32aec-337">Használati és licencalapú díjak számlái</span><span class="sxs-lookup"><span data-stu-id="32aec-337">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="32aec-338">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="32aec-338">Next steps</span></span>

<span data-ttu-id="32aec-339">Tekintse át a témakörrel kapcsolatos információkat a Microsoft partner [webhelyének Operations Readiness erőforrás-katalógusában.](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)</span><span class="sxs-lookup"><span data-stu-id="32aec-339">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="32aec-340">A számlázási és adózási témakörökről, például a számlázási erőforrásokról, a [](https://docs.microsoft.com/partner-center/billing) számlákról, a CSP-számlázásról és az adókról további információt a számlázással kapcsolatos szakaszban Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="32aec-340">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](https://docs.microsoft.com/partner-center/billing) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="32aec-341">A Felhőszolgáltató (CSP) ügyfélbehozatali követelményeinek változásai</span><span class="sxs-lookup"><span data-stu-id="32aec-341">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="32aec-342">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="32aec-342">Categories</span></span>

- <span data-ttu-id="32aec-343">Dátum: 2021-04-02</span><span class="sxs-lookup"><span data-stu-id="32aec-343">Date: 2021-04-02</span></span>
- <span data-ttu-id="32aec-344">Ajánlatok/piacok</span><span class="sxs-lookup"><span data-stu-id="32aec-344">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="32aec-345">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="32aec-345">Summary</span></span>

<span data-ttu-id="32aec-346">Elkötelezettségünk részeként, hogy segítsünk a partnereknek és az ügyfeleknek a bizalom alapján futtatni a munkájukat, további ügyféladatokat kérünk 2021. március 25-ig.</span><span class="sxs-lookup"><span data-stu-id="32aec-346">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="32aec-347">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="32aec-347">Impacted audience</span></span>

<span data-ttu-id="32aec-348">Közvetlen csp-számlázási partnerek és közvetett szolgáltatók, akik új vagy meglévő ügyfelekkel vannak a következő szakaszban felsorolt országokban</span><span class="sxs-lookup"><span data-stu-id="32aec-348">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="32aec-349">Részletek</span><span class="sxs-lookup"><span data-stu-id="32aec-349">Details</span></span>

<span data-ttu-id="32aec-350">A Microsoft megbízhatósági kapcsolaton fut.</span><span class="sxs-lookup"><span data-stu-id="32aec-350">Microsoft runs on trust.</span></span> <span data-ttu-id="32aec-351">Elkötelezettek vagyunk amellett, hogy megfelelő, biztonságos és biztonságos ügyfél-ellenőrzési módszert biztosítsunk az ügyfél-előfizetések tranzakciója során a CSP-programban.</span><span class="sxs-lookup"><span data-stu-id="32aec-351">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="32aec-352">2021. március 25-én bevezetünk egy API- és felhasználói felületi (UI) fejlesztéseket Partnerközpont, amelyek hatással lesznek az alábbi két feltételnek megfelelő partnerekre:</span><span class="sxs-lookup"><span data-stu-id="32aec-352">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="32aec-353">A partner közvetlen számlázási kapcsolattal rendelkezik a Microsofttal (ami azt jelenti, hogy a partner közvetlen számlázási partner vagy közvetett szolgáltató).</span><span class="sxs-lookup"><span data-stu-id="32aec-353">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="32aec-354">A partner az alábbi országokban lévő új vagy meglévő ügyfelekkel működik együtt:</span><span class="sxs-lookup"><span data-stu-id="32aec-354">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="32aec-355">Thaiföld</span><span class="sxs-lookup"><span data-stu-id="32aec-355">Thailand</span></span>
    - <span data-ttu-id="32aec-356">Vietnam</span><span class="sxs-lookup"><span data-stu-id="32aec-356">Vietnam</span></span>
    - <span data-ttu-id="32aec-357">Törökország</span><span class="sxs-lookup"><span data-stu-id="32aec-357">Turkey</span></span>
    - <span data-ttu-id="32aec-358">Lengyelország</span><span class="sxs-lookup"><span data-stu-id="32aec-358">Poland</span></span>
    - <span data-ttu-id="32aec-359">Dél-afrikai Köztársaság</span><span class="sxs-lookup"><span data-stu-id="32aec-359">South Africa</span></span>
    - <span data-ttu-id="32aec-360">India</span><span class="sxs-lookup"><span data-stu-id="32aec-360">India</span></span>
    - <span data-ttu-id="32aec-361">Brazília</span><span class="sxs-lookup"><span data-stu-id="32aec-361">Brazil</span></span>
    - <span data-ttu-id="32aec-362">Irak</span><span class="sxs-lookup"><span data-stu-id="32aec-362">Iraq</span></span>
    - <span data-ttu-id="32aec-363">Mianmar</span><span class="sxs-lookup"><span data-stu-id="32aec-363">Myanmar</span></span>
    - <span data-ttu-id="32aec-364">Dél-Szudán</span><span class="sxs-lookup"><span data-stu-id="32aec-364">South Sudan</span></span>
    - <span data-ttu-id="32aec-365">Szaúd-Arábia</span><span class="sxs-lookup"><span data-stu-id="32aec-365">Saudi Arabia</span></span>
    - <span data-ttu-id="32aec-366">Egyesült Arab Emírségek</span><span class="sxs-lookup"><span data-stu-id="32aec-366">United Arab Emirates</span></span>
    - <span data-ttu-id="32aec-367">Venezuela</span><span class="sxs-lookup"><span data-stu-id="32aec-367">Venezuela</span></span>

<span data-ttu-id="32aec-368">A feltételeknek megfelelő partnereknek be kell majd nyújtaniuk az ügyfél céges regisztrációs azonosítóját (más néven az ügyfél szervezeti INN-ét) és telefonszámát, amikor legközelebb frissítik vagy létrehoznak egy előfizetést az adott ügyfél számára.</span><span class="sxs-lookup"><span data-stu-id="32aec-368">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="32aec-369">Ezek a partnerek középső nevet is megadhatnak az ügyfél számára.</span><span class="sxs-lookup"><span data-stu-id="32aec-369">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="32aec-370">Vegye figyelembe, hogy a céges regisztrációs azonosító hozzáadásakor az üzleti adóazonosítót kell használnia, nem az ügyfél személyes azonosítóját.</span><span class="sxs-lookup"><span data-stu-id="32aec-370">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="32aec-371">Azok a partnerek, akik az alábbi országokban lévő új vagy meglévő ügyfelekkel üzleti partnereket hoznak létre, már elő vannak útjára 2020 novemberében egy korábbi kiadással.</span><span class="sxs-lookup"><span data-stu-id="32aec-371">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="32aec-372">Örményország</span><span class="sxs-lookup"><span data-stu-id="32aec-372">Armenia</span></span>
- <span data-ttu-id="32aec-373">Azerbajdzsán</span><span class="sxs-lookup"><span data-stu-id="32aec-373">Azerbaijan</span></span>
- <span data-ttu-id="32aec-374">Belarusz</span><span class="sxs-lookup"><span data-stu-id="32aec-374">Belarus</span></span>
- <span data-ttu-id="32aec-375">Magyarország</span><span class="sxs-lookup"><span data-stu-id="32aec-375">Hungary</span></span>
- <span data-ttu-id="32aec-376">Kazahsztán</span><span class="sxs-lookup"><span data-stu-id="32aec-376">Kazakhstan</span></span>
- <span data-ttu-id="32aec-377">Kirgizisztán</span><span class="sxs-lookup"><span data-stu-id="32aec-377">Kyrgyzstan</span></span>
- <span data-ttu-id="32aec-378">Moldova</span><span class="sxs-lookup"><span data-stu-id="32aec-378">Moldova</span></span>
- <span data-ttu-id="32aec-379">Oroszország</span><span class="sxs-lookup"><span data-stu-id="32aec-379">Russia</span></span>
- <span data-ttu-id="32aec-380">Tádzsikisztán</span><span class="sxs-lookup"><span data-stu-id="32aec-380">Tajikistan</span></span>
- <span data-ttu-id="32aec-381">Ukrajna</span><span class="sxs-lookup"><span data-stu-id="32aec-381">Ukraine</span></span>
- <span data-ttu-id="32aec-382">Üzbegisztán</span><span class="sxs-lookup"><span data-stu-id="32aec-382">Uzbekistan</span></span>

<span data-ttu-id="32aec-383">A világ többi részén az ügyfelekkel való partneri együttműködés 2021. március végén opcionálisan meg tudja majd adnia az ügyfelek céges regisztrációs azonosítóját, telefonszámát és középső nevét.</span><span class="sxs-lookup"><span data-stu-id="32aec-383">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="32aec-384">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="32aec-384">Next steps</span></span>

- <span data-ttu-id="32aec-385">Részletesebb útmutatásért tekintse át a műszaki dokumentációt és a dedikált [partnergyűjtemény](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) gyakori kérdéseit.</span><span class="sxs-lookup"><span data-stu-id="32aec-385">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="32aec-386">Készüljön fel a módosítások beépítése Partnerközpont API és a webes felhasználói felület használatával.</span><span class="sxs-lookup"><span data-stu-id="32aec-386">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="32aec-387">Az API/SDK-k elérhetők lesznek a teszteléshez.</span><span class="sxs-lookup"><span data-stu-id="32aec-387">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="32aec-388">A további adatokat mindenképpen el kell küldenünk az új ügyfelek előtt, vagy a meglévő ügyféladatok módosításakor.</span><span class="sxs-lookup"><span data-stu-id="32aec-388">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="32aec-389">Ha vezérlőpult-szállító (CPV) megoldást használ, tekintse meg a CPV-t.</span><span class="sxs-lookup"><span data-stu-id="32aec-389">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="32aec-390">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="32aec-390">Questions?</span></span>

<span data-ttu-id="32aec-391">Ha kérdése van a vállalat regisztrációs azonosítójával (más néven INN vagy TIN) kapcsolatban, lépjen kapcsolatba az adótanácsadóval vagy a helyi adóhivatalsal.</span><span class="sxs-lookup"><span data-stu-id="32aec-391">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="32aec-392">A Microsoft nem tud útmutatást nyújtani az adózási kérdésekkel kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="32aec-392">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="32aec-393">Ha támogatásra van szüksége a Microsofttal kapcsolatos műveleteihez, nyisson meg egy [szolgáltatáskérést.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="32aec-393">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="32aec-394">Az e havi termékbelövések és -ajánlatok megtekintése</span><span class="sxs-lookup"><span data-stu-id="32aec-394">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="32aec-395">Kategóriák</span><span class="sxs-lookup"><span data-stu-id="32aec-395">Categories</span></span>

- <span data-ttu-id="32aec-396">Dátum: 2021-04-01</span><span class="sxs-lookup"><span data-stu-id="32aec-396">Date: 2021-04-01</span></span>
- <span data-ttu-id="32aec-397">Képességek</span><span class="sxs-lookup"><span data-stu-id="32aec-397">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="32aec-398">Összefoglalás</span><span class="sxs-lookup"><span data-stu-id="32aec-398">Summary</span></span>

<span data-ttu-id="32aec-399">Közzétették a 2021. áprilisi termékindítási naptárt.</span><span class="sxs-lookup"><span data-stu-id="32aec-399">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="32aec-400">Érintett célközönség</span><span class="sxs-lookup"><span data-stu-id="32aec-400">Impacted audience</span></span>

<span data-ttu-id="32aec-401">Az összes partner, aki a Felhőszolgáltató (CSP) programon keresztül megy keresztül</span><span class="sxs-lookup"><span data-stu-id="32aec-401">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="32aec-402">Részletek</span><span class="sxs-lookup"><span data-stu-id="32aec-402">Details</span></span>

<span data-ttu-id="32aec-403">A 2021. [áprilisi](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) termékindítási naptár már elérhető az Üzemeltetési készenlét erőforrás-katalógusban.</span><span class="sxs-lookup"><span data-stu-id="32aec-403">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="32aec-404">A közelgő termékindításokat és -ajánlatokat itt megtekintheti.</span><span class="sxs-lookup"><span data-stu-id="32aec-404">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="32aec-405">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="32aec-405">Next steps</span></span>

<span data-ttu-id="32aec-406">Tekintse át [a termékindítási naptárt,](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)és ossza meg az információkat a szervezet megfelelő érdekelt felével.</span><span class="sxs-lookup"><span data-stu-id="32aec-406">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="32aec-407">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="32aec-407">Questions?</span></span>

<span data-ttu-id="32aec-408">Az ajánlatokkal kapcsolatos további kérdésekért tekintse meg az érintett Yammer-közösségeket.</span><span class="sxs-lookup"><span data-stu-id="32aec-408">For any further questions about these offers, check your relevant Yammer communities.</span></span>
