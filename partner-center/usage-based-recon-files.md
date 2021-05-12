---
title: Használatalapú egyeztetési fájlok
ms.topic: article
ms.date: 06/08/2020
description: A használatalapú egyeztetési fájlban található összes elemet a Partnerközpont. Néhány példát is tartalmaz.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fc31915660b6a82954daee5fcc8fb2d5292e725c
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/12/2021
ms.locfileid: "109795006"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>A használatalapú egyeztetési fájlok és azok mezőinek Partnerközpont

**Megfelelő szerepkörök:** Fiók-rendszergazdai | Számlázási rendszergazda

A díjak ügyfélhasználattal való összevetéshez hasonlítsa össze az egyeztetési fájlban  található  **ResellerID,** **ResellerName**, és **ResellerBillableAccount** értékeket az ügyfél nevével és előfizetés-azonosítójával a Partnerközpont.

## <a name="fields-in-usage-based-reconciliation-files"></a>A használatalapú egyeztetési fájlok mezői

Az alábbi mezők a használt szolgáltatásokat és a díjakat ismertetik.

| Oszlop | Leírás | Mintaérték(ék) |
| ------ | ----------- | ------------ |
| Partnerazonosító | Partnerazonosító GUID formátumban. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | A partner neve. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Partnerfiók azonosítója. | *1010578050* |
| CustomerCompanyName (Ügyfél vállalatneve) | Az ügyfél szervezetének neve a Partnerközpont. *Nagyon fontos a számla és a rendszerinformációk egyeztetéséhez.* | *Ügyfél tesztelése* |
| MpnId | A CSP-partner MPN-azonosítója. | *4390934* |
| ResellerMpnId | Az előfizetés rekordjának viszonteladójának MPN-azonosítója.  |
| InvoiceNumber (Számlaszám) | Az a számlaszám, ahol a megadott tranzakció megjelenik. | *D020001IVK* |
| ChargeStartDate (Költségindításidátum) | A számlázási ciklus kezdő dátuma, kivéve a korábban fel nem használt rejtett használati adatok dátumának (az előző számlázási ciklusból) való bemutatja. Az időpont mindig a nap kezdete, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate (Költség és költségdátum) | A számlázási ciklus záró dátuma, kivéve a korábban fel nem használt rejtett használati adatok dátumának (az előző számlázási ciklusból) való bemutatja. Az idő mindig a nap vége, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Az előfizetés egyedi azonosítója a Microsoft számlázási platformon. Hasznos lehet azonosítani az előfizetést, amikor kapcsolatba lép az ügyfélszolgálattal. Az egyeztetéshez nincs használva. *Ez nem ugyanaz, mint a partner **felügyeleti** konzolján található előfizetés-azonosító.* | *usCBMgAAAAAAAAAIAA* |
| SubscriptionName | A szolgáltatásajánlat beceneve. | *Microsoft Azure* |
| SubscriptionDescription (Előfizetési leírás) | A szolgáltatásajánlat üzletága. | *Microsoft Azure* |
| OrderID | Rendelés egyedi azonosítója a Microsoft számlázási platformon. Hasznos lehet azonosítani az előfizetést, amikor kapcsolatba lép az ügyfélszolgálattal. Az egyeztetéshez nem használatos. | *566890604832738111* |
| ServiceName | A szóban forgó Azure-szolgáltatás neve. | *VIRTUÁLIS GÉPEK* |
| ServiceType | Az Azure-szolgáltatás adott típusa. | *Service Bus – Egyéni vagy csomag,* *SQL Azure-adatbázis – Business vagy Web Edition* |
| ResourceGuid (Erőforrás GUID azonosítója) | Az összes szolgáltatásadat és díjszabási struktúra egyedi azonosítója. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName nevű erőforrásáról | Az Azure-erőforrás neve. | *Adatátvitel a következőben: (GB)*, *adatátvitel ki (GB)* |
| Region | Az a régió, amelyre a használat vonatkozik. Elsősorban adatátviteli díjak hozzárendelésére használatos, mivel a díjszabás régiónként eltérő. | *Ázsia és a Csendes-óceáni térség*, *Európa,* *Latin-Amerika*, *Észak-Amerika* |
| SKU | Egy ajánlat egyedi Microsoft-azonosítója. | *7UD-00001* |
| DetailLineItemId (RészletekLineItemId) | Egy azonosító és egy mennyiség, amely egy adott számlázási időszakban különböző díjakat számláz ki egy adott szolgáltatásra vagy erőforrásra vonatkozóan. Az Azure rétegzett díjszabása legfeljebb bizonyos mennyiségű számlázható egység esetében lehet egy díjszabás, majd egy másik díj az adott mennyiség után. | *1* |
| ConsumedQuantity | A jelentéskészítési időszak alatt felhasznált szolgáltatás mennyisége (például óra vagy GB). A korábbi jelentéskészítési időszakokból származó nem kiszámlázatlan használatot is magában foglalja. | *11* |
| IncludedQuantity | Az ajánlat részeként foglalt egységek. Általában nem jelen van a CSP-ban. | *0* |
| OverageQuantity (Túl nagyság) | Az ajánlat részeként nem szereplő egységek. Ezeket a partnernek kell kifizetnie. Egyenlő **a ConsumedQuantity és az** **IncludedQuantity értékkel.** | *11* |
| ListPrice (Árlista) | Az ajánlat ára az előfizetés kezdő dátumán lép életbe. | *0,0808 USD* |
| PretaxCharges | Egyenlő **a ListPrist** és a **OverageQuantity** szorzatával, a legközelebbi centre kerekített értékkel. | *0,085 USD* |
| TaxAmount (TaxAmount) | Adó összege. A piac adózási szabályai és adott körülmények alapján. | *0,08 USD* |
| PostTaxTotal | Adó utáni teljes összeg, ha az adó alkalmazható. | *0,93 USD* |
| Pénznem | Pénznem típusa. Minden számlázási entitásnak csak egy pénzneme van. Ellenőrizze, hogy egyezik-e az első számlával, majd a számlázási platform frissítése után. | *EUR* |
| PretaxEffectiveRate (ElőaxEffectiveRate) | Egységenkénti adó előtti ár. Egyenlő a **PretaxCharges** **overageQuantity** értékével elosztva, a legközelebbi centre kerekített értékekkel. | *0,08 USD* |
| PostTaxEffectiveRate | Egységenkénti adókulcs. Egyenlő a **PostTaxTotal** és **a OverageQuantity** értékével, a legközelebbi centre kerekített értékével. Vagy egyenlő a **PretaxEffectiveRate értéktel** és az egységösszegenkénti adóval, a legközelebbi centre kerekített összeggel. | *0,08 USD* |
| ChargeType | A [díj vagy a módosítás](recon-file-charge-types.md) típusa. | Lásd [a díjtípusokat.](recon-file-charge-types.md) |
| CustomerId | Az ügyfél egyedi Microsoft-azonosítója GUID formátumban. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Az ügyfél tartományneve. Ez a mező a második számlázási ciklusig üresen is megjelenhet. | *example.onmicrosoft.com* |
| BillingCycleType (Számlázási ciklustípus) | Idő számlázási gyakorisága.| **Havonta**  |
| Unit (Egység) | Az erőforrás neve **egység.** | *GB* vagy *ÓRA* |
| CustomerBillableAccount | Egyedi fiókazonosító a Microsoft számlázási platformon. | *1280018095* |
| UsageDate | A szolgáltatás üzembe helyezésének dátuma. | *2/1/2019 0:00* |
| MeteredRegion | Azonosítja a régión belüli adatközpont helyét (olyan szolgáltatások esetén, ahol ez az érték alkalmazható és ki van töltve). | *Kelet-Ázsia,* *dél-Kelet-Ázsia,* *Észak-Európa,* *Nyugat-Európa,* USA északi középső régiója, *USA* *déli középső régiója* |
| MeteredService | Azonosítja az egyes Azure-szolgáltatások használatát, ha az nincs külön azonosítva a **ServiceName oszlopban.** Az adatátvitelek jelentése például a *következő: Microsoft Azure – Minden szolgáltatás* a **ServiceName oszlopban.** | *AccessControl,* *CDN,* *Compute,* *Database,* *ServiceBus,* *Storage* |
| MeteredServiceType | A **MeteredService mezőben** található további információ az Azure-szolgáltatások használatáról. | *Külső* |
| Project | A szolgáltatáspéldány ügyfél által megadott neve. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Az adott Azure Service Bus kiépített és használt kapcsolati kapcsolatok száma. | *1,000* 0000 kapcsolat / 30 nap (ha 30 napos hónapban egyénileg létesített kapcsolattal rendelkezik), *25 kapcsolat / 30 nap – Használva: 1.000000* (ha 25 csomag Service Bus-kapcsolattal rendelkezik, és 1-et használt az adott napon) |

## <a name="next-steps"></a>Következő lépések

- [A licencalapú egyeztetési Partnerközpont mezőinek a](license-based-recon-files.md)