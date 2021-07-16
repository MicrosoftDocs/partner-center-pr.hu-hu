---
title: Api-k listája a partnerelemzési adatok eléréséhez
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A partnerelemzési adatok eléréséhez szükséges API-k listája.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376731"
---
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="67b64-103">Elérhető API-k a partnerelemzéshez</span><span class="sxs-lookup"><span data-stu-id="67b64-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="67b64-104">Az alábbiakban a partnerelemzési API-k és a hozzájuk tartozó funkciók listája található.</span><span class="sxs-lookup"><span data-stu-id="67b64-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="67b64-105">Adatkészlet-lekért API-k</span><span class="sxs-lookup"><span data-stu-id="67b64-105">Dataset pull APIs</span></span>

<span data-ttu-id="67b64-106">***1. táblázat: Adatkészlet lekért API-k***</span><span class="sxs-lookup"><span data-stu-id="67b64-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="67b64-107">**API**</span><span class="sxs-lookup"><span data-stu-id="67b64-107">**API**</span></span> | <span data-ttu-id="67b64-108">**Funkció**</span><span class="sxs-lookup"><span data-stu-id="67b64-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="67b64-109">Az összes adatkészlet lekérte</span><span class="sxs-lookup"><span data-stu-id="67b64-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="67b64-110">Lekérhetők az összes elérhető adatkészlet.</span><span class="sxs-lookup"><span data-stu-id="67b64-110">Gets all the available datasets.</span></span> <span data-ttu-id="67b64-111">Az adatkészletek felsorolják a táblákat, oszlopokat, metrikákat és időtartományokat.</span><span class="sxs-lookup"><span data-stu-id="67b64-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="67b64-112">Lekérdezéskezelési API-k</span><span class="sxs-lookup"><span data-stu-id="67b64-112">Query management APIs</span></span>

<span data-ttu-id="67b64-113">***2. táblázat: Lekérdezéskezelési API-k***</span><span class="sxs-lookup"><span data-stu-id="67b64-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="67b64-114">**API**</span><span class="sxs-lookup"><span data-stu-id="67b64-114">**API**</span></span> | <span data-ttu-id="67b64-115">**Funkció**</span><span class="sxs-lookup"><span data-stu-id="67b64-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="67b64-116">Jelentéslekérdezés létrehozása</span><span class="sxs-lookup"><span data-stu-id="67b64-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="67b64-117">Egyéni lekérdezéseket hoz létre, amelyek meghatározzák azt az adatkészletet, amelyből exportálni kell az oszlopokat és metrikákat.</span><span class="sxs-lookup"><span data-stu-id="67b64-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="67b64-118">GET Jelentéslekérdezés</span><span class="sxs-lookup"><span data-stu-id="67b64-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="67b64-119">Lekérdezi a jelentésekben használható összes lekérdezést.</span><span class="sxs-lookup"><span data-stu-id="67b64-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="67b64-120">Alapértelmezés szerint lekérdezi a rendszer és a felhasználó által megadott összes lekérdezést.</span><span class="sxs-lookup"><span data-stu-id="67b64-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="67b64-121">DELETE Report Query</span><span class="sxs-lookup"><span data-stu-id="67b64-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="67b64-122">Törli a felhasználó által megadott lekérdezéseket.</span><span class="sxs-lookup"><span data-stu-id="67b64-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="67b64-123">Jelentéskezelési API-k</span><span class="sxs-lookup"><span data-stu-id="67b64-123">Report management APIs</span></span>

<span data-ttu-id="67b64-124">***3. táblázat: Jelentéskezelési API-k***</span><span class="sxs-lookup"><span data-stu-id="67b64-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="67b64-125">**API**</span><span class="sxs-lookup"><span data-stu-id="67b64-125">**API**</span></span> | <span data-ttu-id="67b64-126">**Funkció**</span><span class="sxs-lookup"><span data-stu-id="67b64-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="67b64-127">Jelentés létrehozása</span><span class="sxs-lookup"><span data-stu-id="67b64-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="67b64-128">Rendszeres időközönként végrehajtandó lekérdezést ütemez.</span><span class="sxs-lookup"><span data-stu-id="67b64-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="67b64-129">TRY Report Query</span><span class="sxs-lookup"><span data-stu-id="67b64-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="67b64-130">Végrehajt egy jelentéslekérdezés-utasítást.</span><span class="sxs-lookup"><span data-stu-id="67b64-130">Executes a Report query statement.</span></span> <span data-ttu-id="67b64-131">Csak 10 rekordot ad vissza, amelyek használatával a partner ellenőrizheti, hogy az adatok a vártnak megfelelőek-e.</span><span class="sxs-lookup"><span data-stu-id="67b64-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="67b64-132">Jelentés lekérése</span><span class="sxs-lookup"><span data-stu-id="67b64-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="67b64-133">Szerezze be az összes ütemezett jelentést.</span><span class="sxs-lookup"><span data-stu-id="67b64-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="67b64-134">Jelentés frissítése</span><span class="sxs-lookup"><span data-stu-id="67b64-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="67b64-135">Jelentésparaméter módosítása.</span><span class="sxs-lookup"><span data-stu-id="67b64-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="67b64-136">Jelentés törlése</span><span class="sxs-lookup"><span data-stu-id="67b64-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="67b64-137">Törli az összes jelentés- és jelentés-végrehajtási rekordot.</span><span class="sxs-lookup"><span data-stu-id="67b64-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="67b64-138">Jelentés-végrehajtások szüneteltetése</span><span class="sxs-lookup"><span data-stu-id="67b64-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="67b64-139">Szünetelteti a jelentések ütemezett végrehajtását.</span><span class="sxs-lookup"><span data-stu-id="67b64-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="67b64-140">Jelentés-végrehajtások folytatása</span><span class="sxs-lookup"><span data-stu-id="67b64-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="67b64-141">Folytatja egy szüneteltetett jelentés ütemezett végrehajtását.</span><span class="sxs-lookup"><span data-stu-id="67b64-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="67b64-142">Jelentés-végrehajtási lekért API-k</span><span class="sxs-lookup"><span data-stu-id="67b64-142">Report execution pull APIs</span></span>

<span data-ttu-id="67b64-143">***4. táblázat: Jelentés-végrehajtási lekért API-k***</span><span class="sxs-lookup"><span data-stu-id="67b64-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="67b64-144">**API**</span><span class="sxs-lookup"><span data-stu-id="67b64-144">**API**</span></span> | <span data-ttu-id="67b64-145">**Funkció**</span><span class="sxs-lookup"><span data-stu-id="67b64-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="67b64-146">Jelentés-végrehajtások lekért száma</span><span class="sxs-lookup"><span data-stu-id="67b64-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="67b64-147">Le kell kapnia az adott jelentés összes végrehajtását.</span><span class="sxs-lookup"><span data-stu-id="67b64-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="67b64-148">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="67b64-148">Next steps</span></span>

- <span data-ttu-id="67b64-149">Az API-kat a [Swagger API URL-címével próbálhatja ki.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="67b64-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>