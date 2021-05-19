---
title: A Dynamics 365 Business Edition áttelepítése
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan mihelheti át a minősített Dynamics 365 Business Edition-ajánlatokat az újabb verziókra, mielőtt lejárnak.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151525"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="8bbac-103">A Dynamics 365 Business Edition-ajánlatok migrálása újabb verziókba</span><span class="sxs-lookup"><span data-stu-id="8bbac-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="8bbac-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Rendszergazdai ügynök | Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="8bbac-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="8bbac-105">2019. január 1-től a Dynamics 365 Business Edition-előfizetéssel nem lehet többé megújítani ezeket az örökölt ajánlatokat; A meglévő előfizetések nem újulnak meg automatikusan a lejáratukkor.</span><span class="sxs-lookup"><span data-stu-id="8bbac-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="8bbac-106">Az előfizetés részleteinek oldalán az előfizetés állapota "Lejárat [dátum] időpontban" állapotra változik az "Automatikus megújítás [dátum] időpontban" állapotra.</span><span class="sxs-lookup"><span data-stu-id="8bbac-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="8bbac-107">Az ügyfelek folytonosságának biztosítása érdekében a lejáró előfizetéseket az alább felsorolt támogatott lehetőségekre kell átemálnia.</span><span class="sxs-lookup"><span data-stu-id="8bbac-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="8bbac-108">Javasoljuk, hogy az ügyfeleket az előfizetés éves záró dátuma előtt új előfizetésekbe költöztetjék, hogy elkerülje az ügyfelek szolgáltatáskimaradását.</span><span class="sxs-lookup"><span data-stu-id="8bbac-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="8bbac-109">Ha az API-t használja (CREST vagy Partnerközpont), a lejáró előfizetéseket az előfizetés záró dátumának és az automatikus megújítás = Hamis tulajdonság kiértékelével találhatja meg.</span><span class="sxs-lookup"><span data-stu-id="8bbac-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="8bbac-110">A kérdéses előfizetések 2019. január 1-jén automatikus megújítás=Hamis értékre lesznek beállítva.</span><span class="sxs-lookup"><span data-stu-id="8bbac-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="8bbac-111">Az ügyfeleket bármikor új csomagba költöztetheti.</span><span class="sxs-lookup"><span data-stu-id="8bbac-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="8bbac-112">A Dynamics 365 Business Edition kiadások kivezetve</span><span class="sxs-lookup"><span data-stu-id="8bbac-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="8bbac-113">Dynamics 365 for Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="8bbac-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="8bbac-114">Dynamics 365 for Team Members, Business edition</span><span class="sxs-lookup"><span data-stu-id="8bbac-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="8bbac-115">Dynamics Business Central – a Dynamics 365 Business Edition új ajánlata</span><span class="sxs-lookup"><span data-stu-id="8bbac-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="8bbac-116">Az új Dynamics Business Central-ajánlatokkal az ügyfelek össze is kapcsolhatják pénzügyi, értékesítési, szolgáltatási és műveleti munkájukat az üzleti folyamatok leegyszerűsítés, az ügyfél-interakciók javítása és a jobb döntések meghozatala érdekében.</span><span class="sxs-lookup"><span data-stu-id="8bbac-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="8bbac-117">A Dynamics 365 Business Central felhőalapú, és csak Felhőszolgáltató (CSP) programpartnerek számára érhető el.</span><span class="sxs-lookup"><span data-stu-id="8bbac-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="8bbac-118">A Dynamics 365 Business Edition-ügyfelek 2020. június 30-ig kedvezményes áttérési díjszabást kaphatnak az új Business Central-ajánlatokhoz.</span><span class="sxs-lookup"><span data-stu-id="8bbac-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="8bbac-119">Ügyfelek váltása új terméktervekre</span><span class="sxs-lookup"><span data-stu-id="8bbac-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="8bbac-120">Ha az ügyfeleket a visszavont SKUS-król újabbakra kívánja átemeltetni, a következő lépésekre van szükség ebben a sorrendben:</span><span class="sxs-lookup"><span data-stu-id="8bbac-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="8bbac-121">Az új előfizetés vásárlása</span><span class="sxs-lookup"><span data-stu-id="8bbac-121">Purchase the new subscription</span></span>
- <span data-ttu-id="8bbac-122">Aktuális felhasználói licencek ismételt hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="8bbac-122">Reassign current user licenses</span></span>
- <span data-ttu-id="8bbac-123">Régi előfizetés lemondása</span><span class="sxs-lookup"><span data-stu-id="8bbac-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="8bbac-124">Az új csomag vásárlása az ügyfél számára</span><span class="sxs-lookup"><span data-stu-id="8bbac-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="8bbac-125">A **bal oldali navigációs** sávon válassza az Ügyfelek lehetőséget, majd válassza ki az új előfizetésre áthelyezni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="8bbac-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="8bbac-126">Válassza **az Előfizetés hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="8bbac-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="8bbac-127">Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek valamelyikét), adja meg a licencek számát, majd válassza a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="8bbac-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="8bbac-128">Az ügyfél most már a régi előfizetéssel és az új előfizetéssel is rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="8bbac-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="8bbac-129">A következő lépés a licencek ismételt hozzárendelése az ügyfél felhasználóihoz.</span><span class="sxs-lookup"><span data-stu-id="8bbac-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="8bbac-130">A **bal oldali navigációs** sávon válassza az Ügyfelek lehetőséget, majd válassza ki a költözni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="8bbac-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="8bbac-131">Válassza **a Felhasználók és licencek lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="8bbac-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="8bbac-132">Egy licenc felhasználóhoz való ismételt hozzárendeléséhez jelölje ki a felhasználót, majd válassza a **Licencek kezelése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="8bbac-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="8bbac-133">A **Licencek kezelése** lapon törölje a Dynamics 365 for Sales/Customer Engagement Plan from Basic (Minősített ajánlat) licencből jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatástervet ahhoz az előfizetéshez, amelybe az ügyfél át lesz költözve.</span><span class="sxs-lookup"><span data-stu-id="8bbac-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="8bbac-134">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8bbac-134">Select **Submit**.</span></span> <span data-ttu-id="8bbac-135">Ezt minden olyan felhasználóval meg kell tenni, akinek új licencre van szüksége.</span><span class="sxs-lookup"><span data-stu-id="8bbac-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="8bbac-136">Miután áthelyezte a licenceket az új előfizetésbe, megszüntetheti a régi előfizetést.</span><span class="sxs-lookup"><span data-stu-id="8bbac-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="8bbac-137">A **bal oldali navigációs** sávon válassza az Ügyfelek lehetőséget, majd válassza ki a költözni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="8bbac-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="8bbac-138">Az előfizetés részletei lapon állítsa a régi előfizetést Felfüggesztettre, majd **válassza** a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="8bbac-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="8bbac-139">A régi előfizetés most fel van függesztve, és az új előfizetés aktív.</span><span class="sxs-lookup"><span data-stu-id="8bbac-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="8bbac-140">A felfüggesztett előfizetés 120 nap után automatikusan fel lesz függesztve.</span><span class="sxs-lookup"><span data-stu-id="8bbac-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="8bbac-141">Az ügyfél nem jár többletköltségsel a régi előfizetésért.</span><span class="sxs-lookup"><span data-stu-id="8bbac-141">Your customer will incur no additional costs for the old subscription.</span></span>
