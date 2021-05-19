---
title: Kereskedelmi piactéri ajánlatok vásárlása
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan vásárolhatnak SaaS-ajánlatokat független szoftverszállítóktól (ISV-ktől) a Partnerközpont piactéren a CSP-programpartnerek.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147853"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Kereskedelmi piactéri termékek vásárlása az ügyfelek számára Partnerközpont


**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök

A Felhőszolgáltató (CSP) program egyik partnereként a kereskedelmi piactéren vásárolhat előfizetéseket az ügyfelei számára a független szoftverszállítók (ISV-k) által kínált bizonyos Szolgáltatott szoftver (SaaS) termékekhez.

Ha ISV SaaS-előfizetéseket kínál ügyfeleinek, megkülönböztetheti vállalkozását. Emellett hozzáférést adhat az ügyfeleknek az adott üzleti igényeiknek megfelelő szoftvercsomaghoz. Ezeknek a piactéri SaaS-termékeknek a licencét és előfizetését is az ISV-közzétevőktől kezelheti, ahogyan a Microsoft-termékek licencét és előfizetését.

Vásárolhat licencalapú **SaaS-előfizetéseket** vagy **használatalapú előfizetéseket.** A licencalapú és a használatalapú számlázás közötti különbségekkel kapcsolatos további információkért lásd a [számlázás alapjait.](billing-basics.md)

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Licencalapú és forgalmi díjas SaaS-előfizetések vásárlása a Partnerközpont

Az ISV-közzétevők által kínált licencalapú vagy forgalmi díjas SaaS-termékek előfizetését ugyanazokkal a folyamatokkal vásárolhatja meg, mint a Microsoft-termékekhez.

Licencalapú vagy forgalmi díjas SaaS-előfizetés Partnerközpont ügyfél-előfizetések létrehozása, felfüggesztése vagy [lemondása.](create-a-new-subscription.md#create-a-new-subscription)

A kereskedelmi [piactéri előfizetések Partnerközpont API-kat](/partner-center/develop/) is használhatja az ügyfelek számára. (Az API-k használatával kapcsolatos Partnerközpont lásd: [Előfizetés létrehozása kereskedelmi piactéri termékekhez.)](/partner-center/develop/create-subscription-azure-marketplace-products)

>[!IMPORTANT]
> A CSP-programban partnerként licencalapú **vagy** forgalmi díjas SaaS-előfizetéseket vásárolhat a csv-közzétevőktől a Partnerközpont.  Ez azt jelenti, hogy bármilyen licencalapú vagy forgalmi díjas  SaaS-ajánlatot [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) megvásárolhat, amelyet az ISV közzétevő tett elérhetővé az Ön számára, beleértve azokat az ajánlatokat is, amelyekhez Hozzáféréssel rendelkezik.  Az ISV-k (például Azure-alkalmazásokat, tárolókat vagy virtuális gépeket érintő használatalapú ajánlatok) kereskedelmi piactéri ajánlatának megvásárlásához vagy kezeléséhez meg kell [Azure Portal.](https://portal.azure.com/)

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Használatalapú előfizetések vásárlása a Azure Portal

A külső ISV-közzétevőktől származó licencalapú SaaS-előfizetésekkel ellentétben a használatalapú előfizetések esetében az ügyfélnek először Azure-előfizetésre van szüksége. A kereskedelmi piactér számlázása, a használatalapú erőforrások az ügyfél Azure-előfizetése alá esnek. Ha az ügyfél már rendelkezik Azure-előfizetéssel, a CSP-program egyik partnere az alábbi lépéseket követve vásárolhat számukra kereskedelmi piactér-előfizetést:

1. Jelentkezzen be a Partnerközpont [irányítópultra,](https://partner.microsoft.com/dashboard)majd válassza az **Ügyfelek** lehetőséget a bal oldali menüben.

2. Válassza ki az adott ügyfelet, majd válassza az **Előfizetések lehetőséget.**  

3. A **Használatalapú előfizetések alatt válassza a** **Minden erőforrás lehetőséget.** Ezzel az Azure felügyeleti portálra kerül.

4. Az Azure felügyeleti portál bal oldali menüjében válassza **az Erőforrás** létrehozása lehetőséget.

5. A **lista tetején** válassza az Összes Azure Marketplace lehetőséget.

6. A lista szűkítéshez használjon szűrőket a Marketplace-lista tetején. Kiválaszthatja például a **Microsoft** vagy  a **Partner** lehetőséget a Közzétevő legördülő listából, hogy csak a Microsoft vagy egy ISV-közzétevő ajánlatát tekintse meg.

7. Válasszon ki egy adott ajánlatot, majd válassza a **Létrehozás lehetőséget.**

## <a name="next-steps"></a>Következő lépések

- [Kereskedelmi piactéri ajánlatok kezelése](csp-commercial-marketplace-purchase.md)