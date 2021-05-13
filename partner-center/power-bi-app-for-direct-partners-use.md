---
title: A Partnerközpont Analytics használata Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan megtekintheti üzleti adatait a Partnerközpont adatelemzési alkalmazás a Power BI-hoz használatával (a CSP közvetlen partnerei számára).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855029"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="71799-103">Üzleti adatok megtekintése a Microsoft Partnerközpont Analytics alkalmazással Power BI</span><span class="sxs-lookup"><span data-stu-id="71799-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="71799-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Értékesítési ügynök | Rendszergazdai ügynök</span><span class="sxs-lookup"><span data-stu-id="71799-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="71799-105">Üzleti adatok megtekintése</span><span class="sxs-lookup"><span data-stu-id="71799-105">View your business data</span></span>

<span data-ttu-id="71799-106">Az üzleti adatok vizuális ábrázolása a Partnerközpont adatelemzési alkalmazás a Power BI-hoz:</span><span class="sxs-lookup"><span data-stu-id="71799-106">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="71799-107">Az ügyfélkör, az előfizetések és a licencek növekedése</span><span class="sxs-lookup"><span data-stu-id="71799-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="71799-108">Az Office 365, a Microsoft Dynamics és a Microsoft Azure használata</span><span class="sxs-lookup"><span data-stu-id="71799-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="71799-109">Az egyes Azure-előfizetések forgalmi díjas erőforrásának napi fogyasztási egységei az elmúlt 60 napra</span><span class="sxs-lookup"><span data-stu-id="71799-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="71799-110">Becsült költség (a legújabb díjkártya alapján)</span><span class="sxs-lookup"><span data-stu-id="71799-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="71799-111">Lehetőség az adatkészletek exportálására és egyéni jelentések létrehozására, ügyfélenként is.</span><span class="sxs-lookup"><span data-stu-id="71799-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="71799-112">A Partnerközpont Analytics alkalmazás előzetes kiadásának adatai</span><span class="sxs-lookup"><span data-stu-id="71799-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="71799-113">Ez az alkalmazás csak a közvetlen partnerek számára Felhőszolgáltató programjában.</span><span class="sxs-lookup"><span data-stu-id="71799-113">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="71799-114">A CSP más partnerei (például közvetett viszonteladók) nem fognak tudni bejelentkezni.</span><span class="sxs-lookup"><span data-stu-id="71799-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="71799-115">A becsült költségek az adók számlázása előtti/számlaadatok, és nem kötelezőek.</span><span class="sxs-lookup"><span data-stu-id="71799-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="71799-116">A becsült költségek csak adatelemzéshez használhatók.</span><span class="sxs-lookup"><span data-stu-id="71799-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="71799-117">Az ügyféladatok előfizetésen alapulnak.</span><span class="sxs-lookup"><span data-stu-id="71799-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="71799-118">Azok az ügyfelek, akikhez a közelmúltban létrehozott fiókokat, de még nem rendelkezik előfizetésekkel, nem szerepelnek a darabszámban.</span><span class="sxs-lookup"><span data-stu-id="71799-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="71799-119">A becsült költség a legújabb díjszabású kártyán alapul, amely a CSP díjszabásán alapul.</span><span class="sxs-lookup"><span data-stu-id="71799-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="71799-120">A napok naptári napok.</span><span class="sxs-lookup"><span data-stu-id="71799-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="71799-121">Business Insights-jelentés</span><span class="sxs-lookup"><span data-stu-id="71799-121">Business Insights report</span></span>

