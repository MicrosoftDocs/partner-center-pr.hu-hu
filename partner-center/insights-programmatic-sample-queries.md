---
title: Mintalekérdezések listája
description: A mintalekérdezésekkel programozott módon férhet hozzá a partnerelemzési adatokhoz.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376659"
---
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="f0d1d-103">Mintalekérdezések Partnerközpont elemzések jelentéséhez</span><span class="sxs-lookup"><span data-stu-id="f0d1d-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="f0d1d-104">Ez a cikk minta lekérdezéseket biztosít a Partner Elemzések jelentésekhez.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="f0d1d-105">Ezeket a lekérdezéseket a Jelentéslekérdezés létrehozása API-végpont hívása segítségével használhatja.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="f0d1d-106">Ha szükséges, a Create Report Query API (Jelentéslekérdezés [létrehozása) API-hívás](insights-programmatic-access-paradigm.md#create-report-query-api) módosításával további oszlopokat adhat hozzá, módosíthatja a számítási időszakot, és szűrési feltételeket adhat hozzá.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="f0d1d-107">Az oszlopnevekkel, attribútumokkal és leírásokkal kapcsolatos részletekért tekintse meg az [adatdefiníciókat ismertetőt.](insights-data-definitions.md)</span><span class="sxs-lookup"><span data-stu-id="f0d1d-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="f0d1d-108">Ügyféladatok</span><span class="sxs-lookup"><span data-stu-id="f0d1d-108">Customer details</span></span>

<span data-ttu-id="f0d1d-109">Ezek a mintalekérdezések az ügyfelek adatait tartalmazó jelentésre vonatkoznak:</span><span class="sxs-lookup"><span data-stu-id="f0d1d-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="f0d1d-110">Földrajzi hely szerint</span><span class="sxs-lookup"><span data-stu-id="f0d1d-110">By geography</span></span>

<span data-ttu-id="f0d1d-111">Egy adott földrajzi régióból származó ügyfelek listája az elmúlt hónapban.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="f0d1d-112">Termékváltozat és számlás bevétel szerint</span><span class="sxs-lookup"><span data-stu-id="f0d1d-112">By SKU and billed revenue</span></span>

<span data-ttu-id="f0d1d-113">Adott termékváltozatot és számlázható bevételt használó ügyfelek listája több mint 20 000 az elmúlt 6 hónapban</span><span class="sxs-lookup"><span data-stu-id="f0d1d-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="f0d1d-114">Rendelkezésre álló helyek szerint</span><span class="sxs-lookup"><span data-stu-id="f0d1d-114">By available seats</span></span>

<span data-ttu-id="f0d1d-115">Az elmúlt hónap első 10 ügyfele a rendelkezésre álló helyek alapján</span><span class="sxs-lookup"><span data-stu-id="f0d1d-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="f0d1d-116">Partnerprofil</span><span class="sxs-lookup"><span data-stu-id="f0d1d-116">Partner Profile</span></span>

<span data-ttu-id="f0d1d-117">Ezek a mintalekérdezések a partnerprofil-jelentésre vonatkoznak:</span><span class="sxs-lookup"><span data-stu-id="f0d1d-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="f0d1d-118">Földrajzi hely szerint</span><span class="sxs-lookup"><span data-stu-id="f0d1d-118">By geography</span></span>

<span data-ttu-id="f0d1d-119">Adott földrajzi listában található partnerek listája.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="f0d1d-120">MPN-partner szerint</span><span class="sxs-lookup"><span data-stu-id="f0d1d-120">By MPN partner</span></span>

<span data-ttu-id="f0d1d-121">Egy PGA MPN-partner alá sorolt partnerek listája</span><span class="sxs-lookup"><span data-stu-id="f0d1d-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="f0d1d-122">Viszonteladói teljesítmény</span><span class="sxs-lookup"><span data-stu-id="f0d1d-122">Reseller Performance</span></span>

