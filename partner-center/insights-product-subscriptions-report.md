---
title: Partnerközpont Elemzések jelentés
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Itt láthatja, hogy mit tesz jól, és hol fejlesztheti tovább az ügyfelek számára értékesít vagy felügyelni képes felhőalapú előfizetéseket.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a1ce0e75817376b5cf1996a56f416acc4bcbd0f3
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376688"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Az irányítópulton elérhető termék-Partnerközpont Elemzések jelentés

**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök | Jelentésmegjelenítő | Vezetői jelentésmegjelenítő

A Product Subscriptions (Termék-előfizetések) jelentés elemzéseket biztosít az Ön által eladott vagy az ügyfelek számára ön által felügyelt felhőalapú előfizetésekkel kapcsolatban. Ez egy termékspecifikus jelentés, amely olyan felhőalapú termékekhez társított előfizetések teljesítményét tartalmazza, mint Office 365, az Azure, a Dynamics stb.

Az alábbi szakaszokat a Termék-előfizetések jelentésből lehet megtekinteni.

- Összefoglalás
- Az előfizetések földrajzi eloszlése
- Előfizetések hozzáadási/lemorzsolódási trendje
- Előfizetések eloszlása partnerhelyek, értékesítési csatorna, termékkódok, partner csatolási típusa, szegmens szerint
- Trend előfizetési államok szerint
- Termékek trendje

 > [!NOTE]
 > Ez a jelentés az irányítópult Elemzések érhető el. A jelentés megtekintéséhez hozzá kell rendelnie egy adott szerepkört a Partnerközpont, például globális rendszergazda, fiók-rendszergazda, jelentésmegjelenítő vagy vezetői jelentésmegjelenítő. További információért tekintse meg a vállalat globális rendszergazdáját. A jelentés bizonyos adattípusai csak a Vezetői jelentésmegjelenítő jogosultsággal rendelkező felhasználók számára is elérhetők lehetnek.

## <a name="summary"></a>Összefoglalás

Az összefoglaló szakasz az ügyfelek számára eladott vagy kezelt előfizetésekkel kapcsolatos fő teljesítménymutatók (KPI-k) pillanatkép-nézetét mutatja be.  

:::image type="content" source="images/insights/sub-report-summary.png" alt-text="előfizetések jelentés összegzése.":::

Az összefoglalás egyes szakaszokkal kapcsolatos további információkért lásd alább:

- Előfizetések:
  - Az Ön által eladott vagy kezelt felhőalapú termék-előfizetések aktuális száma.
  - Előfizetések százalékos növekedése vagy elutasítása a kiválasztott dátumtartományban.
  - A Mikrodiagram a kiválasztott dátumtartományban az előfizetések számát ábrázoló havi trendet mutatja.

- Aktív előfizetések:
  - A felhőalapú termék-előfizetések aktuális száma, termék-telemetria alapján mért aktív használattal. Ez kizárja az Azure-előfizetések összes próbaverziós előfizetését.
  - Az aktív előfizetések százalékos növekedése vagy csökkenése a kiválasztott időszakban.
  - A Mikrodiagram az aktív előfizetések havi trendjét mutatja a kiválasztott dátumtartományban.

- Hozzáadott előfizetések:
  - Az Ön által a kiválasztott dátumtartományban hozzáadott (eladott vagy felügyelt) összes ügyfél-előfizetés. Az aktív **vagy** **megújított** állapotban lévő új előfizetések előfizetésekként vannak megszámadva.
  - Az elmúlt teljes hónapban hozzáadott előfizetések százalékos növekedése vagy csökkenése az első teljes hónaphoz képest.
  - A Mikrodiagram a kiválasztott dátumtartományhoz hozzáadott előfizetések havi trendjét mutatja.

- Lemorzsolódású előfizetések:
  - Az összes ügyfél-előfizetés lemorzsolódása a kiválasztott dátumtartományban. Az ebben a hónapban **megszüntetett** vagy felfüggesztett állapotú előfizetések lemorzsolódású előfizetésnek számítanak.   
  - A kiválasztott dátumtartományban lemorzsolódást jelző előfizetések százalékos aránya.
  - A Mikrodiagram havi trendet mutat be a kiválasztott dátumtartományban lemorzsolódást jelző előfizetések között.

- Előfizetések termékek szerint: Az aktuális előfizetések száma felhőalapú termékek szerint lebontva.

## <a name="geographical-spread-of-subscriptions"></a>Az előfizetések földrajzi eloszlése

