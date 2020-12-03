---
title: Ügyfelek eladása Microsoft Azure foglalások
description: Felhőalapú megoldás-szolgáltatóként megvásárolhatja, értékesítheti vagy kezelheti az ügyfelek számára elérhető Azure-foglalásokat. A partner Center, a Azure Portal vagy a partner Center API használata.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534896"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="09b24-104">Microsoft Azure foglalások eladása a partner Center, a Azure Portal vagy az API-kat használó ügyfeleknek</span><span class="sxs-lookup"><span data-stu-id="09b24-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="09b24-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="09b24-105">**Appropriate roles**</span></span>

- <span data-ttu-id="09b24-106">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="09b24-106">Admin agent</span></span>
- <span data-ttu-id="09b24-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="09b24-107">Global admin</span></span>
- <span data-ttu-id="09b24-108">Segélyszolgálat ügynöke</span><span class="sxs-lookup"><span data-stu-id="09b24-108">Helpdesk agent</span></span>
- <span data-ttu-id="09b24-109">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="09b24-109">Sales agent</span></span>
- <span data-ttu-id="09b24-110">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="09b24-110">User management admin</span></span>

<span data-ttu-id="09b24-111">A felhőalapú megoldás-szolgáltatói programban (CSP) lévő partnerként megvásárolhatja, értékesítheti vagy kezelheti az ügyfelek számára elérhető Azure-foglalásokat.</span><span class="sxs-lookup"><span data-stu-id="09b24-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="09b24-112">A partner Center, a Azure Portal vagy a partner Center API használata.</span><span class="sxs-lookup"><span data-stu-id="09b24-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="09b24-113">Ez a cikk csak a CSP-ben lévő partnerekre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="09b24-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="09b24-114">A más típusú előfizetéseket (például az utólagos elszámolású, az egyéni, a Microsoft-ügyféli szerződést vagy a Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek Ehelyett olvasniuk kell [Az Azure foglalási dokumentációját](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="09b24-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="09b24-115">A CSP programban részt vevő partnerek Microsoft Azure foglalásokat biztosíthatnak ügyfeleiknek.</span><span class="sxs-lookup"><span data-stu-id="09b24-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="09b24-116">Az ügyfelek jelentős megtakarítást érhet el, ha előre foglalják őket.</span><span class="sxs-lookup"><span data-stu-id="09b24-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="09b24-117">Az Azure-foglalások az alábbi módokon kínálják az ügyfelek egyszerűségét és rugalmasságát:</span><span class="sxs-lookup"><span data-stu-id="09b24-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="09b24-118">Egy vagy három éves foglalási feltétel</span><span class="sxs-lookup"><span data-stu-id="09b24-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="09b24-119">Könnyű első lépések; a telepítés másodpercek alatt befejeződött</span><span class="sxs-lookup"><span data-stu-id="09b24-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="09b24-120">Visszavont vagy Exchange fenntartott példányok bármikor a korrigált visszatérítéshez</span><span class="sxs-lookup"><span data-stu-id="09b24-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="09b24-121">Fenntartott példányok használatának kezelése a szervezeti vagy az egyéni részleg szintjén</span><span class="sxs-lookup"><span data-stu-id="09b24-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="09b24-122">Az Azure-foglalások az alábbi módokon nyújthatnak az ügyfeleknek:</span><span class="sxs-lookup"><span data-stu-id="09b24-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="09b24-123">A foglalások jelentős megtakarítást biztosíthatnak az utólagos elszámolású (TB) díjszabásban</span><span class="sxs-lookup"><span data-stu-id="09b24-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="09b24-124">Jobb költségvetés és előrejelzés az előzetes fizetéssel egy évig vagy hároméves feltételek mellett</span><span class="sxs-lookup"><span data-stu-id="09b24-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="09b24-125">Rangsorolt számítási kapacitás az irodákhoz legközelebb eső Azure-régióban</span><span class="sxs-lookup"><span data-stu-id="09b24-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="09b24-126">Az Azure-foglalások biztosítják a végpontok közötti infrastruktúra-megoldások alapját a Microsoft Windows Serverhez és Azure SQL Database hasonló szoftverekkel kombinálva</span><span class="sxs-lookup"><span data-stu-id="09b24-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="09b24-127">Az Azure-foglalásokat a partner központban és a Azure Portal is megvásárolhatja, értékesítheti és kezelheti, valamint használhatja a partner Center API-t is.</span><span class="sxs-lookup"><span data-stu-id="09b24-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="09b24-128">Lehetővé teheti ügyfelei számára, hogy saját Azure-foglalásokat vásárolnak a számukra megvásárolt Azure-előfizetésből.</span><span class="sxs-lookup"><span data-stu-id="09b24-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="09b24-129">Az alábbi hivatkozásokat követve megtudhatja, hogyan.</span><span class="sxs-lookup"><span data-stu-id="09b24-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="09b24-130">Azure-foglalások erőforrásai</span><span class="sxs-lookup"><span data-stu-id="09b24-130">Azure reservations resources</span></span>

|<span data-ttu-id="09b24-131">**További információ**</span><span class="sxs-lookup"><span data-stu-id="09b24-131">**For information about**</span></span>   |<span data-ttu-id="09b24-132">**Olvassa el ezt**</span><span class="sxs-lookup"><span data-stu-id="09b24-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="09b24-133">Az Azure foglalási dokumentációja ügyfelei számára</span><span class="sxs-lookup"><span data-stu-id="09b24-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="09b24-134">Mik az Azure-beli foglalások?</span><span class="sxs-lookup"><span data-stu-id="09b24-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="09b24-135">Azure-foglalások vásárlása az ügyfelek számára a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="09b24-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="09b24-136">Azure-foglalások vásárlása</span><span class="sxs-lookup"><span data-stu-id="09b24-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="09b24-137">Azure-foglalások kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="09b24-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="09b24-138">Azure-foglalások kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="09b24-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="09b24-139">A virtuális gép megfelelő méretének meghatározása és az ügyfél virtuális gép használatának ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="09b24-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="09b24-140">Virtuális gép méretezése az Azure-foglalások maximális használatára</span><span class="sxs-lookup"><span data-stu-id="09b24-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="09b24-141">Azure-foglalások vásárlása a partner Center API használatával</span><span class="sxs-lookup"><span data-stu-id="09b24-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="09b24-142">[Vásárlás Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) a partner Center fejlesztői dokumentációjában</span><span class="sxs-lookup"><span data-stu-id="09b24-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="09b24-143">Engedélyt ad a felhasználóknak a saját Azure-foglalások megvásárlására a CSP-előfizetésből.</span><span class="sxs-lookup"><span data-stu-id="09b24-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="09b24-144">Engedélyt ad az ügyfeleknek a saját Azure-foglalások megvásárlására</span><span class="sxs-lookup"><span data-stu-id="09b24-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |