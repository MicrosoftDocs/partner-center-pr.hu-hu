---
title: Jelentéslekérdezések törlése API – Elemzések adatok
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val törölheti a felhasználó által megadott lekérdezéseket Partnerközpont elemzésekben.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376676"
---
# <a name="delete-report-queries-api"></a><span data-ttu-id="21a6b-103">Jelentéslekérdezések törlése API</span><span class="sxs-lookup"><span data-stu-id="21a6b-103">Delete report queries API</span></span>

<span data-ttu-id="21a6b-104">Ez az API törli a felhasználó által megadott lekérdezéseket.</span><span class="sxs-lookup"><span data-stu-id="21a6b-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="21a6b-105">**Kérés szintaxisa**</span><span class="sxs-lookup"><span data-stu-id="21a6b-105">**Request syntax**</span></span>

|    <span data-ttu-id="21a6b-106">Metódus</span><span class="sxs-lookup"><span data-stu-id="21a6b-106">Method</span></span>    |    <span data-ttu-id="21a6b-107">Kérés URI-ja</span><span class="sxs-lookup"><span data-stu-id="21a6b-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="21a6b-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="21a6b-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="21a6b-109">**Kérelemfejléc**</span><span class="sxs-lookup"><span data-stu-id="21a6b-109">**Request header**</span></span>

|    <span data-ttu-id="21a6b-110">Fejléc</span><span class="sxs-lookup"><span data-stu-id="21a6b-110">Header</span></span>    |    <span data-ttu-id="21a6b-111">Típus</span><span class="sxs-lookup"><span data-stu-id="21a6b-111">Type</span></span>    |    <span data-ttu-id="21a6b-112">Leírás</span><span class="sxs-lookup"><span data-stu-id="21a6b-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="21a6b-113">Engedélyezés</span><span class="sxs-lookup"><span data-stu-id="21a6b-113">Authorization</span></span>    |    <span data-ttu-id="21a6b-114">sztring</span><span class="sxs-lookup"><span data-stu-id="21a6b-114">string</span></span>    |    <span data-ttu-id="21a6b-115">Kötelező.</span><span class="sxs-lookup"><span data-stu-id="21a6b-115">Required.</span></span> <span data-ttu-id="21a6b-116">Az Azure Active Directory (AAD) hozzáférési jogkivonat a következő formában:`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="21a6b-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="21a6b-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21a6b-117">Content-Type</span></span>    |    <span data-ttu-id="21a6b-118">sztring</span><span class="sxs-lookup"><span data-stu-id="21a6b-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="21a6b-119">**Elérésiút-paraméter**</span><span class="sxs-lookup"><span data-stu-id="21a6b-119">**Path parameter**</span></span>

|    <span data-ttu-id="21a6b-120">Paraméter neve</span><span class="sxs-lookup"><span data-stu-id="21a6b-120">Parameter Name</span></span>    |    <span data-ttu-id="21a6b-121">Típus</span><span class="sxs-lookup"><span data-stu-id="21a6b-121">Type</span></span>    |    <span data-ttu-id="21a6b-122">Kötelező</span><span class="sxs-lookup"><span data-stu-id="21a6b-122">Required</span></span>    |    <span data-ttu-id="21a6b-123">Leírás</span><span class="sxs-lookup"><span data-stu-id="21a6b-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="21a6b-124">queryId (lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="21a6b-124">queryId</span></span>     |    <span data-ttu-id="21a6b-125">sztring</span><span class="sxs-lookup"><span data-stu-id="21a6b-125">string</span></span>     |    <span data-ttu-id="21a6b-126">No</span><span class="sxs-lookup"><span data-stu-id="21a6b-126">No</span></span>    |    <span data-ttu-id="21a6b-127">Szűrhet, hogy csak a argumentumban megadott azonosítóval megadott lekérdezések adatait lekérdezze</span><span class="sxs-lookup"><span data-stu-id="21a6b-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="21a6b-128">**Lekérdezési paraméter**</span><span class="sxs-lookup"><span data-stu-id="21a6b-128">**Query parameter**</span></span>

<span data-ttu-id="21a6b-129">None</span><span class="sxs-lookup"><span data-stu-id="21a6b-129">None</span></span>

<span data-ttu-id="21a6b-130">**Hasznos információ kérése**</span><span class="sxs-lookup"><span data-stu-id="21a6b-130">**Request payload**</span></span>

<span data-ttu-id="21a6b-131">None</span><span class="sxs-lookup"><span data-stu-id="21a6b-131">None</span></span>

<span data-ttu-id="21a6b-132">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="21a6b-132">**Glossary**</span></span>

<span data-ttu-id="21a6b-133">None</span><span class="sxs-lookup"><span data-stu-id="21a6b-133">None</span></span>

<span data-ttu-id="21a6b-134">**Válasz**</span><span class="sxs-lookup"><span data-stu-id="21a6b-134">**Response**</span></span>

<span data-ttu-id="21a6b-135">A válasz hasznos adata a következőképpen strukturálva van:</span><span class="sxs-lookup"><span data-stu-id="21a6b-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="21a6b-136">Válaszkód: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="21a6b-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="21a6b-137">Példa válasz hasznos hasznosra:</span><span class="sxs-lookup"><span data-stu-id="21a6b-137">Response payload example:</span></span>

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

<span data-ttu-id="21a6b-138">**Szószedet**</span><span class="sxs-lookup"><span data-stu-id="21a6b-138">**Glossary**</span></span>

<span data-ttu-id="21a6b-139">Ez a tábla határozza meg a válasz legfontosabb elemeit:</span><span class="sxs-lookup"><span data-stu-id="21a6b-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="21a6b-140">Paraméter</span><span class="sxs-lookup"><span data-stu-id="21a6b-140">Parameter</span></span>    |    <span data-ttu-id="21a6b-141">Leírás</span><span class="sxs-lookup"><span data-stu-id="21a6b-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="21a6b-142">QueryId (Lekérdezésazonosító)</span><span class="sxs-lookup"><span data-stu-id="21a6b-142">QueryId</span></span>     |    <span data-ttu-id="21a6b-143">A törölt lekérdezés egyedi UUID-je</span><span class="sxs-lookup"><span data-stu-id="21a6b-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="21a6b-144">Name</span><span class="sxs-lookup"><span data-stu-id="21a6b-144">Name</span></span>     |    <span data-ttu-id="21a6b-145">A törölt lekérdezés neve</span><span class="sxs-lookup"><span data-stu-id="21a6b-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="21a6b-146">Leírás</span><span class="sxs-lookup"><span data-stu-id="21a6b-146">Description</span></span>     |    <span data-ttu-id="21a6b-147">A törölt lekérdezés leírása</span><span class="sxs-lookup"><span data-stu-id="21a6b-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="21a6b-148">Lekérdezés</span><span class="sxs-lookup"><span data-stu-id="21a6b-148">Query</span></span>     |    <span data-ttu-id="21a6b-149">A törölt lekérdezés lekérdezési sztringének jelentése</span><span class="sxs-lookup"><span data-stu-id="21a6b-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="21a6b-150">Típus</span><span class="sxs-lookup"><span data-stu-id="21a6b-150">Type</span></span>     |    <span data-ttu-id="21a6b-151">A felhasználó által létrehozott lekérdezésekhez a userDefined (felhasználó által definiált) beállítás van megállítva</span><span class="sxs-lookup"><span data-stu-id="21a6b-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="21a6b-152">Felhasználó</span><span class="sxs-lookup"><span data-stu-id="21a6b-152">User</span></span>     |    <span data-ttu-id="21a6b-153">A lekérdezést létrehozó felhasználói azonosító</span><span class="sxs-lookup"><span data-stu-id="21a6b-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="21a6b-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="21a6b-154">CreatedTime</span></span>     |    <span data-ttu-id="21a6b-155">A lekérdezés létrehozásának ideje</span><span class="sxs-lookup"><span data-stu-id="21a6b-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="21a6b-156">TotalCount (Teljes összeg)</span><span class="sxs-lookup"><span data-stu-id="21a6b-156">TotalCount</span></span>     |    <span data-ttu-id="21a6b-157">Adatkészletek száma az Érték tömbben</span><span class="sxs-lookup"><span data-stu-id="21a6b-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="21a6b-158">Üzenet</span><span class="sxs-lookup"><span data-stu-id="21a6b-158">Message</span></span>     |    <span data-ttu-id="21a6b-159">Állapotüzenet az API végrehajtásából</span><span class="sxs-lookup"><span data-stu-id="21a6b-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="21a6b-160">StatusCode (Állapotkód)</span><span class="sxs-lookup"><span data-stu-id="21a6b-160">StatusCode</span></span>     |    <span data-ttu-id="21a6b-161">Eredménykód.</span><span class="sxs-lookup"><span data-stu-id="21a6b-161">Result Code.</span></span> <span data-ttu-id="21a6b-162">Lehetséges értékek: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="21a6b-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
