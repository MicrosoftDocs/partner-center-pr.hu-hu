---
title: Partnerközpont Elemzések – CloudAscent Propensity-jelentések
description: További információ a CloudAscent propensity jelentésekről a Partnerközpont. Információkat tartalmaz arról, hogy az ügyfél hogyan nem tud Microsoft-termékeket vásárolni.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 6916d44e3f028fbfd788d3bee54671dbadd874d1
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376810"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="98700-104">Az irányítópulton elérhető CloudAscent propensity Partnerközpont jelentéseket</span><span class="sxs-lookup"><span data-stu-id="98700-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="98700-105">**Megfelelő szerepkörök:** Vezetői jelentésmegjelenítő | Jelentésmegjelenítő</span><span class="sxs-lookup"><span data-stu-id="98700-105">**Appropriate roles**: Executive report viewer | Report viewer</span></span>

<span data-ttu-id="98700-106">A Partnerközpont irányítópult letölthető propenitási adatokat biztosít a CloudAscent programból.</span><span class="sxs-lookup"><span data-stu-id="98700-106">The Partner Center dashboard provides downloadable propensity data from the CloudAscent program.</span></span> <span data-ttu-id="98700-107">Az adatok azt mutatják, hogy az ügyfelek milyen valószínűséggel vásárolhatnak Microsoft-termékeket.</span><span class="sxs-lookup"><span data-stu-id="98700-107">The data shows the customers' likelihood to purchase Microsoft products.</span></span>  <span data-ttu-id="98700-108">Ez a cikk az adatok lebontását, a pontozás használatát és azt ismerteti, hogy mit jelent.</span><span class="sxs-lookup"><span data-stu-id="98700-108">This article describes the breakdown of this data, how to use the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="98700-109">Összefoglaló definíciók</span><span class="sxs-lookup"><span data-stu-id="98700-109">Summary definitions</span></span>

- <span data-ttu-id="98700-110">**SMC-ügyfelek**– Ez a propensitásletöltésben található ügyfelek teljes száma.</span><span class="sxs-lookup"><span data-stu-id="98700-110">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="98700-111">Az ügyfeleket a rekordpartner azonosítja.</span><span class="sxs-lookup"><span data-stu-id="98700-111">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="98700-112">**Szerződések lejárata**– Az aktuális pénzügyi évben meg kell adtunk a lejáró szerződések számát.</span><span class="sxs-lookup"><span data-stu-id="98700-112">**Expire Agreements**– Within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="98700-113">Open Expiring Revenue (Nyitott **lejáró bevétel)**– A nyitott lejáró szerződésekhez kapcsolódó bevétel.</span><span class="sxs-lookup"><span data-stu-id="98700-113">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/insights/customer-opportunity-1.png" alt-text="Képernyőkép az Ügyfelek lehetőségek összegzése irányítópultról.":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="98700-115">CloudAscent SMB-szegmentálás</span><span class="sxs-lookup"><span data-stu-id="98700-115">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="98700-116">A kis- és középvállalati (SMB) szegmens három különálló alszegmensre oszlik.</span><span class="sxs-lookup"><span data-stu-id="98700-116">The small to medium business (SMB) segment is divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="98700-117">**A leggyakoribb nem nem használt ügyfelek** közé tartozik a legnagyobb SMB-ügyfelek, akik a legtöbb lehetőséget kínálják a Microsoft számára.</span><span class="sxs-lookup"><span data-stu-id="98700-117">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="98700-118">A tipikus nem felügyelt ügyfelek hasonló jellemzőkkel rendelkeznek, mint a felügyelt fiókok, sok alkalmazottal, nagy mennyiségű it-költségvetéssel és kiadással, valamint nagy mennyiségű potenciális bevétellel a Microsoft számára.</span><span class="sxs-lookup"><span data-stu-id="98700-118">Typical Top Unmanaged customers share similar characteristics to Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="98700-119">A Nem felső szintű nem hatót kétféleképpen definiáljuk:</span><span class="sxs-lookup"><span data-stu-id="98700-119">We define Top Unmanaged in two ways:</span></span>

   - <span data-ttu-id="98700-120">**A legkorrektebb** felhasználóalapú – 300 vagy több alkalmazottal rendelkező fiókokat tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="98700-120">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="98700-121">User-Based fiókok kiváló célok az első vásárláshoz vagy a felhasználóalapú előfizetési termékek, például a Microsoft 365, a Dynamics 365 vagy a Surface bővítéséhez.</span><span class="sxs-lookup"><span data-stu-id="98700-121">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as Microsoft 365, Dynamics 365, or Surface.</span></span>
   - <span data-ttu-id="98700-122">**Top Unmanaged Compute Based** –, amely 10 ezer dollárnál nagyobb Azure-beli potenciális fiókokat tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="98700-122">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="98700-123">A számítási alapú fiókok tartalmazzák a meglévő Azure-t.</span><span class="sxs-lookup"><span data-stu-id="98700-123">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="98700-124">a jelentős jövő évi potenciális fiókokkal és olyan fiókokkal, amelyek még nem vásárolják meg az Azure-t, de 10 ezer dollárnál nagyobbak az Azure-ra vonatkozó lehetőségeik.</span><span class="sxs-lookup"><span data-stu-id="98700-124">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="98700-125">**A Medium Business** a meglévő ügyfeleket és a 25–300 alkalmazottal rendelkező potenciális ügyfeleket tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="98700-125">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="98700-126">**A kisvállalatok** 10–25 alkalmazottal dolgozó vállalkozásokat foglalnak magába.</span><span class="sxs-lookup"><span data-stu-id="98700-126">**Small Business** includes businesses with 10-25 employees.</span></span>

