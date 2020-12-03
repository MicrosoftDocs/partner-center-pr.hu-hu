---
title: A Dynamics 365 CRM-partneri központ közös értékesítési összekötője
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Szinkronizálja a partner Centerben lévő hivatkozásokat a Dynamics 365 CRM-hez készült közös értékesítési összekötővel. Az értékesítők ezután a Microsofttal közösen értékesíthetők a CRM-rendszereken belül.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 18a54bf777cb987e8f486f85afcf277e04c1055c
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556361"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Közös értékesítésű összekötő a Dynamics 365 CRM-hez – áttekintés

### <a name="appropriate-roles"></a>Megfelelő szerepkörök

- Ajánlói rendszergazda
- Rendszerfelügyeleti webszolgáltatások vagy Rendszertestreszabó a CRM-ben

A partner Center közös értékesítési összekötője lehetővé teszi, hogy az értékesítők a Microsofttal közösen értékesítsenek a CRM-rendszereken belül. Nem kell kiképezniük, hogy a partner centerrel együtt kezeljék a közös értékesítési ajánlatokat. A közös értékesítésű összekötők használatával létrehozhat egy új, közösen értékesíthető hivatkozást a Microsoft-értékesítők bevonásához, a Microsoft-értékesítőtől kapott hivatkozásokat fogad, elfogadhatja/elutasíthatja az átirányítást, módosíthatja az ügyleti értékeket, például az üzlet értékét és a zárási dátumot. Ezeket a közös értékesítési ajánlatokat a Microsoft-értékesítők frissítései is megkapják. Az összes átirányítást megteheti a választott CRM-en belül, nem pedig a partner Centerben. 

A megoldás a Microsoft Power automatizálási megoldásán alapul, és a partner Center API-kat használja.

## <a name="before-you-install---pre-requisites"></a>Az Előfeltételek telepítése előtt

