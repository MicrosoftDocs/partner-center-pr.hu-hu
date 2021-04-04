---
title: Vállalatok migrálása a PMC-ből a partneri központba
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Mi a teendő, ha több vállalatot telepít át a partner Membership Centerből (PMC) a partner Centerbe, és összevonja őket egy partner globális fiókba.
author: parthpandyaMSFT
ms.author: ParthP
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0787056d8d32db4a2975f7488bb65141c240ff88
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132655"
---
# <a name="moving-multiple-companies-to-partner-center-from-partner-membership-center-pmc"></a>Több vállalat áthelyezése a partneri központba a Partner tagsági központból (PMC)

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói felügyeleti rendszergazda
- Felügyeleti ügynök
- Értékesítési ügynök

Amikor a vállalati fiókot a PMC-ről a Partnerközpontba helyezi, előfordulhat, hogy több fiókot helyez át. A partner Centerben ezek a fiókok egyetlen globális fiókba (PGA) lesznek összevonva. Az elsőként áthelyezett fiók a partner globális fiók lesz, és az összes további fiók az első fiókba lesz összevonva. Indítsa el az áthelyezést a vállalati központ PMC-fiókjával. További információkért lásd: [útmutató a PMC-ról a partneri központba való áttelepítéshez](guide-to-migration.md) , vagy tekintse meg ezt a rövid videós [többhelyes fiókot egyszerűen](https://vimeo.com/290335248).

## <a name="move-your-additional-accounts-into-partner-center"></a>További fiókok áthelyezése a fiókpartner-központba

Mivel egy vállalati fiókot már áthelyezett a partneri központba, a bejelentkezéskor tudatja Önnel, hogy melyik fiók már szerepel a partner Centerben.

Ha azt tapasztalja, hogy az áttelepítés után nem a megfelelő vállalati fiók lett megjelölve jogi üzleti tevékenységként, módosíthatja a megjelölést.

1. Lépjen a **partner profiljához.**

2. Győződjön meg arról, hogy a jogi személyként kijelölni kívánt hely szerepel a helyek listáján. Ha nem, adja hozzá.

3. Válassza a **jogi üzleti profil frissítése lehetőséget.**

4. Válassza ki az üzleti és a régiót, és mentse.

:::image type="content" source="images/migration/accountwithus.png" alt-text="Meglévő fiók":::

## <a name="your-company-has-an-account-in-partner-center"></a>A vállalata rendelkezik fiókkal a partner Centerben

Ekkor megjelenik a meglévő fiókja, és egy megjegyzés arról, hogy a vállalat adatai (az aktuálisan bejelentkezett fiók) összevonva lesznek ebbe a fiókba.

:::image type="content" source="images/migration/existingaccount2.png" alt-text="Fiók a partner Centerben":::

Ezen a képernyőn megtekintheti a partner Centerben már létrehozott meglévő fiók (név és címe) adatait, valamint az elsődleges névjegy részleteit.

Válassza a **Folytatás** lehetőséget.

## <a name="what-happens-during-consolidation-of-accounts"></a>Mi történik a fiókok összevonása során

- Ezen a képernyőn semmilyen adat nem módosítható.

- A (jelenleg áthelyezett) PMC-fiók összevonva lesz ebbe a meglévő fiókba

- A HQ és a PMC összes helye a meglévő partner Center-fiókba kerül át helyként

- A konszolidáció befejezése után a fiók adatait a meglévő partner Center-fiókban található helyként fogja látni.

- Az összes MPN-azonosító megőrződik a konszolidáció során

- A meglévő kompetenciák (arany/ezüst), a vásárlások (MAPS/Gold/Silver) és a kapcsolódó előnyök megmaradnak a konszolidáció során

- A munkahelyi e-mail-AZONOSÍTÓval bejelentkezett felhasználó automatikusan MPN-rendszergazdaként és rendszergazdai fiókként lesz hozzáadva a meglévő partner Center-fiókhoz, hogy a fiók szükség szerint felügyelhető legyen.

## <a name="review-your-company-information"></a>A vállalati adatok áttekintése

Ellenőrizze a vállalat adatait, és szükség esetén szerkessze azokat.  A rendszer ezeket a részleteket fogja használni a fiókjának a partner központba való átlépéséhez, ezért ügyeljen arra, hogy a részletek helyesek legyenek.

A részletek a PMC adatain alapulnak, és a rendszer ellenőrzi, hogy a vállalat jogos-e.


:::image type="content" source="images/migration/review.png" alt-text="Részletek áttekintése":::

Ha az áthelyezett fiók ugyanabban az országban vagy régióban található, mint a meglévő fiók, eldöntheti, hogy szeretné-e használni ezt a helyet, vagy egy másikat hozzáadni. Ha úgy dönt, hogy más-más címeket használ, a rendszer ellenőrzi, hogy az adott címen található-e. Ha ugyanazt a lakcímet szeretné használni, akkor a rendszer a meglévő és az elsődleges kapcsolatot fogja használni.

Miután ellenőrizte/szerkesztte az információkat ezen a képernyőn, válassza a **Submit (Küldés** ) lehetőséget, és a rendszer összevonja a fiókokat.

## <a name="partner-profile"></a>Partneri profil

Amikor megtekinti a profilját, a jogi üzleti adatai (a PMC-ban ez a központ) és az összes további hely információi láthatók.

## <a name="next-steps"></a>Következő lépések

- [Áthelyezés a PMC-ből a Partnerközpontba](move-pmc-pc-map.md)
- [Felhasználói fiókok létrehozása](create-user-accounts-and-set-permissions.md)
- [Felhasználói szerepkörök és engedélyek hozzárendelése](permissions-overview.md)
- [A tagsági programok kezelése](renew-mpn-offers.md)
- [A vállalat üzleti profiljának létrehozása](create-a-marketing-profile.md)
- [Ügyfelekkel való kapcsolat az átirányítási szolgáltatásokkal](manage-leads.md)
