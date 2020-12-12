---
title: Problémabejelentés ügyfél nevében
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy mikor kell kibővíteni az ügyfélszolgálati problémát a Microsoftnak, és hogyan lehet támogatási jegyet benyújtani a különböző típusú Microsoft-szolgáltatásokhoz.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: baeb53d237ba1aeb987b08097526eda5c6235512
ms.sourcegitcommit: df7f26b46d1ca46e962e528578d20330804638f9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/11/2020
ms.locfileid: "97153145"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Szolgáltatással kapcsolatos probléma bejelentése az ügyfél nevében – beleértve azt is, hogy mikor és hogyan történik

**A következőre érvényes:**

- Partnerközpont
- A Microsoft Cloud for US Government Partnerközpontja

**Megfelelő szerepkörök**

- Közvetett szolgáltató

Ha az ügyfél olyan szolgáltatási problémát tapasztal, amely nem oldható fel, és amely megfelel a [problémák a Microsoftnak való](escalate-problems-to-microsoft.md)megadásával kapcsolatban ismertetett feltételeknek, a közvetett szolgáltató támogatási jegyet tud benyújtani számukra. Ez a folyamat hasznos lehet a számlázási problémák vagy a viták kiemeléséhez, valamint a csalással kapcsolatos problémák megoldásához is.

## <a name="submit-a-service-request-for-a-customer"></a>Szolgáltatási kérelem küldése az ügyfél számára

1. Válassza a partner Center menü CSP területén a **vevők** lehetőséget.

2. Az ügyfelek lapon válassza ki vagy keresse meg a kívánt ügyfelet
    
3. Az ügyfél menüben válassza a **szolgáltatási kérelmek** elemet.

4. Az **új kérelem** legördülő menüben válassza az **Azure** vagy **az Office 365, a Dynamics 365, a nagyvállalati mobilitási csomag** lehetőséget. A rendszer átirányítja az Microsoft Azure Portal vagy az Office 365 felügyeleti központba.

>[!NOTE]
>Támogatási műveleti partnereink a Dynamics 365-et a CSP-ben lebonyolító támogatási szerződés fenntartásához szükséges a partneri (ASfP) csomag vagy magasabb szintű támogatáshoz. Ez a támogatási szerződés szükséges a Dynamics 365-incidensek beküldéséhez a CSP-ügyfél nevében. [További](https://partner.microsoft.com/support/partnersupport) információ a támogatási szerződés lehetőségeiről.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Ha Azure-beli ügyfél-szolgáltatási kérelmet kell létrehoznia, vegye figyelembe a következőket:
>
>- Ahhoz, hogy Ön, mint a közvetett viszonteladó, szolgáltatási kérelmeket hozzon létre az ügyfél számára az Azure-ban, a közvetett szolgáltatónak hozzáférést kell biztosítania az ügyfél Azure-fiókjához. Ez eltér az Office 365-ügyfelek nevében való felügyelettől.
>
>- Bár a fiókpartner rendszergazdája nem tud szolgáltatási kérelmeket létrehozni az Azure-beli szolgáltatás-portálon, a következő műveleteket végezheti el: hozzon létre egy támogatási csoportot az Azure Service Portalon, és adja meg a csoportnak a támogatási kérések naplózásához szükséges engedélyeket.

1. Válassza az **Új támogatási kérelem** lehetőséget.

2. Töltse ki a támogatási kérést a megfelelő információkkal, majd válassza a **Létrehozás** lehetőséget:

   - A támogatási kérelem **alapjai** szakaszban válassza ki a **Cloud Solution Provider** elemet a **támogatási csomag** mezőben.

   - A támogatási kérelem **kapcsolattartási** adatok szakaszában adja meg az adatait, nem az ügyfél adatait.

3. Később tekintse át az ügyfél szolgáltatási kérelmeit a Microsoft Azure Portalon a **támogatási kérések kezelése** lehetőség kiválasztásával.

Előfordulhat, hogy létre kell hoznia egy támogatási kérést az ügyfél számára, ha nem rendelkezik rendszergazdai engedélyekkel az adott ügyfél számára. Ez két forgatókönyv egyike esetén fordulhat elő:

- A kapcsolat első létrehozásakor nem kért rendszergazdai jogosultságokat.
- Csak az ügyfél Azure-előfizetéseit kezelheti, így nem rendelkezik rendszergazdai engedélyekkel.
 
Mindkét esetben a következő eljárással hozhat létre támogatási kérést. 

1. Másolja az ügyfél tartománynevét a partner Center fiók lapján.

2. Ugrás a következőre: https://portal.azure.com/ [customerdomainname]. 

3. Válassza ki a támogatást igénylő Azure-előfizetést.

4. Válassza az **új támogatási kérelem** lehetőséget, majd kövesse az utasításokat a kérelem létrehozásához. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, nagyvállalati mobilitási csomag

1. A **szolgáltatási kérelem létrehozása** szakaszban válassza ki a megfelelő támogatási kategóriát. Előfordulhat, hogy további cikkek megtekintéséhez a **továbbiak...** elemre kell kattintania.

2. Fejezze be a szolgáltatáskérelem űrlapot, és válassza a **Küldés** lehetőséget.

   > [!TIP]
   > Ügyeljen arra, hogy a kapcsolattartási adatokat is tartalmazza, ne az ügyfelet.

3. Később tekintse át az ügyfél szolgáltatási kérelmeit, ehhez nyissa meg az Office 365 felügyeleti központot, és kattintson az **összes támogatási jegy megtekintése** lehetőségre.

### <a name="support-for-commercial-marketplace-products"></a>A kereskedelmi piactér termékeinek támogatása

A Microsoft nem nyújt terméktámogatást a kereskedelmi piactér termékeihez. Ahhoz, hogy támogatást kapjon, fel kell vennie a kapcsolatot a terméket közzétevő független szoftvergyártóval (ISV-val).

Az ISV kapcsolattartási adatainak megkeresése:

1.  A **piactér** lapon válassza ki azt a terméket, amelyhez segítségre van szüksége.

2.  A termék oldalán találja a támogatási kapcsolattartási adatokat. A következő lehetőségek közül választhat:

    - Az ISV-k webhelyén található támogatási belépési pontra mutató hivatkozás
    - Támogatási e-mail
    - Támogatási Kapcsolattartó telefonszáma

## <a name="faq"></a>GYIK

Az ügyfél nevében elküldhető szolgáltatási kérelmekkel kapcsolatos gyakori kérdésekért lásd az alábbi információkat. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>Mit tartalmaz a támogatási jogosultság része?

A szolgáltatási kérelmeket a partner centeren keresztül kell benyújtani. Az Azure-hoz, Microsoft Office 365, a Microsoft Dynamics CRM Online-hoz és a nagyvállalati mobilitási csomaghoz is elérhetők. A Cloud Solution Provider programban részt vevő partnerként a legfontosabb problémákra számíthat.

A saját partner bérlő támogatása nem része a CSP támogatási juttatásnak. Azonban az Office 365, a Microsoft Dynamics CRM Online és a nagyvállalati mobilitási csomag nem számít fel külön támogatási előfizetési díjat a partnerek és az ügyfelek számára. Az Azure díj ellenében díjat számítunk fel, de ha Ön jogosult a Cloud support vagy más Microsoft Partner Network-(MPN-) kedvezményre, akkor ezeket a díjakat felhasználhatja.

Ez az előny a Cloud Solution Provider programban résztvevő összes partnerre vonatkozik, függetlenül attól, hogy díjköteles vagy próbaverziós időszakon belül van-e. A számlázási és előfizetés-kezelési támogatást a csomag ingyenes összetevője is tartalmazza.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Milyen gyorsan kapok egy kezdeti választ?

A kezdeti válaszidőt a beküldött incidens súlyossága határozza meg. A probléma súlyosságát a szolgáltatási kérelem elküldésekor felmerülő üzleti hatás határozza meg.

A technikai hibajavítási **incidensek** kezdeti válaszideje:

- Kritikus hatás (A súlyossági szint): 2 óra (a szolgáltatások jelentős elvesztése vagy romlása). Éles üzemi szolgáltatások.)
- Mérsékelt hatás ("B" súlyosság): négy óra (a szolgáltatások mérsékelt elvesztése vagy romlása). Az éles üzemi szolgáltatások részben érintettek.)
- Minimális hatás (súlyosság C): nyolc óra (a szolgáltatások minimális elvesztése vagy romlása). A szolgáltatások továbbra is elérhetők vagy nem éles üzemi szolgáltatásokat érintenek.)

