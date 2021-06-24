---
title: Partnerközpont Insights – Ügyféljelentés
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megismerheti a vállalkozása javítására irányuló módszereket. Az ügyféltrendeket földrajzi hely, termék és egyéb attribútumok szerint is láthatja.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f1ec30db0d568c7477b6fba9639e6481ffecaaf5
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565525"
---
# <a name="customers-dashboard-reports-from-partner-center-insights"></a>Az Ügyfelek irányítópult-jelentései a Partnerközpont Insightsból

**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök | Jelentésmegjelenítő | Vezetői jelentésmegjelenítő

Az Ügyfelek irányítópult olyan ügyfelek adatait mutatja meg, akik megvásároltak olyan felhőalapú termékeket, mint az Office, az Azure és a Dynamics. ön által, vagy a segítségével telepítette és felügyeli ezeket a termékeket a bérlőikben. 
 
Az Ügyfelek irányítópult a következő szakaszokból áll: 

- Összefoglalás  
- Az ügyfelek földrajzi eloszlése 
- Ügyfelek hozzáadási/lemorzsolódási trendjei 
- Ügyfelek eloszlása partnerhelyek, ügyfélszegmensek, értékesítési csatorna, partnerek forrásmegjelölési típusa szerint 
- Ügyfélelosztás termék szerint 
- Az ügyfelek eloszlási trendjei partnerhelyek, ügyfélszegmensek, díjszabási modell, partnermegjelölési típus szerint 
- Aktív ügyfelek trendje 

## <a name="summary"></a>Összefoglalás

Az összefoglaló szakasz az ügyfelekkel kapcsolatos fő teljesítménymutatók (KPI-k) pillanatkép-nézetét mutatja be, például az ügyfeleket, az aktív ügyfeleket, az előfizetéseket, a hozzáadott ügyfeleket, a lemorzsolódást mutató ügyfeleket és az egyes termékekhez tartozó ügyfeleket. Az oldalszintű szűrők minden szakaszra vonatkoznak.

:::image type="content" source="images/pci/customerproduct.png" alt-text="Képernyőkép az Ügyfelek összegzése irányítópultról, amely az aktív, a közelmúltban hozzáadott, elveszett/lemorzsolódású vagy adott termék szerint hozzáadott ügyfelek sávdiagramját és számát mutatja.":::

### <a name="customers"></a>Ügyfelek

- A szervezet jelenlegi ügyfeleinek száma különböző forrásmegjelölési típusokon keresztül van társítva az összes felhőalapú termékben, például az Office-ban, az Azure-ban és a Dynamicsben. Az ügyfelek akkor számítanak bele, ha legalább egy aktív állapotú előfizetéssel rendelkezik.  
- Az ügyfelek százalékos arányának elutasítása a kiválasztott dátumtartományban 
- Mikrodiagram, amely a kiválasztott dátumtartományban található ügyfelek havi trendjét mutatja

### <a name="active-customers"></a>Aktív ügyfelek

- Az aktív termékhasználattal (például bármely felhőalapú termék aktív használatával) kapcsolatos ügyfelek aktuális száma.
- Az aktív ügyfelek százalékos növekedése vagy csökkenése a kiválasztott időszakban
- A mikrodiagram egy havi trendet mutat be, amely az aktív ügyfelek számát mutatja a kiválasztott dátumtartományban.

### <a name="customers-added"></a>Hozzáadott ügyfelek

- A kiválasztott időszakban hozzáadott összes ügyfél száma.
- A kiválasztott időszakban hozzáadott ügyfelek %-os növekedése vagy csökkenése.
- A mikrodiagram a kiválasztott dátumtartományhoz hozzáadott ügyfelek havi trendjét mutatja.

### <a name="customers-churned"></a>Lemorzsolódást eltolt ügyfelek
- A kiválasztott időszakban havonta lemorzsolódást jelző ügyfelek száma. Az ügyfél akkor minősül elveszettnek, ha nem rendelkezik egyetlen aktív állapotú előfizetéssel. 
- Az ügyfelek százalékos lemorzsolódása a kiválasztott dátumtartományban 
- A mikrodiagram egy hónapról hónapra vonatkozó trendet mutat a kiválasztott időszakban lemorzsolódást jelző ügyfelekről 
 
### <a name="customers-by-products"></a>Ügyfelek termékek szerint

- Az ügyfelek aktuális száma a különböző felhőalapú termékekben, például az Office 365-ben, az Azure-ban és a Dynamicsben.  

## <a name="geographical-spread-of-your-customers"></a>Az ügyfelek földrajzi eloszlése

