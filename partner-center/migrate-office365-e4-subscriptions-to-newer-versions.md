---
title: Office 365 E4-előfizetések áttelepítése
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Nagyvállalati E4 kiadás 2017. április 7-től ki vanvezetve. Megtudhatja, hogyan miheti át az ügyfél-előfizetéseket az Office 365 újabb verzióiba.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151559"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Office 365 E4-előfizetések migrálása újabb Office 365-verziókba

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Rendszergazdai ügynök | Értékesítési ügynök

Az Office 365 Nagyvállalati E4 csomag ki vanvezetve, 2017. április 7-től. Ezt követően már nem vásárolhat új Office 365 E4-előfizetéseket, és a meglévő E4-előfizetések nem újulnak meg automatikusan a lejáratuk után.

Az E4-előfizetések végén azok törlődnek. Az ügyfelek folytonosságának biztosítása érdekében az E4-előfizetéssel lejáró ügyfeleket az alább felsorolt támogatott termékváltozatra kell átemálni. Javasoljuk, hogy az ügyfeleket az előfizetés éves záró dátuma előtt új előfizetésekbe költöztetjék, hogy elkerülje az ügyfelek szolgáltatáskimaradását. 

> [!NOTE]  
> Az Office 365 Nagyvállalati E4 kereskedelmi és kormányzati termékkódok ki vannakvezetve.
 
Az előfizetés részletek lapján az E4-előfizetés állapota "Lejárat [dátum] időpontban" állapotra módosult az "Automatikus megújítás [dátum]" állapotról. 

Ha az API-t használja (CREST vagy Partnerközpont), a lejáró előfizetéseket az előfizetés záró dátumának és az automatikus megújítás = Hamis tulajdonság kiértékelével derítheti fel. 

Az E4-előfizetések 2017. április 7-én automatikus megújítás=Hamis lesz. Az ügyfeleket bármikor új csomagba költöztetheti. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 Nagyvállalati E4 kiadás helyettesítő csomagja

Dönthet úgy, hogy ugyanazt a funkciót tartja fenn az E4-es verzióval, vagy az ügyfelek az Office 365 és a Skype Vállalati online verzió újabb funkcióit és funkcióit is kihasználhatják. A díjszabás részletei az árlista és az ajánlatlista mátrixában találhatók a Partnerközpont. A Secure Product Enterprise E3 vagy Secure Productive Enterprise E5 az Office 365 Nagyvállalati E3 vagy Az Office 365 Nagyvállalati E5 verzióra vonatkozó alábbi lehetőségeket helyettesítheti.

- 1. lehetőség: Office 365 Nagyvállalati E5 verzió

- 2. lehetőség: Office 365 Nagyvállalati E3+ Skype Vállalati verzió – Felhőalapú PBX

- 3. lehetőség: Office 365 Nagyvállalati E3 + Skype Vállalati verzió Plus CAL (ár- és funkcióparitás az E4-es verzióval)

- 4. lehetőség: Office 365 Nagyvállalati E3 verzió


| Szolgáltatás | 1\. lehetőség | 2\. lehetőség | 3. lehetőség | 4. lehetőség |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Szerezze be az Office 365 Nagyvállalati E4 verzió összes funkcióját? | Igen | Igen | Igen | Nem |
| Office 365-ben kezelt telefonszámok? | Igen | Igen | Nem | Nem |
| A helyszínen és az Office 365-ben kezelt telefonszámok (hibrid telepítés)? | Igen | Igen | Nem | Nem |
| Lehetőség van PSTN hanghívási csomag hozzáadására? | Igen | Igen | Nem | Nem |
| PSTN-konferencia? | Igen | Nem | Nem | Nem |
| Speciális együttműködési, elemzési és biztonsági eszközök? | Igen | Nem | Nem | Nem |
| Interaktív jelentések, irányítópultok és adatvizualizációk? | Igen | Nem | Nem | Nem | 
| Jobban szabályozható az adatbiztonság és -megfelelőség a beépített adatvédelem, átláthatóság és finomított felhasználói vezérlők segítségével? | Igen | Nem | Nem | Nem | 

## <a name="transition-customers-to-new-product-plans"></a>Ügyfelek átváltása új terméktervekbe

A Microsoft folyamatosan kínál új termékeket és szolgáltatásokat a partnereink számára. Ezekben az esetekben szükség lehet az ügyfelek új szolgáltatásokra való frissítéséhez, vagy az előfizetéseiknek a végül leállítható SKUs-ból való áttelepítéséhez. Az ügyfeleknek a visszavont SKUs-ból újabbakra való áttelepítéséhez a következő lépésekre van szükség:

-   Az új előfizetés vásárlása
-   Aktuális felhasználói licencek ismételt hozzárendelése
-   A régi előfizetés lemondása

Kövesse az alábbi lépéseket az ügyfelek Office 365 Nagyvállalati E4-előfizetésének a fenti táblázatban felsorolt lehetőségek egyikére való áttelepítéséhez.

### <a name="step-1---purchase-the-new-subscription"></a>1. lépés – Az új előfizetés megvásárlása

1. A **Partnerközpont** válassza az **Ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza az **Előfizetések hozzáadása lehetőséget.**

2. Válassza ki a katalógusból megvásárolni kívánt előfizetést (ebben az esetben a fenti lehetőségek egyikével), adja meg a licencek számát, majd válassza a **Küldés lehetőséget.**

   Az ügyfélnek most már a régi és az új előfizetéssel, a régi Office 365 Nagyvállalati E4 előfizetéssel és az új "cél" előfizetéssel is rendelkezik, például 1. lehetőség – Office 365 Nagyvállalati E5 verzió.

### <a name="step-2---reassign-the-customers-users-licenses"></a>2. lépés – Az ügyfél felhasználói licencének ismételt hozzárendelése

1. A **Partnerközpont** válassza az **Ügyfelek** lehetőséget, válassza ki az áthelyezni kívánt ügyfelet, majd válassza a Felhasználók és **licencek lehetőséget.** Megnyílik az ügyfél Felhasználók és licencek lapja.

2. A felhasználói licencek ismételt hozzárendeléséhez válassza ki az újra hozzárendelni kívánt felhasználót, majd válassza a **Licencek kezelése lehetőséget.**

3. A **Licencek kezelése lapon** törölje az **Office 365 Nagyvállalati E4** licenc jelölőnégyzet jelölését, és válasszon egy új szolgáltatástervet ahhoz az előfizetéshez, amelybe az ügyfelet átköltöztik.

4. Válassza a **Küldés** lehetőséget. A megerősítő oldal felsorolja az új licenc-hozzárendeléseket.

5. Ismételje meg ugyanezeket a lépéseket minden olyan ügyfélfelhasználóval, akik licencátkiosztást kell hozzárendelni.

A felhasználói licencek új szolgáltatásba való áthelyezését követően biztonságosan megszüntetheti a visszavont előfizetést a legfelső ügyfélszinten.

### <a name="step-3---cancel-the-old-subscription"></a>3. lépés – A régi előfizetés lemondása

1. A **Partnerközpont** válassza az Ügyfelek **lehetőséget.** Válassza ki az áthelyezni kívánt ügyfelet, és válassza ki a megszüntetni kívánt előfizetést.

2. Az előfizetés részleteit tartalmazó lapon állítsa az előfizetés állapotát **Felfüggesztve állapotra.**

3. Válassza a **Küldés** lehetőséget.

A régi előfizetés fel van függesztve, és az új előfizetés aktív. A felfüggesztett előfizetés 120 nap után automatikusan fel lesz függesztve. Az ügyfél nem jár többletköltségekkel a régi előfizetésért.



 



