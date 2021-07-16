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
# <a name="delete-report-queries-api"></a>Jelentéslekérdezések törlése API

Ez az API törli a felhasználó által megadott lekérdezéseket.

**Kérés szintaxisa**

|    Metódus    |    Kérés URI-ja    |
|    ----    |    ----    |
|    DELETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

**Kérelemfejléc**

|    Fejléc    |    Típus    |    Leírás    |
|    ----    |    ----    |    ----    |
|    Engedélyezés    |    sztring    |    Kötelező. Az Azure Active Directory (AAD) hozzáférési jogkivonat a következő formában:`Bearer <token>`    |
|    Content-Type    |    sztring    |    `Application/JSON`    |
|        |        |        |

**Elérésiút-paraméter**

|    Paraméter neve    |    Típus    |    Kötelező    |    Leírás    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId (lekérdezésazonosító)     |    sztring     |    No    |    Szűrhet, hogy csak a argumentumban megadott azonosítóval megadott lekérdezések adatait lekérdezze     |
|        |        |        |        |

**Lekérdezési paraméter**

None

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
|    QueryId (Lekérdezésazonosító)     |    A törölt lekérdezés egyedi UUID-je    |
|    Name     |    A törölt lekérdezés neve    |
|    Leírás     |    A törölt lekérdezés leírása     |
|    Lekérdezés     |    A törölt lekérdezés lekérdezési sztringének jelentése    |
|    Típus     |    A felhasználó által létrehozott lekérdezésekhez a userDefined (felhasználó által definiált) beállítás van megállítva     |
|    Felhasználó     |    A lekérdezést létrehozó felhasználói azonosító     |
|    CreatedTime     |    A lekérdezés létrehozásának ideje     |
|    TotalCount (Teljes összeg)     |    Adatkészletek száma az Érték tömbben     |
|    Üzenet     |    Állapotüzenet az API végrehajtásából     |
|    StatusCode (Állapotkód)     |    Eredménykód. Lehetséges értékek: 200, 400, 401, 403, 500     |
|        |        |
