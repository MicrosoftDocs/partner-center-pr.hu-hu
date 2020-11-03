---
title: Az elfogadás és az elégedettség fokozása
ms.topic: how-to
ms.date: 07/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan használhatók a metrikák a partner Centerben. A metrikák megmutatják, hogy az üzlet egyre növekszik-e, hogyan használják az ügyfelek a licenceket, és hol kell összpontosítaniuk a beruházásokra.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d995d72f6b5f9fb3beafff91eee7518ee999bf6c
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/04/2020
ms.locfileid: "92528126"
---
# <a name="use-metrics-in-partner-center-to-increase-adoption-and-satisfaction"></a>A partner Center metrikáinak használata az elfogadás és az elégedettség növeléséhez

**A következőkre vonatkozik**

- Partnerközpont
- Cloud Solution Provider program

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói rendszergazda
- Felügyeleti ügynök
- Értékesítési ügynök

Partnereink számos mérőszámot használnak annak felmérésére, hogy az üzletük egyre növekszik-e, és hol kell koncentrálnia a befektetésre. A partner Center segítséget nyújt arról, hogy az ügyfelek mikor és hogyan használják a megvásárolt licenceket. Ez az információ elérhető az Office-termékekhez (beleértve a OneDrive for Business szolgáltatást is, amely a SharePoint szolgáltatással együtt számít).

Az összes ügyfél adatait a Cloud Solution Provider programon keresztül tekintheti meg. Egyes ügyfelek más partnerektől vagy közvetlenül a Microsofttól vásárolhatnak licenceket. Ilyen helyzetekben a teljes licencek megjelennek az összes partner között. Ha csak a saját licenceit szeretné megtekinteni, keresse fel az ügyfél előfizetéseit.

> [!NOTE]  
> Jelenleg csak az Office 365 és a Dynamics 365 adatai jelennek meg. A későbbiekben további termékekhez is engedélyezzük az adatfeldolgozást.

## <a name="find-license-and-user-data"></a>Licenc-és felhasználói adatértékek keresése

A licenc-és felhasználói adatait egyetlen ügyfélhez vagy a portfólióhoz is megtalálhatja.

### <a name="find-license-and-user-data-for-a-single-customer"></a>Licenc-és felhasználói adatértékek keresése egyetlen ügyfél számára

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).

2. Válassza ki az **ügyfeleket** a **partner központból**

3. Válasszon egy ügyfelet.

4. Válassza ki az **ügyfél-bepillantást** .

### <a name="find-license-and-user-data-across-your-portfolio"></a>Licencek és felhasználói adatértékek keresése a portfólión belül

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).

2. Válassza az **elemzés** lehetőséget, és válassza ki a menü bármelyik analitikai lehetőségét.

3. Az üzembe helyezési és a használati adatok teljes ügyfél-készletben való letöltéséhez válassza az **Exportálás** (lefelé mutató nyíl) lehetőséget.

Terminológia:

- **Jogosultság** = az a licenc, amelyet a felhasználó használhat (nem felfüggesztette csalás vagy nem fizetés miatt, nem lett frissítve másik licencre, de a felhasználó nem törölte, stb.)

- **Aktív** = ha az előfizetett felhasználó használta a jogosultságot egy adott feladathoz az elmúlt 28 naptári napban.

- **Központi telepítés:%** = hozzárendelt licencek/eladott licencek

- **Használat%** = aktív jogosultságok/összes jogosultság

   Előfordul, hogy a (z)% a kihasználtsága (%) vagy nagyobb, mint 100%. Ennek több oka is lehet:

  - Ha az ügyfél az alkalmazottak forgalmát használta, és a licenc egy új felhasználónak lett átadva.

  - Ha az ügyfél két előfizetéssel rendelkezik egy SKU-hoz, de az egyik türelmi időszakban, letiltva vagy kiépítve van, akkor mindkét előfizetéshez tartozó jogosultságok a 28 napos időszakban is regisztrálhatják az aktív használatot, de csak egy számítanak bele a teljes összegbe.

  - Ha az ügyfél próbaverziós előfizetéssel rendelkezik, a rendszer megszámolja a tevékenységet, de az előfizetés nem számít bele a teljes jogosultságokra.

  - Ha egyes ügyfelek a Yammer jelentősen nagyobb mértékben használják, mint amennyit a licencük jogosult, akkor az adatvesztést jelentősen elferdítheti.

## <a name="next-steps"></a>Következő lépések

Ha sok segítséget és útmutatást szeretne feltenni, a fiókban lévő bevezetési számok alacsonyak, vagy ha értékesítési lehetőségeket keres, érdemes fontolóra vennie a tanfolyamokat. Ha megtanítja ügyfeleinek, hogyan használják jobban a megvásárolt felhőalapú megoldási szoftvereket, nagyobb valószínűséggel fog növekedni a termelékenység és az elégedettség, valamint a támogatási igények csökkenése.

### <a name="considering-how-to-improve-customer-adoption-and-usage---a-couple-scenarios"></a>Az ügyfelek bevezetésének és használatának javítása – néhány forgatókönyv

**Probléma** : a felhasználó bevezetési sebessége alacsony, és számos licenc nincs használatban.

**Mit érdemes figyelembe venni** : Előfordulhat, hogy az ügyfelek nem értik a szoftver által megadható értéket. Segítségre van szükségük annak megtervezésében, hogy milyen módokon tudnák beépíteni őket a mai napig a már folyamatban lévő feladatok egyszerűsítése vagy az új típusú termelékenység lehetővé tétele érdekében.

**Mit kell kipróbálni** : esettanulmányok, felhasználói visszajelzések konkrét forgatókönyvekről, oktatóanyag-Blogokról vagy videókról.

**Probléma** : a Súgó és útmutató kérdéseire nagy mennyiségű támogatási hívás áll rendelkezésre.

**Mit érdemes figyelembe venni** : az ügyfelek a szoftver, a termék verziója vagy a feladataik számára újak lehetnek.

**Mi a kipróbálás** : az ügyfelek általános szakértelmének növelésére, valamint az ügyfelek számára elérhető önkiszolgáló lehetőségek támogatására szolgáló kettős stratégiát is használhat.

Érdemes lehet újratervezni a támogatási webhelyét, hogy a támogatási kapcsolattartási adatain kívül az ügyfél önkiszolgáló [támogatásában](customer-self-support.md) leírt önkiszolgáló lehetőségeket is tartalmazza.

