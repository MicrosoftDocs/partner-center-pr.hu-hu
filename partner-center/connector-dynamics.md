---
title: A Dynamics 365 CRM-partneri központ közös értékesítési összekötője
ms.topic: how-to
ms.date: 02/16/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Szinkronizálja a partner Centerben lévő hivatkozásokat a Dynamics 365 CRM-hez készült közös értékesítési összekötővel. Az értékesítők ezután a Microsofttal közösen értékesíthetők a CRM-rendszereken belül.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: e465130b96886cf2bb77bcd94f56c1a12545a5d5
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645772"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Közös értékesítésű összekötő a Dynamics 365 CRM-hez – áttekintés

### <a name="appropriate-roles"></a>Megfelelő szerepkörök

- Ajánlói rendszergazda
- Rendszerfelügyeleti webszolgáltatások vagy Rendszertestreszabó a CRM-ben

A partner Center közös értékesítési összekötője lehetővé teszi, hogy az értékesítők a Microsofttal közösen értékesítsenek a CRM-rendszereken belül. Nem kell kiképezniük, hogy a partner centerrel együtt kezeljék a közös értékesítési ajánlatokat. A közös értékesítésű összekötők használatával létrehozhat egy új, közösen értékesíthető hivatkozást a Microsoft-értékesítők bevonásához, a Microsoft-értékesítőtől kapott hivatkozásokat fogad, elfogadhatja/elutasíthatja az átirányítást, módosíthatja az ügyleti értékeket, például az üzlet értékét és a zárási dátumot. Ezeket a közös értékesítési ajánlatokat a Microsoft-értékesítők frissítései is megkapják. Az Ön által választott CRM-ben kezelheti az összes átirányítási munkát, nem pedig a partner Centerben. 

A megoldás a Microsoft Power automatizálási megoldásán alapul, és a partner Center API-kat használja.

## <a name="before-you-install---pre-requisites"></a>Az Előfeltételek telepítése előtt

