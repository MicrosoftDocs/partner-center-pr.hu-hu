---
title: A Dynamics 365 CRM-partneri központ közös értékesítési összekötője
description: Szinkronizálja a partner Centerben lévő hivatkozásokat a Dynamics 365 CRM-hez készült közös értékesítési összekötővel. Ezután a Microsofttal együtt értékesítheti a CRM-rendszerét.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 2082424f8203f0d9c50726e1e5ef7b3e3c39d6c2
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768771"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Közös értékesítési összekötő a Dynamics 365 CRM-hez – áttekintés

### <a name="appropriate-roles"></a>Megfelelő szerepkörök

- Ajánlói rendszergazda
- Rendszerfelügyeleti webszolgáltatások vagy Rendszertestreszabó a CRM-ben

A partner Center közös értékesítési összekötői lehetővé teszik, hogy az értékesítők a Microsofttal közösen értékesítsenek a CRM-rendszereken belül. Nem kell kiképezniük, hogy a partner centerrel együtt kezeljék a közös értékesítési ajánlatokat. A közös értékesítésű összekötők használatával új, közösen értékesíthető utalást hozhat létre a Microsoft-értékesítők bevonására, a Microsoft-értékesítőtől érkező hivatkozásokra, az átirányítások elfogadására vagy elutasítására, valamint az üzlet adatainak módosítására, például a Deal Value és a zárás Ezeket a közös értékesítési ajánlatokat a Microsoft-értékesítők frissítései is megkapják. Az Ön által választott CRM-ben kezelheti az összes átirányítási munkát, nem pedig a partner Centerben.

A megoldás a Power automatizáláson alapul, és a partner Center API-kat használja.

## <a name="prerequisites"></a>Előfeltételek

A megoldás telepítése előtt győződjön meg arról, hogy megfelel a következő előfeltételeknek.

