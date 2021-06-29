---
title: Elemzés használata az előfizetési elemzésekhez
ms.topic: article
ms.date: 11/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan használhatja a Partnerközpont, hogy jobban megértse vállalkozását, és hogy az ügyfelek hogyan használják a megvásárolt licenceket.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ae31e7d917e96763e107212a78f28bfa10acf2f4
ms.sourcegitcommit: 3ac88f7925bfe1df90e267ee5c1ee4d752ac92d4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/29/2021
ms.locfileid: "113013318"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a>Elemzések használata az előfizetés bevételével kapcsolatos további információkért

**Megfelelő szerepkörök:** Globális rendszergazdai | MPN-partneri rendszergazda

Egy CSP-vállalkozás fejlesztésének megtervezéséhez fontos tudni, hogy az ügyfelek hogyan használják a Microsoft termékeit. Számos lehetőség áll rendelkezésre az adatok gyűjtésére a Partnerközpont, és adatokat gyűjthet a vállalatról, valamint arról, hogy az ügyfelek hogyan és hogyan használják a megvásárolt licenceket. Ha Ön a közvetlen CSP-modellben van, lehetősége van telepíteni és használni a Partnerközpont adatelemzési alkalmazás a Power BI-hoz további adatok gyűjtése érdekében.

## <a name="access-to-the-subscription-analytics"></a>Hozzáférés az Előfizetési elemzéshez

1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard/home)
1. A csp-Partnerközpont válassza az **Elemzés,** majd az **Előfizetés-elemzés lehetőséget.**

1. A 12 hónapos záró CSP-bevétel az oldal tetején jelenik meg

:::image type="content" source="images/analytics/subscription1.png" alt-text="Előfizetés képernyő.":::

## <a name="trailing-twelve-month-ttm-csp-revenue"></a>Záró Twelve-Month (TTM) CSP-bevétel

A 12 hónapos CSP-bevétel a záró bevételt Felhőszolgáltató USD-ben, partner globális fiókszinten. Az adatok minden hónap első napján frissülnek, így az előző hónap utolsó tizenkettő havi bevételét jelenítik meg. 2020. szeptember 9-én például látnia kell a 2019. szeptember és 2020. augusztus között rögzített időtartamra vonatkozó TTM-et. A szoftver-előfizetések ki vannak zárva. A TTM-bevétel csak azt a jogosult bevételt fogja tükrözni, amelyre a számlákat már kifizették. 

A Partnerközpont megjelenített bevételt a rendszer 12 hónapos rögzített időszakra számítja ki, és nem módosítható rövidebb időszakra.

A bevétel részletezése a partnerhelyi fiók szintjén:

- Válassza a Részletek letöltése hivatkozást, és töltsön le egy .tsv fájlt, amely megjeleníti a TTM-bevételt az összes helyen.

>[!NOTE] 
>Úgy tűnik, hogy a .tsv fájlban az egyes TTM-bevételi számok összege több MPN-azonosítóban nagyobb, mint a pénzügyi kimutatásban látható teljes TTM-Partnerközpont. Ennek az az oka, hogy a letöltött fájlban található több partneri forrásmegjelöléssel rendelkező előfizetések bevétele kétszer is beleszámolhat.

## <a name="subscription-summary"></a>Előfizetés összegzése

A képernyő alsó felében megjelenik az előfizetések összegzése. A következő szűrőkkel tekintse meg a szükséges előfizetési adatokat:  

1. **Időtartam:** Dönthet úgy, hogy a következő előfizetés összegzését látja: 

- 30D – Az elmúlt 30 nap
- 3M – Az elmúlt 3 hónap
- 6M – Az elmúlt 6 hónap
- 12 M – Az elmúlt 12 hónap

2. **Termék típusa:**
 
- Office 365
- Microsoft 365
- Dynamics 365
- EMS

A szűrők alkalmazása nem befolyásolja a jelentés tetején található TTM bevételi metrikát.


 
## <a name="next-steps"></a>Következő lépések

- [Annak elemzése, hogy az ügyfelek hogyan használják a megvásárolt licenceket](increasing-adoption-and-satisfaction.md)  
- [Az ügyféltevékenységi naplók megtekintése](activity-logs.md)
- [Partnerközpont adatelemzési alkalmazás a Power BI-hoz](power-bi-app-for-direct-partners.md)






