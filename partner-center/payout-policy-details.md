---
title: Kifizetési ütemtervek és folyamatok
description: Megismeri a kifizetéseket és tranzakciókat, például a kereskedelmi piactér fizetési ütemezését és a recoupment folyamatokat és egyéb tranzakciókat.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: f2ba8132677eb0a0368021b6d7065f5202589f24
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146952"
---
# <a name="payout-schedules-and-processes"></a>Kifizetési ütemtervek és folyamatok

**Megfelelő szerepkörök:** Fiók-rendszergazdai | Globális rendszergazda

Ez a cikk a Microsoft fizetési ütemezését ismerteti, azt, hogy hol található meg a kifizetés állapota, és hogy az ügyfél hogyan nem fizet.

## <a name="payment-schedules"></a>Fizetési ütemezések

A következő szakaszok a hitelkártya Nagyvállalati Szerződés/számlatranzakciók kifizetési **folyamatát ismertetik.** 

### <a name="enterprise-agreement-transactions"></a>Nagyvállalati Szerződés tranzakciók

Amikor egy ügyfél megvásárol egy terméket a Microsoft AppSource vagy Azure Marketplace meglévő Microsoft Nagyvállalati Szerződés-fiókjával tranzakciókhoz, a következő kifizetési ciklusban, az ügyfélszámla után 30 nappal kiszámlázjuk a kifizetéseket. Az olyan tranzakciók, amelyekben az ügyfél hitelkártyát használ, a kifizetés előtt 30 napos tartási időszak áll a kezében.

