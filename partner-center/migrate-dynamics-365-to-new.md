---
title: A Dynamics 365 Business Edition áttelepítése
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan mihelheti át a minősített Dynamics 365 Business Edition-ajánlatokat az újabb verziókra, mielőtt lejárnak.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151525"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>A Dynamics 365 Business Edition-ajánlatok migrálása újabb verziókba

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Rendszergazdai ügynök | Értékesítési ügynök

2019. január 1-től a Dynamics 365 Business Edition-előfizetéssel nem lehet többé megújítani ezeket az örökölt ajánlatokat; A meglévő előfizetések nem újulnak meg automatikusan a lejáratukkor. Az előfizetés részleteinek oldalán az előfizetés állapota "Lejárat [dátum] időpontban" állapotra változik az "Automatikus megújítás [dátum] időpontban" állapotra.

Az ügyfelek folytonosságának biztosítása érdekében a lejáró előfizetéseket az alább felsorolt támogatott lehetőségekre kell átemálnia. Javasoljuk, hogy az ügyfeleket az előfizetés éves záró dátuma előtt új előfizetésekbe költöztetjék, hogy elkerülje az ügyfelek szolgáltatáskimaradását.

Ha az API-t használja (CREST vagy Partnerközpont), a lejáró előfizetéseket az előfizetés záró dátumának és az automatikus megújítás = Hamis tulajdonság kiértékelével találhatja meg. A kérdéses előfizetések 2019. január 1-jén automatikus megújítás=Hamis értékre lesznek beállítva. Az ügyfeleket bármikor új csomagba költöztetheti. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>A Dynamics 365 Business Edition kiadások kivezetve

- Dynamics 365 for Finance and Operations, Business edition
- Dynamics 365 for Team Members, Business edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central – a Dynamics 365 Business Edition új ajánlata

Az új Dynamics Business Central-ajánlatokkal az ügyfelek össze is kapcsolhatják pénzügyi, értékesítési, szolgáltatási és műveleti munkájukat az üzleti folyamatok leegyszerűsítés, az ügyfél-interakciók javítása és a jobb döntések meghozatala érdekében. A Dynamics 365 Business Central felhőalapú, és csak Felhőszolgáltató (CSP) programpartnerek számára érhető el.
A Dynamics 365 Business Edition-ügyfelek 2020. június 30-ig kedvezményes áttérési díjszabást kaphatnak az új Business Central-ajánlatokhoz.

## <a name="transition-customers-to-new-product-plans"></a>Ügyfelek váltása új terméktervekre

 Ha az ügyfeleket a visszavont SKUS-król újabbakra kívánja átemeltetni, a következő lépésekre van szükség ebben a sorrendben:

- Az új előfizetés vásárlása
- Aktuális felhasználói licencek ismételt hozzárendelése
- Régi előfizetés lemondása

## <a name="purchase-the-new-plan-for-your-customer"></a>Az új csomag vásárlása az ügyfél számára

1. A **bal oldali navigációs** sávon válassza az Ügyfelek lehetőséget, majd válassza ki az új előfizetésre áthelyezni kívánt ügyfelet.
2. Válassza **az Előfizetés hozzáadása lehetőséget.**
3. Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek valamelyikét), adja meg a licencek számát, majd válassza a **Küldés lehetőséget.** 

Az ügyfél most már a régi előfizetéssel és az új előfizetéssel is rendelkezik. A következő lépés a licencek ismételt hozzárendelése az ügyfél felhasználóihoz.

1. A **bal oldali navigációs** sávon válassza az Ügyfelek lehetőséget, majd válassza ki a költözni kívánt ügyfelet.
2. Válassza **a Felhasználók és licencek lehetőséget.**
3. Egy licenc felhasználóhoz való ismételt hozzárendeléséhez jelölje ki a felhasználót, majd válassza a **Licencek kezelése lehetőséget.** 
4. A **Licencek kezelése** lapon törölje a Dynamics 365 for Sales/Customer Engagement Plan from Basic (Minősített ajánlat) licencből jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatástervet ahhoz az előfizetéshez, amelybe az ügyfél át lesz költözve. 
5. Válassza a **Küldés** lehetőséget. Ezt minden olyan felhasználóval meg kell tenni, akinek új licencre van szüksége. 

Miután áthelyezte a licenceket az új előfizetésbe, megszüntetheti a régi előfizetést. 

1. A **bal oldali navigációs** sávon válassza az Ügyfelek lehetőséget, majd válassza ki a költözni kívánt ügyfelet.
2. Az előfizetés részletei lapon állítsa a régi előfizetést Felfüggesztettre, majd **válassza** a **Küldés lehetőséget.**

A régi előfizetés most fel van függesztve, és az új előfizetés aktív. A felfüggesztett előfizetés 120 nap után automatikusan fel lesz függesztve. Az ügyfél nem jár többletköltségsel a régi előfizetésért.
