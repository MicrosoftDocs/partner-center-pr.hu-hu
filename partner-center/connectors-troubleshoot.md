---
title: Az közös értékesítésre vonatkozó ajánló összekötők hibaelhárítása
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg az együttműködési összekötők használatával kapcsolatos gyakori kérdésekre adott válaszokat. Olvassa el ezt a gyakori kérdéseket az együttműködési összekötők hibaelhárításáról.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 939654202a370f6d9ba15d9e62a11be44884b613
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284213"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Az közös értékesítésre vonatkozó ajánló összekötők hibaelhárítása

**A következőre érvényes:**

- Dynamics 365 CRM
- Salesforce CRM

**Megfelelő szerepkörök**

- Ajánlói rendszergazda
- Rendszergazda vagy rendszer testreszabó a CRM-ben

 ## <a name="questions-and-answers-about-pre-requisites"></a>Előfeltételekre és válaszokra adott kérdések és válaszok

1. Használhat az Ön környezetében próbaverziós, közös értékesítésre vonatkozó javaslati összekötő megoldást?

Ha a tesztelési/előkészítési környezetben van, választhatja a próbaverziós megoldást. Az összekötők fizetős verziója havonta 15 USD összegben érhető el az AppSource-ban. A fizetős kapcsolattal naponta 10 000 API-hívást kap. Az összekötők a hivatkozási API-k Partnerközpont burkolók. Amikor az összekötő-megoldások létrehozási vagy frissítési eseményen futnak **a** Partnerközpont vagy a CRM oldalán található lehetőségeken, a rendszer API-hívást hoz létre. 

2. Milyen szerepkörre van szüksége szakaszok létrehozásához a CRM-környezetben?

Azok a felhasználók, akik rendszergazdai vagy rendszer-testreszabók, mindenkire alkalmazhatják a módosításokat. Az alkalmazás minden felhasználója azonban személyre szabhatja a rendszert, és akár a testreszabások egy részét megoszthatja másokkal. 

3. A partner értékesítőknek speciális szerepkörökre van szükségük a Partnerközpont?
 
A partner értékesítőknek a "Ajánlói rendszergazda" szerepkört kell hozzárendelni. További információ: [Engedélyek áttekintése.](create-user-accounts-and-set-permissions.md)

4. Milyen mezőket kell először beállítani a CRM-környezetben? 

• Győződjön meg arról, hogy a pénzneme megfelelő az Ön tartózkodási helyének, és hogy pontosan a CRM-környezetben van. • Az értékesítési csapatnak CRM-felhasználóként kell szerepelve lennie a CRM-környezetben.

5. Milyen előfeltételek szükségesek a Power Automate létrehozásához?

A Power Automate a következőre lesz szüksége:

- Egy Power Automate licenc szükséges.
- Legalább 1 GB tárhely szükséges.

6.  Dynamics 365-előfizetésre van szüksége a Salesforce-összekötők megoldásához?

A Salesforce Connector megoldás típusa "Dynamics Flow", amely támogatja a más CRM-rendszerekkel való szinkronizálást. A megoldáshoz nem szükséges Dynamics 365-példány vagy -előfizetés. A Salesforce-megoldás telepítésekor megjelenik egy legördülő lista a vállalat meglévő CDS-környezetéről. Ki kell választania ezt a környezetet. Emellett ha a "Nem található bejelentkezett felhasználóhoz csatlakoztatott Dynamics 365-szervezet" hibaüzenet jelenik meg, akkor új környezetet kell létrehoznia az összekötőhöz.

## <a name="questions-and-answers-about-configuration"></a>Konfigurációval kapcsolatos kérdések és válaszok

1. Mit kell tenni, ha a következő hibaüzenet jelenik meg a folyamatok aktiválása során az Power Automate Platformon?

Hiba: A(z) Azure Resource Manager kérése a következő hibával meghiúsult: {"error":{"code":"WorkflowTriggerNotFound","message":"Az "e14d00f1-1fdf-4b1b-aaac-54a5064093d3" eseményindító "manuális" eseményindítója nem található."}}". 

Kövesse az alábbi hibaelhárítási lépéseket:

- Törölje a CDS-kapcsolatot, majd hozza létre újra a CDS-kapcsolatokat.
- A gyermekfolyam ki- és bekapcsolás 
- Törölje a megoldást, majd telepítse újra a megoldást. 

