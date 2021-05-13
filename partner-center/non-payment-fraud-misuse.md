---
title: Fizetéselmaradás, csalás vagy visszaélés kezelése
description: Megismerheti az online tranzakciókban szerepet vevő különböző kockázatokat, valamint az online tranzakciók kockázatainak kezeléséhez és enyhítéséhez ajánlott Partnerközpont.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 1d8e59ea2d2e8d40163ea06b305845c37a356f16
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818660"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Fizetés elmaradása, csalás vagy visszaélés a Partnerközpontban

**A következőkre vonatkozik:** Partnerközpont | Partnerközpont a Microsoft Cloud for US Government

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Rendszergazdai ügynök | Számlázási rendszergazda

Pénzügyi felelős azért, hogy az ügyfelek csalárd vásárlásokat vásárolnak, és/vagy az ügyfelek nem fizetik ki a megvásárolt szolgáltatásokat. Ezért határozottan javasoljuk, hogy helyezzen el csalás elleni megelőzési és *észlelési kockázatcsökkentő intézkedéseket.*

A rosszindulatú tevékenység vagy visszaélés elkerülése és/vagy kezelése érdekében fontos a lehetséges kockázatok felismerése, valamint a kitettséget csökkentő szabályzatok és gyakorlatok kidolgozása.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>A Microsoft elfogadható használatra vonatkozó szabályzatának érvényesítése

Ha a Microsoft olyan partneri vagy ügyféltevékenységet észlel, amelyről meggyőződtünk, vagy azt gyanítjuk, hogy megsérti az elfogadható használatra vonatkozó szabályzatot, végre kell léptetjük a kényszerítési lépéseket. Az ügyfél azonnal felfüggeszthető. A Microsoft értesítést kap a kényszerítési műveletekről, vagy frissíti az Ön kérését.

## <a name="abuse-of-service-risks"></a>Szolgáltatási kockázatokkal való visszaélés

**A szolgáltatási kockázatokkal** való visszaélés olyan ügyfeleket jelent, akik a Microsoft elfogadható használatra vonatkozó szabályzatát megsértve használják a felhőszolgáltatásokat.

### <a name="examples-of-abuse-of-service"></a>Példák szolgáltatásokkal való visszaélésre

Példák a Microsoft elfogadható használatra vonatkozó szabályzatának megsértésére:

- Spam
- Hacker
- Elosztott szolgáltatásmegtagadásos (DDoS-) támadások
- Bitcoinbányászat
- Kártevők terjesztése
- Előfizetések újraértékesítése

## <a name="theft-of-service-risks"></a>Szolgáltatáslopási kockázatok

**A szolgáltatás ellopása olyan** ügyfeleket jelent, akiknek nem áll szándékában fizetni a felhasznált szolgáltatásokért. Ez a lopás magában foglalhatja az ellopott fizetési eszközök használatának, a hamis számlázási adatok biztosításának és/vagy a tartozások alapértelmezés szerinti beállításának esetét.

### <a name="examples-of-service-theft"></a>Példák a szolgáltatáslopásra

Ilyen online tranzakciós kockázatok például a következők lehetnek:

- Nem személyesen előforduló tranzakciók ("hitelkártya nem jelen" tranzakciók)
- Helytelenül jelenált identitások
- A kezdeti fizetés előtt kiépített és használt szolgáltatások
- Új piacok és/vagy magas kockázatú régiók online csalás esetén
- Fiók létrehozásának és megvásárlásának automatizálása rossz ak szereplőkkel

## <a name="managing-online-risk"></a>Online kockázatok kezelése

Az alábbi javaslatok segítségével olyan szabályzatokat és eljárásokat fejleszthet, amelyek csökkentik az online tranzakciós kockázatoknak való kitettséget az ügyfélkapcsolatok életciklusában.

### <a name="onboarding-new-customers"></a>Új ügyfelek létrehozása

Javaslatok az új ügyfelek online kockázatainak csökkentésére:

- Ha lehetséges, személyes kapcsolatot létesíthet az ügyfelekkel (például telefonon kapcsolatba léphet az ügyfelekkel).
- Az ügyfelek hitelesítő adatainak és hátterének ellenőrzése jobb módszerekkel (például hitelirodák vagy üzleti kereskedelmi jelentésekkel rendelkező ügynökségek használatával).
- A regisztráció során többtényezős hitelesítést (például SMS-hitelesítést) használhat a robotfiókok létrehozásának és megvásárlásának minimálisra csökkentése érdekében.
- Identitások kezelése és nyomon követése szolgáltatások (például digitális identitásszolgáltatások) használatával.
- Az ügyfelek pénzügyi erősségét szigorú bankkártya-csalásészlelési rendszerekkel mérheti fel.
- Hozzon létre egy egyértelmű gyűjtemény-szabályzatot. Részletezi a gyűjtemények folyamatát, és hogy mikor lesz hatással az előfizetések elérésére a fizetés meg nem fizetése. (Letilthatja a hozzáférést, vagy [felfüggesztheti az](create-a-new-subscription.md#suspend-a-subscription) ügyfél előfizetését fizetés nélküli fizetés esetén.)

### <a name="managing-customer-accounts"></a>Ügyfélfiókok kezelése

Javaslatok az ügyfélfiókok vásárlás utáni kezeléséhez:

- Olyan folyamat megvalósítása, amely gyorsan fogadja, áttekinti, reagál a Microsoft értesítéseire, és válaszol rá.
- Az ügyfelekkel való munka során meg kell érteniük a felhőhasználat üzleti igényeit, miközben a megfelelő monitorozási küszöbértékeket is meg kell tenniük. (Például havi Azure-költségkeretet állíthat be [a](set-an-azure-spending-budget-for-your-customers.md) Partnerközpont. Ez lehetővé teszi az ügyfelek havi használatának figyelét, és értesítést ad, ha az ügyfelek közel vannak a költségvetésükhöz.)
- Az [ügyfél tevékenységnaplóit rendszeresen](activity-logs.md) monitorozva korán észlelheti a csalásokat.
- Gyors művelet gyanús tevékenységek észlelésekor.
- Kerülje, hogy az ügyfelek teljes körű rendszergazdai hozzáférést adjanak az előfizetéshez a kockázatcsökkentési intézkedések első megvalósítása nélkül.

### <a name="managing-customer-billing"></a>Ügyfélszámlázás kezelése

Javaslatok az ügyfelek számlázásának vásárlás utáni kezeléséhez:

- Előrefizetést kérhet a kezdeti tranzakciók és a számlázás előtt.
- Ne fogadja el a magas kockázatú fizetési eszközöket (például előre fizetett kártyákat vagy tárolt értékkártyákat).
- Az ügyfelek kifizetéseinek és az elöregedő számlakövetelések figyelése. Szabványosított mellőzőfolyamatok agresszív kényszerítését a kései kifizetések vagy a fizetés meg nem fizetése esetén.

Az online kockázatok kezelésére vonatkozó részletesebb stratégiákért tekintse meg az Online tranzakciós kockázatkezelési [útmutatót.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
