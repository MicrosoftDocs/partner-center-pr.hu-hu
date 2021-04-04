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
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132621"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="04df6-104">Office 365 E4-előfizetések migrálása újabb Office 365-verziókba</span><span class="sxs-lookup"><span data-stu-id="04df6-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="04df6-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="04df6-105">**Appropriate roles**</span></span>

- <span data-ttu-id="04df6-106">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="04df6-106">Global admin</span></span>
- <span data-ttu-id="04df6-107">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="04df6-107">User management admin</span></span>
- <span data-ttu-id="04df6-108">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="04df6-108">Admin agent</span></span>
- <span data-ttu-id="04df6-109">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="04df6-109">Sales agent</span></span>

<span data-ttu-id="04df6-110">Az Office 365 Enterprise E4-csomag kivonásra kerül, amely 2017. április 7-én érvényes.</span><span class="sxs-lookup"><span data-stu-id="04df6-110">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="04df6-111">Ezen időpont után már nem vásárolhat új Office 365 E4-előfizetést, és a meglévő E4-előfizetések nem fognak automatikusan megújítani a lejárat után.</span><span class="sxs-lookup"><span data-stu-id="04df6-111">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="04df6-112">Az E4-előfizetések végén a rendszer megszakítja őket.</span><span class="sxs-lookup"><span data-stu-id="04df6-112">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="04df6-113">Az ügyfelek folytonosságának biztosítása érdekében az alábbi listában szereplő, az E4-előfizetésekkel rendelkező ügyfeleket egy támogatott SKU-ra kell áttérnie.</span><span class="sxs-lookup"><span data-stu-id="04df6-113">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="04df6-114">Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="04df6-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="04df6-115">Az Office 365 Enterprise E4 kereskedelmi és kormányzati SKU-t is kivonják.</span><span class="sxs-lookup"><span data-stu-id="04df6-115">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="04df6-116">Az előfizetés részletei lapon az E4 előfizetés állapota "lejár [date]" értékre módosult az "automatikus megújítások [date]" kifejezésből.</span><span class="sxs-lookup"><span data-stu-id="04df6-116">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="04df6-117">Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejárati előfizetéseket az előfizetés befejezési dátumának és az automatikus megújítás = hamis tulajdonságnak a kiértékelésével derítheti fel.</span><span class="sxs-lookup"><span data-stu-id="04df6-117">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="04df6-118">Az E4-előfizetések az automatikus megújítás = false értékre lesznek állítva 2017. április 7-én.</span><span class="sxs-lookup"><span data-stu-id="04df6-118">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="04df6-119">Az ügyfeleket bármikor át lehet helyezni egy új csomagba.</span><span class="sxs-lookup"><span data-stu-id="04df6-119">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="04df6-120">Office 365 Enterprise E4 kiadás-helyettesítési tervek</span><span class="sxs-lookup"><span data-stu-id="04df6-120">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="04df6-121">Dönthet úgy is, hogy az E4-es verzióval azonos funkciókat tart fenn, vagy az ügyfelek kihasználhatják az Office 365 és a Skype vállalati online verzió újabb funkcióit és funkcióit.</span><span class="sxs-lookup"><span data-stu-id="04df6-121">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="04df6-122">A díjszabással kapcsolatos részletek a partner Center árlista és ajánlatok listája mátrixában találhatók.</span><span class="sxs-lookup"><span data-stu-id="04df6-122">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="04df6-123">A biztonságos termék nagyvállalati E3 vagy a biztonságos produktív nagyvállalati E5 a következő, az Office 365 nagyvállalati E3 vagy Office 365 Enterprise E5 lehetőségekkel lehet helyettesíteni.</span><span class="sxs-lookup"><span data-stu-id="04df6-123">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="04df6-124">1. lehetőség: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="04df6-124">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="04df6-125">2. lehetőség: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="04df6-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="04df6-126">3. lehetőség: Office 365 Enterprise E3 + Skype for Business Plus CAL (ár és funkció paritása E4-vel)</span><span class="sxs-lookup"><span data-stu-id="04df6-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="04df6-127">4. lehetőség: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="04df6-127">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="04df6-128">Szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="04df6-128">Feature</span></span> | <span data-ttu-id="04df6-129">1\. lehetőség</span><span class="sxs-lookup"><span data-stu-id="04df6-129">Option 1</span></span> | <span data-ttu-id="04df6-130">2\. lehetőség</span><span class="sxs-lookup"><span data-stu-id="04df6-130">Option 2</span></span> | <span data-ttu-id="04df6-131">3. lehetőség</span><span class="sxs-lookup"><span data-stu-id="04df6-131">Option 3</span></span> | <span data-ttu-id="04df6-132">4. lehetőség</span><span class="sxs-lookup"><span data-stu-id="04df6-132">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="04df6-133">Az Office 365 nagyvállalati E4 csomag összes funkciójának beolvasása</span><span class="sxs-lookup"><span data-stu-id="04df6-133">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="04df6-134">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-134">Yes</span></span> | <span data-ttu-id="04df6-135">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-135">Yes</span></span> | <span data-ttu-id="04df6-136">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-136">Yes</span></span> | <span data-ttu-id="04df6-137">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-137">No</span></span> |
| <span data-ttu-id="04df6-138">Az Office 365-ben felügyelt telefonszámok</span><span class="sxs-lookup"><span data-stu-id="04df6-138">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="04df6-139">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-139">Yes</span></span> | <span data-ttu-id="04df6-140">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-140">Yes</span></span> | <span data-ttu-id="04df6-141">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-141">No</span></span> | <span data-ttu-id="04df6-142">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-142">No</span></span> |
| <span data-ttu-id="04df6-143">A telefonszámok a helyszínen és az Office 365-ben (hibrid üzembe helyezés) vannak kezelve?</span><span class="sxs-lookup"><span data-stu-id="04df6-143">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="04df6-144">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-144">Yes</span></span> | <span data-ttu-id="04df6-145">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-145">Yes</span></span> | <span data-ttu-id="04df6-146">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-146">No</span></span> | <span data-ttu-id="04df6-147">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-147">No</span></span> |
| <span data-ttu-id="04df6-148">Lehetősége van PSTN hanghívási terv hozzáadására?</span><span class="sxs-lookup"><span data-stu-id="04df6-148">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="04df6-149">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-149">Yes</span></span> | <span data-ttu-id="04df6-150">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-150">Yes</span></span> | <span data-ttu-id="04df6-151">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-151">No</span></span> | <span data-ttu-id="04df6-152">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-152">No</span></span> |
| <span data-ttu-id="04df6-153">PSTN-konferencia?</span><span class="sxs-lookup"><span data-stu-id="04df6-153">PSTN Conferencing?</span></span> | <span data-ttu-id="04df6-154">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-154">Yes</span></span> | <span data-ttu-id="04df6-155">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-155">No</span></span> | <span data-ttu-id="04df6-156">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-156">No</span></span> | <span data-ttu-id="04df6-157">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-157">No</span></span> |
| <span data-ttu-id="04df6-158">Speciális eszközök az együttműködéshez, az elemzéshez és a biztonsághoz?</span><span class="sxs-lookup"><span data-stu-id="04df6-158">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="04df6-159">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-159">Yes</span></span> | <span data-ttu-id="04df6-160">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-160">No</span></span> | <span data-ttu-id="04df6-161">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-161">No</span></span> | <span data-ttu-id="04df6-162">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-162">No</span></span> |
| <span data-ttu-id="04df6-163">Interaktív jelentések, irányítópultok és adatvizualizációk?</span><span class="sxs-lookup"><span data-stu-id="04df6-163">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="04df6-164">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-164">Yes</span></span> | <span data-ttu-id="04df6-165">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-165">No</span></span> | <span data-ttu-id="04df6-166">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-166">No</span></span> | <span data-ttu-id="04df6-167">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-167">No</span></span> | 
| <span data-ttu-id="04df6-168">Jobban kézben tarthatja az adatbiztonságot és a megfelelőséget a beépített adatvédelem, az átláthatóság és a kifinomult felhasználói vezérlők terén?</span><span class="sxs-lookup"><span data-stu-id="04df6-168">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="04df6-169">Igen</span><span class="sxs-lookup"><span data-stu-id="04df6-169">Yes</span></span> | <span data-ttu-id="04df6-170">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-170">No</span></span> | <span data-ttu-id="04df6-171">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-171">No</span></span> | <span data-ttu-id="04df6-172">Nem</span><span class="sxs-lookup"><span data-stu-id="04df6-172">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="04df6-173">Ügyfelek átváltása új termékekre</span><span class="sxs-lookup"><span data-stu-id="04df6-173">Transition customers to new product plans</span></span>

