---
title: A közös értékesítéssel való átirányítási összekötők hibáinak megoldása
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Válaszok a közös értékesítési összekötők használatával kapcsolatos gyakori kérdésekre. Olvassa el ezt a gyakori kérdéseket a közös értékesítési összekötők hibáinak megoldásához.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/14/2020
ms.locfileid: "92530306"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>A közös értékesítéssel való átirányítási összekötők hibáinak megoldása

**A következőkre vonatkozik:**

- Partnerközpont
- Dynamics 365 CRM
- Salesforce CRM

**Megfelelő szerepkörök**

- Ajánlói rendszergazda
- Rendszerfelügyeleti webszolgáltatások vagy Rendszertestreszabó a CRM-ben

 ## <a name="questions-and-answers-about-pre-requisites"></a>Az előfeltételekkel kapcsolatos kérdések és válaszok

1. Használhat-e a környezetéhez egy próbaverziós, közös értékesítéssel kapcsolatos átirányítási megoldást?

Ha a tesztelési/előkészítési környezetben van, választhatja a próbaverziós megoldást. Az összekötők fizetett verziója a AppSource-on érhető el az USA-ban 15 USD/hó. A fizetős kapcsolatok napi 10K API-hívásokat tesznek szükségessé. Az összekötők a partner Center Referral API-k tetején található burkolók. Ha az összekötői megoldások a partner központ vagy a CRM-oldal lehetőségein a **létrehozási** vagy **frissítési** eseményekhez futnak, egy API-hívás történik.

2. Milyen szerepkörrel kell szakaszt létrehozni a CRM-környezetben?

Azok a felhasználók, akik rendszergazdák vagy rendszertestreszabók, mindenki számára módosíthatják a módosításokat. Az alkalmazás összes felhasználója azonban személyre szabhatja a rendszerállapotot, és másokkal is megoszthatja a testreszabásokat. 

3. A partner-értékesítőknek speciális szerepkörökre van szükségük a partner Centerben való munkához?
 
A partner-értékesítőknek hozzá kell rendelniük az "Ajánlói rendszergazda" szerepkört. További információkért tekintse meg a következő [engedélyek áttekintését) (create-User-accounts-and-set-permissions).

4. Mely mezőket kell elsőként beállítani a CRM-környezetben? 

• Győződjön meg arról, hogy a pénznem megfelelő a tartózkodási helyéhez, és pontosan a CRM-környezetben van. • Az értékesítési csapatnak CRM-felhasználóként kell szerepelnie a CRM-környezetben.

5. Milyen előfeltételek szükségesek a Power automatizáló környezet létrehozásához?

A Power automatizáló környezet használatához a következők szükségesek:

- A rendszer automatizálja a szükséges energiagazdálkodási licencet.
- Legalább 1 GB-nyi tárterület szükséges.

6.  Szüksége van egy Dynamics 365-előfizetésre az Salesforce-összekötők megoldás használatához?

Az Salesforce-összekötő megoldás "Dynamics flow" típusú, amely támogatja a más CRM-rendszerekkel való szinkronizálást. A megoldáshoz nem szükséges Dynamics 365-példány vagy-előfizetés. A Salesforce-megoldás telepítésekor előfordulhat, hogy a vállalat meglévő CDS-környezetének legördülő lista jelenik meg. Ezt a környezetet kell kiválasztania. Továbbá, ha "nem találtunk a bejelentkezett felhasználóhoz csatlakozó Dynamics 365-szervezetet" hibaüzenet jelenik meg, akkor új környezetet kell létrehoznia az összekötőhöz.

## <a name="questions-and-answers-about-configuration"></a>A konfigurációval kapcsolatos kérdések és válaszok

1. Mi a teendő, ha az alábbi hibába ütközne a folyamatok aktiválása a Power automatizáló platformon?

Hiba: a Azure Resource Manager kérése sikertelen volt, hiba: {"Error": {"code": "WorkflowTriggerNotFound", "Message": "a (z)" e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 "trigger" Manual "utasítása nem található."}} ". 

Kövesse az alábbi hibaelhárítási lépéseket:

- Törölje a CDS-kapcsolatot, majd hozza létre újból a CDS-kapcsolatokat.
- A gyermek kikapcsolásának és bekapcsolása 
- Törölje a megoldást, majd telepítse újra a megoldást. 

2.  Mi a teendő, ha a "Bejelentkezés" hibaüzenet jelenik meg egy partneri központ-összekötőnek a Power automatizáló platformban való hozzáadásakor?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Bejelentkezést igénylő hibaüzenet":::

Kövesse ezt a hibaelhárítási lépést:

- A partner Center hitelesítő adataival egyszeri bejelentkezést használhat a flow-környezetbe (flow.microsoft.com).


3. Mi a teendő, ha a következő hibaüzenetet kapja, amikor aktiválja a partneri központot a CRM-folyamatba a Power automatizáló platformon?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Bejelentkezést igénylő hibaüzenet":::

