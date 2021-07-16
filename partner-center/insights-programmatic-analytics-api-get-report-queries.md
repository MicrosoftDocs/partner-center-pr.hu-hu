---
title: Jelentéslekérdezések API-ja – Elemzések adatok lekérdezve
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val lekérdezhető az összes rendelkezésre álló lekérdezés a jelentési API-ban való használatra.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376751"
---
# <a name="get-report-queries-api"></a><span data-ttu-id="ce194-103">Jelentéslekérdezések API-jának le kérése</span><span class="sxs-lookup"><span data-stu-id="ce194-103">Get report queries API</span></span>

<span data-ttu-id="ce194-104">A Jelentéslekérdezések lekérdezi API lekérdezi a jelentésekben használható összes lekérdezést.</span><span class="sxs-lookup"><span data-stu-id="ce194-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="ce194-105">Alapértelmezés szerint lekérdezi az összes rendszer- és felhasználó által megadott lekérdezést.</span><span class="sxs-lookup"><span data-stu-id="ce194-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="ce194-106">**Kérésszintaxis**</span><span class="sxs-lookup"><span data-stu-id="ce194-106">**Request syntax**</span></span>

|    <span data-ttu-id="ce194-107">Metódus</span><span class="sxs-lookup"><span data-stu-id="ce194-107">Method</span></span>    |    <span data-ttu-id="ce194-108">Kérés URI-ja</span><span class="sxs-lookup"><span data-stu-id="ce194-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ce194-109">GET</span><span class="sxs-lookup"><span data-stu-id="ce194-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="ce194-110">**Kérés fejléce**</span><span class="sxs-lookup"><span data-stu-id="ce194-110">**Request header**</span></span>

|    <span data-ttu-id="ce194-111">Fejléc</span><span class="sxs-lookup"><span data-stu-id="ce194-111">Header</span></span>    |    <span data-ttu-id="ce194-112">Típus</span><span class="sxs-lookup"><span data-stu-id="ce194-112">Type</span></span>    |    <span data-ttu-id="ce194-113">Leírás</span><span class="sxs-lookup"><span data-stu-id="ce194-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="ce194-114">Engedélyezés</span><span class="sxs-lookup"><span data-stu-id="ce194-114">Authorization</span></span>    |    <span data-ttu-id="ce194-115">sztring</span><span class="sxs-lookup"><span data-stu-id="ce194-115">string</span></span>    |    <span data-ttu-id="ce194-116">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="ce194-116">Required.</span></span> <span data-ttu-id="ce194-117">Az Azure Active Directory (AAD) hozzáférési jogkivonata a következő formában:`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="ce194-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="ce194-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce194-118">Content-Type</span></span>    |    <span data-ttu-id="ce194-119">sztring</span><span class="sxs-lookup"><span data-stu-id="ce194-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="ce194-120">**Elérésiút-paraméter**</span><span class="sxs-lookup"><span data-stu-id="ce194-120">**Path parameter**</span></span>

<span data-ttu-id="ce194-121">None</span><span class="sxs-lookup"><span data-stu-id="ce194-121">None</span></span>

<span data-ttu-id="ce194-122">**Lekérdezési paraméter**</span><span class="sxs-lookup"><span data-stu-id="ce194-122">**Query parameter**</span></span>

|    <span data-ttu-id="ce194-123">Paraméter neve</span><span class="sxs-lookup"><span data-stu-id="ce194-123">Parameter Name</span></span>    |    <span data-ttu-id="ce194-124">Típus</span><span class="sxs-lookup"><span data-stu-id="ce194-124">Type</span></span>    |    <span data-ttu-id="ce194-125">Kötelező</span><span class="sxs-lookup"><span data-stu-id="ce194-125">Required</span></span>    |    <span data-ttu-id="ce194-126">Leírás</span><span class="sxs-lookup"><span data-stu-id="ce194-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="ce194-127">queryId (lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="ce194-127">queryId</span></span>     |    <span data-ttu-id="ce194-128">sztring</span><span class="sxs-lookup"><span data-stu-id="ce194-128">string</span></span>     |    <span data-ttu-id="ce194-129">No</span><span class="sxs-lookup"><span data-stu-id="ce194-129">No</span></span>    |    <span data-ttu-id="ce194-130">Szűrés, ha csak a argumentumban megadott azonosítóval megadott lekérdezések adatait lekérdezi</span><span class="sxs-lookup"><span data-stu-id="ce194-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="ce194-131">queryName (lekérdezés neve)</span><span class="sxs-lookup"><span data-stu-id="ce194-131">queryName</span></span>     |    <span data-ttu-id="ce194-132">sztring</span><span class="sxs-lookup"><span data-stu-id="ce194-132">string</span></span>     |    <span data-ttu-id="ce194-133">No</span><span class="sxs-lookup"><span data-stu-id="ce194-133">No</span></span>    |    <span data-ttu-id="ce194-134">Szűrhet, hogy csak a argumentumban megadott nevű lekérdezések adatait lekérdezze</span><span class="sxs-lookup"><span data-stu-id="ce194-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="ce194-135">IncludeSystemQueries (Fájlrendszerlekérdezés)</span><span class="sxs-lookup"><span data-stu-id="ce194-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="ce194-136">boolean</span><span class="sxs-lookup"><span data-stu-id="ce194-136">boolean</span></span>     |    <span data-ttu-id="ce194-137">Nem</span><span class="sxs-lookup"><span data-stu-id="ce194-137">No</span></span>    |    <span data-ttu-id="ce194-138">Előre definiált rendszerlekérdezések a válaszban</span><span class="sxs-lookup"><span data-stu-id="ce194-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="ce194-139">IncludeOnlySystemQueries</span><span class="sxs-lookup"><span data-stu-id="ce194-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="ce194-140">boolean</span><span class="sxs-lookup"><span data-stu-id="ce194-140">boolean</span></span>     |    <span data-ttu-id="ce194-141">Nem</span><span class="sxs-lookup"><span data-stu-id="ce194-141">No</span></span>    |    <span data-ttu-id="ce194-142">Csak rendszerlekérdezések szerepeljenek a válaszban</span><span class="sxs-lookup"><span data-stu-id="ce194-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="ce194-143">**Hasznos információ kérése**</span><span class="sxs-lookup"><span data-stu-id="ce194-143">**Request payload**</span></span>

