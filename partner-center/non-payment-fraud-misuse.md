---
title: Fizetéselmaradás, csalás vagy visszaélés kezelése
description: Ismerje meg az online tranzakciók során felmerülő kockázatokat, valamint a kockázatok kezelésével és enyhítésével kapcsolatos ajánlott eljárásokat a partner Centerben.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 75881544097abdfac8d6f96bde37e9700eb28cf7
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132349"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a><span data-ttu-id="a28f2-103">Fizetés elmaradása, csalás vagy visszaélés a Partnerközpontban</span><span class="sxs-lookup"><span data-stu-id="a28f2-103">Managing non-payment, fraud, or misuse in Partner Center</span></span>

<span data-ttu-id="a28f2-104">A következőkre vonatkozik:</span><span class="sxs-lookup"><span data-stu-id="a28f2-104">Applies to:</span></span>

- <span data-ttu-id="a28f2-105">Partneri központ a Microsoft Government cloudhoz</span><span class="sxs-lookup"><span data-stu-id="a28f2-105">Partner Center for Microsoft Government cloud</span></span>

<span data-ttu-id="a28f2-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="a28f2-106">**Appropriate roles**</span></span>

- <span data-ttu-id="a28f2-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="a28f2-107">Global admin</span></span>
- <span data-ttu-id="a28f2-108">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="a28f2-108">User management admin</span></span>
- <span data-ttu-id="a28f2-109">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="a28f2-109">Admin agent</span></span>
- <span data-ttu-id="a28f2-110">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="a28f2-110">Billing admin</span></span>

<span data-ttu-id="a28f2-111">Ön pénzügyi felelőssége, hogy az ügyfelek és/vagy a megvásárolt szolgáltatások nem fizetik ki az ügyfeleit.</span><span class="sxs-lookup"><span data-stu-id="a28f2-111">You are financially responsible for fraudulent purchases by your customers and/or customers' non-payment of purchased services.</span></span> <span data-ttu-id="a28f2-112">Ezért javasoljuk, *hogy a csalások megelőzésére és észlelésére vonatkozó kockázatkezelési vezérlőket helyezzen üzembe*.</span><span class="sxs-lookup"><span data-stu-id="a28f2-112">Therefore, *we strongly recommend that you put in place fraud prevention and detection risk mitigation controls*.</span></span>

<span data-ttu-id="a28f2-113">A csalárd tevékenységek és a visszaélések elkerülése és/vagy elhárítása érdekében fontos megérteni a lehetséges kockázatokat, valamint olyan házirendeket és gyakorlatokat, amelyek csökkenthetik a kitettséget.</span><span class="sxs-lookup"><span data-stu-id="a28f2-113">To avoid and/or address fraudulent activity or misuse, it's important to understand potential risks and to develop policies and practices that can reduce your exposure.</span></span>

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a><span data-ttu-id="a28f2-114">A Microsoft elfogadható használati szabályzatának kényszerítése</span><span class="sxs-lookup"><span data-stu-id="a28f2-114">Enforcement of Microsoft Acceptable Use Policy</span></span>

<span data-ttu-id="a28f2-115">Ha a Microsoft észleli, hogy az Ön által megerősített vagy gyanús partner vagy ügyfél tevékenysége megsérti az elfogadható használati szabályzatot, a rendszer végrehajtja a kényszerítési lépéseket.</span><span class="sxs-lookup"><span data-stu-id="a28f2-115">If Microsoft detects partner or customer activity that we confirm or suspect violates the Acceptable Use Policy, we will take enforcement steps.</span></span> <span data-ttu-id="a28f2-116">Az ügyfelet azonnal fel lehet függeszteni.</span><span class="sxs-lookup"><span data-stu-id="a28f2-116">The customer could be immediately suspended.</span></span> <span data-ttu-id="a28f2-117">A rendszer értesítést küld a kényszerítési műveletekről, vagy frissíti a Microsoft kérelmeit.</span><span class="sxs-lookup"><span data-stu-id="a28f2-117">You'll be notified of enforcement actions or updated on your requests by Microsoft.</span></span>

## <a name="abuse-of-service-risks"></a><span data-ttu-id="a28f2-118">A szolgáltatás kockázataival való visszaélés</span><span class="sxs-lookup"><span data-stu-id="a28f2-118">Abuse of service risks</span></span>

<span data-ttu-id="a28f2-119">A szolgáltatás kockázataival **való visszaélés** azt jelenti, hogy a Microsoft az elfogadható használati szabályzat megsértése miatt a Cloud Services szolgáltatást használja.</span><span class="sxs-lookup"><span data-stu-id="a28f2-119">**Abuse of service** risks means customers who use cloud services in violation of Microsoft's Acceptable Use Policy.</span></span>

