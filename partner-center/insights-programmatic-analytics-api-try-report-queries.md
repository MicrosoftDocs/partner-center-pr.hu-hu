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
# <a name="try-report-queries-api"></a>A jelentéslekérdezések API-jának kipróbálja

Ez az API végrehajt egy Jelentéslekérdezés utasítást. Az API csak 100 rekordot ad vissza, amelyek segítségével partnerként ellenőrizheti, hogy az adatok a vártnak megfelelőek-e.

> [!IMPORTANT]
> Ez az API 100 másodperces lekérdezés-végrehajtási időtúllépéssel rendelkezik. Ha azt veszi észre, hogy az API több mint 100 másodpercet vesz igénybe, nagyon valószínű, hogy a lekérdezés szintaktikailag helyes, különben a 200-astól más hibakódot kapott volna. A jelentés tényleges létrehozása akkor lesz megfelelő, ha a lekérdezési szintaxis helyes.

**Kérés szintaxisa**

|    Metódus    |    Kérés URI-ja    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

**Kérelemfejléc**

|    Fejléc    |    Típus    |    Leírás    |
|    ----    |    ----    |    ----    |
|    Engedélyezés    |    sztring    |    Kötelező. Az Azure Active Directory (AAD) hozzáférési jogkivonat a következő formában:`Bearer <token>`    |
|    Content-Type    |    sztring    |    `Application/JSON`    |
|        |        |        |

**Elérésiút-paraméter**

None

**Lekérdezési paraméter**

|    Paraméter neve    |    Típus    |    Kötelező    |    Leírás    |
|    ----    |    ----    |    ----    |    ----    |
|    exportQuery     |    sztring    |    No    |    Végrehajtandó lekérdezési sztring jelentése     |
|    queryId (lekérdezésazonosító)     |    sztring    |    No    |    Egy érvényes meglévő lekérdezésazonosító. Kölcsönösen kizárják egymást az exportQuery paraméterben megadott lekérdezési sztringekkel    |
|    startTime     |    sztring    |    No    |    A kezdési időpont, amelyből az adatokat szeretnénk. Felülbírálja a lekérdezésben megadott időtartamokat    |
|    endTime     |    sztring    |    No    |    Az adatok kívánt időszakának vége. Felülbírálja a lekérdezésben megadott időtartamokat    |
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

**Szószedet**

Ez a tábla határozza meg a válasz legfontosabb elemeit:

|    Paraméter    |    Leírás    |
|    ----    |    ----    |
|    TotalCount (Teljes összeg)     |    Adatkészletek száma az Érték tömbben     |
|    Üzenet     |    Állapotüzenet az API végrehajtásából     |
|    StatusCode (Állapotkód)     |    Eredménykód. Lehetséges értékek: 200, 400, 401, 403, 500     |
|        |        |
