---
title: Microsoft-termékek kipróbálása ügyfelek számára
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Az ügyfelek 30 napig kipróbálhatják a Microsoft-előfizetési termékeket. Regisztráljon ezekre az ingyenes próbaverziókra a katalógusban, ahogy számos online szolgáltatások.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d6fda82464b9abc30714798a2ee3999d8f93db5
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151134"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>A Microsoft-termékek 30 napos, ingyenes próbaverziója az ügyfeleknek

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Értékesítési ügynök

Az új Microsoft-termékek bevezetésének jó módja, ha 30 napos ingyenes próbaverziót kínál. A katalógusban található próbaverziókra úgy regisztrálhat, mint sok online szolgáltatások. Minden partner részt vehet.

## <a name="available-trial-offers"></a>Elérhető próbaverziós ajánlatok

Az összes függőben lévő próbaverziós ajánlatot megtalálja az Ügyfél **oldalon.** Ez az oldal felsorolja az összes előfizetést, beleértve az ingyenes próbaverziókat és a fizetős előfizetéseket. (Ez a funkció Kínában jelenleg nem érhető el.)

Minden ügyfél egy ingyenes próbaverzióra jogosult minden elérhető ajánlathoz. Kaphatnak például egy ingyenes próbaverziót az Microsoft 365 Business Standardhoz, és egy ingyenes próbaverziót az Office 365 E3-hoz. Ha azonban az ügyfél már az ajánlat tulajdonában van, nem használhat ingyenes próbaverziót ehhez az ajánlathoz.

### <a name="available-products"></a>Elérhető termékek

Az ingyenes próbaverziók a legátfogóbb és legnépszerűbb, licesen alapuló ajánlatokhoz érhetők el. Az új próbaverziós ajánlatok havi rendszerességgel is bevezetve lehetnek.

A partnerek a havi árlistán találhatják meg a próbaverziókat a díjszabási és **ajánlati** oldalon a Partnerközpont. A próbaverziós ajánlatok árlistán a Másodlagos licenctípus oszlopban megjelenik a **"TRIAL"** (PRÓBAVERZIÓ).

Jelenleg nincsenek ingyenes **próbaverziók** kormányzati, oktatási vagy kiegészítő ajánlatokhoz.

## <a name="licenses-for-free-trial-offers"></a>Licencek ingyenes próbaverziós ajánlatokhoz

Minden ingyenes próbaverzió 25 licencet biztosít. Ezt a számot nem módosíthatja a próbaverzió során. Az ingyenes próbaverzióban nem adhat hozzá és nem távolíthat el licenceket. Miután a próbaverziót fizetős előfizetésre konvertálta, további licenceket adhat hozzá az előfizetéshez.

A próbaverziós licenceket ugyanúgy kell hozzárendelni a felhasználókhoz, mint a fizetős szolgáltatási licenceket.

## <a name="sign-customers-up-for-trials"></a>Ügyfelek regisztrációja próbaverzióra

Szerezze be az ügyfél próbaverzióját a Partnerközpont:

1. A **termék** értékesítésének Partnerközpont **katalógust.** 
2. A katalógus Számlázási **gyakoriság beállításában** válassza a **Próbaverziós ajánlat lehetőséget.** Ez lehetővé teszi, hogy csak az ingyenes próbaverziók jelenjenek meg, és letiltsa a nem ingyenes ajánlatokat. A próbaverziók a katalógus **Próbaverziók** lapján fognak ni.
3. Válassza ki a kínálni kívánt ingyenes próbaverziót, majd kattintson a **küldés gombra.** Minden próbaverzió 30 napig tart, amely alatt nem kell fizetni. A próbaverzió során bármikor átválthatja fizetős előfizetésre.

## <a name="converting-trials-to-paid-subscriptions"></a>Próbaverziók konvertálása fizetős előfizetésre

