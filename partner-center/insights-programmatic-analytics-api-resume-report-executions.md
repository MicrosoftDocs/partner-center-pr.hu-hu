---
title: Jelentés-végrehajtási API folytatása – Elemzések adatok
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val folytathatja a szüneteltetett jelentések végrehajtását az Partnerközpont elemzésben.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1372823425f3aefd025ffc3441623c1ceee34e1e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376743"
---
# <a name="resume-report-executions-api"></a><span data-ttu-id="8c7b2-103">Jelentés-végrehajtási API folytatása</span><span class="sxs-lookup"><span data-stu-id="8c7b2-103">Resume report executions API</span></span>

<span data-ttu-id="8c7b2-104">Végrehajtáskor ez az API folytatja egy szüneteltetett jelentés ütemezett végrehajtását.</span><span class="sxs-lookup"><span data-stu-id="8c7b2-104">On execution, this API resumes the scheduled execution of a paused report.</span></span>

<span data-ttu-id="8c7b2-105">**Kérésszintaxis**</span><span class="sxs-lookup"><span data-stu-id="8c7b2-105">**Request syntax**</span></span>

|    <span data-ttu-id="8c7b2-106">Metódus</span><span class="sxs-lookup"><span data-stu-id="8c7b2-106">Method</span></span>    |    <span data-ttu-id="8c7b2-107">Kérés URI-ja</span><span class="sxs-lookup"><span data-stu-id="8c7b2-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="8c7b2-108">PUT</span><span class="sxs-lookup"><span data-stu-id="8c7b2-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

<span data-ttu-id="8c7b2-109">**Kérés fejléce**</span><span class="sxs-lookup"><span data-stu-id="8c7b2-109">**Request header**</span></span>

|    <span data-ttu-id="8c7b2-110">Fejléc</span><span class="sxs-lookup"><span data-stu-id="8c7b2-110">Header</span></span>    |    <span data-ttu-id="8c7b2-111">Típus</span><span class="sxs-lookup"><span data-stu-id="8c7b2-111">Type</span></span>    |    <span data-ttu-id="8c7b2-112">Leírás</span><span class="sxs-lookup"><span data-stu-id="8c7b2-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="8c7b2-113">Engedélyezés</span><span class="sxs-lookup"><span data-stu-id="8c7b2-113">Authorization</span></span>    |    <span data-ttu-id="8c7b2-114">sztring</span><span class="sxs-lookup"><span data-stu-id="8c7b2-114">string</span></span>    |    <span data-ttu-id="8c7b2-115">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="8c7b2-115">Required.</span></span> <span data-ttu-id="8c7b2-116">Az Azure Active Directory (AAD) hozzáférési jogkivonata a következő formában:`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="8c7b2-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="8c7b2-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c7b2-117">Content-Type</span></span>    |    <span data-ttu-id="8c7b2-118">sztring</span><span class="sxs-lookup"><span data-stu-id="8c7b2-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="8c7b2-119">**Elérésiút-paraméter**</span><span class="sxs-lookup"><span data-stu-id="8c7b2-119">**Path parameter**</span></span>

|    <span data-ttu-id="8c7b2-120">Paraméter neve</span><span class="sxs-lookup"><span data-stu-id="8c7b2-120">Parameter Name</span></span>    |    <span data-ttu-id="8c7b2-121">Típus</span><span class="sxs-lookup"><span data-stu-id="8c7b2-121">Type</span></span>    |    <span data-ttu-id="8c7b2-122">Kötelező</span><span class="sxs-lookup"><span data-stu-id="8c7b2-122">Required</span></span>    |    <span data-ttu-id="8c7b2-123">Leírás</span><span class="sxs-lookup"><span data-stu-id="8c7b2-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="8c7b2-124">jelentésazonosító</span><span class="sxs-lookup"><span data-stu-id="8c7b2-124">reportId</span></span>     |    <span data-ttu-id="8c7b2-125">sztring</span><span class="sxs-lookup"><span data-stu-id="8c7b2-125">string</span></span>    |    <span data-ttu-id="8c7b2-126">No</span><span class="sxs-lookup"><span data-stu-id="8c7b2-126">No</span></span>    |    <span data-ttu-id="8c7b2-127">A módosított jelentés azonosítója</span><span class="sxs-lookup"><span data-stu-id="8c7b2-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="8c7b2-128">**Lekérdezési paraméter**</span><span class="sxs-lookup"><span data-stu-id="8c7b2-128">**Query parameter**</span></span>

