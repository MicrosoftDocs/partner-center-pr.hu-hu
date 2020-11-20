---
title: A Salesforce CRM-partneri központ közös értékesítési összekötője
ms.topic: how-to
ms.date: 09/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Szinkronizálja az átirányítási adatokat a Salesforce CRM-tel. Az értékesítők ezután a Microsofttal közösen értékesíthetők a CRM-rendszereken belül.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b73f0b24538daa18b93fa206fce5eda1ab9bc9b9
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947851"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Közös értékesítési összekötő a Salesforce CRM-hez – áttekintés

### <a name="appropriate-roles"></a>Megfelelő szerepkörök

- Ajánlói rendszergazda
- Rendszerfelügyeleti webszolgáltatások vagy Rendszertestreszabó a CRM-ben

A partner Center közös értékesítési összekötője lehetővé teszi, hogy az értékesítők a Microsofttal közösen értékesítsenek a CRM-rendszereken belül. Nem kell kiképezniük, hogy a partner centerrel együtt kezeljék a közös értékesítési ajánlatokat. A közös értékesítésű összekötők használatával új, közösen értékesíthető hivatkozást hozhat létre a Microsoft-értékesítők bevonásához, a Microsoft-értékesítőtől kapott hivatkozásokat, az átirányítások elfogadását/elutasítását, az ügyleti adatok módosítását, például az ügyleti értéket és a zárási dátumot.  Ezeket a közös értékesítési ajánlatokat a Microsoft-értékesítők frissítései is megkapják. Az összes átirányítási munkát elvégezheti, miközben a választott CRM-en belül dolgozik, nem pedig a partner Centerben. 

A megoldás a Microsoft Power automatizálási megoldásán alapul, és a partner Center API-kat használja.

## <a name="before-you-install---pre-requisites"></a>Az Előfeltételek telepítése előtt

