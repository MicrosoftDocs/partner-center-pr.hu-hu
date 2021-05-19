---
title: Licencalapú egyeztetési fájlok
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan olvashatja el a licencalapú egyeztetési fájlokat a Partnerközpont. Ez a cikk a licencalapú felderítési fájl egyes mezőinek jelentését ismerteti.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 041f0fadfea107027ae1d9796d235700e66e6834
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146578"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>A licencalapú egyeztetési Partnerközpont mezőinek a

**A következőkre vonatkozik:** Partnerközpont | Partnerközpont a Microsoft Cloud for US Government

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Számlázási rendszergazdai | Rendszergazdai ügynök

Ha a módosításokat össze kell egyeztetni egy ügyfél rendelésével,  hasonlítsa össze az egyeztetési **Syndication_Partner_Subscription_Number** és az ügyfél előfizetés-Partnerközpont.

## <a name="fields-in-license-based-reconciliation-files"></a>A licencalapú egyeztetési fájlok mezői

| Oszlop | Leírás | Mintaérték |
| ------ | ----------- | ------------ |
| Partnerazonosító | Egyedi azonosító GUID formátumban egy adott számlázási entitáshoz. Az egyeztetéshez nem szükséges. Minden sorban ugyanaz. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Az ügyfél egyedi Microsoft-azonosítója GUID formátumban. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Az ügyfél szervezetének neve a Partnerközpont. *Nagyon fontos mező a számla és a rendszerinformációk egyeztetéséhez.* | *A ügyfél tesztelése* |
| MpnId | A CSP-partner MPN-azonosítója. Tekintse [meg, hogyan elemet ad meg partner szerint.](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *4390934* |
| ResellerMpnId (Viszonteladóimpn-azonosító) | Az előfizetés rekordjának viszonteladójának MPN-azonosítója.  |
| OrderId | Rendelés egyedi azonosítója a Microsoft számlázási platformon. Hasznos lehet azonosítani a rendelést, amikor kapcsolatba lép az ügyfélszolgálattal. Az egyeztetéshez nem használatos. | *566890604832738111* |
| SubscriptionId | Előfizetés egyedi azonosítója a Microsoft számlázási platformon. Hasznos lehet azonosítani az előfizetést, amikor kapcsolatba lép az ügyfélszolgálattal. Az egyeztetéshez nem használatos. *Ez az érték nem  ugyanaz, mint a Partner admin console előfizetés-azonosítója. Ehelyett tekintse meg a **SyndicationPartnerSubscriptionNumber függvényt.*** | *usCBMgAAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Az előfizetések egyedi azonosítója. Egy ügyfél több előfizetéssel is rendelkezik ugyanannak a csomagnak. Ez az oszlop fontos az egyeztetési fájlelemzéshez. Ez a mező a Partner admin **console előfizetés-azonosítójára** van leképezve. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId (Ajánlatazonosító) | Egyedi ajánlatazonosító. Az árlistában meghatározott szabványos ajánlatazonosító. *Ez az érték nem egyezik meg az **árlistán található** ajánlatazonosítóval. Lásd **ehelyett a DurableOfferID függvényt.*** | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId (TartósofferId) | Az árlistában meghatározott egyedi tartósajánlat-azonosító. *Ez az érték megegyezik **az árlistán** található ajánlatazonosítóval.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Az ügyfél által megvásárolt szolgáltatásajánlat neve az árlistában meghatározottak szerint. | *Microsoft Office 365-ös (E3 csomag)* |
| SubscriptionStartDate (Előfizetés kezdődátum) | Az előfizetés kezdési dátuma (UTC). Az időpont mindig a nap kezdete, 0:00. Ez a mező a rendelés elküld utáni napra van beállítva. A **SubscriptionEndDate** értékével együtt használva határozza meg, hogy az ügyfél még az előfizetés első évében van-e, vagy hogy az előfizetést a következő évre újították-e meg. | *2/1/2019 0:00* |
| SubscriptionEndDate (Előfizetési időszak) | Az előfizetés záró dátuma (UTC). Az időpont mindig a nap kezdete, 0:00. A partner számlázási dátumához igazodva *12* hónappal és x nappal a kezdési dátum után, vagy 12 hónappal a megújítás *dátumához képest.* A megújításkor az árak az aktuális árlistára frissülnek. Az automatikus megújítás előtt szükség lehet az ügyfelek kommunikációra. | *2/1/2019 0:00* |
| ChargeStartDate (Díjindításidátum) | A díjak kezdő napja. Az időpont mindig a nap kezdete, 0:00. A napi díjak *(pro-díjak) kiszámítására* használatos, amikor egy ügyfél módosítja a licencszámokat. | *2/1/2019 0:00* |
| ChargeEndDate (Költség és költségdátum) | A díjak záró napja. Az idő mindig a nap vége, 23:59. A napi díjak *(pro-díjak) kiszámítására* használatos, amikor egy ügyfél módosítja a licencszámokat. | *2/28/2019 23:59* |
| ChargeType | A [díj vagy a módosítás](recon-file-charge-types.md) típusa. | Lásd [a díjtípusokat.](recon-file-charge-types.md) |
| UnitPrice | Licencenkénti ár, amely a vásárláskor az árlistában van közzétéve. Győződjön meg arról, hogy ezek megegyeznek a számlázási rendszerben az egyeztetés során tárolt adatokkal. | *6.82* |
| Mennyiség | Licencek száma. Győződjön meg arról, hogy ezek megegyeznek a számlázási rendszerben az egyeztetés során tárolt adatokkal. | *2* |
| Összeg | Mennyiség árának teljes összege. Annak ellenőrzésével ellenőrzi, hogy az összeg kiszámítása megfelel-e az ügyfelek számára kiszámított értéknek. | *13.32* |
| TotalOtherDiscount | Az ezekre a díjakra alkalmazott kedvezmény összege. A kompetencia vagy a MAPS terméklicencei, illetve az ösztönzőre jogosult új előfizetések szintén tartalmazni fognak egy kedvezmény összegét ebben az oszlopban. | *2.32* |
| Részösszeg | Adóz előtti összeg. Ellenőrzi, hogy a részösszeg megfelel-e a várható összegnek kedvezmény esetén. | *11* |
| Adó | Adó összege díj. A piac adószabályainak és konkrét körülményeinek megfelelően. | *0* |
| TotalForCustomer | Összes adó után. Ellenőrzi, hogy számlázott-e adót a számlán. | *11* |
| Pénznem | Pénznem típusa. Minden számlázási entitásnak csak egy pénzneme van. Ellenőrizze, hogy egyezik-e az első számlával. Ellenőrizze újra a főbb számlázási platformok frissítései után. | *EUR* |
| DomainName | Az ügyfél tartományneve. Ez a mező a második számlázási ciklusig üresen is megjelenhet. *Ezt a mezőt ne használja az ügyfél egyedi azonosítójaként. Az ügyfél/partner frissítheti a hiússágot vagy az alapértelmezett tartományt az Office 365 portálon keresztül.* | *example.onmicrosoft.com* |
| SubscriptionName | Előfizetés becenév. Ha nincs megadva becenév, a Partnerközpont **OfferName paramétert használja.** | *PROJECT ONLINE* |
| SubscriptionDescription (Előfizetési leírás) | Az ügyfél által megvásárolt szolgáltatásajánlat neve az árlistában meghatározottak szerint. (Ez a mező megegyezik az **OfferName mezővel.)** | *PROJECT ONLINE PREMIUM PROJEKT ÜGYFÉL NÉLKÜL* |
| BillingCycleType (BillingCycleType) | Egyszeres számlázási gyakoriság.| *Havonta* |
