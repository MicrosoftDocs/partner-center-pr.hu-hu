---
title: A Dynamics 365 CRM-hez készült közös Partnerközpont
description: Szinkronizálhatja a Partnerközpont a Dynamics 365 CRM-hez készült közös értékesítés összekötővel. Ezután a Microsofttal együtt értékesíthet a CRM-rendszerből.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: c399e00394208ec29dd59a41afe7cce1b1d07253
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284332"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>A Dynamics 365 CRM-hez készült közös értékesítés összekötő áttekintése

**Megfelelő szerepkörök**

- Ajánlói rendszergazda
- Rendszergazda vagy rendszer-testreszabó a CRM-ben

Partnerközpont összekötők lehetővé teszik az értékesítők számára, hogy az Ön CRM-rendszereiből együtt értékesítsen a Microsofttal. Nem kell betanítanunk őket ahhoz, hogy az Partnerközpont az közös értékesítések kezeléséhez. Az együttműködési összekötők használatával létrehozhat egy új közös értékesítésre vonatkozó ajánlást, amely kapcsolatba fog hozni egy Microsoft-értékesítőt, használhatja a Microsoft értékesítőjéhez, elfogadhatja vagy elutasíthatja a hivatkozásokat, valamint módosíthatja az olyan ajánlatadatokat, mint az üzlet értéke és a záró dátum. Az ilyen együttműködési ügyletekről a Microsoft értékesítőitől is kaphat frissítéseket. Az összes ajánlását a választott CRM-ben kezelheti, nem pedig Partnerközpont.

A megoldás a Power Automate alapul, és Partnerközpont API-kat használ.

## <a name="prerequisites"></a>Előfeltételek

A megoldás telepítése előtt győződjön meg arról, hogy megfelel az alábbi előfeltételeknek.