### <a name="examples-of-abuse-of-service"></a><span data-ttu-id="a28f2-120">Példák a szolgáltatással való visszaélésre</span><span class="sxs-lookup"><span data-stu-id="a28f2-120">Examples of abuse of service</span></span>

<span data-ttu-id="a28f2-121">A Microsoft elfogadható használati szabályzatának ilyen megsértései például a következők lehetnek:</span><span class="sxs-lookup"><span data-stu-id="a28f2-121">Examples of these violations of Microsoft's acceptable use policy can include:</span></span>

- <span data-ttu-id="a28f2-122">Spam</span><span class="sxs-lookup"><span data-stu-id="a28f2-122">Spamming</span></span>
- <span data-ttu-id="a28f2-123">Hacking</span><span class="sxs-lookup"><span data-stu-id="a28f2-123">Hacking</span></span>
- <span data-ttu-id="a28f2-124">Elosztott szolgáltatásmegtagadási (DDoS) támadások</span><span class="sxs-lookup"><span data-stu-id="a28f2-124">Distributed denial-of-service (DDoS) attacks</span></span>
- <span data-ttu-id="a28f2-125">Bitcoin-bányászat</span><span class="sxs-lookup"><span data-stu-id="a28f2-125">Bitcoin mining</span></span>
- <span data-ttu-id="a28f2-126">Kártevők eloszlása</span><span class="sxs-lookup"><span data-stu-id="a28f2-126">Malware distribution</span></span>
- <span data-ttu-id="a28f2-127">A kalóz előfizetések viszonteladása</span><span class="sxs-lookup"><span data-stu-id="a28f2-127">Resale of pirated subscriptions</span></span>

## <a name="theft-of-service-risks"></a><span data-ttu-id="a28f2-128">A szolgáltatási kockázatok ellopása</span><span class="sxs-lookup"><span data-stu-id="a28f2-128">Theft of service risks</span></span>

<span data-ttu-id="a28f2-129">**A szolgáltatási kockázatok ellopása** azt jelenti, hogy a fogyasztóknak nem kell fizetniük a felhasznált szolgáltatásokért.</span><span class="sxs-lookup"><span data-stu-id="a28f2-129">**Theft of service** risks means customers who have no intention of paying for consumed services.</span></span> <span data-ttu-id="a28f2-130">Ez a lopás a lopott fizetési instrumentumok használatát, a téves számlázási adatok biztosítását és/vagy a fennmaradó egyenlegek alapértelmezett beállítását is magában foglalja.</span><span class="sxs-lookup"><span data-stu-id="a28f2-130">This theft may involve using stolen payment instruments, providing false billing information, and/or defaulting on outstanding balances.</span></span>

### <a name="examples-of-service-theft"></a><span data-ttu-id="a28f2-131">Példák a szolgáltatások ellopására</span><span class="sxs-lookup"><span data-stu-id="a28f2-131">Examples of service theft</span></span>

<span data-ttu-id="a28f2-132">Ilyen online tranzakciós kockázatok például a következők lehetnek:</span><span class="sxs-lookup"><span data-stu-id="a28f2-132">Examples of these online transaction risks can include:</span></span>

- <span data-ttu-id="a28f2-133">A személyesen nem előforduló tranzakciók ("hitelkártya nem jelen" tranzakciók)</span><span class="sxs-lookup"><span data-stu-id="a28f2-133">Transactions that don't occur in person ("credit card not present" transactions)</span></span>
- <span data-ttu-id="a28f2-134">Tévesen használt identitások</span><span class="sxs-lookup"><span data-stu-id="a28f2-134">Misrepresented identities</span></span>
- <span data-ttu-id="a28f2-135">A kezdeti fizetés fogadása előtt kiépített és használt szolgáltatások</span><span class="sxs-lookup"><span data-stu-id="a28f2-135">Services provisioned and used before initial payment is received</span></span>
- <span data-ttu-id="a28f2-136">Feltörekvő piacok és/vagy magas kockázatú régiók online csalások esetén</span><span class="sxs-lookup"><span data-stu-id="a28f2-136">Emerging markets and/or high-risk regions for online fraud</span></span>
- <span data-ttu-id="a28f2-137">A fiókok létrehozásának és a hibás szereplők általi vásárlásának automatizálása</span><span class="sxs-lookup"><span data-stu-id="a28f2-137">Automate account creation and purchasing by bad actors</span></span>

