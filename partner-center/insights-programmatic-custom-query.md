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
# <a name="custom-query-specification"></a><span data-ttu-id="b9f44-103">Egyéni lekérdezési specifikáció</span><span class="sxs-lookup"><span data-stu-id="b9f44-103">Custom query specification</span></span>

<span data-ttu-id="b9f44-104">A partnerek ezzel a lekérdezési specifikációval egyszerűen hozhatnak létre egyéni lekérdezéseket az elemzési táblákból való adatlenyeréshez.</span><span class="sxs-lookup"><span data-stu-id="b9f44-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="b9f44-105">A lekérdezésekkel csak azokat a kívánt oszlopokat és metrikákat választhatja ki, amelyek megfelelnek egy adott feltételnek.</span><span class="sxs-lookup"><span data-stu-id="b9f44-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="b9f44-106">A nyelvi specifikációk egyik fontos része az adatkészlet definíciója, amelyre egyéni lekérdezés írható.</span><span class="sxs-lookup"><span data-stu-id="b9f44-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="b9f44-107">Adathalmazok</span><span class="sxs-lookup"><span data-stu-id="b9f44-107">Datasets</span></span>

<span data-ttu-id="b9f44-108">Ahogy egyes lekérdezések is futnak táblákat és oszlopokat tartalmazó adatbázisokon, az oszlopokból és metrikákból álló adatkészletek egyéni lekérdezései is működnek.</span><span class="sxs-lookup"><span data-stu-id="b9f44-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="b9f44-109">A lekérdezések formában elérhető adatkészletek teljes listája a datasets API használatával szerezhető be.</span><span class="sxs-lookup"><span data-stu-id="b9f44-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="b9f44-110">Ez egy példa egy JSON-ként bemutatott adatkészletre:</span><span class="sxs-lookup"><span data-stu-id="b9f44-110">This is an example of a dataset shown as a JSON:</span></span>

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

## <a name="parts-of-a-dataset"></a><span data-ttu-id="b9f44-111">Az adatkészlet részei</span><span class="sxs-lookup"><span data-stu-id="b9f44-111">Parts of a dataset</span></span>

- <span data-ttu-id="b9f44-112">Az adatkészlet neve az adatbázistábla nevéhez hasonló.</span><span class="sxs-lookup"><span data-stu-id="b9f44-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="b9f44-113">Például: OfficeUsage.</span><span class="sxs-lookup"><span data-stu-id="b9f44-113">For example, OfficeUsage.</span></span> <span data-ttu-id="b9f44-114">Az adatkészletek a kiválasztható oszlopok listáját, például CustomerTenantId oszlopokat tartalmaznak.</span><span class="sxs-lookup"><span data-stu-id="b9f44-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="b9f44-115">Az adatkészletek olyan metrikákat is tartalmaznak, mint az adatbázisok összesítő függvényei.</span><span class="sxs-lookup"><span data-stu-id="b9f44-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="b9f44-116">Például: TotalMonthlyActiveUsers.</span><span class="sxs-lookup"><span data-stu-id="b9f44-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="b9f44-117">Az adatok exportálhatók rögzített időtartamokkal.</span><span class="sxs-lookup"><span data-stu-id="b9f44-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="b9f44-118">Adatkészlet lekérdezésének létrehozása</span><span class="sxs-lookup"><span data-stu-id="b9f44-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="b9f44-119">Ez néhány példalekérdezésekre, amelyek a különböző adattípusok kinyerését mutatják be.</span><span class="sxs-lookup"><span data-stu-id="b9f44-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="b9f44-120">Lekérdezés</span><span class="sxs-lookup"><span data-stu-id="b9f44-120">Query</span></span>|    <span data-ttu-id="b9f44-121">Leírás</span><span class="sxs-lookup"><span data-stu-id="b9f44-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="b9f44-122">**SELECT (KIJELÖLÉS)** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="b9f44-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="b9f44-123">OfficeUsage **TIMESPAN** LAST_MONTH</span><span class="sxs-lookup"><span data-stu-id="b9f44-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="b9f44-124">Ez a lekérdezés lekérdezi az elmúlt 1 hónap összes CusotmerTenantID-ját és a hozzá tartozó PaidAvailableUnits értékeket.</span><span class="sxs-lookup"><span data-stu-id="b9f44-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="b9f44-125">**SELECT (KIJELÖLÉS)** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="b9f44-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="b9f44-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span><span class="sxs-lookup"><span data-stu-id="b9f44-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="b9f44-127">Ez a lekérdezés lekérdezi az első 10 ügyfélbérlőt a fizetős rendelkezésre álló egységek számának csökkenő sorrendjében.</span><span class="sxs-lookup"><span data-stu-id="b9f44-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="b9f44-128">**SELECT (KIJELÖLÉS)** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span><span class="sxs-lookup"><span data-stu-id="b9f44-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="b9f44-129">Ez a lekérdezés lekérdezi az összes olyan ügyfél PaidAvailableUnits és MonthlyActiveUsers értékét, akikNél a MonthlyActiveUser érték nagyobb, mint 100 000.</span><span class="sxs-lookup"><span data-stu-id="b9f44-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="b9f44-130">**SELECT (KIJELÖLÉS)** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span><span class="sxs-lookup"><span data-stu-id="b9f44-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="b9f44-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span><span class="sxs-lookup"><span data-stu-id="b9f44-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="b9f44-132">Ez a lekérdezés lekérdezi a CustomerTenantId és a havi aktív felhasználókat minden hónapra a két CustomerTpId értékkel: "2a31c234-1f4e-4c60-909e-1f4e-909e-76d234f93161 és '80780748-3f9a-11eb-b378-0242ac130002'.</span><span class="sxs-lookup"><span data-stu-id="b9f44-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="b9f44-133">Lekérdezési specifikáció</span><span class="sxs-lookup"><span data-stu-id="b9f44-133">Query specification</span></span>

