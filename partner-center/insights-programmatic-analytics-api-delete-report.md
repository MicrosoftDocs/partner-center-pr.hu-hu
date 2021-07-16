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
# <a name="delete-report-api"></a>Jelentési API törlése

A végrehajtáskor ez az API törli az összes jelentés- és jelentés-végrehajtási rekordot.

**Kérésszintaxis**

|    Metódus    |    Kérés URI-ja    |
|    ----    |    ----    |
|    DELETE    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

**Kérés fejléce**

|    Fejléc    |    Típus    |    Leírás    |
|    ----    |    ----    |    ----    |
|    Engedélyezés    |    sztring    |    Kötelező. Az Azure Active Directory (AAD) hozzáférési jogkivonata a következő formában:`Bearer <token>`    |
|    Content-Type    |    sztring    |    `Application/JSON`    |
|        |        |        |

**Elérésiút-paraméter**

|    Paraméter neve    |    Típus    |    Kötelező    |    Leírás    |
|    ----    |    ----    |    ----    |    ----    |
|    jelentésazonosító     |    sztring    |    No    |    A törölt jelentés azonosítója    |
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

**Szószedet**

Ez a tábla határozza meg a válasz legfontosabb elemeit:

|    Paraméter    |    Leírás    |
|    ----    |    ----    |
|    Jelentésazonosító     |    A törölt jelentés univerzálisan egyedi azonosítója (UUID)     |
|    ReportName (Jelentés neve)     |    A jelentésnek a létrehozás során megadott név     |
|    Leírás     |    A jelentés létrehozása során megadott leírás     |
|    QueryId (Lekérdezésazonosító)     |    A jelentés létrehozásakor átadott lekérdezésazonosító     |
|    Lekérdezés     |    A jelentéshez végrehajtandó lekérdezési szöveg     |
|    Felhasználó     |    A jelentés létrehozásához használt felhasználói azonosító     |
|    CreatedTime     |    A jelentés létrehozási ideje. Az időformátum: yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    A jelentés utolsó módosításának időpontja. Az időformátum: yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    A jelentés létrehozásakor beállított ExecuteNow jelző     |
|    StartTime     |    A jelentés végrehajtásának megkezdésének ideje. Az időformátum: yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus (Jelentésállapot)     |    A jelentés végrehajtásának állapota. A lehetséges értékek: Szüneteltetve, Aktív és Inaktív.     |
|    RecurrenceInterval (Ismétlődés időköze)     |    A jelentés létrehozása során megadott ismétlődési időköz     |
|    RecurrenceCount (Ismétlődés száma)     |    A jelentés létrehozása során megadott ismétlődési szám     |
|    CallbackUrl     |    A kérésben megadott visszahívási URL-cím     |
|    CallbackMethod    |    A kérésben megadott visszahívási metódus    |
|    Formátum     |    A jelentésfájlok formátuma     |
|    TotalCount (Teljes összeg)     |    Adatkészletek száma az Érték tömbben     |
|    Üzenet     |    Állapotüzenet az API végrehajtásából     |
|    StatusCode (Állapotkód)     |    Eredménykód. Lehetséges értékek: 200, 400, 401, 403, 500     |
|        |        |
