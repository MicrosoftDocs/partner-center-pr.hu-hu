---
title: Azure-csomag árlistja CSP-partnerek számára
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan használhatnak a CSP-partnerek Partnerközpont az Azure-csomag előfizetései árlistát.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 6d8e73e664d400e8e6d80e529326e566c5fd88a8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149570"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Az Azure-beli CSP új kereskedelmi felületének árlistája

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Globális rendszergazdai | Az | Értékesítési ügynök | Felhasználókezelő rendszergazda

A CSP-beli új Azure kereskedelmi élmény árlistát a következő Partnerközpont. Az árlista dinamikusan, valós idejű, pontos fájlban jelenik meg, és az árak csak USD-ben jelennek meg. 2021. január 28-tól az EU/EFTA és az Egyesült Királyság régió azon partnerei, akik új ügyfelekkel és meglévő CSP-ügyfelekkel vásárolnak új kereskedelmi ajánlatokat 2020. május 11. előtt először, a vásárlásokért a partnerhely pénznemében kell fizetni.  Az EU-n/EFTA-n és az Egyesült Királyságon kívüli partnerek számlázása továbbra is partnerhelyi pénznemben történik. Olvassa el az [Azure-csomag – számlázás részt.](azure-plan-billing.md)

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Az Azure-csomag díjszabása alatt tekintse meg az előfizetések díjszabását

1. A bal Partnerközpont menüben válassza az **Értékesítés,** majd a **Marketplace lehetőséget.**

2. Az Azure-csomag díjszabása alatt válassza ki azt az országot, amelyre a díjszabást szeretné.

3. Az Exportálás **típusa mellett** válassza az **Azure-csomag fogyasztási díjszabását,** az **Azure-csomag foglalási díjszabását** vagy az **FX-díjszabást.** 

>[!NOTE] 
>**Az FX-árfolyamok** nem országspecifikusak.

4. A **dátum díjszabása mellett** válassza ki a kívánt dátumot, például: **Aktuális**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="országspecifikus":::

>[!NOTE] 
>Két különböző árlistát exportálhat – az Azure-csomag díjszabását és a Marketplace külső díjszabását.

## <a name="azure-price-list-specifics"></a>Az Azure-árlista pontos pontos listája

- Az Azure-csomag díjszabása a piactér oldalának Értékesítés Partnerközpont **érhető el.**

- Az exportálási szolgáltatás elérhető lesz az Azure-csomagfelhasználási szolgáltatásokhoz, az Azure Reservationshez és az FX díjszabáshoz.

- Exportálási lehetőségek:

  - **A mai díjszabás:** Ez tartalmazza az összes mérőt és díjszabást a hónap 1. napától az aktuális hónap aktuális dátumig. Ide tartoznak az új árak, a módosított vagy az eltávolított árak. Minden árnak vannak tényleges kezdő és záró dátumai, amelyek elmagyarázzák, hogy újak vagy eltávolítva vannak-e.

  - **Előző havi díjszabás:** Az egyes erőforrástípusokat havonta töltheti le. A díjszabási fájlokban ez az ebben a hónapban elérhető összes mérőt tartalmazza. Ha a hónap közepén megjelent egy új fogyasztásmérő, akkor a rendelkezésre állását tükröző tényleges dátummal jelennek meg mérőként. Hasonló a megszüntetett árakhoz, és egy záró dátum jelenik meg, amely leírja, hogy mikor nem érhetők el.

  - **FX Rates:** Az FX-díjszabás a hónap 1. napja előtt, 18:00-kor (PST) tölthető le. Ha például novemberi díjszabást szeretne, töltse le az október 31-i díjszabást. Az előző havi FX-díjszabások is elérhetők lesznek.

- Az árlistákban az árak közvetlen árak. Egyes partnerek jogosultak lehetnek a partneri jóváírásra. A partneri jóváírás kiszámításával kapcsolatos információkért olvassa el A partneri jóváírás kiszámításának és kifizetésének [módját.](partner-earned-credit-explanation.md)