|**Témakörök**   |**Részletek**   |**Hivatkozások**   |
|--------------|--------------------|------|
|Microsoft Partner Network (MPN) azonosítója |Érvényes MPN-AZONOSÍTÓra van szüksége.|[Csatlakozás a partner hálózathoz](https://partner.microsoft.com/)|
|Közös értékesítés kész|Az IP-/szolgáltatási megoldásnak közös értékesítéssel kell rendelkeznie.|[Értékesítés a Microsofttal](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Partnerközpont-fiók|A partner Center-bérlőhöz társított MPN-AZONOSÍTÓnak meg kell egyeznie a közös értékesítési megoldáshoz társított MPN-azonosítóval. Az összekötők üzembe helyezése előtt ellenőrizze, hogy látható-e a közös értékesítéssel kapcsolatos hivatkozások a partner Center portálon.|[Saját fiók kezelése](create-user-accounts-and-set-permissions.md)|
|A partner Center felhasználói szerepkörei|Az összekötőket telepítő és használó alkalmazottnak hivatkozói rendszergazdának kell lennie.|[Felhasználói szerepkörök és engedélyek hozzárendelése](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|A CRM-felhasználói szerepkör a rendszergazda vagy a Rendszertestreszabó.|[Szerepkörök társítása a Dynamics 365-ben](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power automatizáló folyamat fiókja|Hozzon létre egy új éles környezetet egy adatbázissal a teszteléshez, az előkészítéshez és a gyártáshoz. Ha már rendelkezik egy adatbázissal meglévő éles környezettel, azt újra használhatja. Az összekötő megoldás telepítésére jogosult felhasználónak rendelkeznie kell egy automatizáló licenccel, és hozzá kell férnie ehhez a környezethez. Ha a telepítés meghiúsul, a folyamat nyomon követheti az előrehaladást, és további információkat kaphat a [Power automatizáló](https://flow.microsoft.com/) szolgáltatásban. Válassza az **előzmények megtekintése** a **megoldások** alatt lehetőséget.|[Környezet létrehozása vagy kezelése](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>A partneri központ átirányítási szinkronizálásának telepítése a Dynamics 365-hez (Power automatizáló megoldás)

1. Nyissa meg a [Power automatizált](https://flow.microsoft.com), és válassza a **környezetek** lehetőséget a jobb felső sarokban. Ebben a lépésben az elérhető CRM-példányok jelennek meg.

1. Válassza ki a megfelelő CRM-példányt a jobb felső sarokban lévő legördülő listából.

1. Válassza a bal oldalon a **megoldások** elemet.

1. A felső menüben válassza a **AppSource megnyitása** hivatkozást.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="A megnyitott AppSource bemutató képernyőkép.":::

1. Keresse meg a következőt: **partner Center-összekötők a Dynamics 365-hez** az előugró képernyőn.  

1. Válassza a **Letöltés most** gombot, majd kattintson a **Folytatás** gombra.

1. Ekkor megjelenik egy oldal, ahol kiválaszthatja az alkalmazás telepítéséhez szükséges CRM-környezetet (Dynamics 365). Fogadja el a feltételeket és kikötéseket.

1. Nyomon követheti a folyamat előrehaladását, és ha a telepítés meghiúsul, további részleteket a Power automatizáló szolgáltatásban **talál** , ehhez válassza az előzmények megjelenítése a **megoldások** alatt lehetőséget.

1. A telepítés befejezése után lépjen vissza a [Power automatizálás](https://flow.microsoft.com) elemre, és válassza a bal oldalon a **megoldások** elemet. A **Dynamics 365-hez készült fiókpartner-szinkronizálás** mostantól elérhető a **megoldások** listájában.

1. Válassza **a partner Center-átirányítási szinkronizálás a Dynamics 365-hez** lehetőséget. A következő automatizálható energiagazdálkodási folyamatok és entitások érhetők el.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Képernyőkép, amely az elérhető CRM jeleníti meg.":::

## <a name="test-before-you-go-live"></a>Tesztelés az élő indítás előtt

Mielőtt telepítené, konfigurálja és testreszabja az automatizálási megoldást az éles környezetben, mindenképpen tesztelje a megoldást egy átmeneti CRM-példányon. A következőkre lesz szüksége:

- Telepítse a Power automatizáló megoldást egy átmeneti környezet CRM-példányára.
- Az automatizálási megoldás konfigurálása és testreszabása átmeneti környezetben.
- Tesztelje a megoldást egy átmeneti CRM-példányon.
- Sikeres tesztelés után importálja felügyelt megoldásként az éles példányba.

## <a name="configure-the-solution"></a>A megoldás konfigurálása

1. Miután telepítette a megoldást a CRM-példányban, térjen vissza a [Power automatizálás](https://flow.microsoft.com/)szolgáltatáshoz.

1. A jobb felső sarokban található **környezetek** legördülő listából válassza ki azt a CRM-példányt, amelyen az automatizálási megoldást telepítette.

1. Olyan kapcsolatokat kell létrehoznia, amelyek a három felhasználói fiókot rendelik hozzá:

   - A partner Center felhasználója az Ajánlói rendszergazdai hitelesítő adatokkal
   - Partnerközpont – események
   - CRM-rendszergazda a megoldás energiagazdálkodási folyamataival

   1. Válassza a bal oldali **kapcsolatok** lehetőséget, majd a listából válassza ki a **partneri központ átirányítási** megoldását.

   1. Hozzon létre egy-egy kapcsolatokat a **kapcsolatok létrehozása** lehetőség kiválasztásával.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="A kapcsolatok létrehozását bemutató képernyőkép.":::

   1. A jobb felső sarokban található keresési sávban keresse meg a **partneri központ hivatkozásait (előzetes verzió)** .

   1. Hozzon létre kapcsolatot a fiókpartner-felhasználó számára az Ajánlói rendszergazda hitelesítő adatokkal kapcsolatos szerepkörével.

   1. Ezután hozzon létre egy partneri központ-esemény kapcsolatot a partner Center-felhasználó számára az átirányítási rendszergazdai hitelesítő adatokkal.

   1. Hozzon létre egy Common Data Service (aktuális környezet) kapcsolatokat a CRM-rendszergazda felhasználó számára.
     
   1. Az összes kapcsolat hozzáadása után a következő kapcsolatokat kell látnia a környezetben.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="A kapcsolatokat bemutató képernyőkép.":::

## <a name="edit-the-connections"></a>Kapcsolatok szerkesztése

1. Térjen vissza a **megoldások** lapra, és válassza az **alapértelmezett megoldás** lehetőséget. Válassza a **kapcsolatok referenciája (előzetes verzió)** lehetőséget az **összes** kiválasztásával.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="A kapcsolatok szerkesztését bemutató képernyőkép.":::

1. Szerkessze az egyes kapcsolatokat egyenként a három pontot ábrázoló ikonra kattintva. Adja hozzá a megfelelő kapcsolatokat.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="A felsorolt kapcsolatokat bemutató képernyőkép.":::

1.  Térjen vissza a **megoldások** lapra, válassza ki a **Dynamics 365-hez készült fiókpartner-szinkronizálás** lehetőséget, majd kapcsolja be a folyamatot úgy, hogy kijelöli a három pont ikont az egyes folyamatok mellett a következő sorozatban. Ha problémák merülnek fel a folyamat bekapcsolásakor, tekintse meg a [testreszabási lépéseket](connector-dynamics.md#customize-synchronization-steps) és a [hibaelhárítási lépéseket](connectors-troubleshoot.md).

Kapcsolja be a folyamatokat a következő sorozatban:

- A partner Center webhook-regisztrációja (belső előzetes verzió)
- Közös értékesítésre hivatkozó hivatkozás létrehozása – Dynamics 365 – partneri központ (belső előzetes verzió)
- Testreszabása Adatok létrehozása vagy beolvasása a Dynamics 365 flow-ból
- Partneri központ – Dynamics 365 – Helper (Insider előzetes verzió)
- A partner Center Microsoft közös értékesítési hivatkozási frissítései a Dynamics 365-as verzióra (Insider előzetes verzió)
- Partneri központ a Dynamics 365-hoz (belső előzetes verzió)
- Dynamics 365 a partneri központba (belső előzetes verzió)
- Dynamics 365 lehetőség a partneri központhoz (belső előzetes verzió)
- Dynamics 365 Microsoft-megoldások a partner Centerhez (Insider előzetes verzió)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>A webhook API-k használata az Erőforrás-változási események regisztrálásához

A partner Center webhook API-k használatával regisztrálhat az Erőforrás-változási eseményekre. Ezeket a változási eseményeket a rendszer HTTP-bejegyzésekként küldi el az URL-címre.

1. Válassza **a partner központ lehetőséget a Dynamics 365 (belső előzetes verzió)** elemre.

1. Válassza a **Szerkesztés** ikont, majd válassza a **http-kérelem fogadása** lehetőséget.

1. Kattintson a **Másolás** ikonra a megadott http post URL-cím másolásához.

   :::image type="content" source="images/webhook-video.gif" alt-text="Képernyőkép, amely a webhookok használatával regisztrálja az erőforrások változásait.":::

1. Válassza ki a **partneri központ webhook-regisztrációját (Insider Preview)** energiagazdálkodási folyamatát, majd válassza a **Futtatás** lehetőséget.

1. Győződjön meg arról, hogy a jobb oldali ablaktáblán megnyílik a **futtatási folyamat** ablak, majd válassza a **Folytatás** lehetőséget.

1. Adja meg a következő részleteket:

   - **Http-trigger végpontja**: ez az URL-cím egy korábbi lépésből lett másolva.
   - **Regisztrálni kívánt események**: válassza ki az összes elérhető eseményt (**hivatkozó által létrehozott**, **hivatkozó-frissített**, **kapcsolódó-Referral-created**, és **kapcsolódó-Referral-frissítve**).
   - **Felülírja a meglévő trigger-végpontokat, ha vannak** ilyenek?: igen. Egy adott webhook-eseményhez csak egy URL-címet lehet regisztrálni.

1. Válassza a **folyamat futtatása** lehetőséget, majd kattintson a **Kész gombra.**

A webhook mostantól képes figyelni, létrehozni és frissíteni az eseményeket.

## <a name="customize-synchronization-steps"></a>Szinkronizálási lépések testreszabása

A CRM-rendszerek kiemelten testre szabhatók, és a CRM-telepítő alapján testreszabhatja az automatizálási megoldást. Ha a partneri központ és a CRM-rendszer között szinkronizálja a közös értékesítésre mutató hivatkozásokat, a partner Center-számítógépen szinkronizált mezők az [Egyéni mezők leképezési útmutatójában](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)jelennek meg.

Kövesse a mező-hozzárendelési útmutatót, és ha szükséges, hajtsa végre a megfelelő módosításokat a Dynamics 365 flow-vagy környezeti változóinak **létrehozásához vagy lekéréséhez** . Ne frissítse a Power automatizálási megoldás más folyamatait, mert ez hatással lehet a jövőbeli megoldás-frissítésekre.

A következő testreszabások érhetők el:

- Pipa **megjelenítése a lehetőség nevében**: alapértelmezés szerint a lehetőség neve mellett pipa jelenik meg, amely jelzi, hogy a partner központ és a Dynamics 365 CRM közötti szinkronizálás sikeresen megtörténik. Hasonlóképpen, ha a szinkronizálás meghiúsul, megjelenik egy kereszt jel is. Ha el szeretné kerülni a lehetőség nevében az ellenőrzések vagy a keresztes jelek hozzáadását, a **lehetőség neve** környezeti változóban állítsa a nem értékre a megjelenítési pipa aktuális értékét.
- **Ügylet értéke**: alapértelmezés szerint a partneri központ Deal (üzlet) értéke szinkronizálva lesz a CRM-ben lévő **estimatedvalue** és onnan. Ha a CRM-ben egy másik mező van, hogy a Deal érték szinkronizáljon:

  - Frissítse az **üzlet értéke** mezőt a Dynamics 365 környezeti változóban a CRM-mező nevével. Ügyeljen arra, hogy a mező nevét adja meg, ne a megjelenítendő nevét.
  - Szerkesztés **[Testreszabás] a Dynamics 365-folyamat létrehozása vagy lekérése**, majd a CRM-ben a **Létrehozás vagy a frissítés lehetőségre** kattintva frissítheti az **új lehetőséget** , és **frissítheti a meglévő lehetőségek** műveleteit, hogy a **DealValue** értékét a CRM megfelelő mezőjéhez rendelje. Továbbá távolítsa el a **DealValue** -hozzárendelést a **becsült bevétel** mezőből.

- **Ügyfél fiókjának országkód**: kötelező megadni egy kétbetűs ORSZÁGKÓDOT (ISO 3166), amikor új hivatkozót hoz létre. Alapértelmezés szerint az országkód a fiók **address1_country** mezőjéből és a CRM-ben lesz szinkronizálva. Ha a CRM-ben egy másik mező van, hogy az országkód szinkronizálva legyen:

   - A kétbetűs kódot tartalmazó fiók nem lookup országkód mezőjénél:
     - Frissítse az **ügyfél fiók országkód** mező nevét a Dynamics 365 környezeti változóban a CRM-mező nevével. Ügyeljen arra, hogy a mező nevét adja meg, ne a megjelenítendő nevét.
     - Szerkessze **[Customize] a Dynamics 365 folyamat létrehozásával vagy lekérésével kapcsolatos részleteket**, és a CRM-műveletben válassza a **Létrehozás vagy a fiók beszerzése** lehetőséget, hogy az **ország** értékét a CRM megfelelő mezőjéhez rendelje. Továbbá távolítsa el az **ország** értékének hozzárendelését az **1: ország/régió** mezőből.

   - A fiók keresési alapú országkód mezőjénél:
     - Vegyen fel egy új egyéni mezőt a fiókba, és automatikusan töltse ki azt egy kétbetűs országkód (ISO 3166) alapján, a lookup-alapú mezőben kiválasztott értéknek megfelelően, és fordítva.
     - Kövesse a nem keresési országkód mező előző lépéseit, hogy szinkronizáljon egy új egyéni mezőt a CRM-ből és a partneri központból.

- **Lehetőség mezői**: ha vannak olyan kötelezően megadandó mezők **, amelyeket fel** kell tölteni, szerkesztenie kell a (z **) [testreszabás] elemet a Dynamics 365 folyamatból** , majd a CRM-ben a **Létrehozás vagy a frissítés lehetőségre** kell kattintania, és az **új lehetőség létrehozása műveletet** kell megadnia az értékek a kötelező mezőkhöz való hozzárendeléséhez az üzleti követelmények alapján.
- **Érdeklődő mezők**: Ha kötelezően kitöltendő mezők **vannak, amelyeket fel** kell tölteni, szerkesztenie kell a **[testreszabás] elemet a Dynamics 365-folyamatból** , és a CRM-ben a létrehozás **vagy frissítés** elemre kell kattintania, és az **új érdeklődő művelettel** kell megadnia az értékeket a kötelező mezőkhöz az üzleti követelmények alapján.
- **Vevőkód**: Ha egy új hivatkozót szinkronizál a partner KÖZPONTJÁTÓL a CRM-be, az automatizálási megoldás megpróbál megkeresni egy meglévő FIÓKOT a CRM-ben az ügyfél vállalatának neve és az irányítószám használatával. Ha nem talál ilyet, egy új felhasználói fiók jön létre a CRM-ben. A keresési feltételek és az új fiók létrehozási részleteinek frissítéséhez szerkessze a **[Testreszabás] elemet a Dynamics 365-folyamat létrehozásához vagy a részletek lekéréséhez** , majd a CRM-ben hozzon létre **vagy kapjon ügyfél-fiókot** , és **hozzon létre egy Vevőkód**

## <a name="update-environment-variable"></a>Környezeti változó frissítése

Környezeti változó értékének frissítése:

1. Nyissa meg a **megoldások** lapot, és válassza az **alapértelmezett megoldás** lehetőséget. Válassza ki a **környezeti változót** az **összes** kiválasztásával.

1. Válassza ki a környezeti változót a frissíteni kívánt értékhez, majd a három pont ikon használatával válassza a **Szerkesztés** lehetőséget.

1. Frissítse az **aktuális értéket** (ne frissítse az **alapértelmezett értéket**) az **új érték** beállítás használatával, és adja meg az értéket. Az értéknek meg kell egyeznie a változó adattípusával. Az igen vagy a nem adattípus például az igen vagy a No értéket fogja fogadni.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Képernyőkép, amely a környezeti változók frissítését mutatja.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Végpontok közötti kétirányú, közös értékesítésre hivatkozó átirányítás szinkronizálása

Miután telepítette, konfigurálta és testre szabta az automatizálási megoldást, tesztelheti a Dynamics 365 és a partner Center közötti, közös értékesítéssel való átirányítások szinkronizálását.

### <a name="prerequisites"></a>Előfeltételek

Ha szinkronizálni szeretné a partner központ és a Dynamics 365 CRM közötti átirányításokat, az automatizálási megoldás egyértelműen kijelölte a Microsoft-specifikus átirányítási mezőket. Ez az azonosítás lehetővé teszi az értékesítő csapatának, hogy eldöntse, hogy mely ajánlásokat szeretné megosztani a Microsofttal a közös értékesítéshez.

Az egyéni mezők és objektumok készletét a rendszer a megoldás telepítésének részeként adja hozzá. Egy CRM-rendszergazda felhasználónak külön CRM-szakaszt kell létrehoznia a **lehetőség** egyéni mezőivel.

A következő egyéni mezők a CRM szakasz részét képezik:

- **Szinkronizálás a partner centerrel**: a lehetőség a partner központtal való szinkronizálása. Alapértelmezés szerint ennek a mezőnek az értéke nem, és az eladótól explicit módon kell megadni az Igen értéket, hogy megossza a Microsofttal való lehetőséget. A partner központból a CRM-be megosztott új hivatkozásokat Igen értékre állítja a rendszer.
- **Hivatkozási azonosító**: a partner Center-hivatkozáshoz tartozó írásvédett azonosító mező.
- **Referral link**: egy írásvédett hivatkozás a partner Centerben lévő hivatkozáshoz.
- **Hogyan segíthet a Microsoft súgója?**: segítségre van szükség a Microsofttól az átirányításhoz. A közös értékesítéssel való hivatkozás létrehozásához válassza ki a Microsofttól kapott megfelelő súgót. Az ügyfél partneri kapcsolatának hozzá kell tartoznia a közös értékesítésre való hivatkozás létrehozásához. Nem közös értékesítésre hivatkozó hivatkozás létrehozásához ne jelölje be ezt a mezőt. A nem közös értékesítésre hivatkozó átirányítást bármikor átalakíthatja egy közös értékesítésre való átirányításra a megfelelő Súgó szükséges beállítás kiválasztásával.
- A **Microsoft partner Center Referral láthatósága**: válassza ki a partneri központ hivatkozásának láthatóságát. A Microsoft-értékesítők számára elérhetővé téve a nem közös értékesítésre irányuló bejelentések a közös értékesítésre alakíthatók. Ha Microsoft súgóra van szükség, a rendszer alapértelmezés szerint az átirányítást a Microsoft-értékesítők számára látja el. Miután ez a mező láthatóként van megjelölve, nem lehet visszaállítani.
- **Microsoft CRM-azonosító**: Ha a Microsoft létrehoz és elfogad egy közös értékesítési hivatkozást, akkor ez a mező a Microsoft CRM-azonosítójával lesz feltöltve.
- **Termékek: elavult**: ne használja ezt a mezőt, vagy adja hozzá a CRM szakaszhoz. Csak visszamenőleges kompatibilitáshoz érhető el. Ehelyett használja a partner Center-megoldásokat.
- **Naplózás**: írásvédett naplózási nyomvonal a partner Center-hivatkozásokkal való szinkronizáláshoz.
- **Microsoft partner Center-megoldások**: egy egyéni objektum, amellyel közös értékesítésre kész megoldások vagy Microsoft-megoldások társíthatók a lehetőséggel. Egy vagy több megoldás is hozzáadható vagy eltávolítható a lehetőségből. A Microsofttal való megosztás előtt legalább egy közös értékesítésre kész vagy Microsoft-megoldást kell hozzáadni a lehetőséghez. Az objektum a lehetőséghez való hozzárendeléséhez frissítse a **lehetőség** űrlapot a CRM-ben.

  Válassza ki a megfelelő lapot a **lehetőség** űrlapon, és adjon hozzá egy alrácsot az itt látható módon.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Képernyőkép, amely megjeleníti a lehetőség űrlapot.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Képernyőkép, amely a Microsoft-megoldásokat jeleníti meg.":::

- A Microsoft-megoldások hozzáadása után előre feltöltheti a kész megoldások közös értékesítését, így az értékesítőknek nem kell felvenniük őket. Új megoldás részleteinek hozzáadásához nyissa meg a Microsoft megoldás részletei objektumot a CRM-ben, és válassza a **rekord hozzáadása** lehetőséget egy bejegyzés hozzáadásához, vagy **Excel-feltöltés** használatával több bejegyzés hozzáadásához.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Képernyőkép, amely a Microsoft új megoldásának részleteit jeleníti meg.":::

### <a name="scenarios"></a>Forgatókönyvek

1. Az átirányítás szinkronizálása a CRM-ben való létrehozáskor vagy frissítésekor, valamint a partner Centerben szinkronizálva:

   1. Jelentkezzen be a Dynamics 365 CRM-környezetbe azokkal a felhasználókkal, akik a CRM **lehetőség** szakaszában láthatók.

   1. Győződjön meg arról, hogy a **Microsoft partner Center** szakasza új lehetőség a Dynamics 365-környezetben való létrehozásakor jelenik meg.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Képernyőkép, amely új lehetőséget mutat.":::

   1. Ha ezt a lehetőséget a partner centerrel szeretné szinkronizálni, ügyeljen arra, hogy a következő mezőket adja meg a kártya nézetben:

      - **Hogyan lehet a Microsoft súgója?**: egy közös értékesítéssel való hivatkozás létrehozásához válasszon ki egy megfelelő Súgó lehetőséget.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Képernyőkép, amely bemutatja, hogyan lehet beolvasni a megfelelő mezőket a kártyás nézetben.":::

      - **Ügyfél elérhetősége**: egy közös értékesítéssel való hivatkozás létrehozásához vegyen fel egy ügyfél-kapcsolattartót a lehetőséghez.
      - **Szinkronizálás a partner centerrel**: igen.
      - **Microsoft-megoldások**: a Microsofttal való felkérés megosztásához adjon hozzá egy érvényes, közös értékesítésre kész vagy Microsoft-megoldást a lehetőséghez.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="A megoldás AZONOSÍTÓját megjelenítő képernyőkép.":::

   1. Miután létrehozta a lehetőséget a Dynamics 365-ben, és a **szinkronizálás a partner centerrel** beállítás Igen értékre van állítva, várjon 10 percet. Ezután jelentkezzen be a partner Center-fiókjába. Az átirányítási adatokat a Dynamics 365 és az **átirányítási azonosító** fogja szinkronizálni. Az **átirányítási hivatkozás** fel lesz töltve. Ha hiba lép fel, a rendszer a **naplózási** mezőt a hiba adataival tölti fel.
     
    1. Hasonlóképpen, ha a Dynamics 365 CRM-ben frissíti a lehetőséget a **partner centerrel való szinkronizálással** , akkor a módosításokat a rendszer a fiókpartner-fiókjában szinkronizálja.

    1. A partner centerrel sikeresen szinkronizált lehetőségek a Dynamics 365-as ✔ ikonnal lesznek azonosítva.

1. Az átirányítás szinkronizálása a partner Centerben létrehozott vagy frissített hivatkozással, és a Dynamics 365 környezetben szinkronizálva:

   1. Jelentkezzen be a partner Center- [irányítópultra](https://partner.microsoft.com/dashboard/home).

   1. A bal oldali menüben válassza a **hivatkozók** lehetőséget.

   1. Hozzon létre egy új, közös értékesítésre vonatkozó hivatkozást a partner Centerből az **új ajánlat** lehetőség kiválasztásával.

   1. Jelentkezzen be a Dynamics 365 CRM-környezetbe.

   1. **Nyissa meg a lehetőségeket**. A partner Centerben létrehozott hivatkozás mostantól szinkronizálva van a Dynamics 365 CRM-ben.

   1. Amikor kijelöl egy szinkronizált átirányítást, a rendszer feltölti a kártya nézetének részleteit.

## <a name="next-steps"></a>Következő lépések

- [Érdeklődők kezelése](manage-leads.md)
- [Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)
- [További információ a Microsoft Power automatizáló platformról](/power-automate/)
- [Partnerközpont – webhookok](/partner-center/develop/partner-center-webhooks)
