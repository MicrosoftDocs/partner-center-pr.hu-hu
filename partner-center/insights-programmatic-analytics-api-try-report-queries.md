---
title: A jelentéslekérdezések API-jának kipróbálja
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val tesztelheti a lekérdezést, és ellenőrizheti az eredményeket Partnerközpont elemzésekben.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376735"
---
# <a name="try-report-queries-api"></a><span data-ttu-id="018b3-103">A jelentéslekérdezések API-jának kipróbálja</span><span class="sxs-lookup"><span data-stu-id="018b3-103">Try report queries API</span></span>

<span data-ttu-id="018b3-104">Ez az API végrehajt egy Jelentéslekérdezés utasítást.</span><span class="sxs-lookup"><span data-stu-id="018b3-104">This API executes a Report query statement.</span></span> <span data-ttu-id="018b3-105">Az API csak 100 rekordot ad vissza, amelyek segítségével partnerként ellenőrizheti, hogy az adatok a vártnak megfelelőek-e.</span><span class="sxs-lookup"><span data-stu-id="018b3-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="018b3-106">Ez az API 100 másodperces lekérdezés-végrehajtási időtúllépéssel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="018b3-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="018b3-107">Ha azt veszi észre, hogy az API több mint 100 másodpercet vesz igénybe, nagyon valószínű, hogy a lekérdezés szintaktikailag helyes, különben a 200-astól más hibakódot kapott volna.</span><span class="sxs-lookup"><span data-stu-id="018b3-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="018b3-108">A jelentés tényleges létrehozása akkor lesz megfelelő, ha a lekérdezési szintaxis helyes.</span><span class="sxs-lookup"><span data-stu-id="018b3-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="018b3-109">**Kérés szintaxisa**</span><span class="sxs-lookup"><span data-stu-id="018b3-109">**Request syntax**</span></span>

|    <span data-ttu-id="018b3-110">Metódus</span><span class="sxs-lookup"><span data-stu-id="018b3-110">Method</span></span>    |    <span data-ttu-id="018b3-111">Kérés URI-ja</span><span class="sxs-lookup"><span data-stu-id="018b3-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="018b3-112">GET</span><span class="sxs-lookup"><span data-stu-id="018b3-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="018b3-113">**Kérelemfejléc**</span><span class="sxs-lookup"><span data-stu-id="018b3-113">**Request header**</span></span>

|    <span data-ttu-id="018b3-114">Fejléc</span><span class="sxs-lookup"><span data-stu-id="018b3-114">Header</span></span>    |    <span data-ttu-id="018b3-115">Típus</span><span class="sxs-lookup"><span data-stu-id="018b3-115">Type</span></span>    |    <span data-ttu-id="018b3-116">Leírás</span><span class="sxs-lookup"><span data-stu-id="018b3-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="018b3-117">Engedélyezés</span><span class="sxs-lookup"><span data-stu-id="018b3-117">Authorization</span></span>    |    <span data-ttu-id="018b3-118">sztring</span><span class="sxs-lookup"><span data-stu-id="018b3-118">string</span></span>    |    <span data-ttu-id="018b3-119">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="018b3-119">Required.</span></span> <span data-ttu-id="018b3-120">Az Azure Active Directory (AAD) hozzáférési jogkivonat a következő formában:`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="018b3-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="018b3-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="018b3-121">Content-Type</span></span>    |    <span data-ttu-id="018b3-122">sztring</span><span class="sxs-lookup"><span data-stu-id="018b3-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="018b3-123">**Elérésiút-paraméter**</span><span class="sxs-lookup"><span data-stu-id="018b3-123">**Path parameter**</span></span>

<span data-ttu-id="018b3-124">None</span><span class="sxs-lookup"><span data-stu-id="018b3-124">None</span></span>

<span data-ttu-id="018b3-125">**Lekérdezési paraméter**</span><span class="sxs-lookup"><span data-stu-id="018b3-125">**Query parameter**</span></span>

