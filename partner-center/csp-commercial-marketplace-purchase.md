---
title: Kereskedelmi Piactéri ajánlatok vásárlása
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy a CSP-program partnerei hogyan használhatják a partner Center Marketplace-t a független szoftvergyártók (ISV-ket) által kínált SaaS-ajánlatok vásárlásához.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 841308d535d4071ee0a8eabf3e70325edea5777c
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979716"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Kereskedelmi piactéren vásárolt termékek vásárlása a partner Centerben


**Megfelelő szerepkörök**

- Globális rendszergazda
- Felügyeleti ügynök

A Cloud Solution Provider (CSP) programban partnerként a kereskedelmi piactéren vásárolhat előfizetéseket ügyfelei számára a független szoftvergyártók (ISV-EK) által kínált, szolgáltatásként nyújtott szoftverként (SaaS).

Az ISV SaaS-előfizetések ügyfelei számára történő biztosításával megkönnyítheti a vállalatok megkülönböztetését. Az ügyfelek számára hozzáférést biztosíthat az adott üzleti igényeknek megfelelő szoftver-kötegekhez is. A piactéren elérhető SaaS-termékek licenceit és előfizetéseit a Microsoft-termékekhez tartozó licencek és előfizetések kezelése során kezelheti.

Vásárolhat **licenc-alapú** SaaS-előfizetéseket vagy **használati alapú** előfizetéseket. Ha többet szeretne megtudni a licenc-alapú és a használati alapú számlázás közötti különbségekről, tekintse meg a [számlázás alapjai](billing-basics.md)című témakört.

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Licenc-alapú és mért SaaS-Előfizetések vásárlása a partner Centerben

Az ISV-gyártók által kínált licenc-alapú vagy mért SaaS-termékek előfizetéseit a Microsoft-termékek előfizetésének megvásárlására használt eljárással vásárolhatja meg.

Ha licenc-alapú vagy mért SaaS-előfizetést szeretne vásárolni a partner Centerben, tekintse meg az [ügyfél-előfizetések létrehozása, felfüggesztése vagy megszakítása](create-a-new-subscription.md#create-a-new-subscription)című témakört.

A [partner Center API](/partner-center/develop/) -k használatával kereskedelmi piactér-előfizetéseket hozhat létre ügyfelei számára. (A partner Center API-k használatával kapcsolatos további információkért lásd: [előfizetés létrehozása kereskedelmi Piactéri termékekhez](/partner-center/develop/create-subscription-azure-marketplace-products).)

>[!IMPORTANT]
> A CSP programban partnerként vásárolhat **licenc-alapú** vagy **mért** SaaS-előfizetéseket a partner centeren belüli ISV-közzétevők közül. Ez azt jelenti, hogy vásárolhat bármilyen **licenccel** vagy **mért** SaaS-ajánlatot, amelyet az ISV közzétevő elérhetővé tett, beleértve az [exkluzív ajánlatokat](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) is, amelyekhez hozzáféréssel rendelkezik. Ha más, kereskedelmi Piactéri ajánlatokat szeretne megvásárolni vagy kezelni (például Azure-alkalmazásokat,-tárolókat vagy virtuális gépeket érintő használaton alapuló ajánlatokat), akkor a [Azure Portalra](https://portal.azure.com/)kell lépnie.

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Használati alapú Előfizetések vásárlása a Azure Portal

A külső gyártótól származó ISV-közzétevők licenc-alapú SaaS-előfizetésével ellentétben a használati előfizetésekhez először az ügyfélnek Azure-előfizetésre van szüksége. A kereskedelmi piactéren a használaton alapuló erőforrások számlázása az ügyfél Azure-előfizetése alá tartozik. Ha az ügyfél Azure-előfizetéssel rendelkezik, a CSP programban található partner a következő lépésekkel vásárolhatja meg a kereskedelmi piactér-előfizetéseket:

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard), majd válassza az **ügyfelek** lehetőséget a bal oldali menüben.

2. Válassza ki az adott ügyfelet, majd válassza az **előfizetések** lehetőséget.  

3. A **használat alapú előfizetések** területen válassza az **összes erőforrás** lehetőséget. Ezzel az Azure felügyeleti portálra kerül.

4. Az Azure felügyeleti portálján válassza az **erőforrás létrehozása** lehetőséget a bal oldali menüben.

5. Az Azure Marketplace-lista tetején kattintson az **összes** megjelenítése lehetőségre.

6. A lista szűkítéséhez használjon szűrőket a piactér lista tetején. Kiválaszthatja például a **Microsoft** vagy a **partner** elemet a **közzétevő** legördülő listából, hogy csak a Microsoft vagy az ISV közzétevő által készített ajánlatokat tekintse meg.

7. Válasszon egy adott ajánlatot, majd válassza a **Létrehozás** lehetőséget.

## <a name="next-steps"></a>További lépések

- [Kereskedelmi Piactéri ajánlatok kezelése](csp-commercial-marketplace-purchase.md)