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
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132740"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="13bc0-103">A Dynamics 365 és a Customer Engagement Plan migrálása az Alapszintű szolgáltatásról (arra jogosult ajánlatokról) újabb verziókra</span><span class="sxs-lookup"><span data-stu-id="13bc0-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="13bc0-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="13bc0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="13bc0-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="13bc0-105">Global admin</span></span>
- <span data-ttu-id="13bc0-106">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="13bc0-106">User management admin</span></span>
- <span data-ttu-id="13bc0-107">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="13bc0-107">Admin agent</span></span>
- <span data-ttu-id="13bc0-108">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="13bc0-108">Sales agent</span></span>

<span data-ttu-id="13bc0-109">Az alapszintű (minősített ajánlatok) előfizetések által kínált, a Dynamics 365 for Sales/Customer engagements csomaggal rendelkező ügyfelek a továbbiakban nem tudják megújítani ezeket a régi ajánlatokat: 2019. január 1-től a meglévő előfizetések lejáratakor a rendszer nem újítja meg automatikusan.</span><span class="sxs-lookup"><span data-stu-id="13bc0-109">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="13bc0-110">Az előfizetés részleteit tartalmazó lapon az előfizetés állapota "lejár [date]" értékre változik a "automatikusan megújítva [date]" állapotból.</span><span class="sxs-lookup"><span data-stu-id="13bc0-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="13bc0-111">Az ügyfelek folytonosságának biztosítása érdekében az alább felsorolt támogatott lehetőségekre kell áttérnie a lejáró előfizetésekkel.</span><span class="sxs-lookup"><span data-stu-id="13bc0-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="13bc0-112">Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="13bc0-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="13bc0-113">Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejárati előfizetéseket az előfizetés befejezési dátumának és az automatikus megújítás = hamis tulajdonságnak a kiértékelésével érheti el.</span><span class="sxs-lookup"><span data-stu-id="13bc0-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="13bc0-114">A kérdéses előfizetések az automatikus megújítás = false értékre lesznek állítva 2019 január 1-jén.</span><span class="sxs-lookup"><span data-stu-id="13bc0-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="13bc0-115">Az ügyfeleket bármikor át lehet helyezni egy új csomagba.</span><span class="sxs-lookup"><span data-stu-id="13bc0-115">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="13bc0-116">A Dynamics 365-ajánlatok kivonulnak</span><span class="sxs-lookup"><span data-stu-id="13bc0-116">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="13bc0-117">Dynamics 365 for Sales Enterprise Edition CRMOL alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-118">Dynamics 365 for Sales Enterprise Edition CRMOL alapszintű (minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="13bc0-118">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="13bc0-119">Dynamics 365 for Sales Enterprise Edition CRMOL alapszintű (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="13bc0-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="13bc0-120">Dynamics 365 for Sales Enterprise Edition (kormányzati díjszabás) CRMOL alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-121">Dynamics 365 for Sales Enterprise Edition, SA for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-122">Dynamics 365 for Sales Enterprise Edition, SA for CRM alapszintű (minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="13bc0-122">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="13bc0-123">Dynamics 365 for Sales Enterprise Edition SA for CRM Basic (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="13bc0-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="13bc0-124">Dynamics 365 for Sales Enterprise Edition (kormányzati díjszabás) az SA-től a CRM alapszintű verzióra (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-126">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (minősített ajánlat) oktatóknak</span><span class="sxs-lookup"><span data-stu-id="13bc0-126">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="13bc0-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="13bc0-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="13bc0-128">Dynamics 365 for Sales Enterprise Edition (Government díjszabás) Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-128">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-129">Dynamics 365 Customer engagement Plan Enterprise Edition CRMOL alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-130">Dynamics 365 Customer engagement Plan Enterprise Edition (kormányzati díjszabás) CRMOL alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-131">Dynamics 365 Customer engagement Plan Enterprise Edition CRMOL alapszintű (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="13bc0-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="13bc0-132">Dynamics 365 Customer engagement Plan Enterprise Edition CRMOL alapszintű (minősített ajánlat) a kari</span><span class="sxs-lookup"><span data-stu-id="13bc0-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="13bc0-133">Dynamics 365 ügyfél-bevonási terv Enterprise Edition for SA a CRM alapszintű (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-134">Dynamics 365 Customer engagement Plan Enterprise Edition (kormányzati díjszabás) from SA for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-135">Dynamics 365 ügyfél-bevonási terv Enterprise Edition for SA for CRM Basic (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="13bc0-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="13bc0-136">Dynamics 365 ügyfél-bevonási terv Enterprise Edition for SA for CRM alapszintű (minősített ajánlat) a kar számára</span><span class="sxs-lookup"><span data-stu-id="13bc0-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="13bc0-137">Dynamics 365 Customer engagement Plan Enterprise Edition Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-138">Dynamics 365 Customer engagement Plan Enterprise Edition (kormányzati díjszabás) Add-On for CRM Basic (minősített ajánlat)</span><span class="sxs-lookup"><span data-stu-id="13bc0-138">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-139">Dynamics 365 Customer engagement Plan Enterprise Edition Add-On a CRM alapszintű (minősített ajánlat) diákoknak</span><span class="sxs-lookup"><span data-stu-id="13bc0-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="13bc0-140">Dynamics 365 Customer engagement Plan Enterprise Edition Add-On for CRM Basic (minősített ajánlat) a kari</span><span class="sxs-lookup"><span data-stu-id="13bc0-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="13bc0-141">Dynamics 365 for Sales/Customer bevonási terv az alapszintű (minősített ajánlatok) – helyettesítő csomagok</span><span class="sxs-lookup"><span data-stu-id="13bc0-141">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="13bc0-142">**Kivont ajánlatok**</span><span class="sxs-lookup"><span data-stu-id="13bc0-142">**Retired offers**</span></span>   

- <span data-ttu-id="13bc0-143">Dynamics 365 CRM alapszintű vagy CRMOL alapszintű (minősített ajánlat) értékesítéséhez</span><span class="sxs-lookup"><span data-stu-id="13bc0-143">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="13bc0-144">Dynamics 365 Customer engagement-terv a CRM Basic vagy a CRMOL alapszintű (minősített ajánlat) alapján</span><span class="sxs-lookup"><span data-stu-id="13bc0-144">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="13bc0-145">**Helyettesítő beállítások**</span><span class="sxs-lookup"><span data-stu-id="13bc0-145">**Replacement options**</span></span>
- <span data-ttu-id="13bc0-146">Dynamics 365 for Sales Professional (új)</span><span class="sxs-lookup"><span data-stu-id="13bc0-146">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="13bc0-147">Dynamics 365 for Sales Professional (új)</span><span class="sxs-lookup"><span data-stu-id="13bc0-147">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="13bc0-148">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="13bc0-148">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="13bc0-149">Dynamics 365 Customer engagement-csomag vagy</span><span class="sxs-lookup"><span data-stu-id="13bc0-149">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="13bc0-150">Dynamics 365-csapat tagjai</span><span class="sxs-lookup"><span data-stu-id="13bc0-150">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="13bc0-151">Ügyfelek átváltása új termékekre</span><span class="sxs-lookup"><span data-stu-id="13bc0-151">Transition customers to new product plans</span></span>

<span data-ttu-id="13bc0-152">A kivont SKU-ügyfelek újabb verzióra való áthelyezéséhez a következő lépések szükségesek ebben a sorrendben:</span><span class="sxs-lookup"><span data-stu-id="13bc0-152">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="13bc0-153">Az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="13bc0-153">Purchase the new subscription</span></span>
- <span data-ttu-id="13bc0-154">Aktuális felhasználói licencek újbóli társítása</span><span class="sxs-lookup"><span data-stu-id="13bc0-154">Reassign current user licenses</span></span>
- <span data-ttu-id="13bc0-155">Régi előfizetés megszakítása</span><span class="sxs-lookup"><span data-stu-id="13bc0-155">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="13bc0-156">Az új csomag megvásárlása az ügyfél számára</span><span class="sxs-lookup"><span data-stu-id="13bc0-156">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="13bc0-157">Válassza a bal oldali NAV- **ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, amelyet át szeretne helyezni az új előfizetésbe.</span><span class="sxs-lookup"><span data-stu-id="13bc0-157">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="13bc0-158">Válassza az **előfizetés hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="13bc0-158">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="13bc0-159">Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikét), adja meg a licencek számát, majd válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="13bc0-159">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="13bc0-160">Az ügyfél most már rendelkezik a régi és az új előfizetéssel is.</span><span class="sxs-lookup"><span data-stu-id="13bc0-160">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="13bc0-161">A következő lépés a licencek ismételt kiosztása az ügyfél felhasználói számára.</span><span class="sxs-lookup"><span data-stu-id="13bc0-161">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="13bc0-162">Válassza ki az **ügyfelek** lehetőséget a bal oldali navigációs listából, majd válassza ki az áthelyezni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="13bc0-162">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="13bc0-163">Válassza **a felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="13bc0-163">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="13bc0-164">Ha licencet szeretne hozzárendelni egy felhasználóhoz, válassza ki a felhasználót, majd válassza a **licencek kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="13bc0-164">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="13bc0-165">A **licencek kezelése** lapon törölje a Dynamics 365 for Sales/Customer engagement-tervet az alapszintű (minősített ajánlat) licencből jelölőnégyzetből, és válasszon ki egy új szolgáltatási csomagot ahhoz az előfizetéshez, amelyet az ügyfél áthelyez.</span><span class="sxs-lookup"><span data-stu-id="13bc0-165">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="13bc0-166">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="13bc0-166">Select **Submit**.</span></span> <span data-ttu-id="13bc0-167">Ezt minden olyan felhasználónak el kell végeznie, akinek új licencre van szüksége.</span><span class="sxs-lookup"><span data-stu-id="13bc0-167">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="13bc0-168">Miután áthelyezte a licenceket az új előfizetésre, megszakíthatja a régi előfizetést.</span><span class="sxs-lookup"><span data-stu-id="13bc0-168">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="13bc0-169">Válassza ki az **ügyfelek** lehetőséget a bal oldali navigációs listából, majd válassza ki az áthelyezni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="13bc0-169">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="13bc0-170">Az előfizetés részletei lapon állítsa a régi előfizetést **felfüggesztve** értékre, és válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="13bc0-170">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="13bc0-171">A régi előfizetés már fel van függesztve, és az új előfizetés aktív.</span><span class="sxs-lookup"><span data-stu-id="13bc0-171">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="13bc0-172">A felfüggesztett előfizetés 120 nap elteltével automatikusan kiépítve lesz.</span><span class="sxs-lookup"><span data-stu-id="13bc0-172">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="13bc0-173">Az ügyfél a régi előfizetéshez nem jár további költségekkel.</span><span class="sxs-lookup"><span data-stu-id="13bc0-173">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



