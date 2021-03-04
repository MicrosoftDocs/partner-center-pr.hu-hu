---
title: Asztali számítógépek számának és díjszabási szintjének megkeresése
ms.topic: how-to
ms.date: 02/18/2021
description: Megtudhatja, hogyan használhatja a Channel ösztönzők platformot (CHIP) a szerződések asztalának darabszámára és díjszabására vonatkozó információk megkereséséhez.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e433b44f158c3e4cefe22027e7f7d3b845991308
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756120"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Megállapodáshoz tartozó munkaállomásszám és díjszabás megkeresése

**Megfelelő szerepkörök**

- Elsődleges kapcsolattartó vagy program rendszergazdája

Az [Explore.MS](https://www.explore.ms/) -be való bejelentkezéssel áttekintheti a szerződést, vagy letöltheti a szerződés részleteit tartalmazó fájlt az asztal darabszáma és a díj szintjén.

## <a name="to-locate-the-information"></a>Az információk megkeresése

### <a name="method-1--explorems"></a>1. módszer – Explore.ms

1. Nyissa meg a [Explore.MS](https://www.explore.ms/) az Internet Explorerben. 

>[!Note]
>Ez a függvény nem hajtható végre a Google Chrome-ban vagy a Microsoft Edge-ben.

2. Jelentkezzen be munkahelyi vagy iskolai fiókjával vagy Live ID azonosítójával.  

3. A **jelentések** mezőben válassza a **szerződések** elemet.

4. Az eredményül kapott lapon adja meg a szerződés számát a **Keresés** mezőben, majd válassza a **Select/Order Columns (oszlopok kiválasztása/rendezés**) lehetőséget.

5. Az előugró ablakban válassza ki a **szerződési asztal száma** lehetőséget az elérhető oszlopok listából, majd a jobbra mutató nyilat választva adja hozzá az oszlopot. Válassza az **OK** lehetőséget.

6. Válassza a **Keresés lehetőséget.**

7. Az eredményül kapott képernyőn görgessen végig az eredmények között, és keresse meg a **Szerződés asztal száma** oszlopot. 

8. Az asztal száma alapján határozza meg a díj szintjét az alábbi díjszabási táblázat alapján.  

| Díj szintje | Asztali számítógépek száma |
| ------ | :-----------: |
|  A | 0 – 2 399    |
|  B | 2 400 – 5 999    |
|  C | 6 000 – 14 999    |
|  T | 15000 +   |

>[!NOTE]
>A nagyvállalati ösztönző szintek az asztali vagy a felhasználók számán alapulnak (amelyik magasabb) a kereskedelmi és az állami szektor (PS) beléptetéséhez. A természetes társított asztali vagy felhasználói számokkal nem rendelkező beléptetések esetén a Microsoft az asztali számítógépek száma vagy a kapcsolódó EA felhasználói száma alapján alkalmazza az asztalokat. <br><br>Ha nincs kísérő EA, a díj szintje a beléptetés díjszabási szintjétől függ. Az üzlet díjszabási szintje a [www.Explore.MS](https://www.explore.ms/)is megtekinthető. <br><br>Ha a meglévő EA/EAS több készlettel és/vagy díjszabással rendelkezik, a Microsoft a legmagasabb szintű díjszabást/készletet fogja igénybe véve, az a szint pedig a legalacsonyabb és a legmagasabb D szint.

#### <a name="pool-and-pricing-levels"></a>Készlet és árképzési szintek

Miután a fenti lépésekkel megkereste a explore.ms a szerződés számát, válassza ki a szerződés számát. Ekkor megnyílik a szerződés részletei oldal, amely a **Szerződés összegzését** és **ajánlatait** mutatja be. Az ajánlatok szakasz a díjszabási szinteket tartalmazza.

## <a name="method-2---chip"></a>2. módszer – CHIP

1. Jelentkezzen be a CHIPre, és válassza az LSP-ösztönzők lehetőséget.

2. A **partneri fizetés összegzése** lapon válassza ki a megtekinteni kívánt jelentési hónapot, majd válassza a **számítás részletei** lehetőséget a legördülő listából az **Exportálás Excelbe**:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Program részleteinek megkeresése":::

3. Az Exportálás elindul, és megnyithatja a fájlt, vagy mentheti/mentheti a célhelyet.

4. A jelentés megnyitása után navigáljon a **DetailReport-FlatFile** lapra a bal alsó sarokban:

:::image type="content" source="images/chip/flatfile.png" alt-text="Lapos fájl letöltése":::

Most megkeresheti a J oszlopban keresett szerződési számot. a hozzárendelt asztalok száma az R oszlopban található, Agreement_DesktopCount feliratú. A jelen Szerződés díjait a "AI" címkével ellátott szinten is megerősítheti.

## <a name="next-steps"></a>Következő lépések

- [A CHIPek elérésével kapcsolatos problémák elhárítása](chip-access-trouble.md)
