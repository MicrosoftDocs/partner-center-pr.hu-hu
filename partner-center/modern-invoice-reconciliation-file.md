---
title: A CSP-vásárlások fájlmezőinek felderítése
ms.topic: conceptual
ms.date: 01/29/2021
description: Ismerje meg a CSP-hez az egy alkalommal vásárolt egyeztetési fájl összes elemét a Partnerközpont, beleértve a mintaértékeket is.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 85946f44e1265ad5012faf9d782609904100c80e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146255"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CsP egy alkalommal vásárolt egyeztetési fájl mezői

**Megfelelő szerepkörök:** Fiók-rendszergazdai | Számlázási ügynök

## <a name="using-the-recon-file"></a>A recon fájl használata
Az alábbi táblázat a CSP-hez az egyszeres vásárlások egyeztetési fájljában található mezők leírását és mintaértékét tartalmazza.

További információ az egyeztetési fájlokról: [Az egyeztetési fájlok használata.](use-the-reconciliation-files.md)

| Oszlop | Leírás | Mintaérték |
| ------ | ----------- | ------------ |
| Partnerazonosító | Egyedi azonosító GUID formátumban egy adott számlázási entitáshoz. Az egyeztetéshez nem szükséges. Minden sorban ugyanaz. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Az ügyfél egyedi Microsoft-azonosítója GUID formátumban. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Az ügyfél szervezetének neve a Partnerközpont. Ez az oszlop fontos a számla és a rendszerinformációk egyeztetéséhez. | *Johnny Modern Cust DE2* |
| CustomerDomainName (Ügyféltartományneve) | Az ügyfél tartományneve. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry (Ügyfél országa) | Az ügyfél helyének országa. Tekintse meg [a régiója országának](./regional-authorization-overview.md) teljes listáját.  | *DE* |
| InvoiceNumber (Számlaszám) | Az egyeztetési fájlhoz társított számlaszám.  | *G002297372* |
| MpnId | A CSP-partner MPN-azonosítója. További információkért lásd: [elemi elemek létrehozása partner szerint.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId (Viszonteladóimpn-azonosító) | Az előfizetés rekordjának viszonteladójának MPN-azonosítója. | *6048879* |
| OrderId | Rendelés egyedi azonosítója a Microsoft számlázási platformon. Hasznos lehet azonosítani a rendelést, amikor kapcsolatba lép az ügyfélszolgálattal. Az egyeztetéshez nem használatos. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | A rendelés rendelésének dátuma (UTC). | *10/3/2020* |
| ProductId | A termék egyedi azonosítója. | *DZH318Z0BNZ5* |
| SkuId (Termékváltozatazonosító) | A termékváltozat egyedi azonosítója. | *006G* |
| AvailabilityId (Rendelkezésre állásiid) | A rendelkezésre állás egyedi azonosítója. | *DZH318Z08B80* |
| SkuName | A termékváltozat neve. | *Táblák – LRS* |
| TermékNév | A termék neve. | *Táblák* |
| ChargeType | A [díj vagy a módosítás](./recon-file-charge-types.md) típusa. | *Új* |
| UnitPrice | Licencenkénti ár, amely a vásárláskor az árlistában van közzétéve. Győződjön meg arról, hogy ezek megegyeznek a számlázási rendszerben az egyeztetés során tárolt adatokkal. | *0.045* |
| Mennyiség | A licencek száma. Győződjön meg arról, hogy ezek megegyeznek a számlázási rendszerben az egyeztetés során tárolt adatokkal. | *1* |
| Részösszeg | Adóz előtti összeg. A részösszegnek meg kell egyoznia a számlázható mennyiség és a tényleges egységár szorzatával. | *0* |
| TaxTotal (Adóösszeg) | Adó összege díj. A piac adószabályainak és konkrét körülményeinek megfelelően. | *0* |
| Összesen | A teljes összeg megegyezik a részösszeggel és az adó összeggel. | *0* |
| Pénznem | A számla az ügyfél pénzneme alapján jön létre. Ez azt jelenti, hogy ha Ön olyan partner, aki különböző számlázható pénznemek ügyfeleivel bonyolít le tranzakciót, minden ügyfél pénznemtípusról számlát fog kapni.  | *EUR* |
| PriceAdjustmentDescription (Áradjustmentdescription) | Az egységár módosításainak okai. Ezek a fő okok, de nem kizárólagosan a tényleges egységár meghatározása. | *["15,0% partneri jóváírás a felügyelt szolgáltatásokhoz"]* |
| Közzétevő neve | A termék kiadója.  | *Microsoft* |
| PublisherId | A közzétevő azonosításához Partnerközpont egyedi azonosító. | *NA* |
| SubscriptionDescription (Előfizetés-leírás) | Az ügyfél által megvásárolt szolgáltatásajánlat neve az árlistában meghatározottak szerint. Ez az oszlop megegyezik az OfferName mezővel. | *Azure-csomag* |
| SubscriptionId | Az előfizetés egyedi azonosítója a Microsoft számlázási platformon. Az egyeztetéshez nincs használva. Vegye figyelembe, hogy ez az azonosító nem ugyanaz, mint a partner felügyeleti konzolján található előfizetés-azonosító. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate (Költségindításidátum) | Az előfizetés számlázási időszakának kezdete. | *9/1/2020* |
| ChargeEndDate (Költség és költségdátum) | Az előfizetés számlázási időszakának végének dátuma. | *2020. 09. 30.* |
| TermAndBillingCycle | Az előfizetés vásárláskor való folytatására vonatkozó kötelezettségvállalás. | *Tárolt adatok (GB/hónap)* |
| EffectiveUnitPrice (Hatályos egységár) | A számlázási ciklus költségeinek kiszámításához használt időegység-ár. A tényleges egységárat a kedvezmények, a számlázási napok korrekciói és egyéb tényezők határozzák meg. További információ: [Effective Unit Price Calculation (Tényleges egységár kiszámítása).](./effective-unit-price-calculation.md)  | *0.03825* |
| UnitType (Egységtípus) | Az egység típusa, amelyben a fogyasztásmérő fel van számolva. | *1 GB/hónap* |
| AlternateId (Alternatívazonosító) | A hivatkozott rendelési sorelem alternatív azonosítója. | *6dc5c039750a* |
| BillableQuantity | A kiszámlázandó teljes mennyiség.  | *0.005001* |
| BillingFrequency | A vásárláskor kiválasztott számlázási csomag. | *NA*  |
| PricingCurrency | Az árlistán szereplő pénznem. | *USD* |
| PCToBCExchangeRate (PcToBCExchangeRate) | A díjszabási pénznemre alkalmazott átváltási árfolyam a számlázási pénznemre. | *0.846202666* |
| PCToBCExchangeRateDate (PcToBCExchangeRateDate) | Az a dátum, amikor a számlázási pénznem díjszabási pénzneme meg van határozva. | *2020. 09. 30.* |
| MeterDescription (MeterDescription) | A mérő leírása.  | *Táblák – Tárolt LRS-adatok (GB/hó)* |
| ReservationOrderId | A foglalási rendelés azonosítója. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | A kredit leírása. | *Azure-használatra vonatkozó kredit* |

>[!NOTE]
>Az Azure-felhasználást egyeztetheti az egyszeres vásárlás felderítési fájljában. Ehhez keresse meg a napi rendszerességgel minősített használat felderítési fájlját, és keresse meg a SubscriptionID-t. Ez megjeleníti az Azure-csomagazonosítóhoz társított összes költséget. Az Azure SubscriptionID jogosultságazonosítóként jelenik meg.

## <a name="next-steps"></a>Következő lépések

- [Számlázás és adók](billing.md)
