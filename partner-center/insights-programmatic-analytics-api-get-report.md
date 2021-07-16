---
title: Jelentés API-k le Elemzések adatok
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val lekérhetők az összes elérhető jelentésazonosító a Partnerközpont elemzésben.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376750"
---
# <a name="get-report-api"></a><span data-ttu-id="7ffa0-103">A jelentés API-jának lekérte</span><span class="sxs-lookup"><span data-stu-id="7ffa0-103">Get report API</span></span>

<span data-ttu-id="7ffa0-104">Ez az API lekért minden ütemezett jelentést.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="7ffa0-105">**Kérés szintaxisa**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-105">**Request syntax**</span></span>

|    <span data-ttu-id="7ffa0-106">Metódus</span><span class="sxs-lookup"><span data-stu-id="7ffa0-106">Method</span></span>    |    <span data-ttu-id="7ffa0-107">Kérés URI-ja</span><span class="sxs-lookup"><span data-stu-id="7ffa0-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="7ffa0-108">GET</span><span class="sxs-lookup"><span data-stu-id="7ffa0-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="7ffa0-109">**Kérelemfejléc**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-109">**Request header**</span></span>

|    <span data-ttu-id="7ffa0-110">Fejléc</span><span class="sxs-lookup"><span data-stu-id="7ffa0-110">Header</span></span>    |    <span data-ttu-id="7ffa0-111">Típus</span><span class="sxs-lookup"><span data-stu-id="7ffa0-111">Type</span></span>    |    <span data-ttu-id="7ffa0-112">Leírás</span><span class="sxs-lookup"><span data-stu-id="7ffa0-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="7ffa0-113">Engedélyezés</span><span class="sxs-lookup"><span data-stu-id="7ffa0-113">Authorization</span></span>    |    <span data-ttu-id="7ffa0-114">sztring</span><span class="sxs-lookup"><span data-stu-id="7ffa0-114">string</span></span>    |    <span data-ttu-id="7ffa0-115">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-115">Required.</span></span> <span data-ttu-id="7ffa0-116">Az Azure Active Directory (AAD) hozzáférési jogkivonat a következő formában:`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="7ffa0-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="7ffa0-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ffa0-117">Content-Type</span></span>    |    <span data-ttu-id="7ffa0-118">sztring</span><span class="sxs-lookup"><span data-stu-id="7ffa0-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="7ffa0-119">**Elérésiút-paraméter**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-119">**Path parameter**</span></span>

<span data-ttu-id="7ffa0-120">None</span><span class="sxs-lookup"><span data-stu-id="7ffa0-120">None</span></span>

<span data-ttu-id="7ffa0-121">**Lekérdezési paraméter**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-121">**Query parameter**</span></span>

|    <span data-ttu-id="7ffa0-122">Paraméter neve</span><span class="sxs-lookup"><span data-stu-id="7ffa0-122">Parameter Name</span></span>    |    <span data-ttu-id="7ffa0-123">Típus</span><span class="sxs-lookup"><span data-stu-id="7ffa0-123">Type</span></span>    |    <span data-ttu-id="7ffa0-124">Kötelező</span><span class="sxs-lookup"><span data-stu-id="7ffa0-124">Required</span></span>    |    <span data-ttu-id="7ffa0-125">Leírás</span><span class="sxs-lookup"><span data-stu-id="7ffa0-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="7ffa0-126">jelentésazonosító</span><span class="sxs-lookup"><span data-stu-id="7ffa0-126">reportId</span></span>     |    <span data-ttu-id="7ffa0-127">sztring</span><span class="sxs-lookup"><span data-stu-id="7ffa0-127">string</span></span>    |    <span data-ttu-id="7ffa0-128">No</span><span class="sxs-lookup"><span data-stu-id="7ffa0-128">No</span></span>    |    <span data-ttu-id="7ffa0-129">Szűrhet, hogy csak az ebben az argumentumban megadott reportId-t tartalmazó jelentések részleteit lekérte</span><span class="sxs-lookup"><span data-stu-id="7ffa0-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="7ffa0-130">reportName (jelentés neve)</span><span class="sxs-lookup"><span data-stu-id="7ffa0-130">reportName</span></span>     |    <span data-ttu-id="7ffa0-131">sztring</span><span class="sxs-lookup"><span data-stu-id="7ffa0-131">string</span></span>    |    <span data-ttu-id="7ffa0-132">No</span><span class="sxs-lookup"><span data-stu-id="7ffa0-132">No</span></span>    |    <span data-ttu-id="7ffa0-133">Szűrhet, hogy csak az ebben az argumentumban megadott reportName paramétert tartalmazó jelentések részleteit lekérte</span><span class="sxs-lookup"><span data-stu-id="7ffa0-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="7ffa0-134">queryId (lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="7ffa0-134">queryId</span></span>     |    <span data-ttu-id="7ffa0-135">sztring</span><span class="sxs-lookup"><span data-stu-id="7ffa0-135">string</span></span>    |    <span data-ttu-id="7ffa0-136">No</span><span class="sxs-lookup"><span data-stu-id="7ffa0-136">No</span></span>    |    <span data-ttu-id="7ffa0-137">Szűrhet, hogy csak az ebben az argumentumban megadott queryId-t tartalmazó jelentések adatait lekérdezze</span><span class="sxs-lookup"><span data-stu-id="7ffa0-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="7ffa0-138">**Hasznos információ kérése**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-138">**Request payload**</span></span>

<span data-ttu-id="7ffa0-139">None</span><span class="sxs-lookup"><span data-stu-id="7ffa0-139">None</span></span>

<span data-ttu-id="7ffa0-140">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-140">**Glossary**</span></span>

<span data-ttu-id="7ffa0-141">None</span><span class="sxs-lookup"><span data-stu-id="7ffa0-141">None</span></span>

<span data-ttu-id="7ffa0-142">**Válasz**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-142">**Response**</span></span>

<span data-ttu-id="7ffa0-143">A válasz hasznos adata a következőképpen strukturálva van:</span><span class="sxs-lookup"><span data-stu-id="7ffa0-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="7ffa0-144">Válaszkód: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="7ffa0-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="7ffa0-145">Példa válasz hasznos hasznosra:</span><span class="sxs-lookup"><span data-stu-id="7ffa0-145">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="7ffa0-146">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-146">**Glossary**</span></span>

<span data-ttu-id="7ffa0-147">Ez a tábla határozza meg a válasz legfontosabb elemeit:</span><span class="sxs-lookup"><span data-stu-id="7ffa0-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="7ffa0-148">Paraméter</span><span class="sxs-lookup"><span data-stu-id="7ffa0-148">Parameter</span></span>    |    <span data-ttu-id="7ffa0-149">Leírás</span><span class="sxs-lookup"><span data-stu-id="7ffa0-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="7ffa0-150">ReportId (Jelentésazonosító)</span><span class="sxs-lookup"><span data-stu-id="7ffa0-150">ReportId</span></span>     |    <span data-ttu-id="7ffa0-151">A létrehozott jelentés egyedi UUID-je</span><span class="sxs-lookup"><span data-stu-id="7ffa0-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="7ffa0-152">ReportName (Jelentés neve)</span><span class="sxs-lookup"><span data-stu-id="7ffa0-152">ReportName</span></span>     |    <span data-ttu-id="7ffa0-153">A jelentésnek a kérelem hasznos információban megadott neve</span><span class="sxs-lookup"><span data-stu-id="7ffa0-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="7ffa0-154">Leírás</span><span class="sxs-lookup"><span data-stu-id="7ffa0-154">Description</span></span>     |    <span data-ttu-id="7ffa0-155">A jelentés létrehozásakor megadott leírás</span><span class="sxs-lookup"><span data-stu-id="7ffa0-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="7ffa0-156">QueryId (Lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="7ffa0-156">QueryId</span></span>     |    <span data-ttu-id="7ffa0-157">A jelentés létrehozásakor átadott lekérdezésazonosító</span><span class="sxs-lookup"><span data-stu-id="7ffa0-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="7ffa0-158">Lekérdezés</span><span class="sxs-lookup"><span data-stu-id="7ffa0-158">Query</span></span>     |    <span data-ttu-id="7ffa0-159">A jelentéshez végrehajtandó szöveg lekérdezése</span><span class="sxs-lookup"><span data-stu-id="7ffa0-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="7ffa0-160">Felhasználó</span><span class="sxs-lookup"><span data-stu-id="7ffa0-160">User</span></span>     |    <span data-ttu-id="7ffa0-161">A jelentés létrehozásához használt felhasználói azonosító</span><span class="sxs-lookup"><span data-stu-id="7ffa0-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="7ffa0-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="7ffa0-162">CreatedTime</span></span>     |    <span data-ttu-id="7ffa0-163">A jelentés létrehozási ideje.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-163">Time the report was created.</span></span> <span data-ttu-id="7ffa0-164">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="7ffa0-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="7ffa0-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="7ffa0-165">ModifiedTime</span></span>     |    <span data-ttu-id="7ffa0-166">A jelentés utolsó módosításának időpontja.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-166">Time the report was last modified.</span></span> <span data-ttu-id="7ffa0-167">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="7ffa0-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="7ffa0-168">executeNow</span><span class="sxs-lookup"><span data-stu-id="7ffa0-168">executeNow</span></span>     |    <span data-ttu-id="7ffa0-169">A jelentés létrehozásakor beállított ExecuteNow jelző</span><span class="sxs-lookup"><span data-stu-id="7ffa0-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="7ffa0-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="7ffa0-170">StartTime</span></span>     |    <span data-ttu-id="7ffa0-171">Megkezdődik az idő végrehajtása.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-171">Time execution will begin.</span></span> <span data-ttu-id="7ffa0-172">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="7ffa0-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="7ffa0-173">ReportStatus (Jelentésállapot)</span><span class="sxs-lookup"><span data-stu-id="7ffa0-173">ReportStatus</span></span>     |    <span data-ttu-id="7ffa0-174">A jelentés végrehajtásának állapota.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-174">Status of the report execution.</span></span> <span data-ttu-id="7ffa0-175">A lehetséges értékek: Szüneteltetve, Aktív és Inaktív.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="7ffa0-176">RecurrenceInterval (Ismétlődés időköze)</span><span class="sxs-lookup"><span data-stu-id="7ffa0-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="7ffa0-177">A jelentés létrehozása során megadott ismétlődési időköz</span><span class="sxs-lookup"><span data-stu-id="7ffa0-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="7ffa0-178">RecurrenceCount (Ismétlődés száma)</span><span class="sxs-lookup"><span data-stu-id="7ffa0-178">RecurrenceCount</span></span>     |    <span data-ttu-id="7ffa0-179">A jelentés létrehozása során megadott ismétlődési szám</span><span class="sxs-lookup"><span data-stu-id="7ffa0-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="7ffa0-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="7ffa0-180">CallbackUrl</span></span>     |    <span data-ttu-id="7ffa0-181">A kérésben megadott visszahívási URL-cím</span><span class="sxs-lookup"><span data-stu-id="7ffa0-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="7ffa0-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="7ffa0-182">CallbackMethod</span></span>    |    <span data-ttu-id="7ffa0-183">A kérésben megadott visszahívási metódus</span><span class="sxs-lookup"><span data-stu-id="7ffa0-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="7ffa0-184">Formátum</span><span class="sxs-lookup"><span data-stu-id="7ffa0-184">Format</span></span>     |    <span data-ttu-id="7ffa0-185">A jelentésfájlok formátuma</span><span class="sxs-lookup"><span data-stu-id="7ffa0-185">Format of the report files</span></span>     |
|    <span data-ttu-id="7ffa0-186">TotalCount (Teljes összeg)</span><span class="sxs-lookup"><span data-stu-id="7ffa0-186">TotalCount</span></span>     |    <span data-ttu-id="7ffa0-187">Adatkészletek száma az Érték tömbben</span><span class="sxs-lookup"><span data-stu-id="7ffa0-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="7ffa0-188">Üzenet</span><span class="sxs-lookup"><span data-stu-id="7ffa0-188">Message</span></span>     |    <span data-ttu-id="7ffa0-189">Állapotüzenet az API végrehajtásából</span><span class="sxs-lookup"><span data-stu-id="7ffa0-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="7ffa0-190">StatusCode (Állapotkód)</span><span class="sxs-lookup"><span data-stu-id="7ffa0-190">StatusCode</span></span>     |    <span data-ttu-id="7ffa0-191">Eredménykód.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-191">Result Code.</span></span> <span data-ttu-id="7ffa0-192">Lehetséges értékek: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="7ffa0-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |