---
title: A Power BI a partner Center Analytics használata
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan tekintheti meg az üzleti adatait a Power BIhez készült partner Center Analytics alkalmazással (a CSP-ben található közvetlen partnereknél).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5bdb166562593b970f40c23921dc80b2a1cb8ad
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633862"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="1f167-103">Üzleti adatai megtekinthetők a Microsoft Power BI partner Center Analytics alkalmazásával</span><span class="sxs-lookup"><span data-stu-id="1f167-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="1f167-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="1f167-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1f167-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="1f167-105">Global admin</span></span>
- <span data-ttu-id="1f167-106">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="1f167-106">User management admin</span></span>
- <span data-ttu-id="1f167-107">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="1f167-107">Sales agent</span></span>
- <span data-ttu-id="1f167-108">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="1f167-108">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="1f167-109">Üzleti adatai megtekintése</span><span class="sxs-lookup"><span data-stu-id="1f167-109">View your business data</span></span>

<span data-ttu-id="1f167-110">Tekintse meg az üzleti adatai vizuális megjelenítését a Power BIhez készült partner Center Analytics-alkalmazással, beleértve a következőket:</span><span class="sxs-lookup"><span data-stu-id="1f167-110">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="1f167-111">Ügyfélkör, előfizetések és licencek növekedése</span><span class="sxs-lookup"><span data-stu-id="1f167-111">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="1f167-112">Az Office 365, a Microsoft Dynamics és a Microsoft Azure termékek használata</span><span class="sxs-lookup"><span data-stu-id="1f167-112">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="1f167-113">Napi fogyasztási egységek minden egyes mért erőforráshoz az elmúlt 60 napra vonatkozóan az egyes Azure-előfizetésekben</span><span class="sxs-lookup"><span data-stu-id="1f167-113">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="1f167-114">Becsült költségek (a legújabb díjszabási kártya alapján)</span><span class="sxs-lookup"><span data-stu-id="1f167-114">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="1f167-115">Lehetőség az adatkészletek exportálására és egyéni jelentések létrehozására, beleértve az ügyfeleket is.</span><span class="sxs-lookup"><span data-stu-id="1f167-115">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="1f167-116">Tudnivalók a partner Center Analytics alkalmazás előzetes kiadásáról</span><span class="sxs-lookup"><span data-stu-id="1f167-116">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="1f167-117">Ez az alkalmazás csak a Cloud Solution Provider program közvetlen partnerei számára érhető el.</span><span class="sxs-lookup"><span data-stu-id="1f167-117">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="1f167-118">A CSP-ben lévő többi partner (például a közvetett viszonteladók) nem tud majd bejelentkezni.</span><span class="sxs-lookup"><span data-stu-id="1f167-118">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="1f167-119">A becsült költségek díjszabása adózási/számlázási, és nem jogilag kötelező.</span><span class="sxs-lookup"><span data-stu-id="1f167-119">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="1f167-120">A becsült költségek csak az adatelemzések esetében használhatók.</span><span class="sxs-lookup"><span data-stu-id="1f167-120">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="1f167-121">Az ügyfél adatai az előfizetéseken alapulnak.</span><span class="sxs-lookup"><span data-stu-id="1f167-121">Customer information is based on subscriptions.</span></span> <span data-ttu-id="1f167-122">Azok az ügyfelek, akikkel a közelmúltban létrehozott fiókokat, de még nem rendelkeznek előfizetéssel, nem számítanak bele a számba.</span><span class="sxs-lookup"><span data-stu-id="1f167-122">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="1f167-123">A becsült költség a legújabb díjszabási kártyán alapul, amely a CSP díjszabásán alapul.</span><span class="sxs-lookup"><span data-stu-id="1f167-123">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="1f167-124">A napok naptári napok.</span><span class="sxs-lookup"><span data-stu-id="1f167-124">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="1f167-125">Üzleti célú adatjelentések</span><span class="sxs-lookup"><span data-stu-id="1f167-125">Business Insights report</span></span>

- <span data-ttu-id="1f167-126">**Ügyfél bérlői**: a megvásárolt előfizetéseket használó ügyfelek eltérő Azure ad-bérlőinak száma</span><span class="sxs-lookup"><span data-stu-id="1f167-126">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="1f167-127">**Új (utolsó 30 nap)**: az új ügyfelek legalább egy előfizetést vásárolnak az elmúlt 30 napban</span><span class="sxs-lookup"><span data-stu-id="1f167-127">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="1f167-128">Forgalom **(utolsó 30 nap)**: az ügyfelek "aktív", "türelmi" vagy "letiltott" előfizetések nélkül</span><span class="sxs-lookup"><span data-stu-id="1f167-128">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="1f167-129">**Új (az elmúlt 24 órában)**: az új ügyfelek legalább egy előfizetést vásárolnak az elmúlt 24 órában</span><span class="sxs-lookup"><span data-stu-id="1f167-129">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="1f167-130">A **becsült havi költség az elmúlt 12 hónapban**: a becsült ÁFA utáni becsült összeg havi száma az elmúlt 12 hónap során összesítve</span><span class="sxs-lookup"><span data-stu-id="1f167-130">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1f167-131">**Becsült költségek termékenként az elmúlt 12 hónapban**: eladott termékek – az elmúlt 12 hónap során összesítve becsült ÁFA után fizetendő összeg.</span><span class="sxs-lookup"><span data-stu-id="1f167-131">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="1f167-132">Ez az állapot a legtöbb bevételt eredményező legfontosabb termékeket jelzi.</span><span class="sxs-lookup"><span data-stu-id="1f167-132">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="1f167-133">Az **elmúlt 12 hónapban** megjelenő ügyfelek: az új ügyfelek és a forgalomban lévő ügyfelek havi hónapja az elmúlt 12 hónap során összesítve</span><span class="sxs-lookup"><span data-stu-id="1f167-133">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1f167-134">**Becsült költségek az ügyfél által az elmúlt 12 hónapban**: az ügyfelek az elmúlt 12 hónapra vonatkozó becsült ÁFA után fizetendő összeg alapján összesítve jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="1f167-134">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="1f167-135">Ez az állapot a legtöbb bevételt eredményező legfontosabb ügyfeleket jelzi.</span><span class="sxs-lookup"><span data-stu-id="1f167-135">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="1f167-136">**Ügyfelek száma termék szerint**: az eladott termékek a társított ügyfelek szerint rendezve.</span><span class="sxs-lookup"><span data-stu-id="1f167-136">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="1f167-137">Ez az állapot a legtöbb ügyfél számára eladott legfontosabb termékeket jelzi.</span><span class="sxs-lookup"><span data-stu-id="1f167-137">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="1f167-138">Előfizetés-áttekintési jelentés</span><span class="sxs-lookup"><span data-stu-id="1f167-138">Subscription Insights report</span></span>

- <span data-ttu-id="1f167-139">**Előfizetés állapota**:</span><span class="sxs-lookup"><span data-stu-id="1f167-139">**Subscription status**:</span></span>