- <span data-ttu-id="71799-122">**Ügyfélbérlők:** Azon ügyfelek különböző Azure AD-bérlőinek száma, akik előfizetéseket vásároltak</span><span class="sxs-lookup"><span data-stu-id="71799-122">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="71799-123">**Új (az elmúlt 30 nap)**: Új ügyfelek, akik legalább egy előfizetést vásárolnak az elmúlt 30 napban</span><span class="sxs-lookup"><span data-stu-id="71799-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="71799-124">**Adatváltozás (az elmúlt 30 nap)**: "aktív", "türelmi" vagy "letiltott" előfizetéssel nem</span><span class="sxs-lookup"><span data-stu-id="71799-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="71799-125">**Új (az elmúlt 24 óra)**: Új ügyfelek, akik legalább egy előfizetést vásárolnak az elmúlt 24 órában</span><span class="sxs-lookup"><span data-stu-id="71799-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="71799-126">Becsült havi költség az elmúlt 12 hónapra: Az adók előtti számlás dollárban becsült összeg havi összesítése az elmúlt **12** hónap időszakában</span><span class="sxs-lookup"><span data-stu-id="71799-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="71799-127">**Termékonkénti becsült** költség az elmúlt 12 hónapra vonatkozóan: Az értékesített termékek az adók előtti számlás dollárban becsült összeg szerint rendezve, az elmúlt 12 hónapra vonatkozóan összesítve.</span><span class="sxs-lookup"><span data-stu-id="71799-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="71799-128">Ez az állapot a legtöbb bevételt hozó leggyakoribb termékeket jelzi.</span><span class="sxs-lookup"><span data-stu-id="71799-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="71799-129">**Az elmúlt 12** hónap ügyfelei: Az új ügyfelek és a lemorzsolódási ügyfelek havi trendje az elmúlt 12 hónapra vonatkozóan havonta</span><span class="sxs-lookup"><span data-stu-id="71799-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="71799-130">Becsült költség ügyfél szerint az elmúlt **12** hónapra vonatkozóan: Ügyfelek az adók előtti, dollárban számlázott becsült összeg szerint rendezve az elmúlt 12 hónapra vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="71799-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="71799-131">Ez az állapot a legtöbb bevételt hozó leggyakoribb ügyfeleket jelzi.</span><span class="sxs-lookup"><span data-stu-id="71799-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="71799-132">**Ügyfelek száma termék szerint:** A társított ügyfelek szerint rendezve értékesített termékek.</span><span class="sxs-lookup"><span data-stu-id="71799-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="71799-133">Ez az állapot a legtöbb ügyfél számára értékesített legnépszerűbb termékeket jelzi.</span><span class="sxs-lookup"><span data-stu-id="71799-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="71799-134">Subscription Insights-jelentés</span><span class="sxs-lookup"><span data-stu-id="71799-134">Subscription Insights report</span></span>

- <span data-ttu-id="71799-135">**Előfizetés állapota:**</span><span class="sxs-lookup"><span data-stu-id="71799-135">**Subscription status**:</span></span>