## <a name="managing-online-risk"></a><span data-ttu-id="a28f2-138">Online kockázat kezelése</span><span class="sxs-lookup"><span data-stu-id="a28f2-138">Managing online risk</span></span>

<span data-ttu-id="a28f2-139">A következő javaslatok segítségével kifejlesztheti a szabályzatokat és a gyakorlatokat, hogy csökkentse az online tranzakciós kockázatokat az ügyfélkapcsolatok életciklusa során.</span><span class="sxs-lookup"><span data-stu-id="a28f2-139">You can use the following recommendations to help you develop policies and practices to reduce your exposure to online transaction risks in the lifecycle of your customer relationships.</span></span>

### <a name="onboarding-new-customers"></a><span data-ttu-id="a28f2-140">Új ügyfelek bevezetése</span><span class="sxs-lookup"><span data-stu-id="a28f2-140">Onboarding new customers</span></span>

<span data-ttu-id="a28f2-141">Az új ügyfelek bevezetéséhez szükséges online veszélyforrások csökkentésére vonatkozó javaslatok a következők:</span><span class="sxs-lookup"><span data-stu-id="a28f2-141">Suggestions for reducing online risks when onboarding new customers include:</span></span>

- <span data-ttu-id="a28f2-142">Hozzon létre személyes kapcsolatot az ügyfelekkel, ha lehetséges (például telefonos kapcsolatfelvételsel).</span><span class="sxs-lookup"><span data-stu-id="a28f2-142">Establish personal relationships with customers when possible (for example, contacting customers by phone).</span></span>
- <span data-ttu-id="a28f2-143">Ellenőrizze az ügyfelek hitelesítő adatait és hátterét a jobb módszerekkel (például a Credit Bureaus vagy az üzleti kereskedelmi jelentéskészítő ügynökségek használatával).</span><span class="sxs-lookup"><span data-stu-id="a28f2-143">Verify customers' credentials and background through better methods (such as using credit bureaus or business commercial report agencies).</span></span>
- <span data-ttu-id="a28f2-144">A többtényezős hitelesítés (például SMS-ellenőrzés) használata a regisztráció során a Robotos fiókok létrehozásával és megvásárlásával kapcsolatos kockázat csökkentése érdekében.</span><span class="sxs-lookup"><span data-stu-id="a28f2-144">Use multi-factor authentication (such as SMS verification) during sign-up to minimize exposure to robotic account creation and purchasing.</span></span>
- <span data-ttu-id="a28f2-145">Az identitások kezelése és nyomon követése szolgáltatásokkal (például a digitális Identity Services használatával).</span><span class="sxs-lookup"><span data-stu-id="a28f2-145">Manage and track identities using services (such as digital identity services).</span></span>
- <span data-ttu-id="a28f2-146">Mérje fel az ügyfelek pénzügyi erejét szigorú hitelkártya-csalások észlelési rendszerein keresztül.</span><span class="sxs-lookup"><span data-stu-id="a28f2-146">Assess customer financial strength through rigorous credit card fraud detection systems.</span></span>
- <span data-ttu-id="a28f2-147">Hozzon létre egy Clear Collections-szabályzatot.</span><span class="sxs-lookup"><span data-stu-id="a28f2-147">Establish a clear collections policy.</span></span> <span data-ttu-id="a28f2-148">Részletesen ismerteti a gyűjtemények folyamatát, és az előfizetések hozzáférését nem kell kifizetni.</span><span class="sxs-lookup"><span data-stu-id="a28f2-148">Detail your collections process and when access to subscriptions will be impacted by non-payment.</span></span> <span data-ttu-id="a28f2-149">(Letilthatja a hozzáférést, vagy [felfüggesztheti az ügyfél előfizetéseit](create-a-new-subscription.md#suspend-a-subscription) a nem fizetéshez.)</span><span class="sxs-lookup"><span data-stu-id="a28f2-149">(You can disable access or [suspend a customer's subscriptions](create-a-new-subscription.md#suspend-a-subscription) for non-payment.)</span></span>

### <a name="managing-customer-accounts"></a><span data-ttu-id="a28f2-150">Ügyfélfiókok kezelése</span><span class="sxs-lookup"><span data-stu-id="a28f2-150">Managing customer accounts</span></span>

<span data-ttu-id="a28f2-151">A vásárlói fiókok a vásárlás utáni kezelésével kapcsolatos javaslatok a következők:</span><span class="sxs-lookup"><span data-stu-id="a28f2-151">Suggestions for managing customer accounts post-purchase include:</span></span>

- <span data-ttu-id="a28f2-152">Hozzon létre egy folyamatot a Microsoft értesítéseinek gyors fogadásához, felülvizsgálatához, kezeléséhez és megválaszolásához.</span><span class="sxs-lookup"><span data-stu-id="a28f2-152">Implement a process to quickly receive, review, act on, and respond to Microsoft notifications.</span></span>
- <span data-ttu-id="a28f2-153">Az ügyfelekkel együttműködve megismerheti a Felhőbeli használat üzleti igényeit a beállítások megfelelő figyelési küszöbértékei mellett.</span><span class="sxs-lookup"><span data-stu-id="a28f2-153">Work with customers to understand their cloud usage business needs while settings appropriate monitoring thresholds.</span></span> <span data-ttu-id="a28f2-154">(Beállíthat például [egy havi Azure-költségkeretet](set-an-azure-spending-budget-for-your-customers.md) a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="a28f2-154">(For example, you can [set a monthly Azure spending budget](set-an-azure-spending-budget-for-your-customers.md) in Partner Center.</span></span> <span data-ttu-id="a28f2-155">Ez a megértés lehetővé teszi az ügyfelek használatának figyelését a hónap során, és értesítést kap, ha az ügyfelek a költségvetésük közeledik.)</span><span class="sxs-lookup"><span data-stu-id="a28f2-155">This understanding allows you to monitor customer usage during the month and be notified when customers are close to their budget.)</span></span>
- <span data-ttu-id="a28f2-156">A csalások korai észlelése érdekében rendszeresen figyelje az [ügyfelek tevékenységének naplóit](activity-logs.md) .</span><span class="sxs-lookup"><span data-stu-id="a28f2-156">Monitor [customer activity logs](activity-logs.md) regularly to help detect fraud early.</span></span>
- <span data-ttu-id="a28f2-157">A rendszer a gyanús tevékenységek észlelésekor gyors műveletet végez.</span><span class="sxs-lookup"><span data-stu-id="a28f2-157">Take quick action when suspicious activities are detected.</span></span>
- <span data-ttu-id="a28f2-158">Ne adja meg az ügyfeleknek teljes körű rendszergazdai hozzáférést az előfizetésekhez a kockázatkezelési vezérlők első alkalmazása nélkül.</span><span class="sxs-lookup"><span data-stu-id="a28f2-158">Avoid giving customers full administrative access to subscriptions without first implementing risk mitigation controls.</span></span>

### <a name="managing-customer-billing"></a><span data-ttu-id="a28f2-159">Ügyfél-számlázás kezelése</span><span class="sxs-lookup"><span data-stu-id="a28f2-159">Managing customer billing</span></span>

<span data-ttu-id="a28f2-160">A vásárlói számlázás utáni kezelési javaslatok a következők:</span><span class="sxs-lookup"><span data-stu-id="a28f2-160">Suggestions for managing customer billing post-purchase include:</span></span>

- <span data-ttu-id="a28f2-161">Előzetes befizetések igénylése a kezdeti tranzakciók és a számlázás előtt.</span><span class="sxs-lookup"><span data-stu-id="a28f2-161">Request prepayments prior to initial transactions and billing.</span></span>
- <span data-ttu-id="a28f2-162">Ne fogadjon el magas kockázatú fizetési eszközöket (például előre fizetett kártyákat vagy tárolt értékű kártyákat).</span><span class="sxs-lookup"><span data-stu-id="a28f2-162">Don't accept high-risk payment instruments (such as pre-paid cards or stored-value cards).</span></span>
- <span data-ttu-id="a28f2-163">Figyelheti az ügyfelek kifizetéseit és az elöregedő fiókok követeléseit.</span><span class="sxs-lookup"><span data-stu-id="a28f2-163">Monitor customer payments and aging accounts receivables.</span></span> <span data-ttu-id="a28f2-164">A késedelmes befizetések és a nem fizetések esetében agresszíven érvényesítheti a szabványosított Dunning-folyamatokat.</span><span class="sxs-lookup"><span data-stu-id="a28f2-164">Aggressively enforce standardized dunning processes for late payments or non-payment.</span></span>

<span data-ttu-id="a28f2-165">Az online kockázat mérséklésével kapcsolatos részletesebb stratégiákat az [online tranzakciós kockázatkezelési útmutatóban találja.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)</span><span class="sxs-lookup"><span data-stu-id="a28f2-165">For more detailed strategies for mitigating online risk, see the [Online transaction risk management guide.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)</span></span>
