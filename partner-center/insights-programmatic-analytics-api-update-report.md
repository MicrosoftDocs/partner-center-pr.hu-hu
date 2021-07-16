---
title: Jelentési API frissítése
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val frissítheti a jelentésparamétereket az Partnerközpont elemzésben.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376734"
---
# <a name="update-report-api"></a><span data-ttu-id="1bd58-103">Jelentési API frissítése</span><span class="sxs-lookup"><span data-stu-id="1bd58-103">Update report API</span></span>

<span data-ttu-id="1bd58-104">Ez az API segít a jelentésparaméterek módosításában.</span><span class="sxs-lookup"><span data-stu-id="1bd58-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="1bd58-105">**Kérés szintaxisa**</span><span class="sxs-lookup"><span data-stu-id="1bd58-105">**Request syntax**</span></span>

|    <span data-ttu-id="1bd58-106">Metódus</span><span class="sxs-lookup"><span data-stu-id="1bd58-106">Method</span></span>    |    <span data-ttu-id="1bd58-107">Kérés URI-ja</span><span class="sxs-lookup"><span data-stu-id="1bd58-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="1bd58-108">PUT</span><span class="sxs-lookup"><span data-stu-id="1bd58-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="1bd58-109">**Kérelemfejléc**</span><span class="sxs-lookup"><span data-stu-id="1bd58-109">**Request header**</span></span>

|    <span data-ttu-id="1bd58-110">Fejléc</span><span class="sxs-lookup"><span data-stu-id="1bd58-110">Header</span></span>    |    <span data-ttu-id="1bd58-111">Típus</span><span class="sxs-lookup"><span data-stu-id="1bd58-111">Type</span></span>    |    <span data-ttu-id="1bd58-112">Leírás</span><span class="sxs-lookup"><span data-stu-id="1bd58-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="1bd58-113">Engedélyezés</span><span class="sxs-lookup"><span data-stu-id="1bd58-113">Authorization</span></span>    |    <span data-ttu-id="1bd58-114">sztring</span><span class="sxs-lookup"><span data-stu-id="1bd58-114">string</span></span>    |    <span data-ttu-id="1bd58-115">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="1bd58-115">Required.</span></span> <span data-ttu-id="1bd58-116">Az Azure Active Directory (AAD) hozzáférési jogkivonat a következő formában:`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="1bd58-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="1bd58-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1bd58-117">Content-Type</span></span>    |    <span data-ttu-id="1bd58-118">sztring</span><span class="sxs-lookup"><span data-stu-id="1bd58-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="1bd58-119">**Elérésiút-paraméter**</span><span class="sxs-lookup"><span data-stu-id="1bd58-119">**Path parameter**</span></span>

|    <span data-ttu-id="1bd58-120">Paraméter neve</span><span class="sxs-lookup"><span data-stu-id="1bd58-120">Parameter Name</span></span>    |    <span data-ttu-id="1bd58-121">Típus</span><span class="sxs-lookup"><span data-stu-id="1bd58-121">Type</span></span>    |    <span data-ttu-id="1bd58-122">Kötelező</span><span class="sxs-lookup"><span data-stu-id="1bd58-122">Required</span></span>    |    <span data-ttu-id="1bd58-123">Leírás</span><span class="sxs-lookup"><span data-stu-id="1bd58-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="1bd58-124">jelentésazonosító</span><span class="sxs-lookup"><span data-stu-id="1bd58-124">reportId</span></span>     |    <span data-ttu-id="1bd58-125">sztring</span><span class="sxs-lookup"><span data-stu-id="1bd58-125">string</span></span>    |    <span data-ttu-id="1bd58-126">No</span><span class="sxs-lookup"><span data-stu-id="1bd58-126">No</span></span>    |    <span data-ttu-id="1bd58-127">A módosított jelentés azonosítója</span><span class="sxs-lookup"><span data-stu-id="1bd58-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="1bd58-128">**Lekérdezési paraméter**</span><span class="sxs-lookup"><span data-stu-id="1bd58-128">**Query parameter**</span></span>

<span data-ttu-id="1bd58-129">None</span><span class="sxs-lookup"><span data-stu-id="1bd58-129">None</span></span>

<span data-ttu-id="1bd58-130">**Hasznos információ kérése**</span><span class="sxs-lookup"><span data-stu-id="1bd58-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="1bd58-131">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="1bd58-131">**Glossary**</span></span>

