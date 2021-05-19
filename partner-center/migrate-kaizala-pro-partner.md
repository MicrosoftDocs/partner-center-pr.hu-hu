---
title: Kaizala Pro-előfizetések migrálása a Microsoft 365-be
description: Útmutató Kaizala Pro-előfizetések áttelepítéséhez Microsoft 365 Office 365-verziókba. Az ügyfelek átváltásának további részleteiért olvassa el ezt a cikket.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146425"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="6bbc2-104">Kaizala Pro Standalone-előfizetések áttelepítése Microsoft 365 Office 365-verziókba</span><span class="sxs-lookup"><span data-stu-id="6bbc2-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="6bbc2-105">**Megfelelő szerepkörök:** Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="6bbc2-105">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="6bbc2-106">2020. július 1-től a Microsoft befejezi az önálló Kaizala Pro szolgáltatás értékesítését.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-106">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="6bbc2-107">Az ügyfelek ezt követően már nem vásárolhatnak új Kaizala Pro-előfizetéseket, és a meglévő Kaizala Pro-előfizetések nem újulnak meg automatikusan a lejáratuk után.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-107">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="6bbc2-108">Az ügyfelek folytonosságának biztosítása érdekében a lejáró Kaizala Pro önálló előfizetéssel az alább felsorolt támogatott termékváltozatra kell átállni az ügyfelekre.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-108">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="6bbc2-109">Javasoljuk, hogy az ügyfeleket az előfizetés éves záró dátuma előtt új előfizetésekbe költöztetjék, hogy elkerülje az ügyfelek szolgáltatáskimaradását.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="6bbc2-110">Ha az API-t használja (CREST vagy Partnerközpont), a lejáró előfizetéseket úgy derítheti fel, ha kiértékeli az előfizetés záró dátumát, valamint az automatikus megújítás tulajdonság false (hamis) értéket ad meg: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="6bbc2-110">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="6bbc2-111">Az E4-előfizetések beállítása `auto renew=False` 2020. július 1-ére lesz beállítva.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-111">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="6bbc2-112">Az ügyfeleket bármikor áthelyezheti egy új csomagba.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-112">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="6bbc2-113">Kaizala Pro Önálló helyettesítő csomagok</span><span class="sxs-lookup"><span data-stu-id="6bbc2-113">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="6bbc2-114">Az új csomagokkal az ügyfelek az új funkciókat és funkciókat is kihasználhatják a Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-114">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="6bbc2-115">A díjszabás részletei az árlista és az ajánlatlista mátrixában találhatók a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-115">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="6bbc2-116">[**Microsoft 365 vállalati verzió,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)beleértve a következőket:</span><span class="sxs-lookup"><span data-stu-id="6bbc2-116">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="6bbc2-117">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="6bbc2-117">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="6bbc2-118">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="6bbc2-118">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="6bbc2-119">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="6bbc2-119">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="6bbc2-120">[**Microsoft 365 az elővonalhoz, beleértve**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)a következőket:</span><span class="sxs-lookup"><span data-stu-id="6bbc2-120">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="6bbc2-121">Microsoft 365 F3 (korábbi nevén F1) Microsoft 365 Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="6bbc2-121">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="6bbc2-122">[**Microsoft 365 vállalati verzióhoz,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)beleértve a következőket:</span><span class="sxs-lookup"><span data-stu-id="6bbc2-122">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="6bbc2-123">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="6bbc2-123">Office 365 E1</span></span>
   - <span data-ttu-id="6bbc2-124">Microsoft 365 E3 és Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="6bbc2-124">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="6bbc2-125">Microsoft 365 E5 és Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="6bbc2-125">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="6bbc2-126">[**Microsoft 365 for Education,**](https://www.microsoft.com/education/buy-license/microsoft365)beleértve a következőket:</span><span class="sxs-lookup"><span data-stu-id="6bbc2-126">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="6bbc2-127">Microsoft 365 A1 és Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="6bbc2-127">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="6bbc2-128">Microsoft 365 A3 és Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="6bbc2-128">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="6bbc2-129">Microsoft 365 A5 és Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="6bbc2-129">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="6bbc2-130">Ügyfelek váltása új terméktervekre</span><span class="sxs-lookup"><span data-stu-id="6bbc2-130">Transition customers to new product plans</span></span>

<span data-ttu-id="6bbc2-131">A Microsoft folyamatosan kínál új termékeket és szolgáltatásokat partnereinknek.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-131">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="6bbc2-132">Ezekben az esetekben szükség lehet az ügyfelek új szolgáltatásokra való frissítéséhez, vagy az előfizetéseiknek a végül leállítható SKUs-ból való áttelepítéséhez.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-132">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="6bbc2-133">Az ügyfeleknek a visszavont SKUs-ból újabbakra való áttelepítéséhez a következő lépésekre van szükség:</span><span class="sxs-lookup"><span data-stu-id="6bbc2-133">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="6bbc2-134">A.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-134">A.</span></span> <span data-ttu-id="6bbc2-135">Az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="6bbc2-135">Purchase the new subscription</span></span>

<span data-ttu-id="6bbc2-136">B.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-136">B.</span></span> <span data-ttu-id="6bbc2-137">Aktuális felhasználói licencek ismételt hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="6bbc2-137">Reassign current user licenses</span></span>

<span data-ttu-id="6bbc2-138">C.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-138">C.</span></span> <span data-ttu-id="6bbc2-139">Régi előfizetés lemondása</span><span class="sxs-lookup"><span data-stu-id="6bbc2-139">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="6bbc2-140">Ügyfelek áttelepítése új csomagokba</span><span class="sxs-lookup"><span data-stu-id="6bbc2-140">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="6bbc2-141">A.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-141">A.</span></span> <span data-ttu-id="6bbc2-142">Az új előfizetés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="6bbc2-142">Purchase the new subscription</span></span>

1. <span data-ttu-id="6bbc2-143">Az új előfizetés megvásárlásához a Partnerközpont **menüben** válassza az Ügyfelek **lehetőséget,** válassza ki az áthelyezni kívánt ügyfelet, majd válassza az **Előfizetések hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6bbc2-143">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="6bbc2-144">Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikével), adja meg a licencek számát, majd válassza a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6bbc2-144">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="6bbc2-145">Az ügyfélnek most már mind a régi, mind az új előfizetéssel, a régi Önálló Kaizala Pro-előfizetéssel és az új "cél" előfizetéssel kell rendelkezik, például 1. lehetőség – Office 365 Nagyvállalati F1 csomag.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-145">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="6bbc2-146">B.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-146">B.</span></span> <span data-ttu-id="6bbc2-147">Aktuális felhasználói licencek ismételt hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="6bbc2-147">Reassign current user licenses</span></span>

1. <span data-ttu-id="6bbc2-148">Az ügyfél felhasználói licencének ismételt hozzárendelése érdekében  a Partnerközpont menüjében válassza az Ügyfelek **lehetőséget,** válassza ki az áthelyezni kívánt ügyfelet, majd válassza a Felhasználók és licencek **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6bbc2-148">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="6bbc2-149">Megnyílik az ügyfél Felhasználók és licencek lapja.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-149">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="6bbc2-150">A felhasználói licenc ismételt hozzárendeléséhez válassza ki az újra hozzárendelni kívánt felhasználót, majd válassza a **Licencek kezelése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6bbc2-150">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="6bbc2-151">A **Licencek kezelése lapon** törölje a Kaizala Pro Standalone license (Önálló Kaizala Pro-licenc) jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatástervet ahhoz az előfizetéshez, amelybe az ügyfelet átköltöztetik.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-151">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="6bbc2-152">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-152">Select **Submit**.</span></span> <span data-ttu-id="6bbc2-153">A megerősítő oldal felsorolja az új licenc-hozzárendeléseket.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-153">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="6bbc2-154">Ugyanezt a folyamatot folytassa a licenc-hozzárendelést használó többi felhasználóval is.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-154">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="6bbc2-155">C.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-155">C.</span></span> <span data-ttu-id="6bbc2-156">Régi előfizetés lemondása</span><span class="sxs-lookup"><span data-stu-id="6bbc2-156">Cancel old subscription</span></span>

<span data-ttu-id="6bbc2-157">Miután a felhasználói licencet az új szolgáltatásba költözteti, biztonságosan megszüntetheti a megszüntetett előfizetést az ügyfél szintjén.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-157">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="6bbc2-158">A **Partnerközpont** válassza az Ügyfelek **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6bbc2-158">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="6bbc2-159">Válassza ki azt az ügyfelet, akinek az előfizetését lemondja.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-159">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="6bbc2-160">Az előfizetés részletei lapon állítsa az előfizetést **Felfüggesztettre.**</span><span class="sxs-lookup"><span data-stu-id="6bbc2-160">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="6bbc2-161">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-161">Select **Submit**.</span></span>

<span data-ttu-id="6bbc2-162">A régi előfizetés fel van függesztve, és az új előfizetés aktív.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-162">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="6bbc2-163">A felfüggesztett előfizetés 120 nap után automatikusan fel lesz függesztve.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-163">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="6bbc2-164">Az ügyfél nem jár további költségekkel a régi előfizetésért.</span><span class="sxs-lookup"><span data-stu-id="6bbc2-164">The customer incurs no additional costs for the old subscription.</span></span>
