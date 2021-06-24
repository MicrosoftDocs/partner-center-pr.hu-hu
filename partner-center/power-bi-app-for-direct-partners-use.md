---
title: A Partnerközpont Analytics használata Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Útmutató üzleti adatainak megtekintéséhez a Partnerközpont adatelemzési alkalmazás a Power BI-hoz használatával (a Felhőszolgáltató (CSP) program közvetlen partnerei számára).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564981"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="22b0b-103">Üzleti adatok megtekintése a Microsoft Partnerközpont Analytics alkalmazással Power BI</span><span class="sxs-lookup"><span data-stu-id="22b0b-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="22b0b-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Értékesítési ügynök | Rendszergazdai ügynök</span><span class="sxs-lookup"><span data-stu-id="22b0b-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="22b0b-105">Üzleti adatok megtekintése</span><span class="sxs-lookup"><span data-stu-id="22b0b-105">View your business data</span></span>

<span data-ttu-id="22b0b-106">Az üzleti adatok vizuális ábrázolása a Microsoft Partnerközpont Analytics alkalmazással, többek között a következő Power BI le:</span><span class="sxs-lookup"><span data-stu-id="22b0b-106">Get a visual representation of your business data with the Partner Center Analytics app for Microsoft Power BI, including:</span></span>

- <span data-ttu-id="22b0b-107">Az ügyfélkör, az előfizetések és a licencek növekedése</span><span class="sxs-lookup"><span data-stu-id="22b0b-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="22b0b-108">Office 365-, Microsoft Dynamics- és Microsoft Azure termékek használata</span><span class="sxs-lookup"><span data-stu-id="22b0b-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="22b0b-109">Az egyes Azure-előfizetések forgalmi díjas erőforrásának napi fogyasztási egységei az elmúlt 60 napra</span><span class="sxs-lookup"><span data-stu-id="22b0b-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="22b0b-110">Becsült költség (a legújabb díjkártya alapján)</span><span class="sxs-lookup"><span data-stu-id="22b0b-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="22b0b-111">Lehetőség az adatkészletek exportálására és egyéni jelentések létrehozására, beleértve az ügyfélenkénti jelentéseket is.</span><span class="sxs-lookup"><span data-stu-id="22b0b-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="22b0b-112">A Partnerközpont Analytics alkalmazás előzetes kiadásának adatai</span><span class="sxs-lookup"><span data-stu-id="22b0b-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="22b0b-113">Ez az alkalmazás csak a Felhőszolgáltató (CSP) program közvetlen partnerei számára való.</span><span class="sxs-lookup"><span data-stu-id="22b0b-113">This app is for direct partners in the Cloud Solution Provider (CSP) program only.</span></span> <span data-ttu-id="22b0b-114">A CSP más partnerei (például közvetett viszonteladók) nem tudnak bejelentkezni.</span><span class="sxs-lookup"><span data-stu-id="22b0b-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="22b0b-115">A becsült költségek adók előtti számlázási/számlaadatok, és nem kötelezőek.</span><span class="sxs-lookup"><span data-stu-id="22b0b-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="22b0b-116">A becsült költségek csak adatelemzéshez használhatók.</span><span class="sxs-lookup"><span data-stu-id="22b0b-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="22b0b-117">Az ügyféladatok az előfizetésen alapulnak.</span><span class="sxs-lookup"><span data-stu-id="22b0b-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="22b0b-118">Azok az ügyfelek, akikhez a közelmúltban létrehozott fiókokat, de még nem rendelkezik előfizetésekkel, nem szerepelnek a darabszámok között.</span><span class="sxs-lookup"><span data-stu-id="22b0b-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="22b0b-119">A becsült költség a legújabb díjszabású kártyán alapul, amely a CSP díjszabásán alapul.</span><span class="sxs-lookup"><span data-stu-id="22b0b-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="22b0b-120">A napok naptári napok.</span><span class="sxs-lookup"><span data-stu-id="22b0b-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="22b0b-121">Business Insights-jelentés</span><span class="sxs-lookup"><span data-stu-id="22b0b-121">Business Insights report</span></span>