<span data-ttu-id="ce194-144">None</span><span class="sxs-lookup"><span data-stu-id="ce194-144">None</span></span>

<span data-ttu-id="ce194-145">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="ce194-145">**Glossary**</span></span>

<span data-ttu-id="ce194-146">None</span><span class="sxs-lookup"><span data-stu-id="ce194-146">None</span></span>

<span data-ttu-id="ce194-147">**Válasz**</span><span class="sxs-lookup"><span data-stu-id="ce194-147">**Response**</span></span>

<span data-ttu-id="ce194-148">A válasz hasznos adata a következőképpen strukturálva van:</span><span class="sxs-lookup"><span data-stu-id="ce194-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="ce194-149">Válaszkód: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="ce194-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="ce194-150">Példa válasz hasznos hasznosra:</span><span class="sxs-lookup"><span data-stu-id="ce194-150">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="ce194-151">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="ce194-151">**Glossary**</span></span>

<span data-ttu-id="ce194-152">Ez a tábla határozza meg a válasz legfontosabb elemeit:</span><span class="sxs-lookup"><span data-stu-id="ce194-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="ce194-153">Paraméter</span><span class="sxs-lookup"><span data-stu-id="ce194-153">Parameter</span></span>    |    <span data-ttu-id="ce194-154">Leírás</span><span class="sxs-lookup"><span data-stu-id="ce194-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ce194-155">QueryId (Lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="ce194-155">QueryId</span></span>     |    <span data-ttu-id="ce194-156">A lekérdezés egyedi UUID-je</span><span class="sxs-lookup"><span data-stu-id="ce194-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="ce194-157">Name</span><span class="sxs-lookup"><span data-stu-id="ce194-157">Name</span></span>     |    <span data-ttu-id="ce194-158">A lekérdezésnek a lekérdezés létrehozásakor megadott név</span><span class="sxs-lookup"><span data-stu-id="ce194-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="ce194-159">Leírás</span><span class="sxs-lookup"><span data-stu-id="ce194-159">Description</span></span>     |    <span data-ttu-id="ce194-160">A lekérdezés létrehozása során megadott leírás</span><span class="sxs-lookup"><span data-stu-id="ce194-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="ce194-161">Lekérdezés</span><span class="sxs-lookup"><span data-stu-id="ce194-161">Query</span></span>     |    <span data-ttu-id="ce194-162">Jelentés lekérdezési sztringe</span><span class="sxs-lookup"><span data-stu-id="ce194-162">Report query string</span></span>     |
|    <span data-ttu-id="ce194-163">Típus</span><span class="sxs-lookup"><span data-stu-id="ce194-163">Type</span></span>     |    <span data-ttu-id="ce194-164">Felhasználó által létrehozott lekérdezésekhez és rendszerhez előre definiált rendszerlekérdezésekhez állítsa be a userDefined értéket</span><span class="sxs-lookup"><span data-stu-id="ce194-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="ce194-165">Felhasználó</span><span class="sxs-lookup"><span data-stu-id="ce194-165">User</span></span>     |    <span data-ttu-id="ce194-166">A lekérdezést létrehozó felhasználói azonosító</span><span class="sxs-lookup"><span data-stu-id="ce194-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="ce194-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="ce194-167">CreatedTime</span></span>     |    <span data-ttu-id="ce194-168">A lekérdezés létrehozásának ideje</span><span class="sxs-lookup"><span data-stu-id="ce194-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="ce194-169">TotalCount (Teljes összeg)</span><span class="sxs-lookup"><span data-stu-id="ce194-169">TotalCount</span></span>     |    <span data-ttu-id="ce194-170">Adatkészletek száma az Érték tömbben</span><span class="sxs-lookup"><span data-stu-id="ce194-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="ce194-171">Üzenet</span><span class="sxs-lookup"><span data-stu-id="ce194-171">Message</span></span>     |    <span data-ttu-id="ce194-172">Állapotüzenet az API végrehajtásából</span><span class="sxs-lookup"><span data-stu-id="ce194-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="ce194-173">StatusCode (Állapotkód)</span><span class="sxs-lookup"><span data-stu-id="ce194-173">StatusCode</span></span>     |    <span data-ttu-id="ce194-174">Eredménykód.</span><span class="sxs-lookup"><span data-stu-id="ce194-174">Result Code.</span></span> <span data-ttu-id="ce194-175">Lehetséges értékek: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="ce194-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