|**Témakörök**   |**Részletek**   |**Hivatkozások**   |
|--------------|--------------------|------|
|Microsoft Partner Network azonosítója |Érvényes MPN-AZONOSÍTÓra van szüksége|Az [MPN](https://partner.microsoft.com/) csatlakoztatása|
|Értékesítésre kész|Az IP-/szolgáltatási megoldásnak közös értékesítéssel kell rendelkeznie.|[Értékesítés a Microsofttal](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnerközpont-fiók|A partner Center-bérlőhöz társított MPN-AZONOSÍTÓnak meg kell egyeznie a közös értékesítési megoldáshoz társított MPN-azonosítóval. Az összekötők üzembe helyezése előtt győződjön meg arról, hogy a partner Center portálon megtekintheti a közös értékesítéssel kapcsolatos hivatkozásokat.|[Saját fiók kezelése](create-user-accounts-and-set-permissions.md)|
|A partner Center felhasználói szerepkörei|Az összekötőket telepítő és használó alkalmazottnak hivatkozói rendszergazdának kell lennie|[Felhasználói szerepkörök és engedélyek hozzárendelése](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|A CRM-felhasználói szerepkör a rendszergazda vagy a rendszertestreszabó|[Szerepkörök társítása a Dynamics 365-ben](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power automatizáló folyamat fiókja|Hozzon létre új éles környezetet az adatbázissal tesztelési, előkészítési és éles környezetben. Ha van meglévő éles környezete az adatbázissal, akkor újra felhasználható. Az összekötő-megoldást telepítő felhasználónak automatizálnia kell a szükséges energiagazdálkodási licencet, és hozzá kell férnie ehhez a környezethez. Nyomon követheti a folyamat előrehaladását, és további részleteket is megtudhat, ha a telepítés nem sikerül a [Power gyorsbüféban](https://flow.microsoft.com/) , ha az előzmények megtekintése elemre kattint|[Környezet létrehozása vagy kezelése](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>A partneri központ átirányítási szinkronizálásának telepítése a Dynamics 365-hez (Power automatizáló megoldás)

1. Nyissa meg a [Power Automatet](https://flow.microsoft.com) , és válassza a **környezetek** lehetőséget a jobb felső sarokban. Ebben a lépésben az elérhető CRM-példányok jelennek meg.

2. Válassza ki a megfelelő CRM-példányt a jobb felső sarokban lévő legördülő menüből.

3. A bal oldali navigációs sávon válassza a **megoldások** elemet.

4. Kattintson a felső menüben található **AppSource megnyitása** hivatkozásra.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource megnyitása":::

5. Keressen rá a Dynamics365-hez készült **partner Center-összekötők** az előugró képernyőn.  

6. Kattintson a **Letöltés most** gombra, és **folytassa a művelettel**.

7. Ekkor megnyílik a lap, amelyen kiválaszthatja az alkalmazás telepítéséhez szükséges CRM-környezetet (Dynamics 365).  Fogadja el a feltételeket és a kikötéseket.

8. Nyomon követheti a folyamat előrehaladását, és további részleteket is megtudhat, ha a telepítés nem sikerül a Power Gyorsbüféban, ha az **előzmények megtekintése** **elemre** kattint
 

9. A telepítés befejezése után váltson vissza a [Power automatizálás](https://flow.microsoft.com) szolgáltatásra, és válassza a bal oldali navigációs terület **megoldásait** . Figyelje meg, hogy a **partneri központ a Dynamics 365-szinkronizálása** elérhető a megoldások listájában.

10. Válassza **a partner Center-átirányítási szinkronizálás a Dynamics 365-hez** lehetőséget. A következő energiagazdálkodási folyamatok és entitások érhetők el:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Rendelkezésre álló CRM":::

## <a name="best-practice-test-before-you-go-live"></a>Ajánlott eljárás: tesztelés az élő indítás előtt

Mielőtt telepítené, konfigurálja és testreszabja az automatizálási megoldást az éles környezetben, mindenképpen tesztelje a megoldást egy átmeneti CRM-példányon.

- Telepítse a Microsoft Power automatizáló megoldást átmeneti környezetben vagy CRM-példányon.
- Konfigurálja és szabja testre a Microsoft Power automatizáló megoldást az átmeneti környezetben.
- Tesztelje a megoldást egy átmeneti vagy CRM-példányon. 
- Sikeres, az importálás felügyelt megoldásként az éles példányra. 

## <a name="configure-the-solution"></a>A megoldás konfigurálása

1. Miután telepítette a megoldást a CRM-példányba, váltson vissza a [Power automatizálás](https://flow.microsoft.com/)szolgáltatásra.


2. A jobb felső sarokban található **környezetek** legördülő listából válassza ki azt a CRM-példányt, amelyen az automatizálási megoldást telepítette.

3. Olyan kapcsolatokat kell létrehoznia, amelyek a három felhasználói fiókot rendelik hozzá:

   - A partner Center felhasználója az Ajánlói rendszergazdai hitelesítő adatokkal

   - Partnerközpont – események

   - A CRM-rendszergazda a megoldásban a Power automatizálja a folyamatokat.

      1. Válassza a bal oldali navigációs sávon a **kapcsolatok** lehetőséget, majd a listából válassza ki a "partner-központra hivatkozó" megoldást.

      2. Hozzon létre egy kapcsolatokat a **kapcsolatok létrehozása** lehetőségre kattintva.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Kapcsolat létrehozása":::

      3. A jobb felső sarokban található keresési sávban keresse meg a **partneri központ hivatkozásait (előzetes verzió)** .

      4. Hozzon létre kapcsolatot a fiókpartner-felhasználó számára az Ajánlói rendszergazda hitelesítő adatokkal kapcsolatos szerepkörével.

      5. Ezután hozzon létre egy partneri központ-esemény kapcsolatot a partner Center-felhasználó számára az Ajánlói rendszergazda hitelesítő adataival.

      6. Hozzon létre egy Common Data Service (aktuális környezet) kapcsolatokat a CRM-rendszergazda felhasználó számára.
     
      7. Az összes hozzáadott kapcsolat után a következő kapcsolatokat kell látnia a környezetben:

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Kapcsolatok":::
   
## <a name="edit-the-connections"></a>Kapcsolatok szerkesztése

1. Térjen vissza a **megoldások** lapra, és válassza az **alapértelmezett megoldás** lehetőséget. Válassza a **kapcsolatok referenciája (előzetes verzió)** lehetőséget az **összes** elemre kattintva.

:::image type="content" source="images/cosellconnectors/dynamics-3.png" alt-text="Kapcsolódás":::

2. Szerkessze az egyes kapcsolatokat egyenként a három pont ikon kiválasztásával. Adja hozzá a megfelelő kapcsolatokat.

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Felsorolt kapcsolatok"::: 

3.  Térjen vissza a megoldások lapra, válassza ki a Dynamics 365-hez készült fiókpartner-szinkronizálás lehetőséget, majd kapcsolja be a folyamatot úgy, hogy az egyes folyamatok melletti három pont ikonra kattint az alábbi sorozatban. Ha a folyamat bekapcsolásakor problémákba ütközik, tekintse meg a [testreszabási lépéseket](connector-dynamics.md#customize-synchronization-steps) és a [hibaelhárítási lépéseket](connectors-troubleshoot.md). 

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

A partner Center webhook API-k lehetővé teszik az Erőforrás-változási események regisztrálását. Ezeket a változási eseményeket a rendszer HTTP-bejegyzésekként küldi el az URL-címre.

1. Válassza **a partner központ lehetőséget a Dynamics 365 (belső előzetes verzió)** elemre.

2. Válassza a **Szerkesztés** ikont, és válassza ki a **http-kérés fogadásakor** lehetőséget.

3. Kattintson a **Másolás** ikonra a megadott http post URL-cím másolásához.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL-cím másolása":::

4. Most válassza ki a "partneri központ webhook-regisztráció (Insider előzetes verzió)" energiaellátás-automatizálási folyamat elemet, és válassza a **Futtatás** lehetőséget.

5. Győződjön meg arról, hogy a jobb oldali ablaktáblán megnyílik a "Futtatás folyamata" ablak, és kattintson a **Folytatás** gombra.

6. Adja meg a következő részleteket:

   - **Http-trigger végpontja**: a korábbi lépésből másolt URL-cím

   - **Regisztrálni kívánt események**: válassza ki az összes elérhető eseményt ("hivatkozó által létrehozott", "referral-frissítve", "kapcsolódó-hivatkozó-létrehozva", "kapcsolódó utasítások – frissítve")

   -**Meglévő eseményindító-végpontok felülírása, ha** van: igen, fontos megjegyezni, hogy egy adott webhook-eseményhez csak egy URL-cím regisztrálhat. Fontos megjegyezni, hogy egy adott webhook-eseményhez csak egy URL-címet lehet regisztrálni. 

7. Válassza a **Futtatás** lehetőséget, majd kattintson a **Kész gombra.**

A webhook mostantól figyelheti az események létrehozását és frissítését.

## <a name="customize-synchronization-steps"></a>Szinkronizálási lépések testreszabása

A CRM-rendszerek kiemelten testre szabhatók, és a CRM-telepítő alapján testreszabhatja az automatizálási megoldást.  Ha a partneri központ és a CRM-rendszer között szinkronizálja a közös értékesítésre mutató hivatkozásokat, a partner Center-számítógépen szinkronizált mezők az [Egyéni mezők leképezési útmutatójában](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)jelennek meg.

Kövesse a mező-hozzárendelési útmutatót, és ha szükséges, hajtsa végre a megfelelő módosításokat a Dynamics 365 flow-vagy környezeti változóinak **létrehozásához vagy lekéréséhez**  . Azt javasoljuk, hogy ne frissítsen semmilyen más folyamatot a Power automatizáló megoldásban, mivel az befolyásolhatja a jövőbeli megoldások frissítéseit. 

Az elérhető testreszabások a következők:

- Bejelölési lehetőség neve: alapértelmezés szerint a lehetőség neve mellett pipa jelenik meg, amely jelzi, hogy a partner központ és a Dynamics 365 CRM közötti szinkronizálás sikeresen megtörténik. Hasonlóképpen, ha a szinkronizálás meghiúsul, megjelenik egy kereszt jel is. Ha nem szeretné, hogy a lehetőség neve vagy a kereszt megjelölés legyen megadva, a lehetőség neve környezeti változóban állítsa a nem értékre a megjelenítési pipa aktuális értékét.

- Az ügylet értéke: alapértelmezés szerint a partner Center **estimatedvalue** a CRM-ben és a-ben szinkronizálva lesz. Ha a CRM-ben egy másik mező van, hogy a Deal érték szinkronizálva legyen:

    a.    Frissítse a Deal Value mező nevét a Dynamics 365 környezeti változóban a CRM-mező nevével. Vegye figyelembe, hogy a mező nevét nem a megjelenítendő név alapján kell megadnia.

    b.    Szerkesztés **[Testreszabás] a Dynamics 365 folyamat létrehozása vagy lekérése**  , majd a CRM-ben a **Létrehozás vagy a frissítés** lehetőségre kattintva a frissítés **új lehetőség** létrehozása és a **meglévő lehetőségekkel** kapcsolatos műveletek frissítése a **DealValue** érték kiosztásához a CRM-ben. Emellett távolítsa el a **DealValue-hozzárendelést** a **becsült bevétel** mezőből.

- Ügyfél fiókjának országkód: kötelező megadni egy kétbetűs országkódot (ISO 3166) egy új hivatkozás létrehozásakor. Alapértelmezés szerint az országkód szinkronizálva lesz a fiók address1_country mezőjével a CRM-ben. Ha a CRM-ben egy másik mező van a következővel való szinkronizáláshoz:

   a.    A nem keresési országkód mező esetében, amely két betűből álló kódot tartalmaz:

   - Frissítse az ügyfél fiók országkód mezőjének nevét a Dynamics 365 környezeti változóban a CRM-mező nevével. Vegye figyelembe, hogy a mező nevét nem a megjelenítendő név alapján kell megadnia.

   - Szerkesztés **[Testreszabás] a Dynamics 365 folyamat létrehozása vagy lekérése**  , majd a CRM-ben az ország értékének megfelelő mezőhöz való hozzárendeléséhez navigáljon a CRM-ben a létrehozás vagy a fiók beszerzése elemre. Továbbá távolítsa el az ország értékének hozzárendelését az 1. hely: ország/régió mezőből.

   b.    Keresési alapú országkód mező a következő fiókban:

   - Vegyen fel egy új egyéni mezőt a fiókba, és automatikusan feltöltse azt kétbetűs országkód (ISO 3166) alapján, a keresési alapú mezőben kiválasztott érték és fordítva.

   - A nem keresési országkód mezőhöz tartozó lépések végrehajtásával szinkronizálja az új egyéni mezőt a CRM-ből és a partner központjából.

- Lehetőség mezői: ha vannak olyan kötelező mezők, amelyeknek fel kell tölteniük a Szerkesztés **[Testreszabás] elemet, vagy le kell kérni a Dynamics 365-folyamat adatait**  , majd navigáljon a **Létrehozás vagy a frissítés lehetőségre** a CRM-ben, és az **új lehetőség létrehozása művelettel** rendeljen értékeket a kötelező mezőkhöz az üzleti követelmények alapján.

- Érdeklődő mezők: ha vannak kötelezően kitöltendő mezők az érdeklődőben, amelyeket fel kell töltenie **[Testreszabás] létrehozás vagy a részletek beolvasása a Dynamics 365 folyamatból**  , majd navigáljon a CRM-beli **érdeklődő létrehozása vagy frissítése** elemre, és frissítsen **egy új érdeklődői műveletet** az értékek a kötelező mezőkhöz való hozzárendeléséhez az üzleti követelmények alapján.

- Vevőkód: Ha egy új hivatkozót szinkronizál a partner központjától a CRM-be, az automatizálási megoldás megpróbál egy meglévő fiókot keresni a CRM-ben az ügyfél vállalatának neve és az irányítószám alapján. Ha nem talál ilyet, a rendszer új felhasználói fiókot hoz létre a CRM-ben. A keresési feltételek és az új fiók létrehozási részleteinek frissítéséhez szerkessze a **[Testreszabás] elemet a Dynamics 365 folyamat alapján** , és navigáljon a CRM-beli **ügyfél-fiók létrehozása vagy lekérése** **művelethez, és hozzon létre egy ügyfél-fiók műveletet**.

## <a name="update-environment-variable"></a>Környezeti változó frissítése

Környezeti változó értékének frissítése:

1. Nyissa meg a **megoldások** lapot, és válassza az **alapértelmezett megoldás** lehetőséget. A minden elemre kattintva válassza ki a **környezeti változót** .

2. Válassza ki a környezeti változót a frissíteni kívánt értékhez, majd kattintson a **Szerkesztés** gombra három pont ikon használatával.

3. Frissítse az **aktuális értéket** (ne frissítse az alapértelmezett értéket) **új érték** beállítással, és adja meg az értéket. Az értéknek meg kell egyeznie a változó adattípusával, például az igen/nem adattípus esetén az igen vagy a No érték lesz elfogadva.

:::image type="content" source="images/cosellconnectors/dynamics-5.png" alt-text="Alapértelmezett értékekhez tartozó mező szerkesztése":::

- Végpontok közötti kétirányú, közös értékesítésre hivatkozó átirányítás szinkronizálása

Miután telepítette, konfigurálta és testreszabta az automatizálási megoldást, tesztelheti a Dynamics 365 és a partner Center közötti összekapcsolási átirányítások szinkronizálását.

### <a name="pre-requisites"></a>Előfeltételek

Ha szinkronizálni szeretné a partner központ és a Dynamics 365 CRM közötti átirányításokat, az automatizálási megoldás egyértelműen kijelölte a Microsoft-specifikus átirányítási mezőket. Ez az azonosítás lehetővé teszi az értékesítő csapatának, hogy eldöntse, hogy mely ajánlásokat szeretné megosztani a Microsofttal a közös értékesítéshez.

Az egyéni mezők és objektumok készlete a megoldás telepítésének részeként lesz hozzáadva. Egy CRM-rendszergazda felhasználónak külön CRM-szakaszt kell létrehoznia a **lehetőség** egyéni mezőivel.

A következő egyéni mezők a CRM szakasz részét képezik:

- **Szinkronizálás a partner centerrel**: legyen szó a Microsoft partner centerrel való szinkronizálásról. Alapértelmezés szerint ennek a mezőnek az értéke nem, és az eladótól explicit módon kell megadni az Igen értéket, hogy megossza a Microsofttal való lehetőséget. A partner központból a CRM-be megosztott új hivatkozásokat Igen értékre állítja a rendszer.

- **Hivatkozási azonosító**: a Microsoft partner Center ajánlójának írásvédett azonosító mezője

- **Referral link**: egy csak olvasható hivatkozás a Microsoft partner Centerben
- **Hogyan segíthet a Microsoft súgója?**: segítségre van szükség a Microsofttól az átirányításhoz. Ha közös értékesítésre vonatkozó hivatkozást szeretne létrehozni, válassza a Microsoft által igényelt megfelelő súgót. Az ügyfél partneri kapcsolatának hozzá kell tartoznia a közös értékesítésre való hivatkozás létrehozásához. Nem közös értékesítésű hivatkozás létrehozásához hagyja ezt a mezőt kiválasztva. A nem közös értékesítéssel való átadásra a megfelelő Súgó szükséges beállítás kiválasztásával bármikor átalakítható a közös értékesítésre való utalás.

- A **Microsoft partner Center Referral láthatósága**: válassza a láthatóság lehetőséget a Microsoft partner Center-hivatkozáshoz. A Microsoft-értékesítők számára a nem értékesíthető hivatkozásokat a közös értékesítésre lehet átalakítani. Ha Microsoft súgóra van szükség, az átirányítási szolgáltatás alapértelmezés szerint a Microsoft-értékesítők számára látható. Ha láthatóként jelölte meg ezt a mezőt, nem lehet visszaállítani.

- **Microsoft CRM-azonosító**: Ha a Microsoft létrehoz és elfogad egy közös értékesítési hivatkozást, akkor ez a mező a Microsoft CRM-azonosítójával lesz feltöltve.

- **Termékek: elavult** – ne használja ezt a mezőt, vagy vegye fel a CRM szakaszba, csak visszamenőleges kompatibilitás érdekében. Használja helyette a Microsoft partner Center-megoldásokat.

- **Naplózás**: írásvédett naplózási nyomvonal a partner Center-hivatkozásokkal való szinkronizáláshoz

- **Microsoft partner Center-megoldások**: egy egyéni objektum, amellyel közös értékesítésre kész megoldások vagy Microsoft-megoldások társíthatók a lehetőséggel. Egy vagy több megoldás is hozzáadható és/vagy eltávolítható a lehetőségből. A Microsofttal való megosztás előtt legalább egy közös értékesítésre kész vagy Microsoft-megoldást kell hozzáadni a lehetőséghez. Az objektum lehetőséghez való hozzárendeléséhez frissítse a lehetőség űrlapot a CRM-ben:

  Válassza ki a megfelelő lapot a lehetőség űrlapon, és adjon hozzá egy alhálózatot az alább látható módon:

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Lehetőség űrlapja":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::



- A Microsoft-megoldások hozzáadása után előre feltöltheti a kész megoldások közös értékesítését, így az értékesítőknek nem kell felvenniük őket. Új megoldás részleteinek hozzáadásához nyissa meg a CRM-ben a Microsoft megoldás részletei objektumot, és kattintson a **rekord hozzáadása** lehetőségre egy bejegyzés hozzáadásához vagy az **Excel-feltöltéshez** több bejegyzés hozzáadásához.

:::image type="content" source="images/dynamic-1a.png" alt-text="Megoldás részletei":::

### <a name="scenarios"></a>FORGATÓKÖNYVEK

1. Átirányítás szinkronizálása a CRM-ben való létrehozáskor vagy frissítésekor, valamint a partner Centerben szinkronizálva:

   1. Jelentkezzen be a Dynamics 365 CRM-környezetbe azokkal a felhasználókkal, akik a CRM **lehetőség** szakaszában láthatók.

   2. Győződjön meg arról, hogy a Microsoft partner Center szakasza akkor jelenik meg, amikor új lehetőséget hoz létre a Dynamics 365 környezetben

   :::image type="content" source="images/dynamic-2a.png" alt-text="Új lehetőség"::: 

   3. Ha ezt a lehetőséget a partner centerrel szeretné szinkronizálni, ügyeljen arra, hogy a következő mezőket adja meg a kártya nézetben:

      - **Hogyan teheti a Microsoft segítségét?**: egy közös értékesítésre hivatkozó hivatkozás létrehozásához válasszon egy megfelelő Súgó lehetőséget.

         :::image type="content" source="images/dynamic-3a.png" alt-text="A megfelelő mezők beolvasása a kártya nézetben":::

      - **Ügyfél elérhetősége**: a közös értékesítéssel való hivatkozás létrehozásához vegyen fel egy ügyfél-kapcsolatfelvételt a lehetőségbe.
      - **Szinkronizálás a partner centerrel**: igen

      - Microsoft-megoldások: a Microsofttal való felkérés megosztásához adjon hozzá egy érvényes, közös értékesítésre kész vagy Microsoft-megoldást a lehetőséghez.
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="Megoldás azonosítója":::

   4. Miután létrejött a lehetőség a Dynamics 365-ben a partner centerrel való szinkronizálással beállítás Igen értékre van állítva, várjon 10 percet, majd jelentkezzen be a partner Center-fiókjába. Az átirányítási adatokat a Dynamics 365 és az átirányítási azonosító fogja szinkronizálni. Az átirányítási hivatkozás fel lesz töltve. Hiba esetén a naplózási mező a hiba adataival lesz feltöltve.
     
    5. Hasonlóképpen, ha a Dynamics 365 CRM-ben a lehetőség frissítésével "igen" értékre állította a "szinkronizálás a partneri központtal" beállítást, a rendszer szinkronizálja a módosításokat a partner Center-fiókban.

    6. A partner centerrel sikeresen szinkronizált lehetőségek a Dynamics 365-as ✔ ikonnal lesznek azonosítva.

2. Az átirányítás szinkronizálása a Microsoft partner Centerben, a Dynamics 365 környezetben szinkronizálva:

   1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/home).

   2. A bal oldali menüben válassza a **hivatkozók** lehetőséget.

   3. Hozzon létre egy új, közös értékesítésre vonatkozó hivatkozást a partner Centerből az  **új ajánlat** lehetőség kiválasztásával.

   4. Jelentkezzen be a Dynamics 365 CRM-környezetbe.

   5. Navigáljon a **lehetőségek megnyitásához**. A Microsoft partner Centerben létrehozott hivatkozás mostantól szinkronizálva van a Dynamics 365 CRM-ben.

   6. Amikor kijelöl egy szinkronizált átirányítást, a rendszer feltölti a kártya nézetének részleteit.

## <a name="next-steps"></a>Következő lépések

- [Érdeklődők kezelése](manage-leads.md)

- [Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)

- [További információ a Microsoft Power automatizáló platformról?](/power-automate/)

- [Partnerközpont – webhookok](/partner-center/develop/partner-center-webhooks)