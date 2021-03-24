---
title: Skype vállalati verzióra előfizetések áttelepíthetők
description: Megtudhatja, hogyan és mikor telepíthet át bizonyos ügyfeleket a lejáró Skype vállalati online verzióra vonatkozó, 1. csomagra vonatkozó új Office 365-verziókra.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 67c1689136892443937748b6cc9e31e4f0ac9983
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028417"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Skype Vállalati online verzió (1. csomag) előfizetéseinek migrálása újabb Office 365-verziókba

A Skype vállalati online verzió 1. csomagjának kivonása megszűnik, hatályba lép 2018. augusztus 1-től. Ezt követően az ügyfelek már nem vásárolhatják meg az új Skype vállalati csomag 1 előfizetést, és a meglévő előfizetések nem fognak automatikusan megújítani, amikor lejárnak, és nem biztosítanak megújítási lehetőséget. Az előfizetés részletei lapon a Skype vállalati online verzió 1. csomag előfizetés állapota "lejár [date]" értékre változott az "automatikus megújítások [date]" kifejezésből.  

Az ügyfelek folytonosságának biztosítása érdekében érdemes átállnia az ügyfeleknek a Skype vállalati online verzió 1. csomagjának előfizetéseit egy támogatott SKU-ra, amely az alábbiakban látható. Javasoljuk, hogy az előfizetések éves befejezési dátuma előtt helyezze át az ügyfeleket új előfizetésekre, hogy elkerülje a szolgáltatások leállását az ügyfelek számára. 

>[!NOTE]
>A Skype vállalati online verzió 1. csomag kereskedelmi és kormányzati SKU-t is kivonják.

Ha az API-t (vagy a CREST vagy a partner centert) használja, a lejáró előfizetéseket az előfizetés befejezési dátumának és az automatikus megújítás = hamis tulajdonságnak a kiértékelésével keresheti meg. A Skype vállalati online csomag 1 előfizetése az automatikus megújítás = false értékre lesz beállítva 2018. szeptember 1-jén. Az ügyfeleket bármikor át lehet helyezni egy új csomagba. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>A Skype vállalati online verzió 1. csomagjának pótlása

Az új csomagokkal az ügyfelek igénybe vehetik az Office 365 újabb funkcióit és funkcióit. A díjszabással kapcsolatos részletek a partner Center árlista és ajánlatok listája mátrixában találhatók. 

- 1. lehetőség: Office 365 Enterprise F1
- 2. lehetőség: Microsoft 365 Nagyvállalati verzió F1
- 3. lehetőség: egyéb Office 365-csomagok

|**Szolgáltatás**    |**1\. lehetőség**   |**2\. lehetőség**   |**3. lehetőség**   |
|:-----------------|:-----------------|:-------------|:------------|
|A Skype vállalati online verzió 1. csomagjának összes funkciójának beolvasása|Igen   |Igen   |Igen   |
|CSEVEGÉS és jelenlét |Igen   |Igen   |Igen   |
|Társközi hang-és videó az IP-címeken keresztül|Igen   |Igen   |Igen   
|Értekezletek csatlakoztatása hitelesített felhasználóként| Igen   |Igen   |Igen   |

## <a name="transition-customers-to-new-product-plans"></a>Ügyfelek átváltása új termékekre

A Microsoft folyamatosan új termékeket és szolgáltatásokat kínál partnereinknek. Ezekben az esetekben előfordulhat, hogy frissítenie kell az ügyfeleket az új szolgáltatásokra, vagy át kell telepítenie az előfizetéseket olyan SKU-ból, amely végül le lesz állítva. Az ügyfelek áttelepítése a kivont SKU-ról újabb verzióra a következő lépések szükségesek:

- Az új előfizetés megvásárlása
- Aktuális felhasználói licencek újbóli társítása
- Régi előfizetés megszakítása

### <a name="migrate-your-customers-to-new-plans"></a>Ügyfelek migrálása új csomagokra

1. Az új előfizetés megvásárlásához a **partner Center menüjéből** válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza az **előfizetések hozzáadása** elemet.

2. Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikét), adja meg a licencek számát, majd válassza a **Küldés** lehetőséget. 

Az ügyfél most már rendelkezik a régi és az új előfizetéssel, a régi Skype vállalati online csomag 1 előfizetéssel és az új "Target" előfizetéssel, például 1. lehetőség – Office 365 Enterprise F1.

3. Az ügyfél felhasználói licencének újbóli hozzárendeléséhez a **partner Center** menüjéből válassza az **ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza a **felhasználók és licencek** lehetőséget. Megnyílik az ügyfél felhasználói és licencek lapja.

4. A felhasználói licenc újbóli hozzárendeléséhez válassza ki az újból hozzárendelni kívánt felhasználót, majd válassza a **licencek kezelése lehetőséget.**

5. A **licencek kezelése** lapon törölje a Skype vállalati online verzió 1. csomagjának licence jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatási csomagot ahhoz az előfizetéshez, amelyet az ügyfél áthelyez.

6. Válassza a **Küldés** lehetőséget. A megerősítést kérő lap felsorolja az új licenc-hozzárendeléseket. Folytassa ugyanezt a folyamatot azoknál a felhasználóknál, akiknek licenc-hozzárendelésre van szükségük.

Miután áthelyezte a felhasználói licencet az új szolgáltatásba, biztonságosan megszakíthatja a kivont előfizetést az ügyfél szintjén.

7. A **partner Center** menüben válassza az **ügyfelek** lehetőséget. Válassza ki azt az ügyfelet, amelynek előfizetését törli.

8. Az előfizetés részletei lapon állítsa az előfizetést **felfüggesztve** értékre.

9. Válassza a **Küldés lehetőséget.**

A régi előfizetés fel van függesztve, és az új előfizetés aktív. A felfüggesztett előfizetés 120 nap elteltével automatikusan kiépítve lesz. Az ügyfél nem számít fel további költséget a régi előfizetéshez.

