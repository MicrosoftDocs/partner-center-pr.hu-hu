---
title: Használaton alapuló egyeztetési fájlok
ms.topic: article
ms.date: 06/08/2020
description: Ismerje meg a partner Center használaton alapuló egyeztetési fájljának összes elemét. Néhány példát is tartalmaz.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a1a2707b12e4bdb7452711019aa8ae43d4b6b1a
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022757"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>A használaton alapuló egyeztetési fájlok és a partnervállalat konkrét mezőinek megismerése

**Megfelelő szerepkörök**

- Fiókadminisztrátor
- Számlázási adminisztrátor

Ha egyeztetni kívánja az ügyfelek használati feladatait, hasonlítsa össze a **ResellerID**, a **viszonteladó neve** és a **ResellerBillableAccount** az egyeztetési fájlból a partner Center **ügyfél** -és **előfizetés-azonosítójával** .

## <a name="fields-in-usage-based-reconciliation-files"></a>Mezők a használaton alapuló egyeztetési fájlokban

Az alábbi mezőkből megtudhatja, hogy mely szolgáltatásokat használták, és milyen arányban.

| Oszlop | Leírás | Minta értéke (i) |
| ------ | ----------- | ------------ |
| PartnerId | A partner azonosítója GUID formátumban. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | A partner neve. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Partner-fiókazonosító. | *1010578050* |
| CustomerCompanyName | Az ügyfél szervezetének neve, ahogy az a partner Centerben szerepel. *Nagyon fontos a számla egyeztetéséhez a rendszeradatokkal.* | *Ügyfél tesztelése* |
| MpnId | A CSP-partner MPN-azonosítója. | *4390934* |
| ResellerMpnId | Az előfizetéshez tartozó rekord viszonteladójának MPN-azonosítója.  |
| InvoiceNumber | A megadott tranzakciót tartalmazó számla száma. | *D020001IVK* |
| ChargeStartDate | A számlázási ciklus kezdő dátuma, kivéve, ha a korábban nem feltöltött látens használati adatok dátumát mutatja (az előző számlázási ciklusból). Az időpont mindig a nap kezdete, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | A számlázási ciklus befejező dátuma, kivéve, ha a korábban nem feltöltött látens használati adatok dátumát jeleníti meg (az előző számlázási ciklusból). Az idő mindig a nap vége, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Egy előfizetéshez tartozó egyedi azonosító a Microsoft számlázási platformon. Hasznos lehet azonosítani az előfizetést, amikor kapcsolatba lép a támogatási szolgálattal. Nem használatos egyeztetéshez. *Ez nem egyezik meg a partner felügyeleti konzol **előfizetés-azonosítójával** .* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | A szolgáltatási ajánlat beceneve. | *Microsoft Azure* |
| SubscriptionDescription | A szolgáltatási ajánlat üzletága. | *Microsoft Azure* |
| OrderID | Egy rendelés egyedi azonosítója a Microsoft számlázási platformon. Hasznos lehet azonosítani az előfizetést, amikor kapcsolatba lép a támogatási szolgálattal. Nem használatos egyeztetéshez. | *566890604832738111* |
| ServiceName | A kérdéses Azure-szolgáltatás neve. | *VIRTUÁLIS GÉPEK* |
| ServiceType | Az Azure-szolgáltatás adott típusa. | *Service Bus – egyéni vagy csomag*, *SQL Azure adatbázis – üzleti vagy webes kiadás* |
| ResourceGuid (Erőforrás GUID azonosítója) | A szolgáltatás összes adatának és árképzési struktúrájának egyedi azonosítója. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName nevű erőforrásáról | Az Azure-Erőforrás neve. | *Adatátvitel (GB)*, *kimenő adatforgalom (GB)* |
| Region | Az a régió, amelyre a használat vonatkozik. Elsődlegesen az adatátviteli díjak kiosztására szolgálnak, mivel a díjszabás régiónként eltérő. | *Ázsia és a csendes-óceáni térség*, *Európa*, *Latin-Amerika*, *Észak-Amerika* |
| SKU | Egyedi Microsoft-azonosító egy ajánlathoz. | *7UD – 00001* |
| DetailLineItemId | Egy adott számlázási időszakban egy szolgáltatás vagy erőforrás különböző díjszabását itemize azonosító és mennyiség. Az Azure-előállítók díjszabása esetében előfordulhat, hogy egy adott mennyiségű számlázható egységhez legfeljebb egy díjat számítunk fel. | *1* |
| ConsumedQuantity | A jelentési időszak alatt felhasznált szolgáltatás mennyisége (például óra vagy GB). A korábbi jelentési időszakok nem számlázott használatát is magában foglalja. | *11* |
| IncludedQuantity | Az ajánlat részét képező egységek. Általában nem szerepel a CSP-ben. | *0* |
| OverageQuantity | Az ajánlat részeként nem szereplő egységek. Ezeket a partnernek kell fizetnie. Egyenlő a **ConsumedQuantity** mínusz **IncludedQuantity**. | *11* |
| ListPrice | Az előfizetés kezdő dátumánál érvényes ár. | *$0,0808* |
| PretaxCharges | Egyenlő a **ListPrist** megszorozva a **OverageQuantity**, a legközelebbi%-ra kerekítve. | *$0,085* |
| TaxAmount | A fizetendő adó összege. A piaci adószabályok és a konkrét körülmények alapján. | *$0,08* |
| PostTaxTotal | ÁFA után összesen, ha az adó érvényes. | *$0,93* |
| Pénznem | Pénznem típusa Minden számlázási entitásnak csak egy pénzneme van. Győződjön meg arról, hogy az megfelel az első számlájának, majd a főbb számlázási platformok frissítései után. | *EUR* |
| PretaxEffectiveRate | Egységenkénti ÁFA díj. Egyenlő a **PretaxCharges** osztva **OverageQuantity**, a legközelebbi%-ra kerekítve. | *$0,08* |
| PostTaxEffectiveRate | Adózás utáni díj egységenként. Egyenlő a **PostTaxTotal** osztva **OverageQuantity**, a legközelebbi%-ra kerekítve. Vagy egyenlő a **PretaxEffectiveRate** és az egységenkénti adókulcs összegével, a legközelebbi%-ra kerekítve. | *$0,08* |
| ChargeType | A [díj](recon-file-charge-types.md) vagy a beállítás típusa. | Tekintse meg a [díjszabási típusokat](recon-file-charge-types.md). |
| CustomerId | Az ügyfél egyedi Microsoft-azonosítója GUID formátumban. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Az ügyfél tartományneve. Ez a mező üresen jelenhet meg a második számlázási ciklusig. | *example.onmicrosoft.com* |
| BillingCycleType | Az idő számlázási gyakorisága.| **Havonta**  |
| Unit (Egység) | Az erőforrás **nevének** egysége. | *GB* vagy *óra* |
| CustomerBillableAccount | Egyedi fiókazonosító a Microsoft számlázási platformon. | *1280018095* |
| UsageDate | A szolgáltatás központi telepítésének dátuma. | *2/1/2019 0:00* |
| MeteredRegion | Meghatározza egy adatközpont helyét a régión belül (azon szolgáltatások esetében, amelyeknél ez az érték alkalmazható és fel van töltve). | *Kelet-Ázsia*, *Dél-Kelet-Ázsia*, *Észak-Európa*, *Nyugat-Európa*, az *USA északi középső* régiója, az *USA déli középső* régiója |
| MeteredService | Azonosítja az egyes Azure-szolgáltatások használatát, ha a **szolgáltatásnév** oszlopban nem kifejezetten van meghatározva. Az adatátvitelek például *Microsoft Azure – minden szolgáltatásként* jelennek meg a **szolgáltatásnév** oszlopban. | *AccessControl*, *CDN*, *számítási*, *adatbázis*, *ServiceBus*, *Storage* |
| MeteredServiceType | Az Azure-szolgáltatások használatának további tisztázását biztosító **MeteredService** mező alcíme. | *KÜLSŐ* |
| Project | A szolgáltatási példány ügyfél által definiált neve. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Az adott napon kiosztott és felhasznált Azure Service Bus kapcsolatok száma. | *1,000000 kapcsolat/30 nap* (ha egy 30 napos hónap alatt külön kiosztott kapcsolatra volt szükség), *25 kapcsolat/30 nap – használatban: 1,000000* (ha 25 csomaggal rendelkezett Service Bus-kapcsolat kiosztott, és az adott napon 1. |

## <a name="next-steps"></a>Következő lépések

- [A partner Center licenc-alapú egyeztető fájljaiban található mezők ismertetése](license-based-recon-files.md)