<span data-ttu-id="8c7b2-129">None</span><span class="sxs-lookup"><span data-stu-id="8c7b2-129">None</span></span>

<span data-ttu-id="8c7b2-130">**Hasznos információ kérése**</span><span class="sxs-lookup"><span data-stu-id="8c7b2-130">**Request payload**</span></span>

<span data-ttu-id="8c7b2-131">None</span><span class="sxs-lookup"><span data-stu-id="8c7b2-131">None</span></span>

<span data-ttu-id="8c7b2-132">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="8c7b2-132">**Glossary**</span></span>

<span data-ttu-id="8c7b2-133">None</span><span class="sxs-lookup"><span data-stu-id="8c7b2-133">None</span></span>

<span data-ttu-id="8c7b2-134">**Válasz**</span><span class="sxs-lookup"><span data-stu-id="8c7b2-134">**Response**</span></span>

<span data-ttu-id="8c7b2-135">A válasz hasznos adata a következőképpen strukturálva van:</span><span class="sxs-lookup"><span data-stu-id="8c7b2-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="8c7b2-136">Válaszkód: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="8c7b2-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="8c7b2-137">Példa válasz hasznos hasznosra:</span><span class="sxs-lookup"><span data-stu-id="8c7b2-137">Response payload example:</span></span>

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

<span data-ttu-id="8c7b2-138">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="8c7b2-138">**Glossary**</span></span>

