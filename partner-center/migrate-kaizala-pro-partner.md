---
title: Kaizala Pro-előfizetések migrálása a Microsoft 365-be
description: Útmutató Kaizala Pro-előfizetések áttelepítéséhez Microsoft 365 Office 365-verziókba. Az ügyfelek átváltásának további részleteiért olvassa el ezt a cikket.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146425"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Kaizala Pro Standalone-előfizetések áttelepítése Microsoft 365 Office 365-verziókba

**Megfelelő szerepkörök:** Értékesítési ügynök

2020. július 1-től a Microsoft befejezi az önálló Kaizala Pro szolgáltatás értékesítését. Az ügyfelek ezt követően már nem vásárolhatnak új Kaizala Pro-előfizetéseket, és a meglévő Kaizala Pro-előfizetések nem újulnak meg automatikusan a lejáratuk után.

Az ügyfelek folytonosságának biztosítása érdekében a lejáró Kaizala Pro önálló előfizetéssel az alább felsorolt támogatott termékváltozatra kell átállni az ügyfelekre. Javasoljuk, hogy az ügyfeleket az előfizetés éves záró dátuma előtt új előfizetésekbe költöztetjék, hogy elkerülje az ügyfelek szolgáltatáskimaradását.

Ha az API-t használja (CREST vagy Partnerközpont), a lejáró előfizetéseket úgy derítheti fel, ha kiértékeli az előfizetés záró dátumát, valamint az automatikus megújítás tulajdonság false (hamis) értéket ad meg: `auto renew = False` .

Az E4-előfizetések beállítása `auto renew=False` 2020. július 1-ére lesz beállítva. Az ügyfeleket bármikor áthelyezheti egy új csomagba.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro Önálló helyettesítő csomagok

Az új csomagokkal az ügyfelek az új funkciókat és funkciókat is kihasználhatják a Microsoft 365. A díjszabás részletei az árlista és az ajánlatlista mátrixában találhatók a Partnerközpont.

- [**Microsoft 365 vállalati verzió,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)beleértve a következőket:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 az elővonalhoz, beleértve**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)a következőket:
   - Microsoft 365 F3 (korábbi nevén F1) Microsoft 365 Office 365 F3
    
- [**Microsoft 365 vállalati verzióhoz,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)beleértve a következőket: 
   - Office 365 E1
   - Microsoft 365 E3 és Office 365 E3
   - Microsoft 365 E5 és Office 365 E5

- [**Microsoft 365 for Education,**](https://www.microsoft.com/education/buy-license/microsoft365)beleértve a következőket: 
    - Microsoft 365 A1 és Office 365 A1
    - Microsoft 365 A3 és Office 365 A3
    - Microsoft 365 A5 és Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Ügyfelek váltása új terméktervekre

A Microsoft folyamatosan kínál új termékeket és szolgáltatásokat partnereinknek. Ezekben az esetekben szükség lehet az ügyfelek új szolgáltatásokra való frissítéséhez, vagy az előfizetéseiknek a végül leállítható SKUs-ból való áttelepítéséhez. Az ügyfeleknek a visszavont SKUs-ból újabbakra való áttelepítéséhez a következő lépésekre van szükség:

A. Az új előfizetés megvásárlása

B. Aktuális felhasználói licencek ismételt hozzárendelése

C. Régi előfizetés lemondása


## <a name="migrate-your-customers-to-new-plans"></a>Ügyfelek áttelepítése új csomagokba

### <a name="a-purchase-the-new-subscription"></a>A. Az új előfizetés megvásárlása

1. Az új előfizetés megvásárlásához a Partnerközpont **menüben** válassza az Ügyfelek **lehetőséget,** válassza ki az áthelyezni kívánt ügyfelet, majd válassza az **Előfizetések hozzáadása lehetőséget.**

2. Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikével), adja meg a licencek számát, majd válassza a **Küldés lehetőséget.**

Az ügyfélnek most már mind a régi, mind az új előfizetéssel, a régi Önálló Kaizala Pro-előfizetéssel és az új "cél" előfizetéssel kell rendelkezik, például 1. lehetőség – Office 365 Nagyvállalati F1 csomag.

### <a name="b-reassign-current-user-licenses"></a>B. Aktuális felhasználói licencek ismételt hozzárendelése

1. Az ügyfél felhasználói licencének ismételt hozzárendelése érdekében  a Partnerközpont menüjében válassza az Ügyfelek **lehetőséget,** válassza ki az áthelyezni kívánt ügyfelet, majd válassza a Felhasználók és licencek **lehetőséget.** Megnyílik az ügyfél Felhasználók és licencek lapja.

2. A felhasználói licenc ismételt hozzárendeléséhez válassza ki az újra hozzárendelni kívánt felhasználót, majd válassza a **Licencek kezelése lehetőséget.**

3. A **Licencek kezelése lapon** törölje a Kaizala Pro Standalone license (Önálló Kaizala Pro-licenc) jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatástervet ahhoz az előfizetéshez, amelybe az ügyfelet átköltöztetik.

4.  Válassza a **Küldés** lehetőséget. A megerősítő oldal felsorolja az új licenc-hozzárendeléseket. Ugyanezt a folyamatot folytassa a licenc-hozzárendelést használó többi felhasználóval is.

### <a name="c-cancel-old-subscription"></a>C. Régi előfizetés lemondása

Miután a felhasználói licencet az új szolgáltatásba költözteti, biztonságosan megszüntetheti a megszüntetett előfizetést az ügyfél szintjén.

1.  A **Partnerközpont** válassza az Ügyfelek **lehetőséget.** Válassza ki azt az ügyfelet, akinek az előfizetését lemondja.

2.  Az előfizetés részletei lapon állítsa az előfizetést **Felfüggesztettre.**

3.  Válassza a **Küldés** lehetőséget.

A régi előfizetés fel van függesztve, és az új előfizetés aktív. A felfüggesztett előfizetés 120 nap után automatikusan fel lesz függesztve. Az ügyfél nem jár további költségekkel a régi előfizetésért.
