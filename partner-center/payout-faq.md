---
title: A Microsoft kereskedelmi piactérről kifizetéssel kapcsolatos gyakori kérdések
description: Választ kaphat a kereskedelmi piactéren befizetésekkel kapcsolatos gyakori kérdésekre. Válaszokat tartalmaz arról, hogy a bevétel miért különbözik a várttól.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 09/11/2020
ms.openlocfilehash: 5775eb497940870344e0d3da85def7c3e717c65f
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/12/2020
ms.locfileid: "94532021"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>A kereskedelmi piactér kifizetésével kapcsolatos gyakori kérdések

Ez a cikk a kereskedelmi piactéren befizetésekkel kapcsolatos gyakori kérdésekre ad választ.

## <a name="earnings-incorrect-or-missing"></a>Helytelen vagy hiányzó bevétel

#### <a name="why-are-my-earnings-missing"></a>Miért hiányoznak a bevételeim?

- Lehetséges, hogy az ügyfélrendelés még nem jogosult kifizetésre. Nem vállalati ügyfélrendelések esetén a Microsofthoz be kell érkeznie az ügyfél általi kifizetésnek, mielőtt a közzétevői bevétel esedékessé válhatna. Nagyvállalati ügyfelrendelések esetén a bevétel a vásárlás dátuma után 1-2 nappal lesz elérhető. Ellenőrizze a rendelés állapotát a [rendelési jelentésekben](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Lehetséges, hogy a 2019 júliusa előtti tranzakciókból származó bevételek nem jelennek meg a tranzakciós előzmények jelentésében. Tekintse át a korábbi kimutatásokat a [Kifizetések letöltésénél](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Tekintse meg a [kifizetési ciklus időkeretét](payment-thresholds-methods-timeframes.md) , és Ismerje meg, hogy mikor jelenjen meg a bevétel a kifizetési utasításban.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Miért különböznek a bevételem a várttól eltérő összegtől?

- Ha az ügyfél részben fizette meg a rendelést, a bevétel összege a költségek és a megfelelő adó kivonása utáni részben fizetett összeg alapján történik.
- Az adó felelősségének ellenőrzését ország szerint. Azon országok esetében, amelyekben az adójogi felelősség a Microsoftot terheli, a Microsoft szedi be és vonja le az adót a közzétevői bevételekből. A kimutatásban szereplő tranzakcióösszeg az adózás utáni összeg. Tekintse meg az [Adó részleteit](tax-details-marketplace.md).
- Az SaaS-és IaaS a standard 20% helyett 10%-os kedvezményt biztosítunk, így 90%-os bevételi arányt kell fizetni. Ez a promóciós ajánlat 2021. június 30-ig érvényes.

**További olvasnivaló** : [kereskedelmi Marketplace kiadói szerződés](https://go.microsoft.com/fwlink/p/?LinkID=699560), [kifizetési szabályzat részletei](payout-policy-details.md), [fizetési küszöbérték, módszer és időkeret](payment-thresholds-methods-timeframes.md), fizetés [a kereskedelmi piactéren](marketplace-get-paid.md), [adózási adatok](tax-details-marketplace.md), [kifizetési utasítások](payout-statement.md), [megrendelések irányítópult a kereskedelmi piactér elemzésében](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Bevételek egyeztetése
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Hogyan egyeztethetem a kifizetési kimutatásokat a megrendeléshez, illetve a használati jelentéseket az elemzésekben?
A kifizetési tranzakció előzményei jelentésben megjelenő AssetID, Rendeléskód és line Item azonosító használata analitikus megrendelések és használati jelentések használatával. Használja ezt a leképezést:

- Payout Transaction History.AssetID = order.OrderID
- Payout Transaction History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Honnan tudhatom, hogy mikor számíthatok kifizetésre az ügyfélrendeléseimmel kapcsolatban?
- Először is használja a assetID, és adja meg az ügyfelek rendeléseit a [megrendelések jelentésekben](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Az ügyfél-előfizetéshez tartozó ügyfél-csatorna keresése az [ügyfelek jelentésében](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- A nagyvállalati ügyfelek esetében a kiadói bevétel a 1-2 nappal a vásárlási rendelés dátuma után jelenik meg.
- A nem vállalati ügyfelek esetében a kiadói bevétel a 1-2 nappal az ügyfél befizetésének kézhezvétele után jelenik meg.

**További olvasnivaló** : [kifizetési utasítások](payout-statement.md), [megrendelések irányítópultja a kereskedelmi piactér elemzésében](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Kifizetési szabályzatok

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Hol található az aktuális közvetítői díj és a kifizetési arány?

- Tekintse meg a kereskedelmi piactérre vonatkozó közzétevői megállapodást. A közvetítői díj általában 20%. A SaaS Co-Sell jogosult tranzakciói díja 10%. A promóciós közvetítői díjakkal kapcsolatban figyelje a bejelentéseket.
- A kifizetési nyilatkozatban a jövedelemszerzési díj meghatározza az adott tranzakcióhoz tartozó tényleges kifizetési arányt.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Mikor számíthatok kifizetésre a Microsofttól, miután megjelentek a bevételek a kimutatásban?
- Miután a bevétele Nincs feldolgozva állapotba kerül, megtekintheti azon hónap esedékességi dátumát, amelyre vonatkozóan a bevételei fel lesznek dolgozva a kifizetéshez. A fizetés előkészítése után a keresőképesség állapota "feldolgozva" állapotúra változik.  A Microsoft az esedékességi hónap 15. napjáig teljesíti a kifizetéseket.
- A hitelkártyával fizetett megrendelések esetében a Microsoft 30 napot tart a kifizetésig.

 **További olvasnivaló** : [kereskedelmi Marketplace kiadói szerződés](https://go.microsoft.com/fwlink/p/?LinkID=699560), [kifizetési szabályzat részletei](payout-policy-details.md), [adózási adatok](tax-details-marketplace.md), [fizetési küszöbérték, módszer és időkeret](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Kifizetések és beállítások

#### <a name="why-is-my-payment-missing"></a>Miért hiányzik a kifizetésem?

- Győződjön meg arról, hogy a kifizetési állapot és az adózási profil állapota *érvényesként* jelenik meg az [Áttekintés oldalon](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- Előfordulhat, hogy nem felel meg a kifizetések minimális küszöbértékének. A kifizetéshez a bevételnek legalább 50 dollárnak kell lennie.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Hogyan beállítani a fiókomat, hogy ne kapjon fizetést?
A [kifizetés a kifizetési profilban](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)is megtartható; Egyszerűen jelölje be a **megtartás gombot**. A Microsoft csak akkor kapja meg a fizetést, ha kiadja a megtartást.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Miért kapom a kifizetést más pénznemben, mint a vásárlási pénznem?

A kifizetés pénzneme a Kifizetési profil területen kiválasztott pénznemen alapul. A vásárlási pénznem az ügyfél által kifizetés pénznemén alapul.

#### <a name="how-do-i-reconcile-adjustments"></a>Hogyan egyeztethetem a módosításokat?

A kifizetési módosítások olyan kifizetési korrekciók, amelyek (például rendszerhibák esetén) kompenzációs módosításokat tesznek lehetővé. A kifizetési kimutatásban az okkód határozza meg a módosítás okát. Ezek nem egyeztethetők össze közvetlenül az egyes tranzakciókkal.

**További olvasnivaló** : [kereskedelmi Marketplace kiadói szerződés](https://go.microsoft.com/fwlink/p/?LinkID=699560), [kifizetési szabályzat részletei](payout-policy-details.md), [adózási adatok](tax-details-marketplace.md), [fizetési küszöbérték, módszer és időkeret](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Adók

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Hogyan állapítható meg a Microsoft vagy a közzétevő között felmerülő adójogi felelősség a kifizetési kimutatásban?

A tranzakciós előzmények letöltései között keresse meg az Adózási modell oszlopot. Itt kétféle lehetőséget láthat: MS által kezelt vagy ISV által kezelt. Tekintse meg az országspecifikus adózási szabályokat és kifizetési vonzatokat az [Adó részletei](tax-details-marketplace.md) részben.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Hogyan tölthetem le a szolgáltatási díjhoz kapcsolódó adónyomtatványokat?

Nyissa meg a **Kifizetések** oldalt, majd a **Kifizetések listája** részt. Megjelenik egy hivatkozás, amely a szolgáltatási díjjal kapcsolatos adónyomtatványra irányítja olyan fizetés esetén, amely szolgáltatási díjra vonatkozó adót tartalmaz.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Hogyan tölthetem le a forrásadóra vonatkozó adónyomtatványt PDF formátumban?

Nyissa meg a *Kifizetések* oldalt, majd a **Kifizetések listája** részt. A kifizetés mellett megjelenik egy hivatkozás, amely a forrásadóra vonatkozó adónyomtatványhoz irányítja.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Hol találom az év végi adónyomtatványokat?

Az év végi adónyomtatványok megtekintéséhez lépjen a [Profil oldalra](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage).

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Hogyan találhatom meg egy tranzakció forrásadóját?
A forrásadó olyan amerikai közzétevők esetében érvényes, akik W-9-es űrlapot nyújtottak be. A forrásadó számítása havi kifizetésen alapul.

**További olvasnivaló** : [kereskedelmi Marketplace kiadói szerződés](https://go.microsoft.com/fwlink/p/?LinkID=699560), [kifizetési szabályzat részletei](payout-policy-details.md)

## <a name="payout-statement-access"></a>Kifizetési nyilatkozathoz való hozzáférés

#### <a name="how-do-i-access-a-payout-statement"></a>Hogyan férhetek hozzá a kifizetési kimutatásokhoz?

1. Ellenőrizze a szerepköreit. *Pénzügyi közreműködő* vagy *fióktulajdonos* szerepkörrel kell rendelkeznie a kifizetési kimutatás eléréséhez.
2. A jobb felső navigációs sávon válassza a **kifizetés** ikont a kifizetési nyilatkozat megtekintéséhez. Válassza a **tranzakciók előzményei** , a **fizetés** és a **Letöltés** lehetőséget.

**További olvasnivaló** : [kifizetési szerepkörök és engedélyek](payout-statement.md#roles-and-permissions), [kifizetési utasítások](payout-statement.md) 

## <a name="payout-statement-report"></a>Kifizetési nyilatkozat jelentés

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Mit jelentenek a tranzakcióletöltés mezői?

Az attribútumok és jelentésük részletes listájáért lásd a [kifizetési utasítások](payout-statement.md) című témakört.

#### <a name="what-is-earning-status"></a>Mi a bevétel állapota?

Ez a bevétel feldolgozatlan, feldolgozott vagy elküldéses formában jelenik meg.

- **Feldolgozatlan** – a bevételek a lejárat dátumánál korábbi időszakig tartanak.
- **Feldolgozva** – a keresetek kiforrtak, és havi fizetésre készülnek. A kifizetéseket minden hónap 15-én adták ki.
- **Elküldve** – a kifizetés a kifizetési profil alapján sikeresen megjelent a banknak.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Hogyan tölthetem le a szolgáltatási díjhoz kapcsolódó adónyomtatványokat?

Nyissa meg a **Kifizetések** oldalt, majd a **Kifizetések listája** részt. Megjelenik egy hivatkozás, amely a szolgáltatási díjjal kapcsolatos adónyomtatványra irányítja olyan fizetés esetén, amely szolgáltatási díjra vonatkozó adót tartalmaz.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Hogyan letölt egy adóelőleg-űrlapot a PDF-ben?

Nyissa meg a **Kifizetések** oldalt, majd a **Kifizetések listája** részt. A kifizetés mellett megjelenik egy hivatkozás, amely a forrásadóra vonatkozó adónyomtatványhoz irányítja.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Hol találom az év végi adónyomtatványokat?

Az év végi adónyomtatványok megtekintéséhez lépjen a [Profil oldalra](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage).

**További olvasnivaló** : [kifizetési utasítások](payout-statement.md), [tranzakciós előzmények letöltése](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Korábbi utasítások

#### <a name="how-do-i-view-historical-information"></a>Hogyan a korábbi információk megtekintése?

A korábbi kimutatásokban 2019 októberétől láthatók a kifizetési adatok pillanatképei. Sajnos a kifizetési információk itt nem frissülnek. A legfrissebb információk megszerzéséhez küldjön egy támogatási jegyet a legfrissebb adatokhoz.

**További olvasnivaló** : [kifizetési utasítások](payout-statement.md), [tranzakciós előzmények letöltése](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>Kifizetés-exportálási API

#### <a name="how-do-i-download-payout-data"></a>Hogyan tudom letölteni a kifizetési adatokat?

Használja a [partneri kifizetési API](https://apidocs.microsoft.com/services/partnerpayouts)-t.

## <a name="next-steps"></a>Következő lépések

- [Fizetés fogadása a kereskedelmi piactéren](marketplace-get-paid.md)
