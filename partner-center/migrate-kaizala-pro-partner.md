---
title: Kaizala Pro-előfizetések migrálása a Microsoft365-be
description: Ismerje meg, hogyan telepíthet át Kaizala Pro-előfizetéseket Microsoft365 vagy Office 365-verzióra. Az ügyfelek átváltásával kapcsolatos további információkért olvassa el ezt a cikket.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530517"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a>Kaizala Pro önálló előfizetések migrálása a Microsoft365 vagy az Office 365 verzióra

2020. július 1-től a Microsoft befejezte a Kaizala Pro önálló szolgáltatás értékesítését. Ezen időpont után az ügyfelek többé nem vásárolhatnak új Kaizala Pro-előfizetéseket, és a meglévő Kaizala Pro-előfizetések nem fognak automatikusan megújítani a lejárat után.

Az ügyfelek folytonosságának biztosítása érdekében az alábbi listában szereplő, a Kaizala Pro önálló előfizetések lejáratával rendelkező ügyfeleket kell átállnia egy támogatott SKU-ra. Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára.

Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejáró előfizetések felderítéséhez az előfizetés befejezési dátumát és az automatikus megújítás tulajdonságot false (hamis) értékre kell kiértékelve: `auto renew = False` .

Az E4-előfizetések `auto renew=False` 2020. július 1-jén lesznek beállítva. Az ügyfeleket bármikor át lehet helyezni egy új csomagba.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro önálló helyettesítési csomagok

Az új csomagokkal az ügyfelek a Microsoft 365 újabb funkcióit és funkcióit vehetik igénybe. A díjszabással kapcsolatos részletek a partner Center árlista és ajánlatok listája mátrixában találhatók.

- [**Üzleti Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), beleértve a következőket:  
   - Alapszintű Microsoft 365 Vállalati verzió
   - Microsoft 365 Vállalati verzió standard
   - Prémium Microsoft 365 Vállalati verzió
    
- [**Microsoft 365 a Frontline számára**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), beleértve a következőket:
   - Microsoft 365 F3 (korábban Microsoft 365 F1) és Office 365 F3
    
- [**Microsoft 365 a vállalat számára**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), beleértve a következőket: 
   - Office 365 E1 csomag
   - Microsoft 365 E3 és Office 365 E3
   - Microsoft 365 E5 és Office 365 E5

- [**Oktatási Microsoft 365**](https://www.microsoft.com/education/buy-license/microsoft365), beleértve a következőket: 
    - Microsoft 365 a1 és Office 365 a1
    - Microsoft 365 a3 és Office 365 a3
    - Microsoft 365 a5 és Office 365 a5 csomag

## <a name="transition-customers-to-new-product-plans"></a>Ügyfelek átváltása új termékekre

A Microsoft folyamatosan új termékeket és szolgáltatásokat kínál partnereinknek. Ezekben az esetekben előfordulhat, hogy frissítenie kell az ügyfeleket az új szolgáltatásokra, vagy át kell telepítenie az előfizetéseket olyan SKU-ból, amely végül le lesz állítva. Az ügyfelek áttelepítése a kivont SKU-ról újabb verzióra a következő lépések szükségesek:

A. Az új előfizetés megvásárlása

B. Aktuális felhasználói licencek újbóli társítása

C. Régi előfizetés megszakítása


## <a name="migrate-your-customers-to-new-plans"></a>Ügyfelek migrálása új csomagokra

### <a name="a-purchase-the-new-subscription"></a>A. Az új előfizetés megvásárlása

1. Az új előfizetés megvásárlásához a **partner Center** menüjéből válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza az **előfizetések hozzáadása** elemet.

2. Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikét), adja meg a licencek számát, majd válassza a **Küldés** lehetőséget.

Az ügyfél most már rendelkezik a régi és az új előfizetéssel, a régi Kaizala Pro önálló előfizetéssel és az új "Target" előfizetéssel, például 1. lehetőség – Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Aktuális felhasználói licencek újbóli társítása

1. Az ügyfél felhasználói licencének újbóli hozzárendeléséhez a **partner Center** menüjéből válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza a **felhasználók és licencek** lehetőséget. Megnyílik az ügyfél felhasználói és licencek lapja.

2. A felhasználói licenc újbóli hozzárendeléséhez válassza ki az újból hozzárendelni kívánt felhasználót, majd válassza a **licencek kezelése** lehetőséget.

3. A **licencek kezelése** lapon törölje a Kaizala Pro önálló licenc jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatási csomagot ahhoz az előfizetéshez, amelyet az ügyfél áthelyez.

4.  Válassza a **Küldés** lehetőséget. A megerősítést kérő lap felsorolja az új licenc-hozzárendeléseket. Folytassa ugyanezt a folyamatot azoknál a felhasználóknál, akiknek licenc-hozzárendelésre van szükségük.

### <a name="c-cancel-old-subscription"></a>C. Régi előfizetés megszakítása

Miután áthelyezte a felhasználói licencet az új szolgáltatásba, biztonságosan megszakíthatja a kivont előfizetést az ügyfél szintjén.

1.  A **partner Center** menüben válassza az **ügyfelek** lehetőséget. Válassza ki azt az ügyfelet, amelynek előfizetését törli.

2.  Az előfizetés részletei lapon állítsa az előfizetést **felfüggesztve** értékre.

3.  Válassza a **Küldés** lehetőséget.

A régi előfizetés fel van függesztve, és az új előfizetés aktív. A felfüggesztett előfizetés 120 nap elteltével automatikusan kiépítve lesz. Az ügyfél nem számít fel további költséget a régi előfizetéshez.