Az ingyenes próbaverziót a rendszer nem konvertálja automatikusan fizetős előfizetésre. 30 nap után az ingyenes próbaverziót fizetős előfizetésre kell konvertálni, különben [lejár.](#expiring-offers) Az ingyenes próbaverziók nem bővíthetők.

A próbaverziót önnek kell fizetős előfizetésre konvertálni. Ezt az [api-k használatával Partnerközpont](#convert-trials-using-partner-center) [vagy a Partnerközpont API-kon keresztül.](#convert-trials-using-apis)

> [!NOTE]
> A Felhőszolgáltató (CSP) program ingyenes próbaverziói nem konvertálhatók másik programbérlőre (például EA, Nyílt vagy MOSP).

### <a name="convert-trials-using-partner-center"></a>Próbaverziók konvertálása a Partnerközpont

A próbaverziókat fizetős előfizetésekké konvertálhatja az Partnerközpont:

1. Kattintson az ügyfél előfizetési oldalára, és válassza az ingyenes próbaverziót.
2. Válassza **a Próbaverzió konvertálása fizetős előfizetésre lehetőséget.**
3. Adja meg a kívánt licencmennyiséget és számlázási gyakoriságot, majd válassza az **Alkalmaz lehetőséget.**
4. A fizetős előfizetés számlázása az átváltási dátummal kezdődik, és az előfizetés automatikusan megújul az átváltási dátumtól 12 hónappal. 

### <a name="convert-trials-using-apis"></a>Próbaverziók konvertálása API-k használatával

Előfordulhat, hogy módosítania kell az API-kat, hogy igazodni tudjanak az ingyenes próbaverzió fizetős előfizetésre való átalakításához. További információt a következő fejlesztői dokumentációban talál:

- [Próbaverziós előfizetés átalakítása fizetőssé](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [A próbaverzió átalakításával kapcsolatos ajánlatok listájának lekérése](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Próbaverziók átalakítás nélkül

Nem minden próbaverzió alakítható át fizetős előfizetésre. A partnerek olyan próbaverziót használhatnak, amely a lejárati dátumig nem rendelkezik konverzióval. A partnerek a próbaverziós ajánlattal azonos szolgáltatásokat támogató, kompatibilis ajánlatokat vásárolhatnak.  Ezt a próbaidőszak lejárta előtt kell tenni, hogy az újonnan megvásárolt ajánlatok szolgáltatásai igazodnak a próbaverzió szolgáltatásaihoz. 

|**Próbaverzió**   |**Kompatibilis kisvállalati ajánlatok**   |**Kompatibilis nagyvállalati ajánlatok**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|A Microsoft Teams kereskedelmi felhő (felhasználó által kezdeményezett) próbaverziója   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (korábban F1), Office 365 nagyvállalati verzió (E1, E3 és E5), Microsoft 365 F1/F3, Microsoft 365 Nagyvállalati verzió (E3)   |

>[!NOTE]
>A fenti ajánlatok hasonló szolgáltatási csomagokkal és hasonló funkciókkal rendelkezik, de az ajánlatok között lehetnek különbségek.

### <a name="expiring-offers"></a>Lejáró ajánlatok

A lejáró ajánlatokról nem kap értesítést. A jövőbeli lejárati dátumok nyomon követéséhez használja az ügyfélnézetet a Partnerközpont API lekérdezése segítségével. Célszerű rendszeresen figyelni ezeket a dátumokat, hogy a döntési ponthoz közeledve megteheti a megfelelő követő műveleteket az ügyfelekkel.

A próbaidőszak lejárta után a próbaidőszakba bejelentkezni próbáló ügyfél lejárati üzenetet fog látni. Az adatok tárolása azonban az adatmegőrzési szabványoknak megfelelően történt. Miután ugyanazokkal a szolgáltatás csomagokkal vásárolt egy új előfizetést, az ügyfél adatai ismét elérhetők lesznek az újonnan aktivált előfizetésből.

## <a name="billing"></a>Számlázás

Az éves számlázás és az ingyenes próbaverziók ugyanazok a szuverén felhőkben és a nyilvános felhőkben. Az egyetlen különbség az indításkor elérhető próbaverziós SKUs.

## <a name="billing-for-free-trials"></a>Ingyenes próbaverziók számlázása

Az ingyenes próbaverziók havi és éves számlázású előfizetések esetén is használhatók. Kiválaszthatja a számlázási gyakoriságot, amikor a próbaverziót fizetős előfizetésre konvertálja.

Az előfizetés kezdő dátuma az átalakítási dátumon alapul. Ha az ingyenes próbaverziót éves számlázású fizetős ajánlatra konvertálják, az előfizetés megújításának dátuma 12 hónap lesz az átváltási dátumtól. Ha az ingyenes próbaverziót havi számlázású fizetős ajánlatra váltja át, az előfizetés megújításának dátuma 12 hónap lesz a számlázási dátumtól az átváltási dátum után.

### <a name="invoices"></a>Számlák

A számlán vagy a licencalapú egyeztetési fájlban nem megjelenik az ingyenes próbaverziók listája. Az ingyenes próbaverziók csak akkor jelennek meg a számlán és a licencalapú egyeztetési fájlban, ha az ingyenes próbaverziót fizetős előfizetésre konvertálta. Az átalakított előfizetés ugyanúgy jelenik meg, mint bármely új előfizetés.

### <a name="incentives"></a>Ösztönzők

Az ingyenes próbaverziók nem befolyásolják az ösztönzőket.

## <a name="support"></a>Támogatás

Az ingyenes próbaverziókra vonatkozó támogatásért küldjön szolgáltatáskérést a Partnerközpont.