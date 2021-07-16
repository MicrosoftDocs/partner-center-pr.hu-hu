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
# <a name="available-apis-for-partner-insights-analytics"></a>Elérhető API-k a partnerelemzéshez

Az alábbiakban a partnerelemzési API-k és a hozzájuk tartozó funkciók listája található.

## <a name="dataset-pull-apis"></a>Adatkészlet-lekért API-k

***1. táblázat: Adatkészlet lekért API-k***

| **API** | **Funkció** |
| --- | --- |
| [Az összes adatkészlet lekérte](insights-programmatic-analytics-api-get-dataset.md) | Lekérhetők az összes elérhető adatkészlet. Az adatkészletek felsorolják a táblákat, oszlopokat, metrikákat és időtartományokat. |
|||

## <a name="query-management-apis"></a>Lekérdezéskezelési API-k

***2. táblázat: Lekérdezéskezelési API-k***

| **API** | **Funkció** |
| --- | --- |
| [Jelentéslekérdezés létrehozása](insights-programmatic-access-paradigm.md#create-report-query-api) | Egyéni lekérdezéseket hoz létre, amelyek meghatározzák azt az adatkészletet, amelyből exportálni kell az oszlopokat és metrikákat. |
| [GET Jelentéslekérdezés](insights-programmatic-analytics-api-get-report-queries.md) | Lekérdezi a jelentésekben használható összes lekérdezést. Alapértelmezés szerint lekérdezi a rendszer és a felhasználó által megadott összes lekérdezést. |
| [DELETE Report Query](insights-programmatic-analytics-api-delete-report-queries.md) | Törli a felhasználó által megadott lekérdezéseket. |
|||

## <a name="report-management-apis"></a>Jelentéskezelési API-k

***3. táblázat: Jelentéskezelési API-k***

| **API** | **Funkció** |
| --- | --- |
| [Jelentés létrehozása](insights-programmatic-access-paradigm.md#create-report-api) | Rendszeres időközönként végrehajtandó lekérdezést ütemez. |
| [TRY Report Query](insights-programmatic-analytics-api-try-report-queries.md) | Végrehajt egy jelentéslekérdezés-utasítást. Csak 10 rekordot ad vissza, amelyek használatával a partner ellenőrizheti, hogy az adatok a vártnak megfelelőek-e. |
| [Jelentés lekérése](insights-programmatic-analytics-api-get-report.md) | Szerezze be az összes ütemezett jelentést. |
| [Jelentés frissítése](insights-programmatic-analytics-api-update-report.md) | Jelentésparaméter módosítása. |
| [Jelentés törlése](insights-programmatic-analytics-api-delete-report.md) | Törli az összes jelentés- és jelentés-végrehajtási rekordot. |
| [Jelentés-végrehajtások szüneteltetése](insights-programmatic-analytics-api-pause-report-executions.md) | Szünetelteti a jelentések ütemezett végrehajtását. |
| [Jelentés-végrehajtások folytatása](insights-programmatic-analytics-api-resume-report-executions.md) | Folytatja egy szüneteltetett jelentés ütemezett végrehajtását. |
|||

## <a name="report-execution-pull-apis"></a>Jelentés-végrehajtási lekért API-k

***4. táblázat: Jelentés-végrehajtási lekért API-k***

| **API** | **Funkció** |
| --- | --- |
| [Jelentés-végrehajtások lekért száma](insights-programmatic-access-paradigm.md#get-report-execution-api) | Le kell kapnia az adott jelentés összes végrehajtását. |
|||

## <a name="next-steps"></a>Következő lépések

- Az API-kat a [Swagger API URL-címével próbálhatja ki.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)