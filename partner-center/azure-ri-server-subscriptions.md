---
title: Azure-foglalások & Server-előfizetések
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg a felhőalapú megoldások szolgáltatójának lehetőségeit az Azure-foglalások és-kiszolgálói előfizetések beolvasásához, üzembe helyezéséhez és kezeléséhez.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0434ad2e6494f5efc1b1e5e2aa003dc6587d7b4e
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691350"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="a622a-103">Azure Reserved VM instances (RI) + kiszolgáló-előfizetések beolvasása, kiépítése, & kezelése</span><span class="sxs-lookup"><span data-stu-id="a622a-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="a622a-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="a622a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a622a-105">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="a622a-105">Admin agent</span></span>
- <span data-ttu-id="a622a-106">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="a622a-106">Global admin</span></span>
- <span data-ttu-id="a622a-107">Segélyszolgálat ügynöke</span><span class="sxs-lookup"><span data-stu-id="a622a-107">Helpdesk agent</span></span>
- <span data-ttu-id="a622a-108">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="a622a-108">Sales agent</span></span>
- <span data-ttu-id="a622a-109">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="a622a-109">User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="a622a-110">Mi az az Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="a622a-110">What are Azure Reservations?</span></span>

<span data-ttu-id="a622a-111">Azure Reservations a virtuális gép egy-vagy hároméves, SQL Database számítási kapacitásának, Azure Cosmos DB átviteli sebességének vagy más Azure-erőforrásoknak az előzetes kifizetésével segítheti a pénz megtakarítását.</span><span class="sxs-lookup"><span data-stu-id="a622a-111">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="a622a-112">Az előzetes fizetés lehetővé teszi, hogy kedvezményt kapjon a felhasznált erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="a622a-112">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="a622a-113">A foglalások jelentősen csökkenthetik a virtuális gépeket, az SQL Database számítási, Azure Cosmos DB és egyéb erőforrás-költségeit akár 72%-kal az utólagos elszámolású árakhoz képest.</span><span class="sxs-lookup"><span data-stu-id="a622a-113">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="a622a-114">A Reservations számlázási kedvezményt nyújt, és nincs hatással az erőforrások futtatási állapotára.</span><span class="sxs-lookup"><span data-stu-id="a622a-114">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="a622a-115">További információ: [Mi a Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="a622a-115">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="a622a-116">Miért vásárolnak az ügyfelek foglalást?</span><span class="sxs-lookup"><span data-stu-id="a622a-116">Why should customers buy a reservation?</span></span>

<span data-ttu-id="a622a-117">Ha az ügyfelek olyan virtuális gépeket, Azure Cosmos DB vagy SQL-adatbázisokat foglalnak magukban, amelyek hosszú ideig futnak, a foglalás megvásárlása a leghatékonyabb megoldást kínálja.</span><span class="sxs-lookup"><span data-stu-id="a622a-117">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="a622a-118">Ha például egy ügyfél a szolgáltatás négy példányát egy foglalás nélkül futtatja, akkor az utólagos elszámolású díjszabásban kell fizetni.</span><span class="sxs-lookup"><span data-stu-id="a622a-118">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="a622a-119">Ha foglalást vásárol az adott erőforráshoz, azonnal megkapja a foglalási kedvezményt.</span><span class="sxs-lookup"><span data-stu-id="a622a-119">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="a622a-120">Az erőforrásokért ezután nem használatalapú fizetéses díjakat kell fizetnie.</span><span class="sxs-lookup"><span data-stu-id="a622a-120">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="a622a-121">Lenyűgöző új Azure-ajánlat a CSP-ben</span><span class="sxs-lookup"><span data-stu-id="a622a-121">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="a622a-122">A Azure Reservations-és kiszolgáló-előfizetések CSP programba való bevonásával a Microsoft jobb lehetőséget biztosít partnerei számára, hogy a gyors ütemben növekvő ügyfelek számára költséghatékony megoldásokat kínáljon a nagy mértékben kiszámítható, állandó Felhőbeli számítási feladatok támogatásához.</span><span class="sxs-lookup"><span data-stu-id="a622a-122">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="a622a-123">A CSP program lehetővé teszi, hogy a partnerek a kereskedelmi ügyfelek nevében beszerezzék, kiépítsék és kezeljék Azure Reservations és kiszolgálói előfizetéseket a Microsoft partner Center és a Azure Portal használatával.</span><span class="sxs-lookup"><span data-stu-id="a622a-123">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="a622a-124">Az Azure-foglalások megvásárlásának módjáról is biztosítunk partnereket a CSP programban.</span><span class="sxs-lookup"><span data-stu-id="a622a-124">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="a622a-125">A CSP-partnerek az [ügyfelek nevében vásárolhatnak Azure-foglalásokat](azure-reservations-buying.md) , és [lehetővé tehetik, hogy az ügyfél megvásárolja a saját foglalásait](give-customers-permission.md) egy korábbi Azure-előfizetésből, amelyet a partner megvásárolt.</span><span class="sxs-lookup"><span data-stu-id="a622a-125">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="a622a-126">Azure Reservations az ügyfelek számára a virtualizáció rugalmasságát számos számítástechnikai megoldás esetében, beleértve a fejlesztést és tesztelést, az alkalmazások futtatását és az adatközpont kiterjesztését.</span><span class="sxs-lookup"><span data-stu-id="a622a-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="a622a-127">A [Azure Reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) például a kereskedelmi ügyfeleink akár 72%-ot is megtakarítanak, és az utólagos elszámolású Azure-beli virtuális gépek díjszabását egyszerűen megvásárolhatja, vagy "lefoglalhatja" a virtuális gépet egy 1 vagy 3 éves időszakra.</span><span class="sxs-lookup"><span data-stu-id="a622a-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="a622a-128">A frissítési garanciával rendelkező Windows Server rendszerű ügyfelek a Azure Hybrid Benefit akár 80%-ot is megtakarítanak, az utólagos elszámolású díjszabást is beleértve.</span><span class="sxs-lookup"><span data-stu-id="a622a-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="a622a-129">A kényszerített árképzés és a páratlan üzembe helyezési rugalmasság páratlan kombinációja esetén az ügyfelek a legjobb általános értéket fogják látni, amikor kiválasztják Azure Reservations.</span><span class="sxs-lookup"><span data-stu-id="a622a-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="a622a-130">Az Azure Portalon megjelenő [vásárlási foglalások](https://docs.microsoft.com/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) .</span><span class="sxs-lookup"><span data-stu-id="a622a-130">See [Purchase Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="a622a-131">Tekintse meg az **Azure ri CSP kereskedelmi díjszabását** a **Microsoft Azure fenntartott példányok** kategóriájában a következő témakörben: a partner Center [díjszabási és ajánlatok](https://partner.microsoft.com/dashboard/sell/pricingandoffers) lapján a szoftveres előfizetések és a Linux ISV éves előfizetések</span><span class="sxs-lookup"><span data-stu-id="a622a-131">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="a622a-132">**Linuxos ISV éves előfizetések**</span><span class="sxs-lookup"><span data-stu-id="a622a-132">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="a622a-133">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="a622a-133">SUSE Linux</span></span>
- <span data-ttu-id="a622a-134">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="a622a-134">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="a622a-135">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="a622a-135">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="a622a-136">**ISV éves előfizetések**</span><span class="sxs-lookup"><span data-stu-id="a622a-136">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="a622a-137">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="a622a-137">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="a622a-138">Első lépések</span><span class="sxs-lookup"><span data-stu-id="a622a-138">Getting started</span></span>

<span data-ttu-id="a622a-139">Ha szeretné megtudni, hogy a lehető leggyorsabban hogyan helyezheti el a Azure Reservationst az ügyfelekkel, és hogyan kezdheti el működés közben a lehető leghamarabb, javasoljuk, hogy tekintse át a következő módszert a készültségi anyagok áttekintéséhez:</span><span class="sxs-lookup"><span data-stu-id="a622a-139">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="a622a-140">Tekintse át és Ismerje meg a [partner Center új kereskedelmi üzemeltetési útmutatóját](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span><span class="sxs-lookup"><span data-stu-id="a622a-140">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="a622a-141">A Azure Reservations-és kiszolgálói előfizetések frissítéseinek megismerése a [partner Center API-ban (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span><span class="sxs-lookup"><span data-stu-id="a622a-141">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="a622a-142">Értékesítés készültsége</span><span class="sxs-lookup"><span data-stu-id="a622a-142">Sales readiness</span></span>

- [<span data-ttu-id="a622a-143">Távoli asztali szolgáltatások (RDS) ügyfél-hozzáférési licenc (CAL) (közlemény)</span><span class="sxs-lookup"><span data-stu-id="a622a-143">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="a622a-144">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="a622a-144">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="a622a-145">Kiszolgálói előfizetések</span><span class="sxs-lookup"><span data-stu-id="a622a-145">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)

- [<span data-ttu-id="a622a-146">SQL DB-foglalások (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="a622a-146">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="a622a-147">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="a622a-147">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="a622a-148">SQL felügyelt példánya (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="a622a-148">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="a622a-149">SUSE és Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="a622a-149">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="a622a-150">Red Hat Linux az Azure-on</span><span class="sxs-lookup"><span data-stu-id="a622a-150">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="a622a-151">SUSE Linux az Azure-on</span><span class="sxs-lookup"><span data-stu-id="a622a-151">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="a622a-152">Linux az Azure-ban</span><span class="sxs-lookup"><span data-stu-id="a622a-152">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="a622a-153">Az Azure díjszabásának áttekintése</span><span class="sxs-lookup"><span data-stu-id="a622a-153">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="a622a-154">Az Azure díjszabásának kalkulátora</span><span class="sxs-lookup"><span data-stu-id="a622a-154">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="a622a-155">Azure Databricks egység foglalásai</span><span class="sxs-lookup"><span data-stu-id="a622a-155">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="a622a-156">Képzés</span><span class="sxs-lookup"><span data-stu-id="a622a-156">Training</span></span>

<span data-ttu-id="a622a-157">Regisztráljon a [kereskedelmi licencelés készültségét ismertető előadások](https://commercial-licensing.eventbuilder.com/FY2019_ALL) és az igény szerinti események megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="a622a-157">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="a622a-158">A korábban rögzített licencelési készültség az igény szerinti eseményeknél többek között a következő témaköröket tartalmazza:</span><span class="sxs-lookup"><span data-stu-id="a622a-158">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="a622a-159">CSP Online Services, CSP Azure és általános licencelési frissítések, beleértve az Azure-t (november 2018)</span><span class="sxs-lookup"><span data-stu-id="a622a-159">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="a622a-160">SQL DB fenntartott kapacitás & példányának rugalmassága (2018. augusztus)</span><span class="sxs-lookup"><span data-stu-id="a622a-160">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="a622a-161">Kiszolgálói előfizetések a CSP-ben (július 2018)</span><span class="sxs-lookup"><span data-stu-id="a622a-161">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="a622a-162">Azure Reservations áttekintése a CSP-ben (május 2018)</span><span class="sxs-lookup"><span data-stu-id="a622a-162">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="a622a-163">Műveletek</span><span class="sxs-lookup"><span data-stu-id="a622a-163">Operations</span></span>

<span data-ttu-id="a622a-164">A [partner Center új kereskedelmi üzemeltetési útmutatója](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf): átfogó útmutató, amely tartalmazza a legfontosabb házirendeket és üzemeltetési szempontokat, például a szerződések, a partneri központ, a számla, az árlista részletei, az ösztönzők, a megbékélési fájl, az API/SDK, a homokozó és az Azure partner megosztott szolgáltatásait.</span><span class="sxs-lookup"><span data-stu-id="a622a-164">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="a622a-165">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="a622a-165">Azure Hybrid Benefit</span></span>

<span data-ttu-id="a622a-166">A [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) a frissítési garanciával rendelkező ügyfeleinknek szóló díjszabási kedvezmény, amely segít maximalizálni a meglévő helyszíni Windows Server-és/vagy SQL Server-licencek értékét az Azure-ba való Migrálás során.</span><span class="sxs-lookup"><span data-stu-id="a622a-166">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="a622a-167">A jogosult ügyfeleknek akár 40%-ot is megtakaríthat az Azure Virtual Machines (infrastruktúra-szolgáltatásként vagy IaaS), és akár 55%-ot is megtakaríthat Azure SQL Database (platform as szolgáltatásként vagy Péterként), és SQL Server az Azure Virtual Machines (IaaS Azure Hybrid Benefit) szolgáltatással, amely az Azure-beli fenntartott példányokkal együtt akár 80%-ra is nő.</span><span class="sxs-lookup"><span data-stu-id="a622a-167">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a622a-168">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="a622a-168">Next steps</span></span>

- [<span data-ttu-id="a622a-169">Azure Hybrid Benefit – GYIK</span><span class="sxs-lookup"><span data-stu-id="a622a-169">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="a622a-170">\* A tényleges megtakarítás a régió, a példány típusa vagy a használat alapján változhat.</span><span class="sxs-lookup"><span data-stu-id="a622a-170">\*Actual savings may vary based on region, instance type, or usage.</span></span>