- **Jogosult szolgáltatások:** A partneri jóváírás az **Azure-csomag** használatának díjszabási oldalán felsorolt szolgáltatásokra vonatkozik, amelyek exportálhatók az [Azure-csomag díjszabási oldalára.](https://partner.microsoft.com/commerce/sales) Vegye figyelembe, hogy az Azure-csomag fogyasztási árának listájában és az Azure-csomagfoglalások Címkék oszlopában vannak olyan kivételek, mint például a harmadik féltől származó termékek, amelyek "harmadik félként" vannak azonosítva.

## <a name="price-list-data"></a>Árlista adatai

|**Mező**   |**Leírás**   |
|--------------------------|:---------------------------|
|ProductTitle (Termékkulcs)  |A termék címe vagy neve|
|Termékazonosító   |A termék azonosítója|
|SKuId (Termékváltozatazonosító)|Termékváltozat azonosítója|
|Termékváltozat|Termékváltozat címe vagy neve|
|Publisher|Az első fél mindig a Microsoft lesz|
|SkuDescription (SkuDescription)|A termékváltozat leírása|
|UnitOfMeasure|A felszámlázható vagy számlázható egységek|
|TermDuration (Időtartam)|Kifejezésalapú termékek esetén a foglalásokra érvényes időszak hossza|
|Piac|A díjszabás piaca|
|Pénznem|A díjszabás pénzneme|
|UnitPrice|Egységár|
|PricingTierRangeMin|Rétegzett díjszabás esetén a minimális ár a következő:|
|PricingTierRangeMax|Rétegzett díjszabás esetén a maximális ár a következő:|
|EffectiveStartDate (Hatályos kezdődátum)|A díjszabás kezdő dátuma|
|EffectiveEndDate (Hatályos ésddátum)|A díjszabás záró dátuma|
|MeterIds (Mérőazonosítók)|A termékváltozat fogyasztásmérő-azonosítója|
|MeterType (Fogyasztásmérő típusa)|Fogyasztásmérő típusa|
|Címkék|Az elem tulajdonságai, az Azure-csomag díjszabása esetén ez az Azure vagy az Azure és a Foglalások (különösen foglalások esetén)|

Az Azure-csomag árlistái a díjszabás és ajánlatok oldalról exportálhatók [a](https://partner.microsoft.com/dashboard/sell/pricingandoffers) Partnerközpont.

## <a name="tiered-pricing"></a>Rétegzett díjszabás

Egyes Azure-csomagfelhasználási szolgáltatások támogatják a rétegzett díjszabást. A partnerek az Azure-csomag árlistán találhatják meg ezeket a termékeket és terméktermékeket. A tarifacsomag-tartományok oszlopában található értékekkel a partnerek a használat alapján megértheti az árat. Az alábbi példában mintaadatokat használva egy három tarifacsomagú termékváltozatunk van.

|**Termelés**   |**SkuId (Termékváltozatazonosító)**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|.50|100001|9223372036854780000|
|DDD123456ABC|01AB|.80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Ebben a példában 101 egység használata esetén a díj 100,80 lenne. Az első 100 egység egy-egy, a következő egységért pedig 0,80-at kell fizetni.

## <a name="pricing-api-for-azure-plan"></a>Az Azure-csomag díjszabási API-ja

A díjszabási [API-val](/partner/develop/pricing) programozott módon lekérheti az Azure-csomag díjszabását a felhasználás és a foglalások számára. A idegen árfolyamokat is lekérheti.

A díjszabási API más végponton van, mint a Partnerközpont API-k. A díjszabási információk között szerepel az Azure-csomag erőforrásainak fogyasztásmérő-díjszabása USD-ben, valamint az Azure-csomag előfizetéseire alkalmazott foglalási díjszabás.

Ez az API lehetővé teszi a partnerek számára a havi árfolyamok lekérését is, mivel az Azure-csomag díjszabása csak USD-ben történik. Az API-k használatával lekérheti a díjszabást és a idegen árfolyamokat is az aktuális hónapra vagy az előző hónapokra.

>[!NOTE]
> A díjszabási API az Azure-csomag díjszabására vonatkozik. Továbbra is a Partnerközpont "Díjszabás és ajánlatok" oldalán közzétett, meglévő RateCard API-t és árlistákat kell használnia a nem Azure-csomag előfizetésében üzembe helyezett Azure-erőforrásokhoz vagy foglalásokhoz. Az Azure-csomag díjszabási API nem támogatja a szoftver-, marketplace- vagy licencalapú díjszabást, például a Microsoft 365 vagy a Dynamics 365 díjszabását.

Az Azure-csomag díjszabására és a idegen árfolyam API-kra vonatkozó további információkért tekintse meg a teljes [díjszabási API-dokumentációt.](/partner/develop/pricing)

## <a name="next-steps"></a>Következő lépések

- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)
