---
title: Jelentés API-k le Elemzések adatok
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val lekérhetők az összes elérhető jelentésazonosító a Partnerközpont elemzésben.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376750"
---
# <a name="get-report-api"></a>A jelentés API-jának lekérte

Ez az API lekért minden ütemezett jelentést.

**Kérés szintaxisa**

|    Metódus    |    Kérés URI-ja    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
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
|    jelentésazonosító     |    sztring    |    No    |    Szűrhet, hogy csak az ebben az argumentumban megadott reportId-t tartalmazó jelentések részleteit lekérte     |
|    reportName (jelentés neve)     |    sztring    |    No    |    Szűrhet, hogy csak az ebben az argumentumban megadott reportName paramétert tartalmazó jelentések részleteit lekérte     |
|    queryId (lekérdezésazonosító)     |    sztring    |    No    |    Szűrhet, hogy csak az ebben az argumentumban megadott queryId-t tartalmazó jelentések adatait lekérdezze     |
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
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

**Szószedet**

Ez a tábla határozza meg a válasz legfontosabb elemeit:

|    Paraméter    |    Leírás    |
|    ----    |    ----    |
|    ReportId (Jelentésazonosító)     |    A létrehozott jelentés egyedi UUID-je     |
|    ReportName (Jelentés neve)     |    A jelentésnek a kérelem hasznos információban megadott neve     |
|    Leírás     |    A jelentés létrehozásakor megadott leírás     |
|    QueryId (Lekérdezésazonosító)     |    A jelentés létrehozásakor átadott lekérdezésazonosító     |
|    Lekérdezés     |    A jelentéshez végrehajtandó szöveg lekérdezése     |
|    Felhasználó     |    A jelentés létrehozásához használt felhasználói azonosító     |
|    CreatedTime     |    A jelentés létrehozási ideje. Az időformátum: yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    A jelentés utolsó módosításának időpontja. Az időformátum: yyyy-MM-ddTHH:mm:ssZ     |
|    executeNow     |    A jelentés létrehozásakor beállított ExecuteNow jelző    |
|    StartTime     |    Megkezdődik az idő végrehajtása. Az időformátum: yyyy-MM-ddTHH:mm:ssZ     |
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