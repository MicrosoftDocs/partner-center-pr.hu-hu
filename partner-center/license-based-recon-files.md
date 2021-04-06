---
title: Licencalapú egyeztetési fájlok
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan olvashatja el a licenc-alapú egyeztetési fájlokat a partner Centerben. Ez a cikk ismerteti a licenc-alapú Recon-fájl egyes mezőinek jelentését.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4c311de4a504785e15cefc7a93f1ee3da396ea7d
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441285"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>A partner Center licenc-alapú egyeztető fájljaiban található mezők ismertetése

**A következőre érvényes:**

- A Microsoft Cloud for US Government Partnerközpontja

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói felügyeleti rendszergazda
- Számlázási adminisztrátor
- Felügyeleti ügynök

Ha egyeztetni szeretné a módosításokat az ügyfél rendelésein, hasonlítsa össze a **Syndication_Partner_Subscription_Numbert** az egyeztetési fájlból a partner Center **előfizetés-azonosítójával** .

## <a name="fields-in-license-based-reconciliation-files"></a>A licenc-alapú egyeztetési fájlok mezői

| Oszlop | Leírás | Mintaérték |
| ------ | ----------- | ------------ |
| PartnerId | Egyedi azonosító GUID formátumban egy adott számlázási entitáshoz. Egyeztetéshez nem szükséges. Ugyanaz az összes sorban. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Az ügyfél egyedi Microsoft-azonosítója GUID formátumban. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Az ügyfél szervezetének neve, ahogy az a partner Centerben szerepel. *Nagyon fontos mező a számla és a rendszerinformációk egyeztetéséhez.* | *Az A ügyfél tesztelése* |
| MpnId | A CSP-partner MPN-azonosítója. Lásd: [How to itemize by partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMpnId | Az előfizetéshez tartozó rekord viszonteladójának MPN-azonosítója.  |
| OrderId | Egy rendelés egyedi azonosítója a Microsoft számlázási platformon. Hasznos lehet a megrendelést azonosítani a támogatáshoz való kapcsolódáskor. Nem használatos egyeztetéshez. | *566890604832738111* |
| SubscriptionId | Egy előfizetéshez tartozó egyedi azonosító a Microsoft számlázási platformon. Hasznos lehet azonosítani az előfizetést, amikor kapcsolatba lép a támogatási szolgálattal. Nem használatos egyeztetéshez. *Ez az érték nem egyezik meg a partner felügyeleti konzol **előfizetés-azonosítójával** . Ehelyett tekintse meg a **SyndicationPartnerSubscriptionNumber** .* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Az előfizetések egyedi azonosítója. Egy ügyfél több előfizetéssel is rendelkezhet ugyanahhoz a csomaghoz. Ez az oszlop fontos a fájl-elemzések egyeztetéséhez. Ez a mező a partner felügyeleti konzol **előfizetés-azonosítóját** képezi le. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Egyedi ajánlat azonosítója. Standard szintű ajánlat azonosítója, a árlista alapján meghatározva. *Ez az érték nem felel meg az **ajánlat azonosítójának** az árlista alapján. Lásd a **DurableOfferID** helyet.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Egyedi tartós ajánlat azonosítója, a árlista alapján meghatározva. *Ez az érték megegyezik az **ajánlat-azonosítóval** az árlista alapján.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Az ügyfél által a árlista alapján megvásárolt szolgáltatási ajánlat neve. | *Microsoft Office 365 (E3 csomag)* |
| SubscriptionStartDate | Az előfizetés kezdő dátuma. Az időpont mindig a nap kezdete, 0:00. Ez a mező a rendelés elküldését követő napra van beállítva. A **SubscriptionEndDate** használatával határozható meg: Ha az ügyfél továbbra is az előfizetés első évében található, vagy ha az előfizetés a következő évre megújítva lett. | *2/1/2019 0:00* |
| SubscriptionEndDate | Az előfizetés befejezési dátuma. Az időpont mindig a nap kezdete, 0:00. *12 hónap, valamint a kezdési dátum utáni **x** nap* , hogy a partner számlázási dátumához vagy a *megújítási dátumhoz képest 12 hónapig* legyen igazítva. A megújítás során az árak az aktuális árlista alapján frissülnek. Az automatikus megújítás előtt szükség lehet az ügyfél-kommunikációra. | *2/1/2019 0:00* |
| ChargeStartDate | A díjak kezdő napja. Az időpont mindig a nap kezdete, 0:00. A napi *díjak (arányos* költségek) kiszámításához használatos, amikor egy ügyfél megváltoztatja a licencek számát. | *2/1/2019 0:00* |
| ChargeEndDate | A díjak befejezési napja. Az idő mindig a nap vége, 23:59. A napi *díjak (arányos* költségek) kiszámításához használatos, amikor egy ügyfél megváltoztatja a licencek számát. | *2/28/2019 23:59* |
| ChargeType | A [díj](recon-file-charge-types.md) vagy a beállítás típusa. | Tekintse meg a [díjszabási típusokat](recon-file-charge-types.md). |
| UnitPrice | Díj/licenc, a vásárlás időpontjában közzétett árlista szerint. Győződjön meg róla, hogy ez megegyezik a számlázási rendszeren tárolt információkkal az egyeztetés során. | *6,82* |
| Mennyiség | A licencek száma. Győződjön meg róla, hogy ez megegyezik a számlázási rendszeren tárolt információkkal az egyeztetés során. | *2* |
| Összeg | A mennyiség árának összege. Annak vizsgálatára szolgál, hogy az összeg kiszámítása megfelel-e az ügyfelek számára kiszámított értéknek. | *13,32* |
| TotalOtherDiscount | A díjakra alkalmazott kedvezmény összege. A kompetenciához vagy TÉRKÉPekhez tartozó licencek, illetve az olyan új előfizetések, amelyek jogosultak a kedvezményre, ebben az oszlopban is szerepelni fognak. | *2,32* |
| Részösszeg | Adózás előtti összeg. Ellenőrzi, hogy a részösszeg megfelel-e a várt összegnek a kedvezmény esetén. | *11* |
| Adó | Adó összegének díja. A piaci adószabályok és a konkrét körülmények alapján. | *0* |
| TotalForCustomer | ÁFA után összesen. Ellenőrzi, hogy a számlán kell-e adót fizetni. | *11* |
| Pénznem | Pénznem típusa Minden számlázási entitásnak csak egy pénzneme van. Ellenőrizze, hogy az megfelel-e az első számlájának. Az összes jelentős számlázási platform frissítése után ismételje meg a műveletet. | *EUR* |
| DomainName | Az ügyfél tartományneve. Ez a mező üresen jelenhet meg a második számlázási ciklusig. *Ne használja ezt a mezőt egyedi azonosítóként az ügyfél számára. Az ügyfél/partner a hiúság vagy az alapértelmezett tartomány frissítését az Office 365 portálon keresztül végezheti el.* | *example.onmicrosoft.com* |
| SubscriptionName | Előfizetés beceneve. Ha nincs megadva becenév, a partner Center a **OfferName** használja. | *PROJECT ONLINE* |
| SubscriptionDescription | Az ügyfél által a árlista alapján megvásárolt szolgáltatási ajánlat neve. (Ez egy, a **OfferName** megegyező mező.) | *PROJECT ONLINE PREMIUM – PROJECT CLIENT NÉLKÜL* |
| BillingCycleType | Egyszeri számlázási gyakoriság.| *Havonta* |