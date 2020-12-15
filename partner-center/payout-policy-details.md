---
title: Kifizetési ütemtervek és folyamatok
description: Ismerje meg a kifizetéseket és tranzakciókat, például a kereskedelmi piactér és egyéb tranzakciók fizetési ütemterveit és újrakapcsolási folyamatait.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 11/25/2020
ms.openlocfilehash: bb7a6673d2dee5a35f1c5be96f354451633eecf5
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492670"
---
# <a name="payout-schedules-and-processes"></a>Kifizetési ütemtervek és folyamatok

**Megfelelő szerepkörök:**

- Fiókadminisztrátor
- Globális rendszergazda

Ez a cikk a Microsoft fizetési ütemtervét tárgyalja, ahol megkeresheti a kifizetés állapotát, és az ügyfél nem teljesített fizetési folyamatát.

## <a name="payment-schedules"></a>Fizetési ütemtervek

A következő szakaszok ismertetik a **nagyvállalati szerződés** és a **bankkártya/számlázási** tranzakciók kifizetési folyamatát.

### <a name="enterprise-agreement-transactions"></a>Tranzakciók Nagyvállalati Szerződés

Ha egy ügyfél Microsoft AppSource vagy az Azure Marketplace-en vásárol egy terméket a meglévő Microsoft-Nagyvállalati Szerződés a tranzakciós szolgáltatásban, akkor a következő kifizetési ciklusban kiállítjuk a kifizetéseket a számlázás utáni 30 napban. Azok a tranzakciók, amelyekben az ügyfél hitelkártyát használ, a kifizetés előtt 30 napos időszakot tart fenn.

