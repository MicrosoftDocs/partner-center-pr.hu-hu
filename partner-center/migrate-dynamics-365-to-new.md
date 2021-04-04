---
title: A Dynamics 365 Business Edition migrálása
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan telepíthet át minősített Dynamics 365 Business Edition-ajánlatokat újabb verzióra a lejárat előtt.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132638"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>A Dynamics 365 Business Edition-ajánlatok migrálása újabb verziókba

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói felügyeleti rendszergazda
- Felügyeleti ügynök
- Értékesítési ügynök

2019. január 1-től a Dynamics 365 Business Edition-előfizetésekkel rendelkező ügyfelek már nem újítják meg ezeket az örökölt ajánlatokat; a meglévő előfizetések lejáratakor a rendszer nem újítja meg automatikusan. Az előfizetés részleteit tartalmazó lapon az előfizetés állapota "lejár [date]" értékre változik a "automatikusan megújítva [date]" állapotból.

Az ügyfelek folytonosságának biztosítása érdekében az alább felsorolt támogatott lehetőségekre kell áttérnie a lejáró előfizetésekkel. Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára.

Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejárati előfizetéseket az előfizetés befejezési dátumának és az automatikus megújítás = hamis tulajdonságnak a kiértékelésével érheti el. A kérdéses előfizetések az automatikus megújítás = false értékre lesznek állítva 2019 január 1-jén. Az ügyfeleket bármikor át lehet helyezni egy új csomagba. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>A Dynamics 365 üzleti kiadása kivonult

- Dynamics 365 for Finance and Operations, Business Edition
- Dynamics 365 for Team Members, Business Edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central – a Dynamics 365 Business Edition új ajánlatai

Az új Dynamics Business Central-ajánlatokkal ügyfelei az üzleti folyamatok egyszerűsítése, az ügyfelek közötti interakciók és a jobb döntések meghozatala érdekében összekapcsolhatják pénzügyi, értékesítési, szolgáltatási és üzemeltetési műveleteit. A Dynamics 365 Business Central felhőalapú és elérhető a Cloud Solution Provider (CSP) program partnerein keresztül.
A Dynamics 365 Business Edition-ügyfelek kedvezményes áttérési díjszabást kaphatnak az új Business Central-ajánlatokhoz, 2020. június 30-ig.

## <a name="transition-customers-to-new-product-plans"></a>Ügyfelek átváltása új termékekre

 A kivont SKU-ügyfelek újabb verzióra való áthelyezéséhez a következő lépések szükségesek ebben a sorrendben:

- Az új előfizetés megvásárlása
- Aktuális felhasználói licencek újbóli társítása
- Régi előfizetés megszakítása

## <a name="purchase-the-new-plan-for-your-customer"></a>Az új csomag megvásárlása az ügyfél számára

1. Válassza a bal oldali NAV- **ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, amelyet át szeretne helyezni az új előfizetésbe.
2. Válassza az **előfizetés hozzáadása** lehetőséget.
3. Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikét), adja meg a licencek számát, majd válassza a **Küldés** lehetőséget. 

Az ügyfél most már rendelkezik a régi és az új előfizetéssel is. A következő lépés a licencek ismételt kiosztása az ügyfél felhasználói számára.

1. Válassza ki az **ügyfelek** lehetőséget a bal oldali navigációs listából, majd válassza ki az áthelyezni kívánt ügyfelet.
2. Válassza **a felhasználók és licencek** lehetőséget.
3. Ha licencet szeretne hozzárendelni egy felhasználóhoz, válassza ki a felhasználót, majd válassza a **licencek kezelése** lehetőséget. 
4. A **licencek kezelése** lapon törölje a Dynamics 365 for Sales/Customer engagement-tervet az alapszintű (minősített ajánlat) licencből jelölőnégyzetből, és válasszon ki egy új szolgáltatási csomagot ahhoz az előfizetéshez, amelyet az ügyfél áthelyez. 
5. Válassza a **Küldés** lehetőséget. Ezt minden olyan felhasználónak el kell végeznie, akinek új licencre van szüksége. 

Miután áthelyezte a licenceket az új előfizetésre, megszakíthatja a régi előfizetést. 

1. Válassza ki az **ügyfelek** lehetőséget a bal oldali navigációs listából, majd válassza ki az áthelyezni kívánt ügyfelet.
2. Az előfizetés részletei lapon állítsa a régi előfizetést **felfüggesztve** értékre, és válassza a **Küldés** lehetőséget.

A régi előfizetés már fel van függesztve, és az új előfizetés aktív. A felfüggesztett előfizetés 120 nap elteltével automatikusan kiépítve lesz. Az ügyfél a régi előfizetéshez nem jár további költségekkel.