- <span data-ttu-id="71799-136">Aktív: "aktív" vagy "türelmi" állapothoz tartozó előfizetések</span><span class="sxs-lookup"><span data-stu-id="71799-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="71799-137">Felfüggesztve: "Letiltott" állapothoz tartozó előfizetések</span><span class="sxs-lookup"><span data-stu-id="71799-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="71799-138">Kiépítve: A "kiépítve" vagy "lejárt" állapothoz tartozó előfizetések</span><span class="sxs-lookup"><span data-stu-id="71799-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="71799-139">**Lejárati állapot:**</span><span class="sxs-lookup"><span data-stu-id="71799-139">**Expiry status**:</span></span>

  - <span data-ttu-id="71799-140">Lejárt: Lejárt előfizetések (ha az előfizetés záró dátuma lejárt)</span><span class="sxs-lookup"><span data-stu-id="71799-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="71799-141">Lejárat 30 nap után: 30 nap után lejáró előfizetések (ahol az előfizetés záró dátuma a következő 30 nap után lesz)</span><span class="sxs-lookup"><span data-stu-id="71799-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="71799-142">Lejárat 30 napon belül: A következő 30 napon belül lejáró előfizetések (ahol az előfizetés záró dátuma ma és a következő 30 nap között van)</span><span class="sxs-lookup"><span data-stu-id="71799-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="71799-143">**Összes előfizetés:**"aktív", "türelmi" vagy "letiltott" állapotú előfizetések</span><span class="sxs-lookup"><span data-stu-id="71799-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="71799-144">**Új (az elmúlt 30 nap)**: Az ügyfelek által az elmúlt 30 napban vásárolt új előfizetések</span><span class="sxs-lookup"><span data-stu-id="71799-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="71799-145">**Új (az elmúlt 24 óra)**: Az ügyfelek által az elmúlt 24 órában vásárolt új előfizetések</span><span class="sxs-lookup"><span data-stu-id="71799-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="71799-146">**Lejárat 30 napon belül:** A következő 30 napon belül lejáró előfizetések</span><span class="sxs-lookup"><span data-stu-id="71799-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="71799-147">**Adatváltozás (az elmúlt 30 nap)**: Az elmúlt 30 napban fel nem adott vagy felfüggesztett előfizetések</span><span class="sxs-lookup"><span data-stu-id="71799-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="71799-148">**Elosztás előfizetés-típusok szerint:** Az összes előfizetés százalékos eloszlása licencalapú és használatalapú előfizetés-típus szerint</span><span class="sxs-lookup"><span data-stu-id="71799-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="71799-149">**Aktív előfizetések száma termék szerint:** Az értékesített termékek az aktív előfizetések száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="71799-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="71799-150">**Az elmúlt 12** hónapra vonatkozó előfizetések: Az új előfizetések és a lemorzsolódási előfizetések havi összesítése az elmúlt 12 hónapra vonatkozóan</span><span class="sxs-lookup"><span data-stu-id="71799-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="71799-151">**Ügyfél-előfizetés részletei:** Az ügyfelek, előfizetések és ajánlatok részletes nézete</span><span class="sxs-lookup"><span data-stu-id="71799-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="71799-152">License Insights-jelentés:</span><span class="sxs-lookup"><span data-stu-id="71799-152">License Insights report:</span></span>

- <span data-ttu-id="71799-153">**Összes licenc:** Az összes licencalapú előfizetésben összesített licencek teljes száma</span><span class="sxs-lookup"><span data-stu-id="71799-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="71799-154">**Új (az elmúlt 30 nap)**: Licenc összeadása az elmúlt 30 napon belül</span><span class="sxs-lookup"><span data-stu-id="71799-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="71799-155">**Adatváltozás (az elmúlt 30 nap)**: Licenc csökkentése az elmúlt 30 napon belül</span><span class="sxs-lookup"><span data-stu-id="71799-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="71799-156">**Új (az elmúlt 24 óra)**: Licenc összeadása az elmúlt 24 órában</span><span class="sxs-lookup"><span data-stu-id="71799-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="71799-157">**Licencek az elmúlt 90 napban:** A licencek kiegészítésének és csökkentésének havi trendje az elmúlt 90 napban havonta</span><span class="sxs-lookup"><span data-stu-id="71799-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="71799-158">**Aktív licencek száma termék szerint:** Aktív licencek száma szerint rendezve értékesített termékek</span><span class="sxs-lookup"><span data-stu-id="71799-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="71799-159">**Aktív licencek száma ügyfél szerint:** Az ügyfelek az aktív licencek száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="71799-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="71799-160">Ügyféllicenc-esemény adatai az elmúlt **90 napban:** Az ügyfelek, előfizetések és előfizetési események részletes nézete, beleértve az esemény dátumát, az esemény nevét, a mennyiséget és a mennyiség változását.</span><span class="sxs-lookup"><span data-stu-id="71799-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="71799-161">Licenchasználati jelentés:</span><span class="sxs-lookup"><span data-stu-id="71799-161">Licenses Usage report:</span></span>