<span data-ttu-id="1bd58-132">Ez a táblázat a válasz elemeinek kulcsdefinícióit sorolja fel.</span><span class="sxs-lookup"><span data-stu-id="1bd58-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="1bd58-133">Paraméter</span><span class="sxs-lookup"><span data-stu-id="1bd58-133">Parameter</span></span>    |    <span data-ttu-id="1bd58-134">Kötelező</span><span class="sxs-lookup"><span data-stu-id="1bd58-134">Required</span></span>    |    <span data-ttu-id="1bd58-135">Leírás</span><span class="sxs-lookup"><span data-stu-id="1bd58-135">Description</span></span>    |    <span data-ttu-id="1bd58-136">Megengedett értékek</span><span class="sxs-lookup"><span data-stu-id="1bd58-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="1bd58-137">ReportName (Jelentés neve)</span><span class="sxs-lookup"><span data-stu-id="1bd58-137">ReportName</span></span>     |    <span data-ttu-id="1bd58-138">Igen</span><span class="sxs-lookup"><span data-stu-id="1bd58-138">Yes</span></span>     |    <span data-ttu-id="1bd58-139">A jelentéshez hozzárendelni fog név</span><span class="sxs-lookup"><span data-stu-id="1bd58-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="1bd58-140">Sztring</span><span class="sxs-lookup"><span data-stu-id="1bd58-140">String</span></span>     |
|    <span data-ttu-id="1bd58-141">Leírás</span><span class="sxs-lookup"><span data-stu-id="1bd58-141">Description</span></span>     |    <span data-ttu-id="1bd58-142">Nem</span><span class="sxs-lookup"><span data-stu-id="1bd58-142">No</span></span>     |    <span data-ttu-id="1bd58-143">A létrehozott jelentés leírása</span><span class="sxs-lookup"><span data-stu-id="1bd58-143">Description of the created report</span></span>     |    <span data-ttu-id="1bd58-144">Sztring</span><span class="sxs-lookup"><span data-stu-id="1bd58-144">String</span></span>     |
|    <span data-ttu-id="1bd58-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="1bd58-145">StartTime</span></span>     |    <span data-ttu-id="1bd58-146">Igen</span><span class="sxs-lookup"><span data-stu-id="1bd58-146">Yes</span></span>    |    <span data-ttu-id="1bd58-147">Időbélyegző, amely után megkezdődik a jelentés létrehozása</span><span class="sxs-lookup"><span data-stu-id="1bd58-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="1bd58-148">Sztring</span><span class="sxs-lookup"><span data-stu-id="1bd58-148">String</span></span>     |
|    <span data-ttu-id="1bd58-149">RecurrenceInterval (Ismétlődés időköze)</span><span class="sxs-lookup"><span data-stu-id="1bd58-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="1bd58-150">Nem</span><span class="sxs-lookup"><span data-stu-id="1bd58-150">No</span></span>     |    <span data-ttu-id="1bd58-151">A jelentés generálás gyakorisága órákban.</span><span class="sxs-lookup"><span data-stu-id="1bd58-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="1bd58-152">A minimális érték 4</span><span class="sxs-lookup"><span data-stu-id="1bd58-152">Minimum value is 4</span></span>     |    <span data-ttu-id="1bd58-153">Egész szám</span><span class="sxs-lookup"><span data-stu-id="1bd58-153">Integer</span></span>     |
|    <span data-ttu-id="1bd58-154">RecurrenceCount (Ismétlődés száma)</span><span class="sxs-lookup"><span data-stu-id="1bd58-154">RecurrenceCount</span></span>     |    <span data-ttu-id="1bd58-155">Nem</span><span class="sxs-lookup"><span data-stu-id="1bd58-155">No</span></span>     |    <span data-ttu-id="1bd58-156">A létrehozandó jelentés száma.</span><span class="sxs-lookup"><span data-stu-id="1bd58-156">Numbers of report to be generated.</span></span> <span data-ttu-id="1bd58-157">Az alapértelmezett érték a határozatlan.</span><span class="sxs-lookup"><span data-stu-id="1bd58-157">Default is indefinite.</span></span>     |    <span data-ttu-id="1bd58-158">Egész szám</span><span class="sxs-lookup"><span data-stu-id="1bd58-158">Integer</span></span>     |
|    <span data-ttu-id="1bd58-159">Formátum</span><span class="sxs-lookup"><span data-stu-id="1bd58-159">Format</span></span>     |    <span data-ttu-id="1bd58-160">Nem</span><span class="sxs-lookup"><span data-stu-id="1bd58-160">No</span></span>    |    <span data-ttu-id="1bd58-161">Az exportált fájl fájlformátuma.</span><span class="sxs-lookup"><span data-stu-id="1bd58-161">File format of the exported file.</span></span> <span data-ttu-id="1bd58-162">Az alapértelmezett érték CSV</span><span class="sxs-lookup"><span data-stu-id="1bd58-162">Default is CSV</span></span>     |    <span data-ttu-id="1bd58-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="1bd58-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="1bd58-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="1bd58-164">CallbackURL</span></span>     |    <span data-ttu-id="1bd58-165">Nem</span><span class="sxs-lookup"><span data-stu-id="1bd58-165">No</span></span>     |    <span data-ttu-id="1bd58-166">https visszahívási URL-cím, amely a jelentés létrehozása esetén lesz meghívva</span><span class="sxs-lookup"><span data-stu-id="1bd58-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="1bd58-167">Sztring</span><span class="sxs-lookup"><span data-stu-id="1bd58-167">String</span></span>     |
|    <span data-ttu-id="1bd58-168">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="1bd58-168">CallbackMethod</span></span>    |    <span data-ttu-id="1bd58-169">Nem</span><span class="sxs-lookup"><span data-stu-id="1bd58-169">No</span></span>    |    <span data-ttu-id="1bd58-170">A visszahíváshoz használt HTTP-metódus</span><span class="sxs-lookup"><span data-stu-id="1bd58-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="1bd58-171">GET/POST</span><span class="sxs-lookup"><span data-stu-id="1bd58-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="1bd58-172">**Válasz**</span><span class="sxs-lookup"><span data-stu-id="1bd58-172">**Response**</span></span>