A Microsoft a kifizetés megkezdése előtt gyakran fordul elő. Ha az ügyfél nem fizet a Microsoftnak, de már kiállítottunk egy kifizetést, tekintse meg az [ügyfél nem fizetési folyamatát](#process-for-customer-non-payment) ismertető szakaszt.

| Esemény | Description | Jelentéskészítés láthatósága | Időzítés |
| --- | --- | --- | --- |
| A tranzakció használata vagy hónapja | Az ügyfél egy szolgáltatást használ vagy vásárol. | [Használati](/azure/marketplace/partner-center-portal/usage-dashboard) vagy [rendelési](/azure/marketplace/partner-center-portal/orders-dashboard) irányítópult | **1. hónap** |
| A Microsoft kiszámítja a számlázási összeget | Teljes használat meghatározása, tranzakciók összesen | [Használati](/azure/marketplace/partner-center-portal/usage-dashboard) vagy [rendelési](/azure/marketplace/partner-center-portal/orders-dashboard) irányítópult | **2. hónap** |
| Kifizetés közzétéve | Az ügynökségi díj és a kifizetés eredményének meghatározása | A [kifizetési utasításban](payout-statement.md) feldolgozatlan van megjelölve a tranzakciós előzményekben | **3. hónap (1. hét)** |
| Kifizetés előkészítése | A bevétel felkészült a havi fizetésre | A [kifizetési utasításban](payout-statement.md) a tranzakciós előzményekben közelgőként van megjelölve | **3. hónap (1. hét)** |
| **Kifizetés elküldése** | **A rendszer elküldi a fizetést a közzétevőnek** | **Elküldve a tranzakció előzményeiben és a [kifizetési nyilatkozat](payout-statement.md) fizetési szakaszában** | **3. hónap (nem később, mint a 15.)** |
| Az ügyfél által fizetett számla | A Microsoft fizetési lehetőséget gyűjt az ügyféltől | Nincs változás besorolás | **4. hónap – 12** |
|

\* A kifizetés dátuma csendes-óceáni téli idő (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Nagyvállalati szerződéssel rendelkező ügyfelek fizetési ütemezése.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Bankkártyával vagy számlával rendelkező tranzakciók (ellenőrzések/huzalok)

Az összes bankkártyával vagy havi számlával történő vásárlás 30 napos időszakot biztosít, amely biztosítja, hogy az ügyfelek az ügyféltől gyűjtsék a forrásokat.

| Esemény | Description | Jelentéskészítés láthatósága | Időzítés |
| --- | --- | --- | --- |
| A tranzakció használata vagy hónapja | Az ügyfél egy szolgáltatást használ vagy vásárol. | [Használati](/azure/marketplace/partner-center-portal/usage-dashboard) vagy [rendelési](/azure/marketplace/partner-center-portal/orders-dashboard) irányítópult | **1. hónap** |
| Az ügyfél által fizetett számla | A teljes használat, a tranzakció teljes értéke és az ügyfél által fizetett számla meghatározása | [Használati](/azure/marketplace/partner-center-portal/usage-dashboard) vagy [rendelési](/azure/marketplace/partner-center-portal/orders-dashboard) irányítópult | **2. hónap** |
| Kifizetés közzétéve | Az ügynökségi díj és a kifizetés eredményének meghatározása | A [kifizetési utasításban](payout-statement.md) feldolgozatlan van megjelölve a tranzakciós előzményekben | **2. hónap** |
| 30 napos időszak | Az alapok, a lehetséges jóváírások és a visszatérítési kérelmek gyűjtésének biztosítása | A [kifizetési utasításban](payout-statement.md) feldolgozatlan van megjelölve a tranzakciós előzményekben | **3. hónap** |
| Kifizetés előkészítése | A bevétel felkészült a havi fizetésre | A [kifizetési utasításban](payout-statement.md) a tranzakciós előzményekben közelgőként van megjelölve | **4. hónap (1. hét)** |
| **Kifizetés elküldése** | **A rendszer elküldi a fizetést a közzétevőnek** | **Elküldve a tranzakció előzményeiben és a [kifizetési nyilatkozat](payout-statement.md) fizetési szakaszában** | **4. hónap (nem később, mint a 15.)** |
|

\* A kifizetés dátuma csendes-óceáni téli idő (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="A hitelkártyára és a számla-ügyfelekre vonatkozó kifizetések ütemezése.":::

## <a name="process-for-customer-non-payment"></a>Az ügyfél nem teljesített fizetési folyamata

Ritkán fordul elő, hogy a Microsoft nem tud befizetni az ügyfelektől a kereskedelmi Marketplace-vásárlásokhoz. Amikor egy ügyfél a számlázási ütemterv szerint nem fizet a Microsoftnak, kezdjük a gyűjtemények folyamatát. Ez a folyamat körülbelül négy hónapot vesz igénybe, és a Microsoft állandó kommunikációját is magában foglalja. Ha a folyamat végén nem érkezik fizetés, a Microsoft a nem begyűjthető módon írja le az alapokat.

Az itt megfogalmazott kifizetési folyamat alapján a Microsoft már kifizette a forrásokat olyan közzétevőknek (Ön), amelyek végső soron nem gyűjthetők. Ezért az ilyen összegek összeegyeztetése folyamatban van. Annak ellenőrzéséhez, hogy a (már fogadott) fizetést egyeztetni lehet-e, értesítést kap, ha az ügyfél a gyűjtemények folyamatában van, és a vásárlások valószínűleg ki lesznek írva.

A Microsoft a következő módszerek egyikének használatával visszakapcsolja az Ön számára már kifizetett kifizetéseket: (1) a Microsoft kivonja a jövőbeli kifizetésekből kifizetett összegeket. Ha például a kifizetések $1 000-es értéke nem gyűjthető és nem írható, a jövőbeli kifizetések visszatartásra kerülnek, amíg a $1 000 vissza nem áll, vagy (2) a Microsoft visszatérítési vagy számlázási közzétevőket igényelhet a nem gyűjtött összegekért.

A következő példa egy ütemezett ütemtervet mutat be:

| Esemény | Hozzávetőleges dátum * | Partner láthatósága |
| --- | --- | --- |
| Példa a kifizetés dátumára | 10/15/2020 | A kifizetési **irányítópulton a** tranzakciós előzmények és a fizetések részben ellátottként van megjelölve |
| <font color="red">Ha az ügyfél nem fizet a Microsoftnak</font> | 12/2/2020 – 12/5/2020 | Nincs változás, ugyanaz, mint fent |
| Az ügyfél megkapja az első késedelmes fizetési értesítő e-mailt | 12/6/2020 | Nincsenek |
| Az ügyfél rendszeresen kap e-maileket a megnövekedett sürgősségről | 12/7/2020 – 1/31/2021 | Nincsenek |
| Valószínűleg a közzétevő értesítést kap a kiírásról | 1/7/2021 | A közzétevőnek küldött e-mail-értesítés, amelyet az ügyfele még nem küldött el. A tranzakció-azonosító és a dollár összege is szerepel. |
| Az ügyfél lemondási értesítést kap | 2/1/2021 | Nincsenek |
| A gyűjtési folyamat vége/az alapok le vannak írva | 2/15/2021 | A közzétevőnek elküldött e-mail-értesítés, amelyből a rendszer kiírta a forrásokat. A tranzakció-azonosító és a dollár összege is szerepel. |
| A kifizetés le van vonva | 2021. 03. 01. | A közzétevő negatív tranzakciót fog látni a partner Center kifizetési utasításban |
| A kifizetés megtagadva | 3/15/2021 | A jövőbeli kifizetések a partner Center kifizetési nyilatkozatában jelennek meg. A közzétevő nem kap fizetést, amíg az egyenleg már nem negatív.  |
|||

\* A kifizetés dátuma csendes-óceáni téli idő (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>A kifizetési fiókhoz való befizetéshez szükséges napok száma

A hónap 15. napján egy adott hónapban minden esedékes fizetést elküldünk, de további időt vesz igénybe, hogy a fizetés elérje a fiókját. A napok száma a fiókhoz használt fizetési módszertől függ, az alább leírtak szerint.

> [!NOTE]
> Az alább látható napok a következők: közelítő; a fizetés több vagy kevesebb időt vehet igénybe a fiókja eléréséhez.

| Payment Method (Fizetési mód)     | A kifizetési fiók eléréséhez szükséges napok száma     |
|--------------------|--------------------------------------------|
| PayPal             | 1 munkanap                             |
| ACH/SEPA           | 2-3 munkanap                          |
| Átutalás      | 7-10 munkanap                         |
|

## <a name="next-steps"></a>Következő lépések

- [Adó részletei](tax-details-marketplace.md)
