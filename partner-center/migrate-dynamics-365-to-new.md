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
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/17/2020
ms.locfileid: "92528006"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="43deb-103">A Dynamics 365 Business Edition-ajánlatok migrálása újabb verziókba</span><span class="sxs-lookup"><span data-stu-id="43deb-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="43deb-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="43deb-104">**Applies to**</span></span>

- <span data-ttu-id="43deb-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="43deb-105">Partner Center</span></span>

<span data-ttu-id="43deb-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="43deb-106">**Appropriate roles**</span></span>
- <span data-ttu-id="43deb-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="43deb-107">Global admin</span></span>
- <span data-ttu-id="43deb-108">Felhasználói rendszergazda</span><span class="sxs-lookup"><span data-stu-id="43deb-108">User admin</span></span>
- <span data-ttu-id="43deb-109">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="43deb-109">Admin agent</span></span>
- <span data-ttu-id="43deb-110">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="43deb-110">Sales agent</span></span>

<span data-ttu-id="43deb-111">2019. január 1-től a Dynamics 365 Business Edition-előfizetésekkel rendelkező ügyfelek már nem újítják meg ezeket az örökölt ajánlatokat; a meglévő előfizetések lejáratakor a rendszer nem újítja meg automatikusan.</span><span class="sxs-lookup"><span data-stu-id="43deb-111">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="43deb-112">Az előfizetés részleteit tartalmazó lapon az előfizetés állapota "lejár [date]" értékre változik a "automatikusan megújítva [date]" állapotból.</span><span class="sxs-lookup"><span data-stu-id="43deb-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="43deb-113">Az ügyfelek folytonosságának biztosítása érdekében az alább felsorolt támogatott lehetőségekre kell áttérnie a lejáró előfizetésekkel.</span><span class="sxs-lookup"><span data-stu-id="43deb-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="43deb-114">Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="43deb-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="43deb-115">Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejárati előfizetéseket az előfizetés befejezési dátumának és az automatikus megújítás = hamis tulajdonságnak a kiértékelésével érheti el.</span><span class="sxs-lookup"><span data-stu-id="43deb-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="43deb-116">A kérdéses előfizetések az automatikus megújítás = false értékre lesznek állítva, január 1-jén 2019.</span><span class="sxs-lookup"><span data-stu-id="43deb-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="43deb-117">Az ügyfeleket bármikor át lehet helyezni egy új csomagba.</span><span class="sxs-lookup"><span data-stu-id="43deb-117">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="43deb-118">A Dynamics 365 üzleti kiadása kivonult</span><span class="sxs-lookup"><span data-stu-id="43deb-118">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="43deb-119">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="43deb-119">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="43deb-120">Dynamics 365 for Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="43deb-120">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="43deb-121">Dynamics Business Central – a Dynamics 365 Business Edition új ajánlatai</span><span class="sxs-lookup"><span data-stu-id="43deb-121">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="43deb-122">Az új Dynamics Business Central-ajánlatokkal ügyfelei az üzleti folyamatok egyszerűsítése, az ügyfelek közötti interakciók és a jobb döntések meghozatala érdekében összekapcsolhatják pénzügyi, értékesítési, szolgáltatási és üzemeltetési műveleteit.</span><span class="sxs-lookup"><span data-stu-id="43deb-122">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="43deb-123">A Dynamics 365 Business Central felhőalapú és elérhető a Cloud Solution Provider (CSP) program partnerein keresztül.</span><span class="sxs-lookup"><span data-stu-id="43deb-123">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="43deb-124">A Dynamics 365 Business Edition-ügyfelek kedvezményes áttérési díjszabást kaphatnak az új Business Central-ajánlatokhoz, 2020. június 30-ig.</span><span class="sxs-lookup"><span data-stu-id="43deb-124">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="43deb-125">Ügyfelek átváltása új termékekre</span><span class="sxs-lookup"><span data-stu-id="43deb-125">Transition customers to new product plans</span></span>

 <span data-ttu-id="43deb-126">A kivont SKU-ügyfelek újabb verzióra való áthelyezéséhez a következő lépések szükségesek ebben a sorrendben:</span><span class="sxs-lookup"><span data-stu-id="43deb-126">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="43deb-127">Az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="43deb-127">Purchase the new subscription</span></span>