A kezdeti válaszidő csak az angol nyelvű támogatás esetében használható. A helyi nyelvi támogatást munkaidőn belül biztosítjuk.
A támogatási jogosultság határain belüli incidensek esetében, de nem minősülnek a hibajavítási incidenseknek, a kezdeti válaszidő akár egy munkanap is lehet.

### <a name="can-i-submit-a-service-request-by-phone"></a>Küldhetek szolgáltatói kérelmet telefonon?

Nem, a program nem támogatja a telefonos támogatást.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Mi történik, ha bejelentkeznek a Azure Portal és a kikerülő partner Centerbe?

Ha közvetlenül jelentkezik be a Microsoft Azure Portalba, a központot saját kontextusban tekinti meg, nem pedig az ügyfél környezetében. Ezért csak akkor jelentkezzen be közvetlenül a Microsoft Azure Portal, amikor szolgáltatási kérést hoz létre saját előfizetéséhez.

A CSP-program támogatási jogosultsága nem nyújt támogatást a saját partner-előfizetéséhez. Ezért meg kell adnia az érvényes támogatási csomag jogosultságát, ha olyan szolgáltatási kérelmet hoz létre, amely a saját partneri előfizetésére vonatkozik. Ilyenek például az MPN-szerződés azonosítója, Premier vagy egy Azure-támogatási csomag. További információ: [Azure-támogatás – gyakori kérdések](https://go.microsoft.com/fwlink/?LinkId=717532).

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Mi történik, ha bejelentkezik az Office 365 felügyeleti központ portálra, és megkerüli a partneri központot?

Ha közvetlenül az Office 365 felügyeleti központba jelentkezik be, a központot a saját kontextusában, nem pedig az ügyfél környezetében tekintheti meg. Ezért csak akkor jelentkezzen be közvetlenül az Office 365 felügyeleti központba, amikor szolgáltatási kérést hoz létre saját előfizetéséhez.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Hogyan további Dynamics 365-támogatást kaphat?

Ha a következőhöz kapcsolódó problémák merülnek fel: Dynamics 365 csomag előfizetések, licencelés, Számlázás, pénzügyi & műveletek, Dynamics 365 termék-licencek, vagy további technikai támogatásra van szükség:
 
Kapcsolatfelvétel a [Dynamics ügyfélszolgálatával](/dynamics365/customer-engagement/admin/contact-technical-support)

[Microsoft Dynamics-támogatás](https://support.microsoft.com/help/4052881/faq-microsoft-dynamics-365-for-unified-operations-iur) olvasása

## <a name="next-steps"></a>Következő lépések

- [Támogatás biztosítása az ügyfeleknek](customer-support.md)
- [A szolgáltatás állapotának ellenőrzése](check-service-health.md)
