---
title: Szoftveres hozzáférési paradigma Elemzések adatokhoz
description: A programozott elemzésekhez használható API-hívási minta magas szintű folyamatának a használata. A partnerelemzési jelentések elérésére vonatkozó API-kat is lefedi.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376677"
---
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="a2d5f-104">Programozott hozzáférési paradigma</span><span class="sxs-lookup"><span data-stu-id="a2d5f-104">Programmatic access paradigm</span></span>

<span data-ttu-id="a2d5f-105">Ez a diagram az új jelentéssablon létrehozásához, az egyéni jelentés ütemezéséhez és a hibaadatok lekéréséhez használt API-hívásmintát mutatja be.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Magas szintű folyamat":::
<span data-ttu-id="a2d5f-107">***1. ábra: Az API-hívási minta magas szintű áramlása***</span><span class="sxs-lookup"><span data-stu-id="a2d5f-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="a2d5f-108">Ez a lista az 1. ábra további részleteit tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="a2d5f-109">Az ügyfélalkalmazás a Jelentéslekérdezés létrehozása API hívásával definiálhatja az egyéni [jelentéssémát/sablont.](#create-report-query-api)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="a2d5f-110">Azt is választhatja, hogy kiválaszt egy jelentéssablont (QueryId) az itt felsorolt jelentéssablontár-minták [közül.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="a2d5f-111">Sikeres létrehozás esetén a Jelentéslekérdezés létrehozása API a QueryId értéket adja vissza.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="a2d5f-112">Az ügyfélalkalmazásnak ezután meg kell hívnia a Jelentés létrehozása [API-t](#create-report-api) a QueryId használatával, valamint a jelentés kezdő dátumát, az ismétlési időközt, az ismétlődést és egy opcionális visszahívási URI-t.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="a2d5f-113">A Sikeres jelentés [létrehozása API a ReportId](#create-report-api) (Jelentésazonosító) értéket adja vissza.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="a2d5f-114">Amint a jelentés adatai letölthetők, az ügyfélalkalmazás értesítést kap a visszahívási URL-címen.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="a2d5f-115">Az ügyfélalkalmazás ezután a [Get Report Executions API](#get-report-execution-api) használatával lekérdezi a jelentés állapotát a jelentés azonosítójával és dátumtartományával.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="a2d5f-116">Sikeresség után a rendszer visszaadja a jelentés letöltési hivatkozását, és az alkalmazás kezdeményezheti az adatok letöltését.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="a2d5f-117">Jelentéslekérdezés nyelvének specifikációja</span><span class="sxs-lookup"><span data-stu-id="a2d5f-117">Report query language specification</span></span>

<span data-ttu-id="a2d5f-118">Bár a [](insights-programmatic-system-queries.md) rendszerlekérdezések segítségével jelentéseket hozhat létre, saját lekérdezéseket is létrehozhat az üzleti igényeinek megfelelően.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="a2d5f-119">Az egyéni lekérdezésekkel kapcsolatos további információkért lásd: [Egyéni lekérdezés specifikációja.](insights-programmatic-custom-query.md)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="a2d5f-120">Jelentéslekérdezés API létrehozása</span><span class="sxs-lookup"><span data-stu-id="a2d5f-120">Create report query API</span></span>