2.  Mit kell tenni, ha a "Bejelentkezés" hibával szembesül, amikor hozzáad egy Partnerközpont-összekötőt a Power Automate Platformhoz?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Bejelentkezést igénylő hibaüzenet":::

Kövesse az alábbi hibaelhárítási lépést:

- A Partnerközpont hitelesítő adataival jelentkezzen be egyszer a folyamatkörnyezetbe (flow.microsoft.com).


3. Mit kell tenni, ha a következő hibaüzenetet kapja a CRM Partnerközpont-folyamat aktiválása közben a Power Automate Platformon?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Frissítést igénylő hibaüzenet":::

Kövesse az alábbi hibaelhárítási lépéseket:

- Először aktiválja a következő két gyermekfolyamatot, mielőtt aktiválja Partnerközpont CRM-folyamathoz.
      - Partnerközpont CRM – Segítő (Insider Preview)
      - Partnerközpont Crm (Insider Preview) microsoftos közös értékesítésre vonatkozó hivatkozási frissítései

4. Mit kell tenni, ha nem tud kapcsolatokat hozzáadni a folyamathoz, amikor megpróbálja szerkeszteni a folyamatot?

Amíg a folyamat fut, kapcsolatokat adhat hozzá a folyamathoz, és minden folyamatot külön-külön adhat hozzá.  Ha a kapcsolatok hozzáadására szolgáló párbeszédpanel nem nyílik meg automatikusan a folyamat szerkesztése közben, akkor külön-külön szerkesztheti a folyamatok egyes lépéseit és al lépéseit.

- Jelölje ki az egyes folyamatokat, és szerkessze őket egyenként.
- A folyamat összes lépésének kibontása 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Kapcsolatokra van szükség":::

- Válassza ki azokat a lépéseket, ahol megjelenik egy figyelmeztető ikon, amely a kapcsolatok társítását és a kapcsolatok hozzáadását kéri. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Folyamat szerkesztése lépésről lépésre":::


5. Mit kell tenni, ha az együttműködési javaslati összekötők megoldásának folyamatai nem kapcsolnak be?

A. Ebben Power Automate a következő sorrendben kell szerkesztenie a folyamatokat, és frissítenie őket, hogy a megfelelő kapcsolatokat használják:

- Partnerközpont webhookregisztráció (Insider Preview)
- Közös értékesítési ajánlás létrehozása – Salesforce Partnerközpont (Insider Preview)
- Partnerközpont Salesforce (Insider Preview) microsoftos közös értékesítési hivatkozási frissítései
- Partnerközpont Salesforce (Insider Preview)
- Salesforce a Partnerközpont (Insider Preview)
- Salesforce Opportunity to Partnerközpont (Insider Preview)
- Salesforce Microsoft Solutions to Partnerközpont (Insider Preview)

 B. Minden egyes folyamatnál válassza a **Csak felhasználók futtatása lehetőséget.** Válassza **a Kapcsolat használata** lehetőséget a Csak **futtatás felhasználója által biztosított helyett.**  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Folyamat aktiválása":::


C. Aktiválja az alábbi folyamatokat:

 - Partnerközpont Microsoft közös értékesítési hivatkozási frissítései a Salesforce-hoz (Insider Preview)

- Salesforce a Partnerközpont (Insider Preview)

    
D. Aktiválja az összes többi folyamat.

E. A Folyamat Partnerközpont webhookregisztrációnál válassza a **Futtatás lehetőséget.** Adja meg **a http URL-címet** az első műveletből **a Partnerközpont Salesforce-folyamatba.** Válassza ki mind a négy lehetőséget a Regisztrálni kívánt **események** alatt, majd válassza az **Igen** lehetőséget a Felülírás lehetőségnél.

## <a name="questions-and-answers-about-runmaintenance"></a>Kérdések és válaszok a futtatásról/karbantartásról

1. Hogyan háríthatja el a folyamat végrehajtása során Power Automate hibákat?

Annak érdekében, hogy a Power Automate folyamat a vártnak megfelelő legyen, és elhárítsa a végrehajtás közbeni hibákat, tekintse meg a [Folyamathibák kijavítása témakört.](/power-automate/fix-flow-failures)

2. Mit kell tenni, ha olyan hivatkozásokat lát, amelyek nincsenek megfelelően szinkronizálva a Partnerközpont CRM-környezetben?
 
