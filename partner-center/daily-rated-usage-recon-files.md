---
title: Napi minősítésű használat egyeztetési fájljai
ms.topic: article
ms.date: 06/12/2020
description: Ismerje meg, hogyan olvashatja el a napi minősített használat egyeztetési fájljait a Partnerközpont. A recon fájl adott mezőinek leírását tartalmazza.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9b5daf91646324a9d4ace92d25736cfd0361ad6c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147275"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Ismerje meg, hogyan olvashatja el a napi minősített használat egyeztetési fájljait a Partnerközpont

**A következőkre vonatkozik:** Partnerközpont | Partnerközpont a Microsoft Cloud for US Government

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Értékesítési ügynök | Helpdesk agent

Ez a cikk a napi minősített használat egyeztetési fájljainak olvasását ismerteti.

>[!NOTE]
>A napi névleges használat általában 24 órát vesz igénybe a Partnerközpont vagy az API-n keresztüli elérése.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>A napi minősítésű használat egyeztetési fájljainak mezői

| Oszlop | Leírás |
| ------ | ----------- |
| Partnerazonosító | Partnerazonosító GUID formátumban. |
| PartnerName | A partner neve. |
| CustomerId | Az ügyfél egyedi Microsoft-azonosítója GUID formátumban. |
| CustomerName | Az ügyfél szervezetének neve a Partnerközpont. *Ez az oszlop fontos a számla és a rendszerinformációk egyeztetéséhez.* |
| CustomerDomainName (Ügyféltartományneve) | Az ügyfél tartományneve. |
| CustomerCountry (Ügyfél országa) | Az az ország, amelyben az ügyfél található. |
| MpnId | A CSP-partner MPN-azonosítója. |
| Tier2MpnId (2. rétegbelimpnazonosító) | Az előfizetés rekordjának viszonteladójának MPN-azonosítója. |
| InvoiceNumber (Számlaszám) | Az a számlaszám, ahol a megadott tranzakció megjelenik. |
| ProductId | A termék azonosítója. |
| SkuId (Termékváltozatazonosító) | Egy adott termékváltozat azonosítója. |
| AvailabilityId (Rendelkezésre állásiid) | Egy adott termékváltozat rendelkezésre állásának azonosítója. Ez az oszlop azt mutatja, hogy a termékváltozat megvásárolható-e az adott országban, pénznemben, iparági szegmensben stb. |
| SkuName | Egy adott termékváltozat címe. |
| TermékNév | A termék neve. |
| Közzétevő neve | A közzétevő neve. |
| PublisherId | A közzétevő GUID formátumú azonosítója. |
| SubscriptionDescription (Előfizetési leírás) | Az ügyfél által megvásárolt szolgáltatásajánlat neve az árlistában meghatározottak szerint. (Ez az oszlop megegyezik az **OfferName mezővel).** |
| SubscriptionId | Előfizetés egyedi azonosítója a Microsoft számlázási platformon. Az egyeztetéshez nem használatos. *Ez az azonosító nem ugyanaz, mint a partner felügyeleti konzolján található előfizetés-azonosító.* |
| ChargeStartDate (Költségindításidátum) | A számlázási ciklus kezdő dátuma (kivéve, ha az előző számlázási ciklusból származó, korábban fel nem használt rejtett használati adatok dátumát mutatja be). Az időpont mindig a nap kezdete, 0:00. |
| ChargeEndDate (Költség és költségdátum) | A számlázási ciklus záró dátuma (kivéve, ha az előző számlázási ciklusból származó, korábban fel nem használt rejtett használati adatok dátumát mutatja be). Az idő mindig a nap vége, 23:59. |
| UsageDate | A szolgáltatás használatának dátuma. |
| MeterType (Mérőtípus) | A fogyasztásmérő típusa. |
| MeterCategory | A használathoz tartozó legfelső szintű szolgáltatás. |
| MeterId | A használt fogyasztásmérő azonosítója. |
| MeterSubCategory | Az Azure-szolgáltatás típusa, amely befolyásolhatja a díjszabást. |
| MeterName | A felhasznált fogyasztásmérő mértékegysége. |
| MeterRegion | Ez az oszlop azonosítja az adatközpont helyét abban a régióban, ahol a MeterRegion alkalmazható és ki van töltve. |
| Unit (Egység) | Az erőforrás neve **egység.** |
| ResourceLocation | Az adatközpont, ahol a fogyasztásmérő fut. |
| ConsumedService | Az Ön által használt Azure platformszolgáltatás. |
| ResourceGroup | Egy azure-megoldáshoz kapcsolódó erőforrásokat tároló tárolót képvisel. |
| ResourceURI | A használt erőforrás URI-ját. |
| ChargeType | A díj vagy módosítás típusa.  |
| UnitPrice | Licencenkénti ár, amely a vásárláskor az árlistában van közzétéve. Győződjön meg arról, hogy ez az ár megegyezik a számlázási rendszerben az egyeztetés során tárolt adatokkal. |
| Mennyiség | Licencek száma. Győződjön meg arról, hogy ez az ár megegyezik a számlázási rendszerben az egyeztetés során tárolt adatokkal. |
| UnitType (Egységtípus) | Az egység típusa, amelynél a fogyasztásmérő fel van számolva.  |
| BillingPreTaxTotal | Az adók előtti teljes számlázási összeg.<br/> _**BillingPreTaxTotal** = FLOOR(([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Az ügyfél földrajzi régiójának pénzneme. |
| PricingPreTaxTotal | Az adók hozzáadása előtti díjszabás. |
| PricingCurrency | Az árlistán szereplő pénznem. |
| ServiceInfo1 | Az adott Service Bus kiépített és használt kapcsolati kapcsolatok száma. |
| ServiceInfo2 | Egy örökölt mező, amely nem kötelező szolgáltatásspecifikus metaadatokat rögzít. |
| Címkék | A felhasználó által beállított Azure-erőforrások logikai rendszerét jelöli. |
| AdditionalInfo | Bármely további információ, amelyet a többi oszlop nem tartalmaz. |
| EffectiveUnitPrice (Hatályos egységár) | Az egységenként felszámított tényleges érték, beleértve az esetleges kedvezményeket, a jóváírást stb. |
| PCToBCExchangeRate | A díjszabási pénznemre alkalmazott árfolyam a számlázási pénznemre. |
| PCToBCExchangeRateDate | Az a dátum, amelyen a számlázási pénznem árképzési pénzneme meg van határozva. |
| EntitlementId (Jogosultságazonosító) | Az Azure-előfizetés azonosítóját jelöli. |
| EntitlementDescription (Jogosultságleíró) | Az Azure-előfizetés azonosítójának nevét jelöli. |
| PartnerEarnedCreditPercentage | Megjeleníti a sorelem PartnerEarnedCredit elemét. A jóváírás 0 vagy 15% lehet |
| CreditPercentage | Megjeleníti az Azure-felhasználási kreditet. A jóváírás 0 vagy 100% lehet. |
| CreditType (Kredittípus) | A kredit típusa. Például: **Azure-kredit alkalmazva.** |
>[!NOTE]
>A napi névleges használat általában 24 órát vesz igénybe, Partnerközpont API-n keresztül jelennek meg.


