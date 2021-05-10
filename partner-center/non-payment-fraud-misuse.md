---
title: Fizetéselmaradás, csalás vagy visszaélés kezelése
description: Megismerheti az online tranzakciók különböző kockázatait, valamint a kockázatok kezeléséhez és enyhítéséhez ajánlott eljárásokat a Partnerközpont.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: c3b7db95bbbd039f8328ddd2785579bb533197cc
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686296"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Fizetés elmaradása, csalás vagy visszaélés a Partnerközpontban

**A következőre érvényes:**

- A Microsoft Cloud for US Government Partnerközpontja

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználókezelő rendszergazda
- Rendszergazdai ügynök
- Számlázási adminisztrátor

Pénzügyi felelősséggel tartozik az ügyfelek és/vagy az ügyfelek által megvásárolt szolgáltatások meg nem fizetése által történő csaló vásárlásokért. Ezért határozottan javasoljuk, hogy helyezzen el csalás elleni megelőzési és *észlelési kockázatcsökkentő intézkedéseket.*

A rosszindulatú tevékenység vagy visszaélés elkerülése és/vagy kezelése érdekében fontos megérteni a lehetséges kockázatokat, és olyan szabályzatokat és eljárásokat kidolgozni, amelyek csökkenthetik a kitettséget.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>A Microsoft elfogadható használatra vonatkozó szabályzatának érvényesítése

Ha a Microsoft olyan partneri vagy ügyféltevékenységet észlel, amely megerősíti, vagy azt gyanítja, hogy megsérti az elfogadható használatra vonatkozó szabályzatot, végre kell léptetjük a kényszerítési lépéseket. Az ügyfél azonnal felfüggeszthető. A Microsoft értesítést kap a kényszerítési műveletekről, vagy frissíti az Ön kérését.

## <a name="abuse-of-service-risks"></a>Szolgáltatási kockázatokkal való visszaélés

**A szolgáltatási kockázatokkal való** visszaélés azt jelenti, hogy a felhőszolgáltatásokat a Microsoft elfogadható használatra vonatkozó szabályzatát megsértő ügyfelek.

### <a name="examples-of-abuse-of-service"></a>Példák a szolgáltatással való visszaélésre

Példák a Microsoft elfogadható használatra vonatkozó szabályzatának megsértésére:

- Spam
- Hacker
- Elosztott szolgáltatásmegtagadásos (DDoS-) támadások
- Bitcoinbányászat
- Kártevők terjesztése
- Előfizetések újraértékesítése

## <a name="theft-of-service-risks"></a>Szolgáltatáslopási kockázatok

**A szolgáltatás ellopása** olyan ügyfeleket jelent, akik nem szándékoznak fizetni a felhasznált szolgáltatásokért. Ez a lopás magában foglalhatja az ellopott fizetési eszközök használatát, hamis számlázási adatok nyújtását és/vagy a tartozások alapértelmezett beállítását.

### <a name="examples-of-service-theft"></a>Szolgáltatáslopási példák

Ilyen online tranzakciós kockázatok például a következők lehetnek:

- Nem személyesen előforduló tranzakciók ("hitelkártya nem jelen" tranzakciók)
- Helytelenül jelenlett identitások
- A kezdeti fizetés előtt kiépített és használt szolgáltatások
- Új piacok és/vagy magas kockázatú régiók online csalások esetén
- Fiók létrehozásának és megvásárlásának automatizálása rossz a szereplőkkel

## <a name="managing-online-risk"></a>Online kockázatok kezelése

Az alábbi javaslatok segítségével olyan szabályzatokat és eljárásokat fejleszthet, amelyek csökkentik az online tranzakciós kockázatoknak való kitettséget az ügyfélkapcsolatok életciklusában.

### <a name="onboarding-new-customers"></a>Új ügyfeleket kell bevetni

Javaslatok az új ügyfelek online kockázatainak csökkentéséhez:

- Ha lehetséges, személyes kapcsolatot létesíthet az ügyfelekkel (például telefonon kapcsolatba léphet az ügyfelekkel).
- Az ügyfelek hitelesítő adatainak és hátterének ellenőrzése jobb módszerekkel (például hitelirodák vagy üzleti kereskedelmi jelentésekkel rendelkező ügynökségek használatával).
- A regisztráció során használjon többtényezős hitelesítést (például SMS-hitelesítést) a robotfiókok létrehozásának és megvásárlásának minimálisra csökkentése érdekében.
- Identitások kezelése és nyomon követése szolgáltatások (például digitális identitásszolgáltatások) használatával.
- Az ügyfelek pénzügyi erősségét szigorú bankkártya-csalásészlelési rendszerekkel mérheti fel.
- Hozzon létre egy egyértelmű gyűjtemény-szabályzatot. Részletezi a gyűjtemények folyamatát, és hogy mikor lesz hatással az előfizetések elérésére a fizetés meg nem fizetése. (Letilthatja a hozzáférést, vagy [felfüggesztheti az](create-a-new-subscription.md#suspend-a-subscription) ügyfél előfizetését fizetés meg nem fizetése esetén.)

### <a name="managing-customer-accounts"></a>Ügyfélfiókok kezelése

Javaslatok az ügyfélfiókok vásárlás utáni kezeléséhez:

- Implementálja a Microsoft értesítései gyors fogadására, áttekintésére, a válaszadásra és a válaszadásra vonatkozó folyamatot.
- Az ügyfelekkel való munka során meg kell érteniük a felhőhasználat üzleti igényeit, miközben a megfelelő monitorozási küszöbértékeket is be kell módosítaniuk. (Például havi [Azure-költségkeretet állíthat](set-an-azure-spending-budget-for-your-customers.md) be a Partnerközpont. Ez lehetővé teszi az ügyfelek havi használatának figyelése és értesítését, ha az ügyfelek közel vannak a költségvetésükhöz.)
- Rendszeresen [figyelje az ügyfél tevékenységnaplóit,](activity-logs.md) hogy korán észlelni tudja a csalásokat.
- Gyors művelet gyanús tevékenységek észlelésekor.
- Kerülje el, hogy az ügyfelek teljes körű rendszergazdai hozzáférést adjanak az előfizetéshez anélkül, hogy kockázatcsökkentési vezérlőket kelljen bevetni.

### <a name="managing-customer-billing"></a>Ügyfélszámlázás kezelése

Javaslatok az ügyfelek számlázásának vásárlás utáni kezeléséhez:

- A kezdeti tranzakciók és számlázás előtt igényeljon előrefizetést.
- Ne fogadja el a magas kockázatú fizetési eszközöket (például előre fizetett kártyákat vagy tárolt értékkártyákat).
- Az ügyfelek kifizetéseinek és az elöregedő fiókokhoz járó igények figyelése. Agresszíven kényszeríti ki a szabványos pénzügyi folyamatokat a kései kifizetések vagy a fizetés meg nem fizetése esetén.

Az online kockázatok kezelésére vonatkozó részletesebb stratégiákért lásd az online tranzakciókockázat kezelési [útmutatóját.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