- <span data-ttu-id="43deb-128">Aktuális felhasználói licencek újbóli társítása</span><span class="sxs-lookup"><span data-stu-id="43deb-128">Reassign current user licenses</span></span>
- <span data-ttu-id="43deb-129">Régi előfizetés megszakítása</span><span class="sxs-lookup"><span data-stu-id="43deb-129">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="43deb-130">Az új csomag megvásárlása az ügyfél számára</span><span class="sxs-lookup"><span data-stu-id="43deb-130">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="43deb-131">Válassza a bal oldali NAV- **ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, amelyet át szeretne helyezni az új előfizetésbe.</span><span class="sxs-lookup"><span data-stu-id="43deb-131">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="43deb-132">Válassza az **előfizetés hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="43deb-132">Select **Add Subscription** .</span></span>
3. <span data-ttu-id="43deb-133">Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikét), adja meg a licencek számát, majd válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="43deb-133">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span> 

<span data-ttu-id="43deb-134">Az ügyfél most már rendelkezik a régi és az új előfizetéssel is.</span><span class="sxs-lookup"><span data-stu-id="43deb-134">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="43deb-135">A következő lépés a licencek ismételt kiosztása az ügyfél felhasználói számára.</span><span class="sxs-lookup"><span data-stu-id="43deb-135">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="43deb-136">Válassza ki az **ügyfelek** lehetőséget a bal oldali navigációs listából, majd válassza ki az áthelyezni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="43deb-136">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="43deb-137">Válassza **a felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="43deb-137">Select **Users and licenses** .</span></span>
3. <span data-ttu-id="43deb-138">Ha licencet szeretne hozzárendelni egy felhasználóhoz, válassza ki a felhasználót, majd válassza a **licencek kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="43deb-138">To reassign a license to a user, select the user and then select **Manage licenses** .</span></span> 
4. <span data-ttu-id="43deb-139">A **licencek kezelése** lapon törölje a Dynamics 365 for Sales/Customer engagement-tervet az alapszintű (minősített ajánlat) licencből jelölőnégyzetből, és válasszon ki egy új szolgáltatási csomagot ahhoz az előfizetéshez, amelyet az ügyfél áthelyez.</span><span class="sxs-lookup"><span data-stu-id="43deb-139">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="43deb-140">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="43deb-140">Select **Submit** .</span></span> <span data-ttu-id="43deb-141">Ezt minden olyan felhasználónak el kell végeznie, akinek új licencre van szüksége.</span><span class="sxs-lookup"><span data-stu-id="43deb-141">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="43deb-142">Miután áthelyezte a licenceket az új előfizetésre, megszakíthatja a régi előfizetést.</span><span class="sxs-lookup"><span data-stu-id="43deb-142">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="43deb-143">Válassza ki az **ügyfelek** lehetőséget a bal oldali navigációs listából, majd válassza ki az áthelyezni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="43deb-143">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="43deb-144">Az előfizetés részletei lapon állítsa a régi előfizetést **felfüggesztve** értékre, és válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="43deb-144">On the subscription detail page, set the old subscription to **Suspended** and select **Submit** .</span></span>

<span data-ttu-id="43deb-145">A régi előfizetés már fel van függesztve, és az új előfizetés aktív.</span><span class="sxs-lookup"><span data-stu-id="43deb-145">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="43deb-146">A felfüggesztett előfizetés 120 nap elteltével automatikusan kiépítve lesz.</span><span class="sxs-lookup"><span data-stu-id="43deb-146">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="43deb-147">Az ügyfél a régi előfizetéshez nem jár további költségekkel.</span><span class="sxs-lookup"><span data-stu-id="43deb-147">Your customer will incur no additional costs for the old subscription.</span></span>
