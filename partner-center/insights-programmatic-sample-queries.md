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
# <a name="sample-queries-for-partner-center-insights-report"></a>Mintalekérdezések Partnerközpont elemzések jelentéséhez

Ez a cikk minta lekérdezéseket biztosít a Partner Elemzések jelentésekhez. Ezeket a lekérdezéseket a Jelentéslekérdezés létrehozása API-végpont hívása segítségével használhatja. Ha szükséges, a Create Report Query API (Jelentéslekérdezés [létrehozása) API-hívás](insights-programmatic-access-paradigm.md#create-report-query-api) módosításával további oszlopokat adhat hozzá, módosíthatja a számítási időszakot, és szűrési feltételeket adhat hozzá.

Az oszlopnevekkel, attribútumokkal és leírásokkal kapcsolatos részletekért tekintse meg az [adatdefiníciókat ismertetőt.](insights-data-definitions.md)

## <a name="customer-details"></a>Ügyféladatok

Ezek a mintalekérdezések az ügyfelek adatait tartalmazó jelentésre vonatkoznak:

### <a name="by-geography"></a>Földrajzi hely szerint

Egy adott földrajzi régióból származó ügyfelek listája az elmúlt hónapban.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>Termékváltozat és számlás bevétel szerint

Adott termékváltozatot és számlázható bevételt használó ügyfelek listája több mint 20 000 az elmúlt 6 hónapban

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>Rendelkezésre álló helyek szerint

Az elmúlt hónap első 10 ügyfele a rendelkezésre álló helyek alapján

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>Partnerprofil

Ezek a mintalekérdezések a partnerprofil-jelentésre vonatkoznak:

### <a name="by-geography"></a>Földrajzi hely szerint

Adott földrajzi listában található partnerek listája.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>MPN-partner szerint

Egy PGA MPN-partner alá sorolt partnerek listája

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Viszonteladói teljesítmény

Ezek a mintalekérdezések a viszonteladói teljesítményjelentésre vonatkoznak:

### <a name="by-geography"></a>Földrajzi hely szerint

Adott földrajzi hely viszonteladóinak listája az elmúlt hónapban.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Viszonteladó szerint

Ügyfélszám, előfizetések száma, összes elérhető hely, összes hozzárendelt hely, adott viszonteladóhoz rendelt teljes bevétel.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>Első 10 bevétel szerint

A 10 legnagyobb viszonteladó az elmúlt hónap teljes bevétele alapján.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Előfizetés részletei

Ezek a mintalekérdezések az előfizetés részleteit tartalmazó jelentésre vonatkoznak:

### <a name="by-renewal-eligibility"></a>Megújítási jogosultság alapján

Azon előfizetések listája, amelyek az elmúlt hónapban nem jogosultak az automatikus megújításra.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Előfizetés állapota szerint

Azon előfizetések listája, amelyek az elmúlt hónapban Letiltva állapotban vannak.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Darabszámok hat hónapig

Előfizetések száma, összes eladott hely, egy adott partner ügyfélszáma az elmúlt hat hónapban.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Azure-használat

Ezek a mintalekérdezések az Azure használati jelentésre vonatkoznak:

### <a name="by-meter-category"></a>Fogyasztásmérő kategóriája szerint

Az Azure használati előfizetések listája a használati egységekkel és az ACR-rel adott fogyasztásmérő-kategóriához az elmúlt hat hónapban.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Összes ACR szerint

Azon Azure-beli használati előfizetések listája, amelyekben az ACR teljes száma meghaladja a 20 000-et az elmúlt hat hónapban

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Következő lépések

- [API-k a partnerelemzési adatok eléréséhez](insights-programmatic-analytics-available-api.md)