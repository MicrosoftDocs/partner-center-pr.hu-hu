---
title: Skype Vállalati verzió-előfizetések áttelepítése
description: Megtudhatja, hogyan és mikor kell a lejáró Skype Vállalati online verzió 1. csomag előfizetésével lejáró ügyfeleket új Office 365-verziókra mirateálni.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: f395987ef647fa6f7ed264c6476ddae419eabc34
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002858"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Skype Vállalati online verzió (1. csomag) előfizetéseinek migrálása újabb Office 365-verziókba

**Megfelelő szerepkörök**

- Értékesítési ügynök

A Skype Vállalati online verzió 1. csomagja 2018. augusztus 1-től ki leszvezetve. Ezt követően az ügyfelek már nem vásárolhatnak új Skype Vállalati verzió 1. csomagra vonatkozó előfizetéseket, és a meglévő előfizetések nem újulnak meg automatikusan a lejáratuk után, és nem biztosítják a megújítási lehetőséget. Az előfizetés részletek lapján a Skype Vállalati online verzió 1. csomagja előfizetési állapota "Lejárat dátuma[dátum]" állapotra módosult a következőről: "Automatikus megújítás [dátum]".  

Az ügyfelek folytonosságának biztosítása érdekében a lejáró Skype Vállalati online verzió 1. csomag előfizetését egy támogatott termékváltozatra kell átemálnia az alább felsorolt támogatott termékváltozatra. Javasoljuk, hogy az ügyfeleket az előfizetés éves záró dátuma előtt új előfizetésekbe költöztetjék, hogy elkerülje az ügyfelek szolgáltatáskimaradását. 

>[!NOTE]
>Mind a Skype Vállalati online verzió 1. csomagja, mind a kormányzati termékkódok ki vannakvezetve.

Ha az API-t használja (CREST vagy Partnerközpont), keresse meg a lejáró előfizetéseket az előfizetés záró dátumának és az automatikus megújítás = Hamis tulajdonság kiértékelével. A Skype Vállalati online verzió 1. csomagja előfizetései 2018. szeptember 1-től automatikus megújítás=Hamis lesz. Az ügyfeleket bármikor áthelyezheti egy új csomagba. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Skype Vállalati online verzió – 1. csomag – cseretervek

Az új csomagokkal az ügyfelek az Office 365 újabb funkcióit és funkcióit is kihasználhatják. A díjszabás részletei az árlista és az ajánlatlista mátrixában találhatók a Partnerközpont. 

- 1. lehetőség: Office 365 Nagyvállalati F1 verzió
- 2. lehetőség: Microsoft 365 Nagyvállalati verzió F1
- 3. lehetőség: Egyéb Office 365-csomagok

|**Szolgáltatás**    |**1\. lehetőség**   |**2\. lehetőség**   |**3. lehetőség**   |
|:-----------------|:-----------------|:-------------|:------------|
|Szerezze be a Skype Vállalati online verzió 1. csomagja összes funkcióját|Igen   |Igen   |Yes   |
|IM és jelenlét |Igen   |Igen   |Yes   |
|Társközi hang- és videó IP-cím alapján|Igen   |Igen   |Yes   
|Értekezletek csatlakozása hitelesített felhasználóként| Igen   |Igen   |Yes   |

## <a name="transition-customers-to-new-product-plans"></a>Ügyfelek átváltása új terméktervekbe

A Microsoft folyamatosan kínál új termékeket és szolgáltatásokat a partnereink számára. Ezekben az esetekben szükség lehet az ügyfelek új szolgáltatásokra való frissítéséhez, vagy az előfizetéseiknek a végül leállítható SKUs-ból való áttelepítéséhez. Az ügyfeleknek a visszavont SKUs-ból újabbakra való áttelepítéséhez a következő lépésekre van szükség:

- Az új előfizetés vásárlása
- Aktuális felhasználói licencek ismételt hozzárendelése
- Régi előfizetés lemondása

### <a name="migrate-your-customers-to-new-plans"></a>Ügyfelek áttelepítése új csomagokba

1. Az új előfizetés megvásárlásához a Partnerközpont **válassza** az Ügyfelek **lehetőséget,** válassza ki az áthelyezni kívánt ügyfelet, majd válassza az **Előfizetések hozzáadása lehetőséget.**

2. Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek valamelyikét), adja meg a licencek számát, majd válassza a **Küldés lehetőséget.** 

Az ügyfélnek most már mind a régi, mind az új előfizetéssel, a régi Skype Vállalati online verzió 1. csomag előfizetésével és az új "cél" előfizetéssel kell rendelkezik, például 1. lehetőség – Office 365 Nagyvállalati F1 csomag.

3. Az ügyfél felhasználói licencének ismételt hozzárendelése érdekében  a Partnerközpont menüjében válassza az Ügyfelek **lehetőséget,** válassza ki az áthelyezni kívánt ügyfelet, majd válassza a Felhasználók és licencek **lehetőséget.** Megnyílik az ügyfél Felhasználók és licencek lapja.

4. A felhasználói licenc ismételt hozzárendeléséhez válassza ki az újra hozzárendelni kívánt felhasználót, majd válassza a **Licencek kezelése lehetőséget.**

5. A **Licencek kezelése lapon** törölje a Skype Vállalati online verzió 1. csomagja licenc jelölőnégyzet jelölését, és válasszon ki egy új szolgáltatástervet ahhoz az előfizetéshez, amelybe az ügyfél átköltöz.

6. Válassza a **Küldés** lehetőséget. A megerősítő oldal felsorolja az új licenc-hozzárendeléseket. Ugyanezt a folyamatot folytathatja a licenc-hozzárendelést használó többi felhasználónál is.

Miután a felhasználói licencet az új szolgáltatásba költözteti, biztonságosan megszüntetheti a visszavont előfizetést az ügyfél szintjén.

7. A **Partnerközpont** válassza az Ügyfelek **lehetőséget.** Válassza ki azt az ügyfelet, akinek az előfizetését lemondja.

8. Az előfizetés részletei lapon állítsa az előfizetést **Felfüggesztettre.**

9. Válassza a **Küldés lehetőséget.**

A régi előfizetés fel van függesztve, és az új előfizetés aktív. A felfüggesztett előfizetés 120 nap után automatikusan fel lesz függesztve. Az ügyfél nem jár többletköltségekkel a régi előfizetésért.

## <a name="next-steps"></a>Következő lépések

- [Tanácsadók: Próbaverziós meghívó létrehozása és küldése az ügyfeleknek az Office 365 kipróbálására](advisors-create-a-trial-invitation.md)
- [Tanácsadók: Ügyfélbázis összeállítása Office 365-próbameghívásokkal és vásárlási ajánlatokkal](advisors-build-your-business.md)
- [Tanácsadók: Vásárlási ajánlat létrehozása](advisor-create-a-purchase-offer.md)
