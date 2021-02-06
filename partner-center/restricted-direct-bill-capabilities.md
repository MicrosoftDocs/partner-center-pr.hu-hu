---
title: Korlátozott közvetlen számlázási képességek
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg a CSP Direct Bill partneri követelményeket és a teendőket a korlátozott lehetőségek elkerüléséhez. Annak megállapítása, hogy a képességei korlátozottak-e.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38fe5d03784d0fcf0796545d31e8272f316d2878
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/06/2021
ms.locfileid: "99623983"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Korlátozott közvetlen számlázási képességek és a CSP közvetlen számlázási partnerekhez szükséges követelmények  

## <a name="overview"></a>Áttekintés

A közvetlen számlázási partnereknek meg kell felelniük az új [követelményeknek](direct-partner-new-requirements.md) , hogy megmaradjanak a CSP Direct Bill partner programban. Ellenkező esetben a közvetlen számlázási funkciókhoz való hozzáférésük végül korlátozott lesz, és bizonyos feladatok elvégzése hosszabb időt is igénybe vehet, például az ügyfelek számára új vásárlásokat.

> [!Note]
> A Microsoft a közvetlen CSP-partneri programra vonatkozó új követelményeket nem teljesítő partnereket tájékoztatni fogja arról, ha a közvetlen számla funkciói korlátozottak lesznek. Ez az összes közvetlen számlázási partnerre vonatkozik, függetlenül attól, hogy a [közvetlen számlázási partnertől a közvetett viszonteladóig való áttérést](transition-direct-to-indirect.md) választotta-e.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Hogyan állapítható meg, hogy a közvetlen számlázási funkciók korlátozottak-e

Az alábbi lépéseket követve ellenőrizheti, hogy a közvetlen számlázási partner bérlőtől a közvetlen számlázási funkciókhoz való hozzáférés korlátozott-e.

1. Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard).

2. Nyissa meg a **Fiókbeállítások**  ->  **jogi profilt**.

3. A **program adatai** területen keresse meg **Microsoft Cloud megoldás szolgáltatójának állapotát**.

4. Ha a program állapota **korlátozott**, az azt jelenti, hogy a közvetlen számlás partner bérlője számára korlátozott a közvetlen számlázási funkciókhoz való hozzáférés.

## <a name="affected-direct-bill-capabilities"></a>Érintett közvetlen számlázási képességek

Ha a közvetlen számla funkciói korlátozottak voltak, már nem lehet új vásárlásokat vásárolni az ügyfelek számára a partner Centerben. Ez a korlátozás az alábbiakat tartalmazza:

- Azure-előfizetések

- Licenc alapú előfizetések

- Új bővítmények hozzáadása meglévő licenc-alapú előfizetésekhez.

- A szoftver-és foglalási termékek (például a szoftveres előfizetések, az örökös szoftverek és az Azure Reserved Virtual Machine instances) egyszeri vásárlása.

A CSP program keretében nem használhatja az [Azure partner megosztott szolgáltatások ajánlatát](shared-services.md) is, hogy új Azure-előfizetéseket vásároljon saját használatra.

A meglévő közvetlen számlázási előfizetéseket a rendszer nem érinti. Érvényesek maradnak, és automatikusan megújulnak. Továbbra is közvetlenül a Microsoft által számlázunk, amíg meg nem szakítják őket. A meglévő előfizetéseket továbbra is a következő módokon kezelheti:

- Meglévő előfizetések felfüggesztése

- Meglévő licenccel rendelkező előfizetések licencek számának módosítása

- A meglévő bővítmények licencek számának beállítása egy előfizetéshez. 
 
    >[!Note] 
    >Nem adhat hozzá új bővítményeket meglévő előfizetésekhez, mert az új vásárlásként lesz kezelve.

- Új Azure-erőforrások üzembe helyezése és meglévő Azure-erőforrások kezelése meglévő Azure-előfizetések alatt. Ide tartoznak az Azure Marketplace-en és a Visual Studio-előfizetéseken keresztül elérhető erőforrások.

Az új vásárlásokon kívül a következő közvetlen számlázási funkciók nem érhetők el a partner Centerben:

- Nem hozhat létre új ügyfél-bérlőket. Az **ügyfél létrehozása** lehetőség a partner központ **ügyfelek** lapján nem lesz elérhető.

- A közvetlen viszonteladói kapcsolatra vonatkozó meghívót nem lehet előkészíteni. A partner Center **ügyfelek** lapján a **viszonteladói kapcsolat kérése** lehetőség nem lesz elérhető.

    >[!NOTE]
    >A közvetlen számlázási partnertől a közvetett viszonteladóig történő áttérés részeként, ha már regisztrálta a közvetlen számlás partner bérlőt közvetett viszonteladóként, akkor a közvetett viszonteladói kapcsolatra vonatkozó meghívót is létrehozhat.

- Nem hozhat létre új homokozó-bérlőt. Minden közvetlen számlázási partner bérlő létrehozhat egy homokozó bérlőt a közvetlen számlázási API-integráció céljára. Ha korábban még nem hozott létre ilyet, nem teheti ezt meg, miután megtörtént a számlázási partneri képesség korlátozása.  

## <a name="next-steps"></a>Következő lépések

- [További információ a közvetett viszonteladók kiválásáról](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [CSP közvetlen partner új követelmények](direct-partner-new-requirements.md)