<span data-ttu-id="f0d1d-123">Ezek a mintalekérdezések a viszonteladói teljesítményjelentésre vonatkoznak:</span><span class="sxs-lookup"><span data-stu-id="f0d1d-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="f0d1d-124">Földrajzi hely szerint</span><span class="sxs-lookup"><span data-stu-id="f0d1d-124">By geography</span></span>

<span data-ttu-id="f0d1d-125">Adott földrajzi hely viszonteladóinak listája az elmúlt hónapban.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="f0d1d-126">Viszonteladó szerint</span><span class="sxs-lookup"><span data-stu-id="f0d1d-126">By reseller</span></span>

<span data-ttu-id="f0d1d-127">Ügyfélszám, előfizetések száma, összes elérhető hely, összes hozzárendelt hely, adott viszonteladóhoz rendelt teljes bevétel.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="f0d1d-128">Első 10 bevétel szerint</span><span class="sxs-lookup"><span data-stu-id="f0d1d-128">Top 10 by revenue</span></span>

<span data-ttu-id="f0d1d-129">A 10 legnagyobb viszonteladó az elmúlt hónap teljes bevétele alapján.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="f0d1d-130">Előfizetés részletei</span><span class="sxs-lookup"><span data-stu-id="f0d1d-130">Subscription Details</span></span>

<span data-ttu-id="f0d1d-131">Ezek a mintalekérdezések az előfizetés részleteit tartalmazó jelentésre vonatkoznak:</span><span class="sxs-lookup"><span data-stu-id="f0d1d-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="f0d1d-132">Megújítási jogosultság alapján</span><span class="sxs-lookup"><span data-stu-id="f0d1d-132">By renewal eligibility</span></span>

<span data-ttu-id="f0d1d-133">Azon előfizetések listája, amelyek az elmúlt hónapban nem jogosultak az automatikus megújításra.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="f0d1d-134">Előfizetés állapota szerint</span><span class="sxs-lookup"><span data-stu-id="f0d1d-134">By subscription state</span></span>

<span data-ttu-id="f0d1d-135">Azon előfizetések listája, amelyek az elmúlt hónapban Letiltva állapotban vannak.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="f0d1d-136">Darabszámok hat hónapig</span><span class="sxs-lookup"><span data-stu-id="f0d1d-136">Counts for six months</span></span>

<span data-ttu-id="f0d1d-137">Előfizetések száma, összes eladott hely, egy adott partner ügyfélszáma az elmúlt hat hónapban.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="f0d1d-138">Azure-használat</span><span class="sxs-lookup"><span data-stu-id="f0d1d-138">Azure Usage</span></span>

<span data-ttu-id="f0d1d-139">Ezek a mintalekérdezések az Azure használati jelentésre vonatkoznak:</span><span class="sxs-lookup"><span data-stu-id="f0d1d-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="f0d1d-140">Fogyasztásmérő kategóriája szerint</span><span class="sxs-lookup"><span data-stu-id="f0d1d-140">By meter category</span></span>

<span data-ttu-id="f0d1d-141">Az Azure használati előfizetések listája a használati egységekkel és az ACR-rel adott fogyasztásmérő-kategóriához az elmúlt hat hónapban.</span><span class="sxs-lookup"><span data-stu-id="f0d1d-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="f0d1d-142">Összes ACR szerint</span><span class="sxs-lookup"><span data-stu-id="f0d1d-142">By total ACR</span></span>

<span data-ttu-id="f0d1d-143">Azon Azure-beli használati előfizetések listája, amelyekben az ACR teljes száma meghaladja a 20 000-et az elmúlt hat hónapban</span><span class="sxs-lookup"><span data-stu-id="f0d1d-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="f0d1d-144">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="f0d1d-144">Next steps</span></span>

- [<span data-ttu-id="f0d1d-145">API-k a partnerelemzési adatok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="f0d1d-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)