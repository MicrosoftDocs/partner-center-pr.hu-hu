---
title: A CSP-hez való egyszeres vásárlások fájlmezőinek felderítése
ms.topic: conceptual
ms.date: 01/29/2021
description: Ismerje meg a CSP egy alkalommal vásárolt egyeztetési fájljában található összes elemet a Partnerközpont, beleértve a mintaértékeket is.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 3264c793dfb2e8592cd059cd84d5bb08769abbcf
ms.sourcegitcommit: c8d1bcf54cdcdc3f827f9210c8abddab02a686fe
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/14/2021
ms.locfileid: "112073798"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP egy alkalommal vásárolt egyeztetési fájl mezői

**Megfelelő szerepkörök:** Fiók-rendszergazdai | Számlázási ügynök

## <a name="using-the-recon-file"></a>A recon fájl használata
Az alábbi táblázat az egyszer megvásárolt CSP egyeztetési fájl mezőinek leírását és mintaértékét tartalmazza.

Az egyeztetési fájlokkal kapcsolatos további információkért lásd: [Az egyeztetési fájlok használata.](use-the-reconciliation-files.md)

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
| TaxTotal (Adóösszeg) | Adó összege díj. A piac adózási szabályai és adott körülmények alapján. | *0* |
| Összesen | A teljes összeg megegyezik a részösszeggel és az adó összeggel. | *0* |
| Pénznem | A számla az ügyfél pénzneme alapján jön létre. Ez azt jelenti, hogy ha Ön olyan partner, aki különböző számlázható pénznemek ügyfeleivel bonyolít le tranzakciót, minden ügyfél pénznemtípusról számlát fog kapni.  | *EUR* |
| PriceAdjustmentDescription (PriceAdjustmentDescription) | Az egységár módosításainak okai. Ezek a fő okok, de nem kizárólagosan a tényleges egységár meghatározása. | *["15,0%- os partneri jóváírás a felügyelt szolgáltatásokért"]* |
| Közzétevő neve | A termék kiadója.  | *Microsoft* |
| PublisherId | A közzétevő azonosítására Partnerközpont egyedi azonosító. | *NA* |
| SubscriptionDescription (Előfizetési leírás) | Az ügyfél által megvásárolt szolgáltatásajánlat neve az árlistában meghatározottak szerint. Ez az oszlop megegyezik az OfferName mezővel. | *Azure-csomag* |
| SubscriptionId | Előfizetés egyedi azonosítója a Microsoft számlázási platformon. Az egyeztetéshez nem használatos. Vegye figyelembe, hogy ez az azonosító nem ugyanaz, mint a partner felügyeleti konzolján található előfizetés-azonosító. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate (Díjindításidátum) | Az előfizetés számlázási időszakának kezdete. | *9/1/2020* |
| ChargeEndDate (Költség és költségdátum) | Az előfizetés számlázási időszakának végének dátuma. | *2020. 09. 30.* |
| TermAndBillingCycle | Az előfizetés vásárláskor való folytatására vonatkozó kötelezettségvállalás. | *Tárolt adatok (GB/hónap)* |
| EffectiveUnitPrice (Hatályos egységár) | A számlázási ciklus költségeinek kiszámításához használt időegység-ár. A tényleges egységárat a kedvezmények, a számlázási napok korrekciói és egyéb tényezők határozzák meg. További információ: [Effective Unit Price Calculation (Tényleges egységár kiszámítása).](./effective-unit-price-calculation.md)  | *0.03825* |
| UnitType (Egységtípus) | Az egység típusa, amelyben a fogyasztásmérő fel van számolva. | *1 GB/hónap* |
| AlternateId (Alternatívazonosító) | A hivatkozott rendelési sorelem alternatív azonosítója. | *6dc5c039750a* |
| BillableQuantity | A kiszámlázandó teljes mennyiség.  | *0.005001* |
| BillingFrequency | A vásárláskor kiválasztott számlázási csomag. | *NA*  |
| PricingCurrency | Az árlistán szereplő pénznem. | *USD* |
| PCToBCExchangeRate | A díjszabási pénznemre alkalmazott átváltási árfolyam a számlázási pénznemre. | *0.846202666* |
| PCToBCExchangeRateDate | Az a dátum, amelyen a számlázási pénznem árképzési pénzneme meg van határozva. | *2020. 09. 30.* |
| MeterDescription (Mérési leírás) | A mérő leírása.  | *Táblák – Tárolt LRS-adatok (GB/hónap)* |
| ReservationOrderId | A foglalási rendelés azonosítója. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | A kredit leírása. | *Azure-felhasználási kredit* |
| SubscriptionStartDate (Előfizetés kezdődátuma) | Az előfizetés vásárlásának dátuma. | *5/1/2021* |
| SubscriptionEndDate | Az előfizetés lejáratának dátuma. | *4/30/2022* |
| ReferenceID (Referenciaazonosító) | Az összekapcsolás a frissítések során történt összes tranzakcióval. | *025d68a6-1bd6-42ab-9636-15e8d776a30e* |
| ProductQualifiers | A bővítmény- vagy próbaverziós vásárlásokat ismerő azonosító. | *["Bővítmény"]* |
| PromotionID (Előléptetésazonosító) | Az előléptetési információk lekéréséhez használt azonosító. | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>Az Azure-használatot az egyszeres vásárlási recon fájlban egyeztetheti. Ehhez keresse meg a napi rendszerességgel minősített használat felderítési fájlját, és keresse meg a SubscriptionID-t. Ez megjeleníti az Azure-csomag azonosítójával kapcsolatos összes költséget. Az Azure SubscriptionID jogosultságazonosítóként jelenik meg.
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>Hogyan csatlakoztathatja az alap előfizetést a frissített előfizetéshez?

Az alaptermék előfizetés-azonosítójával keresse meg a megfelelő referenciaazonosítókat, és használja őket a kapcsolódó tranzakciók lekéréséhez. Az előfizetés-azonosítóval és a referencia-azonosítóval kombinálva egyetlen eseményen keresztül csatlakoztathatja az összes frissítést.

## <a name="next-steps"></a>Következő lépések

- [Számlázás és adók](billing.md)
