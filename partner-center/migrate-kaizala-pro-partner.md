---
title: Kaizala Pro-előfizetések migrálása a Microsoft365-be
description: Ismerje meg, hogyan telepíthet át Kaizala Pro-előfizetéseket Microsoft365 vagy Office 365-verzióra. Az ügyfelek átváltásával kapcsolatos további információkért olvassa el ezt a cikket.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530517"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="ec7d0-104">Kaizala Pro önálló előfizetések migrálása a Microsoft365 vagy az Office 365 verzióra</span><span class="sxs-lookup"><span data-stu-id="ec7d0-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="ec7d0-105">2020. július 1-től a Microsoft befejezte a Kaizala Pro önálló szolgáltatás értékesítését.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-105">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="ec7d0-106">Ezen időpont után az ügyfelek többé nem vásárolhatnak új Kaizala Pro-előfizetéseket, és a meglévő Kaizala Pro-előfizetések nem fognak automatikusan megújítani a lejárat után.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-106">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="ec7d0-107">Az ügyfelek folytonosságának biztosítása érdekében az alábbi listában szereplő, a Kaizala Pro önálló előfizetések lejáratával rendelkező ügyfeleket kell átállnia egy támogatott SKU-ra.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-107">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="ec7d0-108">Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="ec7d0-109">Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejáró előfizetések felderítéséhez az előfizetés befejezési dátumát és az automatikus megújítás tulajdonságot false (hamis) értékre kell kiértékelve: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="ec7d0-109">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="ec7d0-110">Az E4-előfizetések `auto renew=False` 2020. július 1-jén lesznek beállítva.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-110">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="ec7d0-111">Az ügyfeleket bármikor át lehet helyezni egy új csomagba.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-111">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="ec7d0-112">Kaizala Pro önálló helyettesítési csomagok</span><span class="sxs-lookup"><span data-stu-id="ec7d0-112">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="ec7d0-113">Az új csomagokkal az ügyfelek a Microsoft 365 újabb funkcióit és funkcióit vehetik igénybe.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-113">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="ec7d0-114">A díjszabással kapcsolatos részletek a partner Center árlista és ajánlatok listája mátrixában találhatók.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-114">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="ec7d0-115">[**Üzleti Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), beleértve a következőket:</span><span class="sxs-lookup"><span data-stu-id="ec7d0-115">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="ec7d0-116">Alapszintű Microsoft 365 Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="ec7d0-116">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="ec7d0-117">Microsoft 365 Vállalati verzió standard</span><span class="sxs-lookup"><span data-stu-id="ec7d0-117">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="ec7d0-118">Prémium Microsoft 365 Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="ec7d0-118">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="ec7d0-119">[**Microsoft 365 a Frontline számára**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), beleértve a következőket:</span><span class="sxs-lookup"><span data-stu-id="ec7d0-119">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="ec7d0-120">Microsoft 365 F3 (korábban Microsoft 365 F1) és Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="ec7d0-120">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="ec7d0-121">[**Microsoft 365 a vállalat számára**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), beleértve a következőket:</span><span class="sxs-lookup"><span data-stu-id="ec7d0-121">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="ec7d0-122">Office 365 E1 csomag</span><span class="sxs-lookup"><span data-stu-id="ec7d0-122">Office 365 E1</span></span>
   - <span data-ttu-id="ec7d0-123">Microsoft 365 E3 és Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="ec7d0-123">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="ec7d0-124">Microsoft 365 E5 és Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="ec7d0-124">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="ec7d0-125">[**Oktatási Microsoft 365**](https://www.microsoft.com/education/buy-license/microsoft365), beleértve a következőket:</span><span class="sxs-lookup"><span data-stu-id="ec7d0-125">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="ec7d0-126">Microsoft 365 a1 és Office 365 a1</span><span class="sxs-lookup"><span data-stu-id="ec7d0-126">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="ec7d0-127">Microsoft 365 a3 és Office 365 a3</span><span class="sxs-lookup"><span data-stu-id="ec7d0-127">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="ec7d0-128">Microsoft 365 a5 és Office 365 a5 csomag</span><span class="sxs-lookup"><span data-stu-id="ec7d0-128">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="ec7d0-129">Ügyfelek átváltása új termékekre</span><span class="sxs-lookup"><span data-stu-id="ec7d0-129">Transition customers to new product plans</span></span>

<span data-ttu-id="ec7d0-130">A Microsoft folyamatosan új termékeket és szolgáltatásokat kínál partnereinknek.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-130">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="ec7d0-131">Ezekben az esetekben előfordulhat, hogy frissítenie kell az ügyfeleket az új szolgáltatásokra, vagy át kell telepítenie az előfizetéseket olyan SKU-ból, amely végül le lesz állítva.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-131">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="ec7d0-132">Az ügyfelek áttelepítése a kivont SKU-ról újabb verzióra a következő lépések szükségesek:</span><span class="sxs-lookup"><span data-stu-id="ec7d0-132">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="ec7d0-133">A.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-133">A.</span></span> <span data-ttu-id="ec7d0-134">Az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="ec7d0-134">Purchase the new subscription</span></span>

<span data-ttu-id="ec7d0-135">B.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-135">B.</span></span> <span data-ttu-id="ec7d0-136">Aktuális felhasználói licencek újbóli társítása</span><span class="sxs-lookup"><span data-stu-id="ec7d0-136">Reassign current user licenses</span></span>

<span data-ttu-id="ec7d0-137">C.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-137">C.</span></span> <span data-ttu-id="ec7d0-138">Régi előfizetés megszakítása</span><span class="sxs-lookup"><span data-stu-id="ec7d0-138">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="ec7d0-139">Ügyfelek migrálása új csomagokra</span><span class="sxs-lookup"><span data-stu-id="ec7d0-139">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="ec7d0-140">A.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-140">A.</span></span> <span data-ttu-id="ec7d0-141">Az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="ec7d0-141">Purchase the new subscription</span></span>

1. <span data-ttu-id="ec7d0-142">Az új előfizetés megvásárlásához a **partner Center** menüjéből válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza az **előfizetések hozzáadása** elemet.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-142">To purchase the new subscription, from the **Partner Center** menu, select **Customers** , select the customer you want to move, and then select **Add subscriptions** .</span></span>

2. <span data-ttu-id="ec7d0-143">Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikét), adja meg a licencek számát, majd válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-143">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span>