<span data-ttu-id="b9f44-134">Ez a szakasz a lekérdezésdefiníciót és -struktúrát ismerteti.</span><span class="sxs-lookup"><span data-stu-id="b9f44-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="b9f44-135">Nyelvtani referencia</span><span class="sxs-lookup"><span data-stu-id="b9f44-135">Grammar reference</span></span>

<span data-ttu-id="b9f44-136">Ez a táblázat a lekérdezésekben használt szimbólumokat ismerteti.</span><span class="sxs-lookup"><span data-stu-id="b9f44-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="b9f44-137">Lekérdezés</span><span class="sxs-lookup"><span data-stu-id="b9f44-137">Query</span></span>    |    <span data-ttu-id="b9f44-138">Leírás</span><span class="sxs-lookup"><span data-stu-id="b9f44-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="b9f44-139">Választható</span><span class="sxs-lookup"><span data-stu-id="b9f44-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="b9f44-140">Nulla vagy több</span><span class="sxs-lookup"><span data-stu-id="b9f44-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="b9f44-141">Egy vagy több</span><span class="sxs-lookup"><span data-stu-id="b9f44-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="b9f44-142">Vagy / Az egyik lista</span><span class="sxs-lookup"><span data-stu-id="b9f44-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="b9f44-143">Lekérdezésdefiníció</span><span class="sxs-lookup"><span data-stu-id="b9f44-143">Query definition</span></span>

