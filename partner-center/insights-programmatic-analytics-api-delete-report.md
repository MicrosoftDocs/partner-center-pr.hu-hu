---
title: Jelentési API törlése – Elemzések adatok törlése
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val törölheti a jelentések Partnerközpont elemzéseket.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376758"
---
# <a name="delete-report-api"></a><span data-ttu-id="ba3e4-103">Jelentési API törlése</span><span class="sxs-lookup"><span data-stu-id="ba3e4-103">Delete report API</span></span>

<span data-ttu-id="ba3e4-104">A végrehajtáskor ez az API törli az összes jelentés- és jelentés-végrehajtási rekordot.</span><span class="sxs-lookup"><span data-stu-id="ba3e4-104">On execution, this API deletes all of the report and report execution records.</span></span>

<span data-ttu-id="ba3e4-105">**Kérésszintaxis**</span><span class="sxs-lookup"><span data-stu-id="ba3e4-105">**Request syntax**</span></span>

|    <span data-ttu-id="ba3e4-106">Metódus</span><span class="sxs-lookup"><span data-stu-id="ba3e4-106">Method</span></span>    |    <span data-ttu-id="ba3e4-107">Kérés URI-ja</span><span class="sxs-lookup"><span data-stu-id="ba3e4-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ba3e4-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="ba3e4-108">DELETE</span></span>    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="ba3e4-109">**Kérés fejléce**</span><span class="sxs-lookup"><span data-stu-id="ba3e4-109">**Request header**</span></span>

|    <span data-ttu-id="ba3e4-110">Fejléc</span><span class="sxs-lookup"><span data-stu-id="ba3e4-110">Header</span></span>    |    <span data-ttu-id="ba3e4-111">Típus</span><span class="sxs-lookup"><span data-stu-id="ba3e4-111">Type</span></span>    |    <span data-ttu-id="ba3e4-112">Leírás</span><span class="sxs-lookup"><span data-stu-id="ba3e4-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="ba3e4-113">Engedélyezés</span><span class="sxs-lookup"><span data-stu-id="ba3e4-113">Authorization</span></span>    |    <span data-ttu-id="ba3e4-114">sztring</span><span class="sxs-lookup"><span data-stu-id="ba3e4-114">string</span></span>    |    <span data-ttu-id="ba3e4-115">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="ba3e4-115">Required.</span></span> <span data-ttu-id="ba3e4-116">Az Azure Active Directory (AAD) hozzáférési jogkivonata a következő formában:`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="ba3e4-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="ba3e4-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba3e4-117">Content-Type</span></span>    |    <span data-ttu-id="ba3e4-118">sztring</span><span class="sxs-lookup"><span data-stu-id="ba3e4-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="ba3e4-119">**Elérésiút-paraméter**</span><span class="sxs-lookup"><span data-stu-id="ba3e4-119">**Path parameter**</span></span>

|    <span data-ttu-id="ba3e4-120">Paraméter neve</span><span class="sxs-lookup"><span data-stu-id="ba3e4-120">Parameter Name</span></span>    |    <span data-ttu-id="ba3e4-121">Típus</span><span class="sxs-lookup"><span data-stu-id="ba3e4-121">Type</span></span>    |    <span data-ttu-id="ba3e4-122">Kötelező</span><span class="sxs-lookup"><span data-stu-id="ba3e4-122">Required</span></span>    |    <span data-ttu-id="ba3e4-123">Leírás</span><span class="sxs-lookup"><span data-stu-id="ba3e4-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="ba3e4-124">jelentésazonosító</span><span class="sxs-lookup"><span data-stu-id="ba3e4-124">reportId</span></span>     |    <span data-ttu-id="ba3e4-125">sztring</span><span class="sxs-lookup"><span data-stu-id="ba3e4-125">string</span></span>    |    <span data-ttu-id="ba3e4-126">No</span><span class="sxs-lookup"><span data-stu-id="ba3e4-126">No</span></span>    |    <span data-ttu-id="ba3e4-127">A törölt jelentés azonosítója</span><span class="sxs-lookup"><span data-stu-id="ba3e4-127">ID of the report being deleted</span></span>    |
|        |        |        |        |

