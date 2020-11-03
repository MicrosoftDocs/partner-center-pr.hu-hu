---
title: Office 365 E4-előfizetések migrálása
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A Microsoft Office 365 Enterprise E4 kiadása 2017. április 7-én megszűnik. Ismerje meg, hogyan telepítheti át az ügyfél-előfizetéseket az Office 365 újabb verzióira.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/03/2020
ms.locfileid: "92527966"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="f8960-104">Office 365 E4-előfizetések migrálása újabb Office 365-verziókba</span><span class="sxs-lookup"><span data-stu-id="f8960-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="f8960-105">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="f8960-105">**Applies to**</span></span>

-  <span data-ttu-id="f8960-106">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="f8960-106">Partner Center</span></span>

<span data-ttu-id="f8960-107">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="f8960-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="f8960-108">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="f8960-108">Global admin</span></span>
-   <span data-ttu-id="f8960-109">Felhasználói rendszergazda</span><span class="sxs-lookup"><span data-stu-id="f8960-109">User admin</span></span>
-   <span data-ttu-id="f8960-110">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="f8960-110">Admin agent</span></span>
-   <span data-ttu-id="f8960-111">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="f8960-111">Sales agent</span></span>

<span data-ttu-id="f8960-112">Az Office 365 Enterprise E4-csomag kivonásra kerül, amely 2017. április 7-én érvényes.</span><span class="sxs-lookup"><span data-stu-id="f8960-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="f8960-113">Ezen időpont után már nem vásárolhat új Office 365 E4-előfizetést, és a meglévő E4-előfizetések nem fognak automatikusan megújítani a lejárat után.</span><span class="sxs-lookup"><span data-stu-id="f8960-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="f8960-114">Az E4-előfizetések végén a rendszer megszakítja őket.</span><span class="sxs-lookup"><span data-stu-id="f8960-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="f8960-115">Az ügyfelek folytonosságának biztosítása érdekében az alábbi listában szereplő, az E4-előfizetésekkel rendelkező ügyfeleket egy támogatott SKU-ra kell áttérnie.</span><span class="sxs-lookup"><span data-stu-id="f8960-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="f8960-116">Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="f8960-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="f8960-117">Az Office 365 Enterprise E4 kereskedelmi és kormányzati SKU-t is kivonják.</span><span class="sxs-lookup"><span data-stu-id="f8960-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="f8960-118">Az előfizetés részletei lapon az E4 előfizetés állapota "lejár [date]" értékre módosult az "automatikus megújítások [date]" kifejezésből.</span><span class="sxs-lookup"><span data-stu-id="f8960-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="f8960-119">Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejárati előfizetéseket az előfizetés befejezési dátumának és az automatikus megújítás = hamis tulajdonságnak a kiértékelésével derítheti fel.</span><span class="sxs-lookup"><span data-stu-id="f8960-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="f8960-120">Az E4-előfizetések az automatikus megújítás = false értékre lesznek állítva 2017. április 7-én.</span><span class="sxs-lookup"><span data-stu-id="f8960-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="f8960-121">Az ügyfeleket bármikor át lehet helyezni egy új csomagba.</span><span class="sxs-lookup"><span data-stu-id="f8960-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="f8960-122">Office 365 Enterprise E4 kiadás-helyettesítési tervek</span><span class="sxs-lookup"><span data-stu-id="f8960-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="f8960-123">Dönthet úgy is, hogy az E4-es verzióval azonos funkciókat tart fenn, vagy az ügyfelek kihasználhatják az Office 365 és a Skype vállalati online verzió újabb funkcióit és funkcióit.</span><span class="sxs-lookup"><span data-stu-id="f8960-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="f8960-124">A díjszabással kapcsolatos részletek a partner Center árlista és ajánlatok listája mátrixában találhatók.</span><span class="sxs-lookup"><span data-stu-id="f8960-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="f8960-125">A biztonságos termék nagyvállalati E3 vagy a biztonságos produktív nagyvállalati E5 a következő, az Office 365 nagyvállalati E3 vagy Office 365 Enterprise E5 lehetőségekkel lehet helyettesíteni.</span><span class="sxs-lookup"><span data-stu-id="f8960-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="f8960-126">1. lehetőség: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="f8960-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="f8960-127">2. lehetőség: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="f8960-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="f8960-128">3. lehetőség: Office 365 Enterprise E3 + Skype for Business Plus CAL (ár és funkció paritása E4-vel)</span><span class="sxs-lookup"><span data-stu-id="f8960-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="f8960-129">4. lehetőség: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="f8960-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="f8960-130">Szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="f8960-130">Feature</span></span> | <span data-ttu-id="f8960-131">1\. lehetőség</span><span class="sxs-lookup"><span data-stu-id="f8960-131">Option 1</span></span> | <span data-ttu-id="f8960-132">2\. lehetőség</span><span class="sxs-lookup"><span data-stu-id="f8960-132">Option 2</span></span> | <span data-ttu-id="f8960-133">3. lehetőség</span><span class="sxs-lookup"><span data-stu-id="f8960-133">Option 3</span></span> | <span data-ttu-id="f8960-134">4. lehetőség</span><span class="sxs-lookup"><span data-stu-id="f8960-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="f8960-135">Az Office 365 nagyvállalati E4 csomag összes funkciójának beolvasása</span><span class="sxs-lookup"><span data-stu-id="f8960-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="f8960-136">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-136">Yes</span></span> | <span data-ttu-id="f8960-137">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-137">Yes</span></span> | <span data-ttu-id="f8960-138">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-138">Yes</span></span> | <span data-ttu-id="f8960-139">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-139">No</span></span> |
| <span data-ttu-id="f8960-140">Az Office 365-ben felügyelt telefonszámok</span><span class="sxs-lookup"><span data-stu-id="f8960-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="f8960-141">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-141">Yes</span></span> | <span data-ttu-id="f8960-142">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-142">Yes</span></span> | <span data-ttu-id="f8960-143">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-143">No</span></span> | <span data-ttu-id="f8960-144">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-144">No</span></span> |
| <span data-ttu-id="f8960-145">A telefonszámok a helyszínen és az Office 365-ben (hibrid üzembe helyezés) vannak kezelve?</span><span class="sxs-lookup"><span data-stu-id="f8960-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="f8960-146">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-146">Yes</span></span> | <span data-ttu-id="f8960-147">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-147">Yes</span></span> | <span data-ttu-id="f8960-148">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-148">No</span></span> | <span data-ttu-id="f8960-149">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-149">No</span></span> |
| <span data-ttu-id="f8960-150">Lehetősége van PSTN hanghívási terv hozzáadására?</span><span class="sxs-lookup"><span data-stu-id="f8960-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="f8960-151">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-151">Yes</span></span> | <span data-ttu-id="f8960-152">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-152">Yes</span></span> | <span data-ttu-id="f8960-153">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-153">No</span></span> | <span data-ttu-id="f8960-154">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-154">No</span></span> |
| <span data-ttu-id="f8960-155">PSTN-konferencia?</span><span class="sxs-lookup"><span data-stu-id="f8960-155">PSTN Conferencing?</span></span> | <span data-ttu-id="f8960-156">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-156">Yes</span></span> | <span data-ttu-id="f8960-157">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-157">No</span></span> | <span data-ttu-id="f8960-158">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-158">No</span></span> | <span data-ttu-id="f8960-159">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-159">No</span></span> |
| <span data-ttu-id="f8960-160">Speciális eszközök az együttműködéshez, az elemzéshez és a biztonsághoz?</span><span class="sxs-lookup"><span data-stu-id="f8960-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="f8960-161">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-161">Yes</span></span> | <span data-ttu-id="f8960-162">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-162">No</span></span> | <span data-ttu-id="f8960-163">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-163">No</span></span> | <span data-ttu-id="f8960-164">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-164">No</span></span> |
| <span data-ttu-id="f8960-165">Interaktív jelentések, irányítópultok és adatvizualizációk?</span><span class="sxs-lookup"><span data-stu-id="f8960-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="f8960-166">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-166">Yes</span></span> | <span data-ttu-id="f8960-167">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-167">No</span></span> | <span data-ttu-id="f8960-168">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-168">No</span></span> | <span data-ttu-id="f8960-169">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-169">No</span></span> | 
| <span data-ttu-id="f8960-170">Jobban kézben tarthatja az adatbiztonságot és a megfelelőséget a beépített adatvédelem, az átláthatóság és a kifinomult felhasználói vezérlők terén?</span><span class="sxs-lookup"><span data-stu-id="f8960-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="f8960-171">Igen</span><span class="sxs-lookup"><span data-stu-id="f8960-171">Yes</span></span> | <span data-ttu-id="f8960-172">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-172">No</span></span> | <span data-ttu-id="f8960-173">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-173">No</span></span> | <span data-ttu-id="f8960-174">Nem</span><span class="sxs-lookup"><span data-stu-id="f8960-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="f8960-175">Ügyfelek átváltása új termékekre</span><span class="sxs-lookup"><span data-stu-id="f8960-175">Transition customers to new product plans</span></span>