|**Témakörök**   |**Részletek**   |**Hivatkozások**   |
|--------------|--------------------|------|
|Microsoft Partner Network azonosítója |Érvényes MPN-AZONOSÍTÓra van szüksége|Az [MPN](https://partner.microsoft.com/) csatlakoztatása|
|Közös értékesítés kész|Az IP-/szolgáltatási megoldásnak közös értékesítéssel kell rendelkeznie.|[Értékesítés a Microsofttal](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnerközpont-fiók|A partner Center-bérlőhöz társított MPN-AZONOSÍTÓnak meg kell egyeznie a közös értékesítési megoldáshoz társított MPN-azonosítóval. Az összekötők üzembe helyezése előtt győződjön meg arról, hogy a partner Center portálon megtekintheti a közös értékesítéssel kapcsolatos hivatkozásokat.|[Saját fiók kezelése](create-user-accounts-and-set-permissions.md)|
|A partner Center felhasználói szerepkörei|Az összekötőket telepítő és használó alkalmazottnak hivatkozói rendszergazdának kell lennie|[Felhasználói szerepkörök és engedélyek hozzárendelése](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|A CRM-felhasználói szerepkör a rendszergazda vagy a rendszertestreszabó|[Szerepkörök társítása a Salesforce CRM-ben](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power automatizáló folyamat fiókja|Aktív [Power automatizáló](https://flow.microsoft.com) fiók a CRM rendszer-rendszergazda vagy Rendszertestreszabó számára. A telepítés előtt a felhasználónak legalább egyszer be kell jelentkeznie az [energiagazdálkodásba](https://flow.microsoft.com) .|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>A Salesforce-csomag telepítése a Microsoft egyéni mezőihez 

Ha szinkronizálni szeretné az átirányításokat a partner Center és a Salesforce CRM között, akkor az automatizálási megoldásnak egyértelműen azonosítania kell a Microsoft-specifikus átirányítási mezőket. Ezzel a kijelöléssel a partner értékesítői csapatai eldönthetik, hogy mely ajánlásokat szeretnék megosztani a Microsofttal a közös értékesítéshez.

1. A Salesforce-ben aktiválja a **megjegyzéseket** , és adja hozzá a lehetőségek kapcsolódó listához. 
[Referencia](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Aktiválja a **lehetőség csapatait** a következő lépések végrehajtásával: 
    - A telepítőben a **gyors keresés** mező használatával keresse meg a lehetőség csapatának beállításait.
    - Szükség szerint adja meg a beállításokat.
[Referencia](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. A Salesforce-ben telepítse az egyéni mezőket és objektumokat az alábbi Package Installer használatával.
  
[Ide](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) kattintva telepítheti a csomagot bármely vállalatba:


Megjegyzés: Ha egy sandbox-ba telepít, az URL kezdeti részét le kell cserélnie a http://test.salesforce.com

4. A Salesforce-ben adja hozzá a Microsoft-megoldásokat a **lehetőséghez** kapcsolódó listához. A Hozzáadás után kattintson a **csavarkulcs** ikonra és a frissítés tulajdonságai elemre.

## <a name="best-practice-test-before-you-go-live"></a>Ajánlott eljárás: tesztelés az élő indítás előtt

Mielőtt telepítené, konfigurálja és testreszabja az automatizálási megoldást az éles környezetben, mindenképpen tesztelje a megoldást egy átmeneti CRM-példányon.

- Telepítse a Microsoft Power automatizáló megoldást átmeneti környezetben vagy CRM-példányon.

- Készítsen másolatot a megoldásról, és futtassa a konfigurációt és a Power automatizálja a folyamatokat az átmeneti környezetben.

- Tesztelje a megoldást egy átmeneti vagy CRM-példányon.

- Sikeres, az importálás felügyelt megoldásként az üzemi példányra.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>A Salesforce CRM-hez készült partner Center-átirányítási szinkronizálás telepítése

1. Nyissa meg a [Power Automatet](https://flow.microsoft.com) , és válassza a **környezetek** lehetőséget a jobb felső sarokban. Ekkor megjelenik az elérhető CRM-példányok.

2. Válassza ki a megfelelő CRM-példányt a jobb felső sarokban lévő legördülő menüből.

3. A bal oldali navigációs sávon válassza a **megoldások** elemet.

4. Kattintson a felső menüben található **AppSource megnyitása** hivatkozásra.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource megnyitása":::

5. Keressen rá a Salesforce-hez készült **partner Center-összekötők** az előugró képernyőn.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Kattintson a **Letöltés most** gombra, és **folytassa a művelettel**.

7. Ekkor megnyílik a lap, amelyen kiválaszthatja az Salesforce CRM-környezetet az alkalmazás telepítéséhez.  Fogadja el a feltételeket és a kikötéseket.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Rendelkezésre álló CRM":::

8. Ezután átirányítja a **megoldások kezelése** lapra.  A lap alján található nyílgombok segítségével navigáljon a "partneri központhoz". A **telepítés ütemezése** a partner Center Referrals megoldás mellett jelenik meg. A telepítés 10-15 percet vesz igénybe.

9. A telepítés befejezése után váltson vissza a [Power automatizálás](https://flow.microsoft.com) szolgáltatásra, és válassza a bal oldali navigációs terület **megoldásait** . Figyelje meg, hogy a **Salesforce-hez készült fiókpartner-szinkronizálás** a megoldások listájában érhető el.

10. Válassza ki **a partneri központ átirányítási szinkronizálása Salesforce** lehetőséget. A következő energiagazdálkodási folyamatok és entitások érhetők el:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce folyamatok":::



## <a name="configure-the-solution"></a>A megoldás konfigurálása

1. Miután telepítette a megoldást a CRM-példányba, váltson vissza a [Power automatizálás](https://flow.microsoft.com/)szolgáltatásra.

2. A jobb felső sarokban található **környezetek** legördülő listából válassza ki azt a CRM-példányt, amelyen az automatizálási megoldást telepítette.
3. A három felhasználói fiókot összekapcsoló kapcsolatokat kell létrehoznia:
    - A partner Center felhasználója az Ajánlói rendszergazdai hitelesítő adatokkal
    - Partnerközpont – események
    - A CRM-rendszergazda a megoldásban a Power automatizálja a folyamatokat.
4. Válassza a bal oldali navigációs sávon a **kapcsolatok** lehetőséget, majd a listából válassza ki a "partner-központra hivatkozó" megoldást.

5. Hozzon létre egy kapcsolatokat a **kapcsolatok létrehozása** lehetőségre kattintva.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Kapcsolat létrehozása":::

- A jobb felső sarokban található keresési sávban keresse meg a partner Center-hivatkozásokat (előzetes verzió).

- Hozzon létre kapcsolatot a fiókpartner-felhasználó számára az Ajánlói rendszergazda hitelesítő adatokkal kapcsolatos szerepkörével.

-  Ezután hozzon létre egy partneri központ-esemény kapcsolatot a partner Center-felhasználó számára az Ajánlói rendszergazda hitelesítő adataival.

- Hozzon létre egy Salesforce-kapcsolatokat a CRM-rendszergazda felhasználó számára.

-  Az összes hozzáadott kapcsolat után a következő kapcsolatokat kell látnia a környezetben:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Kapcsolatok megfigyelése":::

### <a name="edit-the-connections"></a>Kapcsolatok szerkesztése

1. Térjen vissza a megoldások lapra, és válassza az **alapértelmezett megoldás** lehetőséget.  Válassza a **kapcsolatok referenciája (előzetes verzió)** lehetőséget az **összes** elemre kattintva.
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Összekötők szerkesztésének megkezdése":::

2. Szerkessze az egyes kapcsolatokat egyenként a három pont ikon kiválasztásával. Adja hozzá a megfelelő kapcsolatokat.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Összekötők szerkesztése":::

3. Kapcsolja be a folyamatokat a következő sorozatban:

- A partner Center webhook-regisztrációja (belső előzetes verzió)
- Közös értékesítéssel való hivatkozás létrehozása – Salesforce (belső előzetes verzió)
- Partneri központ a Microsoft közös értékesítési hivatkozási frissítései a Salesforce-be (belső előzetes verzió)
- Partneri központ – Salesforce (belső előzetes verzió)
- Salesforce (Insider előzetes verzió)
- Salesforce lehetőség a partneri központhoz (belső előzetes verzió)
- Salesforce Microsoft-megoldások a partner Centerhez (belső előzetes verzió)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>A webhook API-k használata az Erőforrás-változási események regisztrálásához

A partner Center webhook API-k lehetővé teszik az Erőforrás-változási események regisztrálását. Ezeket a változási eseményeket a rendszer HTTP-bejegyzésekként küldi el az URL-címre.

1. Az URL-cím regisztrálásához válassza a **partner Center webhook-regisztráció (belső előzetes verzió)** energiagazdálkodási folyamatát.

2. Vegyen fel kapcsolatokat az (a.) partner Center-felhasználóhoz az Ajánlói rendszergazdai hitelesítő adatokkal (b.) a következő Kiemelt módon:

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Eseményindító":::

3. Ha ezeket a frissítéseket végzi, a következőt fogja látni:

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhookok":::

4. Mentse a módosításokat, és válassza **a bekapcsolás** lehetőséget.

   A következő lépések végrehajtásával engedélyezheti a partneri központ webhookok számára az események változásának figyelését:

5. Válassza ki **a partneri központot a CRM Salesforce (belső előzetes verzió)**.

6. Válassza a **Szerkesztés** ikont, és válassza ki a **http-kérés fogadásakor** lehetőséget.

7. Kattintson a **Másolás** ikonra a megadott http post URL-cím másolásához.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL-cím másolása":::

8. Most válassza ki a "partneri központ webhook-regisztráció (Insider előzetes verzió)" energiaellátás-automatizálási folyamat elemet, és válassza a **Futtatás** lehetőséget.

9. Győződjön meg arról, hogy a jobb oldali ablaktáblán megnyílik a "Futtatás folyamata" ablak, és kattintson a **Folytatás** gombra.

10. Adja meg a következő részleteket:

    1. **Http-trigger végpontja**: a korábbi lépésből másolt URL-cím

    2. **Regisztrálni kívánt események**: "referral-created" és "referral-frissítve"

    3. **Meglévő trigger-végpontok felülírása (ha van**): igen (Ez felülírja a meglévő végpontokat.)

11. Válassza a **Futtatás** lehetőséget, majd kattintson a **Kész gombra.**

A webhook mostantól figyelheti az események létrehozását és frissítését.

## <a name="customize-synchronization-steps"></a>Szinkronizálási lépések testreszabása

Ha a partneri központ és a CRM-rendszer között szinkronizálja a közös értékesítésre való átirányítást, akkor a partner Center-számítógépen szinkronizált mezők itt vannak felsorolva.

A CRM-rendszerek gyakran testre szabottak. Testreszabhatja a Power automatizáló folyamatokat. Kövesse a mező-hozzárendelési útmutatót, és szükség esetén végezze el a megfelelő módosításokat a Power automatizáló folyamatok lépéseiben.  A Microsoft-partneri központok a CRM-alapú hozzárendelésekhez vannak megadva, de a CRM-környezet alapján a mezők további testreszabására is lehetősége van.

Az egyes energiagazdálkodási folyamatok több lépését az igényeinek megfelelően testre szabhatja. A következő példák az elérhető testreszabásokat szemléltetik:

1. A partner központ létrehozási vagy frissítési eseményeihez tartozó mezők testreszabása a CRM-hivatkozó szinkronizálásához:

   1. Válassza ki a partneri központot a CRM Salesforce (belső előzetes verzió).

   2. Válassza a **Szerkesztés** lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.

   3. Válassza **a (hatókör) lehetőséget az érdeklődő vagy a lehetőség szinkronizálásához**.

2. Ha testre szeretné szabni az események létrehozásához tartozó CRM-mezők leképezéseit, válassza ki, hogy **új megosztott lehetőség van-e, majd**. Válassza ki az allépést, **Ha igen** , majd bontsa ki **az új lehetőség létrehozása lehetőséget a CRM-ben**. Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató segítségével módosíthatja.

   1. A frissítési események CRM-mezőkhöz való hozzárendelésének testreszabásához kattintson a "(hatókör) – az érdeklődő vagy a lehetőség szinkronizálása" elemre.

   2. Válassza ki **, hogy a lehetőség frissítése lehetséges-** e. **Ha igen** , akkor válassza ki az allépést, majd bontsa ki **, ha a partner Centerben és a CRM-ben a lehetőség-objektumok között van különbség**  

   3. Jelölje be az **Igen** , majd a **meglévő frissítése lehetőséget** .

3. A CRM és a számítógép közötti átirányítási szinkronizálás mezőinek testreszabása a frissítési eseményekhez:

   1. Válassza a **Szerkesztés**  lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.

   2. Válassza **a (hatókör) lehetőséget a lehetőség szinkronizálásához**.

   3. Ha a CRM-mezők hozzárendeléseit (mező-hozzárendelések útmutatója alapján) testreszabja a frissítési eseményekhez, akkor válassza ki, hogy van-e **különbség a partner Centerben és a CRM-ben lévő érdeklődő objektumok között**.

   4. Válassza ki az allépést, **Ha igen** , majd bontsa ki az **átirányítási lehetőséget a lehetőségre vonatkozó adattal**.

   Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató alapján módosíthatja.

4. A CRM és a számítógép közötti átirányítási szinkronizálás mezőinek testreszabása az események létrehozásához?

   1. Válassza a **Szerkesztés**  lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.

   2. Válassza ki **(hatókör) az átirányítások szinkronizálását.**

   3. Ha testre kívánja szabni a CRM-mezők hozzárendeléseit (a mező-hozzárendelések útmutatója alapján) az események létrehozásához, válassza a **Microsoft ajánló létrehozása** lehetőséget.

Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató alapján módosíthatja.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Végpontok közötti kétirányú, közös értékesítésre hivatkozó átirányítás szinkronizálása

Miután telepítette, konfigurálta és testreszabta az automatizálási megoldást, tesztelheti a Salesforce CRM és a partner Center közötti, közös értékesítéssel való átirányítások szinkronizálását.

### <a name="pre-requisites"></a>Előfeltételek

Ha szinkronizálni szeretné az átirányításokat a partner Center és a Salesforce CRM között, az automatizálási megoldásnak egyértelműen körzet határának kijelölésében kell a Microsoft-specifikus átirányítási mezőket. Ez az azonosítás biztosítja az értékesítő csapatának, hogy eldöntse, hogy mely ajánlásokat szeretné megosztani a Microsofttal a közös értékesítéshez.

Az egyéni mezők készlete a Salesforce CRM-megoldási **lehetőség** entitásának partneri központhoz való átirányítási szinkronizálásának részeként érhető el. Egy CRM-rendszergazda felhasználónak külön CRM-szakaszt kell létrehoznia a **lehetőség** egyéni mezőivel.

A következő egyéni mezők a CRM szakasz részét képezik:

- **Szinkronizálás a partner centerrel**: a lehetőség szinkronizálása a Microsoft partner centerrel

- **Hivatkozási azonosító**: a Microsoft partner Center ajánlójának írásvédett azonosító mezője

- **Referral link**: egy csak olvasható hivatkozás a Microsoft partner Centerben

- A **Microsoft súgója**: Segítség szükséges a Microsofttól az átirányításhoz

- **Termékek**: a lehetőséghez társított termékek listája

- **Naplózás**: írásvédett naplózási nyomvonal a partner Center-hivatkozásokkal való szinkronizáláshoz

### <a name="scenarios"></a>FORGATÓKÖNYVEK

1. Átirányítás szinkronizálása a CRM-ben való létrehozáskor vagy frissítésekor, valamint a partner Centerben szinkronizálva:

   1. Jelentkezzen be a Salesforce CRM-környezetbe olyan felhasználóval, aki rendelkezik a CRM **lehetőség** szakaszában láthatóval.

   2. Győződjön meg arról, hogy a Salesforce CRM-környezet "új lehetőség" létrehozásakor a következő szakasz jelenik meg

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-környezet":::

   3. Ha ezt a lehetőséget a Microsoft partner centerrel szeretné szinkronizálni, ügyeljen arra, hogy a következő mezőket adja meg a kártya nézetben:

       - "Szinkronizálás a partner központtal": igen
       - "Hogyan lehet a Microsoft súgója?": válasszon a következő lehetőségek közül:
       - Termékek: a termék megoldás-azonosítói

   4. Miután beállította a lehetőség  **szinkronizálását a partner Center** lehetőséggel **Igen**, várjon 10 percet, jelentkezzen be a partner Center-fiókjába. Az átirányítási adatokat a Salesforce CRM-szel szinkronizálja a rendszer.

   5. Ha a "szinkronizálás a partner központtal" beállítás értéke "yes", ha frissíti a lehetőséget a Salesforce CRM-ben, a módosítások szinkronizálva lesznek a partner Center-fiókjával.

   6. A partner centerrel sikeresen szinkronizált lehetőségek a Salesforce CRM ✔ ikonjával lesznek azonosítva.

2. Az átirányítás szinkronizálása, ha a Microsoft partner Centerben létrehozták vagy frissítik az átirányítást, és szinkronizálva vannak a Salesforce CRM-környezetben:

    1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/home).

    2. A bal oldali menüben válassza a **hivatkozók** lehetőséget.

    3. Hozzon létre egy új, közös értékesítésre hivatkozó hivatkozást a partner Centerben az "új üzlet" lehetőségre kattintva.

    4. Jelentkezzen be a Salesforce CRM-környezetbe.

    5. Navigáljon a **lehetőségek megnyitásához**. A Microsoft partner Centerben létrehozott hivatkozás mostantól szinkronizálva van a Salesforce CRM-ben.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce lehetőség képernyő":::

    6. Amikor kijelöl egy szinkronizált átirányítást, a rendszer feltölti a kártya nézetének részleteit.

## <a name="next-steps"></a>Következő lépések

- [Érdeklődők kezelése](manage-leads.md)

- [Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)

- [A partneri központ webhookai](/partner-center/develop/partner-center-webhooks)