- <span data-ttu-id="1f167-140">Aktív: az "aktív" vagy "a" türelmi állapotba tartozó előfizetések</span><span class="sxs-lookup"><span data-stu-id="1f167-140">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="1f167-141">Felfüggesztve: a "Letiltva" állapothoz tartozó előfizetések</span><span class="sxs-lookup"><span data-stu-id="1f167-141">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="1f167-142">Kiépítve: "kiépített" vagy "lejárt" állapotba tartozó előfizetések</span><span class="sxs-lookup"><span data-stu-id="1f167-142">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="1f167-143">**Lejárati állapot**:</span><span class="sxs-lookup"><span data-stu-id="1f167-143">**Expiry status**:</span></span>

  - <span data-ttu-id="1f167-144">Lejárt: már lejárt előfizetések (az előfizetés lejárati dátuma korábbi)</span><span class="sxs-lookup"><span data-stu-id="1f167-144">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="1f167-145">30 nap után lejár: az előfizetések 30 nap után lejárnak (az előfizetés befejezési dátuma pedig a következő 30 nap után)</span><span class="sxs-lookup"><span data-stu-id="1f167-145">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="1f167-146">30 nap alatt lejár: az előfizetések, amelyek a következő 30 napon belül lejárnak (az előfizetés befejezési dátuma ma és a következő 30 nap között van)</span><span class="sxs-lookup"><span data-stu-id="1f167-146">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="1f167-147">**Összes előfizetés**: az "Active", "" in Grace "vagy" disabled "állapotú előfizetések</span><span class="sxs-lookup"><span data-stu-id="1f167-147">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="1f167-148">**Új (utolsó 30 nap)**: az ügyfelek által az elmúlt 30 napban vásárolt új előfizetések</span><span class="sxs-lookup"><span data-stu-id="1f167-148">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="1f167-149">**Új (az elmúlt 24 óra)**: az ügyfelek által az elmúlt 24 órában vásárolt új előfizetések</span><span class="sxs-lookup"><span data-stu-id="1f167-149">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="1f167-150">**30 nap alatt lejár**: az előfizetések, amelyek a következő 30 napon belül lejárnak</span><span class="sxs-lookup"><span data-stu-id="1f167-150">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="1f167-151">Forgalom **(utolsó 30 nap)**: az elmúlt 30 napban kiosztott vagy felfüggesztett (letiltott) előfizetések</span><span class="sxs-lookup"><span data-stu-id="1f167-151">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="1f167-152">**Elosztás előfizetési típusok** szerint: az összes előfizetés%-os elosztása licenc-alapú és használati alapú előfizetési típus szerint</span><span class="sxs-lookup"><span data-stu-id="1f167-152">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="1f167-153">**Aktív előfizetés darabszáma termékenként**: aktív előfizetések száma szerint értékesített termékek száma</span><span class="sxs-lookup"><span data-stu-id="1f167-153">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="1f167-154">**Előfizetések az elmúlt 12 hónapban**: az új előfizetések és a változási előfizetések hónapja az elmúlt 12 hónap során összesített havi gyakorisággal</span><span class="sxs-lookup"><span data-stu-id="1f167-154">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1f167-155">**Ügyfél-előfizetés részletei**: az ügyfelek, előfizetések és ajánlatok részletes áttekintése</span><span class="sxs-lookup"><span data-stu-id="1f167-155">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="1f167-156">Licencelési jelentés:</span><span class="sxs-lookup"><span data-stu-id="1f167-156">License Insights report:</span></span>

- <span data-ttu-id="1f167-157">Összes **licenc**: teljes licenc-alapú előfizetések összesített száma</span><span class="sxs-lookup"><span data-stu-id="1f167-157">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="1f167-158">**Új (utolsó 30 nap)**: licenc hozzáadása az elmúlt 30 napban</span><span class="sxs-lookup"><span data-stu-id="1f167-158">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="1f167-159">Adatforgalom **(utolsó 30 nap)**: a licencek csökkentése az elmúlt 30 napban</span><span class="sxs-lookup"><span data-stu-id="1f167-159">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="1f167-160">**Új (utolsó 24 óra)**: licenc hozzáadása az elmúlt 24 órában</span><span class="sxs-lookup"><span data-stu-id="1f167-160">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="1f167-161">Az **elmúlt 90 napra vonatkozó licencek**: a licencek hozzáadásának hónapja, valamint az elmúlt 90 nap során összesített havi összesítések.</span><span class="sxs-lookup"><span data-stu-id="1f167-161">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="1f167-162">**Aktív licencek száma termék szerint**: az eladott termékek aktív licencek száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="1f167-162">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="1f167-163">**Aktív licencek száma ügyfél szerint**: az ügyfelek az aktív licencek száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="1f167-163">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="1f167-164">**Ügyfél-licencelési esemény részletei az elmúlt 90 napban**: az ügyfelek, előfizetések és előfizetési események részletes nézete, beleértve az esemény dátumát, az esemény nevét, a mennyiséget és a mennyiség változását.</span><span class="sxs-lookup"><span data-stu-id="1f167-164">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="1f167-165">Licencek használati jelentése:</span><span class="sxs-lookup"><span data-stu-id="1f167-165">Licenses Usage report:</span></span>