- <span data-ttu-id="71799-162">**Termék szerint hozzárendelt licencek:** Eladott termékek licenc-hozzárendelések száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="71799-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="71799-163">**Termék szerint használt licencek:** Eladott termékek a licenchasználat száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="71799-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="71799-164">**Hozzárendelt licencek ügyfélelosztása:** Az összes ügyfél százalékos eloszlása 20%-os tartományba osztva licenc-hozzárendelés alapján %</span><span class="sxs-lookup"><span data-stu-id="71799-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="71799-165">**Használatban található licencek ügyfélelosztása:** Az összes ügyfél százalékos eloszlása, 20%-os tartományba oszlása licenchasználat szerint %</span><span class="sxs-lookup"><span data-stu-id="71799-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="71799-166">**Az ügyfél által hozzárendelt licencek:** Az ügyfelek és termékek által hozzárendelt eladott licencek és licencek részletes nézete</span><span class="sxs-lookup"><span data-stu-id="71799-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="71799-167">**Az ügyfél által használt licencek:** Az ügyfelek és termékek által használt eladott licencek és licencek részletes nézete</span><span class="sxs-lookup"><span data-stu-id="71799-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="71799-168">Azure Insights-jelentés:</span><span class="sxs-lookup"><span data-stu-id="71799-168">Azure Insights report:</span></span>

- <span data-ttu-id="71799-169">Használatalapú ügyfelek az elmúlt **12** hónapra vonatkozóan: Az új használatalapú ügyfelek és a lemorzsolódáson alapuló ügyfelek havi összesítése az elmúlt 12 hónap időszakában</span><span class="sxs-lookup"><span data-stu-id="71799-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="71799-170">Használatalapú előfizetések az elmúlt **12** hónapra: Az új használatalapú előfizetések és a lemorzsolódáson alapuló előfizetések havi összesítése az elmúlt 12 hónap időszakában</span><span class="sxs-lookup"><span data-stu-id="71799-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="71799-171">Az ügyfél által az elmúlt 60 nap becsült használati költsége: Használatalapú ügyfelek, az elmúlt **60** napban összesített, az adók előtti, dollárban becsült összeg alapján rendezve.</span><span class="sxs-lookup"><span data-stu-id="71799-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="71799-172">Ez az állapot a legnagyobb bevételt hozó, használaton alapuló ügyfeleket jelzi</span><span class="sxs-lookup"><span data-stu-id="71799-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="71799-173">Becsült használati költség kategória szerint az elmúlt 60 napban: Használatalapú előfizetések mérőkategóriái az elmúlt **60** napban összesített, adók előtti, dollárban becsült összeg szerint rendezve.</span><span class="sxs-lookup"><span data-stu-id="71799-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="71799-174">Becsült használati költség előfizetés szerint az elmúlt **60** napban: Használatalapú előfizetések az adók előtti számlás dollárban becsült összeg szerint, az elmúlt 60 napban összesítve.</span><span class="sxs-lookup"><span data-stu-id="71799-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="71799-175">**Az ügyfelek becsült használati költségei költségkeret** szerint: Az ügyfelek a jelenlegi használati költségkeretük százalékos aránya szerint haladják meg a küszöbértéket (100%).</span><span class="sxs-lookup"><span data-stu-id="71799-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="71799-176">Azure-erőforráshasználati jelentés:</span><span class="sxs-lookup"><span data-stu-id="71799-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="71799-177">**Az Azure-erőforrások** napi használata a kiválasztott időszakban: Az elmúlt 60 nap egyes használatalapú előfizetésében az egyes forgalmi díjas erőforrások napi használati egységei.</span><span class="sxs-lookup"><span data-stu-id="71799-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="71799-178">**Az Azure-erőforrások** becsült használati költsége a kiválasztott időszakra vonatkozóan: Az egyes használatalapú előfizetések minden egyes forgalmi díjas erőforrásának becsült költsége az elmúlt 60 napra vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="71799-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="71799-179">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="71799-179">Next steps</span></span>

- [<span data-ttu-id="71799-180">Partnerközpont Analytics for Power BI alkalmazás áttekintése</span><span class="sxs-lookup"><span data-stu-id="71799-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="71799-181">A Partnerközpont adatelemzési alkalmazás a Microsoft Power BI-hoz telepítése és előzetes verziója</span><span class="sxs-lookup"><span data-stu-id="71799-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
