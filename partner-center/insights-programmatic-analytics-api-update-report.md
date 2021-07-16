---
title: Jelentési API frissítése
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val frissítheti a jelentésparamétereket az Partnerközpont elemzésben.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376734"
---
# <a name="update-report-api"></a>Jelentési API frissítése

Ez az API segít a jelentésparaméterek módosításában.

**Kérés szintaxisa**

|    Metódus    |    Kérés URI-ja    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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
|    jelentésazonosító     |    sztring    |    No    |    A módosított jelentés azonosítója     |
|        |        |        |        |

**Lekérdezési paraméter**

None

**Hasznos információ kérése**

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

**Szószedet**

Ez a táblázat a válasz elemeinek kulcsdefinícióit sorolja fel.

|    Paraméter    |    Kötelező    |    Leírás    |    Megengedett értékek    |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName (Jelentés neve)     |    Igen     |    A jelentéshez hozzárendelni fog név     |    Sztring     |
|    Leírás     |    Nem     |    A létrehozott jelentés leírása     |    Sztring     |
|    StartTime     |    Igen    |    Időbélyegző, amely után megkezdődik a jelentés létrehozása     |    Sztring     |
|    RecurrenceInterval (Ismétlődés időköze)     |    Nem     |    A jelentés generálás gyakorisága órákban. A minimális érték 4     |    Egész szám     |
|    RecurrenceCount (Ismétlődés száma)     |    Nem     |    A létrehozandó jelentés száma. Az alapértelmezett érték a határozatlan.     |    Egész szám     |
|    Formátum     |    Nem    |    Az exportált fájl fájlformátuma. Az alapértelmezett érték CSV     |    CSV/TSV     |
|    CallbackURL     |    Nem     |    https visszahívási URL-cím, amely a jelentés létrehozása esetén lesz meghívva     |    Sztring     |
|    CallbackMethod    |    Nem    |    A visszahíváshoz használt HTTP-metódus    |    GET/POST    |
|        |        |        |        |


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
|    ReportId (Jelentésazonosító)     |    A frissített jelentés univerzálisan egyedi azonosítója (UUID)     |
|    ReportName (Jelentés neve)     |    A jelentésnek a kérelem hasznos információban megadott neve     |
|    Leírás     |    A jelentésnek a kérelem hasznos ában megadott leírás     |
|    QueryId (Lekérdezésazonosító)     |    A jelentés létrehozásakor átadott lekérdezésazonosító     |
|    Lekérdezés     |    A jelentéshez végrehajtandó szöveg lekérdezése     |
|    Felhasználó     |    A jelentés létrehozásához használt felhasználói azonosító     |
|    CreatedTime     |    A jelentés létrehozási ideje. Az időformátum: yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    A jelentés utolsó módosításának időpontja. Az időformátum: yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    A jelentés létrehozásakor beállított ExecuteNow jelző    |
|    StartTime     |    A jelentés végrehajtásának megkezdésének ideje. Az időformátum: yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus (Jelentésállapot)     |    A jelentés végrehajtásának állapota. A lehetséges értékek: Szüneteltetve, Aktív és Inaktív.     |
|    RecurrenceInterval (Ismétlődés időköze)     |    A kérés hasznos adatokban megadott ismétlődési időköz     |
|    RecurrenceCount (Ismétlődés száma)     |    A kérelem hasznos adatokban megadott ismétlődési száma     |
|    CallbackUrl     |    A kérésben megadott visszahívási URL-cím     |
|    CallbackMethod    |    A kérésben megadott visszahívási metódus    |
|    Formátum     |    A jelentésfájlok formátuma     |
|    TotalCount (Teljes összeg)     |    Adatkészletek száma az Érték tömbben     |
|    Üzenet     |    Állapotüzenet az API végrehajtásából     |
|    StatusCode (Állapotkód)     |    Eredménykód. Lehetséges értékek: 200, 400, 401, 403, 500     |
|        |        |