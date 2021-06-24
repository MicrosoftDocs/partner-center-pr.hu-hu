---
title: Partnerközpont – Power BI jelentés
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Itt láthatja, hogy mit csinál jól, és hol javíthatja az Power BI értékesítésre vagy az ügyfelek számára kezelhető előfizetések használatára vonatkozóan.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 75aa86ebc768b9d6d252a29eb84aef97ab99ab0c
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565338"
---
# <a name="power-bi-usage-report-available-from-the-partner-center-insights-dashboard"></a>Power BI a Partnerközpont Insights irányítópultról elérhető használati jelentés

**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök | Jelentésmegjelenítő | Vezetői jelentésmegjelenítő

A Power BI jelentés használati adatokat biztosít az ügyfelek számára értékesített Power BI microsoftos előfizetések használati adatait. Az alábbi szakaszokat a használati Power BI megtekintheti.

- Összefoglalás
- Power BI földrajzi hely szerint
- Power BI termékváltozat szerint
- Előfizetések teljesítménye
- Power BI eloszlása

 > [!NOTE]
 > Ez a jelentés az Insights irányítópulton érhető el. A jelentés megtekintéséhez hozzá kell rendelnie egy adott szerepkört a Partnerközpont, például globális rendszergazda, fiók-rendszergazda, jelentésmegjelenítő vagy vezetői jelentésmegjelenítő. További információért tekintse meg a vállalat globális rendszergazdáját. A jelentés bizonyos adattípusai csak a Vezetői jelentésmegjelenítő jogosultsággal rendelkező felhasználók számára is elérhetők lehetnek.

## <a name="summary"></a>Összefoglalás

Az összefoglaló szakasz az ügyfelek számára értékesített vagy Power BI előfizetésekkel kapcsolatos fő mutatók pillanatkép-nézetét mutatja be. 

- Elérhető helyek: A kiválasztott időszakban eladott licencek teljes száma.

   A Mikrodiagram a rendelkezésre álló helyek számát mutatja a kiválasztott dátumtartományra vonatkozó havi trenddel.

- Hozzárendelt helyek: A kiválasztott időszakban hozzárendelt licencek teljes száma.

   A Mikrodiagram a kiválasztott dátumtartományban a hozzárendelt helyek számát ábrázoló havi trendet mutatja.

- Aktív helyek: Azon licencek teljes száma, amelyek használatban voltak a kiválasztott időszakban. 

   A Mikrodiagram a havi aktív helyek havi trendjét mutatja a kiválasztott időszakra vonatkozóan.

- Aktív használat %: Az aktív helyek teljes száma a rendelkezésre álló helyek százalékos arányában kifejezve a kiválasztott időkerethez. 

   A Mikrodiagram az aktív használat százalékos arányának havi trendjét mutatja a kiválasztott időszakra vonatkozóan.

:::image type="content" source="images/pci/pci-pbi-usage-summary.png" alt-text="Power BI összegzése.":::

## <a name="power-bi-usage-by-geography"></a>Power BI földrajzi hely szerint

A **Power BI földrajzi hely** szerinti használat az elérhető és az aktív helyek eloszlását ábrázolja az ügyfél országa szerint. A térképen a világosabb színek alacsonyabb értékeket, a sötétebbek pedig magasabb értékeket képviselnek. A ráközelítéshez kereshet és kiválaszthat egy országot a rácsban.

A **Number of countries/region (Országok/régiók** száma) táblázat az összes országot/régiót mutatja, ahol az Azure használati eseményei létrejönnek.

Megkeresheti és kiválaszthatja a rács egyik országát a térkép helyének nagyításához. A térkép **Kezdőlap** lehetőségének kiválasztásával visszaállítja az eredeti nézetet.

:::image type="content" source="images/pci/pci-pbi-usage-geography.png" alt-text="Power BI földrajzi hely szerint.":::

## <a name="power-bi-usage-by-sku"></a>Power BI termékváltozat szerint

A Power BI termékváltozatonkénti használati adatok a rendelkezésre álló, az aktív és a hozzárendelt helyek termékváltozatonkénti havi trendjét ábrázolják.

:::image type="content" source="images/pci/pci-pbi-usage-sku.png" alt-text="Power BI termékváltozat szerint.":::

## <a name="subscriptions-performance"></a>Előfizetések teljesítménye

Az Előfizetések teljesítménye az aktív használat havi trendjét jeleníti meg ügyfél-előfizetésenként. Az első 100 ügyfél számlás bevétel szerint adatai megjelennek a táblázatban, és bármely ügyfelet megkeresheti, vagy letöltheti a nyers adatokat az összes előfizetés részleteinek megtekintéséhez.

:::image type="content" source="images/pci/pci-pbi-usage-subscription.png" alt-text="Power BI az előfizetés teljesítményét.":::

## <a name="power-bi-usage-distribution"></a>Power BI eloszlása

A Power BI eloszlása a rendelkezésre álló helyek, az aktív és a hozzárendelt helyek SKUs szerinti bontását ábrázolja.

:::image type="content" source="images/pci/pci-pbi-usage-distribution.png" alt-text="Power BI eloszlása.":::

## <a name="next-steps"></a>Következő lépések

- További jelentésekért lásd: [Partnerközpont Insights.](partner-center-insights.md)

- A jelentést betöltő nyers adatokat az Insights irányítópult Jelentések letöltése szakaszában töltheti le. [További információ](pci-download-reports.md) 