|**Témakörök**   |**Részletek**   |**Hivatkozások**   |
|--------------|--------------------|------|
|Microsoft Partner Network azonosítója |Érvényes MPN-AZONOSÍTÓra van szüksége|Az [MPN](https://partner.microsoft.com/) csatlakoztatása|
|Értékesítésre kész|Az IP-/szolgáltatási megoldásnak közös értékesítéssel kell rendelkeznie.|[Értékesítés a Microsofttal](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnerközpont-fiók|A partner Center-bérlőhöz társított MPN-AZONOSÍTÓnak meg kell egyeznie a közös értékesítési megoldáshoz társított MPN-azonosítóval. Az összekötők üzembe helyezése előtt győződjön meg arról, hogy a partner Center portálon megtekintheti a közös értékesítéssel kapcsolatos hivatkozásokat.|[Saját fiók kezelése](create-user-accounts-and-set-permissions.md)|
|A partner Center felhasználói szerepkörei|Az összekötőket telepítő és használó alkalmazottnak hivatkozói rendszergazdának kell lennie|[Felhasználói szerepkörök és engedélyek hozzárendelése](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|A CRM-felhasználói szerepkör a rendszergazda vagy a rendszertestreszabó|[Szerepkörök társítása a Dynamics 365-ben](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power automatizáló folyamat fiókja|Aktív [Power automatizáló](https://flow.microsoft.com) fiók a CRM rendszer-rendszergazda vagy Rendszertestreszabó számára. A telepítés előtt a felhasználónak legalább egyszer be kell jelentkeznie az [energiagazdálkodásba](https://flow.microsoft.com) .|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>A partneri központ átirányítási szinkronizálásának telepítése a Dynamics 365-hez (Power automatizáló megoldás)

1. Nyissa meg a [Power Automatet](https://flow.microsoft.com) , és válassza a **környezetek** lehetőséget a jobb felső sarokban. Ebben a lépésben az elérhető CRM-példányok jelennek meg.

2. Válassza ki a megfelelő CRM-példányt a jobb felső sarokban lévő legördülő menüből.

3. A bal oldali navigációs sávon válassza a **megoldások** elemet.

4. Kattintson a felső menüben található **AppSource megnyitása** hivatkozásra.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource megnyitása":::

5. Keressen rá a Dynamics365-hez készült **partner Center-összekötők** az előugró képernyőn.  

6. Kattintson a **Letöltés most** gombra, és **folytassa a művelettel**.

7. Ekkor megnyílik a lap, amelyen kiválaszthatja az alkalmazás telepítéséhez szükséges CRM-környezetet (Dynamics 365).  Fogadja el a feltételeket és a kikötéseket.

8. Ezután átirányítja a **megoldások kezelése** lapra.  A lap alján található nyílgombok segítségével navigáljon a "partneri központhoz". A **telepítés ütemezése** a partner Center Referrals megoldás mellett jelenik meg. A telepítés 10-15 percet vesz igénybe. 

9. A telepítés befejezése után váltson vissza a [Power automatizálás](https://flow.microsoft.com) szolgáltatásra, és válassza a bal oldali navigációs terület **megoldásait** . Figyelje meg, hogy a **partneri központ a Dynamics 365-szinkronizálása** elérhető a megoldások listájában.

10. Válassza **a partner Center-átirányítási szinkronizálás a Dynamics 365-hez** lehetőséget. A következő energiagazdálkodási folyamatok és entitások érhetők el:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Rendelkezésre álló CRM":::

## <a name="best-practice-test-before-you-go-live"></a>Ajánlott eljárás: tesztelés az élő indítás előtt

Mielőtt telepítené, konfigurálja és testreszabja az automatizálási megoldást az éles környezetben, mindenképpen tesztelje a megoldást egy átmeneti CRM-példányon.

- Telepítse a Microsoft Power automatizáló megoldást átmeneti környezetben vagy CRM-példányon.
- Készítsen másolatot a megoldásról, és futtassa a konfigurációt és a Power automatizálja a folyamatokat az átmeneti környezetben.
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

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Kapcsolat létrehozása":::

      3. A jobb felső sarokban található keresési sávban keresse meg a **partneri központ hivatkozásait (előzetes verzió)** .

      4. Hozzon létre kapcsolatot a fiókpartner-felhasználó számára az Ajánlói rendszergazda hitelesítő adatokkal kapcsolatos szerepkörével.

      5. Ezután hozzon létre egy partneri központ-esemény kapcsolatot a partner Center-felhasználó számára az Ajánlói rendszergazda hitelesítő adataival.

      6. Hozzon létre egy Common Data Service (aktuális környezet) kapcsolatokat a CRM-rendszergazda felhasználó számára.
       
     
      7. Az összes hozzáadott kapcsolat után a következő kapcsolatokat kell látnia a környezetben:

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Kapcsolatok":::
   
## <a name="edit-the-connections"></a>Kapcsolatok szerkesztése

1. Térjen vissza a **megoldások** lapra, és válassza az **alapértelmezett megoldás** lehetőséget. Válassza a **kapcsolatok referenciája (előzetes verzió)** lehetőséget az **összes** elemre kattintva.

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Kapcsolódás":::

2. Szerkessze az egyes kapcsolatokat egyenként a három pont ikon kiválasztásával. Adja hozzá a megfelelő kapcsolatokat.

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Felsorolt kapcsolatok"::: 

3.  Kapcsolja be a folyamatokat a következő sorozatban:
- A partner Center webhook-regisztrációja (belső előzetes verzió)
- Közös értékesítésre hivatkozó hivatkozás létrehozása – Dynamics 365 – partneri központ (belső előzetes verzió)
- A partner Center Microsoft közös értékesítési hivatkozási frissítései a Dynamics 365-as verzióra (Insider előzetes verzió)
- Partneri központ a Dynamics 365-hoz (belső előzetes verzió)
- Dynamics 365 a partneri központba (belső előzetes verzió)
- Dynamics 365 lehetőség a partneri központhoz (belső előzetes verzió)
- Dynamics 365 Microsoft-megoldások a partner Centerhez (Insider előzetes verzió)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>A webhook API-k használata az Erőforrás-változási események regisztrálásához

A partner Center webhook API-k lehetővé teszik az Erőforrás-változási események regisztrálását. Ezeket a változási eseményeket a rendszer HTTP-bejegyzésekként küldi el az URL-címre.

1. Az URL-cím regisztrálásához válassza a **partner Center webhook-regisztráció (belső előzetes verzió)** energiagazdálkodási folyamatát.

2. Vegyen fel kapcsolatokat az (a.) partner Center-felhasználóhoz az Ajánlói rendszergazdai hitelesítő adatokkal (b.) a következő Kiemelt módon:

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Eseményindító":::

3. Ha ezeket a frissítéseket végzi, a következőt fogja látni:

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhookok":::

4. Mentse a módosításokat, és válassza **a bekapcsolás** lehetőséget.

   A következő lépésekkel engedélyezheti a partneri központ webhookok számára az események változásának figyelését:

5. Válassza **a partner központ lehetőséget a Dynamics 365 (belső előzetes verzió)** elemre.

6. Válassza a **Szerkesztés** ikont, és válassza ki a **http-kérés fogadásakor** lehetőséget.

7. Kattintson a **Másolás** ikonra a megadott http post URL-cím másolásához.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL-cím másolása":::

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

    a. Válassza a partneri központ lehetőséget a Dynamics 365 (belső előzetes verzió) vagy a Salesforce (belső előzetes verzió) elemre.

    b. Válassza a **Szerkesztés** lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.

    c. Válassza **a (hatókör) lehetőséget az érdeklődő vagy a lehetőség szinkronizálásához**.

2. Ha testre szeretné szabni a CRM-mezők hozzárendeléseit (a mező-hozzárendelések útmutatója alapján) az események létrehozásához, válassza ki, hogy **új megosztott lehetőség van-e, majd**. Válassza ki az allépést, **Ha igen** , majd bontsa ki az **új lehetőség létrehozása lehetőséget a CRM-ben**. Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató segítségével módosíthatja.

    d. Ha testre szeretné szabni a CRM-mezők hozzárendeléseit (a mező-hozzárendelések útmutatója alapján) a frissítési események esetében, kattintson a "(hatókör)" lehetőségre az érdeklődő vagy a lehetőség szinkronizálásához.

    e. Válassza ki **, hogy a lehetőség frissítése lehetséges-** e. **Ha igen** , akkor válassza ki az allépést, majd bontsa ki **, ha a partner Centerben és a CRM-ben a lehetőség-objektumok között van különbség**  

    f. Jelölje be az **Igen** , majd a **meglévő frissítése lehetőséget** .

3. A CRM és a számítógép közötti átirányítási szinkronizálás mezőinek testreszabása a frissítési eseményekhez:

    a. Válassza a **Szerkesztés**  lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.

    b. Válassza **a (hatókör) lehetőséget a lehetőség szinkronizálásához**.

    c. A frissítési események CRM-mezőkhöz való hozzárendelésének testreszabásához válassza ki, hogy van-e **különbség a partner Centerben és a CRM-ben lévő érdeklődő objektumok között**. 

    d. Válassza ki az allépést, **Ha igen** , majd bontsa ki az **átirányítási lehetőséget a lehetőségre vonatkozó adattal**.

   Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató alapján módosíthatja.

4. A CRM és a számítógép közötti átirányítási szinkronizálás mezőinek testreszabása az események létrehozásához?

   a. Válassza a **Szerkesztés**  lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.

   b. Válassza ki **(hatókör) az átirányítások szinkronizálását.**

   c. Ha testre kívánja szabni a CRM-mezők hozzárendeléseit (a mező-hozzárendelések útmutatója alapján) az események létrehozásához, válassza a **Microsoft ajánló létrehozása** lehetőséget.

   Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató alapján módosíthatja.

Két környezeti változó lett létrehozva:

- Pipa: azt jelzi, hogy a partner központ és a Dynamics 365 CRM között kétirányú szinkronizálású lehetőségek mellett van-e pipa ikon.

- Csak közös értékesítési lehetőségek szinkronizálása: azt jelenti, hogy csak a közös értékesítési lehetőségeket kívánja szinkronizálni.

A környezeti változók alapértelmezett értékének szerkesztését is választhatja.

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Alapértelmezett értékekhez tartozó mező szerkesztése":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Végpontok közötti kétirányú, közös értékesítésre hivatkozó átirányítás szinkronizálása

Miután telepítette, konfigurálta és testreszabta az automatizálási megoldást, tesztelheti a Dynamics 365 és a partner Center közötti összekapcsolási átirányítások szinkronizálását.

### <a name="pre-requisites"></a>Előfeltételek

Ha szinkronizálni szeretné a partner központ és a Dynamics 365 CRM közötti átirányításokat, az automatizálási megoldás egyértelműen kijelölte a Microsoft-specifikus átirányítási mezőket. Ez az azonosítás lehetővé teszi az értékesítő csapatának, hogy eldöntse, hogy mely ajánlásokat szeretné megosztani a Microsofttal a közös értékesítéshez.

Az egyéni mezők készlete a **lehetőség** entitás részeként érhető el. Egy CRM-rendszergazda felhasználónak külön CRM-szakaszt kell létrehoznia a **lehetőség** egyéni mezőivel.

A következő egyéni mezők a CRM szakasz részét képezik:

- **Szinkronizálás a partner centerrel**: a lehetőség szinkronizálása a Microsoft partner centerrel

- **Hivatkozási azonosító**: a Microsoft partner Center ajánlójának írásvédett azonosító mezője

- **Referral link**: egy csak olvasható hivatkozás a Microsoft partner Centerben

- **Hogyan segíthet a Microsoft súgója?**: Segítség szükséges a Microsoftnak az átirányításhoz

- **Termékek**: a lehetőséghez társított termékek listája

- **Naplózás**: írásvédett naplózási nyomvonal a partner Center-hivatkozásokkal való szinkronizáláshoz

Frissítse a lehetőség űrlapját a Dynamics 365 CRM-ben a termékek mezőhöz tartozó megoldások befoglalásához.

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Lehetőség űrlapja":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a>FORGATÓKÖNYVEK

1. Átirányítás szinkronizálása a CRM-ben való létrehozáskor vagy frissítésekor, valamint a partner Centerben szinkronizálva:

   1. Jelentkezzen be a Dynamics 365 CRM-környezetbe azokkal a felhasználókkal, akik a CRM **lehetőség** szakaszában láthatók.

   2. Győződjön meg arról, hogy a Dynamics 365 környezetben a következő szakasz jelenik meg, amikor létrehoz egy új lehetőséget.

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="A Microsoft partner Center információinak a Dynamics 365-ben való megjelenítését bemutató példa lehetőség szakasza.":::

   3. Ha ezt a lehetőséget a Microsoft partner centerrel szeretné szinkronizálni, ügyeljen arra, hogy a következő mezőket adja meg a kártya nézetben:

      - **Szinkronizálás a partner centerrel**: igen

      - **Hogyan segíthet a Microsoft súgója?**: válasszon a következők közül:

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="A Dynamics 365-es minta lehetőség szakasza, amely a Microsoft-partneri központ súgóját mutatja be a hogyan tud a Microsoft Help? nevű mező mellett.":::

      - **Termékek**: a termék megoldás-azonosítói

   4. Miután létrejött a lehetőség a Dynamics 365-ben a **partner centerrel való szinkronizálással** beállítás **Igen** értékre van állítva, várjon 10 percet, majd jelentkezzen be a partner Center-fiókjába. Az átirányítási adatokat a Dynamics 365-mel szinkronizálja a rendszer.

   5. Hasonlóképpen, ha a Dynamics 365 CRM-ben a lehetőség frissítésével "igen" értékre állította a "szinkronizálás a partneri központtal" beállítást, a rendszer szinkronizálja a módosításokat a partner Center-fiókban.

   6. A partner centerrel sikeresen szinkronizált lehetőségek a Dynamics 365-as ✔ ikonnal lesznek azonosítva.

2. Az átirányítás szinkronizálása a Microsoft partner Centerben, a Dynamics 365 környezetben szinkronizálva:

   1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/home).

   2. A bal oldali menüben válassza a **hivatkozók** lehetőséget.

   3. Hozzon létre egy új, közös értékesítésre hivatkozó hivatkozást a partner Centerben az "új üzlet" lehetőségre kattintva.

   4. Jelentkezzen be a Dynamics 365 CRM-környezetbe.

   5. Navigáljon a **lehetőségek megnyitásához**. A Microsoft partner Centerben létrehozott hivatkozás mostantól szinkronizálva van a Dynamics 365 CRM-ben.

   6. Amikor kijelöl egy szinkronizált átirányítást, a rendszer feltölti a kártya nézetének részleteit.

## <a name="next-steps"></a>Következő lépések

- [Érdeklődők kezelése](manage-leads.md)

- [Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)

- [További információ a Microsoft Power automatizáló platformról?](/power-automate/)

- [A partneri központ webhookai](/partner-center/develop/partner-center-webhooks)