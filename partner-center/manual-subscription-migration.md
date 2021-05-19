---
title: Minősített Dynamics 365-előfizetések áttelepítése
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Útmutató minősített, alapszintű Dynamics 365-előfizetések új előfizetésre való áttelepítéséhez a meglévő előfizetések lejárta előtt.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151644"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="664c4-103">A Dynamics 365 és a Customer Engagement Plan migrálása az Alapszintű szolgáltatásról (arra jogosult ajánlatokról) újabb verziókra</span><span class="sxs-lookup"><span data-stu-id="664c4-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="664c4-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Rendszergazdai ügynök | Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="664c4-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="664c4-105">2019. január 1-jén az alapszintű (minősített ajánlatok) előfizetéssel rendelkező Dynamics 365 for Sales/Customer Engagement-csomaggal rendelkező ügyfelek már nem újíthatja meg ezeket az örökölt ajánlatokat; A meglévő előfizetések nem újulnak meg automatikusan a lejáratukkor.</span><span class="sxs-lookup"><span data-stu-id="664c4-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="664c4-106">Az előfizetés részleteinek oldalán az előfizetés állapota "Lejárat dátuma[dátum]" lesz az "Automatikus megújítás [dátum]" alatt.</span><span class="sxs-lookup"><span data-stu-id="664c4-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="664c4-107">Az ügyfelek folytonosságának biztosítása érdekében érdemes a lejáró előfizetéseket egy támogatott lehetőségre átemálni, az alábbiakban felsoroltak szerint.</span><span class="sxs-lookup"><span data-stu-id="664c4-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="664c4-108">Javasoljuk, hogy az ügyfeleket az előfizetés éves záró dátuma előtt új előfizetésekbe költöztetjék, hogy elkerülje az ügyfelek szolgáltatáskimaradását.</span><span class="sxs-lookup"><span data-stu-id="664c4-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="664c4-109">Ha az API-t használja (CREST vagy Partnerközpont), a lejáró előfizetéseket az előfizetés záró dátumának és az automatikus megújítás = Hamis tulajdonság kiértékelésével találhatja meg.</span><span class="sxs-lookup"><span data-stu-id="664c4-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="664c4-110">A kérdéses előfizetések 2019. január 1-jén automatikus renew=False (automatikus megújítás=Hamis) beállításra lesznek beállítva.</span><span class="sxs-lookup"><span data-stu-id="664c4-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="664c4-111">Az ügyfeleket bármikor áthelyezheti egy új csomagba.</span><span class="sxs-lookup"><span data-stu-id="664c4-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="664c4-112">A Dynamics 365-ajánlatok kivezetve</span><span class="sxs-lookup"><span data-stu-id="664c4-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="664c4-113">Dynamics 365 for Sales Enterprise kiadás CRMOL Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-114">Dynamics 365 for Sales Enterprise kiadás CRMOL Basic (minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="664c4-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="664c4-115">Dynamics 365 for Sales Enterprise kiadás CRMOL Basic (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="664c4-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="664c4-116">Dynamics 365 for Sales Enterprise kiadás (kormányzati díjszabás) CRMOL Alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-117">Dynamics 365 for Sales Enterprise kiadás Az SA for CRM Basicből (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-118">Dynamics 365 for Sales Enterprise kiadás From SA for CRM Basic (Minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="664c4-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="664c4-119">Dynamics 365 for Sales Enterprise kiadás From SA for CRM Basic (Minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="664c4-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="664c4-120">Dynamics 365 for Sales Enterprise kiadás (government pricing) From SA for CRM Basic (Minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-121">Dynamics 365 for Sales Enterprise kiadás Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-122">Dynamics 365 for Sales Enterprise kiadás Add-On for CRM Basic (minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="664c4-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="664c4-123">Dynamics 365 for Sales Enterprise kiadás Add-On for CRM Basic (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="664c4-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="664c4-124">Dynamics 365 for Sales Enterprise kiadás (government pricing) Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-125">Dynamics 365 Customer Engagement-csomag Enterprise kiadás CRMOL Alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-126">Dynamics 365 Customer Engagement Plan Enterprise kiadás (kormányzati díjszabás) CRMOL Alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-127">Dynamics 365 Customer Engagement-csomag Enterprise kiadás CRMOL Alapszintű (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="664c4-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="664c4-128">Dynamics 365 Customer Engagement-Enterprise kiadás CRMOL Alapszintű (minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="664c4-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="664c4-129">Dynamics 365 Customer Engagement csomag Enterprise kiadás AZ SA for CRM Basicből (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-130">Dynamics 365 Customer Engagement Plan Enterprise kiadás (government pricing) From SA for CRM Basic (Minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-131">Dynamics 365 Customer Engagement plan Enterprise kiadás From SA for CRM Basic (Minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="664c4-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="664c4-132">Dynamics 365 Customer Engagement plan Enterprise kiadás From SA for CRM Basic (Minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="664c4-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="664c4-133">Dynamics 365 Customer Engagement Plan Enterprise kiadás Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-134">Dynamics 365 Customer Engagement Plan Enterprise kiadás (government pricing) Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-135">Dynamics 365 Customer Engagement Plan Enterprise kiadás Add-On for CRM Basic (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="664c4-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="664c4-136">Dynamics 365 Customer Engagement plan Enterprise kiadás Add-On for CRM Basic (Minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="664c4-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="664c4-137">Dynamics 365 for Sales/ Customer Engagement-csomag alapszintű (minősített ajánlatok) helyettesítő csomagokból</span><span class="sxs-lookup"><span data-stu-id="664c4-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="664c4-138">**Visszavont ajánlatok**</span><span class="sxs-lookup"><span data-stu-id="664c4-138">**Retired offers**</span></span>   

- <span data-ttu-id="664c4-139">Dynamics 365 for Sales a CRM Basicből vagy a CRMOL Basicből (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="664c4-140">Dynamics 365 Customer Engagement-csomag a CRM Basicből vagy a CRMOL Basicből (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="664c4-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="664c4-141">**Cserebeállítások**</span><span class="sxs-lookup"><span data-stu-id="664c4-141">**Replacement options**</span></span>
- <span data-ttu-id="664c4-142">Dynamics 365 for Sales Professional (ÚJ)</span><span class="sxs-lookup"><span data-stu-id="664c4-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="664c4-143">Dynamics 365 for Sales Professional (ÚJ)</span><span class="sxs-lookup"><span data-stu-id="664c4-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="664c4-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="664c4-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="664c4-145">Dynamics 365 Customer Engagement-csomag vagy</span><span class="sxs-lookup"><span data-stu-id="664c4-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="664c4-146">Dynamics 365-csapattagok</span><span class="sxs-lookup"><span data-stu-id="664c4-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="664c4-147">Ügyfelek váltása új terméktervekre</span><span class="sxs-lookup"><span data-stu-id="664c4-147">Transition customers to new product plans</span></span>

<span data-ttu-id="664c4-148">Ha az ügyfeleket a visszavont SKUS-król újabbakra kívánja átemeltetni, a következő lépésekre van szükség ebben a sorrendben:</span><span class="sxs-lookup"><span data-stu-id="664c4-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="664c4-149">Az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="664c4-149">Purchase the new subscription</span></span>
- <span data-ttu-id="664c4-150">Aktuális felhasználói licencek ismételt hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="664c4-150">Reassign current user licenses</span></span>
- <span data-ttu-id="664c4-151">Régi előfizetés lemondása</span><span class="sxs-lookup"><span data-stu-id="664c4-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="664c4-152">Az új csomag vásárlása az ügyfél számára</span><span class="sxs-lookup"><span data-stu-id="664c4-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="664c4-153">A **bal oldali** navigációs sávon válassza az Ügyfelek lehetőséget, majd válassza ki az új előfizetésre áthelyezni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="664c4-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="664c4-154">Válassza **az Előfizetés hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="664c4-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="664c4-155">Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyike), adja meg a licencek számát, majd válassza a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="664c4-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="664c4-156">Az ügyfél most már a régi előfizetéssel és az új előfizetéssel is rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="664c4-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="664c4-157">A következő lépés a licencek ismételt hozzárendelése az ügyfél felhasználóihoz.</span><span class="sxs-lookup"><span data-stu-id="664c4-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="664c4-158">A **bal oldali** navigációs sávon válassza az Ügyfelek lehetőséget, majd válassza ki az ügyfelet, akinél az áthelyezést választja.</span><span class="sxs-lookup"><span data-stu-id="664c4-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="664c4-159">Válassza **a Felhasználók és licencek lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="664c4-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="664c4-160">Egy licenc felhasználóhoz való ismételt hozzárendeléséhez jelölje ki a felhasználót, majd válassza a **Licencek kezelése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="664c4-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="664c4-161">A **Licencek kezelése** lapon törölje a Dynamics 365 for Sales/Customer Engagement Plan from Basic (Minősített ajánlat) licenc jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatási tervet ahhoz az előfizetéshez, amelybe az ügyfél át lesz költözve.</span><span class="sxs-lookup"><span data-stu-id="664c4-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="664c4-162">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="664c4-162">Select **Submit**.</span></span> <span data-ttu-id="664c4-163">Ezt minden olyan felhasználóval meg kell tenni, akinek új licencre van szüksége.</span><span class="sxs-lookup"><span data-stu-id="664c4-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="664c4-164">Miután áthelyezte a licenceket az új előfizetésbe, megszüntetheti a régi előfizetést.</span><span class="sxs-lookup"><span data-stu-id="664c4-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="664c4-165">A **bal oldali navigációs** sávon válassza az Ügyfelek lehetőséget, majd válassza ki a költözni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="664c4-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="664c4-166">Az előfizetés részletei lapon állítsa a régi előfizetést Felfüggesztettre, majd **válassza** a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="664c4-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="664c4-167">A régi előfizetés most fel van függesztve, és az új előfizetés aktív.</span><span class="sxs-lookup"><span data-stu-id="664c4-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="664c4-168">A felfüggesztett előfizetés 120 nap után automatikusan fel lesz függesztve.</span><span class="sxs-lookup"><span data-stu-id="664c4-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="664c4-169">Az ügyfél nem jár többletköltségsel a régi előfizetésért.</span><span class="sxs-lookup"><span data-stu-id="664c4-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



