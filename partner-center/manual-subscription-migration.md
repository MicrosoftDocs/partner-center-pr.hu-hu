---
title: Minősített Dynamics 365-előfizetések migrálása
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan telepítheti át a minősített, alapszintű Dynamics 365-előfizetéseket egy új előfizetésre a meglévő előfizetések lejárta előtt.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/17/2020
ms.locfileid: "92528007"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="953d3-103">A Dynamics 365 és a Customer Engagement Plan migrálása az Alapszintű szolgáltatásról (arra jogosult ajánlatokról) újabb verziókra</span><span class="sxs-lookup"><span data-stu-id="953d3-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="953d3-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="953d3-104">**Applies to**</span></span>

-  <span data-ttu-id="953d3-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="953d3-105">Partner Center</span></span>

<span data-ttu-id="953d3-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="953d3-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="953d3-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="953d3-107">Global admin</span></span>
-   <span data-ttu-id="953d3-108">Felhasználói rendszergazda</span><span class="sxs-lookup"><span data-stu-id="953d3-108">User admin</span></span>
-   <span data-ttu-id="953d3-109">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="953d3-109">Admin agent</span></span>
-   <span data-ttu-id="953d3-110">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="953d3-110">Sales agent</span></span>

<span data-ttu-id="953d3-111">Az alapszintű (minősített ajánlatok) előfizetések által kínált, a Dynamics 365 for Sales/Customer engagements csomaggal rendelkező ügyfelek a továbbiakban nem tudják megújítani ezeket a régi ajánlatokat: 2019. január 1-től a meglévő előfizetések lejáratakor a rendszer nem újítja meg automatikusan.</span><span class="sxs-lookup"><span data-stu-id="953d3-111">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="953d3-112">Az előfizetés részleteit tartalmazó lapon az előfizetés állapota "lejár [date]" értékre változik a "automatikusan megújítva [date]" állapotból.</span><span class="sxs-lookup"><span data-stu-id="953d3-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="953d3-113">Az ügyfelek folytonosságának biztosítása érdekében az alább felsorolt támogatott lehetőségekre kell áttérnie a lejáró előfizetésekkel.</span><span class="sxs-lookup"><span data-stu-id="953d3-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="953d3-114">Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="953d3-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="953d3-115">Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejárati előfizetéseket az előfizetés befejezési dátumának és az automatikus megújítás = hamis tulajdonságnak a kiértékelésével érheti el.</span><span class="sxs-lookup"><span data-stu-id="953d3-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="953d3-116">A kérdéses előfizetések az automatikus megújítás = false értékre lesznek állítva, január 1-jén 2019.</span><span class="sxs-lookup"><span data-stu-id="953d3-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="953d3-117">Az ügyfeleket bármikor át lehet helyezni egy új csomagba.</span><span class="sxs-lookup"><span data-stu-id="953d3-117">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="953d3-118">A Dynamics 365-ajánlatok kivonulnak</span><span class="sxs-lookup"><span data-stu-id="953d3-118">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="953d3-119">Dynamics 365 for Sales Enterprise Edition CRMOL alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-120">Dynamics 365 for Sales Enterprise Edition CRMOL alapszintű (minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="953d3-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="953d3-121">Dynamics 365 for Sales Enterprise Edition CRMOL alapszintű (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="953d3-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="953d3-122">Dynamics 365 for Sales Enterprise Edition (kormányzati díjszabás) CRMOL alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-123">Dynamics 365 for Sales Enterprise Edition, SA for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-124">Dynamics 365 for Sales Enterprise Edition, SA for CRM alapszintű (minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="953d3-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="953d3-125">Dynamics 365 for Sales Enterprise Edition SA for CRM Basic (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="953d3-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="953d3-126">Dynamics 365 for Sales Enterprise Edition (kormányzati díjszabás) az SA-től a CRM alapszintű verzióra (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="953d3-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="953d3-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="953d3-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="953d3-130">Dynamics 365 for Sales Enterprise Edition (Government díjszabás) Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-130">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-131">Dynamics 365 Customer engagement Plan Enterprise Edition CRMOL alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-132">Dynamics 365 Customer engagement Plan Enterprise Edition (kormányzati díjszabás) CRMOL alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-133">Dynamics 365 Customer engagement Plan Enterprise Edition CRMOL alapszintű (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="953d3-133">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="953d3-134">Dynamics 365 Customer engagement Plan Enterprise Edition CRMOL alapszintű (minősített ajánlat) a kari</span><span class="sxs-lookup"><span data-stu-id="953d3-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="953d3-135">Dynamics 365 ügyfél-bevonási terv Enterprise Edition for SA a CRM alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-136">Dynamics 365 Customer engagement Plan Enterprise Edition (kormányzati díjszabás) from SA for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-137">Dynamics 365 ügyfél-bevonási terv Enterprise Edition for SA for CRM Basic (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="953d3-137">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="953d3-138">Dynamics 365 ügyfél-bevonási terv Enterprise Edition for SA for CRM alapszintű (minősített ajánlat) a kar számára</span><span class="sxs-lookup"><span data-stu-id="953d3-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="953d3-139">Dynamics 365 Customer engagement Plan Enterprise Edition Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-140">Dynamics 365 Customer engagement Plan Enterprise Edition (kormányzati díjszabás) Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="953d3-140">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-141">Dynamics 365 Customer engagement Plan Enterprise Edition Add-On a CRM alapszintű (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="953d3-141">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="953d3-142">Dynamics 365 Customer engagement Plan Enterprise Edition Add-On for CRM Basic (minősített ajánlat) a kari</span><span class="sxs-lookup"><span data-stu-id="953d3-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="953d3-143">Dynamics 365 for Sales/Customer bevonási terv az alapszintű (minősített ajánlatok) – helyettesítő csomagok</span><span class="sxs-lookup"><span data-stu-id="953d3-143">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="953d3-144">**Kivont ajánlatok**</span><span class="sxs-lookup"><span data-stu-id="953d3-144">**Retired offers**</span></span>   

- <span data-ttu-id="953d3-145">Dynamics 365 CRM alapszintű vagy CRMOL alapszintű (minősített ajánlat) értékesítéséhez</span><span class="sxs-lookup"><span data-stu-id="953d3-145">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="953d3-146">Dynamics 365 Customer engagement-terv a CRM Basic vagy a CRMOL alapszintű (minősített ajánlat) alapján</span><span class="sxs-lookup"><span data-stu-id="953d3-146">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="953d3-147">**Helyettesítő beállítások**</span><span class="sxs-lookup"><span data-stu-id="953d3-147">**Replacement options**</span></span>
- <span data-ttu-id="953d3-148">Dynamics 365 for Sales Professional (új)</span><span class="sxs-lookup"><span data-stu-id="953d3-148">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="953d3-149">Dynamics 365 for Sales Professional (új)</span><span class="sxs-lookup"><span data-stu-id="953d3-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="953d3-150">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="953d3-150">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="953d3-151">Dynamics 365 Customer engagement-csomag vagy</span><span class="sxs-lookup"><span data-stu-id="953d3-151">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="953d3-152">Dynamics 365-csapat tagjai</span><span class="sxs-lookup"><span data-stu-id="953d3-152">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="953d3-153">Ügyfelek átváltása új termékekre</span><span class="sxs-lookup"><span data-stu-id="953d3-153">Transition customers to new product plans</span></span>

<span data-ttu-id="953d3-154">A kivont SKU-ügyfelek újabb verzióra való áthelyezéséhez a következő lépések szükségesek ebben a sorrendben:</span><span class="sxs-lookup"><span data-stu-id="953d3-154">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="953d3-155">Az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="953d3-155">Purchase the new subscription</span></span>
- <span data-ttu-id="953d3-156">Aktuális felhasználói licencek újbóli társítása</span><span class="sxs-lookup"><span data-stu-id="953d3-156">Reassign current user licenses</span></span>
- <span data-ttu-id="953d3-157">Régi előfizetés megszakítása</span><span class="sxs-lookup"><span data-stu-id="953d3-157">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="953d3-158">Az új csomag megvásárlása az ügyfél számára</span><span class="sxs-lookup"><span data-stu-id="953d3-158">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="953d3-159">Válassza a bal oldali NAV- **ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, amelyet át szeretne helyezni az új előfizetésbe.</span><span class="sxs-lookup"><span data-stu-id="953d3-159">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="953d3-160">Válassza az **előfizetés hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="953d3-160">Select **Add Subscription** .</span></span>
3. <span data-ttu-id="953d3-161">Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikét), adja meg a licencek számát, majd válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="953d3-161">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span> 

<span data-ttu-id="953d3-162">Az ügyfél most már rendelkezik a régi és az új előfizetéssel is.</span><span class="sxs-lookup"><span data-stu-id="953d3-162">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="953d3-163">A következő lépés a licencek ismételt kiosztása az ügyfél felhasználói számára.</span><span class="sxs-lookup"><span data-stu-id="953d3-163">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="953d3-164">Válassza ki az **ügyfelek** lehetőséget a bal oldali navigációs listából, majd válassza ki az áthelyezni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="953d3-164">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="953d3-165">Válassza **a felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="953d3-165">Select **Users and licenses** .</span></span>
3. <span data-ttu-id="953d3-166">Ha licencet szeretne hozzárendelni egy felhasználóhoz, válassza ki a felhasználót, majd válassza a **licencek kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="953d3-166">To reassign a license to a user, select the user and then select **Manage licenses** .</span></span> 
4. <span data-ttu-id="953d3-167">A **licencek kezelése** lapon törölje a Dynamics 365 for Sales/Customer engagement-tervet az alapszintű (minősített ajánlat) licencből jelölőnégyzetből, és válasszon ki egy új szolgáltatási csomagot ahhoz az előfizetéshez, amelyet az ügyfél áthelyez.</span><span class="sxs-lookup"><span data-stu-id="953d3-167">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="953d3-168">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="953d3-168">Select **Submit** .</span></span> <span data-ttu-id="953d3-169">Ezt minden olyan felhasználónak el kell végeznie, akinek új licencre van szüksége.</span><span class="sxs-lookup"><span data-stu-id="953d3-169">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="953d3-170">Miután áthelyezte a licenceket az új előfizetésre, megszakíthatja a régi előfizetést.</span><span class="sxs-lookup"><span data-stu-id="953d3-170">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="953d3-171">Válassza ki az **ügyfelek** lehetőséget a bal oldali navigációs listából, majd válassza ki az áthelyezni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="953d3-171">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="953d3-172">Az előfizetés részletei lapon állítsa a régi előfizetést **felfüggesztve** értékre, és válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="953d3-172">On the subscription detail page, set the old subscription to **Suspended** and select **Submit** .</span></span>

<span data-ttu-id="953d3-173">A régi előfizetés már fel van függesztve, és az új előfizetés aktív.</span><span class="sxs-lookup"><span data-stu-id="953d3-173">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="953d3-174">A felfüggesztett előfizetés 120 nap elteltével automatikusan kiépítve lesz.</span><span class="sxs-lookup"><span data-stu-id="953d3-174">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="953d3-175">Az ügyfél a régi előfizetéshez nem jár további költségekkel.</span><span class="sxs-lookup"><span data-stu-id="953d3-175">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