4. <span data-ttu-id="98700-127">**A Nagyon kisvállalatok** 1–9 alkalmazottal dolgozó vállalkozásokat foglalnak magába.</span><span class="sxs-lookup"><span data-stu-id="98700-127">**Very Small Business** includes businesses with 1-9 employees.</span></span>

:::image type="content" source="images/insights/customer-opportunity-2.png" alt-text="Ügyfél SMC-típus szerint.":::

<span data-ttu-id="98700-129">**A nem és**  a közepes üzleti alszegetmények a Microsoft és a Microsoft partnerei számára jelentős élettartamú (LTV) ügyfeleket képviselnek.</span><span class="sxs-lookup"><span data-stu-id="98700-129">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="98700-130">Emiatt ezek a szegmensek a növekedést hajtó fő területek.</span><span class="sxs-lookup"><span data-stu-id="98700-130">Because of this, they're the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="98700-131">Ebben a két alszegegben jobb helyzetben vagyunk, hogy a szoftvercsatornát az Microsoft 365-val szerezjük be, további bevételt szerezünk a D365/Azure üzletági (LOB) alkalmazásokkal, és magas LTV-t szeretnénk megvalósítani a Microsoft számára.</span><span class="sxs-lookup"><span data-stu-id="98700-131">In these two subsegments, we're better positioned to acquire the socket with Microsoft 365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="98700-132">Jelenleg két fő lehetőségünk van: 1.</span><span class="sxs-lookup"><span data-stu-id="98700-132">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="98700-133">az ügyfél növekedést ad hozzá; 2.</span><span class="sxs-lookup"><span data-stu-id="98700-133">our customer adds growth; 2.</span></span> <span data-ttu-id="98700-134">míg a felhőbeli szoftvercsatornákat jól Microsoft 365, a Dynamics 365-ben és az Azure-ban nagy lehetőségünk van.</span><span class="sxs-lookup"><span data-stu-id="98700-134">while we do well acquiring cloud sockets leading with Microsoft 365, we have a large opportunity in Dynamics 365 and Azure.</span></span>

<span data-ttu-id="98700-135">Az alábbi képernyőkép a négy SMB-alszegmentet ábrázolja.</span><span class="sxs-lookup"><span data-stu-id="98700-135">The following screenshot represents the four SMB Subsegments.</span></span> <span data-ttu-id="98700-136">A CloudAscent rangsorolnia kell az összes legfontosabb nem nem és közepes üzleti fiók profilkészítését, pontozását és modellezését.</span><span class="sxs-lookup"><span data-stu-id="98700-136">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/insights/customer-opportunity-3.png" alt-text="Az SMB-alszegmentek képernyőképe.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="98700-138">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="98700-138">CloudAscent Machine Learning</span></span>

