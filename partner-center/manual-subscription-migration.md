---
title: Minősített Dynamics 365-előfizetések áttelepítése
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Útmutató minősített, alapszintű Dynamics 365-előfizetések új előfizetésre való áttelepítéséhez a meglévő előfizetések lejárta előtt.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151644"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>A Dynamics 365 és a Customer Engagement Plan migrálása az Alapszintű szolgáltatásról (arra jogosult ajánlatokról) újabb verziókra

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Rendszergazdai ügynök | Értékesítési ügynök

2019. január 1-jén az alapszintű (minősített ajánlatok) előfizetéssel rendelkező Dynamics 365 for Sales/Customer Engagement-csomaggal rendelkező ügyfelek már nem újíthatja meg ezeket az örökölt ajánlatokat; A meglévő előfizetések nem újulnak meg automatikusan a lejáratukkor. Az előfizetés részleteinek oldalán az előfizetés állapota "Lejárat dátuma[dátum]" lesz az "Automatikus megújítás [dátum]" alatt. 

Az ügyfelek folytonosságának biztosítása érdekében érdemes a lejáró előfizetéseket egy támogatott lehetőségre átemálni, az alábbiakban felsoroltak szerint. Javasoljuk, hogy az ügyfeleket az előfizetés éves záró dátuma előtt új előfizetésekbe költöztetjék, hogy elkerülje az ügyfelek szolgáltatáskimaradását.

Ha az API-t használja (CREST vagy Partnerközpont), a lejáró előfizetéseket az előfizetés záró dátumának és az automatikus megújítás = Hamis tulajdonság kiértékelésével találhatja meg. A kérdéses előfizetések 2019. január 1-jén automatikus renew=False (automatikus megújítás=Hamis) beállításra lesznek beállítva. Az ügyfeleket bármikor áthelyezheti egy új csomagba. 

### <a name="the-dynamics-365-offers-being-retired"></a>A Dynamics 365-ajánlatok kivezetve

- Dynamics 365 for Sales Enterprise kiadás CRMOL Basic (minősített ajánlat)
- Dynamics 365 for Sales Enterprise kiadás CRMOL Basic (minősített ajánlat) oktatóknak
- Dynamics 365 for Sales Enterprise kiadás CRMOL Basic (minősített ajánlat) diákoknak
- Dynamics 365 for Sales Enterprise kiadás (kormányzati díjszabás) CRMOL Alapszintű (minősített ajánlat)
- Dynamics 365 for Sales Enterprise kiadás Az SA for CRM Basicből (minősített ajánlat)
- Dynamics 365 for Sales Enterprise kiadás From SA for CRM Basic (Minősített ajánlat) oktatóknak
- Dynamics 365 for Sales Enterprise kiadás From SA for CRM Basic (Minősített ajánlat) diákoknak
- Dynamics 365 for Sales Enterprise kiadás (government pricing) From SA for CRM Basic (Minősített ajánlat)
- Dynamics 365 for Sales Enterprise kiadás Add-On for CRM Basic (minősített ajánlat)
- Dynamics 365 for Sales Enterprise kiadás Add-On for CRM Basic (minősített ajánlat) oktatóknak
- Dynamics 365 for Sales Enterprise kiadás Add-On for CRM Basic (minősített ajánlat) diákoknak
- Dynamics 365 for Sales Enterprise kiadás (government pricing) Add-On for CRM Basic (minősített ajánlat)
- Dynamics 365 Customer Engagement-csomag Enterprise kiadás CRMOL Alapszintű (minősített ajánlat)
- Dynamics 365 Customer Engagement Plan Enterprise kiadás (kormányzati díjszabás) CRMOL Alapszintű (minősített ajánlat)
- Dynamics 365 Customer Engagement-csomag Enterprise kiadás CRMOL Alapszintű (minősített ajánlat) diákoknak
- Dynamics 365 Customer Engagement-Enterprise kiadás CRMOL Alapszintű (minősített ajánlat) oktatóknak
- Dynamics 365 Customer Engagement csomag Enterprise kiadás AZ SA for CRM Basicből (minősített ajánlat)
- Dynamics 365 Customer Engagement Plan Enterprise kiadás (government pricing) From SA for CRM Basic (Minősített ajánlat)
- Dynamics 365 Customer Engagement plan Enterprise kiadás From SA for CRM Basic (Minősített ajánlat) diákoknak
- Dynamics 365 Customer Engagement plan Enterprise kiadás From SA for CRM Basic (Minősített ajánlat) oktatóknak
- Dynamics 365 Customer Engagement Plan Enterprise kiadás Add-On for CRM Basic (minősített ajánlat)
- Dynamics 365 Customer Engagement Plan Enterprise kiadás (government pricing) Add-On for CRM Basic (minősített ajánlat)
- Dynamics 365 Customer Engagement Plan Enterprise kiadás Add-On for CRM Basic (minősített ajánlat) diákoknak
- Dynamics 365 Customer Engagement plan Enterprise kiadás Add-On for CRM Basic (Minősített ajánlat) oktatóknak



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales/ Customer Engagement-csomag alapszintű (minősített ajánlatok) helyettesítő csomagokból

