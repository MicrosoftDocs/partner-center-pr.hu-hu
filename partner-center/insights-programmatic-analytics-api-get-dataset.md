---
title: Az összes adatkészlet API le Elemzések adatok
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val lekérhetők az összes rendelkezésre álló adatkészlet részletei az Partnerközpont elemzésben.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376671"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="30a7d-103">Az összes adat adatkészlet API-jának lekérte</span><span class="sxs-lookup"><span data-stu-id="30a7d-103">Get all datasets API</span></span>

<span data-ttu-id="30a7d-104">A Get all datasets API lekérte az összes rendelkezésre álló adatkészletet.</span><span class="sxs-lookup"><span data-stu-id="30a7d-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="30a7d-105">Az adatkészletek felsorolják a táblákat, oszlopokat, metrikákat és időtartományokat.</span><span class="sxs-lookup"><span data-stu-id="30a7d-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="30a7d-106">**Kérésszintaxis**</span><span class="sxs-lookup"><span data-stu-id="30a7d-106">**Request syntax**</span></span>

|    <span data-ttu-id="30a7d-107">Metódus</span><span class="sxs-lookup"><span data-stu-id="30a7d-107">Method</span></span>    |    <span data-ttu-id="30a7d-108">Kérés URI-ja</span><span class="sxs-lookup"><span data-stu-id="30a7d-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="30a7d-109">GET</span><span class="sxs-lookup"><span data-stu-id="30a7d-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="30a7d-110">**Kérés fejléce**</span><span class="sxs-lookup"><span data-stu-id="30a7d-110">**Request header**</span></span>

|    <span data-ttu-id="30a7d-111">Fejléc</span><span class="sxs-lookup"><span data-stu-id="30a7d-111">Header</span></span>    |    <span data-ttu-id="30a7d-112">Típus</span><span class="sxs-lookup"><span data-stu-id="30a7d-112">Type</span></span>    |    <span data-ttu-id="30a7d-113">Leírás</span><span class="sxs-lookup"><span data-stu-id="30a7d-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="30a7d-114">Engedélyezés</span><span class="sxs-lookup"><span data-stu-id="30a7d-114">Authorization</span></span>    |    <span data-ttu-id="30a7d-115">sztring</span><span class="sxs-lookup"><span data-stu-id="30a7d-115">string</span></span>    |    <span data-ttu-id="30a7d-116">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="30a7d-116">Required.</span></span> <span data-ttu-id="30a7d-117">Az Azure Active Directory (AAD) hozzáférési jogkivonata a következő formában:`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="30a7d-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="30a7d-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30a7d-118">Content-Type</span></span>    |    <span data-ttu-id="30a7d-119">sztring</span><span class="sxs-lookup"><span data-stu-id="30a7d-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="30a7d-120">**Elérésiút-paraméter**</span><span class="sxs-lookup"><span data-stu-id="30a7d-120">**Path parameter**</span></span>

<span data-ttu-id="30a7d-121">None</span><span class="sxs-lookup"><span data-stu-id="30a7d-121">None</span></span>

<span data-ttu-id="30a7d-122">**Lekérdezési paraméter**</span><span class="sxs-lookup"><span data-stu-id="30a7d-122">**Query parameter**</span></span>

|    <span data-ttu-id="30a7d-123">Paraméter neve</span><span class="sxs-lookup"><span data-stu-id="30a7d-123">Parameter Name</span></span>    |    <span data-ttu-id="30a7d-124">Típus</span><span class="sxs-lookup"><span data-stu-id="30a7d-124">Type</span></span>    |    <span data-ttu-id="30a7d-125">Kötelező</span><span class="sxs-lookup"><span data-stu-id="30a7d-125">Required</span></span>    |    <span data-ttu-id="30a7d-126">Leírás</span><span class="sxs-lookup"><span data-stu-id="30a7d-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="30a7d-127">datasetName (adatkészlet neve)</span><span class="sxs-lookup"><span data-stu-id="30a7d-127">datasetName</span></span>    |    <span data-ttu-id="30a7d-128">sztring</span><span class="sxs-lookup"><span data-stu-id="30a7d-128">string</span></span>    |    <span data-ttu-id="30a7d-129">No</span><span class="sxs-lookup"><span data-stu-id="30a7d-129">No</span></span>    |    <span data-ttu-id="30a7d-130">Szűrés egyetlen adatkészlet részleteinek lekért érdekében</span><span class="sxs-lookup"><span data-stu-id="30a7d-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="30a7d-131">**Hasznos információ kérése**</span><span class="sxs-lookup"><span data-stu-id="30a7d-131">**Request payload**</span></span>