<span data-ttu-id="04df6-174">A Microsoft folyamatosan új termékeket és szolgáltatásokat kínál partnereinknek.</span><span class="sxs-lookup"><span data-stu-id="04df6-174">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="04df6-175">Ezekben az esetekben előfordulhat, hogy frissítenie kell az ügyfeleket az új szolgáltatásokra, vagy át kell telepítenie az előfizetéseket olyan SKU-ból, amely végül le lesz állítva.</span><span class="sxs-lookup"><span data-stu-id="04df6-175">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="04df6-176">Az ügyfelek áttelepítése a kivont SKU-ról újabb verzióra a következő lépések szükségesek:</span><span class="sxs-lookup"><span data-stu-id="04df6-176">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="04df6-177">Az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="04df6-177">Purchase the new subscription</span></span>
-   <span data-ttu-id="04df6-178">Aktuális felhasználói licencek újbóli társítása</span><span class="sxs-lookup"><span data-stu-id="04df6-178">Reassign current user licenses</span></span>
-   <span data-ttu-id="04df6-179">A régi előfizetés megszakítása</span><span class="sxs-lookup"><span data-stu-id="04df6-179">Cancel the old subscription</span></span>

<span data-ttu-id="04df6-180">Az alábbi lépéseket követve áttelepítheti az ügyfél Office 365 Enterprise E4-előfizetését a fenti táblázatban található egyik lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="04df6-180">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="04df6-181">1. lépés – az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="04df6-181">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="04df6-182">A **partner Center** menüben válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza az **előfizetések hozzáadása** elemet.</span><span class="sxs-lookup"><span data-stu-id="04df6-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="04df6-183">Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikét), adja meg a licencek számát, majd válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04df6-183">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="04df6-184">Az ügyfél most már rendelkezik a régi és az új előfizetéssel, a régi Office 365 Enterprise E4-előfizetéssel és az új "Target" előfizetéssel, például 1. lehetőség – Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="04df6-184">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="04df6-185">2. lépés – az ügyfél felhasználói licencének újbóli társítása</span><span class="sxs-lookup"><span data-stu-id="04df6-185">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="04df6-186">A **partner Center** menüben válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza a **felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04df6-186">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="04df6-187">Megnyílik az ügyfél felhasználói és licencek lapja.</span><span class="sxs-lookup"><span data-stu-id="04df6-187">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="04df6-188">A felhasználói licencek újbóli hozzárendeléséhez válassza ki az újból hozzárendelni kívánt felhasználót, majd válassza a **licencek kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04df6-188">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="04df6-189">A **licencek kezelése** lapon törölje az **Office 365 Enterprise E4** -licenc jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatási csomagot ahhoz az előfizetéshez, amelyet az ügyfél áthelyez.</span><span class="sxs-lookup"><span data-stu-id="04df6-189">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="04df6-190">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04df6-190">Select **Submit**.</span></span> <span data-ttu-id="04df6-191">A megerősítést kérő lap felsorolja az új licenc-hozzárendeléseket.</span><span class="sxs-lookup"><span data-stu-id="04df6-191">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="04df6-192">Folytassa ugyanezeket a lépéseket minden más ügyfél-felhasználóval, akiknek licenc-hozzárendelésre van szükségük.</span><span class="sxs-lookup"><span data-stu-id="04df6-192">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="04df6-193">Miután áthelyezte a felhasználói licenceket az új szolgáltatásba, biztonságosan megszakíthatja a kivont előfizetést a felső szintű ügyfél szintjén.</span><span class="sxs-lookup"><span data-stu-id="04df6-193">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="04df6-194">3. lépés – a régi előfizetés megszakítása</span><span class="sxs-lookup"><span data-stu-id="04df6-194">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="04df6-195">A **partner Center** menüben válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04df6-195">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="04df6-196">Válassza ki az áthelyezni kívánt ügyfelet, és válassza ki a megszüntetni kívánt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="04df6-196">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="04df6-197">Az előfizetés részletei lapon állítsa az előfizetés állapotát **felfüggesztve** értékre.</span><span class="sxs-lookup"><span data-stu-id="04df6-197">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="04df6-198">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04df6-198">Select **Submit**.</span></span>

<span data-ttu-id="04df6-199">A régi előfizetés fel van függesztve, és az új előfizetés aktív.</span><span class="sxs-lookup"><span data-stu-id="04df6-199">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="04df6-200">A felfüggesztett előfizetés 120 nap elteltével automatikusan kiépítve lesz.</span><span class="sxs-lookup"><span data-stu-id="04df6-200">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="04df6-201">Az ügyfél nem számít fel további költséget a régi előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="04df6-201">The customer incurs no additional costs for the old subscription.</span></span>



 