<span data-ttu-id="98700-139">Az SMB gépi tanulási technológiával használja az értékesítési és marketing ügyfél-előrejelzéseket a nem használt és közepes üzleti szegmensben.</span><span class="sxs-lookup"><span data-stu-id="98700-139">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="98700-140">Hogyan gyűjti és váltja fel a jeleket a propensitásra vonatkozó javaslatokké?</span><span class="sxs-lookup"><span data-stu-id="98700-140">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="98700-141">**Adatgyűjtés:** A webbejárási webbejárások több milliárd ügyféljelet vizsgálnak és gyűjtenek a vállalati tartományok pingelése, a blogbejegyzések figyelése, a kiadások, a közösségi streamek és a technikai fórumok segítségével.</span><span class="sxs-lookup"><span data-stu-id="98700-141">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="98700-142">Az összegyűjtött jelek mellett a firmographics információkat belső és külső forrásokból is gyűjti a rendszer, például a D&B, a Microsoft belső előfizetési és tranzakciós adataiból.</span><span class="sxs-lookup"><span data-stu-id="98700-142">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="98700-143">**Machine Learning:** A jelek be vannak állítva a gépi tanulási modellbe, amely az értékesítési és marketing-előrejelzések strukturált adatkészletét adja ki minden ügyfél számára felhőalapú termék és fürt alapján.</span><span class="sxs-lookup"><span data-stu-id="98700-143">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="98700-144">Minden ügyfél pontozása a Microsoft legfelső szintű SMB-hez hasonló modellel van pontozással, amely meghatározza az ügyfél illeszkedési algoritmusát, valamint az ügyfél online viselkedését integráló gépi tanulási algoritmusokat szándékként definiálja.</span><span class="sxs-lookup"><span data-stu-id="98700-144">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="98700-145">A pontozás olyan fürtökbe van egyesülve, amelyek megmutatják, hogy az ügyfél nem hajlandó Microsoft Cloud-termékeket vásárolni.</span><span class="sxs-lookup"><span data-stu-id="98700-145">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="98700-146">**Optimalizálás:** A Machine Learning rendszer optimalizálja a modelleket a tranzakciós adatok havi és az előfizetési adatok negyedévente való fogyasztásával.</span><span class="sxs-lookup"><span data-stu-id="98700-146">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="98700-147">A nyerés/veszteség adatok használatával a Machine Learning beállítja az algoritmusokat, és ellenőrzi, hogy a modellek a várt módon működnek-e a fürtre vonatkozó javaslatok és az MSX-hez használt lehetőségek összehasonlításával.</span><span class="sxs-lookup"><span data-stu-id="98700-147">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/insights/customer-opportunity-4.png" alt-text="Képernyőkép az SMB gépi tanulásról.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="98700-149">CloudAscent Propensity</span><span class="sxs-lookup"><span data-stu-id="98700-149">CloudAscent Propensity</span></span>

<span data-ttu-id="98700-150">Hogyan jön létre a propensitási javaslatok létrehozása?</span><span class="sxs-lookup"><span data-stu-id="98700-150">How are propensity recommendations created?</span></span>

<span data-ttu-id="98700-151">A webes webbejárási eszközök és a különböző forrásokból származó adatok alapján gyűjtött jelek használatával konszolidáljuk a céges adatokat és az ügyfél közösségimédia-jeleit.</span><span class="sxs-lookup"><span data-stu-id="98700-151">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="98700-152">A pontozás ezeket a jeleket és adatokat használja összehasonlítási modellekben a szándékok illesztési és pontozási modelljeihez.</span><span class="sxs-lookup"><span data-stu-id="98700-152">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="98700-153">Ügyfélfiók illeszkedés</span><span class="sxs-lookup"><span data-stu-id="98700-153">Customer Account Fit</span></span>

   - <span data-ttu-id="98700-154">Belső és külső adatpontok, amelyek a céges adatokat határozzák meg.</span><span class="sxs-lookup"><span data-stu-id="98700-154">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="98700-155">A pontozás a legjobb SMB-hez hasonló modellt használ az ügyfelek összehasonlítására, és annak összehasonlítása érdekében, hogy azok megfelelőek-e a Microsoft Cloud-termékekhez.</span><span class="sxs-lookup"><span data-stu-id="98700-155">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="98700-156">A illeszkedés pontozása negyedévente frissül</span><span class="sxs-lookup"><span data-stu-id="98700-156">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="98700-157">Ügyfélfiók szándéka</span><span class="sxs-lookup"><span data-stu-id="98700-157">Customer Account Intent</span></span>

   - <span data-ttu-id="98700-158">A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot.</span><span class="sxs-lookup"><span data-stu-id="98700-158">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="98700-159">A szándékpontozás felül illeszkedik a fürtök meghatározásához.</span><span class="sxs-lookup"><span data-stu-id="98700-159">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="98700-160">A szándékpontozás havonta frissül.</span><span class="sxs-lookup"><span data-stu-id="98700-160">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/insights/customer-opportunity-5.png" alt-text="CloudAscent SMB prediktív modellek.":::