<span data-ttu-id="ba3e4-128">**Lekérdezési paraméter**</span><span class="sxs-lookup"><span data-stu-id="ba3e4-128">**Query parameter**</span></span>

<span data-ttu-id="ba3e4-129">None</span><span class="sxs-lookup"><span data-stu-id="ba3e4-129">None</span></span>

<span data-ttu-id="ba3e4-130">**Hasznos információ kérése**</span><span class="sxs-lookup"><span data-stu-id="ba3e4-130">**Request payload**</span></span>

<span data-ttu-id="ba3e4-131">None</span><span class="sxs-lookup"><span data-stu-id="ba3e4-131">None</span></span>

<span data-ttu-id="ba3e4-132">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="ba3e4-132">**Glossary**</span></span>

<span data-ttu-id="ba3e4-133">None</span><span class="sxs-lookup"><span data-stu-id="ba3e4-133">None</span></span>

<span data-ttu-id="ba3e4-134">**Válasz**</span><span class="sxs-lookup"><span data-stu-id="ba3e4-134">**Response**</span></span>

<span data-ttu-id="ba3e4-135">A válasz hasznos adata a következőképpen strukturálva van:</span><span class="sxs-lookup"><span data-stu-id="ba3e4-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="ba3e4-136">Válaszkód: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="ba3e4-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="ba3e4-137">Példa válasz hasznos hasznosra:</span><span class="sxs-lookup"><span data-stu-id="ba3e4-137">Response payload example:</span></span>

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

<span data-ttu-id="ba3e4-138">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="ba3e4-138">**Glossary**</span></span>

