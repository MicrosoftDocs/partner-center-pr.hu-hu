---
title: Ösztönzők – Ügyfelek társításával kapcsolatos problémák
description: Ismerje meg, hogyan lehet az igényelt rekordpartner (CPOR) ügyféltársításokkal kapcsolatos problémákat megoldásra.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 8f1c087911e6dd7e58182c99e2b97b7a6b2246d8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152171"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Az igényelt rekordpartner (CPOR) ügyféltársításokkal kapcsolatos problémák

**Megfelelő szerepkörök:** Számlázási rendszergazdai | Globális rendszergazdai | Ösztönzők rendszergazdája

Az alábbi tartalom segít megoldani az ügyfelek társításával kapcsolatos problémákat.

## <a name="domain-tenant-mismatch"></a>Tartomány-bérlő eltérése

A Igényelt rekordpartner (CPOR) társítási igény folyamatában meg kell adnia az ügyfél bérlőazonosítóját és altartományát. Ha olyan hibaüzenetet kap, amely szerint azok nem egyeznek, forduljon az ügyfélhez, és ellenőrizze, hogy a megfelelő adatok adatokat tartalmaznak-e.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Előfizetési hibák a CPOR társításigénylési folyamatában

Előfordulhat, hogy a CPOR társításigénylési folyamatában meg kell adnia egy előfizetést egy termékhez, amelyért a Business Applications (Dynamics 365) keresztül próbál igényelni. Azért kérjük az előfizetést, mert dinamikusan ellenőrizzük, hogy a termék és az előfizetés a igényelt bérlőhöz tartozik-e. Azt is ellenőrizzük, hogy az előfizetés aktív/türelmi állapotú-e.

Ha hibaüzenetet kap, annak több oka is lehet:

- A kiválasztott termék nem létezik az ügyfél bérlőjén
- A megadott előfizetés nem a Dynamicshoz való
- A megadott előfizetés egy CSP-hez tartozik
- Az ügyfél még nem aktiválta/kiépítte az előfizetéshez szükséges termékeket
- Az előfizetést már igényelték
- A megadott azonosító nem előfizetés-azonosító

Ha kérdése van az előfizetés pontosságával kapcsolatban, az ügyféllel együtt ellenőrizze, hogy az előfizetés helyes-e, és hogy a megfelelő bérlőazonosítót használja-e.

Ha ez az útvonal nem oldotta meg a problémát, forduljon a támogatási [szolgálathoz.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="when-subscriptions-will-be-available-to-claim"></a>Mikor lesznek igényelhető előfizetések

Ha előfizetést igényel, hibaüzenetet kap, ha az előfizetés még nem lett kiépítve. Az ügyfélnek számos lépést kell tennie ahhoz, hogy az előfizetés elérhetővé váljon, hogy a CPOR platform felvegye azt, és elérhetővé tegye azt igénylésre. Ha hibaüzenetet kap, amikor megpróbál igényelni egy előfizetést, lépjen kapcsolatba az ügyféllel, és ellenőrizze, hogy az előfizetés ki lett-e építve, és helyes-e az előfizetés, amit igényel. Ha már átveszi ezt az útvonalat, forduljon a támogatási [szolgálathoz.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="which-activity-do-i-choose"></a>Melyik tevékenységet válasszam?

A CPOR igényigény-igénylési platform lehetővé teszi a CPOR-társítási igényeket Business Applications és Microsoft 365 megoldási területekhez. Az egyes megoldási területekre vonatkozó tevékenységek alább olvashatók. Válassza ki a megfelelő tevékenységet a leírások alapján, hogy a jövőben ne kelljen visszaigényelnünk őket. A helytelen tevékenységgel való igénylés kihagyott jogosultságot és ösztönző bevételeket eredményezhet.


| Megoldásterület | Tevékenység | A(3) |
| ------ | ----------- | ----------- |
| Üzleti alkalmazások      | Előzetes értékesítések   | Válassza ki, hogy befolyásolta-e egy jogosult termék megvásárlását, és szeretne-e értékesítés előtti ösztönzőket alkalmazni. Ez a lehetőség csak akkor alkalmazható, ha az ügyfél mennyiségi licencszerződésen vagy Web Directen keresztül vásárolta meg ezeket a termékeket. |
|    |  Használat  | Válassza ki, hogy ön-e a jogosult számítási feladatok bevezetésének és használatának ösztönzése, és szeretne-e használati ösztönzőket alkalmazni. Ez a lehetőség csak akkor alkalmazható, ha az ügyfél mennyiségi licencszerződésen vagy Web Directen keresztül vásárolta meg ezeket a termékeket. |
|    | Bevétel társítása   | Válassza ki, hogy befolyásolta-e egy jogosult termék üzleti befolyásolóként való kiválasztását. Ez a lehetőség csak a bevétel társítására, az ösztönző kifizetésekre nem. Ez a lehetőség csak akkor alkalmazható, ha az ügyfél mennyiségi licencszerződésen vagy Web Directen keresztül vásárolta meg ezeket a termékeket.   |
| Microsoft 365   | Használat   | Válassza ki, hogy ön-e a jogosult számítási feladatok bevezetésének és használatának ösztönzése, és szeretne-e használati ösztönzőket alkalmazni. |

## <a name="which-mpn-do-i-choose"></a>Melyik MPN-t válasszam?

A CPOR társításigénylési folyamatában ki kell választania egy olyan vállalati MPN-t, amely ahhoz a munkához lesz társítva, amit a végfelhasználónál igényel. A vállalat számos MPN-sel is lehet, amelyek némelyike regisztrálható ösztönzőprogramokban, mások pedig egy partnertípushoz, például az FRP FastTrackhez vannak társítva. A CPOR társításigénylési folyamat azonosítja, hogy mely MPN-eket regisztrálta egy ösztönzőprogramban, de nem fogja meghatározni, hogy az adott partnertípusú MPN-e. Fontos, hogy a megfelelő MPN-t válassza, hogy a jövőben ne kelljen visszaigényelnünk. A helytelen MPN-ekkel való igénylés kihagyott jogosultságot és ösztönző bevételeket eredményezhet.

Ha nem tudja, hogy melyik MPN-t használja, lépjen kapcsolatba a globális rendszergazdával.

Ha a használni kívánt MPN nincs regisztrálva, azt az Ösztönzők áttekintése lapon kezelheti [(bejelentkezés](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) szükséges).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Termék kiválasztása vagy előfizetésbe való belépés

Dynamics-termék igénylése és jóváhagyása után a partner megtekintheti az előfizetés azonosítóját a CPOR társítási igényében. A igényléskor az előfizetés aktív vagy türelmi állapotú, de előfordulhat, hogy az előfizetés lejár, és az új előfizetéseket egy külön CPOR-társítási igényben kell igényelni.

## <a name="competing-claims"></a>Versengő jogcímek

Ha CPOR-társítási igényt hoz létre egy ügyfél és egy másik partnerhez már társított terméke(i) számára, az igény egyeztetési eljáráson fog átesni:

1. Miután létrehoz egy új ügyféltársítást, a Microsoft a pontosság érdekében ellenőrzi a társítás adatait és a végrehajtás igazolását.

2. Ha Ön és egy másik partner ugyanazt az ügyfelet és terméket/számítási feladatot követeli meg, a Microsoft áttekinti az egyes partnerek végrehajtási dokumentációját, hogy eldöntse, melyik partnert hagyja jóvá.

3. További információk kérhetőek mindkét partnertől, ami a társítási kérelem feldolgozásának késését okozhatja.

4. A CPOR társítási igényét öt munkanapon belül továbbra is  felülvizsgáljuk, bár az állapota hosszabb ideig Felülvizsgálat alatt maradhat. Ez a forgatókönyv akkor fordulhat elő, ha a Microsoft azzal a partnerrel működik együtt, aki jelenleg a termék/számítási feladat tulajdonában van. Ebben az esetben az igény megjegyzések szakaszában értesítést kap. 

>[!IMPORTANT]
>Ha további információra van szükségünk a CPOR társítási igazolásának (PoE) ellenőrzéséhez, a CPOR társítási igényekkel kapcsolatos megjegyzésekkel kapcsolatos szakaszán keresztül kapcsolatba lépünk Önnel.

## <a name="next-steps"></a>Következő lépések

- [Ismerkedés az ösztönzőkkel](incentives-get-started-intro.md)