**Visszavont ajánlatok**   

- Dynamics 365 for Sales a CRM Basicből vagy a CRMOL Basicből (minősített ajánlat)
- Dynamics 365 Customer Engagement-csomag a CRM Basicből vagy a CRMOL Basicből (minősített ajánlat)

**Cserebeállítások**
- Dynamics 365 for Sales Professional (ÚJ)
- Dynamics 365 for Sales Professional (ÚJ)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement-csomag vagy
- Dynamics 365-csapattagok



## <a name="transition-customers-to-new-product-plans"></a>Ügyfelek váltása új terméktervekre

Ha az ügyfeleket a visszavont SKUS-król újabbakra kívánja átemeltetni, a következő lépésekre van szükség ebben a sorrendben:

- Az új előfizetés megvásárlása
- Aktuális felhasználói licencek ismételt hozzárendelése
- Régi előfizetés lemondása

## <a name="purchase-the-new-plan-for-your-customer"></a>Az új csomag vásárlása az ügyfél számára

1. A **bal oldali** navigációs sávon válassza az Ügyfelek lehetőséget, majd válassza ki az új előfizetésre áthelyezni kívánt ügyfelet.
2. Válassza **az Előfizetés hozzáadása lehetőséget.**
3. Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyike), adja meg a licencek számát, majd válassza a **Küldés lehetőséget.** 

Az ügyfél most már a régi előfizetéssel és az új előfizetéssel is rendelkezik. A következő lépés a licencek ismételt hozzárendelése az ügyfél felhasználóihoz.

1. A **bal oldali** navigációs sávon válassza az Ügyfelek lehetőséget, majd válassza ki az ügyfelet, akinél az áthelyezést választja.
2. Válassza **a Felhasználók és licencek lehetőséget.**
3. Egy licenc felhasználóhoz való ismételt hozzárendeléséhez jelölje ki a felhasználót, majd válassza a **Licencek kezelése lehetőséget.** 
4. A **Licencek kezelése** lapon törölje a Dynamics 365 for Sales/Customer Engagement Plan from Basic (Minősített ajánlat) licenc jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatási tervet ahhoz az előfizetéshez, amelybe az ügyfél át lesz költözve. 
5. Válassza a **Küldés** lehetőséget. Ezt minden olyan felhasználóval meg kell tenni, akinek új licencre van szüksége. 

Miután áthelyezte a licenceket az új előfizetésbe, megszüntetheti a régi előfizetést. 

1. A **bal oldali navigációs** sávon válassza az Ügyfelek lehetőséget, majd válassza ki a költözni kívánt ügyfelet.
2. Az előfizetés részletei lapon állítsa a régi előfizetést Felfüggesztettre, majd **válassza** a **Küldés lehetőséget.**

A régi előfizetés most fel van függesztve, és az új előfizetés aktív. A felfüggesztett előfizetés 120 nap után automatikusan fel lesz függesztve. Az ügyfél nem jár többletköltségsel a régi előfizetésért.
 

 