|**Témakörök**   |**Részletek**   |**Hivatkozások**   |
|--------------|--------------------|------|
|Microsoft Partner Network (MPN) azonosítója |Szüksége van egy érvényes MPN-azonosítóra.|[Csatlakozás a partnerhálózathoz](https://partner.microsoft.com/)|
|Készen áll az értékesítésre|Az IP-/szolgáltatási megoldásnak készen kell állnia az értékesítésre.|[Értékesítés a Microsofttal](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Partnerközpont-fiók|Az Partnerközpont bérlőhöz társított MPN-azonosítónak meg kell egynie az együttműködési megoldáshoz társított MPN-azonosítóval. Az összekötők üzembe helyezése előtt ellenőrizze, hogy látja-e az közös értékesítésre vonatkozó Partnerközpont portálon.|[Saját fiók kezelése](create-user-accounts-and-set-permissions.md)|
|Partnerközpont felhasználói szerepkörök|Az összekötőket telepítő és azt felhasználó alkalmazottnak ajánlói rendszergazdának kell lennie.|[Felhasználói szerepkörök és engedélyek hozzárendelése](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|A CRM felhasználói szerepkör a Rendszergazda vagy a Rendszer testreszava.|[Szerepkörök hozzárendelése a Dynamics 365-ben](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power Automate flow-fiók|Hozzon létre egy új éles környezetet egy adatbázissal teszteléshez, előkészítéshez és éles környezethez. Ha van egy meglévő éles környezete egy adatbázissal, az újra felhasználható. Az összekötő-megoldást telepítő felhasználónak licenccel és Power Automate kell lennie ehhez a környezethez. Ha a telepítés sikertelen, nyomon követheti a folyamat előrehaladását, és további Power Automate [is](https://flow.microsoft.com/) kaphat. A **Megoldások alatt válassza az Előzmények** megtekintése **lehetőséget.**|[Környezet létrehozása vagy kezelése](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>A Partnerközpont szinkronizálásának telepítése a Dynamics 365-hez (Power Automate megoldás)

1. A jobb [felső Power Automate](https://flow.microsoft.com)válassza a **Környezetek** lehetőséget. Ez a lépés az elérhető CRM-példányokat mutatja be.

1. Válassza ki a megfelelő CRM-példányt a jobb felső sarokban található legördülő listából.

1. A **bal oldalon** válassza a Megoldások lehetőséget.

1. Válassza a **felső menü Open AppSource (AppSource** megnyitása) hivatkozását.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Képernyőkép az Open AppSource-ról.":::

1. Az **előugró Partnerközpont keresse meg a Dynamics 365-höz** használható ajánlói összekötőket.  

1. Kattintson a **Lekért most gombra,** majd válassza a Folytatás **lehetőséget.**

1. Megjelenik egy oldal, ahol kiválaszthatja a CRM-környezetet (Dynamics 365) az alkalmazás telepítéséhez. Elfogadja a használati feltételeket.

1. Nyomon követheti a folyamat előrehaladását, és ha a telepítés sikertelen, további részleteket kaphat a Power Automate **Az** előzmények megtekintése lehetőség kiválasztásával a **Megoldások alatt.**

1. A telepítés befejezése után vissza kell mennie a Power Automate [a](https://flow.microsoft.com) bal oldalon válassza a **Megoldások** lehetőséget. **Partnerközpont Dynamics 365** szolgáltatásra vonatkozó hivatkozásszinkronizálás már elérhető a **Megoldások listában.**

1. Válassza **Partnerközpont a Dynamics 365 ajánlói szinkronizálása lehetőséget.** A következő Power Automate folyamatok és entitások érhetők el.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Az elérhető CRM-eket bemutató képernyőkép.":::

## <a name="test-before-you-go-live"></a>Tesztelés az élő adás előtt

Mielőtt telepíti, konfigurálja és testreszabja az Power Automate-megoldást az éles környezetben, mindenképpen tesztelje a megoldást egy átmeneti CRM-példányon. A következőre lesz szüksége:

- Telepítse a Power Automate megoldást egy átmeneti környezet CRM-példányára.
- A megoldás konfigurálása és Power Automate átmeneti környezetben.
- Tesztelje a megoldást egy átmeneti CRM-példányon.
- Sikeres teszt után importálja felügyelt megoldásként az éles példányba.

## <a name="configure-the-solution"></a>A megoldás konfigurálása

1. Miután telepítette a megoldást a CRM-példányban, vissza a [Power Automate.](https://flow.microsoft.com/)

1. A jobb **felső** sarokban található Környezetek legördülő listában válassza ki azt a CRM-példányt, ahová a Power Automate telepítette.

1. A három felhasználói fiókot társító kapcsolatokat kell létrehoznia:

   - Partnerközpont hivatkozási rendszergazdai hitelesítő adatokkal
   - Partnerközpont – események
   - CRM-rendszergazda a Power Automate folyamatokkal a megoldásban

   1. A **bal oldalon** válassza a Kapcsolatok lehetőséget, majd Partnerközpont a listából a Partnerközpont **megoldás** listában.

   1. Hozzon létre egy kapcsolatot a **Kapcsolat létrehozása lehetőség kiválasztásával.**

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="A Kapcsolat létrehozása képernyőképe.":::

   1. Keressen a **Partnerközpont (előzetes verzió)** kifejezésre a jobb felső sarokban található keresősávban.

   1. Hozzon létre egy kapcsolatot a Partnerközpont a ajánlói rendszergazda hitelesítőadat-szerepkörében.

   1. Ezután hozzon létre egy Partnerközpont Események kapcsolatot a Partnerközpont a ajánlói rendszergazdai hitelesítő adatokkal.

   1. Hozzon létre egy kapcsolatot a Common Data Service-hez (az aktuális környezethez) a CRM-rendszergazda felhasználója számára.
     
   1. Az összes kapcsolat hozzáadása után a következő kapcsolatoknak kell látszani a környezetében.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="A kapcsolatokat bemutató képernyőkép.":::

## <a name="edit-the-connections"></a>A kapcsolatok szerkesztése

1. Térjen vissza a **Megoldások lapra,** és válassza az **Alapértelmezett megoldás lehetőséget.** Válassza **a Kapcsolati referencia (előzetes verzió) lehetőséget** az Összes lehetőség **kiválasztásával.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="A kapcsolatok szerkesztését bemutató képernyőkép.":::

1. Szerkessze egyenként a kapcsolatokat a három pont ikon kiválasztásával. Adja hozzá a megfelelő kapcsolatokat.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Képernyőkép a felsorolt kapcsolatokról.":::

1.  Térjen vissza a **Megoldások** lapra, válassza a **Partnerközpont-szinkronizálás a Dynamics 365-hez** lehetőséget, és kapcsolja be a folyamatot az egyes folyamat melletti három pont ikonra kattintva a következő sorrendben. Ha problémákba ütközik a folyamat bekapcsolása közben, tekintse meg a Testreszabási lépések [és](connector-dynamics.md#customize-synchronization-steps) a [Hibaelhárítási lépések témakört.](connectors-troubleshoot.md)

Kapcsolja be a folyamatokat a következő sorrendben:

- Partnerközpont webhookregisztráció (Insider Preview)
- Közös értékesítésre vonatkozó ajánlás létrehozása – Dynamics 365 to Partnerközpont (Insider Preview)
- [Customize] (Testreszabás) Adatok létrehozása vagy lekért adatok a Dynamics 365-folyamatból
- Partnerközpont Dynamics 365 – Helper (Insider Preview)
- Partnerközpont Dynamics 365 (Insider Preview) microsoftos közös értékesítésre vonatkozó hivatkozási frissítései
- Partnerközpont Dynamics 365 (Insider Preview)
- Dynamics 365 to Partnerközpont (Insider Preview)
- Dynamics 365 Opportunity to Partnerközpont (Insider Preview)
- Dynamics 365 Microsoft Solutions to Partnerközpont (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook API-k használata erőforrás-módosítási eseményekre való regisztrációhoz

Az erőforrás-módosítási eseményekre Partnerközpont webhook API-k használatával regisztrálhat. Ezeket a módosítási eseményeket a rendszer HTTP-bejegyzésekként küldi el az URL-címére.

1. Válassza **Partnerközpont a Dynamics 365 (Insider Preview)** lehetőséget.

1. Válassza a **Szerkesztés ikont,** majd a **HTTP-kérések esetén lehetőséget.**

1. Kattintson a **Másolás ikonra** a megadott HTTP POST URL-cím másoláshoz.

   :::image type="content" source="images/webhook-video.gif" alt-text="Képernyőkép az erőforrás-módosítások webhookokkal való regisztrálásával.":::

1. Válassza ki **Partnerközpont webhookregisztráció (Insider Preview)** Power Automate, majd válassza a **Futtatás lehetőséget.**

1. Győződjön meg **arról, hogy a Jobb** oldali panelen megnyílik a Folyamat futtatása ablak, és válassza a Folytatás **lehetőséget.**

1. Adja meg a következő részleteket:

   - **HTTP-eseményindító végpontja:** Ez az URL-cím egy korábbi lépésből lett átmásolva.
   - **Regisztrálható** események: Válassza ki az összes elérhető eseményt **(hivatkozás** által létrehozott, **hivatkozás-frissített,** **related-referral-created**, és **related-referral-updated**).
   - **Meglévő triggervégpont felülírása, ha van?**: Igen. Egy adott webhook-eseményhez csak egy URL-cím regisztrálható.

1. Válassza **a Folyamat futtatása,** majd a Kész **lehetőséget.**

A webhook mostantól figyelheti, létrehozhatja és frissítheti az eseményeket.

## <a name="customize-synchronization-steps"></a>Szinkronizálási lépések testreszabása

A CRM-rendszerek nagymértékben testre szabhatók, és a Power Automate a CRM-beállításoknak megfelelően testre szabhatja a megoldást. Ha az Partnerközpont és a CRM-rendszer szinkronizálja az értékesítésre vonatkozó hivatkozásokat, a Partnerközpont PC-n szinkronizált mezőket az Egyéni mezőleképezés útmutatója sorolja [fel.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Kövesse a mezőleképezési útmutatót, és ha szükséges, hajtsa végre a megfelelő módosításokat a **[Customize] Create or Get Details from Dynamics 365 flow or** environment variables (A Dynamics 365 folyamat- vagy környezeti változóinak létrehozása vagy leése) című témakörben. A megoldás többi folyamatát ne frissítse Power Automate mert az hatással lehet a megoldás jövőbeli frissítésére.

A következő testreszabások érhetők el:

- **Pipa megjelenítése** a lehetőség nevében: Alapértelmezés szerint pipa jelenik meg a lehetőség neve mellett, amely jelzi, hogy a Partnerközpont és a Dynamics 365 CRM közötti szinkronizálás sikeresen megtörtént. Hasonlóképpen, ha a szinkronizálás meghiúsul, keresztjel jelenik meg. Ha nem akar pipát vagy keresztjelölést hozzáadni a  lehetőség nevéhez, állítsa a Lehetőség neve környezeti változóban a Megjelenítendő pipa aktuális értékét Nem értékre.
- **Ajánlat értéke:** Alapértelmezés szerint a rendszer szinkronizálja a Partnerközpont értékét a CRM **estimatedvalue** értékével. Ha a CRM-ben egy másik mező van, amelyből az üzlet értéke szinkronizálható:

  - Frissítse **az Deal value** mező nevét a Dynamics 365 környezeti változóban a CRM mezőnevével. Ügyeljen arra, hogy a mező nevét adja meg, ne a megjelenített nevét.
  - Szerkesztés **[Testreszabás] A Dynamics 365-folyamat** létrehozása  vagy beszerkesztés művelete, majd  a Lehetőség létrehozása vagy frissítése a CRM-ben területen frissítse az Új lehetőség létrehozása és **a** Meglévő lehetőség frissítése műveleteket, hogy az **DealValue** értéket a crm megfelelő mezőjéhez rendelje. Emellett távolítsa el az **DealValue** hozzárendelést a **Becsült bevétel mezőből.**

- **Ügyfélfiók országkódja:** Új hivatkozás létrehozásakor kötelező megadni egy kétbetűs országkódot (ISO 3166). Alapértelmezés szerint az országkód szinkronizálva lesz a fiók fiók address1_country **mezőjéből** a CRM-ben. Ha a CRM-ben egy másik mező van, amelyből az országkód szinkronizálható:

   - Kétbetűs kódot tartalmazó fiók nem keresett országkód mezőjéhez:
     - Frissítse az **Ügyfélfiók országkódja** mező nevét a Dynamics 365 környezeti változóban a CRM mezőnevével. Ügyeljen arra, hogy a mező nevét adja meg, ne a megjelenített nevét.
     - Szerkesztés **[Testreszabás] A Dynamics 365-folyamat** létrehozása  vagy lekért adatai elemre, majd a CRM-művelet Ügyfélfiók létrehozása vagy lekért lépésével rendeljen egy **Ország** értéket a MEGFELELŐ mezőhöz a CRM-ben. Emellett távolítsa el az **Ország** érték-hozzárendelést az **Address 1: Country/Region (Cím 1: Ország/régió) mezőből.**

   - Keresésalapú országkódmező a fiókban:
     - Adjon hozzá egy új egyéni mezőt a fiókhoz, és töltse ki automatikusan egy kétbetűs országkóddal (ISO 3166) a keresőmezőben kiválasztott érték alapján, és fordítva.
     - Kövesse az előző lépéseket a nemlookup országkód mezőhöz egy új egyéni mező szinkronizálásához a CRM-től a Partnerközpont.

- **Lehetőségmezők:** Ha **kötelezően**  kitöltendő mezőket kell megadni a Lehetőség mezőben, szerkessze a [Testreszabás] létrehozására vagy lekért adatokra vonatkozó adatokat a **Dynamics 365-folyamatból,** majd a CRM-ben kattintson a Lehetőség létrehozása vagy frissítése elemre, és frissítse az Új lehetőség létrehozása műveletet, hogy értékeket rendeljen a kötelező mezőkhöz az üzleti követelmények alapján. 
- **Érdeklődőmezők:** Ha kötelező mezőket kell feltölteni az Érdeklődő mezőben, szerkessze a [Testreszabás] Létrehozás  vagy Részletek lefutása **a Dynamics 365-folyamatból** című témakört, majd az Érdeklődő létrehozása vagy frissítése a CRM-ben, és frissítse az Új érdeklődő létrehozása műveletet, hogy értékeket rendeljen **a** kötelező mezőkhöz az üzleti követelmények alapján. 
- **Ügyfélfiók:** Amikor egy új javaslat szinkronizálva van az Partnerközpont-ból a CRM-be, az Power Automate-megoldás megpróbál egy meglévő fiókot keresni a CRM-ben az ügyfél cégnevének és irányítószámának használatával. Ha nem talál ilyen fiókot, a rendszer létrehoz egy új ügyfélfiókot a CRM-ben. A keresési feltételek és az új fiók létrehozásának részleteinek frissítéséhez szerkessze a  **[Testreszabás] Create or Get Details from Dynamics 365 flow (A Dynamics 365-folyamat** létrehozása vagy lekérdezése) parancsát, majd a CRM és az Ügyfélfiók létrehozása műveletben keresse meg az Ügyfélfiók létrehozása vagy beszerkesztása **adatokat.**

## <a name="update-environment-variable"></a>Környezeti változó frissítése

Környezeti változó értékének frissítése:

1. A Megoldások **lapon** válassza az Alapértelmezett **megoldás lehetőséget.** Válassza **a Környezeti változó lehetőséget** az Összes lehetőség **kiválasztásával.**

1. Válassza ki a frissíteni kívánt érték környezeti változóját, majd válassza a Szerkesztés lehetőséget a három pont ikon használatával. 

1. Frissítse **az Aktuális értéket** (ne frissítse az  alapértelmezett **értéket)** az Új érték lehetőséggel, és az értéket meg kell adva. Az értéknek egyeznie kell a változó adattípusának. Az Igen vagy a Nem adattípus például az Igen vagy a Nem értéket fogadja el.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="A környezeti változók frissítését bemutató képernyőkép.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Kétirányú kétirányú értékesítés – hivatkozásszinkronizálás végpontok között

Miután telepítette, konfigurálta és testre szabta a Power Automate-megoldást, tesztelheti a Dynamics 365 és a Partnerközpont.

### <a name="prerequisites"></a>Előfeltételek

A hivatkozások szinkronizálásához a Partnerközpont Dynamics 365 CRM-ben az Power Automate megoldás egyértelműen különül el a Microsoft-specifikus javaslatmezők között. Ez az azonosítás lehetővé teszi az értékesítő csapatok számára, hogy eldöntsék, mely terjesztéseket szeretnék megosztani a Microsofttal az közös értékesítés céljából.

A megoldás telepítésének részeként egyéni mezők és objektumok halmaza lesz hozzáadva. A CRM rendszergazdának létre kell hoznia egy külön CRM-szakaszt a **Lehetőség egyéni mezőkkel.**

Az alábbi egyéni mezőknek a CRM szakasz részeinek kell lennie:

- **Szinkronizálás a Partnerközpont:** Azt határozza meg, hogy szinkronizálja-e a lehetőséget Partnerközpont. Alapértelmezés szerint a mező értéke Nem, és az értékesítőnek explicit módon Igen értékűnek kell lennie ahhoz, hogy megoszton egy lehetőséget a Microsofttal. A CRM-hez Partnerközpont új hivatkozások mezőértéke Igen értékre lesz állítva.
- **Hivatkozásazonosító:** A hivatkozáshoz csak olvasható Partnerközpont mező.
- **Hivatkozás:** A hivatkozásra mutató csak olvasható hivatkozás a Partnerközpont.
- **Hogyan segíthet a Microsoft?**: Segítségre van szükség a Microsofttól a hivatkozáshoz. Közös értékesítésre vonatkozó ajánlás létrehozásához válassza ki a Microsofttól szükséges megfelelő súgót. Az ügyfélkapcsolatot társítanunk kell egy közös értékesítésre vonatkozó ajánlás létrehozására vonatkozó lehetőséggel. Nem közös értékesítésre vonatkozó ajánlás létrehozásához ne jelölje ki ezt a mezőt. Az nem közös értékesítésre vonatkozó ajánlás bármikor átalakítható közös értékesítésre vonatkozó ajánlásként a megfelelő segítségre van szükség.
- **Microsoft Partnerközpont Hivatkozás láthatósága:** Válassza ki a Partnerközpont láthatóságát. Azáltal, hogy láthatóvá teszi a Microsoft értékesítői számára, előfordulhat, hogy egy nem közös értékesítésre vonatkozó ajánlást átalakítunk közös értékesítésre. Ha Microsoft-segítségre van szükség, a hivatkozás alapértelmezés szerint látható a Microsoft értékesítői számára. Miután ez a mező láthatóként van megjelölve, nem lehet visszaállni.
- **Microsoft CRM-azonosító:** Ha a Microsoft létrehoz és elfogad egy közös értékesítésre vonatkozó ajánlást, ez a mező a Microsoft CRM-azonosítóját fogja tartalmazni.
- **Termékek: Elavult:** Ne használja ezt a mezőt, és ne adja hozzá a CRM szakaszhoz. Csak visszamenőleges kompatibilitáshoz érhető el. Használjon Partnerközpont megoldásokat.
- **Naplózás:** Csak olvasható auditálási napló a Partnerközpont való szinkronizáláshoz.
- **Microsoft Partnerközpont Solutions:** Egyéni objektum, amely az értékesítésre kész megoldásokat vagy a Microsoft-megoldásokat társítja a lehetőséggel. Egy vagy több megoldás hozzáadható vagy eltávolítható a lehetőségből. Mielőtt megosztja a Microsofttal, kötelező legalább egy értékesítésre kész vagy Microsoft-megoldást hozzáadni a lehetőséghez. Az objektum lehetőséghez való társításához frissítse a **Lehetőség** űrlapot a CRM-ben.

  Válassza ki a megfelelő lapot a **Lehetőség űrlapon,** és adjon hozzá egy részrácsot az itt látható módon.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="A Lehetőség űrlapot bemutató képernyőkép.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="A Microsoft Solutions képernyőképe.":::

- A Microsoft-megoldások hozzáadása után előre kitöltheti az értékesítésre kész megoldás részleteit, így az értékesítőknek nem kell hozzáadniuk őket. Új megoldás részleteinek hozzáadásához a CRM-ben válassza a  Microsoft Solution Details objektumot, és válassza a Rekord hozzáadása lehetőséget egy bejegyzés hozzáadásához, vagy használja az **Excel-feltöltést** több bejegyzés hozzáadásához.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Az Új Microsoft-megoldás részleteit bemutató képernyőkép.":::

### <a name="scenarios"></a>Forgatókönyvek

1. Hivatkozásszinkronizálás a CRM-ben történő hivatkozás létrehozásakor vagy frissítésekor és a következő Partnerközpont:

   1. Jelentkezzen be a Dynamics 365 CRM-környezetbe azzal a felhasználóval, aki látható a CRM **Lehetőség** szakaszában.

   1. Ha új lehetőséget hoz létre a Dynamics 365-környezetben, győződjön meg arról, hogy a **Microsoft** Partnerközpont szakasz jelen van.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Képernyőkép az Új lehetőség lehetőségről.":::

   1. A lehetőség és a Partnerközpont a következő mezőket kell beállítania a kártyanézetben:

      - **Hogyan segíthet a Microsoft?**: Egy közös értékesítésre vonatkozó ajánlás létrehozásához válasszon ki egy megfelelő súgó lehetőséget.

         :::image type="content" source="images/dynamic-3a.png" alt-text="A kártyanézet megfelelő mezőinek lekért adatait bemutató képernyőkép.":::

      - **Ügyfélkapcsolat:** Ha közös értékesítésre vonatkozó ajánlást szeretne létrehozni, adjon hozzá egy ügyfélkapcsolatot a lehetőséghez.
      - **Szinkronizálás a Partnerközpont:** Igen.
      - **Microsoft-megoldások:** Ha meg szeretne osztani egy ajánlást a Microsofttal, adjon hozzá egy érvényes, közös értékesítésre kész megoldást vagy Microsoft-megoldást a lehetőséghez.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Képernyőkép a Megoldásazonosítóról.":::

   1. Miután létrehozta a lehetőséget a Dynamics 365-ben, és a Szinkronizálás Partnerközpont beállítás Igen, várjon 10 percet.  Ezután jelentkezzen be Partnerközpont fiókjába. A rendszer szinkronizálja a hivatkozásokat a Dynamics 365-sel és **a hivatkozásazonosítóval.** **A hivatkozás ki** lesz töltve. Hiba esetén a Rendszervizsgálat  mező ki lesz töltve hibainformációkkal.
     
    1. Hasonlóképpen, egy olyan lehetőség esetén, amely Partnerközpont Szinkronizálás az Partnerközpont-val lehetőség igenre lett állítva, ha frissíti a lehetőséget a Dynamics 365 CRM-ben, **a** módosítások szinkronizálva lesznek az Partnerközpont fiókjában.

    1. A Dynamics 365 Partnerközpont ban a ✔ sikeresen szinkronizált lehetőségek azonosíthatók.

1. Hivatkozásszinkronizálás a hivatkozás létrehozásakor vagy Partnerközpont Dynamics 365-környezetben való szinkronizálása esetén:

   1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard/home)

   1. A **bal oldali menüben** válassza a Hivatkozások lehetőséget.

   1. Hozzon létre egy új közös értékesítésre vonatkozó ajánlást a Partnerközpont új **ajánlat lehetőség kiválasztásával.**

   1. Jelentkezzen be a Dynamics 365 CRM-környezetbe.

   1. Nyissa meg a **Lehetőségek megnyitása lehetőséget.** A Partnerközpont létrehozott ajánlás most már szinkronizálva van a Dynamics 365 CRM-ben.

   1. Szinkronizált hivatkozás kiválasztásakor a kártyanézet részletei ki lesznek töltve.

## <a name="next-steps"></a>Következő lépések

- [Érdeklődők kezelése](manage-leads.md)
- [Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)
- [További információ a Microsoft Power Automate platformról](/power-automate/)
- [Partnerközpont – webhookok](/partner-center/develop/partner-center-webhooks)
