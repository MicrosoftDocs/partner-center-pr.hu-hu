---
title: Azure Reservations & kiszolgáló-előfizetésekkel
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megismerhet Felhőszolgáltató Azure Reservations- és Server-előfizetések vásárlására, építésére és kezelésére vonatkozó lehetőségeket.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 79175fc7e67fdcdc3195b33859f3609c4caf942f
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149417"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="972cd-103">Azure-beli fenntartott virtuálisgép& példányok (RI) és kiszolgáló-előfizetések vásárlása, kiépítése és kezelése az ügyfelek számára</span><span class="sxs-lookup"><span data-stu-id="972cd-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="972cd-104">**Megfelelő szerepkörök:** Rendszergazdai ügynök | Globális rendszergazdai | Az | Értékesítési ügynök | Felhasználókezelő rendszergazda</span><span class="sxs-lookup"><span data-stu-id="972cd-104">**Appropriate roles**: Admin agent | Global admin | Helpdesk agent | Sales agent | User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="972cd-105">Mi az az Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="972cd-105">What are Azure Reservations?</span></span>

<span data-ttu-id="972cd-106">Az Azure Reservations segítségével pénzt takaríthat meg, ha előre fizet egy vagy három évnyi virtuális gépért, SQL Database számítási kapacitásért, Azure Cosmos DB átviteli sebességért vagy más Azure-erőforrásokért.</span><span class="sxs-lookup"><span data-stu-id="972cd-106">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="972cd-107">Az előzetes fizetés lehetővé teszi, hogy kedvezményt kap a használt erőforrásokra.</span><span class="sxs-lookup"><span data-stu-id="972cd-107">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="972cd-108">A Reservations jelentősen csökkentheti a virtuális gép, az SQL Database számítási, Azure Cosmos DB- és egyéb erőforrások költségeit akár 72%-kal a használat alapján fizetett árakhoz képest.</span><span class="sxs-lookup"><span data-stu-id="972cd-108">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="972cd-109">A Reservations számlázási kedvezményt nyújt, és nincs hatással az erőforrások futtatási állapotára.</span><span class="sxs-lookup"><span data-stu-id="972cd-109">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="972cd-110">További információ: [Mi az az Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="972cd-110">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="972cd-111">Miért érdemes az ügyfeleknek foglalást vásárolniuk?</span><span class="sxs-lookup"><span data-stu-id="972cd-111">Why should customers buy a reservation?</span></span>

<span data-ttu-id="972cd-112">Ha az ügyfelek olyan virtuális gépekkel, Azure Cosmos DB vagy SQL-adatbázisokkal futnak, amelyek hosszú ideig futnak, a foglalás megvásárlása biztosítja számukra a legköltséghatékosabb megoldást.</span><span class="sxs-lookup"><span data-stu-id="972cd-112">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="972cd-113">Ha például egy ügyfél folyamatosan futtatja egy szolgáltatás négy példányát foglalás nélkül, használat alapján kell fizetnie.</span><span class="sxs-lookup"><span data-stu-id="972cd-113">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="972cd-114">Ha ezekhez az erőforrásokhoz vásárolnak foglalást, azonnal kapják meg a foglalási kedvezményt.</span><span class="sxs-lookup"><span data-stu-id="972cd-114">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="972cd-115">Az erőforrásokért ezután nem használatalapú fizetéses díjakat kell fizetnie.</span><span class="sxs-lookup"><span data-stu-id="972cd-115">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="972cd-116">Lenyűgöző új Azure-ajánlat a CSP-ban</span><span class="sxs-lookup"><span data-stu-id="972cd-116">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="972cd-117">Azáltal, hogy az Azure Reservationst és a Kiszolgáló-előfizetéseket a CSP-programba teszi, a Microsoft jobban teszi lehetővé a partnerek számára, hogy a rendkívül kiszámítható, állandó felhőalapú számítási feladatok támogatásához költséghatékonyabb megoldások iránti egyre növekvő ügyféligényeket elégednek ki.</span><span class="sxs-lookup"><span data-stu-id="972cd-117">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="972cd-118">A CSP-program lehetővé teszi a partnerek számára az Azure Reservations- és Server-előfizetések a Kereskedelmi ügyfelek nevében történő megszerzését, üzembe Partnerközpont és Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="972cd-118">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="972cd-119">Még azt is megadjuk a CSP-programunk partnereinek, hogy hogyan vásárolhatók meg az Azure-foglalások.</span><span class="sxs-lookup"><span data-stu-id="972cd-119">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="972cd-120">A CSP-partnerek [vásárolhatnak Azure-foglalásokat](azure-reservations-buying.md) egy [](give-customers-permission.md) ügyfél nevében, vagy engedélyezhetik, hogy az ügyfél megvásárolja a saját foglalását egy korábbi Azure-előfizetésből, amit a partner megvásárolt számukra.</span><span class="sxs-lookup"><span data-stu-id="972cd-120">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="972cd-121">Az Azure Reservations rugalmasságot biztosít az ügyfeleknek a különböző számítástechnikai megoldások virtualizálásában, beleértve a fejlesztést és tesztelést, az alkalmazások futtatását és az adatközpont kibővítését.</span><span class="sxs-lookup"><span data-stu-id="972cd-121">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="972cd-122">A [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) esetében például a kereskedelmi ügyfelek akár 72%-ot is megtakaríthatnak a használat alapján fizetett Azure-beli virtuális gépek díjszabásával szemben, ha egy 1 vagy 3 éves időszakra megvásárolják a virtuális gépet .</span><span class="sxs-lookup"><span data-stu-id="972cd-122">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="972cd-123">A windowsos Azure Hybrid Benefit és Frissítési Garancia ügyfelek akár 80%-kal is pénzt takaríthatnak meg a fizetéses díjszabással szemben.</span><span class="sxs-lookup"><span data-stu-id="972cd-123">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="972cd-124">A lenyűgöző díjszabás és a nem egyező üzembe helyezési rugalmasság egyedülálló kombinációjával az ügyfelek az Azure Reservations kiválasztásakor a legjobb általános értéket látják.</span><span class="sxs-lookup"><span data-stu-id="972cd-124">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="972cd-125">Lásd: [Foglalások vásárlása](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) az Azure Portalon.</span><span class="sxs-lookup"><span data-stu-id="972cd-125">See [Purchase Reservations](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="972cd-126">A **szoftver-előfizetésekért** és a Linux ISV éves előfizetéseiért tekintse meg az Azure RI CSP kereskedelmi árlistát a **Microsoft Azure Reserved Instances** (Fenntartott példányok) kategória Partnerközpont Díjszabás és ajánlatok lapján. [](https://partner.microsoft.com/dashboard/sell/pricingandoffers)</span><span class="sxs-lookup"><span data-stu-id="972cd-126">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="972cd-127">**Linux ISV éves előfizetések**</span><span class="sxs-lookup"><span data-stu-id="972cd-127">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="972cd-128">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="972cd-128">SUSE Linux</span></span>
- <span data-ttu-id="972cd-129">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="972cd-129">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="972cd-130">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="972cd-130">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="972cd-131">**ISV éves előfizetések**</span><span class="sxs-lookup"><span data-stu-id="972cd-131">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="972cd-132">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="972cd-132">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="972cd-133">Első lépések</span><span class="sxs-lookup"><span data-stu-id="972cd-133">Getting started</span></span>

<span data-ttu-id="972cd-134">Annak érdekében, hogy megértsük, hogyan tudja az Azure Reservationst az ügyfelekkel együtt helyezze el, és hogyan tud a lehető leggyorsabban üzemelni, a következő megközelítést javasoljuk a készültségi anyagok áttekintésére:</span><span class="sxs-lookup"><span data-stu-id="972cd-134">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="972cd-135">Tekintse át és Partnerközpont [új kereskedelmi műveletek útmutatóját.](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)</span><span class="sxs-lookup"><span data-stu-id="972cd-135">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="972cd-136">Az Azure Reservations és a Server Subscriptions frissítéseit az [Partnerközpont API(API/SDK) szolgáltatásban értheti](/partner-center/develop/purchase-azure-reserved-vm-instances)meg.</span><span class="sxs-lookup"><span data-stu-id="972cd-136">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="972cd-137">Értékesítési készenlét</span><span class="sxs-lookup"><span data-stu-id="972cd-137">Sales readiness</span></span>

- [<span data-ttu-id="972cd-138">Távoli asztali szolgáltatások (RDS) ügyfél-hozzáférési licenc (CAL) (közlemény)</span><span class="sxs-lookup"><span data-stu-id="972cd-138">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="972cd-139">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="972cd-139">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="972cd-140">Kiszolgáló-előfizetések</span><span class="sxs-lookup"><span data-stu-id="972cd-140">Server Subscriptions</span></span>](./csp-software-subscriptions.md)

- [<span data-ttu-id="972cd-141">SQL DB Reservations (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="972cd-141">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="972cd-142">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="972cd-142">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="972cd-143">SQL Managed Instance (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="972cd-143">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="972cd-144">SUSE és Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="972cd-144">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="972cd-145">Red Hat Linux az Azure-ban</span><span class="sxs-lookup"><span data-stu-id="972cd-145">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="972cd-146">SUSE Linux az Azure-on</span><span class="sxs-lookup"><span data-stu-id="972cd-146">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="972cd-147">Linux az Azure-ban</span><span class="sxs-lookup"><span data-stu-id="972cd-147">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="972cd-148">Az Azure díjszabásának áttekintése</span><span class="sxs-lookup"><span data-stu-id="972cd-148">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="972cd-149">Azure díjkalkulátor</span><span class="sxs-lookup"><span data-stu-id="972cd-149">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="972cd-150">Azure Databricks egységfoglalások</span><span class="sxs-lookup"><span data-stu-id="972cd-150">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="972cd-151">Oktatás</span><span class="sxs-lookup"><span data-stu-id="972cd-151">Training</span></span>

<span data-ttu-id="972cd-152">Regisztráljon a kereskedelmi [licencelési készenlét webináriumok és](https://commercial-licensing.eventbuilder.com/FY2019_ALL) igény szerinti események megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="972cd-152">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="972cd-153">A korábban rögzített, igény szerinti licencelésre való készenlétről szóló események a következő témaköröket tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="972cd-153">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="972cd-154">CSP Online Services, CSP Azure és általános licencelési frissítések, beleértve az Azure-t (2018. november)</span><span class="sxs-lookup"><span data-stu-id="972cd-154">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="972cd-155">Fenntartott SQL DB-& példányméret-rugalmasság (2018. augusztus)</span><span class="sxs-lookup"><span data-stu-id="972cd-155">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="972cd-156">Kiszolgáló-előfizetések a CSP-ben (2018. július)</span><span class="sxs-lookup"><span data-stu-id="972cd-156">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="972cd-157">Az Azure Reservations áttekintése a CSP-ben (2018. május)</span><span class="sxs-lookup"><span data-stu-id="972cd-157">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="972cd-158">Üzemeltetés</span><span class="sxs-lookup"><span data-stu-id="972cd-158">Operations</span></span>

<span data-ttu-id="972cd-159">[Partnerközpont](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)új kereskedelmi műveletek útmutatója: Átfogó útmutató az olyan kulcsfontosságú szabályzatokról és működési szempontokról, mint a szerződések, a rendelés Partnerközpont, a számla, az árlista részletei, az ösztönzők, az egyeztetési fájl, az API/SDK, a Azure Partner Shared Services.</span><span class="sxs-lookup"><span data-stu-id="972cd-159">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="972cd-160">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="972cd-160">Azure Hybrid Benefit</span></span>

<span data-ttu-id="972cd-161">A [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) az Frissítési Garancia-licenccel rendelkező ügyfelek számára díjszabási kedvezmény, amely segít maximalizálni a meglévő helyszíni Windows Server- és/vagy SQL Server-licencbefektetések értékét az Azure-ba való miálás során.</span><span class="sxs-lookup"><span data-stu-id="972cd-161">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="972cd-162">A jogosult ügyfelek akár 40%-ot\* is megtakaríthat az Azure Virtual Machines-ban (szolgáltatásként elérhető infrastruktúra vagy IaaS), és akár 55%-ot is megtakaríthat Azure SQL Database-ban (szolgáltatásként elérhető platform vagy PaaS) és SQL Server-t az Azure Virtual Machines-ben (IaaS) az Azure Hybrid Benefit-sel, ami akár 80%-kal is nő az Azure-beli fenntartott példányokkal együtt.</span><span class="sxs-lookup"><span data-stu-id="972cd-162">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="972cd-163">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="972cd-163">Next steps</span></span>

- [<span data-ttu-id="972cd-164">Azure Hybrid Benefit – GYIK</span><span class="sxs-lookup"><span data-stu-id="972cd-164">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="972cd-165">\*A tényleges megtakarítás régiónként, példánytípustól vagy használattól függően változhat.</span><span class="sxs-lookup"><span data-stu-id="972cd-165">\*Actual savings may vary based on region, instance type, or usage.</span></span>