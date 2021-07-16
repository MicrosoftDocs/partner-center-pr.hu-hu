---
title: Szoftveres hozzáférési paradigma Elemzések adatokhoz
description: A programozott elemzésekhez használható API-hívási minta magas szintű folyamatának a használata. A partnerelemzési jelentések elérésére vonatkozó API-kat is lefedi.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376677"
---
# <a name="programmatic-access-paradigm"></a>Programozott hozzáférési paradigma

Ez a diagram az új jelentéssablon létrehozásához, az egyéni jelentés ütemezéséhez és a hibaadatok lekéréséhez használt API-hívásmintát mutatja be.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Magas szintű folyamat":::
***1. ábra: Az API-hívási minta magas szintű áramlása***

Ez a lista az 1. ábra további részleteit tartalmazza.

1. Az ügyfélalkalmazás a Jelentéslekérdezés létrehozása API hívásával definiálhatja az egyéni [jelentéssémát/sablont.](#create-report-query-api) Azt is választhatja, hogy kiválaszt egy jelentéssablont (QueryId) az itt felsorolt jelentéssablontár-minták [közül.](insights-programmatic-system-queries.md)
2. Sikeres létrehozás esetén a Jelentéslekérdezés létrehozása API a QueryId értéket adja vissza.
3. Az ügyfélalkalmazásnak ezután meg kell hívnia a Jelentés létrehozása [API-t](#create-report-api) a QueryId használatával, valamint a jelentés kezdő dátumát, az ismétlési időközt, az ismétlődést és egy opcionális visszahívási URI-t.
4. A Sikeres jelentés [létrehozása API a ReportId](#create-report-api) (Jelentésazonosító) értéket adja vissza.
5. Amint a jelentés adatai letölthetők, az ügyfélalkalmazás értesítést kap a visszahívási URL-címen.
6. Az ügyfélalkalmazás ezután a [Get Report Executions API](#get-report-execution-api) használatával lekérdezi a jelentés állapotát a jelentés azonosítójával és dátumtartományával.
7. Sikeresség után a rendszer visszaadja a jelentés letöltési hivatkozását, és az alkalmazás kezdeményezheti az adatok letöltését.

## <a name="report-query-language-specification"></a>Jelentéslekérdezés nyelvének specifikációja

Bár a [](insights-programmatic-system-queries.md) rendszerlekérdezések segítségével jelentéseket hozhat létre, saját lekérdezéseket is létrehozhat az üzleti igényeinek megfelelően. Az egyéni lekérdezésekkel kapcsolatos további információkért lásd: [Egyéni lekérdezés specifikációja.](insights-programmatic-custom-query.md)

## <a name="create-report-query-api"></a>Jelentéslekérdezés API létrehozása

Az API segítségével egyéni lekérdezéseket hozhat létre, amelyek meghatározzák azt az adatkészletet, amelyből az oszlopokat és metrikákat exportálni kell. Az API biztosítja azt a rugalmasságot, hogy új jelentéskészítési sablont hozzon létre az üzleti igényeinek megfelelően.  

A rendszerlekérdezések is [használhatók.](insights-programmatic-system-queries.md) Ha nincs szükség egyéni jelentéssablonokra, közvetlenül a megadott rendszerlekérdezések QueryId-jaival hívhatja meg a Jelentési [API](#create-report-api) létrehozása api-t.  

Az alábbi példa bemutatja, hogyan hozhat létre egyéni lekérdezést, amely az elmúlt hónap első 10 ügyfelet tartalmazza bevétel szerint.

### <a name="request-syntax"></a>Kérés szintaxisa

|    Metódus     |    Kérés URI-ja     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>Kérelem fejléce

|    Fejléc     |    Típus     |    Leírás     |
|-------|-----|------|
|    Engedélyezés     |    sztring |Kötelező. Az Azure Active Directory (Azure AD) hozzáférési jogkivonata. A formátum  `Bearer <token>` a következő: .|
|    Content-Type     |sztring |`Application/JSON` |
||||

### <a name="path-parameter"></a>Elérésiút-paraméter

None

### <a name="query-parameter"></a>Lekérdezési paraméter

None

### <a name="sample-request-payload"></a>Minta kérelem hasznosadata

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>Szószedet

Ez a táblázat a kérelem hasznos elemeinek kulcsdefinícióit tartalmazza.

|Paraméter|    Kötelező     |    Leírás     |    Megengedett értékek     |
|-----|    -----    |    -----    |    -----    |
|Name |    Igen     |    A lekérdezés rövid neve     |    sztring     |
|    Leírás     |    Nem     |    A lekérdezés által visszaadott adatok leírása     |    sztring     |
|    Lekérdezés     |    Igen     |    Jelentés lekérdezési sztring     |    Adattípus: sztring <br> [Egyéni lekérdezés](insights-programmatic-custom-query.md) üzleti szükség alapján |
|        |        |        |        |

> [!Note]
> Egyéni lekérdezési mintákért tekintse meg a [példákat a mintalekérdezésekre.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Mintaválasz

A válasz hasznos adata a következőképpen strukturálva van:

Válaszkódok: 200, 400, 401, 403, 500

Példa válasz hasznos hasznosra:

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a>Szószedet

Ez a táblázat a kérelem hasznos elemeinek kulcsdefinícióit tartalmazza.

|    Paraméter     |    Leírás     |
|    ----    |    ----    |
|    QueryId (Lekérdezésazonosító)     |    A létrehozott lekérdezés univerzálisan egyedi azonosítója (UUID)     |
|    Name     |    A lekérdezésnek a kérelem hasznos adatában megadott rövid neve     |
|    Leírás     |    A lekérdezés létrehozása során megadott leírás     |
|    Lekérdezés     |    A lekérdezés létrehozása során bemenetként átadott jelentéslekérdezés     |
|    Típus     |    Állítsa a beállításra: `userDefined`     |
|    Felhasználó     |    A lekérdezés létrehozásához használt felhasználói azonosító     |
|    CreatedTime     |    A lekérdezés a következő formátumban létrehozott UTC-ideje: yyyy-MM-ddTHH:mm:ssZ     |
|    TotalCount (Teljes összeg)     |    Adatkészletek száma az Érték tömbben     |
|    StatusCode (Állapotkód)     |    Eredmény kódja <br> Lehetséges értékek: 200, 400, 401, 403, 500     |
|    message     |    Állapotüzenet az API végrehajtásából     |
|        |        |

## <a name="create-report-api"></a>Jelentési API létrehozása

Ha sikeresen létrehozott egy egyéni jelentéssablont, és [](#create-report-query-api) a Jelentéslekérdezés létrehozása válasz részeként megkapja a QueryID-t, ezt az API-t hívhatja meg, hogy rendszeres időközönként ütemezni tudja a lekérdezések végrehajtását. Beállíthatja a jelentés kézbesítésének gyakoriságát és ütemezését.
A rendszerlekérdezések esetén a Jelentés létrehozása API a QueryId használatával is [hívható.](insights-programmatic-system-queries.md)

### <a name="callback-url"></a>Visszahívási URL

A jelentés létrehozása API visszahívási URL-címet fogad el. Ezt az URL-címet a rendszer a jelentés sikeres létrehozása után fogja meghívni. A visszahívási URL-címnek nyilvánosan elérhetőnek kell lennie. Az URL-cím mellett visszahívási metódus is adható. A visszahívási metódus csak "GET" vagy "POST" lehet. Ha nem ad meg értéket, az alapértelmezett metódus a "POST". A befejezett jelentésazonosítót a visszahívás során mindig vissza kell kapnia.

POST-visszahívás: Ha az átadott `https://www.contosso.com/callback` URL-cím , akkor a visszahívott URL-cím a következő lesz: `https://www.contosso.com/callback/<reportID>` 

GET visszahívás: Ha az átadott `https://www.contosso.com/callback` URL-cím , akkor a visszahívott URL-cím a következő lesz: `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>ExecuteNow-jelentések

Van olyan kiépítés, amely ütemezés nélkül hoz létre jelentést. A jelentés-létrehozási API hasznos adata elfogadhat egy paramétert, amely az API meghívása után a jelentés létrehozására `ExecuteNow` fog sorra hozni. Ha a true (igaz) érték van beállítva, a rendszer figyelmen kívül hagyja a (igaz) mezőket, mivel ezek a jelentések `ExecuteNow` `StartTime` nincsenek `RecurrenceCount` `RecurrenceInterval` ütemezve.

Igaz érték esetén két további mező `ExecuteNow` is átvehet: `QueryStartTime` és `QueryEndTime` . Ez a két mező felülírja `TIMESPAN` a lekérdezésben található mezőt. Ezek a mezők nem alkalmazhatók az ütemezett jelentésekre, mivel az adatok egy meghatározott ideig folyamatosan jönnek létre, amely nem változik.

### <a name="request-syntax"></a>Kérésszintaxis

|    Metódus     |    Kérés URI-ja     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>Kérelem fejléce

|    Fejléc     |    Típus     |    Leírás     |
|-------|-----|------|
|    Engedélyezés     |    sztring |Kötelező. Az Azure Active Directory (Azure AD) hozzáférési jogkivonata. A formátum  `Bearer <token>` a következő: .|
|    Content-Type     |sztring |`Application/JSON` |

### <a name="path-parameter"></a>Elérési út paramétere

None

### <a name="query-parameter"></a>Lekérdezési paraméter

None

### <a name="sample-request-payload"></a>Minta kérelem hasznosadata

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a>Szószedet

A kérelem hasznos elemeinek kulcsdefinícióit az alábbiakban olvashatja:

|    Paraméter     |    Kötelező     |    Leírás     |    Megengedett értékek     |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName (Jelentés neve)     |    Igen     |    A jelentéshez hozzárendelni fog név     |    sztring     |
|    Leírás     |    Nem     |    A létrehozott jelentés leírása     |    sztring     |
|    QueryId (Lekérdezésazonosító)     |    Igen     |    Jelentéslekérdezés azonosítója     |    sztring     |
|    StartTime     |    Igen     |    A jelentés generálás megkezdésének UTC szerinti időbélyege. <br> A formátumnak a következőnek kell lennie: yyyy-MM-ddTHH:mm:ssZ       |    sztring     |
|    ExecuteNow     |    Nem     |    Ezzel a paraméterrel olyan jelentést hozhat létre, amely csak egyszer lesz végrehajtva. `StartTime`A `RecurrenceInterval` és `RecurrenceCount` a értékeket a rendszer figyelmen kívül hagyja, ha true (igaz) érték van beállítva. A jelentés azonnal, aszinkron módon lesz végrehajtva     |    true/false (igaz/hamis)     |
|    QueryStartTime (Lekérdezésindítási idő)     |    Nem     |    Igény szerint megadja az adatokat kinyerő lekérdezés kezdési idejét. Ez a paraméter csak egy olyan végrehajtási jelentésre alkalmazható, amely true `ExecuteNow` (igaz) értékre van állítva. A paraméter lekérdezésben megadott `TIMESPAN` felülbírálásai. A formátum legyen yyyy-MM-ddTHH:mm:ssZ     |    Időbélyeg sztringként     |
|    QueryEndTime (Lekérdezés ideje)     |    Nem     |    Opcionálisan megadja az adatokat kinyerő lekérdezés záró idejét. Ez a paraméter csak egy olyan végrehajtási jelentésre alkalmazható, amely true `ExecuteNow` (igaz) értékre van állítva. A paraméter lekérdezésben megadott `TIMESPAN` felülbírálásai. A formátum legyen yyyy-MM-ddTHH:mm:ssZ     |    Időbélyeg sztringként     |
|    RecurrenceInterval (Ismétlődés időköze)     |    Igen     |    Gyakoriság órákban, amikor a jelentést létre kell hoznunk. <br> A minimális érték 4, a Maximális érték pedig 2160.      |    egész szám     |
|    RecurrenceCount (Ismétlődés száma)     |    Nem     |    A létrehozható jelentések száma.     |    egész szám     |
|    Formátum     |    Nem     |    Az exportált fájl fájlformátuma. <br> Az alapértelmezett érték a CSV.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    Nem     |    Nyilvánosan elérhető URL-cím, amely igény szerint visszahívási célként is konfigurálható     |    Sztring (http URL)     |
|    CallbackMethod     |    Nem     |    A visszahíváshoz használt metódus     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>Mintaválasz

A válasz hasznos adata a következőképpen strukturálva van:

Válaszkódok: 200, 400, 401, 403, 404, 500

Példa válasz hasznos hasznosra:

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a>Szószedet

A válasz elemeinek kulcsdefiníciói az alábbiak:

|    Paraméter     |    Leírás     |
|    ----    |    ----    |
|    Jelentésazonosító     |    A létrehozott jelentés univerzálisan egyedi azonosítója (UUID)     |
|    ReportName (Jelentés neve)     |    A jelentésnek a kérelem hasznos információja alapján megadott név     |
|    Leírás     |    A jelentés létrehozása során megadott leírás     |
|    QueryId (Lekérdezésazonosító)     |    A jelentés létrehozásakor átadott lekérdezésazonosító     |
|    Lekérdezés     |    A jelentéshez végrehajtandó lekérdezési szöveg     |
|    Felhasználó     |    A jelentés létrehozásához használt felhasználói azonosító     |
|    CreatedTime     |    A jelentés a következő formátumban való létrehozásának UTC szerinti ideje: yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    A jelentés utolsó módosításának UTC szerinti időpontja a következő formátumban: yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    `ExecuteNow` a jelentés létrehozásakor beállított jelző     |
|    StartTime     |    A jelentés végrehajtásának UTC szerinti kezdési ideje a következő formátumban: yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus (Jelentésállapot)     |    A jelentés végrehajtásának állapota. A lehetséges értékek a `Paused` , `Active` a és a `Inactive`     |
|    RecurrenceInterval (Ismétlődés időköze)     |    A jelentés létrehozása során megadott ismétlődési időköz     |
|    RecurrenceCount (Ismétlődés száma)     |    A jelentés létrehozása során megadott ismétlődési szám.      |
|    CallbackUrl     |    A kérésben megadott visszahívási URL-cím     |
|    CallbackMethod     |    A kérésben megadott visszahívási metódus     |
|    Formátum     |    A jelentésfájlok formátuma. A lehetséges értékek a `CSV` vagy `TSV` a .     |
|    TotalCount (Teljes összeg)     |    Rekordok száma a Value tömbben     |
|    StatusCode (Állapotkód)     |    Eredmény kódja     |
|    message     |    Lehetséges értékek: 200, 400, 401, 403, 500. Állapotüzenet az API végrehajtásából     |
|        |        |

## <a name="get-report-execution-api"></a>Jelentés-végrehajtási API lekérte

Ezzel a módszerrel lekérdezheti egy jelentés végrehajtásának állapotát a Create Report API -tól kapott [ReportId (Jelentésazonosító) használatával.](#create-report-api) A metódus a jelentés letöltési hivatkozását adja vissza, ha a jelentés letöltésre kész. Ellenkező esetben a metódus visszaadja az állapotot. Ezzel az API-val le is kaphatja az adott jelentés összes végrehajtását.  

>[!IMPORTANT]
>Az API alapértelmezett lekérdezési paraméterei és számára vannak `executionStatus=Completed` `getLatestExecution=true` beállítva. Ezért a jelentés első sikeres végrehajtása előtt az API hívása a 404-es adatokat adja vissza. Függőben lévő végrehajtások a beállításával szerezhetők `executionStatus=Pending` be.

### <a name="request-syntax"></a>Kérésszintaxis

|    Metódus     |    Kérés URI-ja     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>Kérelem fejléce

|    Fejléc     |    Típus     |    Leírás     |
|-------|-----|------|
|    Engedélyezés     |    sztring |Kötelező. Az Azure Active Directory (Azure AD) hozzáférési jogkivonata. A formátum  `Bearer <token>` a következő: .|
|    Content-Type     |sztring |`Application/JSON` |

### <a name="path-parameter"></a>Elérésiút-paraméter

|    Paraméter neve    |    Kötelező    |    Típus    |    Leírás    |
|    ----    |    ----    |    ----    |    ----    |
|    jelentésazonosító    |    Igen    |    sztring    |    Szűrhet, hogy csak az ebben az argumentumban megadott jelentésazonosítóval kapcsolatos jelentések végrehajtási adatait lekérte. Több jelentésazonosítót is meg lehet adni pontosvesszővel (;) elválasztva.    |
|        |        |        |        |

### <a name="query-parameter"></a>Lekérdezési paraméter

|    Paraméter neve    |    Kötelező    |    Típus    |    Leírás    |
|    ----    |    ----    |    ----    |    ----    |
|    executionId (végrehajtásiazonosító)    |    Nem    |    sztring    |    Szűrhet, hogy csak az ebben az argumentumban megadott executionId -et tartalmazó jelentések adatait lekérte. Pontosvesszővel (;) elválasztva több executionId is meg lehet adni.    |
|    executionStatus (végrehajtásiállapot)    |    Nem    |    Sztring/enum    |    Szűrhet, hogy csak az ebben az argumentumban megadott executionStatus jelentéseket tartalmazza. <br> Érvényes értékek: `Pending` , `Running` és `Paused` `Completed` . <br> Az alapértelmezett érték `Completed`. <br> Pontosvesszővel (;) elválasztva több állapot is meg lehet adni.    |
|    getLatestExecution (GetLatestExecution)    |    Nem    |    boolean    |    Az API visszaadja a legutóbbi végrehajtás részleteit. Alapértelmezés szerint ez a paraméter true (igaz) értéket ad meg.<br> Ha úgy dönt, hogy a paraméter értékét false (hamis) értékként adja át, akkor az API az utolsó 90 nap végrehajtási példányait adja vissza.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Minta kérelem hasznosadata

None

### <a name="sample-response"></a>Mintaválasz

A válasz hasznos adata a következőképpen strukturálva van:

Válaszkódok: 200, 400, 401, 403, 404, 500

Példa válasz hasznos hasznosra:

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

Ha a jelentés végrehajtása befejeződött, megjelenik a `Completed` végrehajtás állapota. A jelentést a URL-címének kiválasztásával töltheti `reportAccessSecureLink` le.

### <a name="glossary"></a>Szószedet

A válasz elemeinek kulcsdefiníciói.

|    Paraméter    |    Leírás    |
|    ----    |    ----    |
|    ExecutionId (Végrehajtásiazonosító)    |    A végrehajtási példány univerzálisan egyedi azonosítója (UUID)    |
|    ReportId (Jelentésazonosító)    |    A végrehajtási példányhoz társított jelentésazonosító    |
|    RecurrenceInterval (Ismétlődés időköze)    |    A jelentés létrehozása során megadott ismétlődési időköz    |
|    RecurrenceCount (Ismétlődés száma)    |    A jelentés létrehozása során megadott ismétlődési szám    |
|    CallbackUrl    |    A végrehajtási példányhoz társított visszahívási URL-cím    |
|    CallbackMethod    |    A végrehajtási példányhoz társított visszahívási metódus    |
|    Formátum    |    A végrehajtás végén létrehozott fájl formátuma    |
|    ExecutionStatus (Végrehajtásiállapot)    |    A jelentés-végrehajtási példány állapota. <br> Érvényes értékek: `Pending` , `Running` , `Paused` és `Completed`    |
|    ReportAccessSecureLink    |Hivatkozás, amelyen keresztül a jelentés biztonságosan elérhető        |
|    ReportExpiryTime    |    A jelentéshivatkozás lejáratának UTC szerinti ideje a következő formátumban: yyyy-MM-ddTHH:mm:ssZ    |
|    ReportGeneratedTime (Jelentésgenerált idő)    |    A jelentés a következő formátumban létrehozott UTC-ideje: yyyy-MM-ddTHH:mm:ssZ    |
|    TotalCount (Teljes összeg)    |    Adatkészletek száma az Érték tömbben    |
|    StatusCode (Állapotkód)    |    Eredmény kódja <br> Lehetséges értékek: 200, 400, 401, 403, 404 és 500    |
|    message    |    Állapotüzenet az API végrehajtásából    |
|        |        |

## <a name="next-steps"></a>Következő lépések

- Próbálja ki az API-kat a [swagger API URL-címével](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)
- [Az első API-hívás hívása](insights-programmatic-first-api-call.md)