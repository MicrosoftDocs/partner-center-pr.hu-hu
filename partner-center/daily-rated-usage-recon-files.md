---
title: Napi besorolású használati egyeztetési fájlok
ms.topic: article
ms.date: 06/12/2020
description: Ismerje meg, hogyan olvashatja el a napi rendszerességű használat egyeztetési fájljait a partner Centerben. A Recon-fájlban megadott mezők leírásait tartalmazza.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 531f28ae2bceed2d854c6fb139d0abb837a047b5
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712239"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Ismerje meg, hogyan olvashatja el a napi besorolású használat egyeztetési fájljait a partner Centerben

**A következőre érvényes:**

- Partnerközpont
- A Microsoft Cloud for US Government Partnerközpontja

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Számlázási adminisztrátor
- Értékesítési ügynök
- Segélyszolgálat ügynöke

Ez a cikk azt ismerteti, hogyan olvashatók be a napi rendszerességű használati egyeztetési fájlok.

>[!NOTE]
>A napi névleges használat általában 24 órát vesz igénybe a partner Centerben, vagy az API-n keresztül érhető el.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>A napi rendszerességgel értékelt használati egyeztetési fájlok mezői

| Oszlop | Leírás |
| ------ | ----------- |
| PartnerId | A partner azonosítója GUID formátumban. |
| PartnerName | A partner neve. |
| CustomerId | Az ügyfél egyedi Microsoft-azonosítója GUID formátumban. |
| CustomerName | Az ügyfél szervezetének neve, amelyet a partner Centerben jelentett. *Ez az oszlop fontos a számla rendszer-információkkal való egyeztetéséhez.* |
| CustomerDomainName | Az ügyfél tartományának neve. |
| CustomerCountry | Az az ország, amelyben az ügyfél található. |
| MpnId | A CSP-partner MPN-azonosítója. |
| Tier2MpnId | Az előfizetéshez tartozó rekord viszonteladójának MPN-azonosítója. |
| InvoiceNumber | A megadott tranzakciót tartalmazó számla száma. |
| ProductId | A termék azonosítója. |
| SkuId | Egy adott SKU azonosítója. |
| AvailabilityId | Egy adott SKU rendelkezésre állásának azonosítója. Ebben az oszlopban látható, hogy az SKU megvásárolható-e az adott országban, pénznemben, iparági szegmensben stb. |
| SkuName | Egy adott SKU címe. |
| TermékNév | A termék neve. |
| Közzétevő neve | A közzétevő neve. |
| PublisherId | A közzétevő azonosítója GUID formátumban. |
| SubscriptionDescription | Az ügyfél által a árlista alapján megvásárolt szolgáltatási ajánlat neve. (Ez az oszlop a **OfferName** azonos mezője.) |
| SubscriptionId | Egy előfizetéshez tartozó egyedi azonosító a Microsoft számlázási platformon. Nem használatos egyeztetéshez. *Ez az azonosító nem egyezik meg a partner felügyeleti konzol **előfizetés-azonosítójával** .* |
| ChargeStartDate | A számlázási ciklus kezdő dátuma (kivéve, ha az előző számlázási ciklusból korábban nem feltöltött látens használati adatok dátumát mutatja be). Az időpont mindig a nap kezdete, 0:00. |
| ChargeEndDate | A számlázási ciklus befejező dátuma (kivéve, ha az előző számlázási ciklusból korábban nem feltöltött látens használati adatok dátumát mutatja be). Az idő mindig a nap vége, 23:59. |
| UsageDate | A szolgáltatás használatának dátuma. |
| MeterType | A fogyasztásmérő típusa. |
| MeterCategory | A használathoz tartozó legfelső szintű szolgáltatás. |
| MeterId | A használt fogyasztásmérő azonosítója. |
| MeterSubCategory | Az Azure-szolgáltatás típusa, amely hatással lehet a díjszabásra. |
| MeterName | A felhasznált fogyasztásmérő mértékegysége. |
| MeterRegion | Ez az oszlop azonosítja a régión belüli adatközpont helyét azon szolgáltatások esetében, ahol a MeterRegion alkalmazható és fel van töltve. |
| Unit (Egység) | Az erőforrás **nevének** egysége. |
| ResourceLocation | Az az adatközpont, amelyben a fogyasztásmérő fut. |
| ConsumedService | Az Azure platform szolgáltatás, amelyet használt. |
| ResourceGroup | Egy olyan tárolót jelöl, amely egy Azure-megoldáshoz kapcsolódó erőforrásokat tárol. |
| ResourceURI | A használt erőforrás URI-ja. |
| ChargeType | A díj vagy módosítás típusa.  |
| UnitPrice | Díj/licenc, a vásárlás időpontjában közzétett árlista szerint. Ellenőrizze, hogy ez az ár megfelel-e a számlázási rendszeren tárolt információknak az egyeztetés során. |
| Mennyiség | A licencek száma. Ellenőrizze, hogy ez az ár megfelel-e a számlázási rendszeren tárolt információknak az egyeztetés során. |
| UnitType | Annak az egységnek a típusa, amelyre a mérőszámot fel kell tölteni.  |
| BillingPreTaxTotal | Az összes számlázási összeg az adók előtt.<br/> _**BillingPreTaxTotal** = floor (([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Az ügyfél földrajzi régiójában lévő pénznem. |
| PricingPreTaxTotal | A díjszabás az adók hozzáadása előtt történik. |
| PricingCurrency | Az árlistán szereplő pénznem. |
| ServiceInfo1 | Az adott napon kiépített és felhasznált Service Bus kapcsolatok száma. |
| ServiceInfo2 | Egy örökölt mező, amely a választható szolgáltatásokra vonatkozó metaadatokat rögzíti. |
| Címkék | A felhasználó által beállított Azure-erőforrások logikai szervezetét jelöli. |
| AdditionalInfo | Bármely további információ, amelyet a többi oszlop nem tartalmaz. |
| EffectiveUnitPrice | Az egységenként felszámított tényleges érték, beleértve a kedvezményeket, a megszerzett krediteket és így tovább. |
| PCToBCExchangeRate | A díjszabási pénznemre alkalmazott Exchange-árfolyam a számlázási pénznemhez képest. |
| PCToBCExchangeRateDate | Az a dátum, amikor az árképzési pénznemet meg kell határozni a számlázási pénznemben. |
| EntitlementId | Az Azure-előfizetés AZONOSÍTÓját jelöli. |
| EntitlementDescription | Az Azure-előfizetési azonosító nevét jelöli. |
| PartnerEarnedCreditPercentage | Megjeleníti a sorhoz tartozó PartnerEarnedCredit. A keresett kredit 0 vagy 15 százalék lesz |
| CreditPercentage | Az Azure-beli felhasználási kreditet jeleníti meg. A keresett kredit 0 vagy 100 százalék lesz. |
| CreditType | A kredit típusa. Például az **Azure Credit alkalmazása.** |
>[!NOTE]
>A napi névleges használat általában 24 órát vesz igénybe a partner Centerben, vagy az API-n keresztül érhető el.


