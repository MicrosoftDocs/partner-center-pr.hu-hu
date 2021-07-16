---
title: Az összes adatkészlet API le Elemzések adatok
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezzel az API-val lekérhetők az összes rendelkezésre álló adatkészlet részletei az Partnerközpont elemzésben.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376671"
---
# <a name="get-all-datasets-api"></a>Az összes adat adatkészlet API-jának lekérte

A Get all datasets API lekérte az összes rendelkezésre álló adatkészletet. Az adatkészletek felsorolják a táblákat, oszlopokat, metrikákat és időtartományokat.

**Kérésszintaxis**

|    Metódus    |    Kérés URI-ja    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
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
|    datasetName (adatkészlet neve)    |    sztring    |    No    |    Szűrés egyetlen adatkészlet részleteinek lekért érdekében    |
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
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

**Szószedet**

Ez a tábla határozza meg a válasz legfontosabb elemeit:

|    Paraméter    |    Leírás    |
|    ----    |    ----    |
|    DatasetName (Adatkészlet neve)     |    A tömbobjektum által definiált adatkészlet neve     |
|    SelectableColumns (Kiválaszthatóoszlopok)     |    A kiválasztott oszlopokban megadva nyers oszlopok     |
|    Elérhetőmetriák     |    A kiválasztott oszlopokban megadva az aggregáció/metrika oszlopneveket     |
|    AvailableDateRanges (ElérhetőDateRanges)     |    Az adatkészlet jelentéslekérdezésekben használható dátumtartomány     |
|    minimumRecurrenceInterval     |    Az Ismétlődési időköz minimális értéke     |
|    TotalCount (Teljes összeg)     |    Adatkészletek száma az Érték tömbben     |
|    Üzenet     |    Állapotüzenet az API végrehajtásából     |
|    StatusCode (Állapotkód)     |    Eredménykód. Lehetséges értékek: 200, 400, 401, 403, 500     |
|        |        |