A hivatkozás-szinkronizálás állapotának meghatározásához válassza a Naplózás **lehetőséget.** 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="A hivatkozások szinkronizálása":::

Győződjön meg arról, hogy teljesülnek a következő feltételek:

- A megoldásazonosító a lehetőség részeként van megtéve.

- Kétbetűs országkód szükséges.

- Ha a Microsofttól származó segítség van kiválasztva a lehetőséghez, az ügyfél kapcsolattartási adataira van szükség.

3. Hogyan biztosítható, hogy a hivatkozások kétirányú szinkronizálást biztosítsanak?

Tegye a következőket:

- A partner értékesítőknek meg kell győződni arról, hogy engedélyezték a Szinkronizálás Partnerközpont **lehetőséget** a CRM szakaszban.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Győződjön meg arról, hogy engedélyezte a szinkronizálást":::

- Az értékesítőknek meg kell adniuk a bevételt és a záró dátumot az érdeklődő minősítésekor.

- Ha a CRM-azonosítót  az együttműködési lehetőség létrehozási vagy frissítési szakaszában adja meg, de az adott azonosítóval rendelkező érdeklődői lehetőség nem található a CRM-ben, akkor a rendszer figyelmen kívül hagyja a frissítést vagy létrehozást. 

- Győződjön meg arról, hogy a hivatkozás pénzneme mező be van állítva a Salesforce-környezetben. 

4. Mit kell tenni, ha az összekötő le lesz választva, és nem rendelkezik hivatkozás-szinkronizálással?

Néhány lehetőség a kipróbált lehetőségek közül:

- Ellenőrizze, hogy lejárt-e a felhasználónév vagy jelszó a Partnerközpont-rendszergazdai szerepkörökkel rendelkező felhasználó felhasználója számára.

- A nem szinkronizált lehetőséggel kisebb frissítést is befejezhet, és megfigyelheti, hogy a hivatkozás szinkronizálva lett-e.

- Ha a folyamatok lefuttak és sikertelenek, válassza ki a folyamatot, és küldje el újra a sikertelen futtatásokat.

5. Mit kell tenni, ha hozzáférés-megtagadásos hibákat kap?

Győződjön meg arról, hogy léteznek a megfelelő szerepkörök

- Ajánlói rendszergazdai szerepkör Partnerközpont értékesítő számára 
 
- Rendszergazda vagy rendszer-testreszava szerepkör a CRM-példányon

- Győződjön meg arról, Power Automate flow-fiók felhasználója legalább egyszer https://flow.microsoft.com előre bejelentkezik

6. Ha azt látja, hogy az **ügyfélfiók országkódja** hiányzik egy közös értékesítés létrehozása során, mit kell tennie?

Hozzá kell adni az ISO kétbetűs országkódját az Ügyfélfiókhoz a CRM-ben.

7. Mit kell tenni, ha azt  a hibaüzenetet látja, hogy a megoldásazonosítóra szükség van egy közös értékesítés létrehozása során?

Egy közös értékesítésre vonatkozó javaslat létrehozásához a Microsoft közös értékesítésre kész megoldásra van szüksége. 

8. Mit kell tenni, ha olyan, a crm-sel nem szinkronizált Partnerközpont-ban létrejött, közös értékesítést lehetővé tehetünk, annak ellenére, hogy nincsenek folyamathibák?

Tegye a következőket:

- Miután létrehozott egy új közös értékesítést az Partnerközpont-ban, ellenőrizze, hogy meg lesz-e hívva Partnerközpont-e a Dynamics 365-folyamathoz való Partnerközpont (előfordulhat, hogy többször is meghívja).

- Ha a folyamat meghívásra kerül, ellenőrizze az összes meghívott folyamatot, és azonosítsa a folyamat futását, amely frissíti a CRM-et. A műveleteket követni tudja, és ellenőrizheti, hogy frissült-e a CRM,vagy tapasztalt-e problémát.

- Tekintse **meg az Új üzlet** Partnerközpont, hogy feltöltődik-e a CRM-azonosítóval.

- Győződjön meg arról, hogy az  üzlet nem záródik le véletlenül Won (Megnyert) vagy **Lost** (Elveszett) ként a Partnerközpont.

## <a name="next-steps"></a>Következő lépések

- [Érdeklődők kezelése](manage-leads.md)
 
- [Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)
