---
title: Kifizetési nyilatkozat a kereskedelmi piactérhez a partner Centerben
description: Megtudhatja, hogyan tekintheti meg és exportálhatja a kereskedelmi piactéren a kifizetési adatokat és Összegzéseket
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.date: 09/23/2020
ms.openlocfilehash: 460a7b1992d7db40e0f45d3aeb7e2236e9495e07
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/25/2020
ms.locfileid: "92530127"
---
# <a name="payout-statements"></a>Kifizetési utasítások

A **kifizetési nyilatkozat** áttekintést nyújt a kereskedelmi piactéren eladott ajánlatokból származó kifizetésekről. Megjeleníti a bevétel tranzakciós előzményeit, kibecsüli a következő befizetést, és megjeleníti a fizetési trendeket. A tranzakciós előzményeket és a fizetési utasításokat is letöltheti. Ez a cikk bemutatja, hogyan férhet hozzá a kifizetési nyilatkozathoz, valamint a különböző kifizetések oldalaihoz és letöltésekhez a partner Centerben.

## <a name="roles-and-permissions"></a>Szerepkörök és engedélyek

A kifizetési utasítások eléréséhez hozzá kell rendelnie a **fiók tulajdonosa** vagy a **pénzügyi közreműködő** szerepkört.

| Jelentések/lapok | Fióktulajdonos | Manager | Fejlesztő | Üzleti közreműködő | Pénzügyi közreműködő | Marketingszakértő |
| --- | --- | --- | --- | --- | --- | --- |
| Beszerzési jelentés (beleértve a közel valós idejű adatfeldolgozást) | Megtekinthető | Megtekinthető | Nincs hozzáférés | Nincs hozzáférés | Megtekinthető | Nincs hozzáférés |
| Visszajelzési jelentés/válaszok | Megtekintheti és elküldheti a visszajelzést | Megtekintheti és elküldheti a visszajelzést | Megtekintheti és elküldheti a visszajelzést | Nincs hozzáférés | Nincs hozzáférés | Megtekintheti és elküldheti a visszajelzést |
| Állapotjelentés (a közel valós idejű adatfeldolgozást is beleértve) | Megtekinthető | Megtekinthető | Megtekinthető | Megtekinthető | Nincs hozzáférés | Nincs hozzáférés |
| Használat jelentés | Megtekinthető | Megtekinthető | Megtekinthető | Megtekinthető | Nincs hozzáférés | Nincs hozzáférés |
| Kifizetési fiók | Frissíthet | Nincs hozzáférés | Nincs hozzáférés | Nincs hozzáférés | Frissíthet | Nincs hozzáférés |
| Adózási profil | Frissíthet | Nincs hozzáférés | Nincs hozzáférés | Nincs hozzáférés | Frissíthet | Nincs hozzáférés |
| Kifizetés összegzése | Megtekinthető | Nincs hozzáférés | Nincs hozzáférés | Nincs hozzáférés | Megtekinthető | Nincs hozzáférés |
|

## <a name="access-your-payout-statement"></a>Hozzáférés a kifizetési nyilatkozathoz

