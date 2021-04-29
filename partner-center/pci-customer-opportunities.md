---
title: Partnerközpont Insights – CloudAscent Propensity-jelentések
description: További információ a CloudAscent propensity jelentésekről a Partnerközpont. Arra vonatkozó információkat tartalmaz, hogy az ügyfelek hogyan nem vásárolhatnak Microsoft-termékeket.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 91f64faeec0b97be2797d489e152cb84cbb2e192
ms.sourcegitcommit: 8bd2e2f2f0f6bcd0fa202787df5b3c1f786f88f9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/29/2021
ms.locfileid: "108213446"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="b8e66-104">Az irányítópulton elérhető CloudAscent propensity Partnerközpont jelentéseket</span><span class="sxs-lookup"><span data-stu-id="b8e66-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="b8e66-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="b8e66-105">**Appropriate roles**</span></span>

- <span data-ttu-id="b8e66-106">Vezetői jelentésmegjelenítő</span><span class="sxs-lookup"><span data-stu-id="b8e66-106">Executive report viewer</span></span>
- <span data-ttu-id="b8e66-107">Jelentésmegjelenítő</span><span class="sxs-lookup"><span data-stu-id="b8e66-107">Report viewer</span></span>

<span data-ttu-id="b8e66-108">A Partnerközpont irányítópult letölthető propenitási adatokat biztosít a CloudAscent programból.</span><span class="sxs-lookup"><span data-stu-id="b8e66-108">The Partner Center dashboard provides downloadable propensity data from the CloudAscent program.</span></span> <span data-ttu-id="b8e66-109">Az adatok azt mutatják, hogy az ügyfelek milyen valószínűséggel vásárolhatnak Microsoft-termékeket.</span><span class="sxs-lookup"><span data-stu-id="b8e66-109">The data shows the customers' likelihood to purchase Microsoft products.</span></span>  <span data-ttu-id="b8e66-110">Ez a cikk az adatok lebontását, a pontozás használatát és azt ismerteti, hogy mit jelent.</span><span class="sxs-lookup"><span data-stu-id="b8e66-110">This article describes the breakdown of this data, how to use the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="b8e66-111">Összegzési definíciók</span><span class="sxs-lookup"><span data-stu-id="b8e66-111">Summary definitions</span></span>

- <span data-ttu-id="b8e66-112">**SMC-ügyfelek**– Ez a propensitásletöltésben található ügyfelek teljes száma.</span><span class="sxs-lookup"><span data-stu-id="b8e66-112">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="b8e66-113">Az ügyfeleket a rekordpartner azonosítja.</span><span class="sxs-lookup"><span data-stu-id="b8e66-113">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="b8e66-114">**Szerződések lejárata**– Az aktuális pénzügyi évben meg kell adtunk a lejáró szerződések számát.</span><span class="sxs-lookup"><span data-stu-id="b8e66-114">**Expire Agreements**– Within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="b8e66-115">Open Expiring Revenue (Nyitott **lejáró bevétel)**– A nyitott lejáró szerződésekhez társított bevétel.</span><span class="sxs-lookup"><span data-stu-id="b8e66-115">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Képernyőkép az Ügyfelek lehetőségek összegzése irányítópultról.":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="b8e66-117">CloudAscent SMB-szegmentálás</span><span class="sxs-lookup"><span data-stu-id="b8e66-117">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="b8e66-118">A kis- és középvállalati (SMB) szegmens három különálló alszegmensre oszlik.</span><span class="sxs-lookup"><span data-stu-id="b8e66-118">The small to medium business (SMB) segment is divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="b8e66-119">**A leggyakoribb nem nem használt szolgáltatás a** Legnagyobb SMB-ügyfeleket tartalmazza, akik a legtöbb lehetőséget kínálják a Microsoft számára.</span><span class="sxs-lookup"><span data-stu-id="b8e66-119">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="b8e66-120">A tipikus nem felügyelt ügyfelek hasonló jellemzőkkel rendelkeznek, mint a felügyelt fiókok, sok alkalmazottal, nagy it-költségkeretekkel és kiadásokkal, valamint nagy mennyiségű potenciális bevétellel a Microsoft számára.</span><span class="sxs-lookup"><span data-stu-id="b8e66-120">Typical Top Unmanaged customers share similar characteristics to Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="b8e66-121">A nem nem felső szintűeket kétféleképpen definiáljuk:</span><span class="sxs-lookup"><span data-stu-id="b8e66-121">We define Top Unmanaged in two ways:</span></span>

   - <span data-ttu-id="b8e66-122">**Top Unmanaged User Based**–, 300 vagy több alkalmazottal rendelkező fiókokat tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="b8e66-122">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="b8e66-123">User-Based fiókok kiváló célok az első alkalommal való vásárláshoz, illetve a felhasználóalapú előfizetési termékek (például a Microsoft 365, a Dynamics 365 vagy a Surface) bővítéséhez.</span><span class="sxs-lookup"><span data-stu-id="b8e66-123">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as Microsoft 365, Dynamics 365, or Surface.</span></span>
   - <span data-ttu-id="b8e66-124">**Top Unmanaged Compute Based** ( Top Unmanaged Compute Based – Olyan fiókokat tartalmaz, amelyek azure-beli potenciálisan nagyobbak 10 ezer dollárnál).</span><span class="sxs-lookup"><span data-stu-id="b8e66-124">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="b8e66-125">A számítási alapú fiókok tartalmazzák a meglévő Azure-t.</span><span class="sxs-lookup"><span data-stu-id="b8e66-125">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="b8e66-126">a jelentős jövő évi potenciális fiókokkal és olyan fiókokkal, amelyek még nem vásárolják meg az Azure-t, de az Azure-ra több mint 10 ezer usd-t is el lehet látni.</span><span class="sxs-lookup"><span data-stu-id="b8e66-126">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="b8e66-127">**A Medium Business** a meglévő ügyfeleket és a 25–300 alkalmazottal rendelkező potenciális ügyfeleket tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="b8e66-127">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="b8e66-128">**A kisvállalatok** 10–25 alkalmazottal dolgozó vállalkozásokat foglalnak magába.</span><span class="sxs-lookup"><span data-stu-id="b8e66-128">**Small Business** includes businesses with 10-25 employees.</span></span>

4. <span data-ttu-id="b8e66-129">**A Nagyon kisvállalatok** közé tartoznak az 1–9 alkalmazottal dolgozó üzletek.</span><span class="sxs-lookup"><span data-stu-id="b8e66-129">**Very Small Business** includes businesses with 1-9 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Ügyfél SMC-típus szerint.":::

<span data-ttu-id="b8e66-131">**A nem és a közepes** üzleti alkategóriák a Microsoft és a Microsoft partnerei számára jelentős élettartamú (LTV) ügyfeleket képviselnek. </span><span class="sxs-lookup"><span data-stu-id="b8e66-131">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="b8e66-132">Emiatt ezek a területek a növekedés fő területei ebben a szegmensben.</span><span class="sxs-lookup"><span data-stu-id="b8e66-132">Because of this, they're the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="b8e66-133">Ebben a két alszegben jobb helyzetben vagyunk a szoftvercsatornák Microsoft 365-val való megszerzéséhez, a D365/Azure üzletági (LOB) alkalmazásokból való további bevételhez, és a Microsoft magas LTV-használatának szerzéséhez.</span><span class="sxs-lookup"><span data-stu-id="b8e66-133">In these two subsegments, we're better positioned to acquire the socket with Microsoft 365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="b8e66-134">Jelenleg két fő lehetőségünk van: 1.</span><span class="sxs-lookup"><span data-stu-id="b8e66-134">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="b8e66-135">az ügyfél növekedést ad hozzá; 2.</span><span class="sxs-lookup"><span data-stu-id="b8e66-135">our customer adds growth; 2.</span></span> <span data-ttu-id="b8e66-136">míg a felhőbeli szoftvercsatornákat jól Microsoft 365, a Dynamics 365-ben és az Azure-ban nagy lehetőségünk van.</span><span class="sxs-lookup"><span data-stu-id="b8e66-136">while we do well acquiring cloud sockets leading with Microsoft 365, we have a large opportunity in Dynamics 365 and Azure.</span></span>

<span data-ttu-id="b8e66-137">Az alábbi képernyőkép a négy SMB-alszegmentet ábrázolja.</span><span class="sxs-lookup"><span data-stu-id="b8e66-137">The following screenshot represents the four SMB Subsegments.</span></span> <span data-ttu-id="b8e66-138">A CloudAscent rangsorolnia kell az összes legfontosabb nem nem és közepes üzleti fiók profilkészítését, pontozását és modellezését.</span><span class="sxs-lookup"><span data-stu-id="b8e66-138">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Az SMB-alszegmentek képernyőképe.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="b8e66-140">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="b8e66-140">CloudAscent Machine Learning</span></span>

<span data-ttu-id="b8e66-141">Az SMB gépi tanulási technológiával használja az értékesítési és marketing ügyfél-előrejelzéseket a nem használt és közepes üzleti szegmensben.</span><span class="sxs-lookup"><span data-stu-id="b8e66-141">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="b8e66-142">Hogyan gyűjti és váltja fel a jeleket a propensitási javaslatokké?</span><span class="sxs-lookup"><span data-stu-id="b8e66-142">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="b8e66-143">**Adatgyűjtés:** A webbejárási webbejárások több milliárd ügyféljelet vizsgálnak és gyűjtenek a vállalati tartományok pingelése, a blogbejegyzések figyelése, a kiadások, a közösségi streamek és a technikai fórumok segítségével.</span><span class="sxs-lookup"><span data-stu-id="b8e66-143">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="b8e66-144">Az összegyűjtött jelek mellett a céges adatok olyan belső és külső forrásokból is gyűjtenek adatokat, mint a D&B, a Microsoft belső előfizetési és tranzakciós adatai.</span><span class="sxs-lookup"><span data-stu-id="b8e66-144">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="b8e66-145">**Machine Learning:** A jelek be vannak állítva a gépi tanulási modellbe, amely az egyes ügyfelekre vonatkozó értékesítési és marketing-előrejelzések strukturált adatkészletét adja vissza a felhőalapú termékek és fürtök alapján.</span><span class="sxs-lookup"><span data-stu-id="b8e66-145">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="b8e66-146">Minden ügyfél pontozása a Microsoft legfelső SMB-hez hasonló, az ügyfél illeszkedést meghatározó modelljével, az ügyfél online viselkedését integráló gépi tanulási algoritmusokkal pedig szándékként van meghatározva.</span><span class="sxs-lookup"><span data-stu-id="b8e66-146">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="b8e66-147">A pontozás olyan fürtökbe van egyesülve, amelyek megmutatják, hogy az ügyfél nem hajlandó Microsoft Cloud-termékeket vásárolni.</span><span class="sxs-lookup"><span data-stu-id="b8e66-147">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="b8e66-148">**Optimalizálás:** A Machine Learning optimalizálja a modelleket a tranzakciós adatok havi és az előfizetési adatok negyedévente való fogyasztásával.</span><span class="sxs-lookup"><span data-stu-id="b8e66-148">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="b8e66-149">A nyerés/veszteség adatok használatával a Machine Learning beállítja az algoritmusokat, és ellenőrzi, hogy a modellek a várt módon működnek-e, összehasonlítva a fürtre vonatkozó javaslatokat az MSX-hez használt lehetőségekkel.</span><span class="sxs-lookup"><span data-stu-id="b8e66-149">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Képernyőkép az SMB gépi tanulásról.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="b8e66-151">CloudAscent Propensity</span><span class="sxs-lookup"><span data-stu-id="b8e66-151">CloudAscent Propensity</span></span>

<span data-ttu-id="b8e66-152">Hogyan jön létre a propensitási javaslatok létrehozása?</span><span class="sxs-lookup"><span data-stu-id="b8e66-152">How are propensity recommendations created?</span></span>

<span data-ttu-id="b8e66-153">A webes webbejárási eszközök és a különböző forrásokból származó adatok alapján gyűjtött jelek használatával konszolidáljuk a céges adatokat és az ügyfél közösségimédia-jeleit.</span><span class="sxs-lookup"><span data-stu-id="b8e66-153">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="b8e66-154">A pontozás ezeket a jeleket és adatokat használja összehasonlítási modellekben a szándékok illesztési és pontozási modelljeihez.</span><span class="sxs-lookup"><span data-stu-id="b8e66-154">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="b8e66-155">Ügyfélfiók illeszkedés</span><span class="sxs-lookup"><span data-stu-id="b8e66-155">Customer Account Fit</span></span>

   - <span data-ttu-id="b8e66-156">Belső és külső adatpontok, amelyek a céges adatokat határozzák meg.</span><span class="sxs-lookup"><span data-stu-id="b8e66-156">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="b8e66-157">A illeszkedés pontozása a legjobb SMB-modellhez hasonlóan hasonlítja össze az ügyfeleket, és megnézi, hogy megfelelőek-e a Microsoft Cloud-termékekhez.</span><span class="sxs-lookup"><span data-stu-id="b8e66-157">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="b8e66-158">A illeszkedés pontozása negyedévente frissül</span><span class="sxs-lookup"><span data-stu-id="b8e66-158">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="b8e66-159">Ügyfélfiók szándéka</span><span class="sxs-lookup"><span data-stu-id="b8e66-159">Customer Account Intent</span></span>

   - <span data-ttu-id="b8e66-160">A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot.</span><span class="sxs-lookup"><span data-stu-id="b8e66-160">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="b8e66-161">A szándékpontozás felül megfelel a fürtök meghatározásának.</span><span class="sxs-lookup"><span data-stu-id="b8e66-161">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="b8e66-162">A szándékpontozás havonta frissül.</span><span class="sxs-lookup"><span data-stu-id="b8e66-162">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB prediktív modellek.":::

3. <span data-ttu-id="b8e66-164">Fürtözés</span><span class="sxs-lookup"><span data-stu-id="b8e66-164">Clustering</span></span>

   <span data-ttu-id="b8e66-165">Az illesztési és szándékra vonatkozó jelek egy fürtözési pontszámban vannak összesíteni.</span><span class="sxs-lookup"><span data-stu-id="b8e66-165">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="b8e66-166">A CloudAscent négy fürtből rendelkezik:</span><span class="sxs-lookup"><span data-stu-id="b8e66-166">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="b8e66-167">Act Now – értékesítésre kész ügyfelek</span><span class="sxs-lookup"><span data-stu-id="b8e66-167">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="b8e66-168">Értékelés – marketingre kész ügyfelek</span><span class="sxs-lookup"><span data-stu-id="b8e66-168">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="b8e66-169">Figyelemfelkeltő kampányok</span><span class="sxs-lookup"><span data-stu-id="b8e66-169">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="b8e66-170">Oktatás – szándék oktatása és figyelése</span><span class="sxs-lookup"><span data-stu-id="b8e66-170">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="b8e66-171">A fürtözés lehetővé teszi, hogy a felhasználók adott ügyfeleket célozzanak meg értékesítési és marketinges kezdeményezésekhez olyan szegmenstényezők alapján, mint például a termék, a földrajzi hely, az iparág és a vertikális.</span><span class="sxs-lookup"><span data-stu-id="b8e66-171">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="b8e66-172">A CloudAscent-munkafüzetek **Propensity Model (Propensity-modell)** lapja a propensitást és a becsült térbeli bevételt osztja meg.</span><span class="sxs-lookup"><span data-stu-id="b8e66-172">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="b8e66-173">Az illeszkedés és a szándék fürtözésének meghatározásához a következő lépéseket kell végigmenni:</span><span class="sxs-lookup"><span data-stu-id="b8e66-173">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="b8e66-174">Ml-modellek használatával először kiszámítjuk a Customer Fit Score (Ügyfél illesztési pontszáma) és a Intent Score (szándék pontszáma) értékeket egy 100-as skálán.</span><span class="sxs-lookup"><span data-stu-id="b8e66-174">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="b8e66-175">A pontos pontszámok az ML-modellektől függően változnak.</span><span class="sxs-lookup"><span data-stu-id="b8e66-175">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="b8e66-176">Példa pontszámok alább:</span><span class="sxs-lookup"><span data-stu-id="b8e66-176">Example Scores Below:</span></span>

         |<span data-ttu-id="b8e66-177">**Osztályozás**</span><span class="sxs-lookup"><span data-stu-id="b8e66-177">**Classification**</span></span>|<span data-ttu-id="b8e66-178">**Pontszám**</span><span class="sxs-lookup"><span data-stu-id="b8e66-178">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="b8e66-179">Magas</span><span class="sxs-lookup"><span data-stu-id="b8e66-179">High</span></span>|<span data-ttu-id="b8e66-180">75 - 100</span><span class="sxs-lookup"><span data-stu-id="b8e66-180">75 - 100</span></span>|
         |<span data-ttu-id="b8e66-181">Közepes</span><span class="sxs-lookup"><span data-stu-id="b8e66-181">Medium</span></span>|<span data-ttu-id="b8e66-182">55 - 74</span><span class="sxs-lookup"><span data-stu-id="b8e66-182">55 - 74</span></span>|
         |<span data-ttu-id="b8e66-183">Alacsony</span><span class="sxs-lookup"><span data-stu-id="b8e66-183">Low</span></span>|<span data-ttu-id="b8e66-184">30 - 54</span><span class="sxs-lookup"><span data-stu-id="b8e66-184">30 - 54</span></span>|
         |<span data-ttu-id="b8e66-185">Nagyon alacsony</span><span class="sxs-lookup"><span data-stu-id="b8e66-185">Very Low</span></span>|<span data-ttu-id="b8e66-186">0 - 29</span><span class="sxs-lookup"><span data-stu-id="b8e66-186">0 - 29</span></span>|

      2. <span data-ttu-id="b8e66-187">A fenti szabályt használva a vállalatokat magas, közepes, alacsony és nagyon alacsony besorolásúként osztályozjuk mind az ügyfél illeszkedési, mind a szándékjel alapján.</span><span class="sxs-lookup"><span data-stu-id="b8e66-187">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit and Intent Signals.</span></span>

      3. <span data-ttu-id="b8e66-188">Az ügyfelek illeszkedési és szándékjeleit egy 2D-s mátrixon ábrázoljuk, és minden metszet a nem megfelelőséget jelképez.</span><span class="sxs-lookup"><span data-stu-id="b8e66-188">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span> <span data-ttu-id="b8e66-189">Például: Magas illeszkedés + Magas szándék = A1, amely a legnagyobb propensitást képviseli.</span><span class="sxs-lookup"><span data-stu-id="b8e66-189">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="b8e66-190">Végül ezek a szegmensek csoportosítva alkotnak fürtöt.</span><span class="sxs-lookup"><span data-stu-id="b8e66-190">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="b8e66-191">Például az A1, A2, A3, A4 az Act Now fürtöt alkotják.</span><span class="sxs-lookup"><span data-stu-id="b8e66-191">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent-modellek.":::

   <span data-ttu-id="b8e66-193">Javasoljuk, hogy ezeknél az ügyfeleknél az Act Now (Most járjon el) és a Evaluate customers (Ügyfelek kiértékelése) célcsoportot célozza meg.</span><span class="sxs-lookup"><span data-stu-id="b8e66-193">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="b8e66-194">CloudAscent-termékek & modellek</span><span class="sxs-lookup"><span data-stu-id="b8e66-194">CloudAscent Products & Models</span></span>