<span data-ttu-id="b9f44-144">A lekérdezési utasítás a következő záradékokkal rendelkezik: SelectClause, FromClause, WhereClause, OrderClause, LimitClause és TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="b9f44-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="b9f44-145">**Válassza aClause lehetőséget:**`SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="b9f44-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="b9f44-146">**ColumOrMetricName:** Az adatkészletben definiált oszlopok és metrikák</span><span class="sxs-lookup"><span data-stu-id="b9f44-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="b9f44-147">**FromClause :**`FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="b9f44-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="b9f44-148">**DatasetName:** Az Adatkészleten belül definiált adatkészlet neve</span><span class="sxs-lookup"><span data-stu-id="b9f44-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="b9f44-149">**WhereClause:**`WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="b9f44-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="b9f44-150">**FilterCondition:** ColumOrMetricName operátor értéke</span><span class="sxs-lookup"><span data-stu-id="b9f44-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="b9f44-151">**Operátor:**`=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="b9f44-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="b9f44-152">**Érték:** Szám | StringLiteral | MultiNumberList | MultiStringList</span><span class="sxs-lookup"><span data-stu-id="b9f44-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="b9f44-153">**Number (Szám):**`-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="b9f44-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="b9f44-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="b9f44-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="b9f44-155">**MultiNumberList:**`(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="b9f44-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="b9f44-156">**MultiStringList:**`(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="b9f44-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="b9f44-157">**OrderClause:**`ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="b9f44-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="b9f44-158">**OrderCondition:**`ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="b9f44-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="b9f44-159">**LimitClause:**`LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="b9f44-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="b9f44-160">**TimeSpan ::**`TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="b9f44-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="b9f44-161">Lekérdezési struktúra</span><span class="sxs-lookup"><span data-stu-id="b9f44-161">Query Structure</span></span>

<span data-ttu-id="b9f44-162">A jelentéslekérdezés több részből áll:</span><span class="sxs-lookup"><span data-stu-id="b9f44-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="b9f44-163">Az egyes részeket az alábbiakban ismertetjük.</span><span class="sxs-lookup"><span data-stu-id="b9f44-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="b9f44-164">A lekérdezés ezen része határozza meg az exportált oszlopokat.</span><span class="sxs-lookup"><span data-stu-id="b9f44-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="b9f44-165">A kiválasztható oszlopok az adatkészlet *selectableColumns* és *availableMetrics* szakaszaiban felsorolt mezők.</span><span class="sxs-lookup"><span data-stu-id="b9f44-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="b9f44-166">A kulcsszó `DISTINCT` a után is megadva `SELECT` lehet.</span><span class="sxs-lookup"><span data-stu-id="b9f44-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="b9f44-167">Ha meg van adva, akkor a végleges exportált sorok mindig a kiválasztott oszlopok különböző `DISTINCT` értékeit tartalmazzák.</span><span class="sxs-lookup"><span data-stu-id="b9f44-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="b9f44-168">A rendszer a kiválasztott oszlopok minden egyes kombinációjához kiszámítja a metrikákat, ezért nincs szükség kulcsszóra, ha egy metrikaoszlop szerepel `DISTINCT` a kiválasztott oszloplistában.</span><span class="sxs-lookup"><span data-stu-id="b9f44-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="b9f44-169">**Példa**</span><span class="sxs-lookup"><span data-stu-id="b9f44-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="b9f44-170">A lekérdezés ezen része azt az adatkészletet jelöli, amelyből az adatokat exportálni kell.</span><span class="sxs-lookup"><span data-stu-id="b9f44-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="b9f44-171">Az itt megadott adatkészlet nevének érvényes adatkészletnévnek kell lennie, amelyet az adatkészletek API ad vissza.</span><span class="sxs-lookup"><span data-stu-id="b9f44-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="b9f44-172">**Példa**</span><span class="sxs-lookup"><span data-stu-id="b9f44-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="b9f44-173">A lekérdezés ezen része az adatkészlet szűrési feltételeinek megadására használható.</span><span class="sxs-lookup"><span data-stu-id="b9f44-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="b9f44-174">A végső exportált fájlban csak az ebben a záradékban felsorolt feltételeknek megfelelő sorok lesznek jelen.</span><span class="sxs-lookup"><span data-stu-id="b9f44-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="b9f44-175">A szűrési feltétel a *selectableColumns* és az *availableMetrics oszlop bármelyik oszlopán lehet.*</span><span class="sxs-lookup"><span data-stu-id="b9f44-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="b9f44-176">A szűrési feltételben megadott értékek csak akkor lehet számok vagy sztringek listája, ha az operátor `IN` vagy `NOT IN` .</span><span class="sxs-lookup"><span data-stu-id="b9f44-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="b9f44-177">Az értékek mindig adhatók literális sztringként, és a rendszer natív típusú oszlopokká konvertálja őket.</span><span class="sxs-lookup"><span data-stu-id="b9f44-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="b9f44-178">Több szűrési feltételt ÉS művelettel kell elválasztani.</span><span class="sxs-lookup"><span data-stu-id="b9f44-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="b9f44-179">**Példa**</span><span class="sxs-lookup"><span data-stu-id="b9f44-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="b9f44-180">A lekérdezés ezen része határozza meg az exportált sorok rendelési kritériumait.</span><span class="sxs-lookup"><span data-stu-id="b9f44-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="b9f44-181">A rendelést definiáló oszlopoknak a *selectableColumns* oszlopból és az *elérhetőMetriákból* kell állva lennie.</span><span class="sxs-lookup"><span data-stu-id="b9f44-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="b9f44-182">Ha nincs megadva a rend iránya, az alapértelmezett érték a DESC lesz az oszlopban.</span><span class="sxs-lookup"><span data-stu-id="b9f44-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="b9f44-183">A sorrend több oszlopra is definiálható úgy, hogy a feltételeket vesszővel választja el.</span><span class="sxs-lookup"><span data-stu-id="b9f44-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="b9f44-184">**Példa**</span><span class="sxs-lookup"><span data-stu-id="b9f44-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="b9f44-185">A lekérdezés ezen része határozza meg az exportálni kívánt sorok számát.</span><span class="sxs-lookup"><span data-stu-id="b9f44-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="b9f44-186">A megadott számnak pozitív, nem nulla egész számnak kell lennie.</span><span class="sxs-lookup"><span data-stu-id="b9f44-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="b9f44-187">A lekérdezés ezen része határozza meg az adatok exportálásának időtartamát.</span><span class="sxs-lookup"><span data-stu-id="b9f44-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="b9f44-188">A lehetséges értékeknek az *adatkészlet definíciójában található availableDateRanges* mezőben kell lennie.</span><span class="sxs-lookup"><span data-stu-id="b9f44-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="b9f44-189">Kis- és nagybetűk bizalmasság a lekérdezés specifikációiban</span><span class="sxs-lookup"><span data-stu-id="b9f44-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="b9f44-190">A specifikáció teljesen nem érzékeny a kis- és a kis- és a kis- és a nagy- és a kis- és a nagy- és a kis- és nagy között.</span><span class="sxs-lookup"><span data-stu-id="b9f44-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="b9f44-191">Az előre definiált kulcsszavak, oszlopnevek és értékek kis- és nagybetűkkel határozhatóak meg.</span><span class="sxs-lookup"><span data-stu-id="b9f44-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b9f44-192">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="b9f44-192">Next steps</span></span>

- [<span data-ttu-id="b9f44-193">Rendszerlekérdezések listája</span><span class="sxs-lookup"><span data-stu-id="b9f44-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="b9f44-194">Mintalekérdezések listája</span><span class="sxs-lookup"><span data-stu-id="b9f44-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)