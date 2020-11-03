---
title: Nem fizetés, csalás vagy visszaélés kezelése
description: Ismerje meg az online tranzakciók során felmerülő kockázatokat, valamint a kockázatok kezelésével és enyhítésével kapcsolatos ajánlott eljárásokat a partner Centerben.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 43a35f91be9ce656157065a3d19b3643ddeff68a
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528478"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Fizetés elmaradása, csalás vagy visszaélés a Partnerközpontban

A következőkre vonatkozik:

- Partnerközpont
- Az USA kormányzati szerveinek Microsoft Cloud a partneri központ

**Megfelelő szerepkörök**
- Globális rendszergazda
- Felhasználói rendszergazda
- Felügyeleti ügynök
- Számlázási adminisztrátor

Ön pénzügyi felelőssége, hogy az ügyfelek és/vagy a megvásárolt szolgáltatások nem fizetik ki az ügyfeleit. Ezért javasoljuk, *hogy a csalások megelőzésére és észlelésére vonatkozó kockázatkezelési vezérlőket helyezzen üzembe* .

A csalárd tevékenységek és a visszaélések elkerülése és/vagy elhárítása érdekében fontos megérteni a lehetséges kockázatokat, valamint olyan házirendeket és gyakorlatokat, amelyek csökkenthetik a kitettséget.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>A Microsoft elfogadható használati szabályzatának kényszerítése

Ha a Microsoft észleli, hogy az Ön által megerősített vagy gyanús partner vagy ügyfél tevékenysége megsérti az elfogadható használati szabályzatot, a rendszer végrehajtja a kényszerítési lépéseket. Az ügyfelet azonnal fel lehet függeszteni. A rendszer értesítést küld a kényszerítési műveletekről, vagy frissíti a Microsoft kérelmeit.

## <a name="abuse-of-service-risks"></a>A szolgáltatás kockázataival való visszaélés

A szolgáltatás kockázataival **való visszaélés** azt jelenti, hogy a Microsoft az elfogadható használati szabályzat megsértése miatt a Cloud Services szolgáltatást használja.

### <a name="examples-of-abuse-of-service"></a>Példák a szolgáltatással való visszaélésre

A Microsoft elfogadható használati szabályzatának ilyen megsértései például a következők lehetnek:

- Spam
- Hacking
- Elosztott szolgáltatásmegtagadási (DDoS) támadások
- Bitcoin-bányászat
- Kártevők eloszlása
- A kalóz előfizetések viszonteladása

## <a name="theft-of-service-risks"></a>A szolgáltatási kockázatok ellopása

**A szolgáltatási kockázatok ellopása** azt jelenti, hogy a fogyasztóknak nem kell fizetniük a felhasznált szolgáltatásokért. Ez a lopás a lopott fizetési instrumentumok használatát, a téves számlázási adatok biztosítását és/vagy a fennmaradó egyenlegek alapértelmezett beállítását is magában foglalja.

### <a name="examples-of-service-theft"></a>Példák a szolgáltatások ellopására

Ilyen online tranzakciós kockázatok például a következők lehetnek:

- A személyesen nem előforduló tranzakciók ("hitelkártya nem jelen" tranzakciók)
- Tévesen használt identitások
- A kezdeti fizetés fogadása előtt kiépített és használt szolgáltatások
- Feltörekvő piacok és/vagy magas kockázatú régiók online csalások esetén
- A fiókok létrehozásának és a hibás szereplők általi vásárlásának automatizálása

## <a name="managing-online-risk"></a>Online kockázat kezelése

A következő javaslatok segítségével kifejlesztheti a szabályzatokat és a gyakorlatokat, hogy csökkentse az online tranzakciós kockázatokat az ügyfélkapcsolatok életciklusa során.

### <a name="onboarding-new-customers"></a>Új ügyfelek bevezetése

Az új ügyfelek bevezetéséhez szükséges online veszélyforrások csökkentésére vonatkozó javaslatok a következők:

- Hozzon létre személyes kapcsolatot az ügyfelekkel, ha lehetséges (például telefonos kapcsolatfelvételsel).
- Ellenőrizze az ügyfelek hitelesítő adatait és hátterét a jobb módszerekkel (például a Credit Bureaus vagy az üzleti kereskedelmi jelentéskészítő ügynökségek használatával).
- A többtényezős hitelesítés (például SMS-ellenőrzés) használata a regisztráció során a Robotos fiókok létrehozásával és megvásárlásával kapcsolatos kockázat csökkentése érdekében.
- Az identitások kezelése és nyomon követése szolgáltatásokkal (például a digitális Identity Services használatával).
- Mérje fel az ügyfelek pénzügyi erejét szigorú hitelkártya-csalások észlelési rendszerein keresztül.
- Hozzon létre egy Clear Collections-szabályzatot. Részletesen ismerteti a gyűjtemények folyamatát, és az előfizetések hozzáférését nem kell kifizetni. (Letilthatja a hozzáférést, vagy [felfüggesztheti az ügyfél előfizetéseit](create-a-new-subscription.md#suspend-a-subscription) a nem fizetéshez.)

### <a name="managing-customer-accounts"></a>Ügyfélfiókok kezelése

A vásárlói fiókok a vásárlás utáni kezelésével kapcsolatos javaslatok a következők:

- Hozzon létre egy folyamatot a Microsoft értesítéseinek gyors fogadásához, felülvizsgálatához, kezeléséhez és megválaszolásához.
- Az ügyfelekkel együttműködve megismerheti a Felhőbeli használat üzleti igényeit a beállítások megfelelő figyelési küszöbértékei mellett. (Beállíthat például [egy havi Azure-költségkeretet](set-an-azure-spending-budget-for-your-customers.md) a partner Centerben. Ez a megértés lehetővé teszi az ügyfelek használatának figyelését a hónap során, és értesítést kap, ha az ügyfelek a költségvetésük közeledik.)
- A csalások korai észlelése érdekében rendszeresen figyelje az [ügyfelek tevékenységének naplóit](activity-logs.md) .
- A rendszer a gyanús tevékenységek észlelésekor gyors műveletet végez.
- Ne adja meg az ügyfeleknek teljes körű rendszergazdai hozzáférést az előfizetésekhez a kockázatkezelési vezérlők első alkalmazása nélkül.

### <a name="managing-customer-billing"></a>Ügyfél-számlázás kezelése

A vásárlói számlázás utáni kezelési javaslatok a következők:

- Előzetes befizetések igénylése a kezdeti tranzakciók és a számlázás előtt.
- Ne fogadjon el magas kockázatú fizetési eszközöket (például előre fizetett kártyákat vagy tárolt értékű kártyákat).
- Figyelheti az ügyfelek kifizetéseit és az elöregedő fiókok követeléseit. A késedelmes befizetések és a nem fizetések esetében agresszíven érvényesítheti a szabványosított Dunning-folyamatokat.

Az online kockázat mérséklésével kapcsolatos részletesebb stratégiákat az [online tranzakciós kockázatkezelési útmutatóban találja.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
