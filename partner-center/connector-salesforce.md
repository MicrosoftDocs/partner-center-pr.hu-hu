---
title: A Salesforce CRM-összekötő Partnerközpont
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Szinkronizálja a Partnerközpont a Salesforce CRM-mel. Az értékesítők ezután együtt értékesíthet a Microsofttal az Ön CRM-rendszereiből.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276977"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM-hez készült közös értékesítési összekötő – áttekintés

**Megfelelő szerepkörök:** Ajánlói rendszergazdai | Rendszergazda vagy rendszer testreszabó a CRM-ben

Partnerközpont összekötő lehetővé teszi az értékesítők számára, hogy az Ön CRM-rendszereiből együtt értékesítsen a Microsofttal. Nem kell betanítanunk őket ahhoz, hogy a Partnerközpont az értékesítések kezeléséhez. Az értékesítésre vonatkozó összekötők használatával létrehozhat egy új közös értékesítésre vonatkozó ajánlást egy Microsoft-értékesítő bevonásához, a Microsoft értékesítőjéhez való terjesztés fogadásához, az elfogadási/elutasítási hivatkozásokhoz, az üzletadatok módosításához, például az üzlet értékéhez és a záró dátumhoz.  Emellett a Microsoft értékesítőitől is kaphat frissítéseket ezekről az együttműködési ügyletekről. Az összes ajánlása a választott CRM-ben működik, és nem a Partnerközpont. 

A megoldás a Microsoft Power Automate Solution-alapú, és Partnerközpont API-kat használ.

## <a name="before-you-install---pre-requisites"></a>Telepítés előtt – előfeltételek

|**Témakörök**   |**Részletek**   |**Hivatkozások**   |
|--------------|--------------------|------|
|Microsoft Partner Network azonosítója |Szüksége van egy érvényes MPN-azonosítóra|Csatlakozás az [MPN-hez](https://partner.microsoft.com/)|
|Az együtt értékesítésre kész|Az IP-/szolgáltatási megoldásnak készen kell állnia az együtt értékesítésre.|[Értékesítés a Microsofttal](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnerközpont-fiók|A bérlőhöz társított MPN-Partnerközpont meg kell egynie az együttműködési megoldáshoz társított MPN-azonosítóval. Az összekötők üzembe helyezése előtt ellenőrizze, hogy látja-e az Partnerközpont-hez kapcsolódó hivatkozásokat.|[Saját fiók kezelése](create-user-accounts-and-set-permissions.md)|
|Partnerközpont felhasználói szerepkörök|Az összekötőket telepítő és azt felhasználó alkalmazottnak ajánlói rendszergazdának kell lennie|[Felhasználói szerepkörök és engedélyek hozzárendelése](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|A CRM felhasználói szerepkör a rendszergazda vagy a rendszer testre szabója|[Szerepkörök hozzárendelése a Salesforce CRM-ben](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow-fiók|Aktív fiók [Power Automate](https://flow.microsoft.com) CRM-rendszerrendszergazdának vagy rendszer-testreszabónak. A felhasználónak legalább [Power Automate](https://flow.microsoft.com) be kell jelentkeznie az alkalmazásba.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>A Salesforce-csomag telepítése a Microsoft Custom Fieldshez 

A Partnerközpont és a Salesforce CRM Power Automate megoldásnak egyértelműen azonosítania kell a Microsoft-specifikus javaslatmezőket. Ez a demarkáció lehetővé teszi a partner értékesítői csapatok számára, hogy eldöntsék, mely terjesztéseket szeretnék megosztani a Microsofttal az közös értékesítéshez.

1. A Salesforce-ban aktiválja a **Jegyzeteket,** és adja hozzá a lehetőségekhez kapcsolódó listához. 
[Referencia](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. A **lehetőségcsapatok aktiválásához** kövesse az alábbi lépéseket: 
    - A Telepítőben a **Gyors keresés mezőben** keresse meg a Lehetőségcsoport beállításait.
    - Szükség szerint adja meg a beállításokat.
[Referencia](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. A Salesforce-ban telepítsen egyéni mezőket és objektumokat a [csomagtelepítővel.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) Ezzel bármely vállalatnál telepítheti a csomagot.

>[!NOTE]
>Ha a telepítést egy védőfalba telepíti, az URL-cím kezdeti részét a következőre kell cserélnie: http://test.salesforce.com

4. A Salesforce-ban adja hozzá a Microsoft-megoldásokat a **Lehetőséggel** kapcsolatos listához. A hozzáadás után válassza a **csavarkulcs ikont,** és frissítse a tulajdonságokat

## <a name="best-practice-test-before-you-go-live"></a>Ajánlott eljárás: Tesztelés az élő adás előtt

Mielőtt telepíti, konfigurálja és testreszabja a Power Automate megoldást az éles környezetben, mindenképpen tesztelje a megoldást egy átmeneti CRM-példányon.

- Telepítse a Microsoft Power Automate megoldást egy átmeneti környezetbe/CRM-példányba.

- Másolja le a megoldást, futtassa a konfigurációt, Power Automate folyamat testreszabását az átmeneti környezetben.

- Tesztelje a megoldást egy átmeneti/CRM-példányon.

- Sikeresség után importálja felügyelt megoldásként az éles példányba.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>A Partnerközpont szinkronizálásának telepítése a Salesforce CRM-hez

1. A jobb [felső Power Automate](https://flow.microsoft.com) válassza a **Környezetek** lehetőséget. Itt érhetők el az elérhető CRM-példányok.

2. Válassza ki a megfelelő CRM-példányt a jobb felső sarokban található legördülő menüből.

3. A **bal oldali navigációs** sávon válassza a Megoldások lehetőséget.

4. Válassza a **felső menü Open AppSource (AppSource** megnyitása) hivatkozását.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Nyissa meg az AppSource-t.":::

5. Az **előugró Partnerközpont keresse meg** a Salesforce-hez használható ajánlói összekötőket.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce.":::

6. Kattintson a **Get it now (Lekért most) gombra,** majd a **Continue (Folytatás) gombra.**

7. Ez megnyitja az oldalt, ahol kiválaszthatja a Salesforce CRM-környezetet az alkalmazás telepítéséhez.  Elfogadja a használati feltételeket.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Elérhető CRM-ek.":::

8. Ezután a Megoldások kezelése **lapra lesz irányítva.**  Lépjen a "Partnerközpont" lapra az oldal alján található nyílgombokkal. **Az ütemezett telepítésnek** a javaslati megoldás Partnerközpont kell megjelennie. A telepítés 10–15 percet fog igénybe venni.

9. A telepítés befejezése után lépjen vissza az Power Automate, [és](https://flow.microsoft.com) válassza a **Megoldások** lehetőséget a bal oldali navigációs területen. Figyelje **Partnerközpont, hogy a Salesforce-hez való** hivatkozásszinkronizálás elérhető a Megoldások listában.

10. Válassza **Partnerközpont a Salesforce-hez való hivatkozásszinkronizálás lehetőséget.** A következő Power Automate folyamatok és entitások érhetők el:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce-folyamatok.":::



## <a name="configure-the-solution"></a>A megoldás konfigurálása

1. Miután telepítette a megoldást a CRM-példányban, lépjen vissza a [Power Automate.](https://flow.microsoft.com/)

2. A jobb **felső** sarokban található Környezetek legördülő menüből válassza ki azt a CRM-példányt, ahová a Power Automate telepítette.
3. A három felhasználói fiókot társító kapcsolatokat kell létrehoznia:
    - Partnerközpont rendszergazdai hitelesítő adatok megadása a felhasználónak
    - Partnerközpont – események
    - CRM-rendszergazda a Power Automate folyamatokkal a megoldásban.
4. A **bal oldali** navigációs sávon válassza a Kapcsolatok lehetőséget, majd válassza a "Partnerközpont" megoldást a listából.

5. A Kapcsolat létrehozása gombra **kattintva hozzon létre egy kapcsolatot.**

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Kapcsolat létrehozása.":::

- Keressen a Partnerközpont (előzetes verzió) kifejezésre a jobb felső sarokban található keresősávban.

- Hozzon létre egy kapcsolatot a Partnerközpont a ajánlói rendszergazda hitelesítőadat-szerepkörében.

-  Ezután hozzon létre egy Partnerközpont Események kapcsolatot a Partnerközpont a ajánlói rendszergazda hitelesítő adataival.

- Hozzon létre egy kapcsolatot a Salesforce számára a CRM-rendszergazdai felhasználó számára.

-  Miután hozzáadta az összes kapcsolatot, a következő kapcsolatoknak kell látszani a környezetében:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Kapcsolatok megfigyelése.":::

### <a name="edit-the-connections"></a>A kapcsolatok szerkesztése

1. Térjen vissza a Megoldások lapra, és válassza az **Alapértelmezett megoldás lehetőséget.**  A Minden elemre kattintva válassza a Kapcsolati **referencia (előzetes verzió)** **lehetőséget.**
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Kezdje meg az összekötő szerkesztését.":::

2. Szerkessze egyenként a kapcsolatokat a három pont ikon kiválasztásával. Adja hozzá a megfelelő kapcsolatokat.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Összekötők szerkesztése.":::

3. Kapcsolja be a folyamatokat a következő sorrendben:

- Partnerközpont regisztrációja (Insider Preview)
- Közös értékesítési ajánlás létrehozása – Salesforce Partnerközpont (Insider Preview)
- Partnerközpont Microsoft Co-sell Referral Updates to Salesforce (Insider Preview) (Microsoft Co-sell referral Updates to Salesforce (Insider Preview) (A Salesforce (Belső előzetes verzió) frissítései)
- Partnerközpont Salesforce (Insider Preview)
- A Salesforce Partnerközpont (Insider Preview)
- Salesforce Opportunity to Partnerközpont (Insider Preview)
- A Salesforce Microsoft Solutions Partnerközpont (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook API-k használata erőforrás-módosítási eseményekre való regisztrációhoz

A Partnerközpont Webhook API-k lehetővé teszik, hogy regisztráljon az erőforrás-módosítási eseményekre. Ezeket a módosítási eseményeket a rendszer HTTP-bejegyzésekként küldi el az URL-címére.

1. Az URL-cím regisztráláshoz válassza Partnerközpont **webhookregisztráció (Insider Preview)** lehetőséget a Power Automate folyamathoz.

2. Adjon hozzá kapcsolatokat (a.) Partnerközpont felhasználóhoz a hivatkozások rendszergazdai hitelesítő adataival (b.) Partnerközpont eseményekhez az alább kiemelt módon

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Ravaszt.":::

3. A frissítések során a következőt fogja látni:

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhookok.":::

4. Mentse a módosításokat, és válassza **a Bekapcsolás lehetőséget.**

   Ha engedélyezni Partnerközpont, hogy a webhookok figyeljék az események változásait, hajtsa végre a következő lépéseket:

5. Válassza **Partnerközpont Salesforce CRM (Insider Preview)** lehetőséget.

6. Válassza a **Szerkesztés ikont,** majd **a HTTP-kérések esetén lehetőséget.**

7. Kattintson a **Másolás ikonra** a megadott HTTP POST URL-cím másoláshoz.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Url-cím másolása.":::

8. Válassza ki a "Partnerközpont Regisztráció (Insider Preview)" folyamatot, Power Automate futtatás **lehetőséget.**

9. Győződjön meg arról, hogy a jobb oldali panelen megnyílik a "Folyamat futtatása" ablak, és válassza a **Folytatás lehetőséget.**

10. Adja meg a következő részleteket:

    1. **HTTP-eseményindító végpontja:** Az URL-cím kimásolható a korábbi lépésből

    2. **Regisztrálni szükséges események:**"referral-created" és "referral-updated"

    3. **Meglévő triggervégpont felülírása, ha van:** Igen (Ez felülírja a meglévő végpontokat.)

11. Válassza a **Futtatás,** majd a Kész **lehetőséget.**

A webhook most már képes figyelni az események létrehozására és frissítésére.

## <a name="customize-synchronization-steps"></a>Szinkronizálási lépések testreszabása

Ha az értékesítésre vonatkozó hivatkozásokat a Partnerközpont és a CRM-rendszer szinkronizálja, itt megjelenik az Partnerközpont számítógépen szinkronizált mezők listája.

A CRM-rendszerek gyakran nagymértékben testre vannak szabva. A folyamatokat testre Power Automate testreszabhatja. Kövesse a mezőleképezési útmutatót, és szükség esetén hajtsa végre a megfelelő módosításokat a Power Automate lépésekben.  A Microsoft Partnerközpontok és CRM-leképezések is rendelkezésre állnak, de az Ön CRM-környezete alapján további testreszabási beállításokat is választhat a mezőkhöz.

Az egyes folyamatfolyamatok Power Automate az igényeinek megfelelően testre szabhatók. Az alábbiakban példákat talál az elérhető testreszabási lehetőségekre:

1. A CRM-hivatkozásszinkronizálásra vonatkozó beállításokban található létrehozási vagy frissítési események Partnerközpont testre szabhatja:

   1. Válassza Partnerközpont a Salesforce CRM (Insider Preview) lehetőséget.

   2. Válassza **a Szerkesztés** lehetőséget a folyamat szerkesztéséhez Power Automate testreszabásához.

   3. Válassza **a (Hatókör) Az érdeklődő vagy lehetőség szinkronizálása lehetőséget.**

2. A CRM-mezőleképezések eseményekhez való testreszabásához válassza az Új Megosztott lehetőség lehetőséget, majd **a lehetőséget.** Ha igen,  válassza az allépést, majd bontsa ki **az Új lehetőség létrehozása a CRM-ben lehetőséget.** Az ebben a szakaszban található leképezéseket a Mezőleképezés útmutatója segítségével szerkesztheti.

   1. A CRM-mezőleképezések frissítési eseményekhez való testreszabásához válassza az "(Hatókör) Az érdeklődő vagy lehetőség szinkronizálása" lépést.

   2. Válassza **az If it's update to an opportunity (Lehetőség frissítése esetén) lehetőséget, majd a lehetőséget.** Ha igen,  jelölje ki az allépést, majd bontsa ki a Lehetőségobjektumok közötti különbség a Partnerközpont **CRM-ben, majd a et.**  

   3. Válassza a **Ha igen,** majd a **Meglévő lehetőség frissítése lehetőséget**

3. A CRM–PC hivatkozásszinkronizálás mezőinek testreszabása a frissítési eseményekhez:

   1. Válassza **a Szerkesztés**  lehetőséget a folyamat szerkesztéséhez Power Automate testreszabásához.

   2. Válassza **a (Hatókör) Lehetőség szinkronizálása lehetőséget.**

   3. A frissítési események CRM-mezőleképezésének testreszabásához (a mezőleképezési útmutató alapján) jelölje be a Ha van különbség a crm és a Partnerközpont érdeklődőobjektumai között, akkor **lehetőséget.**

   4. Ha igen,  válassza az allépést, majd bontsa ki a Hivatkozás frissítése **lehetőségadatokkal lépést.**

   Az ebben a szakaszban található leképezéseket a Mezőleképezés útmutatója alapján szerkesztheti.

4. A CRM-számítógépekre történő hivatkozásszinkronizálás mezőinek testreszabása események létrehozásához?

   1. Válassza **a Szerkesztés**  lehetőséget a folyamat szerkesztéséhez Power Automate testreszabásához.

   2. Válassza **a (Hatókör) Javaslatszinkronizálás lehetőséget.**

   3. A CRM-mezőleképezések (mezőleképezési útmutató alapján) események létrehozásához való testreszabásához válassza a **Microsoft-ajánlás létrehozása lehetőséget.**

Az ebben a szakaszban található leképezéseket a Mezőleképezés útmutatója alapján szerkesztheti.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Végpontok között kétirányú kétirányú társ-értékesítés – hivatkozásszinkronizálás

Miután telepítette, konfigurálta és testre szabta a Power Automate megoldást, tesztelheti a Salesforce CRM és a Partnerközpont.

### <a name="pre-requisites"></a>Előfeltételek

A Partnerközpont és a Salesforce CRM közötti szinkronizáláshoz a Power Automate megoldásnak egyértelműen el kell különítenünk a Microsoft-specifikus javaslatmezőket. Ez az azonosítás lehetővé teszi az értékesítő csapatok számára, hogy eldöntsék, mely terjesztéseket szeretnék megosztani a Microsofttal az értékesítéshez.

Egyéni mezők egy készlete érhető el a Partnerközpont a Salesforce CRM megoldáshoz Lehetőség **entitás** részeként. A CRM-rendszergazdáknak külön CRM-szakaszt kell létrehozniuk a **Lehetőség egyéni mezőkkel.**

Az alábbi egyéni mezőknek a CRM szakasz részeinek kell lennie:

- **Szinkronizálás Partnerközpont:** A lehetőség szinkronizálása a Microsoft Partnerközpont

- **Hivatkozásazonosító:** Egy csak olvasható azonosító mező a Microsoft Partnerközpont számára

- **Hivatkozás hivatkozása:** A Microsoft Partnerközpont

- **Hogyan segíthet a Microsoft:** Segítségre van szükség a Microsofttól a hivatkozáshoz?

- **Termékek:** A lehetőséghez társított termékek listája

- **Naplózás:** Csak olvasható auditálási napló a Partnerközpont való szinkronizáláshoz

### <a name="scenarios"></a>Forgatókönyvek:

1. Hivatkozásszinkronizálás a CRM-ben történő hivatkozás létrehozásakor vagy frissítésekor és a következő Partnerközpont:

   1. Jelentkezzen be a Salesforce CRM-környezetbe egy olyan felhasználóval, aki látható a CRM **Lehetőség** szakaszában.

   2. Ellenőrizze, hogy a következő szakasz jelen van-e az "Új lehetőség" Salesforce CRM-környezetben való létrehozásakor

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-környezet.":::

   3. Ha szinkronizálni szeretné ezt a lehetőséget a Microsoft Partnerközpont, állítsa be a következő mezőket a kártyanézetben:

       - "Szinkronizálás a Partnerközpont": Igen
       - "Hogyan segíthet a Microsoft?": Válasszon az alábbi lehetőségek közül:
       - Termékek: A termék megoldás-számai

   4. Miután beállította a Szinkronizálás a következővel  **lehetőséget Partnerközpont** **igen,** várjon 10 percet, jelentkezzen be a Partnerközpont fiókjába. A rendszer szinkronizálja a hivatkozásokat a Salesforce CRM-mel.

   5. Ha a "Szinkronizálás Partnerközpont" beállítás "Igen" van beállítva, akkor ha frissíti a lehetőséget a Salesforce CRM-ben, a módosítások szinkronizálva lesznek az Partnerközpont fiókkal.

   6. A Salesforce CRM-ben a Partnerközpont sikeresen szinkronizált lehetőségeket a ✔ azonosítja.

2. Hivatkozásszinkronizálás a Microsoft-ügyfélben létrehozott vagy frissített hivatkozások Partnerközpont Salesforce CRM-környezetben való szinkronizálása esetén:

    1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard/home)

    2. A **bal oldali menüben** válassza a Hivatkozások lehetőséget.

    3. Hozzon létre egy új közös értékesítésre vonatkozó ajánlást a Partnerközpont "Új üzlet" lehetőségre kattintva.

    4. Jelentkezzen be a Salesforce CRM-környezetbe.

    5. Lépjen a **Megnyitási lehetőségek lapra.** A Microsoft Partnerközpont létrehozott hivatkozás most már szinkronizálva van a Salesforce CRM-ben.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="A Salesforce lehetőség képernyője.":::

    6. Szinkronizált hivatkozás kiválasztásakor a kártyanézet részletei ki lesznek töltve.

## <a name="next-steps"></a>Következő lépések

- [Érdeklődők kezelése](manage-leads.md)

- [Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)

- [Partnerközpont – webhookok](/partner-center/develop/partner-center-webhooks)
