---
title: Gyakori kérdések a partnerelemzések programozott hozzáférésével kapcsolatban
description: Választ kaphat a partnerelemzési adatok API-n keresztüli elérésével kapcsolatos gyakori kérdésekre.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 5645a834c2b6a84920ba032198f7f62aa1487c47
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376726"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Gyakori kérdések az elemzési adatokhoz való szoftveres hozzáféréssel kapcsolatban

Ez a cikk a partnerelemzési adatok programozott módon való elérésével kapcsolatos gyakori kérdésekre ad választ a Partnerközpont.

## <a name="api-responses"></a>API-válaszok

Milyen forgatókönyvekben kaphatok a 200-astól eltérő (sikeres) API-választ?

Ez a táblázat ismerteti az API-válaszokat, és hogy mi a következő, ha megkapja azokat.

|    Hibaleírás     |    Hibakód     |    Hibaelhárítás     |
|    ----    |    ----    |    ----    |
|    Nem engedélyezett     |    401     |    Ez egy hitelesítési kivétel. Ellenőrizze a Azure Active Directory (AAD) jogkivonat helyességét. Az AAD-jogkivonat 60 percig érvényes, amely után újra létre kell hoznia az AAD-jogkivonatot.     |
|    Érvénytelen táblanév     |    400     |    Az adatkészlet neve helytelen. Az adatkészlet nevének újraellenőrzéséhez hívja meg a "Get All Datasets" API-t.     |
|    Helytelen oszlopnév     |    400     |    A lekérdezés oszlopának neve helytelen. Ellenőrizze újra az oszlop nevét a "Get All Datasets" API hívással, vagy tekintse meg az oszlopneveket az adatdefiníciókban    |
|    Null vagy hiányzó érték     |    400     |    Előfordulhat, hogy az API kérelem hasznos adatának részeként hiányoznak a kötelező paraméterek.     |
|    Érvénytelen jelentésparaméterek     |    400     |    Győződjön meg arról, hogy a jelentés paraméterei helyesek. Előfordulhat például, hogy 4-esnél kisebb értéket ad a RecurrenceInterval paraméterhez.     |
|    Az ismétlődési időköznek 4 és 2160 közé kell esnie     |    400     |    Győződjön meg arról, hogy a RecurrenceInterval kérésparaméter értéke 4 és 2160 közé esik.     |
|    Érvénytelen lekérdezésazonosító     |    400     |    Ellenőrizze újra a létrehozott QueryId-t.     |
|    Érvénytelen jelentésparaméterek létrehozása – A jelentés kezdési ideje legyen legalább 4 óra az aktuális UTC-időtől     |    400     |    A Start Time paraméter a hasznos kérések részeként nem lehet a múltban. A jelentés kezdési ideje legalább 4 óra legyen az aktuális UTC-időponttól.     |
|    A kért "sztring" érték nem található     |    400     |    Ellenőrizze, hogy frissítette-e a kérés paramétereit `callbackurl` vagy formátumát.     |
|    Nem található elem adott szűrőkkel.     |    404     |    Ellenőrizze a Get Report Executions API-ban használt reportID paramétert.     |
|    Az adott szűrési feltételekhez nem történtek végrehajtások. Ellenőrizze újra a jelentésazonosítót vagy a executionId-t, és próbálja újra az API-t a jelentés ütemezett végrehajtási ideje után     |    404     |    Győződjön meg arról, hogy a reportId helyes. Próbálja meg újra az API-t a jelentés ütemezett végrehajtási ideje után a kérelem hasznos adatában megadottak szerint.     |
|    Belső hiba történt a jelentés létrehozásakor. Korrelációs azonosító <>     |    500     |    Győződjön meg arról, hogy a *StartTime,* *QueryStartTime* és *QueryEndTime* mezők dátumformátuma helyes.     |
|    A szolgáltatás nem érhető el    |    500     |    Ha folyamatosan elérhetetlenné válik egy szolgáltatás (5xx hiba), nyisson egy támogatási jegyet.    |
|        |        |        |

## <a name="no-records"></a>Nincsenek rekordok

A 200-as API-választ kapom, amikor letöltem a jelentést a biztonságos helyről. Miért nem kapok rekordokat?
Ellenőrizze, hogy a lekérdezésben lévő sztring tartalmazza-e az oszlopfejléc egyik megengedett értékét. Ez a lekérdezés például nulla eredményt ad vissza:

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

Ebben a példában a megengedett értékei a `IsDuplicateRowForPGA` 0 vagy az 1. A különböző [oszlopok összes](insights-data-definitions.md) lehetséges értékét az Adatdefiníciókban tekintse meg.
