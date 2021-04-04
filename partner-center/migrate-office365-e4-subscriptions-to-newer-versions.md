---
title: Office 365 E4-előfizetések migrálása
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A Microsoft Office 365 Enterprise E4 kiadása 2017. április 7-én megszűnik. Ismerje meg, hogyan telepítheti át az ügyfél-előfizetéseket az Office 365 újabb verzióira.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132621"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Office 365 E4-előfizetések migrálása újabb Office 365-verziókba

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói felügyeleti rendszergazda
- Felügyeleti ügynök
- Értékesítési ügynök

Az Office 365 Enterprise E4-csomag kivonásra kerül, amely 2017. április 7-én érvényes. Ezen időpont után már nem vásárolhat új Office 365 E4-előfizetést, és a meglévő E4-előfizetések nem fognak automatikusan megújítani a lejárat után.

Az E4-előfizetések végén a rendszer megszakítja őket. Az ügyfelek folytonosságának biztosítása érdekében az alábbi listában szereplő, az E4-előfizetésekkel rendelkező ügyfeleket egy támogatott SKU-ra kell áttérnie. Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára. 

> [!NOTE]  
> Az Office 365 Enterprise E4 kereskedelmi és kormányzati SKU-t is kivonják.
 
Az előfizetés részletei lapon az E4 előfizetés állapota "lejár [date]" értékre módosult az "automatikus megújítások [date]" kifejezésből. 

Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejárati előfizetéseket az előfizetés befejezési dátumának és az automatikus megújítás = hamis tulajdonságnak a kiértékelésével derítheti fel. 

Az E4-előfizetések az automatikus megújítás = false értékre lesznek állítva 2017. április 7-én. Az ügyfeleket bármikor át lehet helyezni egy új csomagba. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 Enterprise E4 kiadás-helyettesítési tervek

Dönthet úgy is, hogy az E4-es verzióval azonos funkciókat tart fenn, vagy az ügyfelek kihasználhatják az Office 365 és a Skype vállalati online verzió újabb funkcióit és funkcióit. A díjszabással kapcsolatos részletek a partner Center árlista és ajánlatok listája mátrixában találhatók. A biztonságos termék nagyvállalati E3 vagy a biztonságos produktív nagyvállalati E5 a következő, az Office 365 nagyvállalati E3 vagy Office 365 Enterprise E5 lehetőségekkel lehet helyettesíteni.

- 1. lehetőség: Office 365 Enterprise E5

- 2. lehetőség: Office 365 Enterprise E3 + Skype for Business Cloud PBX

- 3. lehetőség: Office 365 Enterprise E3 + Skype for Business Plus CAL (ár és funkció paritása E4-vel)

- 4. lehetőség: Office 365 Enterprise E3


| Szolgáltatás | 1\. lehetőség | 2\. lehetőség | 3. lehetőség | 4. lehetőség |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Az Office 365 nagyvállalati E4 csomag összes funkciójának beolvasása | Igen | Igen | Igen | Nem |
| Az Office 365-ben felügyelt telefonszámok | Igen | Igen | Nem | Nem |
| A telefonszámok a helyszínen és az Office 365-ben (hibrid üzembe helyezés) vannak kezelve? | Igen | Igen | Nem | Nem |
| Lehetősége van PSTN hanghívási terv hozzáadására? | Igen | Igen | Nem | Nem |
| PSTN-konferencia? | Igen | Nem | Nem | Nem |
| Speciális eszközök az együttműködéshez, az elemzéshez és a biztonsághoz? | Igen | Nem | Nem | Nem |
| Interaktív jelentések, irányítópultok és adatvizualizációk? | Igen | Nem | Nem | Nem | 
| Jobban kézben tarthatja az adatbiztonságot és a megfelelőséget a beépített adatvédelem, az átláthatóság és a kifinomult felhasználói vezérlők terén? | Igen | Nem | Nem | Nem | 

## <a name="transition-customers-to-new-product-plans"></a>Ügyfelek átváltása új termékekre

A Microsoft folyamatosan új termékeket és szolgáltatásokat kínál partnereinknek. Ezekben az esetekben előfordulhat, hogy frissítenie kell az ügyfeleket az új szolgáltatásokra, vagy át kell telepítenie az előfizetéseket olyan SKU-ból, amely végül le lesz állítva. Az ügyfelek áttelepítése a kivont SKU-ról újabb verzióra a következő lépések szükségesek:

-   Az új előfizetés megvásárlása
-   Aktuális felhasználói licencek újbóli társítása
-   A régi előfizetés megszakítása

Az alábbi lépéseket követve áttelepítheti az ügyfél Office 365 Enterprise E4-előfizetését a fenti táblázatban található egyik lehetőségre.

### <a name="step-1---purchase-the-new-subscription"></a>1. lépés – az új előfizetés megvásárlása

1. A **partner Center** menüben válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza az **előfizetések hozzáadása** elemet.

2. Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikét), adja meg a licencek számát, majd válassza a **Küldés** lehetőséget.

   Az ügyfél most már rendelkezik a régi és az új előfizetéssel, a régi Office 365 Enterprise E4-előfizetéssel és az új "Target" előfizetéssel, például 1. lehetőség – Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>2. lépés – az ügyfél felhasználói licencének újbóli társítása

1. A **partner Center** menüben válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza a **felhasználók és licencek** lehetőséget. Megnyílik az ügyfél felhasználói és licencek lapja.

2. A felhasználói licencek újbóli hozzárendeléséhez válassza ki az újból hozzárendelni kívánt felhasználót, majd válassza a **licencek kezelése** lehetőséget.

3. A **licencek kezelése** lapon törölje az **Office 365 Enterprise E4** -licenc jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatási csomagot ahhoz az előfizetéshez, amelyet az ügyfél áthelyez.

4. Válassza a **Küldés** lehetőséget. A megerősítést kérő lap felsorolja az új licenc-hozzárendeléseket.

5. Folytassa ugyanezeket a lépéseket minden más ügyfél-felhasználóval, akiknek licenc-hozzárendelésre van szükségük.

Miután áthelyezte a felhasználói licenceket az új szolgáltatásba, biztonságosan megszakíthatja a kivont előfizetést a felső szintű ügyfél szintjén.

### <a name="step-3---cancel-the-old-subscription"></a>3. lépés – a régi előfizetés megszakítása

1. A **partner Center** menüben válassza az **ügyfelek** lehetőséget. Válassza ki az áthelyezni kívánt ügyfelet, és válassza ki a megszüntetni kívánt előfizetést.

2. Az előfizetés részletei lapon állítsa az előfizetés állapotát **felfüggesztve** értékre.

3. Válassza a **Küldés** lehetőséget.

A régi előfizetés fel van függesztve, és az új előfizetés aktív. A felfüggesztett előfizetés 120 nap elteltével automatikusan kiépítve lesz. Az ügyfél nem számít fel további költséget a régi előfizetéshez.



 



