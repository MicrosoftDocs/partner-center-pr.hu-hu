---
title: A partner Center-bejelentések előfizetési jelentése
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, mit csinál jól, és hogyan javíthatja az ügyfelei számára eladott vagy kezelt felhőalapú előfizetésekkel kapcsolatos információkat.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 019e489b4738515639bf181591dfbc671e1b795d
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086192"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>A termék-előfizetésekről szóló jelentés a partner Center bepillantást ismertető irányítópultján érhető el

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felügyeleti ügynök
- Jelentés megjelenítője
- Executive Report Viewer

A Product Subscriptions jelentés az Ön által eladott vagy az ügyfelek számára felügyelt felhőalapú előfizetések elemzését jeleníti meg. Ez egy termékspecifikus jelentés, amely magában foglalja a felhőalapú termékekhez, például az Office 365, az Azure, a Dynamics és más szolgáltatásokhoz társított előfizetések teljesítményét.

A következő szakaszt a Product Subscriptions jelentésből tekintheti meg.

- Összefoglalás
- Az előfizetések földrajzi eloszlása
- Előfizetések hozzáadása/adatforgalom trendje
- Előfizetés eloszlása partneri helyszínek, értékesítési csatorna, SKU, partneri csatolás típusa, szegmens
- Trend előfizetési állapotok szerint
- Termékek trendje

 > [!NOTE]
 > Ez a jelentés az áttekintések irányítópultján érhető el. A jelentés megtekintéséhez hozzá kell rendelnie egy adott szerepkört a partner Centerben, például a globális rendszergazda, a fiók rendszergazdája, a jelentéskészítő vagy a Executive Report Viewer. További információ: a vállalat globális rendszergazdája. a jelentésben megadott adattípusok csak a Executive Report Viewer jogosultságokkal rendelkező felhasználók számára is elérhetők.

## <a name="summary"></a>Összefoglalás

Az összefoglalás szakasz az ügyfelek számára eladott vagy az Ön által kezelt előfizetésekhez kapcsolódó fő teljesítménymutatók (KPI-k) pillanatképét jeleníti meg.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="előfizetések jelentésének összegzése":::

Az összefoglalás egyes szakaszaival kapcsolatos további információkért lásd alább:

- Előfizetések:
  - Az Ön által eladott vagy kezelt felhőalapú termék-előfizetések aktuális száma.
  - Az előfizetések százalékos növekedése vagy elutasítása a kiválasztott dátumtartomány alatt.
  - A Micro diagram az előfizetések havi hónapját mutatja be a kiválasztott dátumtartomány során.

- Aktív előfizetések:
  - A termék telemetria alapján mért aktív használattal rendelkező felhőalapú termék-előfizetések aktuális száma. Ez kizárja az összes próba-előfizetést az Azure-előfizetések esetében.
  - Az aktív előfizetések százalékos növekedése vagy elutasítása a kiválasztott időszakban.
  - A Micro diagram az aktív előfizetések hónapról hónapra eső trendjét mutatja be a kiválasztott dátumtartomány szerint.

- Hozzáadott előfizetések:
  - A kiválasztott dátumtartomány szerint hozzáadott összes ügyfél-előfizetés (eladott vagy felügyelt). Az **aktív** vagy **megújított** állapotú új előfizetések a hozzáadott előfizetéseknek számítanak.
  - Az utolsó teljes hónapban hozzáadott előfizetések százalékos növekedése vagy csökkenése az első teljes hónaphoz képest.
  - A Micro diagram a kiválasztott időtartományban hozzáadott előfizetések havi trendjét mutatja be.

- Átadott előfizetések:
  - A kiválasztott dátumtartomány során megjelenő összes ügyfél-előfizetés. Az ebben a hónapban **felépített** vagy **felfüggesztett** állapotú előfizetések megkerülő előfizetésnek számítanak.  
  - A kijelölt időtartományban megjelenő előfizetések százalékos aránya.
  - A Micro diagram a kiválasztott dátumtartomány szerint átadott előfizetések havi trendjét mutatja be.

- Előfizetések termékek szerint: a jelenlegi előfizetések számának bontása felhőalapú termékek alapján.