Az **Előfizetések földrajzi hely szerint nézet** az összes előfizetés földrajzi eloszlását mutatja az ügyfélpiacok szerint. A teljes előfizetési összeg az eladott és az aktív előfizetéseket is tartalmazza.

A **Number of countries/region (Országok/régiók** száma) táblázat az összes országot/régiót mutatja, ahol rendelkezik előfizetéssel, valamint az összes és aktív előfizetés országonkénti összegét.

Megkeresheti és kiválaszthatja a rács egyik országát a térkép helyének nagyításához. A térkép **Kezdőlap** lehetőségének lenyomása az eredeti nézetre való visszaállításhoz. Vigye az egérmutatót a térképre az összes előfizetés és aktív előfizetés országonkénti megtekintéséhez. A rács mindkét mezője rendezhető.

:::image type="content" source="images/insights/sub-report-sub-by-geography.png" alt-text="előfizetések földrajzi hely szerint.":::

## <a name="subscription-addschurns"></a>Előfizetések hozzáadása/lemorzsolódásai

Ez a nézet az előfizetések trendjét mutatja. Ezek különböző kategóriákra vannak bontva (Új, Meglévő, Lemorzsolódás) a kiválasztott dátumtartományhoz. Az X tengely a kiválasztott dátumtartomány hónapját jelöli. Az Y tengely az előfizetések számát jelöli. A lemorzsolódású előfizetések az Y tengely negatív skáláján vannak ábrázolva. 

A halmozott oszlopdiagram az új, meglévő és lemorzsolódásos előfizetések havi bontását mutatja be. Újraépítheti az oszlopdiagramot adott veremelemekre bontva. Válassza ki ezeket az elemeket a jelmagyarázatban. A diagram tetején található csúszkával is nagyíthat egy adott időszakot.

:::image type="content" source="images/insights/sub-report-sub-adds-churns.png" alt-text="előfizetés hozzáadása és lemorzsolódása.":::

## <a name="subscription-distribution"></a>Előfizetések eloszlása

Ez a nézet az aktuális előfizetések lebontását mutatja be a Microsoft Partner Network-helyek, az ügyfélszegmensek, az értékesítési csatorna/Azure-díjszabási modell és a forrásmegjelölés típusa szerint. A kategóriák szerinti lebontás megtekintéséhez válassza ki a megfelelő lapokat. A tortadiagram adott elemkategóriák részletezése alapján való felépítéséhez válassza ki ezeket az elemkategóriákat a jelmagyarázatban.

:::image type="content" source="images/insights/sub-report-distribution.png" alt-text="előfizetés-elosztás.":::

## <a name="subscription-state-distribution"></a>Előfizetés állapotának eloszlása

Ebben a nézetben az aktuális ügyfél-előfizetések eloszlása látható az előfizetés állapota vagy állapota szerint. Ez a következő előfizetési államokat tartalmazza: **Aktív,** **Letiltva,** **Megszüntetve,** **Open,** **InGracePeriod,** **Lezárt** és **Egyéb.**

:::image type="content" source="images/insights/sub-report-sub-states.png" alt-text="előfizetés állapotának eloszlása.":::

## <a name="products-trend"></a>Termékek trendje

Ebben a nézetben egy sávdiagram és két tortadiagram látható. A sávdiagram az előfizetések havi trendjét mutatja kereskedelmi termékek, például az Azure, a Office és a Dynamics szerint.

A két tortadiagram az aktuális ügyfél-előfizetések lebontását mutatja. Az első tortadiagram termékek szerint bontja az előfizetéseket. A második tortadiagram az előfizetéseket SKUs vagy plans szerint bontja. Amikor kiválaszt egy terméket  a Termékek tortadiagram szerinti részletezésben, a szomszédos tortadiagramon az adott termék előfizetései oszlának meg termék termékterméke szerint.

:::image type="content" source="images/insights/sub-report-prods-trend.png" alt-text="terméktrend.":::

> [!NOTE]
 > Előfordulhat, hogy az előfizetések száma termékkódok szerint van oszlva, és nem mindig egyezik meg az adott termékre vonatkozó teljes előfizetési számokkal. Ez akkor fordulhat elő, ha egy ügyfél több termékterméket vásárolt ugyanazon termék-előfizetés keretében.

## <a name="next-steps"></a>Következő lépések

- További jelentések: [Partnerközpont Elemzések.](partner-center-insights.md)

>[!NOTE] 
> A jelentést betöltő nyers adatokat az irányítópult Jelentések letöltése Elemzések töltheti le. [További információ](insights-download-reports.md) 