Az aktuális ügyfelek, a jelenlegi aktív ügyfelek és a kiválasztott dátumtartományban újonnan hozzáadott ügyfelek száma az ügyfél országával van földrajzilag leképezve. A metrika alatt megjelenített százalékos arányok az adott ország százalékos hozzájárulását jelzik az adott metrika összegének százalékos arányában. Ha a kurzort a térkép fölé húzza, megtekintheti az adott ország összes aktív, új felhasználóját. Megkeresheti és kiválaszthatja a rács egyik országát a térkép helyének nagyításához. A térképen a Kezdőlap  gombra kattintva visszaállítható az eredeti nézet. A rács összes oszlopa rendezhető.  

:::image type="content" source="images/pci/customersgeo.png" alt-text="Képernyőkép az Partnerközpont Insights-ügyfél földrajzi hely szerint jelentésről, amely az összesített, hozzáadott és új ügyfelek listáját jeleníti meg régiónként.":::

## <a name="customer-adds-and-churns"></a>Ügyfél hozzáadása és lemorzsolódása

A kiválasztott dátumtartományra lebontott új, meglévő és lemorzsolódású ügyfelek trendje. Az X tengely a kiválasztott dátumtartomány hónapját, az Y tengely pedig az ügyfelek számát jelöli. A lemorzsolódást jelző ügyfeleket az Y tengely negatív skálája képviseli. A halmozott oszlopdiagram az új, meglévő és lemorzsolódású ügyfeleket mutatja be a hónapra. A jelmagyarázatban lévő elemek kiválasztásával újraépítheti az oszlopdiagramot adott veremelemekből. A diagram tetején található csúszkával nagyíthat egy adott időszakot. 

:::image type="content" source="images/pci/customerslost.png" alt-text="Képernyőkép az Partnerközpont Insights-ügyféljelentésről sávdiagrammal, amely az adott időszakban hozzáadott és elveszett vagy lemorzsolsolódású ügyfelek számát mutatja.":::

## <a name="customer-distribution"></a>Ügyfelek eloszlása

Az aktuális ügyfelek lebontása a Microsoft Partner Network (MPN) helye, ügyfélszegmensek, értékesítési csatorna/Azure-díjszabási modell és a forrásmegjelölés típusa szerint. Válassza ki a diagram feletti megfelelő lapokat a kategóriák szerinti lebontás megtekintéséhez. A diagramot a jelmagyarázat elemeinek kiválasztásával vagy kijelölésének kiválasztásával újraépítheti. 

## <a name="customers-by-products"></a>Ügyfelek termékek szerint

Az aktuális ügyfelek darabszámának részletezése termékek és termékkódok/csomagok szerint. Válasszon ki egy terméket a termék-lebontás tortadiagramon a mellette található, termékekkel/csomagokkal kapcsolatos lebontás megtekintéséhez.

:::image type="content" source="images/pci/customerbyprod.png" alt-text="Képernyőkép a Customers by product (Ügyfelek termék szerint) jelentésről, amely két radiális diagramot mutat – az egyik az ügyfelek termék szerinti lebontását, a másik pedig az ügyfél termékváltozat szerinti lebontását mutatja.":::

## <a name="customer-distribution-trend"></a>Ügyfélelosztási trend 

Az ügyfelek a kiválasztott dátumtartományon belül való eloszlásának havi trendje piacok, szegmensek, az MPN-helyek és az azok által megvásárolt termékek szerint. Válassza ki a megfelelő lapokat a diagramon a trend kategóriák szerint való megtekintéséhez. Az X tengely a kiválasztott dátumtartomány hónapját jelöli, az Y tengely pedig a kiválasztott kategóriához tartozó ügyfelek számát (Lap kiválasztása). Ha a kurzort a diagram oszlopai fölé húzza, megtekintheti az egyes vermek értékeinek lebontott értékeit. A diagram tetején található csúszkával nagyíthat egy adott időszakot.   

:::image type="content" source="images/pci/customerdistri.png" alt-text="Képernyőkép az Ügyfélelosztási trendjelentésről, amely piac, szegmens, partnerhely vagy termék szerint megtekinthető sávdiagramokat tartalmaz.":::

## <a name="active-customers"></a>Aktív ügyfelek

Havi trenddiagram, amely a kiválasztott dátumtartomány aktív és teljes ügyfeleit hasonlítja össze. Az oszlopok az aktív ügyfelek számát jelölik minden hónapban, a sor pedig az összes ügyfelet jelöli minden hónapban. 

:::image type="content" source="images/pci/activecustomer.png" alt-text="Képernyőkép az Partnerközpont Insights Active Customers (Aktív ügyfelek) jelentésről, amely az aktív ügyfelek idősávdiagramját mutatja.":::

## <a name="next-steps"></a>Következő lépések

További jelentésekért lásd: [Partnerközpont Insights.](partner-center-insights.md)

>[!NOTE]
> A jelentést betöltő nyers adatokat az Insights irányítópult Jelentések letöltése szakaszában töltheti le. [További információ](pci-download-reports.md) 
