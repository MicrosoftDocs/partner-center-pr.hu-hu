---
title: A Dynamics 365 Business Edition migrálása
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan telepíthet át minősített Dynamics 365 Business Edition-ajánlatokat újabb verzióra a lejárat előtt.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132638"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="fb0a4-103">A Dynamics 365 Business Edition-ajánlatok migrálása újabb verziókba</span><span class="sxs-lookup"><span data-stu-id="fb0a4-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="fb0a4-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="fb0a4-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fb0a4-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="fb0a4-105">Global admin</span></span>
- <span data-ttu-id="fb0a4-106">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="fb0a4-106">User management admin</span></span>
- <span data-ttu-id="fb0a4-107">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="fb0a4-107">Admin agent</span></span>
- <span data-ttu-id="fb0a4-108">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="fb0a4-108">Sales agent</span></span>

<span data-ttu-id="fb0a4-109">2019. január 1-től a Dynamics 365 Business Edition-előfizetésekkel rendelkező ügyfelek már nem újítják meg ezeket az örökölt ajánlatokat; a meglévő előfizetések lejáratakor a rendszer nem újítja meg automatikusan.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-109">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="fb0a4-110">Az előfizetés részleteit tartalmazó lapon az előfizetés állapota "lejár [date]" értékre változik a "automatikusan megújítva [date]" állapotból.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="fb0a4-111">Az ügyfelek folytonosságának biztosítása érdekében az alább felsorolt támogatott lehetőségekre kell áttérnie a lejáró előfizetésekkel.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="fb0a4-112">Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="fb0a4-113">Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejárati előfizetéseket az előfizetés befejezési dátumának és az automatikus megújítás = hamis tulajdonságnak a kiértékelésével érheti el.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="fb0a4-114">A kérdéses előfizetések az automatikus megújítás = false értékre lesznek állítva 2019 január 1-jén.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="fb0a4-115">Az ügyfeleket bármikor át lehet helyezni egy új csomagba.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-115">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="fb0a4-116">A Dynamics 365 üzleti kiadása kivonult</span><span class="sxs-lookup"><span data-stu-id="fb0a4-116">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="fb0a4-117">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="fb0a4-117">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="fb0a4-118">Dynamics 365 for Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="fb0a4-118">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="fb0a4-119">Dynamics Business Central – a Dynamics 365 Business Edition új ajánlatai</span><span class="sxs-lookup"><span data-stu-id="fb0a4-119">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="fb0a4-120">Az új Dynamics Business Central-ajánlatokkal ügyfelei az üzleti folyamatok egyszerűsítése, az ügyfelek közötti interakciók és a jobb döntések meghozatala érdekében összekapcsolhatják pénzügyi, értékesítési, szolgáltatási és üzemeltetési műveleteit.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-120">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="fb0a4-121">A Dynamics 365 Business Central felhőalapú és elérhető a Cloud Solution Provider (CSP) program partnerein keresztül.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-121">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="fb0a4-122">A Dynamics 365 Business Edition-ügyfelek kedvezményes áttérési díjszabást kaphatnak az új Business Central-ajánlatokhoz, 2020. június 30-ig.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-122">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="fb0a4-123">Ügyfelek átváltása új termékekre</span><span class="sxs-lookup"><span data-stu-id="fb0a4-123">Transition customers to new product plans</span></span>

 <span data-ttu-id="fb0a4-124">A kivont SKU-ügyfelek újabb verzióra való áthelyezéséhez a következő lépések szükségesek ebben a sorrendben:</span><span class="sxs-lookup"><span data-stu-id="fb0a4-124">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="fb0a4-125">Az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="fb0a4-125">Purchase the new subscription</span></span>
- <span data-ttu-id="fb0a4-126">Aktuális felhasználói licencek újbóli társítása</span><span class="sxs-lookup"><span data-stu-id="fb0a4-126">Reassign current user licenses</span></span>
- <span data-ttu-id="fb0a4-127">Régi előfizetés megszakítása</span><span class="sxs-lookup"><span data-stu-id="fb0a4-127">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="fb0a4-128">Az új csomag megvásárlása az ügyfél számára</span><span class="sxs-lookup"><span data-stu-id="fb0a4-128">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="fb0a4-129">Válassza a bal oldali NAV- **ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, amelyet át szeretne helyezni az új előfizetésbe.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-129">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="fb0a4-130">Válassza az **előfizetés hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-130">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="fb0a4-131">Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikét), adja meg a licencek számát, majd válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-131">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="fb0a4-132">Az ügyfél most már rendelkezik a régi és az új előfizetéssel is.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-132">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="fb0a4-133">A következő lépés a licencek ismételt kiosztása az ügyfél felhasználói számára.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-133">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="fb0a4-134">Válassza ki az **ügyfelek** lehetőséget a bal oldali navigációs listából, majd válassza ki az áthelyezni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-134">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="fb0a4-135">Válassza **a felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-135">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="fb0a4-136">Ha licencet szeretne hozzárendelni egy felhasználóhoz, válassza ki a felhasználót, majd válassza a **licencek kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-136">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="fb0a4-137">A **licencek kezelése** lapon törölje a Dynamics 365 for Sales/Customer engagement-tervet az alapszintű (minősített ajánlat) licencből jelölőnégyzetből, és válasszon ki egy új szolgáltatási csomagot ahhoz az előfizetéshez, amelyet az ügyfél áthelyez.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-137">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="fb0a4-138">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-138">Select **Submit**.</span></span> <span data-ttu-id="fb0a4-139">Ezt minden olyan felhasználónak el kell végeznie, akinek új licencre van szüksége.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-139">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="fb0a4-140">Miután áthelyezte a licenceket az új előfizetésre, megszakíthatja a régi előfizetést.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-140">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="fb0a4-141">Válassza ki az **ügyfelek** lehetőséget a bal oldali navigációs listából, majd válassza ki az áthelyezni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-141">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="fb0a4-142">Az előfizetés részletei lapon állítsa a régi előfizetést **felfüggesztve** értékre, és válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-142">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="fb0a4-143">A régi előfizetés már fel van függesztve, és az új előfizetés aktív.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-143">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="fb0a4-144">A felfüggesztett előfizetés 120 nap elteltével automatikusan kiépítve lesz.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-144">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="fb0a4-145">Az ügyfél a régi előfizetéshez nem jár további költségekkel.</span><span class="sxs-lookup"><span data-stu-id="fb0a4-145">Your customer will incur no additional costs for the old subscription.</span></span>