- <span data-ttu-id="1f167-166">**A termék által hozzárendelt licencek**: az eladott termékek licenc-hozzárendelések száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="1f167-166">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="1f167-167">**Termék által használt licencek**: a licencek használati száma szerint rendezve értékesített termékek</span><span class="sxs-lookup"><span data-stu-id="1f167-167">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="1f167-168">**A hozzárendelt licencek ügyfél-eloszlása**: a teljes ügyfelek%-os elosztása a licenc-hozzárendeléssel számított 20%-ban</span><span class="sxs-lookup"><span data-stu-id="1f167-168">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="1f167-169">A **használatban lévő licencek ügyfél-eloszlása**:%-ban a teljes ügyfél%-os elosztása a licencek kihasználtsága alapján%-kal megszakadt.</span><span class="sxs-lookup"><span data-stu-id="1f167-169">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="1f167-170">**Ügyfél által hozzárendelt licencek**: az eladott licencek és az ügyfelek és termékek által hozzárendelt licencek részletes nézete</span><span class="sxs-lookup"><span data-stu-id="1f167-170">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="1f167-171">**Ügyfél által használt licencek**: az eladott licencek és az ügyfelek és termékek által használt licencek részletes nézete</span><span class="sxs-lookup"><span data-stu-id="1f167-171">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="1f167-172">Azure-beli bepillantást ismertető jelentés:</span><span class="sxs-lookup"><span data-stu-id="1f167-172">Azure Insights report:</span></span>

- <span data-ttu-id="1f167-173">A **használaton alapuló ügyfelek az elmúlt 12 hónapban**: az új, használati alapú ügyfelek és a felhasználható használaton alapuló ügyfelek havi hónapjának trendje az elmúlt 12 hónap során összesítve</span><span class="sxs-lookup"><span data-stu-id="1f167-173">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1f167-174">**Használaton alapuló előfizetések az elmúlt 12 hónapban**: az új használati-alapú előfizetések és a felhasználható használaton alapuló előfizetések havi hónapja az elmúlt 12 hónap során összesítve</span><span class="sxs-lookup"><span data-stu-id="1f167-174">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1f167-175">Az **ügyfél által az elmúlt 60 napban becsült használati költségek**: a használaton alapuló ügyfelek az utolsó 60 nap során összesítve becsült ÁFA nélküli számla összegét használják.</span><span class="sxs-lookup"><span data-stu-id="1f167-175">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="1f167-176">Ez az állapot a legtöbb bevételt eredményező, legszélesebb körű használatú ügyfeleket jelzi</span><span class="sxs-lookup"><span data-stu-id="1f167-176">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="1f167-177">A **becsült használati költségek kategóriánként az elmúlt 60 napban**: a használati alapú előfizetések kategóriái az utolsó 60 nap során összesített, a számlán becsült, ÁFA nélküli számla összegével.</span><span class="sxs-lookup"><span data-stu-id="1f167-177">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="1f167-178">Az **előfizetés becsült használati díja az elmúlt 60 napban**: a használaton alapuló előfizetések száma az utolsó 60 nap során összesített, ÁFA nélkül számlázott összeg alapján.</span><span class="sxs-lookup"><span data-stu-id="1f167-178">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="1f167-179">Az **ügyfél becsült használati díja költségvetés szerint**: az ügyfelek a jelenlegi használati költségkeretük százalékában meghaladják a küszöbértéket (100%).</span><span class="sxs-lookup"><span data-stu-id="1f167-179">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="1f167-180">Azure-Erőforrás-használati jelentés:</span><span class="sxs-lookup"><span data-stu-id="1f167-180">Azure Resource Usage report:</span></span>

- <span data-ttu-id="1f167-181">Az **Azure-erőforrások napi használata a kiválasztott időszakra** vonatkozóan: az elmúlt 60 napon belül minden használaton alapuló előfizetéshez tartozó napi fogyasztási egység</span><span class="sxs-lookup"><span data-stu-id="1f167-181">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="1f167-182">A **kiválasztott időszakra vonatkozó Azure-erőforrások becsült használati díja**: az elmúlt 60 napban megadott időszakra vonatkozó, a legújabb díjszabási kártyán alapuló becsült költségek az egyes használati alapú előfizetésekben</span><span class="sxs-lookup"><span data-stu-id="1f167-182">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="1f167-183">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="1f167-183">Next steps</span></span>

- [<span data-ttu-id="1f167-184">A Power BI alkalmazáshoz készült partner Center Analytics áttekintése</span><span class="sxs-lookup"><span data-stu-id="1f167-184">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="1f167-185">A Partnerközpont adatelemzési alkalmazás a Microsoft Power BI-hoz telepítése és előzetes verziója</span><span class="sxs-lookup"><span data-stu-id="1f167-185">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
