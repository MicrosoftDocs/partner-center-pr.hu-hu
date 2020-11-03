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
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529911"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="bf512-104">Microsoft Azure foglalások eladása a partner Center, a Azure Portal vagy az API-kat használó ügyfeleknek</span><span class="sxs-lookup"><span data-stu-id="bf512-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="bf512-105">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="bf512-105">**Applies to**</span></span>

- <span data-ttu-id="bf512-106">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="bf512-106">Partner Center</span></span>
- <span data-ttu-id="bf512-107">Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="bf512-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="bf512-108">Partnerek a CSP programban</span><span class="sxs-lookup"><span data-stu-id="bf512-108">Partners in the CSP program</span></span>

<span data-ttu-id="bf512-109">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="bf512-109">**Appropriate roles**</span></span>

- <span data-ttu-id="bf512-110">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="bf512-110">Admin agent</span></span>
- <span data-ttu-id="bf512-111">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="bf512-111">Global admin</span></span>
- <span data-ttu-id="bf512-112">Segélyszolgálat ügynöke</span><span class="sxs-lookup"><span data-stu-id="bf512-112">Helpdesk agent</span></span>
- <span data-ttu-id="bf512-113">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="bf512-113">Sales agent</span></span>
- <span data-ttu-id="bf512-114">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="bf512-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="bf512-115">Ez a cikk csak a Cloud Solution Provider (CSP) programban található partnerekre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="bf512-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="bf512-116">A más típusú előfizetéseket (például az utólagos elszámolású, az egyéni, a Microsoft-ügyféli szerződést vagy a Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek Ehelyett olvasniuk kell [Az Azure foglalási dokumentációját](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="bf512-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="bf512-117">A CSP programban részt vevő partnerek Microsoft Azure foglalásokat biztosíthatnak ügyfeleiknek.</span><span class="sxs-lookup"><span data-stu-id="bf512-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="bf512-118">Az ügyfelek jelentős megtakarítást érhet el, ha előre foglalják őket.</span><span class="sxs-lookup"><span data-stu-id="bf512-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="bf512-119">Az Azure-foglalások az alábbi módokon kínálják az ügyfelek egyszerűségét és rugalmasságát:</span><span class="sxs-lookup"><span data-stu-id="bf512-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="bf512-120">Egy vagy három éves foglalási feltétel</span><span class="sxs-lookup"><span data-stu-id="bf512-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="bf512-121">Könnyű első lépések; a telepítés másodpercek alatt befejeződött</span><span class="sxs-lookup"><span data-stu-id="bf512-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="bf512-122">Visszavont vagy Exchange fenntartott példányok bármikor a korrigált visszatérítéshez</span><span class="sxs-lookup"><span data-stu-id="bf512-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="bf512-123">Fenntartott példányok használatának kezelése a szervezeti vagy az egyéni részleg szintjén</span><span class="sxs-lookup"><span data-stu-id="bf512-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="bf512-124">Az Azure-foglalások az alábbi módokon nyújthatnak az ügyfeleknek:</span><span class="sxs-lookup"><span data-stu-id="bf512-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="bf512-125">A foglalások jelentős megtakarítást biztosíthatnak az utólagos elszámolású (TB) díjszabásban</span><span class="sxs-lookup"><span data-stu-id="bf512-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="bf512-126">Jobb költségvetés és előrejelzés az előzetes fizetéssel egy évig vagy hároméves feltételek mellett</span><span class="sxs-lookup"><span data-stu-id="bf512-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="bf512-127">Rangsorolt számítási kapacitás az irodákhoz legközelebb eső Azure-régióban</span><span class="sxs-lookup"><span data-stu-id="bf512-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="bf512-128">Az Azure-foglalások biztosítják a végpontok közötti infrastruktúra-megoldások alapját a Microsoft Windows Serverhez és Azure SQL Database hasonló szoftverekkel kombinálva</span><span class="sxs-lookup"><span data-stu-id="bf512-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="bf512-129">Az Azure-foglalásokat a partner központban és a Azure Portal is megvásárolhatja, értékesítheti és kezelheti, valamint használhatja a partner Center API-t is.</span><span class="sxs-lookup"><span data-stu-id="bf512-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="bf512-130">Lehetővé teheti ügyfelei számára, hogy saját Azure-foglalásokat vásárolnak a számukra megvásárolt Azure-előfizetésből.</span><span class="sxs-lookup"><span data-stu-id="bf512-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="bf512-131">Az alábbi hivatkozásokat követve megtudhatja, hogyan.</span><span class="sxs-lookup"><span data-stu-id="bf512-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="bf512-132">Azure-foglalások erőforrásai</span><span class="sxs-lookup"><span data-stu-id="bf512-132">Azure reservations resources</span></span>

|<span data-ttu-id="bf512-133">**További információ**</span><span class="sxs-lookup"><span data-stu-id="bf512-133">**For information about**</span></span>   |<span data-ttu-id="bf512-134">**Olvassa el ezt**</span><span class="sxs-lookup"><span data-stu-id="bf512-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="bf512-135">Az Azure foglalási dokumentációja ügyfelei számára</span><span class="sxs-lookup"><span data-stu-id="bf512-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="bf512-136">Mik az Azure-beli foglalások?</span><span class="sxs-lookup"><span data-stu-id="bf512-136">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="bf512-137">Azure-foglalások vásárlása az ügyfelek számára a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="bf512-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="bf512-138">Azure-foglalások vásárlása</span><span class="sxs-lookup"><span data-stu-id="bf512-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="bf512-139">Azure-foglalások kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="bf512-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="bf512-140">Azure-foglalások kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="bf512-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="bf512-141">A virtuális gép megfelelő méretének meghatározása és az ügyfél virtuális gép használatának ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="bf512-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="bf512-142">Virtuális gép méretezése az Azure-foglalások maximális használatára</span><span class="sxs-lookup"><span data-stu-id="bf512-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="bf512-143">Azure-foglalások vásárlása a partner Center API használatával</span><span class="sxs-lookup"><span data-stu-id="bf512-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="bf512-144">[Vásárlás Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) a partner Center fejlesztői dokumentációjában</span><span class="sxs-lookup"><span data-stu-id="bf512-144">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="bf512-145">Engedélyt ad a felhasználóknak a saját Azure-foglalások megvásárlására a CSP-előfizetésből.</span><span class="sxs-lookup"><span data-stu-id="bf512-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="bf512-146">Engedélyt ad az ügyfeleknek a saját Azure-foglalások megvásárlására</span><span class="sxs-lookup"><span data-stu-id="bf512-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |