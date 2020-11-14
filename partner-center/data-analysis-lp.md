---
title: Analytics használata az előfizetési elemzésekhez
ms.topic: article
ms.date: 11/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan használhatja az elemzést a partner Centerben az üzleti tevékenység jobb megismeréséhez, valamint arról, hogy az ügyfelek hogyan használják a megvásárolt licenceket.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19e7cf9442660a24d36b5f7c20fab156fdc0d59a
ms.sourcegitcommit: bfc9e6f6476766cf10ba714f03ca2e96560003b1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2020
ms.locfileid: "94626072"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a>Az előfizetés bevételének megismerése az Analytics használatával

**Megfelelő szerepkörök**

- Globális rendszergazda
- MPN-partner rendszergazdája

Egy CSP-vállalkozás fejlesztésének megtervezéséhez fontos tudni, hogy az ügyfelek hogyan használják a Microsoft termékeit. Több lehetőség is van az adatok összegyűjtésére a partner Centerben, és a vállalaton és az ügyfeleken is gyűjthet adatokat a megvásárolt licencek használatával. Ha a CSP Direct modellben van, lehetősége van arra is, hogy a Power BI a partner Center Analytics alkalmazást is telepítse és használja a további adatok összegyűjtéséhez.

## <a name="access-to-the-subscription-analytics"></a>Hozzáférés az előfizetés-elemzéshez

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/home).
1. A partner Center menüjéből válassza az **elemzés** , majd az **előfizetés-elemzés** lehetőséget.

1. A jelenleg tizenkét hónapos CSP-bevétel megjelenik az oldal tetején.

:::image type="content" source="images/analytics/subscription1.png" alt-text="Előfizetés képernyő":::

## <a name="trailing-twelve-month-ttm-csp-revenue"></a>Záró Twelve-Month (TTM) CSP-bevétel

A 12 hónapos CSP-bevétel nyomon követő befizetése a felhőalapú megoldás szolgáltatói programjának bevételét jelenti USD-ben a partner globális fiók szintjén. A rendszer minden hónap 8. napján frissíti az adatmennyiséget, hogy az előző hónap végéig a tizenkét hónapos bevételt jelenítse meg. Például szeptember 9-én a 2020-es rögzített időszakra vonatkozóan láthatja az TTM-t az 2020 augusztus 2019-ig terjedő időszakban.

A partner Centerben megjelenő bevétel tizenkét hónapos rögzített időtartamra van kiszámítva, és nem módosítható rövidebb időszakra.

A partner helyének fiókja szintjén megjelenő bevétel részletezésének megtekintéséhez:

- Válassza ki a "részletek letöltése" hivatkozást, és töltsön le egy. TSV fájlt, amely megjeleníti a TTM bevételét az összes helyen.

>[!NOTE] 
>Előfordulhat, hogy a. TSV fájlban lévő MPN-azonosítók között az egyes TTM-bevételi számok összegzése nagyobb, mint a TTM megjelenő teljes bevétel. Ennek az az oka, hogy a bevételt a letöltött fájlban több partneri kapcsolattal rendelkező előfizetések esetében kétszer is megszámoljuk.

## <a name="subscription-summary"></a>Előfizetés összefoglalása

A képernyő alsó fele az előfizetések összegzését jeleníti meg. Használja a következő szűrőket a szükséges előfizetés részleteinek megtekintéséhez:  

1. **Időtartam** : dönthet úgy, hogy megtekinti az előfizetés összegzését 

- 30D – elmúlt 30 nap
- 3M – elmúlt 3 hónap
- 6M – elmúlt 6 hónap
- 12M – elmúlt 12 hónap

2. **Terméktípus** :
 
- Office 365
- Microsoft 365
- Dynamics 365
- EMS

Ezen szűrők alkalmazása nem befolyásolja a jelentés elején található TTM bevételi mérőszámot.


 
## <a name="next-steps"></a>További lépések

- [Elemezze, hogy az ügyfelek hogyan használják a megvásárolt licenceket](increasing-adoption-and-satisfaction.md)  
- [Az ügyféltevékenységi naplók megtekintése](activity-logs.md)
- [A Power BIhez készült partner Center Analytics-alkalmazás](power-bi-app-for-direct-partners.md)






