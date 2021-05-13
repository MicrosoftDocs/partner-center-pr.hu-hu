---
title: Az ösztönző és a program részleteinek megtekintése
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Ezekkel az oldalakkal megtekintheti és kezelheti Ösztönzőprogram állapotát
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 798fde02b87e8f8105dad6d00c32b050fb90097e
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818745"
---
# <a name="view-your-incentives-program-details"></a>Az ösztönzőprogram részleteinek megtekintése

**Megfelelő szerepkörök:** Ösztönzők rendszergazdai | Ösztönzők felhasználói | Globális rendszergazdai | MPN-partner rendszergazdája

Ez a cikk a **Saját ösztönzők áttekintése** oldalt ismerteti, amely az ösztönző programok általános állapotát, valamint az egyes programok állapotát mutatja be minden helyen. Emellett a különböző regisztrációs állapotokat is megadja.

>[!NOTE]
>További információ az ösztönzőkről és az ösztönző funkciókról a Partnerközpont: [Partnerbefektetések és](https://partner.microsoft.com/membership/partner-incentives) ösztönzők (bejelentkezés szükséges).

## <a name="access-the-incentives-overview-page"></a>Az ösztönzők áttekintő oldalának elérése

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard).
1. Válassza **az Ösztönzők,** majd **az Áttekintés lehetőséget** a menüből.
1. A bevételek és kifizetések összegzése az oldal tetején, a további részletek pedig az alatta lévő táblázatban tekinthetők meg. A kapcsolódó táblázatot rendezheti, csoportosíthatja és kibonthatja:

   - Az oszlop alapján való rendezéshez válassza ki az oszlop nevét.
   - A program szerint való csoportosításhoz válassza a **táblázat fölötti Program** szerint lapot.
   - A hely alapján való csoportosításhoz válassza a **táblázat fölötti Hely** szerint lapot.
   - Egy adott csoporton belüli regisztrációk további részleteinek megtekintéséhez válassza a sávnyíl szimbólumot egy adott sor végén. Ez a sávnyíl kibontja a nézetet.
1. Ha további művelet szükséges a programban történő regisztráláshoz, akkor ez az információ az **Állapot** oszlopban jelenik meg. Ebben az esetben kattintson a sávnyíl szimbólumra a szükséges lépések megtekintéséhez.

## <a name="enrollment-status"></a>A regisztráció állapota

Az alábbi táblázat az Állapot oszlopban látható különböző regisztrációs **állapotokat ismerteti.**

| **Állapot**         | **Akkor jelenik meg, ha** |
|:------------------------------------|:------------------|
| Szükséges beavatkozás  | A partner elfogadta az ösztönzőprogramba való regisztrációra vonatkozó meghívót, de előfordulhat, hogy frissítenie kell a banki vagy adóinformációkat. A következő **lépésekért** vagy hivatkozásokért tekintse meg a Műveletek szükséges oszlopot a banki vagy adóinformációk frissítéséhez a Partnerközpont. |
| Megszűnt  | Az adott ösztönzőprogram már nem érhető el az ösztönzőrendszerben. |
| Regisztrálva  | Az összes adó- és banki adat ellenőrizve lett. A partnernek nincs szüksége további regisztrációs műveletre. |
| Regisztráció  | A felhasználó nem ösztönző-rendszergazda, és a  regisztráció a Szükséges művelet vagy **a beléptetési államok érvényességének érvényesítésében** van.|
| Inaktív /nem alkalmas | Előfordulhat, hogy az ösztönzőprogram jelenleg nincs megnyitva a regisztrációhoz, vagy a partner nem felel meg az aktuális regisztrációs vagy újraregisztrációs jogosultságnak. <br><br> Ha az állapot **Nem alkalmazható,** akkor a partner nem felel meg a program jelenlegi jogosultsági követelményeinek; A regisztrációs állapot alatt található **Jogosultsági** követelmények megtekintése hivatkozásra kattintva láthatja a jogosultsági követelményeket és a követelmények közül melyik teljesült. <br><br> Az ösztönzőprogramban  már nem aktív virtuális szervezeti (VORG) vagy partner globális fiók (PGA) regisztrációk inaktív állapotát is láthatja.  |
| Meghívott  | Új ösztönzőprogram-regisztrációs meghívó lett elküldve a partnernek, de a partner még nem indította el a regisztrációs folyamatot. Az Actions required **(Műveletek szükségesek)** oszlopban a következő lépések és a kapcsolódó hivatkozások megjelenik.  |
| Regisztráció érvényességének igénylése  | A partner már kitöltötte vagy frissítette egy új vagy meglévő regisztráció banki és adóinformációját, és arra vár, hogy a Microsoft érvényesítse ezt az információt. Az ellenőrzési folyamat **során** a regisztráció ellenőrzése akár 48 óráig is megjelenhet.  |

## <a name="see-your-payment-information"></a>Fizetési adatok

Válassza a képernyő jobb felső sarkában található kifizetési ikont a különböző összegzések eléréséhez:

- Tranzakcióelőzmények
- Kifizetések
- Adatok exportálása

:::image type="content" source="images/payouts/payout-overview.png" alt-text="A kifizetés ikont mutatja be a Partnerközpont jobb felső sarkában":::

Ez az információ az ösztönző teljes bevételeit és kifizetéseit tartalmazza az ösztönző programokba történő regisztrálás óta. Ezen a lapon a bevételeket és a kifizetéseket hely vagy program alapján rendezve is megtekintheti, emellett minden további műveletet láthat, amelyre egy adott helyen lévő programban való regisztrációhoz szüksége lehet. 

A Partner [Payout API-val](https://apidocs.microsoft.com/services/partnerpayouts) közvetlenül is csatlakozhat a kifizetési tranzakciókhoz és a fizetési adatokhoz, és beszerezheti őket. További [információ: Kifizetési](payout-statement.md) kimutatások.

## <a name="next-steps"></a>Következő lépések

- [Kifizetési utasítások](payout-statement.md)
