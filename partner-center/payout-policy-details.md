---
title: Kifizetési szabályzat részletei – Microsoft kereskedelmi piactér
description: Ismerje meg a kereskedelmi Piactéri kifizetési szabályzatokkal kapcsolatos részleteket, beleértve az ütemterveket és a visszakapcsolást.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: mingshen-ms
ms.author: mingshen
ms.date: 09/28/2020
ms.openlocfilehash: eec5f85f38280757bc1e5d5c36a4dd1ac5ce8d22
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530480"
---
# <a name="payout-policy-details"></a>Fizetési szabályzat részletei

Ez a cikk a Microsoft kifizetési folyamatát, a kifizetési ütemtervet ismerteti, ahol megtalálhatja a kifizetés és a visszakapcsolási szabályzat állapotát.

## <a name="payment-schedules"></a>Fizetési ütemtervek

A következő szakaszok ismertetik a kifizetési folyamatokat.

### <a name="enterprise-agreement-transactions-after-may-1-2020"></a>Tranzakciók Nagyvállalati Szerződés május 1-től 2020

#### <a name="update-to-our-commercial-marketplace-publisher-payout-model"></a>Frissítés a kereskedelmi piactér kiadójának kifizetési modelljére

2020. május 1-től frissítjük az Azure Marketplace-en vásárolt termékekkel kapcsolatos kifizetési szabályzatot, vagy Microsoft-Nagyvállalati Szerződés AppSource ügyfeleinknek. Ha egy ügyfél az Azure Marketplace-ről vagy AppSource-ből vásárol egy terméket a meglévő Microsoft-Nagyvállalati Szerződés a 2020. május 1. után, akkor a következő kifizetési ciklusban megjelenő kifizetési ciklusban megkezdjük a kifizetések kiadását. Azok a tranzakciók, amelyekben az ügyfél hitelkártyát használ, változatlanok maradnak, és a nyereményt megelőzően 30 napos időszakot is megtartanak. Ez a táblázat a kifizetési ütemterv részleteit jeleníti meg.