Kövesse az alábbi hibaelhárítási lépéseket:

- Először aktiválja a következő két alárendelt folyamatot a partner központ CRM-folyamatba való aktiválása előtt.
      - Partneri központ és CRM – Helper (belső előzetes verzió)
      - A partner Center Microsoft közös értékesítési hivatkozási frissítései a CRM-ben (belső előzetes verzió)

4. Mi a teendő, ha nem tud kapcsolatokat hozzáadni a folyamathoz, amikor megkísérli a folyamat szerkesztését?

Ha a folyamat futása közben kapcsolatokat ad hozzá a folyamathoz, akkor az egyes folyamatokhoz való hozzáadása külön történik.  Ha a kapcsolatok hozzáadására szolgáló párbeszédpanel nem nyílik meg automatikusan a folyamat szerkesztése közben, akkor a folyamatok egyes lépéseit és allépéseit egyenként is szerkesztheti.

- Válassza ki az egyes folyamatokat, és szerkessze azokat egyenként.
- A folyamat összes lépésének kibontása 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Bejelentkezést igénylő hibaüzenet":::

- Válassza ki azokat a lépéseket, amelyekben a rendszer figyelmeztető ikont kér a kapcsolatok hozzárendelésére, valamint kapcsolatok hozzáadására. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Bejelentkezést igénylő hibaüzenet":::


5. Mi a teendő, ha a közös értékesítésre hivatkozó összekötők megoldásának folyamatai nem kapcsolják be?

A. A Power Gyorsbüféban a folyamatokat a következő sorrendben kell szerkesztenie, és frissítenie kell őket a megfelelő kapcsolatok használatára:

- A partner Center webhook-regisztrációja (belső előzetes verzió)
- Közös értékesítéssel való hivatkozás létrehozása – Salesforce (belső előzetes verzió)
- Partneri központ a Microsoft közös értékesítési hivatkozási frissítései a Salesforce-be (belső előzetes verzió)
- Partneri központ – Salesforce (belső előzetes verzió)
- Salesforce (Insider előzetes verzió)
- Salesforce lehetőség a partneri központhoz (belső előzetes verzió)
- Salesforce Microsoft-megoldások a partner Centerhez (belső előzetes verzió)

 B. Mindegyik folyamat esetében válassza a **csak a felhasználók futtatása** lehetőséget. Válassza a **kapcsolatok használata** lehetőséget a **csak futtatást használó felhasználó** számára.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Bejelentkezést igénylő hibaüzenet":::


C. Aktiválja az alábbi említett folyamatokat:

 - Partneri központ a Microsoft közös értékesítési hivatkozási frissítései a Salesforce-be (belső előzetes verzió)

- Salesforce (Insider előzetes verzió)

    
D. Aktiválja az összes fennmaradó folyamatot.

E. A flow-partneri központ webhookjának regisztrációja lapon válassza a **Futtatás** lehetőséget. Adja meg a Salesforce folyamathoz a **partner Center** első műveletének **http URL-címét** . Válassza a mind a négy lehetőséget a **regisztráláshoz** , majd válassza az **Igen** lehetőséget a felülíráshoz.

## <a name="questions-and-answers-about-runmaintenance"></a>A futtatással/karbantartással kapcsolatos kérdések és válaszok

1. Hogyan történik a hibák elhárítása a Power automatizálási folyamat végrehajtása során?

Ha biztosítani szeretné, hogy a teljesítmény-automatizálási folyamatok a várt módon fussanak, és a hibák elhárítása a végrehajtás során történik, tekintse meg a [folyamatok hibáinak](/power-automate/fix-flow-failures)elhárítása

2. Mi a teendő, ha olyan hivatkozásokat lát, amelyek nincsenek megfelelően szinkronizálva a partner Centerben vagy a CRM-környezetben?
 
Az átirányítási szinkronizálás állapotának meghatározásához válassza a **naplózás** lehetőséget. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Bejelentkezést igénylő hibaüzenet":::

Győződjön meg arról, hogy teljesülnek a következő feltételek:

- A megoldás azonosítója a lehetőség részeként van megadva.

- Két betűs országkód szükséges.

- Ha a Microsoft segítségére van kiválasztva a lehetőségre, az ügyfél kapcsolattartási adatai szükségesek.

3. Hogyan lehet meggyőződni arról, hogy az átirányítások kétirányú szinkronizálást végeznek?

Hajtsa végre a következő lépéseket:

- A partner-értékesítőknek biztosítaniuk kell, hogy engedélyezve legyenek a **partner centerrel való szinkronizálás** a CRM szakaszban.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Bejelentkezést igénylő hibaüzenet" néven a partner Centerben.

## <a name="next-steps"></a>Következő lépések

- [Érdeklődők kezelése](manage-leads.md)
 
- [Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)