A kifizetés gyakran azelőtt történik meg, hogy a Microsoft fizetési adatokat gyűjt az ügyféltől. Ha [az ügyfél nem](#process-for-customer-non-payment) fizeti ki a Microsoftot, de már kibocsátott kifizetést, a lenti Fizetés meg nem fizetése esetén az ügyfél általunk tett műveleteket lásd alább.

| Esemény | Description | Jelentés láthatósága | Időzítés* |
| --- | --- | --- | --- |
| Használat vagy a tranzakció hónapja | Az ügyfél egy szolgáltatást használ vagy vásárol. | [Használati](/azure/marketplace/partner-center-portal/usage-dashboard) vagy [rendelési](/azure/marketplace/partner-center-portal/orders-dashboard) irányítópult | **1. hónap** |
| A Microsoft kiszámítja a számlázási összeget | A teljes használat és az összes tranzakció meghatározása | [Használati](/azure/marketplace/partner-center-portal/usage-dashboard) vagy [rendelési](/azure/marketplace/partner-center-portal/orders-dashboard) irányítópult | **2. hónap** |
| Kifizetés közzétéve | Az ügynökségi díj és a kifizetési bevételek meghatározása | Feldolgozatlanként megjelölve a kifizetési kimutatás [tranzakcióelőzményében](payout-statement.md) | **3. hónap (1. hét)** |
| Kifizetés előkészítése | A bevételek elő vannak készítve a havi kifizetéshez | A kifizetési kimutatásban közelgőként van megjelölve a [tranzakcióelőzmények között](payout-statement.md) | **3. hónap (1. hét)** |
| **Elküldött kifizetések** | **A rendszer elküldi a kifizetést a közzétevőnek** | **Elküldöttként megjelölve a tranzakcióelőzmények között és a kifizetési kimutatás Kifizetések [szakaszában](payout-statement.md)** | **3. hónap (legkésőbb 15. hónap)** |
| Az ügyfél által kifizetett számla | A Microsoft fizetési adatokat gyűjt az ügyféltől | Nincs változás besorolás | **4– 12. hónap** |
|

\* A kifizetés dátuma a csendes-óceáni téli idő (PST) szerint van megszava.

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Nagyvállalati Szerződéssel kötött ügyfelek kifizetésének ütemterve.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Tranzakciók hitelkártyával vagy számlával (csekk/átutalás)

A hitelkártyával vagy havi számlával való vásárlások 30 napos tartási időszakkal garantálják, hogy az összegeket az ügyféltől gyűjtsék be.

| Esemény | Description | Jelentés láthatósága | Időzítés* |
| --- | --- | --- | --- |
| Használat vagy a tranzakció hónapja | Az ügyfél egy szolgáltatást használ vagy vásárol. | [Használati](/azure/marketplace/partner-center-portal/usage-dashboard) vagy [rendelési](/azure/marketplace/partner-center-portal/orders-dashboard) irányítópult | **1. hónap** |
| Az ügyfél által kifizetett számla | A teljes használat, a teljes tranzakciós érték és az ügyfél által fizetett számla meghatározása | [Használati](/azure/marketplace/partner-center-portal/usage-dashboard) vagy [rendelési](/azure/marketplace/partner-center-portal/orders-dashboard) irányítópult | **2. hónap** |
| Kifizetés közzétéve | Az ügynökségi díj és a kifizetési bevételek meghatározása | Feldolgozatlanként megjelölve a kifizetési kimutatás [tranzakcióelőzményében](payout-statement.md) | **2. hónap** |
| 30 napos tartási időszak | A források gyűjtésének, a lehetséges visszatérítések és a visszatérítési kérelmek igénylésének biztosítása | Feldolgozatlanként megjelölve a kifizetési kimutatás [tranzakcióelőzményében](payout-statement.md) | **3. hónap** |
| Kifizetés előkészítése | A bevételek elő vannak készítve a havi kifizetéshez | A kifizetési kimutatásban közelgőként van megjelölve a [tranzakcióelőzmények között](payout-statement.md) | **4. hónap (1. hét)** |
| **Elküldött kifizetések** | **A rendszer elküldi a kifizetést a közzétevőnek** | **Elküldveként megjelölve a tranzakcióelőzmények között és a kifizetési kimutatás Kifizetések [szakaszában](payout-statement.md)** | **4. hónap (nem később, mint 15.)** |
|

\* A kifizetés dátuma a csendes-óceáni téli idő (PST) szerint van meg.

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="A hitelkártya- és számlázási ügyfelek kifizetésének idővonala.":::

## <a name="process-for-customer-non-payment"></a>Az ügyfél meg nem fizetésének folyamata

Ritka esetekben a Microsoft nem tud fizetéseket gyűjteni az ügyfelektől a kereskedelmi piactéren történő vásárlásokért. Ha egy ügyfél nem fizet a Microsoftnak a számlázási ütemezés szerint, megkezdjük a gyűjtési folyamatot. Ez a folyamat körülbelül négy hónapot vesz igénybe, és a Microsoft állandó kommunikációját is magában foglalja. Ha a folyamat végéig nem érkezik kifizetés, a Microsoft nem feldolgozhatóként írja le az összeget.

Az itt említett kifizetési folyamat szerint előfordulhat, hogy a Microsoft már kifizette az összeget olyan közzétevőknek (Ön), amelyek végső soron nemcolhatóak. Ezért van egy eljárásunk az összegek egyeztetésének folyamatára. Annak érdekében, hogy figyelmeztetést kap arról, hogy a (már kapott) kifizetése egyeztetve lehet, értesítést kap, ha egy ügyfél a gyűjteményi folyamatban van, és a vásárlások várhatóan le lesznek írva.

A Microsoft az alábbi módszerek egyikével újra beveszi a már kifizetett kifizetéseket: (1) A Microsoft kivonhatja a ki nem fizetett összegeket a jövőbeli kifizetésekből; Ha például a kifizetésekben szereplő 1000 USD nemoszloposnak és leírhatónak minősül, a jövőbeli kifizetéseket a rendszer mindaddig visszatartja, amíg az 1000 USD-t helyre nem állják, vagy (2) a Microsoft visszatérítést vagy számla-közzétevőket kérhet a nem be nem emelt összegekért.

Az alábbi ütemezés erre mutat példát:

| Esemény | Hozzávetőleges dátum* | Partnerek láthatósága |
| --- | --- | --- |
| Példa kifizetési dátumra | 10/15/2020 | Elküldöttként **megjelölve a** Tranzakcióelőzmények és a Kifizetések szakaszban a Kifizetési irányítópulton |
| <font color="red">Ha az ügyfél nem fizet a Microsoftnak</font> | 12/2/2020 – 12/5/2020 | Nincs változás, ugyanaz, mint fent |
| Az ügyfél megkapja az első kései fizetési e-mailt | 12/6/2020 | None |
| Az ügyfél rendszeres e-maileket kap a sürgősség növeléséről | 12/7/2020 – 1/31/2021 | None |
| A közzétevő valószínűleg értesítést kap a kiírásról | 1/7/2021 | A közzétevőnek küldött e-mail-értesítés arról, hogy az ügyfél még nem küldte el a kifizetést. A tranzakcióazonosítót és a dollárban fizetendő összeget tartalmazza. |
| Az ügyfél felmondási értesítést kap | 2/1/2021 | None |
| A gyűjtési folyamat véget ér/ az összeget leírják | 2/15/2021 | A közzétevőnek küldött e-mail-értesítés arról, hogy az összeget leírták. A tranzakcióazonosítót és a dollárban fizetendő összeget tartalmazza. |
| A kifizetés le van vonva | 2021. 03. 01. | A közzétevő negatív tranzakciót fog látni a Partnerközpont kimutatásban |
| Kifizetés visszatartva | 3/15/2021 | A jövőbeli kifizetések a kifizetési kimutatásban Partnerközpont jelennek meg. A közzétevő csak akkor kapja meg a kifizetést, ha az egyenleg már nem negatív.  |
|||

\* A kifizetés dátuma a csendes-óceáni téli idő (PST) szerint van meg.

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>A kifizetési számla eléréséhez való kifizetések napjainak száma

Általában a hónap 15. napján, egy adott hónapban esedékes kifizetéseket küldjük el, de a kifizetésnek más időbe telik, hogy elérje a fiókját. A napok száma a fiókjához használt fizetési módtól függ, az alábbiakban leírtak szerint.

> [!NOTE]
> Az alábbi napok száma hozzávetőleges; bármely kifizetés több vagy kevesebb időt is vegyen el a fiókjához való eléréshez.

| Payment Method (Fizetési mód)     | A kifizetési számla eléréséhez napjainak száma     |
|--------------------|--------------------------------------------|
| PayPal             | 1 üzleti nap                             |
| ACH/SEPA           | 2–3 munkanap                          |
| Átutalás      | 7–10 munkanap                         |
|

## <a name="next-steps"></a>Következő lépések

- [Adó részletei](tax-details-marketplace.md)