> [!NOTE]
> Ha az ügyfél nem fizet, de már kiállítottunk Önnek egy kifizetést, tekintse meg az [ügyfél nem fizetési folyamatát](#process-for-customer-non-payment) alább.

| Esemény  | Dátum (UTC) | Partner láthatósága: partneri központ – kifizetési jelentés  |  Partner láthatósága: a partner Center Analytics\* |
| --- | --- | --- | --- |
| Tranzakció vagy havi használat | 8/1/2020 – 8/31/2020 | N/A | **Használati jelentés** : új felhasználás látható (négy óránként frissül)<br>**Rendelési jelentés** : N/A |
| Befejezési időszak (hónap) | 8/31/2020 | N/A | **Használati jelentés** : hónap végi felhasználás látható<br>**Rendelési jelentés** : N/A |
| Megrendelés létrehozva | 9/3/2020 – 9/7/2020 | N/A | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Kifizetési kereset kiszámítása | 9/4/2020 – 9/10/2020 | A kifizetési irányítópult tranzakciós előzményeiben **feldolgozatlan** megjelölve | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Havi kifizetés | 10/5/2020 | A kifizetési irányítópulton a tranzakciós előzményekben **közelgőként** van megjelölve | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Kifizetés dátuma\** | 10/15/2020 | A tranzakció **Sent** előzményeiben és a kifizetési irányítópult fizetések szakaszában ellátottként van megjelölve | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Vevői számla összegyűjtve | 12/1/2020 | A tranzakció **Sent** előzményeiben és a kifizetési irányítópult fizetések szakaszában ellátottként van megjelölve | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések  |
|  |  |  |  |

\* A használati és rendelési jelentések a partner Center elemzés szakaszában érhetők el. \* *. A kifizetés dátuma csendes-óceáni téli idő (PST).

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>Bankkártyát vagy számlát használó ügyfelek

Az összes bankkártyával vagy havi számlával történő vásárlás 30 napos időszakot biztosít, amely biztosítja, hogy a rendszer kiürítse az alapokat, és nincsenek jóváírások vagy csalás gyanúja.

| Esemény  | Dátum (UTC) | Partner láthatósága: partneri központ – kifizetési jelentés  |  Partner láthatósága: a partner Center Analytics\*  |
| --- | --- | --- | --- |
| Tranzakció vagy havi használat | 8/1/2019 - 8/31/2019 | N/A | **Használati jelentés** : új felhasználás látható (négy óránként frissül)<br>**Rendelési jelentés** : N/A |
| Befejezési időszak (hónap) | 8/31/2019 | N/A | **Használati jelentés** : hónap végi felhasználás látható<br>**Rendelési jelentés** : N/A |
| Megrendelés létrehozva | 9/3/2019 – 9/7/2019 | N/A | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Vevői számla összegyűjtve | 9/7/2019 – 9/10/2019 | N/A | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Kifizetés kiszámítása | 9/8/2019 -9/12/2019 | A kifizetési irányítópult tranzakciós előzményeiben **feldolgozatlan** megjelölve | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Havi kifizetés | 11/5/2019\* | A kifizetési irányítópulton a tranzakciós előzményekben **közelgőként** megjelölve | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Kifizetés dátuma\** | 11/15/2019 | A tranzakció előzményeiben és a kifizetési irányítópult fizetések szakaszában **eljuttatott** jelöléssel ellátottként van megjelölve | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
|  |  |  |  |

\* A használati és rendelési jelentések a partner Center elemzés szakaszában érhetők el.</br>\** A kifizetés dátuma csendes-óceáni téli idő (PST).

### <a name="enterprise-agreement-transactions-prior-to-may-1-2020"></a>A tranzakciók Nagyvállalati Szerződés május 1. előtt, 2020

Az ezen dátum előtt bekövetkezett összes vásárlás feldolgozása és kifizetése az alábbi ütemterv szerint történik, miután a Microsoft begyűjtötte az ügyfelektől érkező fizetést, és feldolgozta a piactér díját.

| Esemény  | Dátum (UTC)  | Partner láthatósága: partneri központ – kifizetési jelentés  |  Partner láthatósága: a partner Center Analytics\*  |
| --- | --- | --- | --- |
| Tranzakció vagy havi használat | 8/1/2019 – 8/31/2019 | N/A | **Használati jelentés** : új felhasználás látható (négy óránként frissül)<br>**Rendelési jelentés** : N/A |
| Befejezési időszak (hónap) | 8/31/2019 | N/A | **Használati jelentés** : hónap végi felhasználás látható<br>**Rendelési jelentés** : N/A |
| Megrendelés létrehozva | 9/3/2019 – 9/7/2019 | N/A | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Vevői számla összegyűjtve | 12/1/2019 | N/A | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Kifizetés kiszámítása | 12/5/2019 – 12/7/2019 | A kifizetési irányítópult tranzakciós előzményeiben **feldolgozatlan** megjelölve | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Havi kifizetés | 1/5/2019 | A kifizetési irányítópulton a tranzakciós előzményekben **közelgőként** megjelölve | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
| Kifizetés dátuma\** | 1/15/2019 | **A tranzakció** előzményeiben és a kifizetési irányítópult fizetések szakaszában ellátottként megjelölt | **Használati jelentés** : a Rendeléskód/OrderLineItemID által megjelenített felhasználás<br>**Rendelési jelentés** : aktívként megjelenített Vevői megrendelések |
|  |  |  |  |

\* A használati és rendelési jelentések a partner Center elemzés szakaszában érhetők el.</br>\** A kifizetés dátuma csendes-óceáni téli idő (PST).

## <a name="process-for-customer-non-payment"></a>Az ügyfél nem teljesített fizetési folyamata

Ritkán fordul elő, hogy a Microsoft nem tud befizetni az ügyfelektől a kereskedelmi Marketplace-vásárlásokhoz. Amikor egy ügyfél a számlázási ütemterv szerint nem fizet a Microsoftnak, kezdjük a gyűjtemények folyamatát. Ez a folyamat körülbelül négy hónapot vesz igénybe, és a Microsoft állandó kommunikációját is magában foglalja. Ha a folyamat végén nem érkezik fizetés, a Microsoft a nem begyűjthető módon írja le az alapokat.

Az itt megfogalmazott kifizetési folyamat alapján a Microsoft már kifizette a forrásokat olyan közzétevőknek (Ön), amelyek végső soron nem gyűjthetők. Ezért az ilyen összegek összeegyeztetése folyamatban van. Annak ellenőrzéséhez, hogy a (már fogadott) fizetést egyeztetni lehet-e, értesítést kap, ha az ügyfél a gyűjtemények folyamatában van, és a vásárlások valószínűleg ki lesznek írva.

A Microsoft a következő módszerek egyikének használatával visszakapcsolja az Ön számára már kifizetett kifizetéseket: (1) a Microsoft kivonja a jövőbeli kifizetésekből kifizetett összegeket. Ha például a kifizetések $1 000-es értéke nem gyűjthető és nem írható, a jövőbeli kifizetések visszatartásra kerülnek, amíg a $1 000 vissza nem áll, vagy (2) a Microsoft visszatérítési vagy számlázási közzétevőket igényelhet a nem gyűjtött összegekért.

A következő példa egy ütemezett ütemtervet mutat be:

| Esemény | Hozzávetőleges dátum | Partner láthatósága |
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

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>A kifizetési fiókhoz való befizetéshez szükséges napok száma

A hónap 15. napján egy adott hónapban minden esedékes fizetést elküldünk, de további időt vesz igénybe, hogy a fizetés elérje a fiókját. A napok száma a fiókhoz használt fizetési módszertől függ, az alább leírtak szerint.

> [!NOTE]
> Az alább látható napok a következők: közelítő; a fizetés hosszabb vagy rövidebb időt is igénybe vehet a fiókja eléréséhez.

| Payment Method (Fizetési mód)     | A kifizetési fiók eléréséhez szükséges napok száma     |
|--------------------|--------------------------------------------|
| PayPal             | 1 munkanap                             |
| ACH/SEPA           | 2-3 munkanap                          |
| Átutalás      | 7-10 munkanap                         |
|

## <a name="next-steps"></a>Következő lépések

- [Adó részletei](tax-details-marketplace.md)