<span data-ttu-id="1bd58-173">A válasz hasznos adata a következőképpen strukturálva van:</span><span class="sxs-lookup"><span data-stu-id="1bd58-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="1bd58-174">Válaszkód: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="1bd58-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="1bd58-175">Példa válasz hasznos hasznosra:</span><span class="sxs-lookup"><span data-stu-id="1bd58-175">Response payload example:</span></span>

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
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="1bd58-176">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="1bd58-176">**Glossary**</span></span>

<span data-ttu-id="1bd58-177">Ez a tábla határozza meg a válasz legfontosabb elemeit:</span><span class="sxs-lookup"><span data-stu-id="1bd58-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="1bd58-178">Paraméter</span><span class="sxs-lookup"><span data-stu-id="1bd58-178">Parameter</span></span>    |    <span data-ttu-id="1bd58-179">Leírás</span><span class="sxs-lookup"><span data-stu-id="1bd58-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="1bd58-180">ReportId (Jelentésazonosító)</span><span class="sxs-lookup"><span data-stu-id="1bd58-180">ReportId</span></span>     |    <span data-ttu-id="1bd58-181">A frissített jelentés univerzálisan egyedi azonosítója (UUID)</span><span class="sxs-lookup"><span data-stu-id="1bd58-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="1bd58-182">ReportName (Jelentés neve)</span><span class="sxs-lookup"><span data-stu-id="1bd58-182">ReportName</span></span>     |    <span data-ttu-id="1bd58-183">A jelentésnek a kérelem hasznos információban megadott neve</span><span class="sxs-lookup"><span data-stu-id="1bd58-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="1bd58-184">Leírás</span><span class="sxs-lookup"><span data-stu-id="1bd58-184">Description</span></span>     |    <span data-ttu-id="1bd58-185">A jelentésnek a kérelem hasznos ában megadott leírás</span><span class="sxs-lookup"><span data-stu-id="1bd58-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="1bd58-186">QueryId (Lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="1bd58-186">QueryId</span></span>     |    <span data-ttu-id="1bd58-187">A jelentés létrehozásakor átadott lekérdezésazonosító</span><span class="sxs-lookup"><span data-stu-id="1bd58-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="1bd58-188">Lekérdezés</span><span class="sxs-lookup"><span data-stu-id="1bd58-188">Query</span></span>     |    <span data-ttu-id="1bd58-189">A jelentéshez végrehajtandó szöveg lekérdezése</span><span class="sxs-lookup"><span data-stu-id="1bd58-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="1bd58-190">Felhasználó</span><span class="sxs-lookup"><span data-stu-id="1bd58-190">User</span></span>     |    <span data-ttu-id="1bd58-191">A jelentés létrehozásához használt felhasználói azonosító</span><span class="sxs-lookup"><span data-stu-id="1bd58-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="1bd58-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="1bd58-192">CreatedTime</span></span>     |    <span data-ttu-id="1bd58-193">A jelentés létrehozási ideje.</span><span class="sxs-lookup"><span data-stu-id="1bd58-193">Time the report was created.</span></span> <span data-ttu-id="1bd58-194">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="1bd58-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1bd58-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="1bd58-195">ModifiedTime</span></span>     |    <span data-ttu-id="1bd58-196">A jelentés utolsó módosításának időpontja.</span><span class="sxs-lookup"><span data-stu-id="1bd58-196">Time the report was last modified.</span></span> <span data-ttu-id="1bd58-197">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="1bd58-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1bd58-198">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="1bd58-198">ExecuteNow</span></span>     |    <span data-ttu-id="1bd58-199">A jelentés létrehozásakor beállított ExecuteNow jelző</span><span class="sxs-lookup"><span data-stu-id="1bd58-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="1bd58-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="1bd58-200">StartTime</span></span>     |    <span data-ttu-id="1bd58-201">A jelentés végrehajtásának megkezdésének ideje.</span><span class="sxs-lookup"><span data-stu-id="1bd58-201">Time the report execution will begin.</span></span> <span data-ttu-id="1bd58-202">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="1bd58-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1bd58-203">ReportStatus (Jelentésállapot)</span><span class="sxs-lookup"><span data-stu-id="1bd58-203">ReportStatus</span></span>     |    <span data-ttu-id="1bd58-204">A jelentés végrehajtásának állapota.</span><span class="sxs-lookup"><span data-stu-id="1bd58-204">Status of the report execution.</span></span> <span data-ttu-id="1bd58-205">A lehetséges értékek: Szüneteltetve, Aktív és Inaktív.</span><span class="sxs-lookup"><span data-stu-id="1bd58-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="1bd58-206">RecurrenceInterval (Ismétlődés időköze)</span><span class="sxs-lookup"><span data-stu-id="1bd58-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="1bd58-207">A kérés hasznos adatokban megadott ismétlődési időköz</span><span class="sxs-lookup"><span data-stu-id="1bd58-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="1bd58-208">RecurrenceCount (Ismétlődés száma)</span><span class="sxs-lookup"><span data-stu-id="1bd58-208">RecurrenceCount</span></span>     |    <span data-ttu-id="1bd58-209">A kérelem hasznos adatokban megadott ismétlődési száma</span><span class="sxs-lookup"><span data-stu-id="1bd58-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="1bd58-210">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="1bd58-210">CallbackUrl</span></span>     |    <span data-ttu-id="1bd58-211">A kérésben megadott visszahívási URL-cím</span><span class="sxs-lookup"><span data-stu-id="1bd58-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="1bd58-212">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="1bd58-212">CallbackMethod</span></span>    |    <span data-ttu-id="1bd58-213">A kérésben megadott visszahívási metódus</span><span class="sxs-lookup"><span data-stu-id="1bd58-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="1bd58-214">Formátum</span><span class="sxs-lookup"><span data-stu-id="1bd58-214">Format</span></span>     |    <span data-ttu-id="1bd58-215">A jelentésfájlok formátuma</span><span class="sxs-lookup"><span data-stu-id="1bd58-215">Format of the report files</span></span>     |
|    <span data-ttu-id="1bd58-216">TotalCount (Teljes összeg)</span><span class="sxs-lookup"><span data-stu-id="1bd58-216">TotalCount</span></span>     |    <span data-ttu-id="1bd58-217">Adatkészletek száma az Érték tömbben</span><span class="sxs-lookup"><span data-stu-id="1bd58-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="1bd58-218">Üzenet</span><span class="sxs-lookup"><span data-stu-id="1bd58-218">Message</span></span>     |    <span data-ttu-id="1bd58-219">Állapotüzenet az API végrehajtásából</span><span class="sxs-lookup"><span data-stu-id="1bd58-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="1bd58-220">StatusCode (Állapotkód)</span><span class="sxs-lookup"><span data-stu-id="1bd58-220">StatusCode</span></span>     |    <span data-ttu-id="1bd58-221">Eredménykód.</span><span class="sxs-lookup"><span data-stu-id="1bd58-221">Result Code.</span></span> <span data-ttu-id="1bd58-222">Lehetséges értékek: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="1bd58-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |