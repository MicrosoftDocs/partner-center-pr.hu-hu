---
title: Microsoft-termékek kipróbálása az ügyfelek számára
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Az ügyfelek 30 napig kipróbálhatják a Microsoft előfizetési termékeit. Regisztráljon az ingyenes próbaverzióra a katalógusban, akárcsak sok más online szolgáltatások.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a51504a5e560f8a8041c448c3e5d9e7f0cfdae07
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528471"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>30 napos ingyenes próbaverziók a Microsoft-termékekhez

**A következőkre vonatkozik**

- Partnerközpont

**Megfelelő szerepkörök**
-   Globális rendszergazda 
-   Felhasználói rendszergazda
-   Értékesítési ügynök

Az ügyfelek új Microsoft-termékekhez való bevezetésének jó módja, ha 30 napos ingyenes próbaverziót kínál. A katalógus próbaverzióit ugyanúgy regisztrálhat, mint sok más online szolgáltatások. Minden partner részt vehet.

## <a name="available-trial-offers"></a>Elérhető próbaverziós ajánlatok

Az összes függőben lévő próbaverziós ajánlatot megtalálhatja az **ügyfél** oldalán. Ezen az oldalon az összes előfizetés szerepel, beleértve az ingyenes próbaverziókat és a fizetős előfizetéseket. (Ez a szolgáltatás jelenleg nem érhető el Kínában.)

Minden ügyfél egy ingyenes próbaverzióra jogosult minden elérhető ajánlathoz. Például beszerezhetnek egy ingyenes próbaverziót Microsoft 365 Vállalati verzió standard és egy ingyenes próbaverzióra az Office 365 E3-hoz. Ha azonban az ügyfél már rendelkezik az ajánlattal, nem használhat ingyenes próbaverziót az ajánlathoz.

### <a name="available-products"></a>Elérhető termékek

Az ingyenes próbaverziók a legátfogóbb és legnépszerűbb licesen-alapú ajánlatokhoz érhetők el. Az új próbaverziós ajánlatokat havi rendszerességgel lehet bevezetni.

A partnerek a partner központ **díjszabás és ajánlatok** lapján a havi árlista keretében kereshetnek próbaverziókat. A próbaverziós ajánlatok a **másodlagos licenc típusa** oszlopban a "próbaverzió" szerepelnek.

Jelenleg nincsenek **ingyenes próbaverziók** kormányzati ajánlatokhoz, oktatási ajánlatokhoz vagy kiegészítő ajánlatokhoz.

## <a name="licenses-for-free-trial-offers"></a>Licencek ingyenes próbaverziós ajánlatokhoz

Az összes ingyenes próbaverzió 25 licencet biztosít. Ez a szám nem módosítható a próbaverzióban. Az ingyenes próbaverzióban nem adhat hozzá és nem távolíthat el licenceket. A próbaverzió fizetett előfizetésre való konvertálása után további licenceket adhat hozzá az előfizetéshez.

A próbaverziós licenceket ugyanúgy kell hozzárendelni a felhasználókhoz, mint a fizetős szolgáltatások licence.

## <a name="sign-customers-up-for-trials"></a>Ügyfelek regisztrálása próbaverzióra

Próbaverzió beszerzése az ügyfélnek a partner Centerben:

1. A partner Centerben **válassza a** **katalógus** lehetőséget. 
2. A katalógusban, a **Számlázási gyakoriság** listából válassza a **próbaverziós ajánlat lehetőséget** . Ez lehetővé teszi, hogy csak az ingyenes kísérletek megjelenjenek és letiltsák a nem ingyenes egyéb ajánlatokat. A próbaverziók a katalógus **próbaverziók** lapján jelennek meg.
3. Válassza ki az ajánlathoz használni kívánt ingyenes próbaverziót, majd kattintson a **Submit (Küldés** ) gombra. Az összes próbaverzió 30 napig tart, amíg nem számlázunk. A próbaverzióban bármikor átalakíthatja a fizetős előfizetést is.

## <a name="converting-trials-to-paid-subscriptions"></a>Próbaverziók konvertálása fizetős előfizetésekre

Az ingyenes próbaverziót a rendszer nem konvertálja automatikusan fizetős előfizetésre. Harminc nap elteltével egy ingyenes próbaverziót kell konvertálni egy fizetős előfizetésre, vagy [lejár](#expiring-offers). Az ingyenes próbaverziókat nem lehet kiterjeszteni.

A próbaverziót a fizetős előfizetésbe kell alakítania. Ezt [a partner Center](#convert-trials-using-partner-center) vagy [a partner Center API](#convert-trials-using-apis)-k segítségével teheti meg.

> [!NOTE]
> A Cloud Solution Provider (CSP) programhoz tartozó ingyenes próbaverziók nem alakíthatók át másik programbeli bérlőre (például EA, Open vagy MOSP).

### <a name="convert-trials-using-partner-center"></a>Próbaverziók konvertálása a partner Center használatával

A próbaverziókat fizetős előfizetésekre is konvertálhatja a partner Center használatával:

1. Lépjen az ügyfél előfizetése oldalra, és válassza ki az ingyenes próbaverziót.
2. Válassza **a próbaverzió konvertálása fizetős előfizetésre** lehetőséget.
3. Adja meg a kívánt licenc mennyiségét és a számlázási gyakoriságot, majd kattintson az **alkalmaz** gombra.
4. A fizetős előfizetés számlázása az átalakítás dátumától kezdődik, és az előfizetés az átalakítás dátumától számítva tizenkét hónappal meghosszabbítja az előfizetést. 

### <a name="convert-trials-using-apis"></a>Kísérletek konvertálása API-k használatával

Előfordulhat, hogy módosítania kell az API-kat, hogy az ingyenes próbaverziót egy fizetős előfizetésre konvertálja. További információkért tekintse meg a következő fejlesztői dokumentációt:

- [Próbaverziós előfizetés átalakítása fizetős verzióra](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [A próbaverziós konvertálási ajánlatok listájának beolvasása](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Konverzió nélküli próbaverziók

Nem minden próbaverzió konvertálható fizetős előfizetésre. A partnerek olyan próbaverziót használhatnak, amely nem rendelkezik konverzióval a lejárati dátumig. A partnerek olyan kompatibilis ajánlatokat is vásárolhatnak, amelyek ugyanazt a szolgáltatást támogatják, mint a próbaverziós ajánlat.  Ezt a próbaidőszak lejárta előtt kell elvégezni, hogy az újonnan megvásárolt ajánlatok szolgáltatásait a próbaverzió szolgáltatásaihoz igazítsa. 

|**Próba**   |**Kompatibilis kisméretű üzleti ajánlatok**   |**Kompatibilis nagyvállalati ajánlatok**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Microsoft Teams – kereskedelmi felhő (felhasználó által kezdeményezett) próbaverzió   |Alapszintű, Microsoft 365 Vállalati verzió standard, Microsoft 365 Vállalati verzió Premium Microsoft 365 Vállalati verzió   | F3 (korábban F1), Office 365 vállalati (E1, E3 és E5), M365 F1/F3, M365 Enterprise (E3)   |

>[!NOTE]
>A fenti ajánlat hasonló szolgáltatásokkal rendelkezik, mint a hasonló funkciókkal, azonban lehetséges, hogy az ajánlatok között eltérések állnak fenn.

### <a name="expiring-offers"></a>Lejáró ajánlatok

A lejárati ajánlatokat nem fogja értesíteni. A közelgő lejárati dátumokat a partner központ ügyfél nézetében vagy az API lekérdezésével követheti nyomon. Érdemes gyakran figyelni ezeket a dátumokat, hogy a megfelelő követő műveleteket hajtsa végre az ügyfelekkel a döntési pontokhoz közeledve.

A próbaverzió lejártát követően egy lejárati üzenet jelenik meg, amely a próbaverzióba való bejelentkezést kísérli meg. Az adatok tárolása azonban az adatmegőrzési szabályokkal összhangban történik. Miután megvásárolt egy új előfizetést ugyanazzal a szolgáltatási csomaggal, az ügyfél adatai az újonnan aktivált előfizetésből is elérhetők.

## <a name="billing"></a>Számlázás

Az éves számlázási és ingyenes próbaverziók megegyeznek a szuverén felhőkben és a nyilvános felhőben. Az egyetlen különbség az indításkor elérhető próbaverziós SKU.

## <a name="billing-for-free-trials"></a>Ingyenes próbaverziók számlázása

Az ingyenes próbaverziók havi és éves díj ellenében is felhasználhatók. Ha a próbaverziót fizetős előfizetésre alakítja át, akkor kiválaszthatja a számlázási gyakoriságot.

Az előfizetés kezdő dátuma az átalakítás dátumától függ. Ha az ingyenes próbaverziót az éves számlázással rendelkező fizetős ajánlatra konvertáljuk, az előfizetés megújításának dátuma tizenkét hónap lesz az átalakítás dátumától számítva. Ha az ingyenes próbaverziót havi számlázással rendelkező fizetős ajánlatra konvertáljuk, az előfizetés megújításának dátuma tizenkét hónap lesz az átalakítás dátumát követő számlázási dátumtól számítva.

### <a name="invoices"></a>Számlák

A számlán vagy a licenc-alapú egyeztetési fájlban felsorolt ingyenes próbaverziók nem jelennek meg. Az ingyenes próbaverziók csak akkor jelennek meg a számlán és a licencelésen alapuló egyeztetési fájlban, ha az ingyenes próbaidőszakot egy fizetős előfizetésre konvertálja. Az átalakított előfizetés ugyanúgy fog megjelenni, mint bármely új előfizetés.

### <a name="incentives"></a>Ösztönzők

Az ingyenes próbaverziók nem érintik az ösztönzőket.

## <a name="support"></a>Támogatás

Az ingyenes próbaverziók támogatásához küldje el a szolgáltatási kérelmet a partner centeren keresztül.