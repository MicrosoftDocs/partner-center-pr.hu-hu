---
title: Szoftver és megoldások vásárlása a Azure Marketplace
description: Megismerheti az eszközöket, amelyek leegyszerűsítik és leegyszerűsítik a szoftvervásárlásokat és -Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 04/15/2021
ms.openlocfilehash: cfe37f26ad685ca723336d8559d15d4a64048f4b
ms.sourcegitcommit: 2ad9e61fa5b9941f927ebf44c459b6c1bd055b9d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/08/2021
ms.locfileid: "109630083"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace vásárlás

Azure Marketplace számos olyan eszközzel és funkcióval rendelkezik, amelyek leegyszerűsítik és leegyszerűsítik a vásárlási szabályzat megvásárlásának, számlázásának és kezelésének folyamatát.

## <a name="simplified-procurement"></a>Egyszerűsített beszerzés

Az Azure Marketplace-en különböző vásárlási lehetőségek állnak rendelkezésére, amelyekkel leegyszerűsítheti a beszerzési folyamatot. Ha az Azure-fiókjához társított hitelkártyával vásárol termékeket, az összes vásárlás egyetlen számlán lesz összesülve, és a választott hitelkártyára lesz kiszámlázva. Ha Ön nagy ügyfél, vásárolhat egy Nagyvállalati Szerződés. Nagyvállalati Szerződés esetén a szoftvervásárlások automatikusan szerepelnek az Azure-számlán. A számla elején az Azure használati díjai jelennek meg, amelyeket az Azure Marketplace díjai követnek.

Ha a vásárlást Azure Marketplace, kiküszöbölheti az egyéni szállítói kapcsolatok és számlák kezelésével kapcsolatos összetettséget. Egyetlen, összevont havi számlát kap a Microsofttól, amely a vásárlásokat és Azure Marketplace Azure-díjakat is tartalmazza.

## <a name="permission-to-purchase"></a>Vásárlásra vonatkozó engedély

Miután megtalálta a megfelelő szoftveralkalmazást, a vásárlás egyszerű. Ehhez azonban megfelelő engedélyekre lesz szüksége az Azure-előfizetésen belül. Mivel az Azure szerepköralapú Access Control (RBAC) modellt üzemeltet,  a fiókjának előfizetés-tulajdonosi vagy közreműködői engedélyekkel kell rendelkeznie a vásárláshoz. [](/azure/role-based-access-control/overview) 

A vásárlás befejezése előtt győződjön meg arról, hogy a felhasználó a megfelelő konfigurációval rendelkezik az Azure-bérlőben. Ez segít megelőzni a vásárlás során előforduló hibákat.

A Azure Marketplace felhasználói élményben keresse meg Azure Portal megvásárolni kívánt alkalmazást,  majd válassza a Létrehozás vagy beállítás **+ előfizetés lehetőséget.** Az új megoldás használata előtt meg kell adnia néhány információt.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Az ajánlat Létrehozása gomb.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="A Beállítás és feliratkozás gomb.":::

Ha egy megoldást szeretne üzembe helyezni a Azure Marketplace online  áruházból, válassza a Termékleírás oldalon a Lekért most lehetőséget, majd jelentkezzen be Azure-fiókjának hitelesítő adataival.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="A Azure Marketplace bejelentkezési párbeszédpanel.":::

Miután bejelentkezett, a rendszer átirányítja a termékhez a Azure Portal a vásárlás befejezéséhez.

## <a name="purchase-policy-management"></a>Vásárlási szabályzat kezelése

A Microsoft lehetővé teszi a felhasználói vásárlások kezelését a számlázási profilon keresztül Azure-előfizetés-rendszergazdaként. Három lehetőség közül választhat:

- **Ingyenes és fizetős** – Lehetővé teszi, hogy a felhasználók bármilyen Azure Marketplace szoftveralkalmazást szerezzenek be.
- **Ingyenes** – Lehetővé teszi, hogy a felhasználók csak ingyenes szoftvereket telepítsenek Azure Marketplace.
- **Nem** – Megakadályozza, hogy a felhasználók szoftvereket telepítsenek Azure Marketplace.

Ezek a beállítások az Azure-előfizetéshez hozzáféréssel rendelkező összes felhasználóra vonatkoznak, ami lehetővé teszi az it-beszerzések szabályozását a Azure Portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Az it-beszerzés szabályozása a Azure Portal":::

## <a name="cost-management"></a>Költségkezelés

Amikor termékeket vásárol a Azure Marketplace, olyan elemzéseket szeretne kapni, amelyek segítenek a költségek kezelésében. Azure Cost Management ingyenes eszköz a megvásárolt termékek információinak megtekintéséhez. A Cost Management részletesen is láthatja, hogy milyen szolgáltatásokra költ pénzt az idő alatt, és hogyan követik nyomon ezek a költségek a beállított költségvetéseket. A költségvetések beállítása mellett jelentéseket is ütemezhet, és elemezheti az előfizetési költségeket. A költségelemzésről Azure Cost Management a költségek elemzéséről és Microsoft Learn költségvetések létrehozásáról a következővel: [Azure Cost Management.](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)

Az Azure Cost Management költségelemző eszközével megtekintheti az Azure Marketplace-díjakat és a számlákat.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="A Azure Cost Management információkhoz juthat a megvásárolt termékekről.":::

## <a name="purchase-validation-checks"></a>Vásárlásérvényesítési ellenőrzések

Ha egy ajánlatot egy Azure Marketplace keresztül vásárol, az több okból is meghiúsulhat. A parancssori felület (CLI) használata nagyobb valószínűséggel okoz hibákat, mivel előfordulhat, hogy olyan ajánlatot próbál vásárolni, amely nem érhető el vagy nem látható a Azure Marketplace. A vásárlás meghiúsulhat az alábbi ellenőrzéseken:

1. Az előfizetés egy Nagyvállalati Szerződés (EA) tagja, és az EA-rendszergazda letiltotta Azure Marketplace vásárlásokat.
1. Az EA-rendszergazda csak ingyenes ajánlatokhoz engedélyezte a vásárlásokat, az ajánlat pedig fizetős ajánlat.
1. Az ajánlat nem található a piactéren.
1. A független szoftverszállító (ISV) elavult (korábban nem értékesíti) az ajánlatot, legalább az Ön régiójában.
1. A használt előfizetés egy olyan régióban található számlázási fiókhoz tartozik, ahol az ajánlat nem érhető el.
1. Az előfizetési/számlázási fiók nincs érvényes fizetési eszközhöz (például érvényes hitelkártyához) társítva.
1. Az előfizetés egy Felhőszolgáltató (CSP) tulajdonában van, és az isV elutasította az értékesítést egy CSP-n keresztül.
1. A privát Marketplace engedélyezve van az előfizetéshez, és az ajánlat nem szerepel az engedélyezett ajánlatok listáján.
1. Az ajánlat privát/előzetes verziójú adott ügyfelek számára, és az előfizetés nem szerepel az engedélyezett ügyfelek listájában.

## <a name="next-steps"></a>Következő lépések

- [Számlázás és számlakiállítás](billing-invoicing.md)