<span data-ttu-id="8c7b2-139">Ez a tábla határozza meg a válasz legfontosabb elemeit:</span><span class="sxs-lookup"><span data-stu-id="8c7b2-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="8c7b2-140">Paraméter</span><span class="sxs-lookup"><span data-stu-id="8c7b2-140">Parameter</span></span>    |    <span data-ttu-id="8c7b2-141">Leírás</span><span class="sxs-lookup"><span data-stu-id="8c7b2-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="8c7b2-142">Jelentésazonosító</span><span class="sxs-lookup"><span data-stu-id="8c7b2-142">ReportId</span></span>     |    <span data-ttu-id="8c7b2-143">A folytatott jelentés univerzálisan egyedi azonosítója (UUID)</span><span class="sxs-lookup"><span data-stu-id="8c7b2-143">Universally unique identifier (UUID) of the resumed report</span></span>     |
|    <span data-ttu-id="8c7b2-144">ReportName (Jelentés neve)</span><span class="sxs-lookup"><span data-stu-id="8c7b2-144">ReportName</span></span>     |    <span data-ttu-id="8c7b2-145">A jelentésnek a létrehozás során megadott név</span><span class="sxs-lookup"><span data-stu-id="8c7b2-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="8c7b2-146">Leírás</span><span class="sxs-lookup"><span data-stu-id="8c7b2-146">Description</span></span>     |    <span data-ttu-id="8c7b2-147">A jelentés létrehozása során megadott leírás</span><span class="sxs-lookup"><span data-stu-id="8c7b2-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="8c7b2-148">QueryId (Lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="8c7b2-148">QueryId</span></span>     |    <span data-ttu-id="8c7b2-149">A jelentés létrehozásakor átadott lekérdezésazonosító</span><span class="sxs-lookup"><span data-stu-id="8c7b2-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="8c7b2-150">Lekérdezés</span><span class="sxs-lookup"><span data-stu-id="8c7b2-150">Query</span></span>     |    <span data-ttu-id="8c7b2-151">A jelentéshez végrehajtandó lekérdezési szöveg</span><span class="sxs-lookup"><span data-stu-id="8c7b2-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="8c7b2-152">Felhasználó</span><span class="sxs-lookup"><span data-stu-id="8c7b2-152">User</span></span>     |    <span data-ttu-id="8c7b2-153">A jelentés létrehozásához használt felhasználói azonosító</span><span class="sxs-lookup"><span data-stu-id="8c7b2-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="8c7b2-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="8c7b2-154">CreatedTime</span></span>     |    <span data-ttu-id="8c7b2-155">A jelentés létrehozási ideje.</span><span class="sxs-lookup"><span data-stu-id="8c7b2-155">Time the report was created.</span></span> <span data-ttu-id="8c7b2-156">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="8c7b2-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="8c7b2-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="8c7b2-157">ModifiedTime</span></span>     |    <span data-ttu-id="8c7b2-158">A jelentés utolsó módosításának időpontja.</span><span class="sxs-lookup"><span data-stu-id="8c7b2-158">Time the report was last modified.</span></span> <span data-ttu-id="8c7b2-159">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="8c7b2-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="8c7b2-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="8c7b2-160">ExecuteNow</span></span>     |    <span data-ttu-id="8c7b2-161">A jelentés létrehozásakor beállított ExecuteNow jelző</span><span class="sxs-lookup"><span data-stu-id="8c7b2-161">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="8c7b2-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="8c7b2-162">StartTime</span></span>     |    <span data-ttu-id="8c7b2-163">A jelentés végrehajtásának megkezdésének ideje.</span><span class="sxs-lookup"><span data-stu-id="8c7b2-163">Time the report execution will begin.</span></span> <span data-ttu-id="8c7b2-164">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="8c7b2-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="8c7b2-165">ReportStatus (Jelentésállapot)</span><span class="sxs-lookup"><span data-stu-id="8c7b2-165">ReportStatus</span></span>     |    <span data-ttu-id="8c7b2-166">A jelentés végrehajtásának állapota.</span><span class="sxs-lookup"><span data-stu-id="8c7b2-166">Status of the report execution.</span></span> <span data-ttu-id="8c7b2-167">A lehetséges értékek: Szüneteltetve, Aktív és Inaktív.</span><span class="sxs-lookup"><span data-stu-id="8c7b2-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="8c7b2-168">RecurrenceInterval (Ismétlődés időköze)</span><span class="sxs-lookup"><span data-stu-id="8c7b2-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="8c7b2-169">A jelentés létrehozása során megadott ismétlődési időköz</span><span class="sxs-lookup"><span data-stu-id="8c7b2-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="8c7b2-170">RecurrenceCount (Ismétlődés száma)</span><span class="sxs-lookup"><span data-stu-id="8c7b2-170">RecurrenceCount</span></span>     |    <span data-ttu-id="8c7b2-171">A jelentés létrehozása során megadott ismétlődési szám</span><span class="sxs-lookup"><span data-stu-id="8c7b2-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="8c7b2-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="8c7b2-172">CallbackUrl</span></span>     |    <span data-ttu-id="8c7b2-173">A kérésben megadott visszahívási URL-cím</span><span class="sxs-lookup"><span data-stu-id="8c7b2-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="8c7b2-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="8c7b2-174">CallbackMethod</span></span>    |    <span data-ttu-id="8c7b2-175">A kérésben megadott visszahívási metódus</span><span class="sxs-lookup"><span data-stu-id="8c7b2-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="8c7b2-176">Formátum</span><span class="sxs-lookup"><span data-stu-id="8c7b2-176">Format</span></span>     |    <span data-ttu-id="8c7b2-177">A jelentésfájlok formátuma</span><span class="sxs-lookup"><span data-stu-id="8c7b2-177">Format of the report files</span></span>     |
|    <span data-ttu-id="8c7b2-178">TotalCount (Teljes összeg)</span><span class="sxs-lookup"><span data-stu-id="8c7b2-178">TotalCount</span></span>     |    <span data-ttu-id="8c7b2-179">Adatkészletek száma az Érték tömbben</span><span class="sxs-lookup"><span data-stu-id="8c7b2-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="8c7b2-180">Üzenet</span><span class="sxs-lookup"><span data-stu-id="8c7b2-180">Message</span></span>     |    <span data-ttu-id="8c7b2-181">Állapotüzenet az API végrehajtásából</span><span class="sxs-lookup"><span data-stu-id="8c7b2-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="8c7b2-182">StatusCode (Állapotkód)</span><span class="sxs-lookup"><span data-stu-id="8c7b2-182">StatusCode</span></span>     |    <span data-ttu-id="8c7b2-183">Eredménykód.</span><span class="sxs-lookup"><span data-stu-id="8c7b2-183">Result Code.</span></span> <span data-ttu-id="8c7b2-184">Lehetséges értékek: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="8c7b2-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