3. <span data-ttu-id="98700-162">Fürtözés</span><span class="sxs-lookup"><span data-stu-id="98700-162">Clustering</span></span>

   <span data-ttu-id="98700-163">Az illeszkedés és a szándék jelzése egy fürtözési pontszámba van összevonva.</span><span class="sxs-lookup"><span data-stu-id="98700-163">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="98700-164">A CloudAscent négy fürtből rendelkezik:</span><span class="sxs-lookup"><span data-stu-id="98700-164">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="98700-165">Act Now – értékesítésre kész ügyfelek</span><span class="sxs-lookup"><span data-stu-id="98700-165">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="98700-166">Értékelés – marketingre kész ügyfelek</span><span class="sxs-lookup"><span data-stu-id="98700-166">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="98700-167">Figyelemfelkeltő kampányok</span><span class="sxs-lookup"><span data-stu-id="98700-167">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="98700-168">Oktatás – a szándék oktatása és figyelése</span><span class="sxs-lookup"><span data-stu-id="98700-168">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="98700-169">A fürtözés lehetővé teszi, hogy a felhasználók adott ügyfeleket célozzanak meg értékesítési és marketinges kezdeményezésekhez olyan szegmenstényezők alapján, mint például a termék, a földrajzi hely, az iparág és a vertikális.</span><span class="sxs-lookup"><span data-stu-id="98700-169">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="98700-170">A CloudAscent-munkafüzetek **Propensity Model (Propensity-modell)** lapja a propensitást és a becsült térbeli bevételt osztja meg.</span><span class="sxs-lookup"><span data-stu-id="98700-170">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="98700-171">Az illeszkedés és a szándék fürtözésének meghatározásához a következő lépéseket kell végigmenni:</span><span class="sxs-lookup"><span data-stu-id="98700-171">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="98700-172">A ML modellek használatával először 100-as skálán számítjuk ki a Customer Fit Score (Ügyfél illesztési pontszáma) és a intent Score (szándék pontszáma) értékeket.</span><span class="sxs-lookup"><span data-stu-id="98700-172">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="98700-173">A pontos pontszámok a modelltől függően ML változhatnak.</span><span class="sxs-lookup"><span data-stu-id="98700-173">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="98700-174">Példa pontszámok alább:</span><span class="sxs-lookup"><span data-stu-id="98700-174">Example Scores Below:</span></span>

         |<span data-ttu-id="98700-175">**Osztályozás**</span><span class="sxs-lookup"><span data-stu-id="98700-175">**Classification**</span></span>|<span data-ttu-id="98700-176">**Pontszám**</span><span class="sxs-lookup"><span data-stu-id="98700-176">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="98700-177">Magas</span><span class="sxs-lookup"><span data-stu-id="98700-177">High</span></span>|<span data-ttu-id="98700-178">75 - 100</span><span class="sxs-lookup"><span data-stu-id="98700-178">75 - 100</span></span>|
         |<span data-ttu-id="98700-179">Közepes</span><span class="sxs-lookup"><span data-stu-id="98700-179">Medium</span></span>|<span data-ttu-id="98700-180">55 - 74</span><span class="sxs-lookup"><span data-stu-id="98700-180">55 - 74</span></span>|
         |<span data-ttu-id="98700-181">Alacsony</span><span class="sxs-lookup"><span data-stu-id="98700-181">Low</span></span>|<span data-ttu-id="98700-182">30 - 54</span><span class="sxs-lookup"><span data-stu-id="98700-182">30 - 54</span></span>|
         |<span data-ttu-id="98700-183">Nagyon alacsony</span><span class="sxs-lookup"><span data-stu-id="98700-183">Very Low</span></span>|<span data-ttu-id="98700-184">0 - 29</span><span class="sxs-lookup"><span data-stu-id="98700-184">0 - 29</span></span>|

      2. <span data-ttu-id="98700-185">A fenti szabályt használva a vállalatokat magas, közepes, alacsony és nagyon alacsony besorolásúként soroljuk be mind az Ügyfél illeszkedési, mind a Szándékjelzők esetében.</span><span class="sxs-lookup"><span data-stu-id="98700-185">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit and Intent Signals.</span></span>

      3. <span data-ttu-id="98700-186">Az ügyfelek illeszkedési és szándékjeleit egy 2D-s mátrixon ábrázoljuk, és az egyes metszetek a szándékot jelképezik.</span><span class="sxs-lookup"><span data-stu-id="98700-186">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span> <span data-ttu-id="98700-187">Például: Magas illeszkedés + Magas szándék = A1, amely a legnagyobb propensitást képviseli.</span><span class="sxs-lookup"><span data-stu-id="98700-187">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="98700-188">Végül ezek a szegmensek csoportosítva alkotnak fürtöt.</span><span class="sxs-lookup"><span data-stu-id="98700-188">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="98700-189">Például az A1, A2, A3, A4 az Act Now fürtöt alkotják.</span><span class="sxs-lookup"><span data-stu-id="98700-189">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/insights/customer-opportunity-6.png" alt-text="CloudAscent-modellek.":::

   <span data-ttu-id="98700-191">Javasoljuk, hogy ezeknél az ügyfeleknél az Act Now (Most járjon el) és a Evaluate customers (Ügyfelek kiértékelése) célcsoportot célozza meg.</span><span class="sxs-lookup"><span data-stu-id="98700-191">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="98700-192">CloudAscent-termékek & modellek</span><span class="sxs-lookup"><span data-stu-id="98700-192">CloudAscent Products & Models</span></span>

<span data-ttu-id="98700-193">Az alábbi ábra a CloudAscent szolgáltatáson belüli egyes támogatói modelleket tartalmazza:</span><span class="sxs-lookup"><span data-stu-id="98700-193">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/insights/customer-opportunity-7.png" alt-text="CloudAscent propensity modell.":::

<span data-ttu-id="98700-195">A téreltérmodellek olyan meglévő Microsoft-ügyfelek előrejelzései, akik nem tartalmaznak terméket, és/vagy nettó új potenciális ügyfelek.</span><span class="sxs-lookup"><span data-stu-id="98700-195">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="98700-196">Az upsell modellek tranzakciós adatok használatával jelezik előre az Azure-beli és a Microsoft 365 potenciálisan várható szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="98700-196">Upsell models use transaction data to predict the potential for upsell in Azure and Microsoft 365 SKUs.</span></span>

<span data-ttu-id="98700-197">Ezek az ügyfelek már az Azure-ral vagy a Microsoft 365 is rendelkezik, és az upsell modell azt mutatja, hogy valószínűleg többet fognak vásárolni a meglévő termékváltozatukból.</span><span class="sxs-lookup"><span data-stu-id="98700-197">These customers will already have both Azure or Microsoft 365 and the upsell model shows that they’re likely to purchase more of their existing SKU.</span></span>

<span data-ttu-id="98700-198">Az EOS a Win 7, Office 2010, SQL Server és Windows ügyfeleket is megosztja.</span><span class="sxs-lookup"><span data-stu-id="98700-198">EOS shares the end of service (EOS) customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="98700-199">Az EOS-adatokat a rendszer lekérte az MS Sales szolgáltatásból, és átfedi őket a CloudAscent propensity modellel, ha elérhető.</span><span class="sxs-lookup"><span data-stu-id="98700-199">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="98700-200">Az EOS-adatok a Modern Workben és az Azure Salesben játszódnak.</span><span class="sxs-lookup"><span data-stu-id="98700-200">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