Jelentkezzen be a [partner Centerbe](https://partner.microsoft.com/dashboard/home) , és válassza ki a képernyő jobb felső sarkában található kifizetési ikont a különböző összefoglalók eléréséhez:

- Tranzakciók előzményei
- Kifizetések
- Adatok exportálása

:::image type="content" source="images/payouts/payout-overview.png" alt-text="A partner Center portál jobb felső sarkában látható kifizetési ikon ábrázolása":::

A [partneri kifizetési API](https://apidocs.microsoft.com/services/partnerpayouts) -val a kifizetési tranzakciók és a fizetési műveletek közvetlen összekapcsolására és beszerzésére is lehetősége van.


## <a name="transaction-history"></a>Tranzakciók előzményei

A **tranzakciók előzményei** oldalon látható a bevétel összegzése, a becsült következő fizetés, valamint a bevétel és a fizetések trendje az elmúlt 36 hónapban. Ebből a szakaszból a tranzakciók részleteit is letöltheti.

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="A partner Center portál jobb felső sarkában látható kifizetési ikon ábrázolása":::

- **Bevétel az idei évre** – a befizetett keresetek teljes bevétele és bontása, amelyet a rendszer a következő hónapban fog fizetni.
- **Becsült fizetési hónap** – az elkövetkező hónapokban várható teljes bevétel.
- **Bevétel és fizetési trend** – havi kereseti és fizetési összegek az elmúlt 36 hónapban.
- **Letöltés** – tranzakció részleteinek letöltése. csv vagy. TSV formátumban.

A lap jobb felső sarkában található dátumtartomány-kijelöléssel szűrheti az oldal kimenetét az elmúlt 3, 6, 12 vagy 36 hónap megjelenítéséhez. Vagy válasszon ki egy egyéni dátumtartományt, amely legfeljebb 36 hónapig terjedhet ki. Az alapértelmezett dátumtartomány 12 hónap.

:::image type="content" source="images/payouts/search-filter.png" alt-text="A partner Center portál jobb felső sarkában látható kifizetési ikon ábrázolása":::

### <a name="transaction-history-summary"></a>Tranzakció előzményeinek összegzése

Ez a jövedelemszerzési adatokat jeleníti meg, beleértve az eladott termékből származó bevétel dátumát, állapotát és a becsült fizetési hónapot.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="A partner Center portál jobb felső sarkában látható kifizetési ikon ábrázolása":::

- **Megszerzett dátum** – a vásárlás dátuma.
- **Kereset típusa** – a keresett típus, például értékesítés, árengedmény vagy Co-op.
- **Teljes összeg** – a nettó bevétel összege. Ez azt jelenti, hogy a kereskedelmi piactéren ez a standard szintű Piactéri díj levonása után történik.
- **Állapot** – három lehetőség közül választhat:
    - **Közelgő** – a bevétel függőben lévő hűtési időszakban van.
    - **Feldolgozott** – a bevétel a következő befizetéshez készül.
    - **Elküldve** – a bevételeket kifizették.
- **Becsült fizetési hónap** – a bevételt várhatóan fizető hónap.

A jövedelemszerzési tranzakciók akkor jelennek meg, ha a tranzakció megfelel a kifizetési jogosultságnak. Annak megismeréséhez, hogy miért lehet hiányzó vagy váratlan eredmény, tekintse meg a [kereskedelmi Marketplace-kifizetések gyakori kérdéseit](payout-faq.md#why-are-my-earnings-missing).

### <a name="transaction-history-download"></a>Tranzakciós előzmények letöltése

Ha további részleteket szeretne megtekinteni egy adott feladatról, válassza a **Letöltés** lehetőséget az oldal tetején. A következő táblázat a jelentés egyes oszlopait mutatja be.

| Oszlop neve | Leírás | Ösztönző programok/piactérek alkalmazhatósága |
| --- | --- | --- |
| agreementEndDate | Szerződés befejezési dátuma | Ösztönzők – csak néhány program |
| agreementNumber | Szerződés száma | Ösztönzők – csak néhány program |
| agreementStartDate | Szerződés kezdő dátuma | Ösztönzők – csak néhány program |
| calculationDate | A keresett adat kiszámításának dátuma a rendszeren | Mind |
| claimId | Jogcím egyedi azonosítója | Ösztönzők – csak néhány program |
| customerCountry | Ügyfél országa/régiója | piacterek |
| customerEmail |  |  |
| Customername ( | Mindig üres lesz | Csak ösztönző programok (kivétel: OEM) és piactér |
| customerTenantId |  |  |
| distributorId | Terjesztő azonosítója | Ösztönzők – csak néhány program |
| distributorName | Terjesztő neve | Ösztönzők – csak néhány program |
| earningAmount | Jövedelemszerzési összeg az eredeti tranzakció pénznemében | Mind |
| earningAmountInLastPaymentCurrency | Az utolsó fizetési pénznemben befizetett összeg (a mező üresen marad, ha nem fizettek ki előzetes fizetést) |  |
| earningAmountUSD | Jövedelemszerzési összeg USD-ben | Mind |
| earningDate | A kereset dátuma | Mind |
| earningExchangeRate | A megfelelő USD összeg megjelenítéséhez használt árfolyam | Mind |
| earningId | Az egyes keresések egyedi azonosítója | Mind |
| earningRate | A tranzakciós mennyiségre alkalmazott ösztönzők aránya a kereset létrehozásához | Mind |
| earningType | Azt jelzi, hogy díj, árengedmény, Co-op, értékesítés stb. | Mind |
| exchangeRateDate | Az EarningAmount USD kiszámításához használt Exchange-árfolyam dátuma | Mind |
| externalReferenceId | A program egyedi azonosítója | Közvetlen fizetési programok (ösztönzők és piactér) |
| externalReferenceIdLabel | Egyedi azonosító felirata | Közvetlen fizetési programok (ösztönzők és piactér) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Számla száma (csak a vállalati verzióra vonatkozik) | Ösztönzők és piactér – csak néhány program |
| lastPaymentCurrency | Utolsó fizetési pénznem (a mező üresen marad, ha nem fizettek ki előzetes fizetést) |  |
| szintje | Üzleti szabályt jelez a beszerzéshez | Mind |
| LicensingProgramName | A licencelési program neve |  |
| LineItemId | Egyéni sor az ügyfél számláján |  |
| localProviderSeller | Helyi szolgáltató/a rekord eladója |  |
| Lejárat hónapja | A becsült fizetési hónap | Mind |
| OrderId | Az ügyfél számlára vonatkozik  | piacterek |
| parentProductId | Egyedi szülő termék azonosítója. Ha nincs fölérendelt termék a tranzakcióhoz, akkor a szülő termék azonosítója = termékazonosító. | piacterek |
| parentProductName | A szülő termék neve. Ha nincs fölérendelt termék a tranzakcióhoz, akkor a szülő terméknév = terméknév nevet adja meg. | piacterek |
| participantId | A program keretében keresett partner elsődleges identitása | Mind |
| participantIdType | Elsősorban program-azonosító az ösztönző programok és az eladó számára, ha a piactéren | Mind |
| participantName | A jövedelemszerzési partner neve | Mind |
| partnerCountryCode | A jövedelemszerzési partner helye/országa/régiója | Mind |
| partNumber | Mindig üres lesz | Néhány ösztönző program és piactér |
| paymentId | A fizetés egyedi azonosítója. Ez a szám általában a banki utasításban látható | Csak SAP-fizetések |
| paymentStatus | Fizetési állapot | Mind |
| paymentStatusDescription | A fizetési állapot rövid leírása | Mind |
| productId | Egyedi termékazonosító | piacterek |
| productName | A tranzakcióhoz társított terméknév | Mind |
| productType | A termék típusa, például alkalmazás, bővítmény vagy játék | piacterek |
| Programkód | A program nevével leképezhető karakterlánc |  |
| Programnév | Ösztönző/tároló program neve | Mind |
| purchaseOrderCoverageEndDate | Mindig üres lesz | Ösztönző program – ICC |
| purchaseOrderCoverageStartDate | Mindig üres lesz | Ösztönző program – ICC |
| purchaseOrderType | Mindig üres lesz | Ösztönző program – ICC |
| purchaseTypeCode | Mindig üres lesz | Ösztönző program – ICC |
| quantity | A programtól függően változhat. A tranzakciós programok számlázott mennyiségét jelzi. | Mind |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Viszonteladó azonosítója | Ösztönzők – csak néhány program |
| Viszonteladó neve | Viszonteladó neve |  |
| SkuId | A közzététel során definiált SKU-azonosító. Egy ajánlat több SKU-val is rendelkezhet, de egy SKU csak egyetlen ajánlattal társítható. Ösztönzők – csak néhány program |  |
| storeFee | A Microsoft által a tárolóban az alkalmazás vagy a bővítmény elérhetővé tételének díjaként megőrzött összeg | piacterek |
| subscriptionEndDate | Előfizetés befejezési dátuma | Ösztönzők – csak néhány program |
| subscriptionId | Az ügyfélhez társított előfizetés-azonosító | Ösztönzők – csak néhány program |
| subscriptionStartDate | Előfizetés kezdő dátuma | Ösztönzők – csak néhány program |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Az adók (értékesítési, használati, ÁFA/GST-adók) átutalásával megbízott fél | piacterek |
| taxRemitted | Átutalt adó mennyisége (értékesítés, felhasználás vagy ÁFA/GST-adó) | piacterek |
| taxState | Ügyfél állapota |  |
| taxZipCode | Az ügyfél irányítószáma |  |
| tpan | A harmadik féltől származó ad-hálózatot jelzi | csak a piactéren elérhető hirdetések |
| transactionAmount | A tranzakció összege az eredeti tranzakció pénznemében, amely alapján létrejött a kereset | Mind |
| transactionAmountUSD | Tranzakció összege USD-ben | Mind |
| transactionCountryCode | Az ország/régió kódja, amelyben a tranzakció történt |  |
| transactionCurrency | A pénznem, amelyben az eredeti ügyfél-tranzakció bekövetkezett (ez nem a partneri hely pénzneme) | Mind |
| transactionDate | A tranzakció dátuma. Olyan programok esetében hasznos, amelyekben sok tranzakció járul hozzá egy adott keresethez | Mind |
| transactionExchangeRate | A megfelelő tranzakció USD-értékének megjelenítésére használt árfolyam dátuma | Mind |
| Tranzakcióazonosító | A tranzakció egyedi azonosítója | Mind |
| transactionPaymentMethod | A tranzakcióhoz használt ügyfél-fizetési eszköz, például kártya, mobil szolgáltatói számlázás vagy PayPal | piacterek |
| transactionType | A tranzakció típusa, mint például a vásárlás, a visszatérítés, a sztornírozás vagy a jóváírás | piacterek |
| számítási feladat | Számítási feladat | Ösztönzők – csak néhány program |
|

## <a name="payments"></a>Kifizetések

A **Payments** oldalon megtudhatja, hogy a Microsoft milyen pénzt szerzett. Azt is megmutatja, hogy mikor és mennyit kell fizetnie.

>[!Note]
> Ahhoz, hogy jogosult legyen a kifizetésre, a bevételnek el kell érnie a $50-es [fizetési küszöbértéket](payment-thresholds-methods-timeframes.md) . További információ: [Microsoft kiadói szerződés](https://go.microsoft.com/fwlink/?LinkID=699560).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="A partner Center portál jobb felső sarkában látható kifizetési ikon ábrázolása":::

- Az **év összes kifizetett összege** – a teljes összegért az év minden programja esetében, az Egyesült államokbeli dollárban.
- **Következő becsült fizetés** – az egyszeri következő fizetés érkezik Önhöz (még akkor is, ha hamarosan mások is érkeznek), USA dollárban.
- **Utolsó fizetés** – a legutóbbi fizetés összegét (amerikai dollárban), a program nevét és a programot.
- **Fizetés forrás szerint** – az elmúlt 12 hónapban kifizetett összegek (amerikai dollárban).

### <a name="payments-list"></a>Kifizetések listája

A **Payments (kifizetések** ) tábla a fizetős és a függőben lévő fizetések listáját tartalmazza. A szolgáltatási díj adózási adatait PDF formátumban töltheti le, és megtekintheti egy adott fizetés részleteit.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="A partner Center portál jobb felső sarkában látható kifizetési ikon ábrázolása":::

- **Fizetős** – az összes befizetés sikeresen elküldése. A legördülő menüben válassza ki az évet az adott évben kiadott kifizetések szűréséhez.
- **Függőben** – közelgő fizetések.
- **Szolgáltatási díj adója (PDF-űrlap)** – a szolgáltatás díjas adójához tartozó fizetések esetében elérhető. A szolgáltatási díj adókat **más adók** mutatják be.
- **Nézet** – a rendszer átirányítja a tranzakciós előzményekre a kifizetés részét képező keresetek listájával.

Annak megismeréséhez, hogy miért lehet hiányzó vagy váratlan eredmény, tekintse meg a [kereskedelmi Marketplace-kifizetések gyakori kérdéseit](payout-faq.md#why-are-my-earnings-missing).

### <a name="payment-status"></a>Fizetési állapot

A következő táblázat ismerteti a különböző jövedelemszerzési állapotokat.

| Jövedelemszerzési állapot | Ok | Partneri beavatkozás szükséges? |
| --- | --- | --- |
| Feldolgozatlan | A kereset jogosult a fizetésre. Ebben az állapotban marad az ösztönző program program útmutatójában meghatározott hűtési időszakra vonatkozóan. | Nem |
| Közelgő | A függőben lévő belső felülvizsgálatok által a fizetés feldolgozása előtt generált fizetési sorrend. | Nem |
| Függőben lévő adó számla | Az adó számla nem teljes vagy érvénytelen. | A fizetés előtt frissítenie kell az áfát |
| Elutasította a felülvizsgálat során | A rendszer elutasította a fizetést a felülvizsgálat során. | Részletekért forduljon a Microsoft ügyfélszolgálatához |
| Sikertelen | A fizetés Microsoft rendszerhiba miatt nem sikerült. | Részletekért forduljon a Microsoft ügyfélszolgálatához |
| Folyamatban | A fizetés folyamatban van. | Nem |
| Helytelen fizetés | A fizetési Újracsatlakozás folyamatban van. | Nem |
| Elküldött | A rendszer elküldje a fizetést a banknak. | Nem |
| Újrafeldolgozás | A fizetés Microsoft rendszerhibát észlelt, és folyamatban van az újrafeldolgozása. | Nem |
| Reversed | A fizetést a bank fordította, és a következő fizetési ciklusban ismét elküldi a rendszer. | Nem |
| Számlaösszeg elutasítva | Az adó számla elutasítása a felülvizsgálat során megtörtént. Az összes függőben lévő kifizetés addig tart, amíg az adó számla felülvizsgálata be nem fejeződik. | Részletekért forduljon a Microsoft ügyfélszolgálatához |
| Adózási számla a felülvizsgálat alatt | Az adó számla felülvizsgálata folyamatban van. A kifizetését az adó-számla jóváhagyása után bocsátja ki a rendszer. | Nem |
| Elutasítva | A Bank elutasította a fizetést. | Részletekért forduljon a bankhoz. |
|

### <a name="payments-download"></a>Kifizetések letöltése

Ha további részleteket szeretne megtudni a kifizetésekről, válassza a **Letöltés** lehetőséget az oldal tetején. A következő táblázat a jelentés egyes oszlopait mutatja be.

| Oszlop neve | Leírás |
| --- | --- |
| participantID | A program keretében keresett partner elsődleges identitása |
| participantIDType | Általában a program azonosítója az ösztönző programokhoz és az eladói AZONOSÍTÓhoz az áruházi programokhoz |
| participantName | A jövedelemszerzési partner neve |
| Programnév | Ösztönzők/tárolási program neve |
| szerzett | Az adott programhoz/participantID tartozó fizetési pénznemben szerzett összeg |
| earnedUSD | A program/résztvevő azonosítója számára elért összeg USD-ben |
| withheldTax | A program-vagy participantID fizetési pénznemében visszatartott adó összege |
| salesTax | A program-vagy participantID tartozó fizetési adó teljes összege (csak ösztönző programok esetén alkalmazható) |
| serviceFeeTax | A program/participantID (csak az áruházi programokra és az Azure Marketplace-re vonatkozó) pénznemben fizetendő serviceFeeTax teljes mennyisége |
| totalPayment | Teljes kifizetés a helyi pénznemben, kivéve a visszatartási adót, valamint a program-vagy participantID vonatkozó forgalmi adót (ha van ilyen). |
| currencyCode | Fizetés a pénznemkóddal |
| paymentMethod | A partner fizetéséhez használt módszer, például az elektronikus banki átutalás, a jóváírási Megjegyzés |
| paymentID | A fizetés egyedi azonosítója. Ez a szám általában a banki utasításban látható (csak az SAP-fizetésekre vonatkozik). |
| paymentStatus | Fizetési állapot |
| paymentStatusDescription | A fizetési állapot rövid leírása |
| paymentDate | A Microsofttól érkezett fizetési határidő |
|

## <a name="export-data"></a>Adatok exportálása

Az **adatexportálás** lap nem frissül a sajátján. Előfordulhat, hogy manuálisan kell frissítenie a lapot a legfrissebb információk megtekintéséhez. Válassza ki a három lapot a **tranzakciók előzményeinek** , a **fizetések** , a **tranzakciós összefoglalás** vagy a **korábbi utasítások** exportálásához.

Előfordulhat, hogy a szűrő **nem érhető** el az Adathiba miatt. Ez akkor fordulhat elő, ha az alapértelmezett időszakot három hónapban választotta ki, majd kiválasztott egy fizetési azonosítót az adott időszakon kívüli keresőből. Ha ez történik, bontsa ki az időtartamot, és próbálkozzon újra.

Íme egy példa a kifizetések exportálására:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="A partner Center portál jobb felső sarkában látható kifizetési ikon ábrázolása":::

### <a name="historical-statements"></a>Korábbi utasítások

Az **adatexportálás** összegzése is hozzáférést biztosít a korábbi utasításokhoz.

> [!NOTE]
> A korábbi utasítások Pillanatképek, és nem frissülnek. Ha szükséges, forduljon az [ügyfélszolgálathoz](https://partner.microsoft.com/support/v2/?stage=1) , és kérje a legfrissebb adatkérést.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="A partner Center portál jobb felső sarkában látható kifizetési ikon ábrázolása" állapottal megegyező összes bevételt kizárják.
- Az olyan szűrők, mint a 3M, 6M vagy 12M, nem lesznek érvényesek a korábbi utasítások szakaszra.

### <a name="historical-statement-downloads"></a>Korábbi utasítások letöltése

Az alábbi táblázat a korábbi utasítások egyes oszlopait mutatja be.

| Mező neve | Leírás |
| --- | --- |
| Bevétel forrása | A bevétel forrása, amely alapján a tranzakció bekövetkezett, például Microsoft Store, Windows Phone-telefon áruház, Windows áruház 8 vagy reklám |
| Rendelésazonosító | Egyedi megrendelési azonosító. Ez az azonosító lehetővé teszi a vásárlási tranzakciók azonosítását a megfelelő nem vásárlási tranzakciókkal, például a visszatérítéssel vagy a jóváírásokkal kapcsolatban. Mindkettő ugyanazzal a megrendelési AZONOSÍTÓval fog rendelkezni. Továbbá, ha van olyan felosztott díj, amelyben több fizetési módszert használtak egyetlen vásárláshoz, akkor a vásárlási tranzakciók összekapcsolhatók. |
| Tranzakcióazonosító | Egyedi tranzakció-azonosító. |
| Tranzakció dátuma és időpontja | A tranzakció dátuma és időpontja (UTC). |
| Szülő termék azonosítója | Egyedi szülő termék azonosítója. Ha nincs fölérendelt termék a tranzakcióhoz, akkor a szülő termék azonosítója = termékazonosító. |
| Termék azonosítója | Egyedi termékazonosító. |
| Szülő terméknév | A szülő termék neve. Ha nincs fölérendelt termék a tranzakcióhoz, akkor a szülő terméknév = terméknév nevet adja meg. |
| Terméknév | A termék neve |
| Termék típusa | A termék típusa, például alkalmazás, bővítmény vagy játék |
| Mennyiség | Ha a bevételi forrás Microsoft Store for Business, a mennyiség a megvásárolt licencek számát jelöli. Az összes többi bevételi forrás esetében a mennyiség mindig 1 lesz. Még akkor is, ha egy tranzakció két sorra van felosztva, mert két különböző fizetési módszert használtak, az egyes sorok egy 1. mennyiséget jelenítenek meg. |
| Transaction Type (Tranzakció típusa) | A tranzakció típusa, mint például a vásárlás, a visszatérítés, a sztornírozás vagy a jóváírás |
| Fizetési mód | A tranzakcióhoz használt ügyfél-fizetési eszköz, például kártya, mobil szolgáltatói számlázás vagy PayPal |
| Ország/régió | Az ország/régió, ahol a tranzakció történt |
| Helyi szolgáltató/eladó | Helyi szolgáltató/a rekord eladója |
| Tranzakció pénzneme | A tranzakció pénzneme |
| Tranzakció mennyisége | A tranzakció mennyisége |
| Átutalt adó | Átutalt adó mennyisége (értékesítés, felhasználás vagy ÁFA/GST-adó) |
| Nettó visszaigazolások | Tranzakciós összeg, amely kevesebb adót átutalt |
| Tárolási díj | A Microsoft által a tárolóban az alkalmazás vagy a bővítmény elérhetővé tételének díjaként megőrzött nettó bevételezések százalékos aránya |
| Alkalmazás folytatása | Nettó visszaigazolások mínusz a tárolási díj |
| Visszatartott adók | Visszatartott jövedelemadó-mennyiség (a **fenntartott** CSV-fájlban található) |
| Payment | Az alkalmazás a vonatkozó jövedelemadó-forrásadót is csökkenti (a tranzakció pénznemében megjelenő mennyiség). Nem szerepel a **fenntartott** CSV-fájlban. |
| FX-díj | A tranzakció pénznemének fizetési pénznemre való átalakításához használt deviza-árfolyam |
| Kifizetés pénzneme | Az a pénznem, amelyben a fizetést elvégezték |
| Átváltott fizetés | Fizetési pénznemre átváltott fizetési összeg az FX-díj használatával |
| Adó-kiutalás modell | Az adók (értékesítési, használati, ÁFA/GST-adók) átutalásával megbízott fél |
| Jogosultság dátuma és időpontja | Az a dátum és idő, amikor a tranzakció bevétele jogosulttá válik a kifizetésre (UTC). A kifizetések létrehozásakor a tranzakció a kifizetés létrehozási dátuma előtt (csak a **fenntartott** CSV-fájlban foglalt) jogosultsági dátummal folytatódik. |
| Díjak | Megjeleníti a tranzakció mennyisége oszlopban összesített összes díj részletezését (csak az Azure Marketplace-en, nem tartalmazza a **fenntartott** CSV-fájl részét). |
|||

## <a name="next-steps"></a>További lépések

- [Partner Payout API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Fizetési szabályzat részletei](payout-policy-details.md)
- Számlázási támogatásért forduljon a kereskedelmi piactér [közzétevő támogatásához](https://partner.microsoft.com/support/v2/?stage=1).