<span data-ttu-id="ec7d0-144">Az ügyfél most már rendelkezik a régi és az új előfizetéssel, a régi Kaizala Pro önálló előfizetéssel és az új "Target" előfizetéssel, például 1. lehetőség – Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-144">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="ec7d0-145">B.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-145">B.</span></span> <span data-ttu-id="ec7d0-146">Aktuális felhasználói licencek újbóli társítása</span><span class="sxs-lookup"><span data-stu-id="ec7d0-146">Reassign current user licenses</span></span>

1. <span data-ttu-id="ec7d0-147">Az ügyfél felhasználói licencének újbóli hozzárendeléséhez a **partner Center** menüjéből válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza a **felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-147">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers** , select the customer you are moving, and then select **Users and licenses** .</span></span> <span data-ttu-id="ec7d0-148">Megnyílik az ügyfél felhasználói és licencek lapja.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-148">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="ec7d0-149">A felhasználói licenc újbóli hozzárendeléséhez válassza ki az újból hozzárendelni kívánt felhasználót, majd válassza a **licencek kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-149">To reassign user license, select the user to reassign and then select **Manage licenses** .</span></span>

3. <span data-ttu-id="ec7d0-150">A **licencek kezelése** lapon törölje a Kaizala Pro önálló licenc jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatási csomagot ahhoz az előfizetéshez, amelyet az ügyfél áthelyez.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-150">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="ec7d0-151">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-151">Select **Submit** .</span></span> <span data-ttu-id="ec7d0-152">A megerősítést kérő lap felsorolja az új licenc-hozzárendeléseket.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-152">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="ec7d0-153">Folytassa ugyanezt a folyamatot azoknál a felhasználóknál, akiknek licenc-hozzárendelésre van szükségük.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-153">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="ec7d0-154">C.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-154">C.</span></span> <span data-ttu-id="ec7d0-155">Régi előfizetés megszakítása</span><span class="sxs-lookup"><span data-stu-id="ec7d0-155">Cancel old subscription</span></span>

<span data-ttu-id="ec7d0-156">Miután áthelyezte a felhasználói licencet az új szolgáltatásba, biztonságosan megszakíthatja a kivont előfizetést az ügyfél szintjén.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-156">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="ec7d0-157">A **partner Center** menüben válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-157">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="ec7d0-158">Válassza ki azt az ügyfelet, amelynek előfizetését törli.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-158">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="ec7d0-159">Az előfizetés részletei lapon állítsa az előfizetést **felfüggesztve** értékre.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-159">In the subscription detail page, set the subscription to **Suspended** .</span></span>

3.  <span data-ttu-id="ec7d0-160">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-160">Select **Submit** .</span></span>

<span data-ttu-id="ec7d0-161">A régi előfizetés fel van függesztve, és az új előfizetés aktív.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-161">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="ec7d0-162">A felfüggesztett előfizetés 120 nap elteltével automatikusan kiépítve lesz.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-162">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="ec7d0-163">Az ügyfél nem számít fel további költséget a régi előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="ec7d0-163">The customer incurs no additional costs for the old subscription.</span></span>
