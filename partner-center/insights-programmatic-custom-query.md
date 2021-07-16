---
title: Egyéni lekérdezési specifikáció
description: Megtudhatja, hogyan hozhat létre egyéni lekérdezéseket az adatok elemzési táblákból való kinyeréséhez.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376729"
---
# <a name="custom-query-specification"></a>Egyéni lekérdezési specifikáció

A partnerek ezzel a lekérdezési specifikációval egyszerűen hozhatnak létre egyéni lekérdezéseket az elemzési táblákból való adatlenyeréshez. A lekérdezésekkel csak azokat a kívánt oszlopokat és metrikákat választhatja ki, amelyek megfelelnek egy adott feltételnek. A nyelvi specifikációk egyik fontos része az adatkészlet definíciója, amelyre egyéni lekérdezés írható.

## <a name="datasets"></a>Adathalmazok

Ahogy egyes lekérdezések is futnak táblákat és oszlopokat tartalmazó adatbázisokon, az oszlopokból és metrikákból álló adatkészletek egyéni lekérdezései is működnek. A lekérdezések formában elérhető adatkészletek teljes listája a datasets API használatával szerezhető be.

Ez egy példa egy JSON-ként bemutatott adatkészletre:

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a>Az adatkészlet részei

- Az adatkészlet neve az adatbázistábla nevéhez hasonló. Például: OfficeUsage. Az adatkészletek a kiválasztható oszlopok listáját, például CustomerTenantId oszlopokat tartalmaznak.
- Az adatkészletek olyan metrikákat is tartalmaznak, mint az adatbázisok összesítő függvényei. Például: TotalMonthlyActiveUsers.
- Az adatok exportálhatók rögzített időtartamokkal.

## <a name="formulating-a-query-on-a-dataset"></a>Adatkészlet lekérdezésének létrehozása

Ez néhány példalekérdezésekre, amelyek a különböző adattípusok kinyerését mutatják be.

|Lekérdezés|    Leírás    |
|----|    ----    |
|**SELECT (KIJELÖLÉS)** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **TIMESPAN** LAST_MONTH|    Ez a lekérdezés lekérdezi az elmúlt 1 hónap összes CusotmerTenantID-ját és a hozzá tartozó PaidAvailableUnits értékeket.    |
|**SELECT (KIJELÖLÉS)** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10|    Ez a lekérdezés lekérdezi az első 10 ügyfélbérlőt a fizetős rendelkezésre álló egységek számának csökkenő sorrendjében.     |
|**SELECT (KIJELÖLÉS)** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS |    Ez a lekérdezés lekérdezi az összes olyan ügyfél PaidAvailableUnits és MonthlyActiveUsers értékét, akikNél a MonthlyActiveUser érték nagyobb, mint 100 000.     |
|**SELECT (KIJELÖLÉS)** CustomerTenantId, Month, MonthlyActiveUsers **FROM** <br>OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002') |    Ez a lekérdezés lekérdezi a CustomerTenantId és a havi aktív felhasználókat minden hónapra a két CustomerTpId értékkel: "2a31c234-1f4e-4c60-909e-1f4e-909e-76d234f93161 és '80780748-3f9a-11eb-b378-0242ac130002'.     |
|        |        |

## <a name="query-specification"></a>Lekérdezési specifikáció

Ez a szakasz a lekérdezésdefiníciót és -struktúrát ismerteti.

## <a name="grammar-reference"></a>Nyelvtani referencia

Ez a táblázat a lekérdezésekben használt szimbólumokat ismerteti.

|    Lekérdezés    |    Leírás    |
|    ----    |    ----    |
|    `?`    |    Választható    |
|    `*`    |    Nulla vagy több    |
|    `+`    |    Egy vagy több    |
|    `\|`    |    Vagy / Az egyik lista    |
|        |        |

## <a name="query-definition"></a>Lekérdezésdefiníció

A lekérdezési utasítás a következő záradékokkal rendelkezik: SelectClause, FromClause, WhereClause, OrderClause, LimitClause és TimeSpan.

