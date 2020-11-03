---
title: Ösztönzők – Ügyfelek társításával kapcsolatos problémák
description: Ismerje meg, hogy miként lehet olyan problémákat kezelni, amelyek felmerülhetnek a Recording (CPOR) Customer-társítások használatakor.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: ab2c26cf097d6212375382cadd9ac5f4f80b5c2a
ms.sourcegitcommit: b91119c587d37b4ed36dda00c2b0b1946beb3012
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/17/2020
ms.locfileid: "92528386"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>A Recording (CPOR) ügyfél-társítások által jelentett problémák

**A következőkre vonatkozik:**

- Partnerközpont

**Megfelelő szerepkörök:**

- Számlázási adminisztrátor
- Globális rendszergazda
- Ösztönzők rendszergazdája

Az alábbi tartalom segítséget nyújt az ügyfelekkel való együttműködés során felmerülő problémák megoldásában.

## <a name="domain-tenant-mismatch"></a>Tartomány – bérlői eltérés

A Record (CPOR) Association jogcím-adatforgalom igénylése során a rendszer kérni fogja, hogy adja meg az ügyfél bérlői AZONOSÍTÓját és altartományát. Ha hibaüzenetet kap arról, hogy nem egyeznek, forduljon az ügyfélhez, és győződjön meg arról, hogy a megfelelő adatokkal rendelkezik.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Előfizetési hibák a CPOR társítási jogcím folyamatában

A CPOR-társítási jogcím folyamata során előfordulhat, hogy meg kell adnia egy előfizetést egy olyan termékhez, amelyet a Business Applications (Dynamics 365) használatával szeretne igényelni. Azt javasoljuk, hogy az előfizetést, mert dinamikusan ellenőrzi, hogy a termék és az előfizetés az igényelt bérlőhöz tartozik-e. Azt is ellenőrzi, hogy az előfizetés aktív/türelmi állapotban van-e.

Ha a hibaüzenetet kapja, több okból is előfordulhat:

- A kiválasztott termék nem létezik az ügyfél bérlőjén
- A megadott előfizetés nem a Dynamics számára
- A megadott előfizetés egy CSP-hez tartozik
- Az ügyfél még nem aktiválta/kiépítte az adott előfizetéshez tartozó termékeket
- Az előfizetést már igényelték
- A megadott azonosító nem előfizetés-azonosító

Ha kérdése van az előfizetés pontosságával kapcsolatban, használja az ügyfelet, és győződjön meg arról, hogy az előfizetés helyes, és hogy a megfelelő bérlői azonosítót használta.

Ha ez az útvonal nem oldotta meg a problémát, forduljon az [ügyfélszolgálathoz](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Ha előfizetések lesznek elérhetők a jogcím számára

Az előfizetés igénylése esetén hibaüzenetet kap, ha még nincs kiépítve az előfizetés. Az ügyfélnek több lépésből kell kiválasztania ahhoz, hogy az előfizetés elérhetővé váljon a CPOR platform számára, és elérhetővé tegye azt a jogcím számára. Ha az előfizetés igénylése során hibaüzenetet kap, forduljon az ügyfélhez, és győződjön meg arról, hogy a szolgáltatás ki lett építve, és hogy a megfelelő előfizetés helyes. Ha már megtette ezt az útvonalat, forduljon az [ügyfélszolgálathoz](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Melyik tevékenységet válasszam?

A CPOR-igénylési platform lehetővé teszi a Business Applications és Microsoft 365 megoldási területekhez kapcsolódó CPOR-társítási jogcímeket. Az egyes megoldási területeken érvényes tevékenységek a következők. A leírások alapján válassza ki a megfelelő tevékenységet, hogy a későbbiekben ne kelljen visszaigényelni. A helytelen tevékenység igénylése kimaradt jogosultságokat és ösztönző bevételeket eredményezhet.


| Megoldásterület | Tevékenység | Alkalmazható a következőre: |
| ------ | ----------- | ----------- |
| Üzleti alkalmazások      | Vásárlás előtti   | Válassza ki, hogy befolyásolta-e egy jogosult termék megvásárlását, és az értékesítés előtti ösztönzőket szeretné alkalmazni. Ez a lehetőség csak akkor érvényes, ha az ügyfél mennyiségi licencszerződésen vagy a web-Directen keresztül vásárolta meg ezeket a termékeket. |
|    |  Használat  | Válassza ki, hogy elvégezte-e a megfelelő számítási feladatok elfogadását és használatát, és alkalmazni kívánja a használati ösztönzőket. Ez a lehetőség csak akkor érvényes, ha az ügyfél mennyiségi licencszerződésen vagy a web-Directen keresztül vásárolta meg ezeket a termékeket. |
|    | Bevételi társítás   | Akkor válassza ki, ha befolyásolta a jogosult termék kiválasztását üzleti befolyásként. Ez a lehetőség csak bevételi társításra szolgál, nem pedig ösztönző kifizetésekre. Ez a lehetőség csak akkor érvényes, ha az ügyfél mennyiségi licencszerződésen vagy a web-Directen keresztül vásárolta meg ezeket a termékeket.   |
| Microsoft 365   | Használat   | Válassza ki, hogy elvégezte-e a megfelelő számítási feladatok elfogadását és használatát, és alkalmazni kívánja a használati ösztönzőket. |

## <a name="which-mpn-do-i-choose"></a>Melyik MPN-t válasszam?

A CPOR társítási jogcím folyamata során a rendszer arra kéri, hogy válasszon egy vállalat MPN-t, amelyet a végfelhasználónál igényelt munkához kell társítani. Előfordulhat, hogy a vállalata számos MPNs rendelkezik, amelyek közül néhányat ösztönző programokban lehet regisztrálni, és mások is társítva vannak, például a FRP-FastTrack. Az CPOR-hozzárendelési jogcím folyamata azonosítja, hogy mely MPNs legyenek regisztrálva egy ösztönző programban, de nem fogja tudni, hogy az MPN egy adott partner típusú. Fontos, hogy kiválassza a megfelelő MPN-t, hogy a jövőben ne kelljen visszaigényelni. A helytelen MPN-jogcím kimaradó jogosultságot és ösztönző bevételt eredményezhet.

Ha nem tudja, melyik MPN-t használja, forduljon a globális rendszergazdához.

Ha a használni kívánt MPN-t nem regisztrálja, akkor az [ösztönzők áttekintése lapon](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) kezelheti ezt a lehetőséget (bejelentkezés szükséges).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Termék kiválasztása és előfizetés beléptetése

Egy Dynamics-termék igénylése és jóváhagyása esetén a partner maga is megtekintheti az előfizetés AZONOSÍTÓját a CPOR társítási jogcímben. Ha ezt az előfizetést igényli, aktív vagy türelmi állapotban van, de előfordulhat, hogy az előfizetés véget ér, és az új előfizetéseket külön CPOR-társítási jogcímben kell igényelni.

## <a name="competing-claims"></a>Versengő jogcímek

Ha olyan CPOR-társítási jogcímet hoz létre egy ügyfélhez és azokhoz a termékhez, amely már egy másik partnerhez van társítva, akkor a jogcímek választottbírósági eljárással fognak járni:

1. Miután létrehoz egy új ügyféltársítást, a Microsoft a pontosság érdekében ellenőrzi a társítás adatait és a végrehajtás igazolását.

2. Ha Ön és egy másik partner ugyanazt az ügyfelet és terméket/munkaterhelést igényli, a Microsoft áttekinti a partnereknek a végrehajtási dokumentációt, hogy meghatározzák, melyik partnert kell jóváhagyni.

3. Mindkét partnertől további információkat is kérhetnek, ami késleltetheti a társulási kérelem feldolgozását.

4. Az CPOR-társítási jogcímet továbbra is öt munkanapon belül felülvizsgáljuk, bár az állapotuk hosszabb ideig is megmarad a _felülvizsgálat alatt_ . Ez a forgatókönyv akkor fordulhat elő, ha a Microsoft együttműködik a terméket/munkaterhelést jelenleg birtokló partnerrel. Ha ez a helyzet, értesítést kap a jogcím megjegyzések szakaszában. 

>[!IMPORTANT]
>Ha további információra van szükségünk a CPOR-hozzárendelési igazolás végrehajtásának (PoE) ellenőrzéséhez, a CPOR-társítási jogcím megjegyzései szakaszban fogunk kapcsolatba lépni Önnel.

## <a name="next-steps"></a>Következő lépések

- [Az ösztönzők első lépései](incentives-get-started-intro.md)
