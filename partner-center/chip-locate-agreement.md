---
title: Asztalszám és díjszint megkeresése
ms.topic: how-to
ms.date: 02/18/2021
description: Megtudhatja, hogyan használhatja a Channel Incentives platformot (CHIP) egy szerződés asztalszámára és díjszintjére vonatkozó információk megkeresése érdekében.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276938"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Megállapodáshoz tartozó munkaállomásszám és díjszabás megkeresése

**Megfelelő szerepkörök:** Elsődleges kapcsolattartó vagy program-rendszergazda

Bejelentkezhet a explore.ms [a](https://www.explore.ms/) szerződés áttekintéséhez, vagy letölthet egy fájlt, amely tartalmazza az asztalok számára és a díjszintre vonatkozó szerződésadatokat.

## <a name="to-locate-the-information"></a>Az információk megkeres

### <a name="method-1--explorems"></a>1. módszer – Explore.ms

1. Nyissa [explore.ms](https://www.explore.ms/) a Internet Explorer. 

>[!Note]
>Ezt a funkciót nem hajthatja végre a Google Chrome-ban vagy Microsoft Edge.

2. Jelentkezzen be munkahelyi/iskolai fiókjával vagy élő azonosítójával.  

3. A Jelentések **mezőben** válassza a **Szerződések lehetőséget.**

4. Az eredményül kapott oldalon írja be a szerződés számát a **Keresőmezőbe,** majd válassza az **Oszlopok kijelölése/megrendelése lehetőséget.**

5. Az előugró ablakban válassza az Agreement Desktop Count (Egyezmény **asztalszáma)** lehetőséget az elérhető oszlopok listájából, majd válassza a jobbra mutató nyilat az oszlop hozzáadásához. Válassza az **OK** lehetőséget.

6. Válassza a **Keresés lehetőséget.**

7. Az eredményül kapott képernyőn görgessen végig az eredményeken, és keresse meg az **Agreement Desktop Count (Szerződés asztalszáma)** oszlopot. 

8. Az asztalok számát használva állapítsa meg a díjszintet az alábbi díjtáblában.  

| Díjszint | Asztalok száma |
| ------ | :-----------: |
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  T | 15,000+   |

>[!NOTE]
>A vállalati ösztönzőszintek a kereskedelmi és közszférában (PS) végzett regisztrációkban az asztali vagy felhasználói számon (amelyik magasabb) alapulnak. A természetes módon társított asztali vagy felhasználói számmal nem társított regisztrációk esetén a Microsoft az asztalok számát a hozzá tartozó EA asztali számítógépszáma vagy felhasználószáma alapján alkalmazza. <br><br>Ha nincs hozzá kapcsolódó EA, a díjszint a regisztráció díjszabásán alapul. Az ajánlat díjszabási szintje a következő oldalon [is www.explore.ms.](https://www.explore.ms/) <br><br>Ha a meglévő EA/EAS-on több készlet- és/vagy díjszabási szint található, a Microsoft a legmagasabb hozzárendelt díjszabási/készletszinten fizet az ösztönzőkért, és az A szint a legalacsonyabb, a D szint pedig a legmagasabb.

#### <a name="pool-and-pricing-levels"></a>Készlet- és díjszabási szintek

Miután rákeresett a szerződésszámra a explore.ms a fent ismertetett lépésekkel, válassza ki a szerződés számát. Ezzel meg fog jelenni a szerződés részleteit tartalmazó oldal, amelyen a Szerződés **összegzése** és az **Ajánlatok látható.** Az ajánlatok szakasz a tarifacsomagokat tartalmazza.

## <a name="method-2---chip"></a>2. módszer – CHIP

1. Jelentkezzen be a CHIP-be, és válassza az LSP-ösztönzők lehetőséget.

2. A Partner **fizetési összefoglalása lapon** válassza ki a megtekinteni  kívánt jelentési hónapot, majd válassza a Számítás részletei lehetőséget az Exportálás Excelbe legördülő **menüből:**

:::image type="content" source="images/chip/chiplocate.png" alt-text="Keresse meg a program részleteit.":::

3. Megnyílik az exportálás, és megnyithatja a fájlt, vagy mentheti/mentheti a célhelyre.

4. Ha a jelentés meg van nyitva, lépjen a **DetailReport-FlatFile** lapra a bal alsó sarokban:

:::image type="content" source="images/chip/flatfile.png" alt-text="Egyszerű fájl letöltése.":::

Most már rákereshet a keresett szerződésszámra a J oszlopban. A hozzárendelt asztalok számát az R oszlopban találja, amely az Agreement_DesktopCount. A szerződés díjszintjét az "AI" címkével jelölt Szint oszlopban is megerősítheti.

## <a name="next-steps"></a>Következő lépések

- [CHIP-hozzáférési problémák elhárítása](chip-access-trouble.md)