<span data-ttu-id="b8e66-195">Az alábbi ábra a CloudAscent szolgáltatáson belüli egyes támogatói modelleket tartalmazza:</span><span class="sxs-lookup"><span data-stu-id="b8e66-195">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent propensity modell.":::

<span data-ttu-id="b8e66-197">A téreltérmodellek olyan meglévő Microsoft-ügyfelek előrejelzései, akik nem tartalmaznak terméket, és/vagy nettó új potenciális ügyfelek.</span><span class="sxs-lookup"><span data-stu-id="b8e66-197">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="b8e66-198">Az upsell modellek tranzakciós adatokkal jelezik előre az Azure-beli és a Microsoft 365 potenciális lehetőségeit.</span><span class="sxs-lookup"><span data-stu-id="b8e66-198">Upsell models use transaction data to predict the potential for upsell in Azure and Microsoft 365 SKUs.</span></span>

<span data-ttu-id="b8e66-199">Ezek az ügyfelek már most is az Azure-ral vagy a Microsoft 365, és az upsell modell azt mutatja, hogy valószínűleg többet fognak vásárolni a meglévő termékváltozatukból.</span><span class="sxs-lookup"><span data-stu-id="b8e66-199">These customers will already have both Azure or Microsoft 365 and the upsell model shows that they’re likely to purchase more of their existing SKU.</span></span>

<span data-ttu-id="b8e66-200">Az EOS a Win 7, az Office 2010, a SQL Server és a Windows Server esetében megosztja a szolgáltatásvégi (EOS) ügyfeleket.</span><span class="sxs-lookup"><span data-stu-id="b8e66-200">EOS shares the end of service (EOS) customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="b8e66-201">Az EOS-adatokat a rendszer lekérte az MS Sales szolgáltatásból, és átfedi őket a CloudAscent propensity modellel, ha elérhető.</span><span class="sxs-lookup"><span data-stu-id="b8e66-201">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="b8e66-202">Az EOS-adatok a Modern Workben és az Azure Salesben játszódnak.</span><span class="sxs-lookup"><span data-stu-id="b8e66-202">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
