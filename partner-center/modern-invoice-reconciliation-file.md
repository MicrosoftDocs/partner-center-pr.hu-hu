---
title: Felderítési fájl mezői a CSP egyszeri vásárlásokhoz
ms.topic: conceptual
ms.date: 01/29/2021
description: Ismerje meg a CSP egyszeri beszerzési egyeztetési fájljának összes elemét a partner Centerben, beleértve a Sample értékeket is.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 74974c68c607ddcee4aff6abd53284a60653fb0b
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712256"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP egyszeri beszerzési egyeztetési fájl mezői

## <a name="using-the-recon-file"></a>A Recon-fájl használata
Az alábbi táblázat a CSP egyszeri vásárlások esetében az egyeztetési fájlban lévő mezők leírásait és mintáit tartalmazza.

Az egyeztetési fájlokkal kapcsolatos további információkért lásd: [a megbékélési fájlok használata](use-the-reconciliation-files.md).

| Oszlop | Leírás | Mintaérték |
| ------ | ----------- | ------------ |
| PartnerId | Egyedi azonosító GUID formátumban egy adott számlázási entitáshoz. Egyeztetéshez nem szükséges. Ugyanaz az összes sorban. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Az ügyfél egyedi Microsoft-azonosítója GUID formátumban. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Az ügyfél szervezetének neve, amelyet a partner Centerben jelentett. Ez az oszlop fontos a számla rendszer-információkkal való egyeztetéséhez. | *Johnny modern vevő DE2* |
| CustomerDomainName | Az ügyfél tartományneve. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Az az ország, ahol az ügyfele található. Tekintse meg a régió [országainak teljes listáját](./regional-authorization-overview.md) .  | *DE* |
| InvoiceNumber | Az egyeztetési fájllal társított számla száma.  | *G002297372* |
| MpnId | A CSP-partner MPN-azonosítója. További információ: [How to itemize by partner](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| ResellerMpnId | Az előfizetéshez tartozó rekord viszonteladójának MPN-azonosítója. | *6048879* |
| OrderId | Egy rendelés egyedi azonosítója a Microsoft számlázási platformon. Hasznos lehet a megrendelést azonosítani a támogatáshoz való kapcsolódáskor. Nem használatos egyeztetéshez. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | A megrendelés elhelyezésének dátuma. | *10/3/2020* |
| ProductId | A termék egyedi azonosítója. | *DZH318Z0BNZ5* |
| SkuId | Az SKU egyedi azonosítója. | *006G* |
| AvailabilityId | A rendelkezésre állás egyedi azonosítója. | *DZH318Z08B80* |
| SkuName | Az SKU neve. | *Táblák – LRS* |
| TermékNév | A termék neve. | *Táblák* |
| ChargeType | A [díj](./recon-file-charge-types.md) vagy a beállítás típusa. | *Új* |
| UnitPrice | Díj/licenc, a vásárlás időpontjában közzétett árlista szerint. Győződjön meg róla, hogy ez megegyezik a számlázási rendszeren tárolt információkkal az egyeztetés során. | *0,045* |
| Mennyiség | A licencek száma. Győződjön meg róla, hogy ez megegyezik a számlázási rendszeren tárolt információkkal az egyeztetés során. | *1* |
| Részösszeg | Adózás előtti összeg. A részösszegnek egyenlőnek kell lennie a számlázandó mennyiséggel, szorozva az egység érvényes árával. | *0* |
| TaxTotal | Adó összegének díja. A piaci adószabályok és a konkrét körülmények alapján. | *0* |
| Összesen | A teljes összeg egyenlő a részösszegtel és az adó összegével. | *0* |
| Pénznem | A számla az ügyfél pénznemének kontextusában jön létre. Ez azt jelenti, hogy ha Ön olyan partner, amely különböző számlázható pénznemekkel rendelkező ügyfelekkel rendelkezik, minden egyes ügyfél-pénznem típushoz számlát fog kapni.  | *EUR* |
| PriceAdjustmentDescription | Az egység árának módosításainak okai. Ezek a fő okok, de nem korlátozódnak a hatályos egység árának meghatározására. | *["15,0%-os partneri kredit a felügyelt szolgáltatások számára"]* |
| Közzétevő neve | A termék közzétevője.  | *Microsoft* |
| PublisherId | A partner Center által a közzétevő azonosítására használt egyedi azonosító. | *NA* |
| SubscriptionDescription | Az ügyfél által a árlista alapján megvásárolt szolgáltatási ajánlat neve. Ez az oszlop a OfferName azonos mezője. | *Azure-csomag* |
| SubscriptionId | Egy előfizetéshez tartozó egyedi azonosító a Microsoft számlázási platformon. Nem használatos egyeztetéshez. Vegye figyelembe, hogy ez az azonosító nem egyezik meg a partner felügyeleti konzol előfizetés-azonosítójával. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Az a dátum, amikor a partneri központ felszámítja az előfizetési díjat. Ha az előfizetést éves számlázási időszakra és havi számlázási csomagra vásárolja meg, akkor az első egyeztetési fájlban ez az a nap, amikor az előfizetés megvásárlásra kerül. A következő egyeztetési fájllal kezdődően a rendszer 30 nappal növeli a növekményt. | *9/1/2020* |
| ChargeEndDate | Az előfizetés számlázási ciklusára vonatkozó díjak befejezési napja. Ha az előfizetést éves számlázási időszakra és havi számlázási csomagra vásárolja meg, akkor az első egyeztetési fájlban ez az előfizetés megvásárlását követő 30. nap. A következő egyeztetési fájllal kezdődően a rendszer 30 nappal növeli a növekményt. | *2020. 09. 30.* |
| TermAndBillingCycle | A vásárlás időpontjában az előfizetés folytatásához szükséges időtartam. | *Tárolt adat (GB/hó)* |
| EffectiveUnitPrice | Az elszámolási egység díja a számlázási ciklus árának kiszámításához. A kedvezmények, a számlázási napok módosítása és más tényezők határozzák meg a hatályos egység árát. További információ: a [hatékony egység árának kiszámítása](./effective-unit-price-calculation.md).  | *0,03825* |
| UnitType | Az egység típusa, amelyben a mérőszámot terhelik. | *1 GB/hónap* |
| AlternateId | A hivatkozott rendeléssor-tétel alternatív azonosítója | *6dc5c039750a* |
| BillableQuantity | Az összes Számlázandó mennyiség.  | *0,005001* |
| BillingFrequency | A vásárlás időpontjában kiválasztott számlázási csomag. | *NA*  |
| PricingCurrency | Az árlistán szereplő pénznem. | *USD* |
| PCToBCExchangeRate | A díjszabási pénznemre alkalmazott Exchange-árfolyam a számlázási pénznemre. | *0,846202666* |
| PCToBCExchangeRateDate | Az a dátum, amikor az árképzési pénznemet meg kell határozni a számlázási pénznemben. | *2020. 09. 30.* |
| MeterDescription | Mérőműszer leírása.  | *Táblák – tárolt LRS-adatkészletek (GB/hó)* |
| ReservationOrderId | A foglalási rendelés azonosítója. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | A kredit leírása. | *Azure-beli felhasználási kredit* |

>[!NOTE]
>Az Azure-beli felhasználást az egyszeri vásárlási felderítési fájlban is összehangolhatja. Ehhez nyissa meg a napi értékelésű használati felderítési fájlt, és keresse meg a SubscriptionID. Ekkor megjelenik az Azure-csomag azonosítójával kapcsolatos összes költség. Az Azure-SubscriptionID EntitlementID jelenik meg.

## <a name="next-steps"></a>Következő lépések

- [Számlázás és adók](billing.md)
