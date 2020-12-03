---
title: A CSP-partnerek Azure-csomagjának árlista
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ebből a cikkből megtudhatja, hogy a CSP program partnerei hogyan használhatják a partner centert az Azure-csomag előfizetéseit tartalmazó árlista megtekintéséhez.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 02cea980626ec32d3dd60f646b1f8744130792ea
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534726"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Az Azure-beli CSP új kereskedelmi felületének árlistája

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Számlázási adminisztrátor
- Globális rendszergazda
- Segélyszolgálat ügynöke
- Értékesítési ügynök
- Felhasználói felügyeleti rendszergazda

A CSP új Azure-beli kereskedelmi élményének árlista a következő címen érhető el: a partner Centerben. Az árlista dinamikus kézbesítése valós időben történik, és az árak csak USD-ben jelennek meg. A számlázás azonban az ügyfél pénznemének megfelelő támogatott pénznemben történik. Az ügyfél pénznemének megfizetésével kapcsolatos további információkért olvassa el az [Azure-csomag számlázása](azure-plan-billing.md)című témakört.

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Az Azure-csomag díjszabása alá tartozó előfizetések díjszabása

1. A bal oldali partner központ menüjében válassza az **értékesítés** , majd a **piactér** lehetőséget.

2. Az Azure-csomag díjszabása területen válassza ki azt az országot, amelynek díjszabását meg szeretné jeleníteni.

3. Az **Exportálás típusa** elemnél válassza az **Azure-csomag fogyasztásának díjszabása**, az **Azure Plan Reservations díjszabása** vagy az **FX-díjak** lehetőséget. 

>[!NOTE] 
>Az **FX díjszabása** nem országspecifikus.

4. A **dátum díjszabása** mellett válassza ki a kívánt dátumot, például: **current**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="ország-specifikus":::

>[!NOTE] 
>Két különböző árlistát is exportálhat – az Azure-csomag díjszabása és a piactér harmadik féltől származó díjszabása.

## <a name="azure-price-list-specifics"></a>Az Azure árlista sajátosságai

- Az Azure-csomag díjszabása a partner Center piactér lapján, az **értékesítés** alatt érhető el.

- Az export elérhető lesz az Azure Plan fogyasztási szolgáltatások, a Azure Reservations és a FX-díjak esetében.

- Az exportálási lehetőségek a következők:

  - A **mai díjszabás**: ide tartozik a hónap első napjának összes mérőszáma és díjszabása az aktuális hónap aktuális dátumára. Ez magában foglalja az új árakat, a megváltozott árakat vagy az eltávolított árakat. Az összes ár érvényes kezdési és befejezési dátummal fog elmagyarázni, hogy új vagy eltávolítva vannak-e.

  - **Előző havi díjszabás**: az egyes típusú erőforrások letöltése havonta történik. A díjszabási fájlok esetében ez magában foglalja az adott hónapban elérhető összes mérőszámot is. Ha a hónap közepén egy új mérőszám jelent meg, akkor az a rendelkezésre állását tükröző, érvényes dátummal rendelkező mérőszámként jelenik meg. A megszüntetett árakhoz hasonlóan, ha már nem érhető el, a tényleges befejezési dátum leírását mutatja be.

  - **FX-díjak**: az FX díjait a hónap első napjánál, 06:00 PST-ig töltheti le a rendszer. Ha például a novemberi díjszabást szeretné használni, töltse le a díjszabást október 31-én. Az előző hónap FX díjszabása is elérhető lesz.

- Az árlista árai a közvetlen árak. Egyes partnerek jogosultak lehetnek a partner által létrehozott kreditek használatára. A partner által szerzett kreditek kiszámításának módjával kapcsolatos információkért olvassa el, [Hogyan számítják ki és fizetik ki a partner által szerzett kreditet](partner-earned-credit-explanation.md).

