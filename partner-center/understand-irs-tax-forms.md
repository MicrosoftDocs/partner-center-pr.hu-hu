---
title: A Microsoft által kiadott adóhatósági adózási űrlapok ismertetése
description: Ismerje meg a Microsoft által kiadott adózási űrlapokat, beleértve azokat is, akik megkapják azokat, és amikor elérhetővé teszik őket.
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.localizationpriority: medium
ms.date: 09/30/2020
ms.openlocfilehash: 42c5d6f0d31e6509253fe44d5b97606fc688f177
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712817"
---
# <a name="understand-irs-tax-forms-issued-by-microsoft"></a>A Microsoft által kiadott adóhatósági adózási űrlapok ismertetése

A Microsoft évente egy vagy több előfizetést is kaphat. Ez a tartózkodási helytől, valamint a kapott értékesítések és kifizetések mennyiségétől függ. A Microsoft köteles kiadni ezeket az űrlapokat, és azokat a belső bevételi szolgáltatással (IRS).

Ez a cikk részletesebben ismerteti ezeket az űrlapokat, beleértve az azok fogadását és a rendelkezésre állásuk időpontját is.

## <a name="types-of-tax-forms"></a>Az adózási űrlapok típusai

| IRS-adó űrlapja | Description | Rendelkezésre állás |
|--------------|-------------|--------------|
|1099 – MISC, 1099-K | Értékesítési tevékenységhez és/vagy a Microsoft piactéren való részvételhez nyújtott fizetésekhez kapcsolódóan | A nyomtatott űrlapok **január 31-ig** vagy azt megelőzően postmarked lesznek. a PDF-másolatok a [partner Centerben](https://partner.microsoft.com/dashboard) lesznek elérhetők (a **partner Center fiók beállításaiban** a **kifizetések és adók > a kifizetések és az adó-profilok** között). |
|1042 – S | A kifizetésekhez kapcsolódóan, amelyekre Egyesült Államok forrásadó vonatkozik | A nyomtatott űrlapok **március 15**-én vagy azt megelőzően postmarked lesznek. a PDF-másolatok a partner Centerben lesznek elérhetők (a **partner Center fejlesztői beállításaiban** a **kifizetések és az adó >** a kifizetések és az adó profilok között).  |

> [!NOTE]
> Az IRS-adózási űrlapokon használt címnek a [kifizetési fiók és az adózási űrlapok beállításakor](set-up-your-payout-account.md)az adó-profilban szereplő címről származik. Ha a címe módosult, ügyeljen arra, hogy frissítse az **adózási profilban** szereplő címeket.

A rendszer a következő címekről küldi el az adó űrlapokat:

**Egyesült államokbeli állampolgárok:**

| Üzleti csoport         | Jogi személy          | Cím                                          |
|------------------------|-----------------------|--------------------------------------------------|
| Windows, Office, Azure | Microsoft Corporation | One Microsoft Way<br>Redmond, WA 98052 USA       |
| Hirdetés            | Microsoft online Inc. | 6880 Sierra Center Parkway<br>Reno, NV 98511 USA |

**Nem amerikai állampolgárok:**

| Üzleti csoport         | Jogi személy          | Cím                                          |
|------------------------|-----------------------|--------------------------------------------------|
| Windows, Office, Azure | Microsoft Ireland Operations Limited (a Microsoft Corporation által a Microsoft Corporation minősített közvetítőként működő Microsoft Ireland általi fizetése) | Egy Microsoft-hely<br>Dél-megyei üzleti Park<br>Leopardstown, Dublin 18, D18 P521, Írország|
| Hirdetés          | A Microsoft Ireland Operations Limited (a Microsoft online Inc. fizetési ügynökként működő Microsoft Ireland) | Egy Microsoft-hely<br>South County& üzleti Park<br>Leopardstown, Dublin 18, D18 P521, Írország |
| Hirdetés            | Microsoft online Inc. | 6880 Sierra Center Parkway<br>Reno, NV 98511 USA |

>[!NOTE]
> \* A Microsoft Ireland Operations Limited a következő országok állampolgárainak fizet ki hirdetési bevételeket: Ausztria, Belgium, Bulgária, Horvátország, Ciprus, Csehország, Dánia, Észtország, Finnország, Franciaország, Németország, Görögország, Magyarország, Írország, Egyesült Királyság, Olaszország, Lettország, Liechtenstein, Litvánia, Luxemburg, Málta, Monaco, Hollandia, Norvégia, Lengyelország, Portugália, Románia, Szlovákia, Szlovénia, Dél-Afrika, Spanyolország, Svédország, Svájc, Egyesült Királyság

## <a name="for-developers-located-in-the-united-states"></a>A Egyesült Államokban található fejlesztők számára

| Ha Egyesült Államok a fizetős alkalmazásokat értékesítő fejlesztő vagyok, és...   | A következő űrlapot kell megkapnia: |
|------------------------|-----------------------|
| Több **mint 200 alkalmazás értékesítésével** rendelkezem, és a vonatkozó adózási évben a **$20 000 USD-nél nagyobb** mennyiségű értékesítési összeg szerepel (**nem** számítva a Brazíliában és Kínában a Microsoft Store a Windows 10 rendszeren.)| **1099 – K:**<br/>Filer: Microsoft Corporation<br/>Ein: \* \* \* \* \* 4442<br/><br/>**Fontos:** A 1099 – K űrlap **bruttó vásárlási** összegeket tartalmaz, és nem fizet Önnek.| 
| **Legalább $10-os fizetést** kaptam a Brazíliában és kínában a Microsoft Store a Windows 10-es vagy (II) értékesítések keretében a Minecraft piactéren.<br/><br/>**OR**<br/><br/>Legalább $600 érkezett a Microsoft által a vonatkozó adózási évben nem kapcsolódó, az alkalmazás értékesítésével kapcsolatos kifizetésekben (például a versenytől vagy promóciótól származó ösztönző kifizetések vagy kifizetések)| **1099 – MISC:**<br/>Megbízó: Microsoft Corporation<br/>Ein: \* \* \* \* \* 4442<br/><br/>**Fontos:** Bizonyos üzleti entitások nem kapnak 1099 – MISC űrlapot, a Microsofttól kapott fizetési összegektől függetlenül.  További információért forduljon a Tax Professional szolgáltatáshoz.| 
| A fentiek egyike sem érvényes.| Nincsenek |
| <br/><br/>**Ha Egyesült Államok fejlesztő vagyok, aki hirdetéseket dolgoz fel az alkalmazásokban, és...** |<br/><br/>**A következő űrlapot kell megkapnia:** |
|**Legalább $600-as összeget** kaptam az alkalmazásokban lévő hirdetésektől az alkalmazandó adózási évben. | **1099 – MISC:**<br/>Megbízó: Microsoft online Inc<br/>Ein: \* \* \* \* \* 0505<br/><br/>**Fontos:** Bizonyos üzleti entitások nem kapnak 1099 – MISC űrlapot, a Microsofttól kapott fizetési összegektől függetlenül.  További információért forduljon a Tax Professional szolgáltatáshoz. |
| A vonatkozó adózási évben az alkalmazásokban lévő hirdetésektől kapott **befizetések esetében kevesebb, mint $600** . | Nincsenek |


## <a name="for-developers-located-outside-of-the-united-states"></a>A Egyesült Államokon kívül található fejlesztők számára


| **Kérdés** | **Válasz** |
|---|---|
| **1042-S formátumú űrlapot kaptam a Microsofttól. Mi ez?** | A Microsoft megadta Önnek a 1042-S űrlapokat vagy űrlapokat, mivel a Egyesült Államok adóhatóságnak bejelentésnek minősülő bevételt kifizette, és a rendszer visszatartási adót jelentett.  Ehhez a jelentési követelményhez a 1042-S formanyomtatványt használjuk. | 
| **Mit tegyek az űrlapokkal?** | Általában nincs szükség konkrét műveletre az Ön részéről. A 1042-S űrlap akkor lehet hasznos, ha a helyi adóhatóságot bármilyen adójóváírás esetén alkalmazni kívánja.  További információt a témakörről a saját adó-tanácsadókkal foglalkozó cikkben talál. | 
| **Miért nem fizettek adót a W8 űrlap elvégzése után?** | Az adókat a következők esetén fogja visszatartani:<br/><br/>1. nem fejezte be helyesen az W8 szakaszt, vagy <br/>2. Ön olyan országban lakik, amely nem rendelkezik a Egyesült Államokkal rendelkező adózási szerződéssel.<br/><br/>A partneri központot bármikor felkeresheti egy frissített W8 űrlap beküldéséhez.<br/><br/> **Megjegyzés:** Nem minden bevételt adó forrásadó vonatkozik. | 
| **Egy frissített W8 űrlapot készítettem érvényes szerződési információkkal. A Microsoft visszatéríti a visszatartott adót?** | Ha az adót visszatartották, nem lehet visszatéríteni. Vegye fel a kapcsolatot az adóügyi tanácsadókkal, és beszéljen arról, hogy igényelhet-e helyi kreditet az ilyen adókhoz, vagy hogy kérhet-e visszatérítést az IRS-től. | 
| **Milyen értékesítési jelentések készülnek a 1042-S formanyomtatványon?** | Csak **a Egyesült Államokban található, az adó-visszatartásnak minősülő vásárlóknak** szóló eladások bejelentése.  Az összes többi értékesítés nem tekinthető bemutatandónak. | 
| **Miért kaptam három példányban ugyanazt az űrlapot, 1042-S-t egy borítékban?** | Az IRS-szabályoknak három példányban kell megadniuk az űrlapot:<br/><br/>– Az egyik a címzett rekordjaihoz<br/>-Az egyik a Egyesült Államok szövetségi adóbevallásának bejelentése (ha van ilyen)<br/>-Az egyik a Egyesült Államok állapotának visszaadására vonatkozó adóbevallás (ha van ilyen) |

> [!NOTE]
> Ha további kérdései vagy az **IRS-adózási űrlapokkal** kapcsolatos problémái vannak, lépjen a [Súgó és támogatás](https://partner.microsoft.com/dashboard/support/) elemre a partner Center irányítópultján. A Microsoft nem tud válaszolni az adott adózási körülményekkel kapcsolatos kérdésekre; ezekre a kérdésekre kérjük, kérjen tanácsot az adó szakembertől.

## <a name="next-steps"></a>Következő lépések

- [Fizetés fogadása a kereskedelmi piactéren](marketplace-get-paid.md)
