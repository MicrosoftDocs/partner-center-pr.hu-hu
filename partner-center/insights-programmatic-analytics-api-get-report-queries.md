---
title: Jelentéslekérdezések API-ja – Elemzések adatok lekérdezve
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val lekérdezhető az összes rendelkezésre álló lekérdezés a jelentési API-ban való használatra.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376751"
---
# <a name="get-report-queries-api"></a>Jelentéslekérdezések API-jának le kérése

A Jelentéslekérdezések lekérdezi API lekérdezi a jelentésekben használható összes lekérdezést. Alapértelmezés szerint lekérdezi az összes rendszer- és felhasználó által megadott lekérdezést.

**Kérésszintaxis**

|    Metódus    |    Kérés URI-ja    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

**Kérés fejléce**

|    Fejléc    |    Típus    |    Leírás    |
|    ----    |    ----    |    ----    |
|    Engedélyezés    |    sztring    |    Kötelező. Az Azure Active Directory (AAD) hozzáférési jogkivonata a következő formában:`Bearer <token>`    |
|    Content-Type    |    sztring    |    `Application/JSON`    |
|        |        |        |

**Elérésiút-paraméter**

None

**Lekérdezési paraméter**

|    Paraméter neve    |    Típus    |    Kötelező    |    Leírás    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId (lekérdezésazonosító)     |    sztring     |    No    |    Szűrés, ha csak a argumentumban megadott azonosítóval megadott lekérdezések adatait lekérdezi     |
|    queryName (lekérdezés neve)     |    sztring     |    No    |    Szűrhet, hogy csak a argumentumban megadott nevű lekérdezések adatait lekérdezze     |
|    IncludeSystemQueries (Fájlrendszerlekérdezés)     |    boolean     |    Nem    |    Előre definiált rendszerlekérdezések a válaszban     |
|    IncludeOnlySystemQueries     |    boolean     |    Nem    |    Csak rendszerlekérdezések szerepeljenek a válaszban     |
|        |        |        |        |


**Hasznos információ kérése**

None

**Szószedet**

None

**Válasz**

A válasz hasznos adata a következőképpen strukturálva van:

Válaszkód: 200, 400, 401, 403, 404, 500

Példa válasz hasznos hasznosra:

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

**Szószedet**

Ez a tábla határozza meg a válasz legfontosabb elemeit:

|    Paraméter    |    Leírás    |
|    ----    |    ----    |
|    QueryId (Lekérdezésazonosító)     |    A lekérdezés egyedi UUID-je     |
|    Name     |    A lekérdezésnek a lekérdezés létrehozásakor megadott név     |
|    Leírás     |    A lekérdezés létrehozása során megadott leírás     |
|    Lekérdezés     |    Jelentés lekérdezési sztringe     |
|    Típus     |    Felhasználó által létrehozott lekérdezésekhez és rendszerhez előre definiált rendszerlekérdezésekhez állítsa be a userDefined értéket     |
|    Felhasználó     |    A lekérdezést létrehozó felhasználói azonosító     |
|    CreatedTime     |    A lekérdezés létrehozásának ideje     |
|    TotalCount (Teljes összeg)     |    Adatkészletek száma az Érték tömbben     |
|    Üzenet     |    Állapotüzenet az API végrehajtásából     |
|    StatusCode (Állapotkód)     |    Eredménykód. Lehetséges értékek: 200, 400, 401, 403, 500     |
|        |        |