- **Jogosult szolgáltatások**: a partner által létrehozott kreditek az **Azure-csomag** használati díjszabási partnerei által az Azure-csomag [díjszabási](https://partner.microsoft.com/commerce/sales) oldalán felsorolt szolgáltatásokra érvényesek. Vegye figyelembe, hogy a harmadik féltől származó termékek, például a (z) "harmadik fél" néven azonosíthatók, az Azure-csomag használati árlista és az Azure-csomag foglalásának címkék oszlopában vannak kivételek.

## <a name="price-list-data"></a>Árlista-adatlista

|**Mező**   |**Leírás**   |
|--------------------------|:---------------------------|
|ProductTitle  |A termék címe vagy neve|
|Termékazonosító   |A termék azonosítója|
|SKuId|SKU azonosítója|
|SkuTitle|Az SKU címe vagy neve|
|Publisher|az 1. fél mindig a Microsoft lesz|
|SkuDescription|Az SKU leírása|
|UnitOfMeasure|A felszámított vagy számlázott egységek|
|TermDuration|A kifejezésen alapuló termékek esetében a feltételek hossza, a foglalásokra alkalmazható.|
|Piaci|A díjszabás piaca|
|Pénznem|A díjszabás pénzneme|
|Egységár|Egységár|
|PricingTierRangeMin|A többszintű díjszabáshoz a minimális díj vonatkozik|
|PricingTierRangeMax|A többszintes díjszabás esetében a maximális ár vonatkozik|
|EffectiveStartDate|A díjszabás kezdő dátuma|
|EffectiveEndDate|A díjszabás záró dátuma|
|Meterid|A termék SKU-azonosítójának azonosítója|
|MeterType|Fogyasztásmérő típusa|
|Címkék|Az elem tulajdonságai az Azure-csomag díjszabásához ez az Azure vagy az Azure és a foglalások (kifejezetten a foglalások esetében).|

Az Azure-csomag árlista a partner Center [díjszabási és ajánlatok oldaláról](https://partner.microsoft.com/dashboard/sell/pricingandoffers) is exportálható.

## <a name="tiered-pricing"></a>Lépcsőzetes díjszabás

Néhány Azure-beli csomag-használati szolgáltatás támogatja a többplatformos díjszabást. A partnerek ezeket a termékeket és SKU-ket az Azure-csomag árlista listájában érhetik el. A díjszabási rétegek oszlopaiban található értékekkel rendelkező elemek lehetővé teszik a partnerek számára, hogy a használat alapján megértsék az árakat. Az alábbi példában a mintaadatok használatával három díjszabási csomaggal rendelkezünk egy termék SKU-val.

|**ProductId**   |**SkuId**   |**Egységár**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|.50|100001|9223372036854780000|
|DDD123456ABC|01AB|.80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Ebben a példában, ha az 101 egység használatos, a díj 100,80. Az első 100 egység az egyik, és a következő egységért díjat számítunk fel. 80.

## <a name="pricing-api-for-azure-plan"></a>Az Azure-csomag díjszabási API-ját

A [díjszabási API](/partner/develop/pricing) -val programozott módon kérheti le az Azure-csomag díjszabását a használat és a foglalások számára. A devizák díjszabását is lekérheti.

A díjszabási API egy másik végponton van, mint a többi partner Center API-k. A díjszabási információ az Azure-csomag-előfizetések esetében az USD-ben, az Azure-csomag erőforrásainak és a foglalások díjszabását tartalmazza.

Ez az API a partnerek számára is lehetővé teszi a havi árfolyamok beolvasását, mivel az Azure-csomag díjszabása csak USD értékű. Az API-kkal az aktuális hónap vagy az előző hónapok díjszabását és árfolyamait is lekérheti.

>[!NOTE]
> A díjszabási API az Azure-csomag díjszabására vonatkozik. Továbbra is használhatja a RateCard API-t és árlistát az Azure-erőforrások, illetve a nem Azure-beli csomag előfizetésekre telepített foglalások oldalának "díjszabás és ajánlatok" lapján. Az Azure-csomag díjszabási API-ját nem támogatja a szoftverek, a piactér vagy a licenc alapú díjszabás, például a Microsoft 365 vagy a Dynamics 365.

Az Azure-csomag díjszabásával és a deviza-díjszabási API-kkal kapcsolatos további információkért tekintse meg a teljes [díjszabási API dokumentációját](/partner/develop/pricing).

## <a name="next-steps"></a>További lépések

- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)