<span data-ttu-id="30a7d-132">None</span><span class="sxs-lookup"><span data-stu-id="30a7d-132">None</span></span>

<span data-ttu-id="30a7d-133">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="30a7d-133">**Glossary**</span></span>

<span data-ttu-id="30a7d-134">None</span><span class="sxs-lookup"><span data-stu-id="30a7d-134">None</span></span>

<span data-ttu-id="30a7d-135">**Válasz**</span><span class="sxs-lookup"><span data-stu-id="30a7d-135">**Response**</span></span>

<span data-ttu-id="30a7d-136">A válasz hasznos adata a következőképpen strukturálva van:</span><span class="sxs-lookup"><span data-stu-id="30a7d-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="30a7d-137">Válaszkód: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="30a7d-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="30a7d-138">Példa válasz hasznos hasznosra:</span><span class="sxs-lookup"><span data-stu-id="30a7d-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="30a7d-139">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="30a7d-139">**Glossary**</span></span>

<span data-ttu-id="30a7d-140">Ez a tábla határozza meg a válasz legfontosabb elemeit:</span><span class="sxs-lookup"><span data-stu-id="30a7d-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="30a7d-141">Paraméter</span><span class="sxs-lookup"><span data-stu-id="30a7d-141">Parameter</span></span>    |    <span data-ttu-id="30a7d-142">Leírás</span><span class="sxs-lookup"><span data-stu-id="30a7d-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="30a7d-143">DatasetName (Adatkészlet neve)</span><span class="sxs-lookup"><span data-stu-id="30a7d-143">DatasetName</span></span>     |    <span data-ttu-id="30a7d-144">A tömbobjektum által definiált adatkészlet neve</span><span class="sxs-lookup"><span data-stu-id="30a7d-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="30a7d-145">SelectableColumns (Kiválaszthatóoszlopok)</span><span class="sxs-lookup"><span data-stu-id="30a7d-145">SelectableColumns</span></span>     |    <span data-ttu-id="30a7d-146">A kiválasztott oszlopokban megadva nyers oszlopok</span><span class="sxs-lookup"><span data-stu-id="30a7d-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="30a7d-147">Elérhetőmetriák</span><span class="sxs-lookup"><span data-stu-id="30a7d-147">AvailableMetrics</span></span>     |    <span data-ttu-id="30a7d-148">A kiválasztott oszlopokban megadva az aggregáció/metrika oszlopneveket</span><span class="sxs-lookup"><span data-stu-id="30a7d-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="30a7d-149">AvailableDateRanges (ElérhetőDateRanges)</span><span class="sxs-lookup"><span data-stu-id="30a7d-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="30a7d-150">Az adatkészlet jelentéslekérdezésekben használható dátumtartomány</span><span class="sxs-lookup"><span data-stu-id="30a7d-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="30a7d-151">minimumRecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="30a7d-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="30a7d-152">Az Ismétlődési időköz minimális értéke</span><span class="sxs-lookup"><span data-stu-id="30a7d-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="30a7d-153">TotalCount (Teljes összeg)</span><span class="sxs-lookup"><span data-stu-id="30a7d-153">TotalCount</span></span>     |    <span data-ttu-id="30a7d-154">Adatkészletek száma az Érték tömbben</span><span class="sxs-lookup"><span data-stu-id="30a7d-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="30a7d-155">Üzenet</span><span class="sxs-lookup"><span data-stu-id="30a7d-155">Message</span></span>     |    <span data-ttu-id="30a7d-156">Állapotüzenet az API végrehajtásából</span><span class="sxs-lookup"><span data-stu-id="30a7d-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="30a7d-157">StatusCode (Állapotkód)</span><span class="sxs-lookup"><span data-stu-id="30a7d-157">StatusCode</span></span>     |    <span data-ttu-id="30a7d-158">Eredménykód.</span><span class="sxs-lookup"><span data-stu-id="30a7d-158">Result Code.</span></span> <span data-ttu-id="30a7d-159">Lehetséges értékek: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="30a7d-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
