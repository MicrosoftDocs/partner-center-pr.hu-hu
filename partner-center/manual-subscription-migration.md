---
title: Minősített Dynamics 365-előfizetések migrálása
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan telepítheti át a minősített, alapszintű Dynamics 365-előfizetéseket egy új előfizetésre a meglévő előfizetések lejárta előtt.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/17/2020
ms.locfileid: "92528007"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>A Dynamics 365 és a Customer Engagement Plan migrálása az Alapszintű szolgáltatásról (arra jogosult ajánlatokról) újabb verziókra

**A következőkre vonatkozik**

-  Partnerközpont

**Megfelelő szerepkörök**
-   Globális rendszergazda
-   Felhasználói rendszergazda
-   Felügyeleti ügynök
-   Értékesítési ügynök

Az alapszintű (minősített ajánlatok) előfizetések által kínált, a Dynamics 365 for Sales/Customer engagements csomaggal rendelkező ügyfelek a továbbiakban nem tudják megújítani ezeket a régi ajánlatokat: 2019. január 1-től a meglévő előfizetések lejáratakor a rendszer nem újítja meg automatikusan. Az előfizetés részleteit tartalmazó lapon az előfizetés állapota "lejár [date]" értékre változik a "automatikusan megújítva [date]" állapotból. 

Az ügyfelek folytonosságának biztosítása érdekében az alább felsorolt támogatott lehetőségekre kell áttérnie a lejáró előfizetésekkel. Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára.

Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejárati előfizetéseket az előfizetés befejezési dátumának és az automatikus megújítás = hamis tulajdonságnak a kiértékelésével érheti el. A kérdéses előfizetések az automatikus megújítás = false értékre lesznek állítva, január 1-jén 2019. Az ügyfeleket bármikor át lehet helyezni egy új csomagba. 

### <a name="the-dynamics-365-offers-being-retired"></a>A Dynamics 365-ajánlatok kivonulnak

- Dynamics 365 for Sales Enterprise Edition CRMOL alapszintű (minősített ajánlat)
- Dynamics 365 for Sales Enterprise Edition CRMOL alapszintű (minősített ajánlat) oktatóknak
- Dynamics 365 for Sales Enterprise Edition CRMOL alapszintű (minősített ajánlat) diákoknak
- Dynamics 365 for Sales Enterprise Edition (kormányzati díjszabás) CRMOL alapszintű (minősített ajánlat)
- Dynamics 365 for Sales Enterprise Edition, SA for CRM Basic (minősített ajánlat)
- Dynamics 365 for Sales Enterprise Edition, SA for CRM alapszintű (minősített ajánlat) oktatóknak
- Dynamics 365 for Sales Enterprise Edition SA for CRM Basic (minősített ajánlat) diákoknak
- Dynamics 365 for Sales Enterprise Edition (kormányzati díjszabás) az SA-től a CRM alapszintű verzióra (minősített ajánlat)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (minősített ajánlat)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (minősített ajánlat) oktatóknak
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (minősített ajánlat) diákoknak
- Dynamics 365 for Sales Enterprise Edition (Government díjszabás) Add-On for CRM Basic (minősített ajánlat)
- Dynamics 365 Customer engagement Plan Enterprise Edition CRMOL alapszintű (minősített ajánlat)
- Dynamics 365 Customer engagement Plan Enterprise Edition (kormányzati díjszabás) CRMOL alapszintű (minősített ajánlat)
- Dynamics 365 Customer engagement Plan Enterprise Edition CRMOL alapszintű (minősített ajánlat) diákoknak
- Dynamics 365 Customer engagement Plan Enterprise Edition CRMOL alapszintű (minősített ajánlat) a kari
- Dynamics 365 ügyfél-bevonási terv Enterprise Edition for SA a CRM alapszintű (minősített ajánlat)
- Dynamics 365 Customer engagement Plan Enterprise Edition (kormányzati díjszabás) from SA for CRM Basic (minősített ajánlat)
- Dynamics 365 ügyfél-bevonási terv Enterprise Edition for SA for CRM Basic (minősített ajánlat) diákoknak
- Dynamics 365 ügyfél-bevonási terv Enterprise Edition for SA for CRM alapszintű (minősített ajánlat) a kar számára
- Dynamics 365 Customer engagement Plan Enterprise Edition Add-On for CRM Basic (minősített ajánlat)
- Dynamics 365 Customer engagement Plan Enterprise Edition (kormányzati díjszabás) Add-On for CRM Basic (minősített ajánlat)
- Dynamics 365 Customer engagement Plan Enterprise Edition Add-On a CRM alapszintű (minősített ajánlat) diákoknak
- Dynamics 365 Customer engagement Plan Enterprise Edition Add-On for CRM Basic (minősített ajánlat) a kari



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales/Customer bevonási terv az alapszintű (minősített ajánlatok) – helyettesítő csomagok

**Kivont ajánlatok**   

- Dynamics 365 CRM alapszintű vagy CRMOL alapszintű (minősített ajánlat) értékesítéséhez
- Dynamics 365 Customer engagement-terv a CRM Basic vagy a CRMOL alapszintű (minősített ajánlat) alapján

**Helyettesítő beállítások**
- Dynamics 365 for Sales Professional (új)
- Dynamics 365 for Sales Professional (új)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer engagement-csomag vagy
- Dynamics 365-csapat tagjai



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
 

 