|    <span data-ttu-id="018b3-126">Paraméter neve</span><span class="sxs-lookup"><span data-stu-id="018b3-126">Parameter Name</span></span>    |    <span data-ttu-id="018b3-127">Típus</span><span class="sxs-lookup"><span data-stu-id="018b3-127">Type</span></span>    |    <span data-ttu-id="018b3-128">Kötelező</span><span class="sxs-lookup"><span data-stu-id="018b3-128">Required</span></span>    |    <span data-ttu-id="018b3-129">Leírás</span><span class="sxs-lookup"><span data-stu-id="018b3-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="018b3-130">exportQuery</span><span class="sxs-lookup"><span data-stu-id="018b3-130">exportQuery</span></span>     |    <span data-ttu-id="018b3-131">sztring</span><span class="sxs-lookup"><span data-stu-id="018b3-131">string</span></span>    |    <span data-ttu-id="018b3-132">No</span><span class="sxs-lookup"><span data-stu-id="018b3-132">No</span></span>    |    <span data-ttu-id="018b3-133">Végrehajtandó lekérdezési sztring jelentése</span><span class="sxs-lookup"><span data-stu-id="018b3-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="018b3-134">queryId (lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="018b3-134">queryId</span></span>     |    <span data-ttu-id="018b3-135">sztring</span><span class="sxs-lookup"><span data-stu-id="018b3-135">string</span></span>    |    <span data-ttu-id="018b3-136">No</span><span class="sxs-lookup"><span data-stu-id="018b3-136">No</span></span>    |    <span data-ttu-id="018b3-137">Egy érvényes meglévő lekérdezésazonosító.</span><span class="sxs-lookup"><span data-stu-id="018b3-137">A valid existing query ID.</span></span> <span data-ttu-id="018b3-138">Kölcsönösen kizárják egymást az exportQuery paraméterben megadott lekérdezési sztringekkel</span><span class="sxs-lookup"><span data-stu-id="018b3-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="018b3-139">startTime</span><span class="sxs-lookup"><span data-stu-id="018b3-139">startTime</span></span>     |    <span data-ttu-id="018b3-140">sztring</span><span class="sxs-lookup"><span data-stu-id="018b3-140">string</span></span>    |    <span data-ttu-id="018b3-141">No</span><span class="sxs-lookup"><span data-stu-id="018b3-141">No</span></span>    |    <span data-ttu-id="018b3-142">A kezdési időpont, amelyből az adatokat szeretnénk.</span><span class="sxs-lookup"><span data-stu-id="018b3-142">Start time from which we want the data.</span></span> <span data-ttu-id="018b3-143">Felülbírálja a lekérdezésben megadott időtartamokat</span><span class="sxs-lookup"><span data-stu-id="018b3-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="018b3-144">endTime</span><span class="sxs-lookup"><span data-stu-id="018b3-144">endTime</span></span>     |    <span data-ttu-id="018b3-145">sztring</span><span class="sxs-lookup"><span data-stu-id="018b3-145">string</span></span>    |    <span data-ttu-id="018b3-146">No</span><span class="sxs-lookup"><span data-stu-id="018b3-146">No</span></span>    |    <span data-ttu-id="018b3-147">Az adatok kívánt időszakának vége.</span><span class="sxs-lookup"><span data-stu-id="018b3-147">End time till which we want the data.</span></span> <span data-ttu-id="018b3-148">Felülbírálja a lekérdezésben megadott időtartamokat</span><span class="sxs-lookup"><span data-stu-id="018b3-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="018b3-149">**Hasznos információ kérése**</span><span class="sxs-lookup"><span data-stu-id="018b3-149">**Request payload**</span></span>

<span data-ttu-id="018b3-150">None</span><span class="sxs-lookup"><span data-stu-id="018b3-150">None</span></span>

<span data-ttu-id="018b3-151">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="018b3-151">**Glossary**</span></span>

<span data-ttu-id="018b3-152">None</span><span class="sxs-lookup"><span data-stu-id="018b3-152">None</span></span>

<span data-ttu-id="018b3-153">**Válasz**</span><span class="sxs-lookup"><span data-stu-id="018b3-153">**Response**</span></span>

<span data-ttu-id="018b3-154">A válasz hasznos adata a következőképpen strukturálva van:</span><span class="sxs-lookup"><span data-stu-id="018b3-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="018b3-155">Válaszkód: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="018b3-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="018b3-156">Példa válasz hasznos hasznosra:</span><span class="sxs-lookup"><span data-stu-id="018b3-156">Response payload example:</span></span>

```json
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="018b3-157">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="018b3-157">**Glossary**</span></span>

<span data-ttu-id="018b3-158">Ez a tábla határozza meg a válasz legfontosabb elemeit:</span><span class="sxs-lookup"><span data-stu-id="018b3-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="018b3-159">Paraméter</span><span class="sxs-lookup"><span data-stu-id="018b3-159">Parameter</span></span>    |    <span data-ttu-id="018b3-160">Leírás</span><span class="sxs-lookup"><span data-stu-id="018b3-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="018b3-161">TotalCount (Teljes összeg)</span><span class="sxs-lookup"><span data-stu-id="018b3-161">TotalCount</span></span>     |    <span data-ttu-id="018b3-162">Adatkészletek száma az Érték tömbben</span><span class="sxs-lookup"><span data-stu-id="018b3-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="018b3-163">Üzenet</span><span class="sxs-lookup"><span data-stu-id="018b3-163">Message</span></span>     |    <span data-ttu-id="018b3-164">Állapotüzenet az API végrehajtásából</span><span class="sxs-lookup"><span data-stu-id="018b3-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="018b3-165">StatusCode (Állapotkód)</span><span class="sxs-lookup"><span data-stu-id="018b3-165">StatusCode</span></span>     |    <span data-ttu-id="018b3-166">Eredménykód.</span><span class="sxs-lookup"><span data-stu-id="018b3-166">Result Code.</span></span> <span data-ttu-id="018b3-167">Lehetséges értékek: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="018b3-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
