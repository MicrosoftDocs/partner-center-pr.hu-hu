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
ms.openlocfilehash: 6c486d4866b0a2a912801d2648a1822418687078
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431697"
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
| CustomerCompanyName (Ügyfél vállalatneve) | Az ügyfél szervezetének neve a Partnerközpont. *Ez nagyon fontos a számla és a rendszerinformációk egyeztetéséhez.* | *Ügyfél tesztelése* |
| MpnId | Microsoft Partner Network (MPN) azonosítóját a Felhőszolgáltató (CSP) partnerhez. | *4390934* |
| ResellerMpnId (Viszonteladóimpn-azonosító) | Az előfizetés rekordjának viszonteladójának MPN-azonosítója.  |
| InvoiceNumber (Számlaszám) | Az a számlaszám, ahol a megadott tranzakció megjelenik. | *D020001IVK* |
| ChargeStartDate (Díjindításidátum) | A számlázási ciklus kezdő dátuma, kivéve a korábban fel nem használt rejtett használati adatok dátumának (az előző számlázási ciklusból) való bemutatja. Az időpont mindig a nap kezdete, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate (Költség és költségdátum) | A számlázási ciklus záró dátuma, kivéve a korábban fel nem használt rejtett használati adatok dátumának (az előző számlázási ciklusból) való bemutatja. Az idő mindig a nap vége, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Előfizetés egyedi azonosítója a Microsoft számlázási platformon. Hasznos lehet azonosítani az előfizetést, amikor kapcsolatba lép az ügyfélszolgálattal. Az egyeztetéshez nem használatos. *Ez nem ugyanaz, mint a **partner-felügyeleti** konzolon található előfizetés-azonosító.* | *usCBMgAAAAAAAAAIA* |
| SubscriptionName | A szolgáltatásajánlat beceneve. | *Microsoft Azure* |
| SubscriptionDescription (Előfizetési leírás) | A szolgáltatásajánlat üzletága. | *Microsoft Azure* |
| OrderID | Rendelés egyedi azonosítója a Microsoft számlázási platformon. Hasznos lehet azonosítani az előfizetést, amikor kapcsolatba lép az ügyfélszolgálattal. Az egyeztetéshez nem használatos. | *566890604832738111* |
| ServiceName | A szóban forgó Azure-szolgáltatás neve. | *VIRTUÁLIS GÉPEK* |
| ServiceType | Az Azure-szolgáltatás adott típusa. | *Service Bus – Egyéni vagy csomag,* *SQL Azure-adatbázis – Business vagy Web Edition* |
| ResourceGuid (Erőforrás GUID azonosítója) | Az összes szolgáltatásadat és díjszabási struktúra egyedi azonosítója. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName nevű erőforrásáról | Az Azure-erőforrás neve. | *Adatátvitel a következőben: (GB)*, *adatátvitel ki (GB)* |
| Region | Az a régió, amelyre a használat vonatkozik. Elsősorban adatátviteli díjak hozzárendelésére használatos, mivel a díjszabás régiónként eltérő. | *Ázsia és a Csendes-óceáni térség*, *Európa,* *Latin-Amerika*, *Észak-Amerika* |
| SKU | Egy ajánlat egyedi Microsoft-azonosítója. | *7UD-00001* |
| DetailLineItemId (RészleteklineItemId) | Egy azonosító és egy mennyiség, amely egy adott számlázási időszakban egy szolgáltatás vagy erőforrás különböző díjszabását tartalmazza. Az Azure-rétegzett díjszabás esetében egy díj legfeljebb bizonyos mennyiségű számlázható egységre lehet kiszámlázható, majd egy másik díj az adott mennyiség után. | *1* |
| ConsumedQuantity | A jelentéskészítési időszak alatt felhasznált szolgáltatás mennyisége (például óra vagy GB). A korábbi jelentéskészítési időszakokból származó nem kiszámlázatlan használatot is magában foglalja. | *11* |
| IncludedQuantity | Az ajánlat részeként foglalt egységek. Általában nem jelen van a CSP-ban. | *0* |
| OverageQuantity | Az ajánlat részeként nem szereplő egységek. Ezeket a partnernek kell kifizetnie. Egyenlő **a ConsumedQuantity értékkel és** **az IncludedQuantity értékkel.** | *11* |
| ListPrice (Listaár) | Az ajánlat ára az előfizetés kezdő dátumán lép életbe. | *0,0808 USD* |
| PretaxCharges | Egyenlő **a ListPrist** és az **OverageQuantity** szorzatával, a legközelebbi centre kerekített értékkel. | *0,085 USD* |
| TaxAmount (TaxAmount) | Adó összege. A piac adózási szabályai és adott körülmények alapján. | *0,08 USD* |
| PostTaxTotal (PostTaxTotal) | Adó utáni összeg, ha alkalmazható adó. | *0,93 USD* |
| Pénznem | Pénznem típusa. Minden számlázási entitásnak csak egy pénzneme van. Ellenőrizze, hogy egyezik-e az első számlával, majd a számlázási platform jelentős frissítései után. | *EUR* |
| PretaxEffectiveRate (ElőaxEffectiveRate) | Egységenkénti adó előtti ár. Egyenlő **a PretaxCharges** és a **OverageQuantity** osztva a legközelebbi centre kerekített értékével. | *0,08 USD* |
| PostTaxEffectiveRate | Egységenkénti adóárak után. Egyenlő a **PostTaxTotal** érték és a **OverageQuantity** osztálva, a legközelebbi centre kerekített értékével. Vagy megegyezik a **PretaxEffectiveRate** értéknek és az egységösszegenkénti adókulcsnak a legközelebbi centre kerekített értékén. | *0,08 USD* |
| ChargeType | A [díj vagy a módosítás](recon-file-charge-types.md) típusa. | Lásd: [Díjtípusok.](recon-file-charge-types.md) |
| CustomerId | Az ügyfél egyedi Microsoft-azonosítója GUID formátumban. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Az ügyfél tartományneve. Ez a mező a második számlázási ciklusig üresen is megjelenhet. | *example.onmicrosoft.com* |
| BillingCycleType (Számlázási ciklustípus) | Idő számlázási gyakorisága.| **Havonta**  |
| Unit (Egység) | Az erőforrás neve **egység.** | *GB* vagy *ÓRA* |
| CustomerBillableAccount | Egyedi fiókazonosító a Microsoft számlázási platformon. | *1280018095* |
| UsageDate | A szolgáltatás üzembe helyezésének dátuma. | *2/1/2019 0:00* |
| MeteredRegion | Azonosítja a régión belüli adatközpont helyét (olyan szolgáltatások esetén, ahol ez az érték alkalmazható és ki van töltve). | *Kelet-Ázsia,* *dél-Kelet-Ázsia,* *Észak-Európa,* *Nyugat-Európa,* USA északi középső régiója, *USA* *déli középső régiója* |
| MeteredService | Azonosítja az egyes Azure-szolgáltatások használatát, ha az nincs külön azonosítva a **ServiceName oszlopban.** Az adatátvitelek jelentése például a *következő: Microsoft Azure – Minden szolgáltatás* a **ServiceName oszlopban.** | *AccessControl,* *CDN,* *Compute,* *Database,* *ServiceBus,* *Storage* |
| MeteredServiceType (MeteredServiceType) | A **MeteredService mezőben** található, amely további tisztázást biztosít az Azure-szolgáltatások használatáról. | *Külső* |
| Project | A szolgáltatáspéldány ügyfél által megadott neve. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Az adott Azure Service Bus kiépített és használt kapcsolatok száma. | *1,000* 0000 kapcsolat / 30 nap (ha 30 napos hónapon belül egyénileg létesített kapcsolattal rendelkezik), *25 Kapcsolat / 30 nap – Használt: 1.000000* (ha 25 csomag kiépített Service Bus-kapcsolattal rendelkezik, és 1-et használt az adott napon) |

## <a name="next-steps"></a>Következő lépések

- [A licencalapú egyeztetési Partnerközpont mezőinek a](license-based-recon-files.md)