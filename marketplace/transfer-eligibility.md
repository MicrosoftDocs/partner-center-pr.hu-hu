---
title: Átruházási jogosultság – az előfizetés számlázási fiókok közötti továbbítására vonatkozó irányelvek, Azure Marketplace
description: A kereskedelmi ellenőrzésekre vonatkozó irányelvek a Azure Portalban lévő számlázási fiókok közötti előfizetés átadása előtt.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412556"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Az előfizetés számlázási fiókok közötti átvitelének jogosultsága

Az [előfizetést átviheti](/azure/cost-management-billing/understand/subscription-transfer) az egyik számlázási fiókból a másikba a Azure Portal számlázási szakaszában. Az átvitel előtt a rendszer az előfizetést a harmadik féltől származó termékek esetében ellenőrzi. Az átvitel csak akkor engedélyezett, ha az *összes* termék el van távolítva az átvitelre (lásd az alábbi [feltételeket](#criteria-for-transfer-approval-or-denial) ). A rendszer a következő lépések elvégzése érdekében a megfelelő hibaüzeneteket fogja létrehozni a nem egyértelmű alkalmazások számára.

> [!NOTE]
> Ez a cikk nem vonatkozik az SaaS-ajánlatokra, mert az SaaS-erőforrások egy bérlőhöz, nem pedig előfizetéshez vannak csatolva. Az SaaS-erőforrások az egyik számlázási fiókból a másikba vihetők át, de az erőforrás és az Azure-támogatás támogatási kérelemként történik.

## <a name="criteria-for-transfer-approval-or-denial"></a>Az átvitel jóváhagyásának vagy elutasításának feltételei

Az előfizetés nem vihető át, ha a harmadik féltől származó alkalmazásai megfelelnek a következő feltételeknek:

- A célként megadott fiók kereskedelmi jellegű, és az alkalmazás leválasztása partnereken keresztül történik.
- Az alkalmazás a kiválasztott partnerek számára választható, és a cél fiók nem szerepel az engedélyezési listán.
- Az ajánlat előzetes ajánlat volt a múltban a kiválasztott előfizetésekhez, vagy egy privát ajánlat volt, és az előfizetés már nem szerepel az engedélyezési listán.
- Az új számlázási fiók olyan régióban található, amely eltér az ajánlat eladásának helyétől, és az ajánlat nem értékesíthető ebben a régióban.

A letiltott átvitel mindaddig érvényben marad, amíg el nem távolítja az erőforrást az előfizetésből, amely után újra próbálkozhat az átvitelsel.

## <a name="next-steps"></a>Következő lépések

[Támogatás kérése Microsoft AppSource és az Azure Marketplace-en](get-support.md)

