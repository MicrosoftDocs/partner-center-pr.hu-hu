---
title: Kifizetési utasítások
description: Ismerje meg a kifizetési kimutatásokat és összegzéseket, valamint a fizetési adatok Microsoft-fiókból való megtekintésének és exportálásának Partnerközpont
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: 4e9ab721fe356dbcdff7316a5ed5b52c81f2d4eb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152596"
---
# <a name="payout-statements"></a>Kifizetési utasítások

**Megfelelő szerepkörök:** Fiók-rendszergazdai | Globális rendszergazda

A **Kifizetési kimutatás** áttekintést nyújt a kereskedelmi piactéren keresztül értékesített ajánlatok kifizetéseiről. Megjeleníti a bevételek tranzakciós előzményeit, becslést ad a következő kifizetésre, és megjeleníti a fizetési trendeket. A tranzakciós előzményeket és a fizetési kimutatásokat is letöltheti. Ez a cikk azt ismerteti, hogyan férhet hozzá a kifizetési kimutatáshoz, valamint a különböző kifizetési oldalakhoz és letöltéshez, amelyek a Partnerközpont.

>[!NOTE]
>Csak a társított MPN-adatokat és -programokat fogja látni. Ha további adatokat szeretne látni, forduljon a fiókad rendszergazdájához az engedélyekért. 

## <a name="roles-and-permissions"></a>Szerepkörök és engedélyek

Egy kifizetési kimutatás eléréséhez a Fióktulajdonos  vagy a Pénzügyi közreműködő **szerepkört kell hozzárendelni.**

| Jelentések/oldalak | Fióktulajdonos | Manager | Fejlesztő | Üzleti közreműködő | Pénzügyi közreműködő | Marketingszakértő |
| --- | --- | --- | --- | --- | --- | --- |
| Beszerzési jelentés (beleértve a közel valós idejű adatokat) | Megtekintheti | Megtekintheti | Nincs hozzáférés | Nincs hozzáférés | Megtekintheti | Nincs hozzáférés |
| Visszajelzési jelentés/válaszok | Megtekintheti és küldhet visszajelzést | Megtekintheti és küldhet visszajelzést | Megtekintheti és küldhet visszajelzést | Nincs hozzáférés | Nincs hozzáférés | Megtekintheti és küldhet visszajelzést |
| Állapotjelentés (beleértve a közel valós idejű adatokat) | Megtekintheti | Megtekintheti | Megtekintheti | Megtekintheti | Nincs hozzáférés | Nincs hozzáférés |
| Használat jelentés | Megtekintheti | Megtekintheti | Megtekintheti | Megtekintheti | Nincs hozzáférés | Nincs hozzáférés |
| Kifizetési számla | Frissíthet | Nincs hozzáférés | Nincs hozzáférés | Nincs hozzáférés | Frissíthet | Nincs hozzáférés |
| Adóprofil | Frissíthet | Nincs hozzáférés | Nincs hozzáférés | Nincs hozzáférés | Frissíthet | Nincs hozzáférés |
| Kifizetés összegzése | Megtekintheti | Nincs hozzáférés | Nincs hozzáférés | Nincs hozzáférés | Megtekintheti | Nincs hozzáférés |
|

## <a name="access-your-payout-statement"></a>Hozzáférés a kifizetési kimutatáshoz

