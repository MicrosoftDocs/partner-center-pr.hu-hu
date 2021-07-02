---
title: A Salesforce CRM-összekötő Partnerközpont
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Szinkronizálja a hivatkozásokat Partnerközpont Salesforce CRM-mel. Az értékesítők ezután együtt értékesíthet a Microsofttal az Ön CRM-rendszereiből.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 726e9071347e1590885b4bf82676f7767311f945
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173685"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM-hez készült közös értékesítési összekötő – áttekintés

**Megfelelő szerepkörök:** Ajánlói rendszergazdai | Rendszergazda vagy rendszer-testreszabó a CRM-ben

Partnerközpont összekötő lehetővé teszi az értékesítők számára, hogy az Ön CRM-rendszereiből együtt értékesítsen a Microsofttal. Nem kell betanítanunk őket ahhoz, hogy az Partnerközpont az értékesítések kezeléséhez. Az együttműködési összekötők használatával létrehozhat egy új közös értékesítésre vonatkozó ajánlást egy Microsoft-értékesítő bevonásához, a Microsoft-értékesítőtől kapott hivatkozások fogadásához, az elfogadási/elutasítási hivatkozásokhoz, az üzletadatok módosításához, például az üzlet értékéhez és a záró dátumhoz.  Emellett a Microsoft értékesítőitől is kaphat frissítéseket ezekkel az együttműködési ügyletekkel kapcsolatosakról. Az összes ajánlását a választott CRM-ben, és nem a saját Partnerközpont.

A megoldás a Microsoft Power Automate Solution-alapú, és Partnerközpont API-kat használ.

## <a name="before-you-install---pre-requisites"></a>Telepítés előtt – előfeltételek

