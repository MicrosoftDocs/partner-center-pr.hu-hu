---
title: Az ösztönző és a program részleteinek megtekintése
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: A következő lapok segítségével megtekintheti és kezelheti az ösztönző programok állapotát
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4c4b3a9a71027f5fb02bc29566c20c214e3df371
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022808"
---
# <a name="view-your-incentives-program-details"></a>Ösztönző program részleteinek megtekintése

**Megfelelő szerepkörök**

- Ösztönző rendszergazda
- Ösztönző felhasználó
- Globális rendszergazda
- MPN-partner rendszergazdája

Ez a cikk a **saját ösztönzők áttekintése** lapot ismerteti, amely az ösztönző programok általános állapotát, valamint az egyes programok állapotát mutatja be az egyes helyeken. Emellett a regisztráció különböző állapotait is megadja.

>[!NOTE]
>További információ a fiókpartner ösztönzőkről és ösztönző funkcióiról: [partner Investments and ösztönzők](https://partner.microsoft.com/membership/partner-incentives) (bejelentkezés szükséges).

## <a name="access-the-incentives-overview-page"></a>Az ösztönzők áttekintése oldal elérése

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard).
1. Válassza az **ösztönzők**, majd az **Áttekintés** lehetőséget a menüből.
1. A bevételek és kifizetések összegzése az oldal tetején, a további részletek pedig az alatta lévő táblázatban tekinthetők meg. A csatolt táblázatot is rendezheti, csoportosíthatja és kiterjesztheti:

   - Az oszlop szerinti rendezéshez válassza ki az oszlop nevét.
   - A program szerinti csoportosításhoz válassza a tábla fölötti **program** fület.
   - A hely szerinti csoportosításhoz válassza a tábla fölötti **hely** fület.
   - Egy adott csoporton belüli beléptetések részleteinek megtekintéséhez válassza ki a Chevron szimbólumot az adott sor végén. Ez a Chevron kibővíti a nézetet.
1. Ha további művelet szükséges a programban történő regisztráláshoz, akkor ez az információ az **Állapot** oszlopban jelenik meg. Ebben az esetben kattintson a sávnyíl szimbólumra a szükséges lépések megtekintéséhez.

## <a name="enrollment-status"></a>A regisztráció állapota

Az alábbi táblázat az **állapot** oszlopban látható különböző beléptetési állapotokat ismerteti.

| **Állapot**         | **Akkor jelenik meg, ha** |
|:------------------------------------|:------------------|
| Szükséges beavatkozás  | A partner elfogadta a beléptetési meghívást egy ösztönző programban, de előfordulhat, hogy frissítenie kell a banki vagy adózási adatokat. Tekintse meg a **szükséges műveletek** oszlopot a következő lépésekhez, illetve a banki vagy adózási információk a partner Centerben való frissítéséhez kapcsolódó hivatkozásokat. |
| Megszűnt  | Az ösztönző rendszer már nem kínálja fel a konkrét ösztönző programot. |
| Regisztrálva  | Az összes adózási és banki információ ellenőrzése megtörtént. A partner nem igényel további regisztrációs műveletet. |
| Regisztráció  | A felhasználó nem ösztönző rendszergazda, és a regisztráció a **szükséges művelet** vagy a **beléptetési** állapotok ellenőrzése folyamatban van.|
| Inaktív/nem jogosult | Előfordulhat, hogy az ösztönző program jelenleg nem nyílik meg a regisztrációhoz, vagy a partner nem felel meg a beléptetésre vagy az újbóli regisztrációra vonatkozó jelenlegi jogosultságnak. <br><br> Ha az állapot nem **jogosult**, akkor a partner nem felel meg a programra vonatkozó jelenlegi jogosultsági követelményeknek; a regisztráció állapota alatt **látható támogathatósági követelmények hivatkozásra kattintva megtekintheti** a jogosultsági követelményeket, valamint a követelmények teljesülését. <br><br> Előfordulhat, **hogy a virtuális** szervezet (VORG) vagy a partner globális fiók (PGA) regisztrációjának inaktív állapota is megjelenhet, amelyek már nem aktívak az ösztönző programban.  |
| Meghívott  | A rendszer elküldte az új ösztönző program beléptetési meghívását a partnernek, de a partner még nem indította el a beléptetési folyamatot. A szomszédos, **szükséges műveletek** oszlop a következő lépéseket és a kapcsolódó hivatkozásokat jeleníti meg.  |
| Regisztráció ellenőrzése  | A partner már befejezte vagy frissítette a banki és adózási adatokat egy új vagy meglévő regisztrációhoz, és arra vár, hogy a Microsoft érvényesítse ezeket az információkat. Az érvényesítési folyamat során a **beléptetés ellenőrzése** akár 48 óráig is megjelenhet.  |

## <a name="see-your-payment-information"></a>Tekintse meg a fizetési adatokat

A különböző összefoglalók eléréséhez válassza a képernyő jobb felső sarkában található kifizetés ikont:

- Tranzakciók előzményei
- Kifizetések
- Adatok exportálása

:::image type="content" source="images/payouts/payout-overview.png" alt-text="A partner Center portál jobb felső sarkában látható kifizetési ikon ábrázolása":::

Ez az információ az ösztönző teljes bevételeit és kifizetéseit tartalmazza az ösztönző programokba történő regisztrálás óta. Ezen a lapon a bevételeket és a kifizetéseket hely vagy program alapján rendezve is megtekintheti, emellett minden további műveletet láthat, amelyre egy adott helyen lévő programban való regisztrációhoz szüksége lehet. 

A [partneri kifizetési API](https://apidocs.microsoft.com/services/partnerpayouts) -val a kifizetési tranzakciók és a fizetési műveletek közvetlen összekapcsolására és beszerzésére is lehetősége van. További információért lásd a [kifizetési utasítások](payout-statement.md) című témakört.

## <a name="next-steps"></a>Következő lépések

- [Kifizetési utasítások](payout-statement.md)