Jelentkezzen be a [Partnerközpont,](https://partner.microsoft.com/dashboard/home) és válassza a képernyő jobb felső sarkában található kifizetés ikont a különböző összegzések eléréséhez:

- Tranzakcióelőzmények
- Kifizetések
- Adatok exportálása

:::image type="content" source="images/payouts/payout-overview.png" alt-text="A portál jobb felső sarkában található Kifizetés ikont Partnerközpont ábrázolja":::

A Partner Payout [API-val](https://apidocs.microsoft.com/services/partnerpayouts) közvetlenül is csatlakozhat a kifizetési tranzakciókhoz és a fizetési adatokhoz, és beszerezheti őket.


## <a name="transaction-history"></a>Tranzakcióelőzmények

A **Tranzakciós előzmények** oldalon megjelenik a bevételek összegzése, a becsült következő kifizetés, valamint a bevételek és kifizetések trendje az elmúlt 36 hónapra. A tranzakció részleteit ebből a szakaszból is letöltheti.<br><br>Ez a jelentés a kifizetésre jogosult összes bevételt megjeleníti, a még el nem küldött kifizetéseket is beleértve. A bevételek akkor jogosultak kifizetésre, ha egy isv az Partnerközpont összes banki és adóinformációját kitöltötte, >50 usd-t keresett, az ISV-fiók aktív, az ügyfél számlázása (NAGYvállalati tranzakciók esetén) vagy a kifizetés fogadása (nem EA-tranzakciók esetén).

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Tranzakció áttekintése.":::

- **Idei elküldött bevételek** – Az összes bevétel és a bevételek lebontása, amelyek kifizetése és kifizetése a következő hónapban várható.
- **Becsült kifizetési hónap** – Az összes várható bevétel a következő hónapokban.
- **Bevételek és kifizetési trend** – Havi bevétel és kifizetés összege az elmúlt 36 hónapra.
- **Letöltés** – Tranzakció részleteinek letöltése .csv vagy .tsv formátumban.

Az oldal jobb felső sarkában található dátumtartomány-kijelölés használatával szűrheti az oldal kimenetét az elmúlt 3, 6, 12 vagy 36 hónapra. Vagy válasszon ki egy legfeljebb 36 hónapos egyéni dátumtartományt. Az alapértelmezett dátumtartomány 12 hónap. Szűrhet a regisztrációs azonosító, a program, a fizetési azonosító, a bevétel típusa, a mozgató és az állapot alapján is. Az adatok az aktuális pénzügyi évre (július 1. – június 30.) és az azt megelőző két pénzügyi évre érhetők el.

:::image type="content" source="images/payouts/search-filter.png" alt-text="A keresési szűrő az oldal jobb felső részen található.":::

A bevételről további részleteket az oldal jobb oldalán található lefelé mutató nyílra kattintva talál. Ha így tesz, megjelenik a mozgató, a bevétel összege, a termék és az ügyfél. Ha ezek az adatok valamilyen okból nem érhetők el, de hozzáférésre van szüksége, forduljon az ügyfélszolgálathoz. Ha a bevétel egy módosítás eredménye, és nem tranzakció, akkor a Product és a Customer mezők nem jelennek meg.

### <a name="transaction-history-summary"></a>Tranzakcióelőzmények összegzése

Ez a nézet a bevétel részleteit jeleníti meg, beleértve az eladott bevételi dátumok, az állapot és a becsült kifizetési hónap bevételének forrását.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Tranzakcióelőzmények.":::

- **Megszerzett érték** – A vásárlás dátuma.
- **Bevételi típus** – A bevétel típusa, például értékesítés, értékesítés vagy együttműködés.
- **Teljes összeg** – A nettó bevétel összege. A kereskedelmi piactéren ez a standard Marketplace-díj levonása után jelent.
- **Állapot** – Három lehetőség közül választhat:
    - **Közelgő** – A bevételek hűtési időszakra vannak függőben.
    - **Feldolgozott –** A bevételek elő vannak készítve a következő kifizetésre.
    - **Elküldött** – A bevételek ki vannak fizetve.
- **Becsült kifizetési hónap** – A bevétel várható kifizetésének hónapja. További [információért tekintse meg](#estimated-payment-month) a következő szakaszt.

A bevételi tranzakciók akkor jelennek meg, ha a tranzakció megfelel a kifizetési jogosultságnak. Ha meg kell értenie, hogy miért hiányoznak vagy váratlan bevételek, tekintse meg a kereskedelmi piactéri kifizetésekre vonatkozó gyakori [kérdéseket.](payout-faq.md#why-are-my-earnings-missing)

#### <a name="estimated-payment-month"></a>Becsült fizetési hónap

A Tranzakcióelőzmények oldal mostantól tartalmaz egy táblázatot, amely a következő néhány hónap becsült kifizetésének összegét mutatja. Ezt az információt a Tranzakcióelőzmények és az Összefoglalás jelentés exportálási táblázatában is megtekintheti és letöltheti. Ezek az információk megkönnyítik az egyeztetéseket és a fizetési előrejelzéseket.

A becsült fizetési hónap számítása programkonfigurációs szabályok és ütemtervek alapján történik, és a következő/jövőbeli fizetési ciklusban lesz feldolgozva.

A becsült kifizetési hónap jelenleg az együttműködési lehetőség kivételével minden bevételi típushoz elérhető, amely **Nem alkalmazható értékként jelenik meg.** A 2020. július 1. előtti bevételek esetén a Becsült fizetési hónap Nem **érhető el értékként jelenik meg.**

Az alábbi táblázat egy becsült fizetési hónapra mutat példát.

| Month (hónap) | Összeg |
| ------ | :-----------: |
|  2020. szeptember |  7 273,99 USD   |
|  2020. október | 8 692,30 USD  |
|  Nov-2020 | 107,89 USD  |

A becsült összeg több okból is eltérhet a tényleges összegtől:

- Bevétel újraszámítása: A bevételek újraszámítása esetén a tényleges összeg eltérő lesz
- Helyesbítések: A tényleges összeg az eltért vagy elküldött módosításoktól függően változik.
- Szabályok módosítása: A szabályok módosítása tükrözheti a ténylegesen kifizetett összeg újraszámítását
- Kötelezettség: Fizetési hiba esetén a tényleges összeg eltérő lehet

Vegye figyelembe, hogy a kifizetése csak a tervezett hónapban szabadul fel, ha a program küszöbértéke és a kifizetések jogosultsági szabályai teljesülnek. Ezek a szabályok többek között az alábbi listára korlátozódnak:

- Az adóprofilnak naprakésznek kell lennie
- A bevételeknek meg kell felelnie a program útmutatójában meghatározott minimális bevételi küszöbértéknek, vagy meg kell haladni azt.
- Kifizetés visszatartva: Ha a profilok hozzárendelési oldalán a "Fizetésem visszatartva" lehetőséget választja.
- Fizetési eszköz nem érhető el: A fizetési vagy/és adóprofil nincs befejezve.

### <a name="transaction-history-download"></a>Tranzakciós előzmények letöltése

A bevételről további részleteket az **oldal** tetején található Letöltés lehetőséget választva talál. Az alábbi táblázat ismerteti a jelentés egyes oszlopát.

>[!NOTE]
>A Tranzakciós előzmények letöltési exportálása 2020 augusztusában két új mezőt tartalmaz:
>
>- **lastPaymentCurrency (lastPaymentCurrency)**  Az a pénznem, amelyben a legutóbbi fizetés érkezett az összes olyan MPN-ről, amelyhez a jelenleg bejelentkezett partner hozzáféréssel rendelkezik. Ha nem érkezik kifizetés, az utolsó fizetési pénznem amerikai dollár lesz.
>- **earningAmountInLastPaymentCurrency**  A bevétel összege az utolsó fizetési pénznemben.

| Oszlop neve | Leírás | Az ösztönzőprogramok/piacterek alkalmazhatósága |
| --- | --- | --- |
| agreementEndDate | Szerződés záró dátuma | Ösztönzők – csak néhány program |
| agreementNumber (szerződés száma) | Szerződésszám | Ösztönzők – csak néhány program |
| agreementStartDate (szerződésindításidátum) | Szerződés kezdő dátuma | Ösztönzők – csak néhány program |
| calculationDate (számításdátum) | A bevétel kiszámításának dátuma a rendszerben | Mind |
| claimId (jogcímazonosító) | Jogcím egyedi azonosítója | Ösztönzők – csak néhány program |
| customerCountry (ügyfél országa) | Ügyfél országa/régiója | Piacokon |
| customerEmail |  |  |
| customerName (ügyfél neve) | Lehet, hogy üres | Csak ösztönzőprogramok (kivétel: OEM) és piacterek. CSP-tranzakciók esetén a piacterek a CSP nevét fogják mutatni |
| customerTenantId (customerTenantId) |  |  |
| distributorId (terjesztőazonosító) | Terjesztő azonosítója | Ösztönzők – csak néhány program |
| distributorName (forgalmazó neve) | Terjesztő neve | Ösztönzők – csak néhány program |
| earningAmount | Bevételi összeg az eredeti tranzakció pénznemében | Mind |
| earningAmountInLastPaymentCurrency | Bevételi összeg az utolsó fizetési pénznemben (a mező üres lesz, ha nem fizették ki a korábbi kifizetéseket) |  |
| earningAmountUSD | Bevétel USD-ben | Mind |
| earningDate (bevételidátum) | A bevétel dátuma | Mind |
| earningExchangeRate | A megfelelő USD összegének megjelenítése az átváltási árfolyam alapján | Mind |
| earningId (bevételazonosító) | Az egyes bevételi pontok egyedi azonosítója | Mind |
| earningRate (bevételi arány) | A bevételt generáló tranzakció összegére alkalmazott ösztönzők aránya | Mind |
| earningType (bevétel típusa) | Jelzi, hogy díjról, ingatlanról, együttműködésről, értékesítésről és így tovább | Mind |
| exchangeRateDate | A EarningAmount USD kiszámításához használt árfolyamdátum | Mind |
| externalReferenceId (externalReferenceId) | A program egyedi azonosítója | Közvetlen fizetéses programok (ösztönzők és piacterek) |
| externalReferenceIdLabel | Egyedi azonosítócímke | Közvetlen fizetéses programok (ösztönzők és piacterek) |
| instantRebateAmount |  |  |
| invoiceDate (számla dátuma) |  |  |
| invoiceNumber (számlaszám) | Számlaszám (csak nagyvállalatok esetén alkalmazható) | Ösztönzők és piacterek – csak néhány program |
| lastPaymentCurrency (lastPaymentCurrency) | Utolsó fizetési pénznem (a mező üres lesz, ha még nem fizették ki) |  |
| Kar | A bevétel üzleti szabályát jelzi | Mind |
| LicensingProgramName (Licencprogram neve) | A licencprogram neve |  |
| LineItemId (Sorazonosító) | Egyedi sor az ügyfél számlájában |  |
| localProviderSeller | Helyi szolgáltató/rekord értékesítője |  |
| Esedékesség hónapja | A becsült fizetési hónap | Mind |
| OrderId | Az ügyfél számlájához kapcsolódik  | Piacokon |
| parentProductId (parentProductId) | A szülőtermék egyedi azonosítója. Ha nincs szülőtermék a tranzakcióhoz, akkor a Szülő termék azonosítója = Termékazonosító. | Piacokon |
| parentProductName (parentProductName) | A szülőtermék neve. Ha nincs szülőtermék a tranzakcióhoz, akkor a Szülőtermék neve = Terméknév. | Piacokon |
| résztvevő-azonosító | A program keretében bevételt kapó partner elsődleges identitása | Mind |
| participantIdType (résztvevőazonosító típusa) | Többnyire az ösztönzőprogramok programazonosítója és a piacterek Értékesítői IF azonosítója | Mind |
| résztvevő neve | A bevételt kereső partner neve | Mind |
| partnerCountryCode | A bevételt kereső partner helye/országa/régiója | Mind |
| partNumber | Mindig üres lesz | Néhány ösztönzőprogram és piactér |
| paymentId (fizetésiazonosító) | Egyedi azonosító, amely a tranzakciós jelentés összes tranzakcióját egy adott kifizetéssel korrelálja a fizetési jelentésben | Mind |
| paymentStatus (kifizetésiállapot) | Fizetési állapot | Mind |
| paymentStatusDescription (kifizetési leírás) | A fizetési állapot rövid leírása | Mind |
| productId | Egyedi termékazonosító | Piacokon |
| Productname | A tranzakcióhoz csatolt terméknév | Mind |
| productType | Termék típusa, például Alkalmazás, Bővítmény vagy Játék | Piacokon |
| Programkód | A program nevével leképezni való sztring |  |
| programName | Ösztönző/áruházi program neve | Mind |
| purchaseOrderCoverageEndDate | Mindig üres lesz | Ösztönzőprogram – CRI |
| purchaseOrderCoverageStartDate | Mindig üres lesz | Ösztönzőprogram – CRI |
| purchaseOrderType | Mindig üres lesz | Ösztönzőprogram – CRI |
| purchaseTypeCode | Mindig üres lesz | Ösztönzőprogram – CRI |
| quantity | A programtól függően változik. Tranzakciós programok számlázandó mennyiségét jelzi | Mind |
| reasonCode (okkód) |  |  |
| resellerCountry |  |  |
| resellerId | Viszonteladó azonosítója | Ösztönzők – csak néhány program |
| resellerName | Viszonteladó neve |  |
| SkuId (Termékváltozatazonosító) | A közzététel során meghatározott termékváltozat-azonosító. Egy ajánlat több termékváltozattal is lehet, de egy termékváltozat csak egyetlen ajánlathoz társítható. Ösztönzők – csak néhány program |  |
| storeFee | A Microsoft által az alkalmazásnak vagy bővítménynek az Áruházban való elérhetővé tevésért fizetendő díjként megőrzhető összeg | Piacokon |
| subscriptionEndDate | Előfizetés záró dátuma | Ösztönzők – csak néhány program |
| subscriptionId | Az ügyfélhez társított előfizetés-azonosító | Ösztönzők – csak néhány program |
| subscriptionStartDate (előfizetés kezdődátuma) | Előfizetés kezdő dátuma | Ösztönzők – csak néhány program |
| taxCity (adóváros) |  |  |
| taxCountry (ország) |  |  |
| taxRemitModel | Az adók (értékesítés, használat vagy áfa/GST-adók) átutalásáért felelős fél | Piacokon |
| taxRemitted (megadó) | A kivetített adó összege (értékesítés, felhasználás vagy áfa/GST-adó) | Piacokon |
| taxState | Az ügyfél állapota |  |
| taxZipCode | Az ügyfél irányítószáma |  |
| tpan (tpan) | A külső hirdetéshálózatot jelzi | marketplaces Csak hirdetések |
| transactionAmount (tranzakció összege) | A bevételt generáló tranzakció összege az eredeti tranzakció pénznemében | Mind |
| transactionAmountUSD | Tranzakció összege USD-ben | Mind |
| transactionCountryCode | Ország/régió kódja, amelyben a tranzakció történt |  |
| transactionCurrency | Az eredeti ügyféltranzakció pénzneme (ez nem a partner helyének pénzneme) | Mind |
| transactionDate (tranzakció dátuma) | A tranzakció dátuma. Olyan programokhoz hasznos, amelyekben számos tranzakció járul hozzá egy bevételhez | Mind |
| transactionExchangeRate | Az átváltási árfolyam dátuma, amely a megfelelő usd-hez tartozó tranzakció összegét mutatja | Mind |
| transactionId (tranzakcióazonosító) | A tranzakció egyedi azonosítója | Mind |
| transactionPaymentMethod | A tranzakcióhoz használt ügyfél fizetési eszköze, például Kártya, Mobilszolgáltató számlázása vagy PayPal | Piacokon |
| transactionType (tranzakciótípus) | A tranzakció típusa, például vásárlás, visszatérítés, megfordítás vagy költség-visszacsatolás | Piacokon |
| számítási feladat | Számítási feladat | Ösztönzők – csak néhány program |
|

### <a name="transaction-adjustment-codes"></a>Tranzakciókorrekciós kódok

Az alábbi táblázat a módosítások okkódját és azok leírását sorolja fel.

|**Okkód**   |**Leírás**   |
|------------------|:-------------------------------------|
| AR-megfelelőség | Olyan módosítás, amely csökkenti a bevételeket, ha a partner nem időben fizeti ki a Microsoft-számlákat. |
| Együttműködésváltás | Az együttműködési bevételek másik időszakra való átcsoportosítása, vagy az együttműködési bevételek átalakításával. |
| Műveletek módosítása | A Microsoft rendszerszámítási hibáit kijavító módosítás. |
| Ops Adjustment Microsoft helytelen kalkulatív | A helytelenszámításokat kijavító módosítás. |
| Ops Adjustment Microsoft helytelen regisztráció | A regisztrációval kapcsolatos hibásszámítások módosítása. |
| Partnerleképezés (előfizetés) MCI/CSP | Az előfizetések helytelen igazítását kijavító módosítás. |
| Szabályzat kivétele | A programszabályt felülbíráló módosítás.  |
| Előző időszak bevételei | Az aktuális bevételi időszakon kívüli bevételek korrekciója. |

## <a name="payments"></a>Kifizetések

A **Kifizetések** lapon részletesen olvashat arról, hogy mennyi pénzt keresett a Microsofttal. Azt is megmutatja, hogy mikor és mennyit kell fizetni.

>[!Note]
> Ahhoz, hogy jogosult legyen a kifizetésre, a bevételnek el kell érnie az 50 usd fizetési küszöbértéket. [](payment-thresholds-methods-timeframes.md) További információkért lásd: [Microsoft-közzétevői szerződés.](/legal/marketplace/msft-publisher-agreement)

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Kifizetések áttekintése képernyő.":::

- **Az idei teljes** kifizetés – Az ebben az évben kifizetett teljes összeg, amerikai dollárban az összes programért.
- **Következő becsült kifizetés** – Az egyetlen következő kifizetés, amely hamarosan érkezik (még akkor is, ha hamarosan mások is lesznek), amerikai dollárban.
- **Utolsó kifizetés** – A legutóbbi kifizetés összege (amerikai dollárban), a program neve és programja.
- **Kifizetés forrás szerint** – A kifizetések összege (amerikai dollárban), programonként, az elmúlt 12 hónapra.

### <a name="payments-list"></a>Kifizetések listája

A **Kifizetések listája táblázat** a fizetős és a függőben lévő kifizetéseket jeleníti meg. Letöltheti a szolgáltatási díj adóinformációját PDF formátumban, és megtekintheti az adott kifizetés bevételi adatait.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Tranzakcióelőzmények exportálása":::

- **Paid** (Fizetős) – Minden sikeresen elküldött kifizetés. Válassza ki az évet a legördülő menüben az abban az évben kiadott kifizetések szűréséhez.
- **Függőben –** Közelgő kifizetések.
- **Szolgáltatási díj adója (PDF-űrlap)** – A szolgáltatási díj adója hatálya alá tartozó kifizetésekhez érhető el. A szolgáltatási díjak adói az **Egyéb adók között jelennek meg.**
- **View** (Nézet) – A tranzakciós előzményekre irányítja át a kifizetésben szereplő bevételek listáját.

Ha meg kell értenie, hogy miért hiányoznak vagy váratlan bevételek, tekintse meg a kereskedelmi piactéri kifizetésekre vonatkozó gyakori [kérdéseket.](payout-faq.md#why-are-my-earnings-missing)

### <a name="payment-status"></a>Fizetési állapot

Az alábbi táblázat a különböző bevételi állapotokat ismerteti.

| Bevétel állapota | Ok | Partneri beavatkozásra van szükség? |
| --- | --- | --- |
| Feldolgozatlan | A bevétel jogosult a kifizetésre. Ebben az állapotban marad egy hűtési időszakban, ahogyan azt a program útmutatója Ösztönzőprogram. | No |
| Közelgő | Függőben lévő belső felülvizsgálatra váró fizetési rendelés a fizetés feldolgozása előtt. | No |
| Függőben lévő adószámla | Az adószámla hiányos vagy érvénytelen. | A fizetés előtt frissítenie kell az adószámlát |
| Elutasítva a felülvizsgálat során | A kifizetést a felülvizsgálat során elutasították. | Részletekért forduljon a Microsoft ügyfélszolgálatához |
| Sikertelen | A fizetés a Microsoft rendszerhiba miatt meghiúsult. | Részletekért forduljon a Microsoft ügyfélszolgálatához |
| Folyamatban | A kifizetés folyamatban van. | No |
| Helytelen fizetés | Folyamatban van a kifizetések újrafizetése. | No |
| Elküldött | A kifizetés el lett küldve a banknak. | No |
| Újrafeldolgozási | A kifizetés során a Microsoft rendszerhiba lépett fel, és folyamatban van a folyamat újrafeldolgozása. | No |
| Reversed | A kifizetést a bank visszavonta, és a következő fizetési ciklusban újra elküldjük. | No |
| Elutasított adószámla | Az adószámla el lett utasítva a felülvizsgálat során. Az összes függőben lévő kifizetés fel lesz függve, amíg az adószámla áttekintése be nem fejeződik. | Részletekért forduljon a Microsoft ügyfélszolgálatához |
| Felülvizsgálat alatt szereplő adószámla | Az adószámla felülvizsgálata folyamatban van. A kifizetése az adószámla jóváhagyása után lesz felszabadítva. | No |
| Elutasítva | A kifizetést a bank elutasította. | A részletekért forduljon a bankhoz. |
|

### <a name="payments-download"></a>Kifizetések letöltése

 Az alábbi táblázat ismerteti a jelentés egyes oszlopát. A kifizetésekkel kapcsolatos további részletekért válassza **a** Letöltés lehetőséget a Kifizetések oldal tetején.

| Oszlop neve | Leírás |
| --- | --- |
| résztvevőazonosító | A program keretében bevételt szerező partner elsődleges identitása |
| participantIDType (résztvevőazonosító típusa) | Általában az ösztönzőprogramok programazonosítója és az áruházi programok értékesítői azonosítója |
| résztvevő neve | A bevételi partner neve |
| programName | Ösztönzők/áruházi program neve |
| Szerzett | Az adott program/résztvevőazonosító fizetendő összege a Fizetési pénznemben |
| earnedUSD | A program/résztvevő azonosítója után kapott összeg, USD-ben |
| withheldTax | A program/résztvevőazonosító fizetési pénznemében visszatartott adó összege |
| salesTax (értékesítés adója) | A program/résztvevőazonosító fizetendő pénznemében szereplő értékesítési adó teljes összege (csak ösztönzőprogramok esetén alkalmazható) |
| serviceFeeTax | A program/résztvevőazonosító serviceFeeTax teljes összege (csak áruházi programokra és Azure Marketplace pénznemben) |
| teljes kifizetés | Teljes kifizetés helyi pénznemben, a visszatartott adó és a program/résztvevőazonosító értékesítési adójának (ha van) nélkül |
| currencyCode | Pénznemkód fizetése |
| paymentMethod | A partner fizetési módszere, például elektronikus banki átutalás, jóváírás |
| paymentID (fizetésiazonosító) | A kifizetés egyedi azonosítója. Ez a szám általában látható a banki kimutatásban (csak SAP-kifizetések esetén alkalmazható). |
| paymentStatus | Fizetési állapot |
| paymentStatusDescription (paymentStatusDescription) | A fizetési állapot rövid leírása |
| paymentDate (kifizetésidátum) | A Microsoft által küldött kifizetés dátuma |
|

## <a name="export-data"></a>Adatok exportálása

Az **Adatok exportálása** lap nem frissül egyedül. Előfordulhat, hogy a legfrissebb adatokhoz manuálisan kell frissítenie az oldalt. A három lapfül közül kiválasztva exportálhatja a **Tranzakciós** előzményeket, a **Kifizetéseket,** a **Tranzakció összegzése** adatokat vagy a **korábbi kimutatásokat.**

A szűrő "Nincs elérhető **adat" hibaüzenetet eredményezhet.** Ez akkor fordulhat elő, ha az alapértelmezett időszakot három hónapon belül választotta ki, majd az adott időszakon kívüli bevételből kiválasztott egy fizetési azonosítót. Ha ez történik, bontsa ki az időszakot, és próbálkozzon újra.

Példa a kifizetések exportálására:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Fizetési jelentés exportálása.":::

### <a name="historical-statements"></a>Korábbi utasítások

Az **Adatok exportálása** összegzés az előzmény-utasításokhoz is hozzáférést biztosít.

> [!NOTE]
> A korábbi állítások pillanatképek, és nem frissülnek. Ha szükséges, forduljon az [ügyfélszolgálathoz,](https://partner.microsoft.com/support/v2/?stage=1) és kérje a legfrissebb adatokat.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Korábbi utasítások exportálása.":::

- A 2019. július 1. előtti tranzakcióelőzmények kezelése külön történik, és a későbbi előzményjelentések különböző mezőit használja.
- Az örökölt tranzakcióelőzmények egyik oszlopa "Fenntartott", amely a modern előzmények "Bevételek" oszlopának felel meg, azzal a kivételsel, hogy kizárja az összes olyan bevételt, amelynek állapota "Payment Sent" (Elküldött fizetés).
- Az olyan szűrők, mint a 3M, a 6M vagy a 12M, nem vonatkoznak az Előzmény utasítások szakaszra.

### <a name="historical-statement-downloads"></a>Korábbi kimutatások letöltései

Az alábbi táblázat egy korábbi utasítás minden oszlopát ismerteti.

| Mező neve | Description |
| --- | --- |
| Bevétel forrása | A bevétel forrása a tranzakció helyének (például Microsoft Store, Windows Phone-telefon Store, Windows Store 8 vagy advertising) alapján |
| Rendelésazonosító | Egyedi rendelésazonosító. Ez az azonosító lehetővé teszi, hogy azonosítsa a vásárlási tranzakciókat a megfelelő nem vásárlási tranzakciókkal, például visszatérítésekkel vagy költségtérítésekkel. Mindkettőnek ugyanaz lesz a rendelésazonosítója. Emellett, ha felosztott díj van, és több fizetési módot használtak egyetlen vásárláshoz, lehetővé teszi a vásárlási tranzakciók csatolását. |
| Tranzakcióazonosító | Egyedi tranzakcióazonosító. |
| Tranzakció dátuma és ideje | A tranzakció dátuma és időpontja (UTC). |
| Szülőtermék azonosítója | A szülőtermék egyedi azonosítója. Ha nincs szülőtermék a tranzakcióhoz, akkor a Szülő termék azonosítója = Termékazonosító. |
| Termék azonosítója | Egyedi termékazonosító. |
| Szülőtermék neve | A szülőtermék neve. Ha nincs szülőtermék a tranzakcióhoz, akkor a Szülőtermék neve = Terméknév. |
| Terméknév | A termék neve |
| Termék típusa | Termék típusa, például alkalmazás, bővítmény vagy játék |
| Mennyiség | Ha a Revenue Source (Bevétel forrása) Microsoft Store Vállalatoknak, a Quantity (Mennyiség) a megvásárolt licencek számát jelöli. Minden más bevételi forrás esetén a Mennyiség mindig 1 lesz. Még ha egyetlen tranzakció két sorelemre is fel van osztva, mert két különböző fizetési módot használtak, minden sorelemnél 1 mennyiség fog mutatni. |
| Transaction Type (Tranzakció típusa) | A tranzakció típusa, például vásárlás, visszatérítés, megfordítás vagy költség-visszacsatolás |
| Fizetési mód | A tranzakcióhoz használt ügyfél fizetési eszköze, például Kártya, Mobilszolgáltató számlázása vagy PayPal |
| Ország/régió | Ország/régió, ahol a tranzakció történt |
| Helyi szolgáltató /értékesítő | Helyi szolgáltató/rekord értékesítője |
| Tranzakció pénzneme | A tranzakció pénzneme |
| Tranzakció összege | A tranzakció összege |
| Adó újrakérte | A kivetített adó mennyisége (értékesítés, felhasználás vagy áfa-/GST-adó) |
| Nettó nyugták | A tranzakció összege a kivetített adóval kevesebb |
| Áruházi díj | A Microsoft által az alkalmazás vagy bővítmény Áruházban való elérhetővé fizetéseként megőrzhető nettó bevételek százalékos aránya |
| Alkalmazás-folytatások | Nettó bevételek az áruházi díjból levonva |
| Adókat visszatartott | A visszatartott bevételi adó mennyisége (a fenntartott **CSV-fájlban** nem szerepel) |
| Payment | Az alkalmazás kevesebb alkalmazható bevételi adóelőleget (a tranzakciós pénznemben látható összeget) folytat. A Reserved **CSV-fájl** nem tartalmazza. |
| FX Rate | A tranzakciós pénznem fizetési pénznemre való átváltási árfolyama |
| Kifizetés pénzneme | A kifizetés pénzneme |
| Átváltott fizetés | A fizetési pénznemre átváltott fizetési összeg az FX-árfolyam használatával |
| Adóátcsoport-lási modell | Az adók (értékesítés, használat vagy áfa/GST-adók) átutalásáért felelős fél |
| Jogosultság dátuma és ideje | A tranzakció bevételének dátuma és időpontja jogosulttá válik a kifizetésre (UTC). A kifizetési folyamat a kifizetési dátum előtti jogosultsági dátummal (csak a Fenntartott  CSV-fájlban szerepel) tartalmazza a tranzakciókat. |
| Díjak | A Transaction Amount (Tranzakció összege) oszlopban összesített összes díj részleteit jeleníti meg (csak az Azure Marketplace, a **Fenntartott** CSV-fájl nem tartalmazza). |
|||

## <a name="next-steps"></a>Következő lépések

- [Partner Payout API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Fizetési szabályzat részletei](payout-policy-details.md)
- Számlázási támogatásért forduljon a kereskedelmi piactér [közzétevőinek ügyfélszolgálatához.](https://partner.microsoft.com/support/v2/?stage=1)