|**Témakörök**|**Részletek**|**Hivatkozások**|
|--------------|--------------------|------|
|Microsoft Partner Network azonosítója |Érvényes MPN-azonosítóra van szüksége|Csatlakozás az [MPN-hez](https://partner.microsoft.com/)|
|Készen áll az értékesítésre|Az IP-/szolgáltatási megoldásnak készen kell állnia az értékesítésre.|[Értékesítés a Microsofttal](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Partnerközpont-fiók|A Partnerközpont bérlőhöz társított MPN-azonosítónak meg kell egynie az együttműködési megoldáshoz társított MPN-azonosítóval. Az összekötők üzembe helyezése előtt ellenőrizze, hogy látja-e az Partnerközpont-hez kapcsolódó hivatkozásokat.|[Saját fiók kezelése](create-user-accounts-and-set-permissions.md)|
|Partnerközpont szerepkörök|Az összekötőket telepítő és azt felhasználó alkalmazottnak ajánlói rendszergazdának kell lennie|[Felhasználói szerepkörök és engedélyek hozzárendelése](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|A CRM felhasználói szerepkör rendszergazdai vagy rendszer-testreszabó szerepkör|[Szerepkörök hozzárendelése a Salesforce CRM-ben](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow fiók|Hozzon létre egy új éles környezetet egy adatbázissal teszteléshez, előkészítéshez és éles környezethez. Ha van egy meglévő éles környezete egy adatbázissal, az újra felhasználható. Az összekötő-megoldást telepítő felhasználónak licenccel és Power Automate kell lennie ehhez a környezethez. Ha a telepítés meghiúsul, figyelheti a folyamat előrehaladását, [és Power Automate](https://flow.microsoft.com/) információkat kaphat. A **Megoldások alatt válassza az Előzmények** megtekintése **lehetőséget.**|[Környezet létrehozása vagy kezelése](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Salesforce-csomag telepítése Microsoft Custom Fieldshez

A hivatkozások szinkronizálásához a Partnerközpont És a Salesforce CRM Power Automate megoldásnak egyértelműen azonosítania kell a Microsoft-specifikus javaslati mezőket. Ez a demarkálás lehetővé teszi a partner értékesítői csapatok számára, hogy eldöntsék, mely terjesztéseket szeretnék megosztani a Microsofttal az közös értékesítéshez.

1. A Salesforce-ban aktiválja a **Jegyzeteket,** és adja hozzá a lehetőségekhez kapcsolódó listához. [Referencia](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. A **lehetőségcsapatok aktiválásához** kövesse az alábbi lépéseket:
    - A Telepítőben a **Gyors keresés mezőben** keresse meg a Lehetőségcsoport Gépház.
    - Szükség szerint adja meg a beállításokat. [Referencia](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. Telepítsen egyéni mezőket és objektumokat a Salesforce-ban a [csomagtelepítővel.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) Ezzel a telepítővel bármely vállalatnál telepítheti a csomagot.

    >[!NOTE]
    >Ha a telepítést egy védőfalba telepíti, az URL-cím kezdeti részét a következőre kell cserélnie: `http://test.salesforce.com` .

1. A Salesforce-ban adja hozzá a Microsoft-megoldásokat a **Lehetőséggel** kapcsolatos listához. A hozzáadás után válassza a **csavarkulcs ikont,** és frissítse a tulajdonságokat

## <a name="best-practice-test-before-you-go-live"></a>Ajánlott eljárás: Tesztelés az élő adás előtt

Mielőtt telepíti, konfigurálja és testreszabja a Power Automate megoldást az éles környezetben, mindenképpen tesztelje a megoldást egy átmeneti CRM-példányon.

- Telepítse a Microsoft Power Automate megoldást egy átmeneti környezetbe/CRM-példányba.

- Másolatot készítsen a megoldásról, futtassa a konfigurációt, Power Automate folyamat testreszabását az átmeneti környezetben.

- Tesztelje a megoldást egy átmeneti/CRM-példányon.

- Sikeresség után importálja felügyelt megoldásként az éles példányba.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>A Partnerközpont szinkronizálásának telepítése a Salesforce CRM-hez

1. A jobb [felső Power Automate](https://flow.microsoft.com) válassza a **Környezetek** lehetőséget. Itt érhetők el az elérhető CRM-példányok.

1. Válassza ki a megfelelő CRM-példányt a jobb felső sarokban található legördülő listából.

1. A **bal oldali** navigációs sávon válassza a Megoldások lehetőséget.

1. Válassza a **felső menü Open AppSource (AppSource** megnyitása) hivatkozását.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Nyissa meg az AppSource-t.":::

1. Az **előugró Partnerközpont keresse meg a Salesforce-hez** használható ajánlói összekötőket.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="A Get It Now képernyőképe.":::

1. Kattintson a **Get it now (Lekért most)** gombra, majd válassza a Continue (Folytatás) **lehetőséget.**

1. A következő oldalon válassza ki a Salesforce CRM-környezetet az alkalmazás telepítéséhez. Elfogadja a használati feltételeket.

1. Ezután a Megoldás kezelése **lapra lesz irányítva.**  Navigáljon a "Partnerközpont" elemhez az oldal alján található nyílgombokkal. **Az ütemezett telepítésnek** a javaslati megoldás Partnerközpont kell megjelennie. A telepítés 10–15 percet is igénybe fog venni.

1. A telepítés befejezése után lépjen vissza az [Power Automate,](https://flow.microsoft.com) és válassza a **Megoldások** lehetőséget a bal oldali navigációs területen. Figyelje **meg Partnerközpont hogy a Salesforce-hez használható hivatkozásszinkronizálás** már elérhető a Megoldások listában.

1. Válassza **Partnerközpont Hivatkozásszinkronizálás a Salesforce-ban lehetőséget.** A következő Power Automate folyamatok és entitások érhetők el:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Salesforce-folyamatok.":::

## <a name="configure-the-solution"></a>A megoldás konfigurálása

1. Miután telepítette a megoldást a CRM-példányban, lépjen vissza a [Power Automate.](https://flow.microsoft.com/)

1. A **jobb felső** sarokban található Környezetek legördülő menüben válassza ki azt a CRM-példányt, ahová a Power Automate telepítette.

1. A három felhasználói fiókot társító kapcsolatokat kell létrehoznia:

   - Partnerközpont rendszergazdai hitelesítő adatokkal
   - Partnerközpont – események
   - CRM-rendszergazda a Power Automate folyamatokkal a megoldásban

   1. A **bal oldali** navigációs sávon válassza a Kapcsolatok lehetőséget, majd Partnerközpont **a** listából a Hivatkozási megoldás listában.

   1. Hozzon létre egy kapcsolatot a **Kapcsolat létrehozása lehetőség kiválasztásával.**

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="A Kapcsolat létrehozása képernyőképe.":::

   1. Keressen a **Partnerközpont (előzetes verzió)** kifejezésre a jobb felső sarokban található keresősávban.

   1. Hozzon létre egy kapcsolatot a Partnerközpont ajánlói rendszergazdai hitelesítőadat-szerepkörben.

   1. Ezután hozzon létre egy Partnerközpont Események kapcsolatot a Partnerközpont a ajánlói rendszergazda hitelesítő adataival.

   1. Hozzon létre egy kapcsolatot a Salesforce számára a CRM-rendszergazdai felhasználó számára.
  
   1. Hozzon létre egy kapcsolatot a Microsoft Dataverse számára a CRM-rendszergazdai felhasználó számára.

   1. Az összes kapcsolat hozzáadása után a következő kapcsolatoknak kell látszani a környezetben:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="A kapcsolatok megfigyelését bemutató képernyőkép.":::

### <a name="edit-the-connections"></a>A kapcsolatok szerkesztése

1. Térjen vissza a **Megoldások lapra,** és válassza az **Alapértelmezett megoldás lehetőséget.** Válassza **a Kapcsolati referencia (előzetes verzió) lehetőséget** az All **(Összes) gombra kattintva.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="A kapcsolatok szerkesztését bemutató képernyőkép.":::

1. Szerkessze egyenként a kapcsolatokat a három pont ikon kiválasztásával. Adja hozzá a megfelelő kapcsolatokat.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Az atht képernyőképe az összekötők szerkesztését mutatja be.":::

1. Kapcsolja be a folyamatokat a következő sorrendben:
   - Partnerközpont regisztrációja (Insider Preview)
   - [Customize] (Testreszabás) Részletek létrehozása vagy lekért adatok a Salesforce-ból
   - Közös értékesítésű Referral-Salesforce létrehozása Partnerközpont (Insider Preview)
   - Partnerközpont Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)  
   - Partnerközpont Salesforce (Insider Preview)
   - A Salesforce Partnerközpont (Insider Preview)
   - Salesforce Opportunity to Partnerközpont (Insider Preview)
   - Salesforce Microsoft Solutions to Partnerközpont (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook API-k használata erőforrás-módosítási eseményekre való regisztrációhoz

Az erőforrás-módosítási eseményekre Partnerközpont webhook API-k használatával regisztrálhat. Ezeket a módosítási eseményeket a rendszer HTTP-bejegyzésekként küldi el az URL-címére.

1. Válassza **Partnerközpont Salesforce CRM (Insider Preview)** lehetőséget.

1. Válassza a **Szerkesztés ikont,** majd **a HTTP-kérések esetén lehetőséget.**

1. Kattintson a **Másolás ikonra** a megadott **HTTP POST URL-cím másoláshoz.**

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Az URL-cím másolását bemutató képernyőkép.":::

1. Válassza ki **Partnerközpont webhookregisztráció (Insider Preview)** Power Automate folyamatot, majd válassza a **Futtatás lehetőséget.**

1. Győződjön meg **arról, hogy a Jobb** oldali panelen megnyílik a Folyamat futtatása ablak, és válassza a Folytatás **lehetőséget.**

1. Adja meg a következő részleteket:

   - **HTTP-eseményindító végpontja:** Ez az URL-cím egy korábbi lépésből lett átmásolva.
   - **Regisztrálható** események: Válassza ki az összes elérhető eseményt **(hivatkozás** által létrehozott, **hivatkozás-frissített,** **related-referral-created**, és **related-referral-updated**).
   - **Meglévő triggervégpont felülírása, ha van?**: Igen. Egy adott webhook-eseményhez csak egy URL-cím regisztrálható.

1. Válassza **a Folyamat futtatása,** majd a Kész **lehetőséget.**

A webhook mostantól figyelheti, létrehozhatja és frissítheti az eseményeket.

## <a name="customize-synchronization-steps"></a>Szinkronizálási lépések testreszabása

A CRM-rendszerek nagymértékben testre vannak szabva, és a Power Automate a CRM-beállításoknak megfelelően testre szabhatók. Ha az Partnerközpont és a CRM-rendszer szinkronizálja az értékesítésre vonatkozó hivatkozásokat, a Partnerközpont PC-n szinkronizált mezőket az Egyéni mezőleképezés útmutatója sorolja [fel.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Kövesse a mezőleképezési útmutatót, és ha szükséges, hajtsa végre a megfelelő módosításokat a [Customize] Create or Get Details from Salesforce or environment variables **([Testreszabás] Create or Get Details from Salesforce or** environment variables (A Salesforce-ból vagy környezeti változókból) területen. A megoldás többi folyamatát ne frissítse Power Automate mert az hatással lehet a megoldás jövőbeli frissítésére.

A következő testreszabások érhetők el:

- **Pipa megjelenítése** a lehetőség nevében: Alapértelmezés szerint egy pipa jelenik meg a lehetőség neve mellett, amely jelzi, hogy a Partnerközpont és a Salesforce CRM közötti szinkronizálás sikeresen megtörtént. Hasonlóképpen, ha a szinkronizálás meghiúsul, keresztjel jelenik meg. Ha nem akar pipát vagy keresztjelölést hozzáadni a  lehetőség nevéhez, állítsa a Lehetőség neve környezeti változóban a Megjelenítendő pipa aktuális értékét Nem értékre.

- **Fázis neve:**

  - **Aktív fázis neve:** Ez a fázis egy lehetőség értékesítési folyamatában a Salesforce-ban.  Egy aktív szakaszt képvisel, és egyenértékű egy elfogadott állapotban lévő ajánlással a Partnerközpont. Ez lehet az értékesítési folyamat következő fázisa a visszatartott szakasz után. Ha a Lehetőség értékesítési szakaszát a "hold" fázisból aktív szakaszba ugorja, a rendszer elfogadja a Partnerközpont és a módosítások szinkronizálása meg fog kezdődni.

  - **On-hold stage name**:A fázis neve egy lehetőség értékesítési folyamatában a Salesforce-ban. Ez egy hold-hold fázist képvisel. A Microsofttól megosztott, még nem elfogadott új társértékesítési ajánlások erre a fázisra lesznek beállítva a Salesforce-ban. Az adott lehetőségben a "hold" fázisban végrehajtott módosítások nem szinkronizálódnak a Partnerközpont. Ha a Lehetőség értékesítési szakaszát ebből a visszatartott szakaszból kiveszi, a rendszer elfogadja a Partnerközpont és a módosítások szinkronizálása meg fog kezdődni.

- **Ügyfélfiók országkódja:** Új ajánlás létrehozásakor kötelező megadni egy kétbetűs országkódot (ISO 3166). Alapértelmezés szerint az országkód szinkronizálva lesz a fiók **BillingCountry mezőjéből** a Salesforce-ban. Ha a Salesforce-ban egy másik mező van, amelyből az országkód szinkronizálható:

  - Kétbetűs kódot tartalmazó fiók nem lookup országkód mezőjéhez:

    - Frissítse **az Ügyfélfiók országkódja** mező nevét a Salesforce környezeti változóban a CRM mezőnevével. Ügyeljen arra, hogy a mező nevét adja meg, ne a megjelenítendő nevét.

    - Szerkessze **a** **[Testreszabás] Create or Get Details from Salesforce**(Részletek létrehozása vagy lekért részletei) adatokat a Salesforce-ból, majd a **CRM-ben** az Ügyfélfiók létrehozása vagy lekérte művelettel rendeljen egy Ország értéket a MEGFELELŐ mezőhöz a CRM-ben. Emellett távolítsa el az **Ország** érték-hozzárendelést a **BillingCountry (Számlázási ország) mezőből.**

  - Keresésalapú országkód-mező a fiókban:

    - Adjon hozzá egy új egyéni mezőt a fiókban, és töltse ki automatikusan egy kétbetűs országkóddal (ISO 3166) a keresőmezőben kiválasztott érték alapján, és fordítva.

    - Kövesse az előző lépéseket a nemlookup országkód mezőhöz egy új egyéni mező szinkronizálásához a CRM-től a Partnerközpont.

- **Ajánlat értéke:** Alapértelmezés szerint a rendszer szinkronizálja a Partnerközpont értékét a **CRM-ben** az Összeg értékével. Ha a CRM-ben egy másik mező van, amelyből az üzlet értéke szinkronizálható:

  - Frissítse **az Deal value mező** nevét a Salesforce környezeti változóban a CRM mezőnevével. Ügyeljen arra, hogy a mező nevét adja meg, ne a megjelenítendő nevét.

  - Szerkesztés **[Testreszabás]** A Salesforce-ból létrehozhat  vagy lekért részleteket, majd a  Lehetőség létrehozása vagy frissítése a CRM-ben területen frissítheti az Új lehetőség létrehozása és a Meglévő lehetőség frissítése műveleteket, hogy a **DealValue** a megfelelő mezőhöz legyen hozzárendelve **a** Salesforce-ban.

- **Ajánlat érték pénznemkódja:** Az üzlet érték pénznemkódmezője a Salesforce-ban. Ez a mező API-neve lesz használva a Lehetőség ajánlatértékének pénznemkódjának lekért értékéhez, amikor a Microsoft-fiókban létrehozza vagy frissíti a Partnerközpont. Ha az deal value currency kódmező eltér az alapértelmezett **CurrencyIsoCode** mezőtől, frissítse ennek a környezeti változónak az aktuális értékét.

  - Frissítse **az Deal value currency** mező nevét a Salesforce környezeti változóban a CRM mezőnevével. Ügyeljen arra, hogy a mező nevét adja meg, ne a megjelenítendő nevét.

  - Szerkesztés **[Testreszabás]** A Salesforce-ból létrehozhat  vagy lekért részleteket, majd a  Lehetőség létrehozása vagy frissítése a CRM-ben területen frissítheti az Új lehetőség létrehozása és **a** Meglévő lehetőség frissítése műveleteket, hogy a **DealValueCurrency** érték a Salesforce megfelelő mezőjéhez legyen hozzárendelve.

- **Társértékesítési lehetőség szinkronizálása:** Ha igenre van **állítva,** csak az együttértékesítési és folyamatmegosztási lehetőségek lesznek szinkronizálva a Partnerközpont Salesforce-ból. Ha a **nem,** akkor az érdeklődők, az értékesítések és a folyamatmegosztási lehetőségek szinkronizálva lesznek a Partnerközpont Salesforce-hoz. Ez a változó nincs hatással a Salesforce-ból a Partnerközpont.

## <a name="update-environment-variable"></a>Környezeti változó frissítése

Környezeti változó értékének frissítése:

1. A Megoldások **lapon** válassza az Alapértelmezett **megoldás lehetőséget.** Válassza **a Környezeti változó lehetőséget** az Összes lehetőség **kiválasztásával.**

1. Válassza ki a frissíteni kívánt érték környezeti változóját, majd válassza a Szerkesztés lehetőséget a három pont ikon használatával. 

1. Frissítse **az Aktuális értéket** (ne frissítse az  alapértelmezett **értéket)** az Új érték lehetőséggel, és az értéket meg kell adva. Az értéknek egyeznie kell a változó adattípusának. Az Igen vagy a Nem adattípus például az Igen vagy a Nem értéket fogadja el.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="A környezeti változók frissítését bemutató képernyőkép.":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Kétirányú kétirányú kétirányú értékesítés – hivatkozásszinkronizálás végpontok között

Miután telepítette, konfigurálta és testreszabta a Power Automate-megoldást, tesztelheti a Salesforce CRM és a Partnerközpont.

### <a name="pre-requisites"></a>Előfeltételek

A Partnerközpont és a Salesforce CRM közötti szinkronizáláshoz a Power Automate megoldásnak egyértelműen el kell különítenünk a Microsoft-specifikus javaslatmezőket. Ez az azonosítás lehetővé teszi az értékesítő csapatok számára, hogy eldöntsék, mely terjesztéseket szeretnék megosztani a Microsofttal az értékesítéshez.

Egyéni mezők egy készlete érhető el a Partnerközpont a Salesforce CRM megoldáshoz Lehetőség **entitás** részeként. A CRM-rendszergazdáknak külön CRM-szakaszt kell létrehozniuk a **Lehetőség egyéni mezőkkel.**

Az alábbi egyéni mezőknek a CRM szakasz részeinek kell lennie:

- **Szinkronizálás Partnerközpont:** Azt határozza meg, hogy szinkronizálja-e a lehetőséget a Partnerközpont. Alapértelmezés szerint a mező értéke Nem, és az értékesítőnek explicit módon Igen értékre kell állítania, hogy megoszton egy lehetőséget a Microsofttal. A CRM-hez Partnerközpont új hivatkozások mezőértéke Igen értékre lesz állítva.

- **Ajánlóazonosító:** A Microsoft által megadott, csak olvasható Partnerközpont mező.

- **Hivatkozás hivatkozása:** A Microsoft-fiókban található hivatkozás csak olvasható Partnerközpont.

- **Hogyan segíthet a Microsoft:** Segítségre van szükség a Microsofttól a hivatkozáshoz? Egy közös értékesítésre vonatkozó ajánlás létrehozásához válassza ki a Microsofttól szükséges megfelelő súgót. Az ügyfélkapcsolatot társnak kell társítanunk ahhoz a lehetőséghez, hogy közös értékesítésre vonatkozó ajánlást hozzunk létre. Nem közös értékesítésre vonatkozó ajánlás létrehozásához ne jelölje ki ezt a mezőt. A nem közös értékesítésre vonatkozó ajánlás bármikor átalakítható egy közös értékesítésre vonatkozó ajánlásra a megfelelő, segítségre van szükség lehetőség kiválasztásával.

- **Microsoft Partnerközpont Hivatkozás láthatósága:** Válassza ki a Partnerközpont láthatóságát. Ha láthatóvá teszi a Microsoft értékesítői számára, előfordulhat, hogy egy nem közös értékesítésre vonatkozó ajánlás át lesz alakítva közös értékesítésre. Ha Microsoft-segítségre van szükség, a hivatkozás alapértelmezés szerint látható a Microsoft értékesítői számára. Miután ez a mező láthatóként van megjelölve, nem lehet visszaállni.

- **Microsoft CRM azonosító:** Ha a Microsoft létrehoz és elfogad egy közös értékesítésre vonatkozó ajánlást, ez a mező a Microsoft CRM-azonosítóját fogja tartalmazni.

- **Microsoft Partnerközpont Solutions:** Egyéni objektum, amely az értékesítésre kész megoldásokat vagy a Microsoft-megoldásokat társítja a lehetőséggel. Egy vagy több megoldás hozzáadható vagy eltávolítható a lehetőségből. Mielőtt megosztja a Microsofttal, kötelező legalább egy értékesítésre kész vagy Microsoft-megoldást hozzáadni a lehetőséghez. Az objektum lehetőséghez való társításához frissítse a **Lehetőség** űrlapot a CRM-ben.

- **Naplózás:** Csak olvasható auditálási napló a Partnerközpont való szinkronizáláshoz

### <a name="scenarios"></a>Forgatókönyvek

1. Hivatkozásszinkronizálás a CRM-ben történő hivatkozás létrehozásakor vagy frissítésekor és a következő Partnerközpont:

   1. Jelentkezzen be a Salesforce CRM-környezetbe egy olyan felhasználóval, aki látható a CRM **Lehetőség** szakaszában.

   1. Győződjön meg arról, hogy a **Microsoft Partnerközpont** szakasz jelen van, amikor új **lehetőséget** hoz létre a Salesforce CRM-környezetben.

   1. A Salesforce CRM-ben Partnerközpont sikeres szinkronizálási lehetőségeket ✔ ikon jelöli.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="A Salesforce-környezet képernyőképe.":::

   1. A lehetőség Microsoft-fiókkal való Partnerközpont a következő mezőket kell beállítania a kártyanézetben:

      - **Hogyan segíthet a Microsoft?**: Egy közös értékesítésre vonatkozó ajánlás létrehozásához válasszon ki egy megfelelő súgó lehetőséget.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="A kártyanézet megfelelő mezőinek lekért adatait bemutató képernyőkép.":::

      - **Szinkronizálás Partnerközpont:** Igen
      - **Ügyfélkapcsolat:** Egy közös értékesítésre vonatkozó ajánlás létrehozásához adjon hozzá egy ügyfélkapcsolatot a lehetőséghez.
      - **Microsoft-megoldások:** Ha meg szeretne osztani egy javaslatot a Microsofttal, adjon hozzá egy érvényes, közös értékesítésre kész megoldást vagy a Microsoft-megoldást a lehetőséghez.

   1. Miután beállította a Szinkronizálás a következővel **lehetőséget Partnerközpont** **Igen,** várjon 10 percet, jelentkezzen be a Partnerközpont fiókjába. A rendszer szinkronizálja a hivatkozásokat a Salesforce CRM-mel, a hivatkozás pedig ki lesz töltve. Ha hiba történik, a rendszer a naplózási mezőt hibainformációkkal tölti fel.

   1. Hasonlóképpen, ha **a** Szinkronizálás az Partnerközpont beállítás igenre van állítva, ha frissíti a lehetőséget a Salesforce CRM-ben, a módosítások szinkronizálva lesznek a Partnerközpont fiókjával.

2. Hivatkozásszinkronizálás a Microsoft-ügyfélben létrehozott vagy frissített hivatkozások Partnerközpont Salesforce CRM-környezetben való szinkronizálása esetén:

    1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard/home)

    1. A **bal oldali** menüben válassza a Hivatkozások lehetőséget.

    1. Hozzon létre egy új közös értékesítésre vonatkozó ajánlást a Partnerközpont "Új üzlet" lehetőségre kattintva.

    1. Jelentkezzen be a Salesforce CRM-környezetbe.

    1. Lépjen a **Megnyitási lehetőségek lapra.** A Microsoft Partnerközpont létrehozott ajánlás most már szinkronizálva van a Salesforce CRM-ben.

    1. Szinkronizált hivatkozás kiválasztásakor a rendszer feltölti a kártyanézet részleteit.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="A Salesforce lehetőségoldalának képernyőképe.":::

>[!NOTE]
>**Segítségre van szüksége az üzembe helyezéssel?**
>Ha segítségre van szüksége az értékesítési ajánlási összekötő üzembe helyezésével kapcsolatosakhoz, kapcsolatba kell lépjen egy partner műszaki tanácsadójával. Segítséget nyújthatnak az üzembe helyezéshez, és ajánlott eljárásokat nyújthatnak a sikeres implementációhoz.
>
>További információkért lásd: Műszaki előzetes és üzembe [helyezési szolgáltatási](technical-benefits.md) kérés elküldése

## <a name="next-steps"></a>Következő lépések

- [Érdeklődők kezelése](manage-leads.md)

- [Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)

- [Partnerközpont – webhookok](/partner-center/develop/partner-center-webhooks)