<span data-ttu-id="f8960-176">A Microsoft folyamatosan új termékeket és szolgáltatásokat kínál partnereinknek.</span><span class="sxs-lookup"><span data-stu-id="f8960-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="f8960-177">Ezekben az esetekben előfordulhat, hogy frissítenie kell az ügyfeleket az új szolgáltatásokra, vagy át kell telepítenie az előfizetéseket olyan SKU-ból, amely végül le lesz állítva.</span><span class="sxs-lookup"><span data-stu-id="f8960-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="f8960-178">Az ügyfelek áttelepítése a kivont SKU-ról újabb verzióra a következő lépések szükségesek:</span><span class="sxs-lookup"><span data-stu-id="f8960-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="f8960-179">Az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="f8960-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="f8960-180">Aktuális felhasználói licencek újbóli társítása</span><span class="sxs-lookup"><span data-stu-id="f8960-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="f8960-181">A régi előfizetés megszakítása</span><span class="sxs-lookup"><span data-stu-id="f8960-181">Cancel the old subscription</span></span>

<span data-ttu-id="f8960-182">Az alábbi lépéseket követve áttelepítheti az ügyfél Office 365 Enterprise E4-előfizetését a fenti táblázatban található egyik lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="f8960-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="f8960-183">1. lépés – az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="f8960-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="f8960-184">A **partner Center** menüben válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza az **előfizetések hozzáadása** elemet.</span><span class="sxs-lookup"><span data-stu-id="f8960-184">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Add subscriptions** .</span></span>

