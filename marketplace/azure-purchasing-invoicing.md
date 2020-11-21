---
title: Szoftverek és megoldások vásárlása az Azure Marketplace-ről
description: Ismerje meg azokat az eszközöket, amelyek egyszerűbbé és egyszerűbbé teszik a szoftverek vásárlását és felügyeletét az Azure Marketplace-en.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: b93ce1394326887b4265114c58527c36379101d9
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007547"
---
# <a name="azure-marketplace-purchasing"></a>Az Azure Marketplace megvásárlása

Az Azure Marketplace számos olyan eszközzel és funkcióval rendelkezik, amely egyszerűbbé és egyszerűbbé teszi a vásárlási házirend megvásárlását, számlázását és kezelését.

## <a name="simplified-procurement"></a>Egyszerűsített beszerzés

Az Azure Marketplace-en különböző vásárlási lehetőségek állnak rendelkezésére, amelyekkel leegyszerűsítheti a beszerzési folyamatot. Ha az Azure-fiókjához társított bankkártyát használ, az összes vásárlás konszolidálva lesz egyetlen számlán, és a választott bankkártyára kerül. Ha Ön nagy ügyfél, megvásárolhatja Nagyvállalati Szerződés használatával. A nagyvállalati szerződéssel rendelkező szoftvereket a rendszer automatikusan felveszi az Azure-számlába. A számla elején az Azure használati díjai jelennek meg, amelyeket az Azure Marketplace díjai követnek.

Az Azure Marketplace-en való vásárlás során nem kell az egyes szállítói kapcsolatok és számlák kezelésének összetettségét kizárni. A Microsoft egyetlen, összevont havi számlát kap, amely az Azure Marketplace-vásárlásokat és az Azure-díjakat is tartalmazza.

## <a name="permission-to-purchase"></a>A vásárláshoz szükséges engedély

Miután megtalálta a megfelelő szoftvert, a vásárlás befejezése egyszerű. Az Azure-előfizetésben azonban megfelelő engedélyekkel kell rendelkeznie. Mivel az Azure [szerepköralapú Access Control](https://docs.microsoft.com/azure/role-based-access-control/overview) (RBAC) modellen működik, a fióknak **előfizetés-tulajdonosi** vagy **közreműködői** engedélyekkel kell rendelkeznie a vásárláshoz.

A vásárlás befejezése előtt ellenőrizze, hogy a felhasználó rendelkezik-e a megfelelő konfigurációval az Azure-bérlőben. Ez segít megelőzni a hibák megvásárlását.

Az Azure Marketplace-en a Azure Portalban keresse meg a megvásárolni kívánt alkalmazást, majd válassza a **Létrehozás** vagy **beállítás + előfizetés** lehetőséget. A rendszer kérni fogja, hogy az új megoldás használata előtt végezzen el néhány információt.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Az ajánlat létrehozása gomb.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="A beállítás + előfizetés gomb.":::

Ha az Azure Marketplace online áruházból szeretne megoldást telepíteni, válassza a **Letöltés most** lehetőséget a termékleírás lapon, majd jelentkezzen be az Azure-fiókja hitelesítő adataival.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Az Azure Marketplace bejelentkezési párbeszédpanelje.":::

A bejelentkezés után a rendszer átirányítja a termékre a Azure Portal a vásárlás befejezéséhez.

## <a name="purchase-policy-management"></a>A házirend-kezelés megvásárlása

A Microsoft lehetővé teszi a felhasználói vásárlások kezelését a számlázási profilon keresztül az Azure-előfizetés rendszergazdájaként. Három lehetőség közül választhat:

- **Ingyenes és fizetős** – lehetővé teszi, hogy a felhasználók bármilyen Azure Marketplace-alkalmazást szerezzenek be.
- **Ingyenes** – lehetővé teszi a felhasználók számára, hogy csak az Azure piactéren telepítsenek ingyenes szoftvereket.
- **Nem** – megakadályozza, hogy a felhasználók szoftvert telepítsenek az Azure piactéren.

Ezek a beállítások az Azure-előfizetéshez hozzáféréssel rendelkező összes felhasználóra érvényesek, amely lehetővé teszi az IT-beszerzések vezérlését a Azure Portalon keresztül.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Az informatikai beszerzések szabályozása a Azure Portal":::

## <a name="cost-management"></a>Cost Management

Az Azure Marketplace-en vásárolt termékekhez olyan bepillantást szeretne kapni, amelyek segítenek a költségek kezelésében. Azure Cost Management a megvásárolt termékekkel kapcsolatos információk megtekintésére szolgáló ingyenes eszköz. A Cost Management használatával megtekintheti, hogy milyen szolgáltatásokra költ pénzt, és hogyan követheti nyomon ezeket a költségeket a beállított költségkeretek alapján. A költségvetések beállítása mellett a jelentések is ütemezhetők, és az előfizetési költségek is elemezhetők. További információ a Azure Cost Managementről: a Microsoft Learn modul [elemzése a költségek elemzéséhez és a költségvetések létrehozása Azure Cost Management](https://docs.microsoft.com/learn/modules/analyze-costs-create-budgets-azure-cost-management/)használatával.

Az Azure Cost Management költségelemző eszközével megtekintheti az Azure Marketplace-díjakat és a számlákat.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="A Azure Cost Management használatával betekintést nyerhet a megvásárolt termékekbe.":::

## <a name="next-steps"></a>Következő lépések

- [Számlázás és számlázás](billing-invoicing.md)