- <span data-ttu-id="22b0b-122">**Ügyfélbérlők:** Az előfizetéseket Azure Active Directory (Azure AD-) ügyfelek különböző bérlőinek száma</span><span class="sxs-lookup"><span data-stu-id="22b0b-122">**Customer tenants**: Number of distinct Azure Active Directory (Azure AD) tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="22b0b-123">**Új (az elmúlt 30 nap)**: Új ügyfelek, akik legalább egy előfizetést vásárolnak az elmúlt 30 napban</span><span class="sxs-lookup"><span data-stu-id="22b0b-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="22b0b-124">**Adatváltozás (az elmúlt 30 nap)**: "aktív", "türelmi" vagy "letiltott" előfizetéssel nem</span><span class="sxs-lookup"><span data-stu-id="22b0b-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="22b0b-125">**Új (az elmúlt 24 óra)**: Új ügyfelek, akik legalább egy előfizetést vásárolnak az elmúlt 24 órában</span><span class="sxs-lookup"><span data-stu-id="22b0b-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="22b0b-126">Becsült havi költség az elmúlt 12 hónapra: Az adók előtti számlás dollárban becsült összeg havi összesítése az elmúlt **12** hónap időszakában</span><span class="sxs-lookup"><span data-stu-id="22b0b-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="22b0b-127">**Termékonkénti becsült** költség az elmúlt 12 hónapra vonatkozóan: Az értékesített termékek az adók előtti számlás dollárban becsült összeg szerint rendezve, az elmúlt 12 hónapra vonatkozóan összesítve.</span><span class="sxs-lookup"><span data-stu-id="22b0b-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="22b0b-128">Ez az állapot a legtöbb bevételt hozó leggyakoribb termékeket jelzi.</span><span class="sxs-lookup"><span data-stu-id="22b0b-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="22b0b-129">**Az elmúlt 12** hónap ügyfelei: Az új ügyfelek és a lemorzsolódási ügyfelek havi trendje az elmúlt 12 hónapra vonatkozóan havonta</span><span class="sxs-lookup"><span data-stu-id="22b0b-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="22b0b-130">Becsült költség ügyfél szerint az elmúlt **12** hónapra vonatkozóan: Ügyfelek az adók előtti, dollárban számlázott becsült összeg szerint rendezve az elmúlt 12 hónapra vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="22b0b-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="22b0b-131">Ez az állapot a legtöbb bevételt hozó leggyakoribb ügyfeleket jelzi.</span><span class="sxs-lookup"><span data-stu-id="22b0b-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="22b0b-132">**Ügyfelek száma termék szerint:** A társított ügyfelek szerint rendezve értékesített termékek.</span><span class="sxs-lookup"><span data-stu-id="22b0b-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="22b0b-133">Ez az állapot a legtöbb ügyfél számára értékesített legnépszerűbb termékeket jelzi.</span><span class="sxs-lookup"><span data-stu-id="22b0b-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="22b0b-134">Subscription Insights-jelentés</span><span class="sxs-lookup"><span data-stu-id="22b0b-134">Subscription Insights report</span></span>

- <span data-ttu-id="22b0b-135">**Előfizetés állapota:**</span><span class="sxs-lookup"><span data-stu-id="22b0b-135">**Subscription status**:</span></span>

- <span data-ttu-id="22b0b-136">Aktív: "aktív" vagy "türelmi" állapothoz tartozó előfizetések</span><span class="sxs-lookup"><span data-stu-id="22b0b-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="22b0b-137">Felfüggesztve: "Letiltott" állapothoz tartozó előfizetések</span><span class="sxs-lookup"><span data-stu-id="22b0b-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="22b0b-138">Kiépítve: A "kiépítve" vagy "lejárt" állapothoz tartozó előfizetések</span><span class="sxs-lookup"><span data-stu-id="22b0b-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="22b0b-139">**Lejárati állapot:**</span><span class="sxs-lookup"><span data-stu-id="22b0b-139">**Expiry status**:</span></span>

  - <span data-ttu-id="22b0b-140">Lejárt: Lejárt előfizetések (ha az előfizetés záró dátuma lejárt)</span><span class="sxs-lookup"><span data-stu-id="22b0b-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="22b0b-141">Lejárat 30 nap után: 30 nap után lejáró előfizetések (ahol az előfizetés záró dátuma a következő 30 nap után lesz)</span><span class="sxs-lookup"><span data-stu-id="22b0b-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="22b0b-142">Lejárat 30 napon belül: A következő 30 napon belül lejáró előfizetések (ahol az előfizetés záró dátuma ma és a következő 30 nap között van)</span><span class="sxs-lookup"><span data-stu-id="22b0b-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="22b0b-143">**Összes előfizetés:** Az "aktív", a "türelmi időszakban" vagy a "letiltva" állapotú előfizetések</span><span class="sxs-lookup"><span data-stu-id="22b0b-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="22b0b-144">**Új (az elmúlt 30 nap)**: Az ügyfelek által az elmúlt 30 napban vásárolt új előfizetések</span><span class="sxs-lookup"><span data-stu-id="22b0b-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="22b0b-145">**Új (az elmúlt 24 óra)**: Az ügyfelek által az elmúlt 24 órában vásárolt új előfizetések</span><span class="sxs-lookup"><span data-stu-id="22b0b-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="22b0b-146">**Lejárat 30 napon belül:** A következő 30 napon belül lejáró előfizetések</span><span class="sxs-lookup"><span data-stu-id="22b0b-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="22b0b-147">**Adatváltozás (az elmúlt 30 nap)**: Az elmúlt 30 napban fel lett függesztve vagy fel lett függesztve (letiltva) előfizetések</span><span class="sxs-lookup"><span data-stu-id="22b0b-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="22b0b-148">**Elosztás előfizetés-típusok szerint:** Az összes előfizetés százalékos eloszlása licencalapú és használatalapú előfizetés-típus szerint</span><span class="sxs-lookup"><span data-stu-id="22b0b-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="22b0b-149">**Aktív előfizetések száma termék szerint:** Eladott termékek az aktív előfizetések száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="22b0b-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="22b0b-150">**Előfizetések az elmúlt 12 hónapra:** Az új előfizetések és a lemorzsolódási előfizetések havi trendje az elmúlt 12 hónapra vonatkozóan</span><span class="sxs-lookup"><span data-stu-id="22b0b-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="22b0b-151">**Ügyfél-előfizetés részletei:** Az ügyfelek, előfizetések és ajánlatok részletes nézete</span><span class="sxs-lookup"><span data-stu-id="22b0b-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="22b0b-152">License Insights-jelentés:</span><span class="sxs-lookup"><span data-stu-id="22b0b-152">License Insights report:</span></span>

- <span data-ttu-id="22b0b-153">**Összes licenc:** Az összes licencalapú előfizetésben összesített licencek teljes száma</span><span class="sxs-lookup"><span data-stu-id="22b0b-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="22b0b-154">**Új (az elmúlt 30 nap)**: Licenc összeadása az elmúlt 30 napon belül</span><span class="sxs-lookup"><span data-stu-id="22b0b-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="22b0b-155">**Adatváltozás (az elmúlt 30 nap)**: Licenc csökkentése az elmúlt 30 napon belül</span><span class="sxs-lookup"><span data-stu-id="22b0b-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="22b0b-156">**Új (az elmúlt 24 óra)**: Licenc összeadása az elmúlt 24 órában</span><span class="sxs-lookup"><span data-stu-id="22b0b-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="22b0b-157">**Licencek az elmúlt 90 napban:** A licencek kiegészítésének és csökkentésének havi trendje az elmúlt 90 napban havonta</span><span class="sxs-lookup"><span data-stu-id="22b0b-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="22b0b-158">**Aktív licencek száma termék szerint:** Eladott termékek aktív licencek száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="22b0b-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="22b0b-159">**Aktív licencek száma ügyfél szerint:** Az ügyfelek az aktív licencek száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="22b0b-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="22b0b-160">Ügyféllicenc-esemény adatai az elmúlt **90 napban:** Az ügyfelek, előfizetések és előfizetési események részletes nézete, beleértve az esemény dátumát, az esemény nevét, a mennyiséget és a mennyiség változását.</span><span class="sxs-lookup"><span data-stu-id="22b0b-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="22b0b-161">Licenchasználati jelentés:</span><span class="sxs-lookup"><span data-stu-id="22b0b-161">Licenses Usage report:</span></span>

- <span data-ttu-id="22b0b-162">**Termék szerint hozzárendelt licencek:** Eladott termékek licenc-hozzárendelések száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="22b0b-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="22b0b-163">**Termék szerint használt licencek:** Eladott termékek a licenchasználat száma szerint rendezve</span><span class="sxs-lookup"><span data-stu-id="22b0b-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="22b0b-164">**Hozzárendelt licencek ügyfélelosztása:** Az összes ügyfél százalékos eloszlása 20%-os tartományra bontva licenc-hozzárendelés alapján %</span><span class="sxs-lookup"><span data-stu-id="22b0b-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="22b0b-165">**Használatban található licencek ügyfélelosztása:** Az összes ügyfél százalékos eloszlása, 20%-os tartományba oszlása licenchasználat szerint %</span><span class="sxs-lookup"><span data-stu-id="22b0b-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="22b0b-166">**Az ügyfél által hozzárendelt licencek:** Az ügyfelek és termékek által hozzárendelt eladott licencek és licencek részletes nézete</span><span class="sxs-lookup"><span data-stu-id="22b0b-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="22b0b-167">**Az ügyfél által használt licencek:** Az ügyfelek és termékek által használt eladott licencek és licencek részletes nézete</span><span class="sxs-lookup"><span data-stu-id="22b0b-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="22b0b-168">Azure Insights-jelentés:</span><span class="sxs-lookup"><span data-stu-id="22b0b-168">Azure Insights report:</span></span>

- <span data-ttu-id="22b0b-169">Használatalapú ügyfelek az elmúlt **12** hónapra vonatkozóan: Az új használatalapú ügyfelek és a lemorzsolódáson alapuló ügyfelek havi összesítése az elmúlt 12 hónap időszakában</span><span class="sxs-lookup"><span data-stu-id="22b0b-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="22b0b-170">Használatalapú előfizetések az elmúlt **12** hónapra: Az új használatalapú előfizetések és a lemorzsolódáson alapuló előfizetések havi összesítése az elmúlt 12 hónap időszakában</span><span class="sxs-lookup"><span data-stu-id="22b0b-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="22b0b-171">Az ügyfél által az elmúlt **60** nap becsült használati költsége: Használatalapú ügyfelek az adók előtti számlás dollárban becsült összeg szerint rendezve az elmúlt 60 napban.</span><span class="sxs-lookup"><span data-stu-id="22b0b-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="22b0b-172">Ez az állapot a legnagyobb bevételt hozó, használaton alapuló ügyfeleket jelzi</span><span class="sxs-lookup"><span data-stu-id="22b0b-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="22b0b-173">Becsült használati költség kategória szerint az elmúlt **60** napra vonatkozóan: Használatalapú előfizetések fogyasztásmérő-kategóriái, az elmúlt 60 nap során összesített, adók előtti, dollárban becsült összeg szerint rendezve.</span><span class="sxs-lookup"><span data-stu-id="22b0b-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="22b0b-174">Becsült használati költség előfizetés szerint az elmúlt **60** napban: Használatalapú előfizetések az adók előtti számlás dollárban becsült összeg szerint, az elmúlt 60 napban összesítve.</span><span class="sxs-lookup"><span data-stu-id="22b0b-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="22b0b-175">**Az ügyfelek becsült használati költsége a** költségkeret alapján: Az ügyfelek a jelenlegi használati költségkeretük százalékos aránya szerint rendezve túllépik a küszöbértéket (100%).</span><span class="sxs-lookup"><span data-stu-id="22b0b-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="22b0b-176">Azure-erőforráshasználati jelentés:</span><span class="sxs-lookup"><span data-stu-id="22b0b-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="22b0b-177">**Az Azure-erőforrások napi** használata a kiválasztott időszakban: Az egyes használatalapú előfizetések egyes forgalmi díjas erőforrásainak napi használati egységei az elmúlt 60 napra vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="22b0b-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="22b0b-178">**Az Azure-erőforrások becsült** használati költsége a kiválasztott időszakra vonatkozóan: Becsült költség az egyes használatalapú előfizetések használati díjának legutóbbi díjszabása alapján az elmúlt 60 napra vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="22b0b-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="22b0b-179">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="22b0b-179">Next steps</span></span>

- [<span data-ttu-id="22b0b-180">Partnerközpont Analytics for Power BI alkalmazás áttekintése</span><span class="sxs-lookup"><span data-stu-id="22b0b-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="22b0b-181">A Partnerközpont adatelemzési alkalmazás a Microsoft Power BI-hoz telepítése és előzetes verziója</span><span class="sxs-lookup"><span data-stu-id="22b0b-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