<span data-ttu-id="a2d5f-121">Az API segítségével egyéni lekérdezéseket hozhat létre, amelyek meghatározzák azt az adatkészletet, amelyből az oszlopokat és metrikákat exportálni kell.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="a2d5f-122">Az API biztosítja azt a rugalmasságot, hogy új jelentéskészítési sablont hozzon létre az üzleti igényeinek megfelelően.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="a2d5f-123">A rendszerlekérdezések is [használhatók.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="a2d5f-124">Ha nincs szükség egyéni jelentéssablonokra, közvetlenül a megadott rendszerlekérdezések QueryId-jaival hívhatja meg a Jelentési [API](#create-report-api) létrehozása api-t.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="a2d5f-125">Az alábbi példa bemutatja, hogyan hozhat létre egyéni lekérdezést, amely az elmúlt hónap első 10 ügyfelet tartalmazza bevétel szerint.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="a2d5f-126">Kérés szintaxisa</span><span class="sxs-lookup"><span data-stu-id="a2d5f-126">Request syntax</span></span>

|    <span data-ttu-id="a2d5f-127">Metódus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-127">Method</span></span>     |    <span data-ttu-id="a2d5f-128">Kérés URI-ja</span><span class="sxs-lookup"><span data-stu-id="a2d5f-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="a2d5f-129">POST</span><span class="sxs-lookup"><span data-stu-id="a2d5f-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="a2d5f-130">Kérelem fejléce</span><span class="sxs-lookup"><span data-stu-id="a2d5f-130">Request header</span></span>

|    <span data-ttu-id="a2d5f-131">Fejléc</span><span class="sxs-lookup"><span data-stu-id="a2d5f-131">Header</span></span>     |    <span data-ttu-id="a2d5f-132">Típus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-132">Type</span></span>     |    <span data-ttu-id="a2d5f-133">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="a2d5f-134">Engedélyezés</span><span class="sxs-lookup"><span data-stu-id="a2d5f-134">Authorization</span></span>     |    <span data-ttu-id="a2d5f-135">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-135">string</span></span> |<span data-ttu-id="a2d5f-136">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-136">Required.</span></span> <span data-ttu-id="a2d5f-137">Az Azure Active Directory (Azure AD) hozzáférési jogkivonata.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="a2d5f-138">A formátum  `Bearer <token>` a következő: .</span><span class="sxs-lookup"><span data-stu-id="a2d5f-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="a2d5f-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2d5f-139">Content-Type</span></span>     |<span data-ttu-id="a2d5f-140">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="a2d5f-141">Elérésiút-paraméter</span><span class="sxs-lookup"><span data-stu-id="a2d5f-141">Path parameter</span></span>

<span data-ttu-id="a2d5f-142">None</span><span class="sxs-lookup"><span data-stu-id="a2d5f-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="a2d5f-143">Lekérdezési paraméter</span><span class="sxs-lookup"><span data-stu-id="a2d5f-143">Query parameter</span></span>

<span data-ttu-id="a2d5f-144">None</span><span class="sxs-lookup"><span data-stu-id="a2d5f-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="a2d5f-145">Minta kérelem hasznosadata</span><span class="sxs-lookup"><span data-stu-id="a2d5f-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="a2d5f-146">Szószedet</span><span class="sxs-lookup"><span data-stu-id="a2d5f-146">Glossary</span></span>

<span data-ttu-id="a2d5f-147">Ez a táblázat a kérelem hasznos elemeinek kulcsdefinícióit tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="a2d5f-148">Paraméter</span><span class="sxs-lookup"><span data-stu-id="a2d5f-148">Parameter</span></span>|    <span data-ttu-id="a2d5f-149">Kötelező</span><span class="sxs-lookup"><span data-stu-id="a2d5f-149">Required</span></span>     |    <span data-ttu-id="a2d5f-150">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-150">Description</span></span>     |    <span data-ttu-id="a2d5f-151">Megengedett értékek</span><span class="sxs-lookup"><span data-stu-id="a2d5f-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="a2d5f-152">Name</span><span class="sxs-lookup"><span data-stu-id="a2d5f-152">Name</span></span> |    <span data-ttu-id="a2d5f-153">Igen</span><span class="sxs-lookup"><span data-stu-id="a2d5f-153">Yes</span></span>     |    <span data-ttu-id="a2d5f-154">A lekérdezés rövid neve</span><span class="sxs-lookup"><span data-stu-id="a2d5f-154">Friendly name of the query</span></span>     |    <span data-ttu-id="a2d5f-155">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-155">string</span></span>     |
|    <span data-ttu-id="a2d5f-156">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-156">Description</span></span>     |    <span data-ttu-id="a2d5f-157">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-157">No</span></span>     |    <span data-ttu-id="a2d5f-158">A lekérdezés által visszaadott adatok leírása</span><span class="sxs-lookup"><span data-stu-id="a2d5f-158">Description of what the query returns</span></span>     |    <span data-ttu-id="a2d5f-159">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-159">string</span></span>     |
|    <span data-ttu-id="a2d5f-160">Lekérdezés</span><span class="sxs-lookup"><span data-stu-id="a2d5f-160">Query</span></span>     |    <span data-ttu-id="a2d5f-161">Igen</span><span class="sxs-lookup"><span data-stu-id="a2d5f-161">Yes</span></span>     |    <span data-ttu-id="a2d5f-162">Jelentés lekérdezési sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-162">Report query string</span></span>     |    <span data-ttu-id="a2d5f-163">Adattípus: sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-163">Data type: string</span></span> <br> <span data-ttu-id="a2d5f-164">[Egyéni lekérdezés](insights-programmatic-custom-query.md) üzleti szükség alapján</span><span class="sxs-lookup"><span data-stu-id="a2d5f-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="a2d5f-165">Egyéni lekérdezési mintákért tekintse meg a [példákat a mintalekérdezésekre.](insights-programmatic-sample-queries.md)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="a2d5f-166">Mintaválasz</span><span class="sxs-lookup"><span data-stu-id="a2d5f-166">Sample response</span></span>

<span data-ttu-id="a2d5f-167">A válasz hasznos adata a következőképpen strukturálva van:</span><span class="sxs-lookup"><span data-stu-id="a2d5f-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="a2d5f-168">Válaszkódok: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="a2d5f-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="a2d5f-169">Példa válasz hasznos hasznosra:</span><span class="sxs-lookup"><span data-stu-id="a2d5f-169">Response payload example:</span></span>

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a><span data-ttu-id="a2d5f-170">Szószedet</span><span class="sxs-lookup"><span data-stu-id="a2d5f-170">Glossary</span></span>

<span data-ttu-id="a2d5f-171">Ez a táblázat a kérelem hasznos elemeinek kulcsdefinícióit tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="a2d5f-172">Paraméter</span><span class="sxs-lookup"><span data-stu-id="a2d5f-172">Parameter</span></span>     |    <span data-ttu-id="a2d5f-173">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="a2d5f-174">QueryId (Lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-174">QueryId</span></span>     |    <span data-ttu-id="a2d5f-175">A létrehozott lekérdezés univerzálisan egyedi azonosítója (UUID)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="a2d5f-176">Name</span><span class="sxs-lookup"><span data-stu-id="a2d5f-176">Name</span></span>     |    <span data-ttu-id="a2d5f-177">A lekérdezésnek a kérelem hasznos adatában megadott rövid neve</span><span class="sxs-lookup"><span data-stu-id="a2d5f-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="a2d5f-178">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-178">Description</span></span>     |    <span data-ttu-id="a2d5f-179">A lekérdezés létrehozása során megadott leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="a2d5f-180">Lekérdezés</span><span class="sxs-lookup"><span data-stu-id="a2d5f-180">Query</span></span>     |    <span data-ttu-id="a2d5f-181">A lekérdezés létrehozása során bemenetként átadott jelentéslekérdezés</span><span class="sxs-lookup"><span data-stu-id="a2d5f-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="a2d5f-182">Típus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-182">Type</span></span>     |    <span data-ttu-id="a2d5f-183">Állítsa a beállításra: `userDefined`</span><span class="sxs-lookup"><span data-stu-id="a2d5f-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="a2d5f-184">Felhasználó</span><span class="sxs-lookup"><span data-stu-id="a2d5f-184">User</span></span>     |    <span data-ttu-id="a2d5f-185">A lekérdezés létrehozásához használt felhasználói azonosító</span><span class="sxs-lookup"><span data-stu-id="a2d5f-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="a2d5f-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="a2d5f-186">CreatedTime</span></span>     |    <span data-ttu-id="a2d5f-187">A lekérdezés a következő formátumban létrehozott UTC-ideje: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a2d5f-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a2d5f-188">TotalCount (Teljes összeg)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-188">TotalCount</span></span>     |    <span data-ttu-id="a2d5f-189">Adatkészletek száma az Érték tömbben</span><span class="sxs-lookup"><span data-stu-id="a2d5f-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="a2d5f-190">StatusCode (Állapotkód)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-190">StatusCode</span></span>     |    <span data-ttu-id="a2d5f-191">Eredmény kódja</span><span class="sxs-lookup"><span data-stu-id="a2d5f-191">Result Code</span></span> <br> <span data-ttu-id="a2d5f-192">Lehetséges értékek: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="a2d5f-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="a2d5f-193">message</span><span class="sxs-lookup"><span data-stu-id="a2d5f-193">message</span></span>     |    <span data-ttu-id="a2d5f-194">Állapotüzenet az API végrehajtásából</span><span class="sxs-lookup"><span data-stu-id="a2d5f-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="a2d5f-195">Jelentési API létrehozása</span><span class="sxs-lookup"><span data-stu-id="a2d5f-195">Create report API</span></span>

<span data-ttu-id="a2d5f-196">Ha sikeresen létrehozott egy egyéni jelentéssablont, és [](#create-report-query-api) a Jelentéslekérdezés létrehozása válasz részeként megkapja a QueryID-t, ezt az API-t hívhatja meg, hogy rendszeres időközönként ütemezni tudja a lekérdezések végrehajtását.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="a2d5f-197">Beállíthatja a jelentés kézbesítésének gyakoriságát és ütemezését.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="a2d5f-198">A rendszerlekérdezések esetén a Jelentés létrehozása API a QueryId használatával is [hívható.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="a2d5f-199">Visszahívási URL</span><span class="sxs-lookup"><span data-stu-id="a2d5f-199">Callback URL</span></span>

<span data-ttu-id="a2d5f-200">A jelentés létrehozása API visszahívási URL-címet fogad el.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="a2d5f-201">Ezt az URL-címet a rendszer a jelentés sikeres létrehozása után fogja meghívni.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="a2d5f-202">A visszahívási URL-címnek nyilvánosan elérhetőnek kell lennie.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="a2d5f-203">Az URL-cím mellett visszahívási metódus is adható.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="a2d5f-204">A visszahívási metódus csak "GET" vagy "POST" lehet.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="a2d5f-205">Ha nem ad meg értéket, az alapértelmezett metódus a "POST".</span><span class="sxs-lookup"><span data-stu-id="a2d5f-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="a2d5f-206">A befejezett jelentésazonosítót a visszahívás során mindig vissza kell kapnia.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="a2d5f-207">POST-visszahívás: Ha az átadott `https://www.contosso.com/callback` URL-cím , akkor a visszahívott URL-cím a következő lesz: `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="a2d5f-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="a2d5f-208">GET visszahívás: Ha az átadott `https://www.contosso.com/callback` URL-cím , akkor a visszahívott URL-cím a következő lesz: `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="a2d5f-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="a2d5f-209">ExecuteNow-jelentések</span><span class="sxs-lookup"><span data-stu-id="a2d5f-209">ExecuteNow reports</span></span>

<span data-ttu-id="a2d5f-210">Van olyan kiépítés, amely ütemezés nélkül hoz létre jelentést.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="a2d5f-211">A jelentés-létrehozási API hasznos adata elfogadhat egy paramétert, amely az API meghívása után a jelentés létrehozására `ExecuteNow` fog sorra hozni.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="a2d5f-212">Ha a true (igaz) érték van beállítva, a rendszer figyelmen kívül hagyja a (igaz) mezőket, mivel ezek a jelentések `ExecuteNow` `StartTime` nincsenek `RecurrenceCount` `RecurrenceInterval` ütemezve.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="a2d5f-213">Igaz érték esetén két további mező `ExecuteNow` is átvehet: `QueryStartTime` és `QueryEndTime` .</span><span class="sxs-lookup"><span data-stu-id="a2d5f-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="a2d5f-214">Ez a két mező felülírja `TIMESPAN` a lekérdezésben található mezőt.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="a2d5f-215">Ezek a mezők nem alkalmazhatók az ütemezett jelentésekre, mivel az adatok egy meghatározott ideig folyamatosan jönnek létre, amely nem változik.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="a2d5f-216">Kérésszintaxis</span><span class="sxs-lookup"><span data-stu-id="a2d5f-216">Request syntax</span></span>

|    <span data-ttu-id="a2d5f-217">Metódus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-217">Method</span></span>     |    <span data-ttu-id="a2d5f-218">Kérés URI-ja</span><span class="sxs-lookup"><span data-stu-id="a2d5f-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="a2d5f-219">POST</span><span class="sxs-lookup"><span data-stu-id="a2d5f-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="a2d5f-220">Kérelem fejléce</span><span class="sxs-lookup"><span data-stu-id="a2d5f-220">Request header</span></span>

|    <span data-ttu-id="a2d5f-221">Fejléc</span><span class="sxs-lookup"><span data-stu-id="a2d5f-221">Header</span></span>     |    <span data-ttu-id="a2d5f-222">Típus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-222">Type</span></span>     |    <span data-ttu-id="a2d5f-223">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="a2d5f-224">Engedélyezés</span><span class="sxs-lookup"><span data-stu-id="a2d5f-224">Authorization</span></span>     |    <span data-ttu-id="a2d5f-225">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-225">string</span></span> |<span data-ttu-id="a2d5f-226">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-226">Required.</span></span> <span data-ttu-id="a2d5f-227">Az Azure Active Directory (Azure AD) hozzáférési jogkivonata.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="a2d5f-228">A formátum  `Bearer <token>` a következő: .</span><span class="sxs-lookup"><span data-stu-id="a2d5f-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="a2d5f-229">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2d5f-229">Content-Type</span></span>     |<span data-ttu-id="a2d5f-230">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="a2d5f-231">Elérési út paramétere</span><span class="sxs-lookup"><span data-stu-id="a2d5f-231">Path Parameter</span></span>

<span data-ttu-id="a2d5f-232">None</span><span class="sxs-lookup"><span data-stu-id="a2d5f-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="a2d5f-233">Lekérdezési paraméter</span><span class="sxs-lookup"><span data-stu-id="a2d5f-233">Query Parameter</span></span>

<span data-ttu-id="a2d5f-234">None</span><span class="sxs-lookup"><span data-stu-id="a2d5f-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="a2d5f-235">Minta kérelem hasznosadata</span><span class="sxs-lookup"><span data-stu-id="a2d5f-235">Sample request payload</span></span>

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a><span data-ttu-id="a2d5f-236">Szószedet</span><span class="sxs-lookup"><span data-stu-id="a2d5f-236">Glossary</span></span>

<span data-ttu-id="a2d5f-237">A kérelem hasznos elemeinek kulcsdefinícióit az alábbiakban olvashatja:</span><span class="sxs-lookup"><span data-stu-id="a2d5f-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="a2d5f-238">Paraméter</span><span class="sxs-lookup"><span data-stu-id="a2d5f-238">Parameter</span></span>     |    <span data-ttu-id="a2d5f-239">Kötelező</span><span class="sxs-lookup"><span data-stu-id="a2d5f-239">Required</span></span>     |    <span data-ttu-id="a2d5f-240">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-240">Description</span></span>     |    <span data-ttu-id="a2d5f-241">Megengedett értékek</span><span class="sxs-lookup"><span data-stu-id="a2d5f-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="a2d5f-242">ReportName (Jelentés neve)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-242">ReportName</span></span>     |    <span data-ttu-id="a2d5f-243">Igen</span><span class="sxs-lookup"><span data-stu-id="a2d5f-243">Yes</span></span>     |    <span data-ttu-id="a2d5f-244">A jelentéshez hozzárendelni fog név</span><span class="sxs-lookup"><span data-stu-id="a2d5f-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="a2d5f-245">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-245">string</span></span>     |
|    <span data-ttu-id="a2d5f-246">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-246">Description</span></span>     |    <span data-ttu-id="a2d5f-247">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-247">No</span></span>     |    <span data-ttu-id="a2d5f-248">A létrehozott jelentés leírása</span><span class="sxs-lookup"><span data-stu-id="a2d5f-248">Description of the created report</span></span>     |    <span data-ttu-id="a2d5f-249">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-249">string</span></span>     |
|    <span data-ttu-id="a2d5f-250">QueryId (Lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-250">QueryId</span></span>     |    <span data-ttu-id="a2d5f-251">Igen</span><span class="sxs-lookup"><span data-stu-id="a2d5f-251">Yes</span></span>     |    <span data-ttu-id="a2d5f-252">Jelentéslekérdezés azonosítója</span><span class="sxs-lookup"><span data-stu-id="a2d5f-252">Report query ID</span></span>     |    <span data-ttu-id="a2d5f-253">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-253">string</span></span>     |
|    <span data-ttu-id="a2d5f-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="a2d5f-254">StartTime</span></span>     |    <span data-ttu-id="a2d5f-255">Igen</span><span class="sxs-lookup"><span data-stu-id="a2d5f-255">Yes</span></span>     |    <span data-ttu-id="a2d5f-256">A jelentés generálás megkezdésének UTC szerinti időbélyege.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="a2d5f-257">A formátumnak a következőnek kell lennie: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a2d5f-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="a2d5f-258">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-258">string</span></span>     |
|    <span data-ttu-id="a2d5f-259">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="a2d5f-259">ExecuteNow</span></span>     |    <span data-ttu-id="a2d5f-260">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-260">No</span></span>     |    <span data-ttu-id="a2d5f-261">Ezzel a paraméterrel olyan jelentést hozhat létre, amely csak egyszer lesz végrehajtva.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="a2d5f-262">`StartTime`A `RecurrenceInterval` és `RecurrenceCount` a értékeket a rendszer figyelmen kívül hagyja, ha true (igaz) érték van beállítva.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="a2d5f-263">A jelentés azonnal, aszinkron módon lesz végrehajtva</span><span class="sxs-lookup"><span data-stu-id="a2d5f-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="a2d5f-264">true/false (igaz/hamis)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-264">true/false</span></span>     |
|    <span data-ttu-id="a2d5f-265">QueryStartTime (Lekérdezésindítási idő)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-265">QueryStartTime</span></span>     |    <span data-ttu-id="a2d5f-266">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-266">No</span></span>     |    <span data-ttu-id="a2d5f-267">Igény szerint megadja az adatokat kinyerő lekérdezés kezdési idejét.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="a2d5f-268">Ez a paraméter csak egy olyan végrehajtási jelentésre alkalmazható, amely true `ExecuteNow` (igaz) értékre van állítva.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="a2d5f-269">A paraméter lekérdezésben megadott `TIMESPAN` felülbírálásai.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="a2d5f-270">A formátum legyen yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a2d5f-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="a2d5f-271">Időbélyeg sztringként</span><span class="sxs-lookup"><span data-stu-id="a2d5f-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="a2d5f-272">QueryEndTime (Lekérdezés ideje)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-272">QueryEndTime</span></span>     |    <span data-ttu-id="a2d5f-273">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-273">No</span></span>     |    <span data-ttu-id="a2d5f-274">Opcionálisan megadja az adatokat kinyerő lekérdezés záró idejét.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="a2d5f-275">Ez a paraméter csak egy olyan végrehajtási jelentésre alkalmazható, amely true `ExecuteNow` (igaz) értékre van állítva.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="a2d5f-276">A paraméter lekérdezésben megadott `TIMESPAN` felülbírálásai.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="a2d5f-277">A formátum legyen yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a2d5f-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="a2d5f-278">Időbélyeg sztringként</span><span class="sxs-lookup"><span data-stu-id="a2d5f-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="a2d5f-279">RecurrenceInterval (Ismétlődés időköze)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="a2d5f-280">Igen</span><span class="sxs-lookup"><span data-stu-id="a2d5f-280">Yes</span></span>     |    <span data-ttu-id="a2d5f-281">Gyakoriság órákban, amikor a jelentést létre kell hoznunk.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="a2d5f-282">A minimális érték 4, a Maximális érték pedig 2160.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="a2d5f-283">egész szám</span><span class="sxs-lookup"><span data-stu-id="a2d5f-283">integer</span></span>     |
|    <span data-ttu-id="a2d5f-284">RecurrenceCount (Ismétlődés száma)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-284">RecurrenceCount</span></span>     |    <span data-ttu-id="a2d5f-285">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-285">No</span></span>     |    <span data-ttu-id="a2d5f-286">A létrehozható jelentések száma.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="a2d5f-287">egész szám</span><span class="sxs-lookup"><span data-stu-id="a2d5f-287">integer</span></span>     |
|    <span data-ttu-id="a2d5f-288">Formátum</span><span class="sxs-lookup"><span data-stu-id="a2d5f-288">Format</span></span>     |    <span data-ttu-id="a2d5f-289">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-289">No</span></span>     |    <span data-ttu-id="a2d5f-290">Az exportált fájl fájlformátuma.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-290">File format of the exported file.</span></span> <br> <span data-ttu-id="a2d5f-291">Az alapértelmezett érték a CSV.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-291">Default is CSV.</span></span>    |    <span data-ttu-id="a2d5f-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="a2d5f-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="a2d5f-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="a2d5f-293">CallbackUrl</span></span>     |    <span data-ttu-id="a2d5f-294">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-294">No</span></span>     |    <span data-ttu-id="a2d5f-295">Nyilvánosan elérhető URL-cím, amely igény szerint visszahívási célként is konfigurálható</span><span class="sxs-lookup"><span data-stu-id="a2d5f-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="a2d5f-296">Sztring (http URL)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-296">String (http URL)</span></span>     |
|    <span data-ttu-id="a2d5f-297">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="a2d5f-297">CallbackMethod</span></span>     |    <span data-ttu-id="a2d5f-298">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-298">No</span></span>     |    <span data-ttu-id="a2d5f-299">A visszahíváshoz használt metódus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-299">The method to be used for callback</span></span>     |    <span data-ttu-id="a2d5f-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="a2d5f-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="a2d5f-301">Mintaválasz</span><span class="sxs-lookup"><span data-stu-id="a2d5f-301">Sample response</span></span>

<span data-ttu-id="a2d5f-302">A válasz hasznos adata a következőképpen strukturálva van:</span><span class="sxs-lookup"><span data-stu-id="a2d5f-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="a2d5f-303">Válaszkódok: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="a2d5f-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="a2d5f-304">Példa válasz hasznos hasznosra:</span><span class="sxs-lookup"><span data-stu-id="a2d5f-304">Response payload example:</span></span>

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a><span data-ttu-id="a2d5f-305">Szószedet</span><span class="sxs-lookup"><span data-stu-id="a2d5f-305">Glossary</span></span>

<span data-ttu-id="a2d5f-306">A válasz elemeinek kulcsdefiníciói az alábbiak:</span><span class="sxs-lookup"><span data-stu-id="a2d5f-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="a2d5f-307">Paraméter</span><span class="sxs-lookup"><span data-stu-id="a2d5f-307">Parameter</span></span>     |    <span data-ttu-id="a2d5f-308">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="a2d5f-309">Jelentésazonosító</span><span class="sxs-lookup"><span data-stu-id="a2d5f-309">ReportId</span></span>     |    <span data-ttu-id="a2d5f-310">A létrehozott jelentés univerzálisan egyedi azonosítója (UUID)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="a2d5f-311">ReportName (Jelentés neve)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-311">ReportName</span></span>     |    <span data-ttu-id="a2d5f-312">A jelentésnek a kérelem hasznos információja alapján megadott név</span><span class="sxs-lookup"><span data-stu-id="a2d5f-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="a2d5f-313">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-313">Description</span></span>     |    <span data-ttu-id="a2d5f-314">A jelentés létrehozása során megadott leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="a2d5f-315">QueryId (Lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-315">QueryId</span></span>     |    <span data-ttu-id="a2d5f-316">A jelentés létrehozásakor átadott lekérdezésazonosító</span><span class="sxs-lookup"><span data-stu-id="a2d5f-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="a2d5f-317">Lekérdezés</span><span class="sxs-lookup"><span data-stu-id="a2d5f-317">Query</span></span>     |    <span data-ttu-id="a2d5f-318">A jelentéshez végrehajtandó lekérdezési szöveg</span><span class="sxs-lookup"><span data-stu-id="a2d5f-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="a2d5f-319">Felhasználó</span><span class="sxs-lookup"><span data-stu-id="a2d5f-319">User</span></span>     |    <span data-ttu-id="a2d5f-320">A jelentés létrehozásához használt felhasználói azonosító</span><span class="sxs-lookup"><span data-stu-id="a2d5f-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="a2d5f-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="a2d5f-321">CreatedTime</span></span>     |    <span data-ttu-id="a2d5f-322">A jelentés a következő formátumban való létrehozásának UTC szerinti ideje: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a2d5f-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a2d5f-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="a2d5f-323">ModifiedTime</span></span>     |    <span data-ttu-id="a2d5f-324">A jelentés utolsó módosításának UTC szerinti időpontja a következő formátumban: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a2d5f-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a2d5f-325">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="a2d5f-325">ExecuteNow</span></span>     |    <span data-ttu-id="a2d5f-326">`ExecuteNow` a jelentés létrehozásakor beállított jelző</span><span class="sxs-lookup"><span data-stu-id="a2d5f-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="a2d5f-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="a2d5f-327">StartTime</span></span>     |    <span data-ttu-id="a2d5f-328">A jelentés végrehajtásának UTC szerinti kezdési ideje a következő formátumban: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a2d5f-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a2d5f-329">ReportStatus (Jelentésállapot)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-329">ReportStatus</span></span>     |    <span data-ttu-id="a2d5f-330">A jelentés végrehajtásának állapota.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-330">Status of the report execution.</span></span> <span data-ttu-id="a2d5f-331">A lehetséges értékek a `Paused` , `Active` a és a `Inactive`</span><span class="sxs-lookup"><span data-stu-id="a2d5f-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="a2d5f-332">RecurrenceInterval (Ismétlődés időköze)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="a2d5f-333">A jelentés létrehozása során megadott ismétlődési időköz</span><span class="sxs-lookup"><span data-stu-id="a2d5f-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="a2d5f-334">RecurrenceCount (Ismétlődés száma)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-334">RecurrenceCount</span></span>     |    <span data-ttu-id="a2d5f-335">A jelentés létrehozása során megadott ismétlődési szám.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="a2d5f-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="a2d5f-336">CallbackUrl</span></span>     |    <span data-ttu-id="a2d5f-337">A kérésben megadott visszahívási URL-cím</span><span class="sxs-lookup"><span data-stu-id="a2d5f-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="a2d5f-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="a2d5f-338">CallbackMethod</span></span>     |    <span data-ttu-id="a2d5f-339">A kérésben megadott visszahívási metódus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="a2d5f-340">Formátum</span><span class="sxs-lookup"><span data-stu-id="a2d5f-340">Format</span></span>     |    <span data-ttu-id="a2d5f-341">A jelentésfájlok formátuma.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-341">Format of the report files.</span></span> <span data-ttu-id="a2d5f-342">A lehetséges értékek a `CSV` vagy `TSV` a .</span><span class="sxs-lookup"><span data-stu-id="a2d5f-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="a2d5f-343">TotalCount (Teljes összeg)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-343">TotalCount</span></span>     |    <span data-ttu-id="a2d5f-344">Rekordok száma a Value tömbben</span><span class="sxs-lookup"><span data-stu-id="a2d5f-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="a2d5f-345">StatusCode (Állapotkód)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-345">StatusCode</span></span>     |    <span data-ttu-id="a2d5f-346">Eredmény kódja</span><span class="sxs-lookup"><span data-stu-id="a2d5f-346">Result Code</span></span>     |
|    <span data-ttu-id="a2d5f-347">message</span><span class="sxs-lookup"><span data-stu-id="a2d5f-347">message</span></span>     |    <span data-ttu-id="a2d5f-348">Lehetséges értékek: 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="a2d5f-349">Állapotüzenet az API végrehajtásából</span><span class="sxs-lookup"><span data-stu-id="a2d5f-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="a2d5f-350">Jelentés-végrehajtási API lekérte</span><span class="sxs-lookup"><span data-stu-id="a2d5f-350">Get report execution API</span></span>

<span data-ttu-id="a2d5f-351">Ezzel a módszerrel lekérdezheti egy jelentés végrehajtásának állapotát a Create Report API -tól kapott [ReportId (Jelentésazonosító) használatával.](#create-report-api)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="a2d5f-352">A metódus a jelentés letöltési hivatkozását adja vissza, ha a jelentés letöltésre kész.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="a2d5f-353">Ellenkező esetben a metódus visszaadja az állapotot.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="a2d5f-354">Ezzel az API-val le is kaphatja az adott jelentés összes végrehajtását.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="a2d5f-355">Az API alapértelmezett lekérdezési paraméterei és számára vannak `executionStatus=Completed` `getLatestExecution=true` beállítva.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="a2d5f-356">Ezért a jelentés első sikeres végrehajtása előtt az API hívása a 404-es adatokat adja vissza.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="a2d5f-357">Függőben lévő végrehajtások a beállításával szerezhetők `executionStatus=Pending` be.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="a2d5f-358">Kérésszintaxis</span><span class="sxs-lookup"><span data-stu-id="a2d5f-358">Request syntax</span></span>

|    <span data-ttu-id="a2d5f-359">Metódus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-359">Method</span></span>     |    <span data-ttu-id="a2d5f-360">Kérés URI-ja</span><span class="sxs-lookup"><span data-stu-id="a2d5f-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="a2d5f-361">GET</span><span class="sxs-lookup"><span data-stu-id="a2d5f-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="a2d5f-362">Kérelem fejléce</span><span class="sxs-lookup"><span data-stu-id="a2d5f-362">Request header</span></span>

|    <span data-ttu-id="a2d5f-363">Fejléc</span><span class="sxs-lookup"><span data-stu-id="a2d5f-363">Header</span></span>     |    <span data-ttu-id="a2d5f-364">Típus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-364">Type</span></span>     |    <span data-ttu-id="a2d5f-365">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="a2d5f-366">Engedélyezés</span><span class="sxs-lookup"><span data-stu-id="a2d5f-366">Authorization</span></span>     |    <span data-ttu-id="a2d5f-367">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-367">string</span></span> |<span data-ttu-id="a2d5f-368">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-368">Required.</span></span> <span data-ttu-id="a2d5f-369">Az Azure Active Directory (Azure AD) hozzáférési jogkivonata.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="a2d5f-370">A formátum  `Bearer <token>` a következő: .</span><span class="sxs-lookup"><span data-stu-id="a2d5f-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="a2d5f-371">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2d5f-371">Content-Type</span></span>     |<span data-ttu-id="a2d5f-372">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="a2d5f-373">Elérésiút-paraméter</span><span class="sxs-lookup"><span data-stu-id="a2d5f-373">Path parameter</span></span>

|    <span data-ttu-id="a2d5f-374">Paraméter neve</span><span class="sxs-lookup"><span data-stu-id="a2d5f-374">Parameter Name</span></span>    |    <span data-ttu-id="a2d5f-375">Kötelező</span><span class="sxs-lookup"><span data-stu-id="a2d5f-375">Required</span></span>    |    <span data-ttu-id="a2d5f-376">Típus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-376">Type</span></span>    |    <span data-ttu-id="a2d5f-377">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="a2d5f-378">jelentésazonosító</span><span class="sxs-lookup"><span data-stu-id="a2d5f-378">reportId</span></span>    |    <span data-ttu-id="a2d5f-379">Igen</span><span class="sxs-lookup"><span data-stu-id="a2d5f-379">Yes</span></span>    |    <span data-ttu-id="a2d5f-380">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-380">string</span></span>    |    <span data-ttu-id="a2d5f-381">Szűrhet, hogy csak az ebben az argumentumban megadott jelentésazonosítóval kapcsolatos jelentések végrehajtási adatait lekérte.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="a2d5f-382">Több jelentésazonosítót is meg lehet adni pontosvesszővel (;) elválasztva.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="a2d5f-383">Lekérdezési paraméter</span><span class="sxs-lookup"><span data-stu-id="a2d5f-383">Query parameter</span></span>

|    <span data-ttu-id="a2d5f-384">Paraméter neve</span><span class="sxs-lookup"><span data-stu-id="a2d5f-384">Parameter Name</span></span>    |    <span data-ttu-id="a2d5f-385">Kötelező</span><span class="sxs-lookup"><span data-stu-id="a2d5f-385">Required</span></span>    |    <span data-ttu-id="a2d5f-386">Típus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-386">Type</span></span>    |    <span data-ttu-id="a2d5f-387">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="a2d5f-388">executionId (végrehajtásiazonosító)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-388">executionId</span></span>    |    <span data-ttu-id="a2d5f-389">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-389">No</span></span>    |    <span data-ttu-id="a2d5f-390">sztring</span><span class="sxs-lookup"><span data-stu-id="a2d5f-390">string</span></span>    |    <span data-ttu-id="a2d5f-391">Szűrhet, hogy csak az ebben az argumentumban megadott executionId -et tartalmazó jelentések adatait lekérte.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="a2d5f-392">Pontosvesszővel (;) elválasztva több executionId is meg lehet adni.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="a2d5f-393">executionStatus (végrehajtásiállapot)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-393">executionStatus</span></span>    |    <span data-ttu-id="a2d5f-394">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-394">No</span></span>    |    <span data-ttu-id="a2d5f-395">Sztring/enum</span><span class="sxs-lookup"><span data-stu-id="a2d5f-395">String/enum</span></span>    |    <span data-ttu-id="a2d5f-396">Szűrhet, hogy csak az ebben az argumentumban megadott executionStatus jelentéseket tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="a2d5f-397">Érvényes értékek: `Pending` , `Running` és `Paused` `Completed` .</span><span class="sxs-lookup"><span data-stu-id="a2d5f-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="a2d5f-398">Az alapértelmezett érték `Completed`.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="a2d5f-399">Pontosvesszővel (;) elválasztva több állapot is meg lehet adni.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="a2d5f-400">getLatestExecution (GetLatestExecution)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-400">getLatestExecution</span></span>    |    <span data-ttu-id="a2d5f-401">Nem</span><span class="sxs-lookup"><span data-stu-id="a2d5f-401">No</span></span>    |    <span data-ttu-id="a2d5f-402">boolean</span><span class="sxs-lookup"><span data-stu-id="a2d5f-402">boolean</span></span>    |    <span data-ttu-id="a2d5f-403">Az API visszaadja a legutóbbi végrehajtás részleteit.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="a2d5f-404">Alapértelmezés szerint ez a paraméter true (igaz) értéket ad meg.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="a2d5f-405">Ha úgy dönt, hogy a paraméter értékét false (hamis) értékként adja át, akkor az API az utolsó 90 nap végrehajtási példányait adja vissza.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="a2d5f-406">Minta kérelem hasznosadata</span><span class="sxs-lookup"><span data-stu-id="a2d5f-406">Sample Request Payload</span></span>

<span data-ttu-id="a2d5f-407">None</span><span class="sxs-lookup"><span data-stu-id="a2d5f-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="a2d5f-408">Mintaválasz</span><span class="sxs-lookup"><span data-stu-id="a2d5f-408">Sample Response</span></span>

<span data-ttu-id="a2d5f-409">A válasz hasznos adata a következőképpen strukturálva van:</span><span class="sxs-lookup"><span data-stu-id="a2d5f-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="a2d5f-410">Válaszkódok: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="a2d5f-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="a2d5f-411">Példa válasz hasznos hasznosra:</span><span class="sxs-lookup"><span data-stu-id="a2d5f-411">Response payload example:</span></span>

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="a2d5f-412">Ha a jelentés végrehajtása befejeződött, megjelenik a `Completed` végrehajtás állapota.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="a2d5f-413">A jelentést a URL-címének kiválasztásával töltheti `reportAccessSecureLink` le.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="a2d5f-414">Szószedet</span><span class="sxs-lookup"><span data-stu-id="a2d5f-414">Glossary</span></span>

<span data-ttu-id="a2d5f-415">A válasz elemeinek kulcsdefiníciói.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="a2d5f-416">Paraméter</span><span class="sxs-lookup"><span data-stu-id="a2d5f-416">Parameter</span></span>    |    <span data-ttu-id="a2d5f-417">Leírás</span><span class="sxs-lookup"><span data-stu-id="a2d5f-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="a2d5f-418">ExecutionId (Végrehajtásiazonosító)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-418">ExecutionId</span></span>    |    <span data-ttu-id="a2d5f-419">A végrehajtási példány univerzálisan egyedi azonosítója (UUID)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="a2d5f-420">ReportId (Jelentésazonosító)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-420">ReportId</span></span>    |    <span data-ttu-id="a2d5f-421">A végrehajtási példányhoz társított jelentésazonosító</span><span class="sxs-lookup"><span data-stu-id="a2d5f-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="a2d5f-422">RecurrenceInterval (Ismétlődés időköze)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="a2d5f-423">A jelentés létrehozása során megadott ismétlődési időköz</span><span class="sxs-lookup"><span data-stu-id="a2d5f-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="a2d5f-424">RecurrenceCount (Ismétlődés száma)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-424">RecurrenceCount</span></span>    |    <span data-ttu-id="a2d5f-425">A jelentés létrehozása során megadott ismétlődési szám</span><span class="sxs-lookup"><span data-stu-id="a2d5f-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="a2d5f-426">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="a2d5f-426">CallbackUrl</span></span>    |    <span data-ttu-id="a2d5f-427">A végrehajtási példányhoz társított visszahívási URL-cím</span><span class="sxs-lookup"><span data-stu-id="a2d5f-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="a2d5f-428">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="a2d5f-428">CallbackMethod</span></span>    |    <span data-ttu-id="a2d5f-429">A végrehajtási példányhoz társított visszahívási metódus</span><span class="sxs-lookup"><span data-stu-id="a2d5f-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="a2d5f-430">Formátum</span><span class="sxs-lookup"><span data-stu-id="a2d5f-430">Format</span></span>    |    <span data-ttu-id="a2d5f-431">A végrehajtás végén létrehozott fájl formátuma</span><span class="sxs-lookup"><span data-stu-id="a2d5f-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="a2d5f-432">ExecutionStatus (Végrehajtásiállapot)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-432">ExecutionStatus</span></span>    |    <span data-ttu-id="a2d5f-433">A jelentés-végrehajtási példány állapota.</span><span class="sxs-lookup"><span data-stu-id="a2d5f-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="a2d5f-434">Érvényes értékek: `Pending` , `Running` , `Paused` és `Completed`</span><span class="sxs-lookup"><span data-stu-id="a2d5f-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="a2d5f-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="a2d5f-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="a2d5f-436">Hivatkozás, amelyen keresztül a jelentés biztonságosan elérhető</span><span class="sxs-lookup"><span data-stu-id="a2d5f-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="a2d5f-437">ReportExpiryTime</span><span class="sxs-lookup"><span data-stu-id="a2d5f-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="a2d5f-438">A jelentéshivatkozás lejáratának UTC szerinti ideje a következő formátumban: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a2d5f-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="a2d5f-439">ReportGeneratedTime (Jelentésgenerált idő)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="a2d5f-440">A jelentés a következő formátumban létrehozott UTC-ideje: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a2d5f-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="a2d5f-441">TotalCount (Teljes összeg)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-441">TotalCount</span></span>    |    <span data-ttu-id="a2d5f-442">Adatkészletek száma az Érték tömbben</span><span class="sxs-lookup"><span data-stu-id="a2d5f-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="a2d5f-443">StatusCode (Állapotkód)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-443">StatusCode</span></span>    |    <span data-ttu-id="a2d5f-444">Eredmény kódja</span><span class="sxs-lookup"><span data-stu-id="a2d5f-444">Result Code</span></span> <br> <span data-ttu-id="a2d5f-445">Lehetséges értékek: 200, 400, 401, 403, 404 és 500</span><span class="sxs-lookup"><span data-stu-id="a2d5f-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="a2d5f-446">message</span><span class="sxs-lookup"><span data-stu-id="a2d5f-446">message</span></span>    |    <span data-ttu-id="a2d5f-447">Állapotüzenet az API végrehajtásából</span><span class="sxs-lookup"><span data-stu-id="a2d5f-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="a2d5f-448">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="a2d5f-448">Next steps</span></span>

- <span data-ttu-id="a2d5f-449">Próbálja ki az API-kat a [swagger API URL-címével](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="a2d5f-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="a2d5f-450">Az első API-hívás hívása</span><span class="sxs-lookup"><span data-stu-id="a2d5f-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)