2. <span data-ttu-id="f8960-185">Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikét), adja meg a licencek számát, majd válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8960-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span>

   <span data-ttu-id="f8960-186">Az ügyfél most már rendelkezik a régi és az új előfizetéssel, a régi Office 365 Enterprise E4-előfizetéssel és az új "Target" előfizetéssel, például 1. lehetőség – Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="f8960-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="f8960-187">2. lépés – az ügyfél felhasználói licencének újbóli társítása</span><span class="sxs-lookup"><span data-stu-id="f8960-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="f8960-188">A **partner Center** menüben válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza a **felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8960-188">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Users and licenses** .</span></span> <span data-ttu-id="f8960-189">Megnyílik az ügyfél felhasználói és licencek lapja.</span><span class="sxs-lookup"><span data-stu-id="f8960-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="f8960-190">A felhasználói licencek ismételt hozzárendeléséhez válassza ki az újból hozzárendelni kívánt felhasználót, majd válassza a **licencek kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8960-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses** .</span></span>

3. <span data-ttu-id="f8960-191">A **licencek kezelése** lapon törölje az **Office 365 Enterprise E4** -licenc jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatási csomagot ahhoz az előfizetéshez, amelyet az ügyfél áthelyez.</span><span class="sxs-lookup"><span data-stu-id="f8960-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="f8960-192">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8960-192">Select **Submit** .</span></span> <span data-ttu-id="f8960-193">A megerősítést kérő lap felsorolja az új licenc-hozzárendeléseket.</span><span class="sxs-lookup"><span data-stu-id="f8960-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="f8960-194">Folytassa ugyanezeket a lépéseket minden más ügyfél-felhasználóval, akiknek licenc-hozzárendelésre van szükségük.</span><span class="sxs-lookup"><span data-stu-id="f8960-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="f8960-195">Miután áthelyezte a felhasználói licenceket az új szolgáltatásba, biztonságosan megszakíthatja a kivont előfizetést a felső szintű ügyfél szintjén.</span><span class="sxs-lookup"><span data-stu-id="f8960-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="f8960-196">3. lépés – a régi előfizetés megszakítása</span><span class="sxs-lookup"><span data-stu-id="f8960-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="f8960-197">A **partner Center** menüben válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8960-197">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="f8960-198">Válassza ki az áthelyezni kívánt ügyfelet, és válassza ki a megszüntetni kívánt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="f8960-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="f8960-199">Az előfizetés részletei lapon állítsa az előfizetés állapotát **felfüggesztve** értékre.</span><span class="sxs-lookup"><span data-stu-id="f8960-199">In the subscription details page, set the subscription status to **Suspended** .</span></span>

3. <span data-ttu-id="f8960-200">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8960-200">Select **Submit** .</span></span>

<span data-ttu-id="f8960-201">A régi előfizetés fel van függesztve, és az új előfizetés aktív.</span><span class="sxs-lookup"><span data-stu-id="f8960-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="f8960-202">A felfüggesztett előfizetés 120 nap elteltével automatikusan kiépítve lesz.</span><span class="sxs-lookup"><span data-stu-id="f8960-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="f8960-203">Az ügyfél nem számít fel további költséget a régi előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="f8960-203">The customer incurs no additional costs for the old subscription.</span></span>



 