<span data-ttu-id="ba3e4-139">Ez a tábla határozza meg a válasz legfontosabb elemeit:</span><span class="sxs-lookup"><span data-stu-id="ba3e4-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="ba3e4-140">Paraméter</span><span class="sxs-lookup"><span data-stu-id="ba3e4-140">Parameter</span></span>    |    <span data-ttu-id="ba3e4-141">Leírás</span><span class="sxs-lookup"><span data-stu-id="ba3e4-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ba3e4-142">Jelentésazonosító</span><span class="sxs-lookup"><span data-stu-id="ba3e4-142">ReportId</span></span>     |    <span data-ttu-id="ba3e4-143">A törölt jelentés univerzálisan egyedi azonosítója (UUID)</span><span class="sxs-lookup"><span data-stu-id="ba3e4-143">Universally unique identifier (UUID) of the deleted report</span></span>     |
|    <span data-ttu-id="ba3e4-144">ReportName (Jelentés neve)</span><span class="sxs-lookup"><span data-stu-id="ba3e4-144">ReportName</span></span>     |    <span data-ttu-id="ba3e4-145">A jelentésnek a létrehozás során megadott név</span><span class="sxs-lookup"><span data-stu-id="ba3e4-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="ba3e4-146">Leírás</span><span class="sxs-lookup"><span data-stu-id="ba3e4-146">Description</span></span>     |    <span data-ttu-id="ba3e4-147">A jelentés létrehozása során megadott leírás</span><span class="sxs-lookup"><span data-stu-id="ba3e4-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="ba3e4-148">QueryId (Lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="ba3e4-148">QueryId</span></span>     |    <span data-ttu-id="ba3e4-149">A jelentés létrehozásakor átadott lekérdezésazonosító</span><span class="sxs-lookup"><span data-stu-id="ba3e4-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="ba3e4-150">Lekérdezés</span><span class="sxs-lookup"><span data-stu-id="ba3e4-150">Query</span></span>     |    <span data-ttu-id="ba3e4-151">A jelentéshez végrehajtandó lekérdezési szöveg</span><span class="sxs-lookup"><span data-stu-id="ba3e4-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="ba3e4-152">Felhasználó</span><span class="sxs-lookup"><span data-stu-id="ba3e4-152">User</span></span>     |    <span data-ttu-id="ba3e4-153">A jelentés létrehozásához használt felhasználói azonosító</span><span class="sxs-lookup"><span data-stu-id="ba3e4-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="ba3e4-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="ba3e4-154">CreatedTime</span></span>     |    <span data-ttu-id="ba3e4-155">A jelentés létrehozási ideje.</span><span class="sxs-lookup"><span data-stu-id="ba3e4-155">Time the report was created.</span></span> <span data-ttu-id="ba3e4-156">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="ba3e4-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ba3e4-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="ba3e4-157">ModifiedTime</span></span>     |    <span data-ttu-id="ba3e4-158">A jelentés utolsó módosításának időpontja.</span><span class="sxs-lookup"><span data-stu-id="ba3e4-158">Time the report was last modified.</span></span> <span data-ttu-id="ba3e4-159">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="ba3e4-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ba3e4-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="ba3e4-160">ExecuteNow</span></span>     |    <span data-ttu-id="ba3e4-161">A jelentés létrehozásakor beállított ExecuteNow jelző</span><span class="sxs-lookup"><span data-stu-id="ba3e4-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="ba3e4-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="ba3e4-162">StartTime</span></span>     |    <span data-ttu-id="ba3e4-163">A jelentés végrehajtásának megkezdésének ideje.</span><span class="sxs-lookup"><span data-stu-id="ba3e4-163">Time the report execution will begin.</span></span> <span data-ttu-id="ba3e4-164">Az időformátum: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="ba3e4-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ba3e4-165">ReportStatus (Jelentésállapot)</span><span class="sxs-lookup"><span data-stu-id="ba3e4-165">ReportStatus</span></span>     |    <span data-ttu-id="ba3e4-166">A jelentés végrehajtásának állapota.</span><span class="sxs-lookup"><span data-stu-id="ba3e4-166">Status of the report execution.</span></span> <span data-ttu-id="ba3e4-167">A lehetséges értékek: Szüneteltetve, Aktív és Inaktív.</span><span class="sxs-lookup"><span data-stu-id="ba3e4-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="ba3e4-168">RecurrenceInterval (Ismétlődés időköze)</span><span class="sxs-lookup"><span data-stu-id="ba3e4-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="ba3e4-169">A jelentés létrehozása során megadott ismétlődési időköz</span><span class="sxs-lookup"><span data-stu-id="ba3e4-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="ba3e4-170">RecurrenceCount (Ismétlődés száma)</span><span class="sxs-lookup"><span data-stu-id="ba3e4-170">RecurrenceCount</span></span>     |    <span data-ttu-id="ba3e4-171">A jelentés létrehozása során megadott ismétlődési szám</span><span class="sxs-lookup"><span data-stu-id="ba3e4-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="ba3e4-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="ba3e4-172">CallbackUrl</span></span>     |    <span data-ttu-id="ba3e4-173">A kérésben megadott visszahívási URL-cím</span><span class="sxs-lookup"><span data-stu-id="ba3e4-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="ba3e4-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="ba3e4-174">CallbackMethod</span></span>    |    <span data-ttu-id="ba3e4-175">A kérésben megadott visszahívási metódus</span><span class="sxs-lookup"><span data-stu-id="ba3e4-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="ba3e4-176">Formátum</span><span class="sxs-lookup"><span data-stu-id="ba3e4-176">Format</span></span>     |    <span data-ttu-id="ba3e4-177">A jelentésfájlok formátuma</span><span class="sxs-lookup"><span data-stu-id="ba3e4-177">Format of the report files</span></span>     |
|    <span data-ttu-id="ba3e4-178">TotalCount (Teljes összeg)</span><span class="sxs-lookup"><span data-stu-id="ba3e4-178">TotalCount</span></span>     |    <span data-ttu-id="ba3e4-179">Adatkészletek száma az Érték tömbben</span><span class="sxs-lookup"><span data-stu-id="ba3e4-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="ba3e4-180">Üzenet</span><span class="sxs-lookup"><span data-stu-id="ba3e4-180">Message</span></span>     |    <span data-ttu-id="ba3e4-181">Állapotüzenet az API végrehajtásából</span><span class="sxs-lookup"><span data-stu-id="ba3e4-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="ba3e4-182">StatusCode (Állapotkód)</span><span class="sxs-lookup"><span data-stu-id="ba3e4-182">StatusCode</span></span>     |    <span data-ttu-id="ba3e4-183">Eredménykód.</span><span class="sxs-lookup"><span data-stu-id="ba3e4-183">Result Code.</span></span> <span data-ttu-id="ba3e4-184">Lehetséges értékek: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="ba3e4-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