- **Válassza aClause lehetőséget:**`SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName:** Az adatkészletben definiált oszlopok és metrikák
- **FromClause :**`FROM DatasetName`
    - **DatasetName:** Az Adatkészleten belül definiált adatkészlet neve
- **WhereClause:**`WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition:** ColumOrMetricName operátor értéke
        - **Operátor:**`=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Érték:** Szám | StringLiteral | MultiNumberList | MultiStringList
            - **Number (Szám):**`-? [0-9]+ (. [0-9] [0-9]*)?`
            - **StringLiteral**:  `' [a-zA-Z0-9_]*'`
            - **MultiNumberList:**`(Number (,Number)*)`
            - **MultiStringList:**`(StringLiteral (,StringLiteral)*)`
- **OrderClause:**`ORDER BY OrderCondition (,OrderCondition)`
    - **OrderCondition:**`ColumOrMetricName (ASC | DESC)*`
- **LimitClause:**`LIMIT [0-9]+`
- **TimeSpan ::**`TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Lekérdezési struktúra

A jelentéslekérdezés több részből áll:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Az egyes részeket az alábbiakban ismertetjük.

### `SELECT`

A lekérdezés ezen része határozza meg az exportált oszlopokat. A kiválasztható oszlopok az adatkészlet *selectableColumns* és *availableMetrics* szakaszaiban felsorolt mezők.

A kulcsszó `DISTINCT` a után is megadva `SELECT` lehet. Ha meg van adva, akkor a végleges exportált sorok mindig a kiválasztott oszlopok különböző `DISTINCT` értékeit tartalmazzák. A rendszer a kiválasztott oszlopok minden egyes kombinációjához kiszámítja a metrikákat, ezért nincs szükség kulcsszóra, ha egy metrikaoszlop szerepel `DISTINCT` a kiválasztott oszloplistában.

**Példa**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

A lekérdezés ezen része azt az adatkészletet jelöli, amelyből az adatokat exportálni kell. Az itt megadott adatkészlet nevének érvényes adatkészletnévnek kell lennie, amelyet az adatkészletek API ad vissza.

**Példa**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

A lekérdezés ezen része az adatkészlet szűrési feltételeinek megadására használható. A végső exportált fájlban csak az ebben a záradékban felsorolt feltételeknek megfelelő sorok lesznek jelen. A szűrési feltétel a *selectableColumns* és az *availableMetrics oszlop bármelyik oszlopán lehet.* A szűrési feltételben megadott értékek csak akkor lehet számok vagy sztringek listája, ha az operátor `IN` vagy `NOT IN` . Az értékek mindig adhatók literális sztringként, és a rendszer natív típusú oszlopokká konvertálja őket. Több szűrési feltételt ÉS művelettel kell elválasztani.

**Példa**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

A lekérdezés ezen része határozza meg az exportált sorok rendelési kritériumait. A rendelést definiáló oszlopoknak a *selectableColumns* oszlopból és az *elérhetőMetriákból* kell állva lennie. Ha nincs megadva a rend iránya, az alapértelmezett érték a DESC lesz az oszlopban. A sorrend több oszlopra is definiálható úgy, hogy a feltételeket vesszővel választja el.

**Példa**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

A lekérdezés ezen része határozza meg az exportálni kívánt sorok számát. A megadott számnak pozitív, nem nulla egész számnak kell lennie.

### `TIMESPAN`

A lekérdezés ezen része határozza meg az adatok exportálásának időtartamát. A lehetséges értékeknek az *adatkészlet definíciójában található availableDateRanges* mezőben kell lennie.

### <a name="case-sensitivity-in-query-specification"></a>Kis- és nagybetűk bizalmasság a lekérdezés specifikációiban

A specifikáció teljesen nem érzékeny a kis- és a kis- és a kis- és a nagy- és a kis- és a nagy- és a kis- és nagy között. Az előre definiált kulcsszavak, oszlopnevek és értékek kis- és nagybetűkkel határozhatóak meg.

## <a name="next-steps"></a>Következő lépések

- [Rendszerlekérdezések listája](insights-programmatic-system-queries.md)
- [Mintalekérdezések listája](insights-programmatic-sample-queries.md)