## <a name="geographical-spread-of-subscriptions"></a>Az előfizetések földrajzi eloszlása

Az **előfizetések** földrajzi nézet szerint az összes előfizetés földrajzi eloszlása látható az ügyfelek piacain. A teljes előfizetés összege az eladott előfizetéseket és az aktív előfizetéseket is tartalmazza.

Az **országok/** régiók tábla száma megadja az összes olyan országot/régiót, ahol előfizetéssel rendelkezik, valamint a teljes és az aktív előfizetések országonkénti összegét.

Megkeresheti és kiválaszthatja a rács egyik országát, hogy a térképen lévő helyre nagyítson. A térképen a **Home (Kezdőlap** ) lehetőség megnyomásával visszaállíthatja az eredeti nézetet. Vigye az egérmutatót a térképen az ország összes előfizetésének és aktív előfizetésének megtekintéséhez. A rács mindkét mezője rendezhető.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="előfizetések földrajz szerint":::

## <a name="subscription-addschurns"></a>Előfizetés – Hozzáadás/adatforgalom

Ez a nézet az előfizetések trendjét mutatja be. Ezek különböző kategóriákba vannak bontva (új, meglévő, átváltott) a kiválasztott dátumtartomány esetében. Az X tengely a kiválasztott dátumtartomány hónapját jelöli. Az Y tengely az előfizetés darabszámát jelöli. Az átvett előfizetések az Y tengely negatív skáláján jelennek meg. 

A halmozott oszlopdiagram a hónap új, meglévő és átadott előfizetésének részletezését mutatja be. Az oszlopdiagram újraépíthető a megadott stack-elemek szerinti bontásban. Ehhez jelölje ki a jelmagyarázatban szereplő adott elemeket. A diagram tetején található csúszkát is használhatja egy adott időszak nagyításához.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="előfizetés-hozzáadások és-adatforgalom":::

## <a name="subscription-distribution"></a>Előfizetés eloszlása

Ez a nézet az MPN-helyekkel, az ügyfél-szegmensekkel, az értékesítési csatornával/az Azure díjszabási modellel és a kiosztási típussal (például DPOR, DAP és egyebek) kapcsolatos aktuális előfizetések részletezését mutatja be. Válassza ki a megfelelő lapokat a kategóriák szerinti bontás megtekintéséhez. Ha a tortadiagramot adott elem-kategóriák részletezésével szeretné felépíteni, válassza ki a jelmagyarázatban az elemek kategóriáit.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="előfizetés eloszlása":::

## <a name="subscription-state-distribution"></a>Előfizetés állapotának eloszlása

Ez a nézet az aktuális ügyfél-előfizetések eloszlását mutatja az előfizetés állapota vagy állapota alapján. Ez a következő előfizetési állapotokat tartalmazza: **aktív**, **Letiltva**, **kiépített**, **nyitott**, **türelmi időszakban**, **lezárt** és **mások**.

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="előfizetés állapotának eloszlása":::

## <a name="products-trend"></a>Termékek trendje

Ebben a nézetben egy sávdiagram és két tortadiagram látható. A sávdiagram a kereskedelmi termékek, például az Azure, az Office, a Dynamics stb. által lebontott előfizetések havi trendjét mutatja be.

A két tortadiagram az aktuális ügyfél-előfizetések részletezését jeleníti meg. Az első tortadiagram a termékek előfizetéseit bontja. A második tortadiagram az előfizetéseket az SKU-i vagy a csomagok alapján bontja le. Amikor kijelöl egy terméket a **Products (termékek** ) kördiagramban, a szomszédos tortadiagram megjeleníti a termék előfizetései SKU alapján történő részletezését.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="termékek trendje":::

> [!NOTE]
 > Az előfizetések száma az SKU szerint lebontva nem mindig egyezik meg az adott termékhez tartozó összes előfizetés számával. Ez akkor fordulhat elő, ha egy ügyfél több SKU-t vásárolt ugyanazzal a termék-előfizetéssel.

## <a name="next-steps"></a>Következő lépések

- További jelentések: [partner Center](partner-center-insights.md)-információk.

>[!NOTE] 
> A jelentést az elemzések irányítópultjának letöltési jelentések részéből töltheti le. [További információ](pci-download-reports.md) 
