---
title: Korlátozott közvetlen számlázási képességek
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg a Felhőszolgáltató (CSP) közvetlen számlázási partnerekre vonatkozó követelményeit, és hogy mi a helyzet a képességek korlátozásának elkerüléséhez. Derítse ki, hogy korlátozva vannak-e a képességei.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5bc33101809a805ba591be5a9b51d8dfff2397b
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551418"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Korlátozott közvetlen számlázási képességek és a közvetlen számlázási partnerek CSP-hez szükséges követelményei

**Megfelelő szerepkörök:** Globális rendszergazda

## <a name="overview"></a>Áttekintés

A közvetlen számlázási partnereknek meg kell felelnie az új követelményeknek, hogy a Felhőszolgáltató (CSP) közvetlen számlázási partnerprogramjában maradjanak. [](direct-partner-new-requirements.md) Ellenkező esetben a közvetlen számlázási képességekhez való hozzáférésük idővel korlátozott lesz, és tovább végezhet bizonyos feladatokat, például új vásárlásokat az ügyfeleik számára.

> [!Note]
> A Közvetlen csp-partnerprogram követelményeinek nem megfelelő közvetlen számlázási partnereket a Microsoft értesíti, ha a közvetlen számlázási képességeik korlátozva lesznek. Ez az összes közvetlen számlázási partnerre vonatkozik, függetlenül attól, hogy a közvetlen számlázási partnerről a közvetett viszonteladókra való áttérés mellett döntöttek-e. [](transition-direct-to-indirect.md)  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Hogyan lehet tudni, hogy korlátozva vannak-e a közvetlen számlázási képességek?

Annak megerősítéséhez, hogy a közvetlen számlázási partner bérlője hozzáférése a közvetlen számlázási képességekhez korlátozva van-e, kövesse az alábbi lépéseket.

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard).

2. Ugrás a **Fiókbeállítások**  >  **Jogi profil elemre.**

3. A **Programadatok alatt** keresse meg **a Microsoft felhőszolgáltató állapotát.**

4. Ha a program állapotának **értéke** korlátozott, az azt jelenti, hogy a közvetlen számlázási partner bérlője nem férhet hozzá a közvetlen számlázási képességekhez.

## <a name="affected-direct-bill-capabilities"></a>A közvetlen számlázás érintett képességei

Ha a közvetlen számlázási lehetőségek korlátozva vannak, nem vásárolhat új vásárlásokat az ügyfelek számára a Partnerközpont. Ez a korlátozás a következőket foglalja magában:

- Azure-előfizetések

- Licencalapú előfizetések

- Új bővítmények hozzáadása meglévő licencalapú előfizetéshez.

- Vásároljon szoftvereket és foglalási termékeket (például szoftver-előfizetéseket, folyamatos szoftvereket és Azure Reserved Virtual Machine-példányokat).

A CSP-program [keretében elérhető Azure-partner](shared-services.md) megosztott szolgáltatásokra vonatkozó ajánlattal nem vásárolhat saját használatra új Azure-előfizetéseket.

A meglévő közvetlen számlázási előfizetések nem érintettek. Érvényesek maradnak, és automatikusan újraújulnak. A Microsoft továbbra is közvetlenül számláz, amíg le nem mondja őket. Továbbra is a következő módokon kezelheti a meglévő előfizetéseket:

- Meglévő előfizetések felfüggesztése

- Meglévő licencalapú előfizetések licencszámának beállítása

- Módosíthatja az előfizetés meglévő bővítményei licencszámát. 

    >[!Note]
    >A meglévő előfizetések nem adhatnak hozzá új bővítményeket, mivel a rendszer új vásárlásként kezeli őket.

- Új Azure-erőforrások üzembe helyezése és meglévő Azure-erőforrások kezelése meglévő Azure-előfizetések alatt. Ide tartoznak az előfizetések és előfizetések Azure Marketplace Visual Studio erőforrások is.

Az új vásárlások mellett nem férhet hozzá a következő közvetlen számlázási képességekhez a Partnerközpont:

- Nem hozhat létre új ügyfélbérlőket. Az **Ügyfél létrehozása lehetőség** nem **érhető** el a Partnerközpont oldalán.

- Nem hozhat létre közvetlen viszonteladói kapcsolatot kérő meghívót az ügyfélnek. A  **viszonteladói kapcsolat kérése** lehetőség nem érhető el az Ügyfelek Partnerközpont lapon.

    >[!NOTE]
    >A közvetlen számlázási partnerről a közvetett viszonteladóra való áttérés részeként, ha a közvetlen számlázási partnerbérlőt már regisztrálta közvetett viszonteladóként, meghívót hozhat létre a közvetett viszonteladói kapcsolatot kérő ügyfélnek.

- Nem hozhat létre új sandbox-bérlőt. Minden közvetlen számlázási partnerbérlő létrehozhat egy sandbox-bérlőt a közvetlen számlázási API-integrációhoz. Ha még nem hozott létre egyet, a közvetlen számlázási partnerképességének korlátozását követően erre nincs jogosultsága.  

## <a name="next-steps"></a>Következő lépések

- [További információ a közvetett viszonteladóvá válásról](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [A közvetlen CSP-partnerre vonatkozó új követelmények](direct-partner-new-requirements.md)
