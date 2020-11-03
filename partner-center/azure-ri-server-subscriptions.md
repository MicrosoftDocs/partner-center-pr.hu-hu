---
title: Azure-foglalások & Server-előfizetések
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg a felhőalapú megoldások szolgáltatójának lehetőségeit az Azure-foglalások és-kiszolgálói előfizetések beolvasásához, üzembe helyezéséhez és kezeléséhez.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3c08e897a8f5d7c11b36627b0c24ad2da3f92329
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529910"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="04f32-103">Azure Reserved VM instances (RI) + kiszolgáló-előfizetések beolvasása, kiépítése, & kezelése</span><span class="sxs-lookup"><span data-stu-id="04f32-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="04f32-104">A következőkre vonatkozik:</span><span class="sxs-lookup"><span data-stu-id="04f32-104">Applies to:</span></span>

- <span data-ttu-id="04f32-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="04f32-105">Partner Center</span></span>

<span data-ttu-id="04f32-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="04f32-106">**Appropriate roles**</span></span>

- <span data-ttu-id="04f32-107">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="04f32-107">Admin agent</span></span>
- <span data-ttu-id="04f32-108">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="04f32-108">Global admin</span></span>
- <span data-ttu-id="04f32-109">Segélyszolgálat ügynöke</span><span class="sxs-lookup"><span data-stu-id="04f32-109">Helpdesk agent</span></span>
- <span data-ttu-id="04f32-110">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="04f32-110">Sales agent</span></span>
- <span data-ttu-id="04f32-111">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="04f32-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="04f32-112">Ez a cikk csak a Cloud Solution Provider (CSP) programban található partnerekre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="04f32-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="04f32-113">A más típusú előfizetéseket (például az utólagos elszámolású, az egyéni, a Microsoft-ügyféli szerződést vagy a Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek Ehelyett olvasniuk kell [Az Azure foglalási dokumentációját](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="04f32-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="04f32-114">Mi az az Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="04f32-114">What are Azure Reservations?</span></span>

<span data-ttu-id="04f32-115">Azure Reservations a virtuális gép egy-vagy hároméves, SQL Database számítási kapacitásának, Azure Cosmos DB átviteli sebességének vagy más Azure-erőforrásoknak az előzetes kifizetésével segítheti a pénz megtakarítását.</span><span class="sxs-lookup"><span data-stu-id="04f32-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="04f32-116">Az előzetes fizetés lehetővé teszi, hogy kedvezményt kapjon a felhasznált erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="04f32-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="04f32-117">A foglalások jelentősen csökkenthetik a virtuális gépeket, az SQL Database számítási, Azure Cosmos DB és egyéb erőforrás-költségeit akár 72%-kal az utólagos elszámolású árakhoz képest.</span><span class="sxs-lookup"><span data-stu-id="04f32-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="04f32-118">A Reservations számlázási kedvezményt nyújt, és nincs hatással az erőforrások futtatási állapotára.</span><span class="sxs-lookup"><span data-stu-id="04f32-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="04f32-119">További információ: [Mi a Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="04f32-119">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="04f32-120">Miért vásárolnak az ügyfelek foglalást?</span><span class="sxs-lookup"><span data-stu-id="04f32-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="04f32-121">Ha az ügyfelek olyan virtuális gépeket, Azure Cosmos DB vagy SQL-adatbázisokat foglalnak magukban, amelyek hosszú ideig futnak, a foglalás megvásárlása a leghatékonyabb megoldást kínálja.</span><span class="sxs-lookup"><span data-stu-id="04f32-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="04f32-122">Ha például egy ügyfél a szolgáltatás négy példányát egy foglalás nélkül futtatja, akkor az utólagos elszámolású díjszabásban kell fizetni.</span><span class="sxs-lookup"><span data-stu-id="04f32-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="04f32-123">Ha foglalást vásárol az adott erőforráshoz, azonnal megkapja a foglalási kedvezményt.</span><span class="sxs-lookup"><span data-stu-id="04f32-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="04f32-124">Az erőforrásokért ezután nem használatalapú fizetéses díjakat kell fizetnie.</span><span class="sxs-lookup"><span data-stu-id="04f32-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="04f32-125">Lenyűgöző új Azure-ajánlat a CSP-ben</span><span class="sxs-lookup"><span data-stu-id="04f32-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="04f32-126">A Azure Reservations-és kiszolgáló-előfizetések CSP programba való bevonásával a Microsoft jobb lehetőséget biztosít partnerei számára, hogy a gyors ütemben növekvő ügyfelek számára költséghatékony megoldásokat kínáljon a nagy mértékben kiszámítható, állandó Felhőbeli számítási feladatok támogatásához.</span><span class="sxs-lookup"><span data-stu-id="04f32-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="04f32-127">A CSP program lehetővé teszi, hogy a partnerek a kereskedelmi ügyfelek nevében beszerezzék, kiépítsék és kezeljék Azure Reservations és kiszolgálói előfizetéseket a Microsoft partner Center és a Azure Portal használatával.</span><span class="sxs-lookup"><span data-stu-id="04f32-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="04f32-128">Az Azure-foglalások megvásárlásának módjáról is biztosítunk partnereket a CSP programban.</span><span class="sxs-lookup"><span data-stu-id="04f32-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="04f32-129">A CSP-partnerek az [ügyfelek nevében vásárolhatnak Azure-foglalásokat](azure-reservations-buying.md) , és [lehetővé tehetik, hogy az ügyfél megvásárolja a saját foglalásait](give-customers-permission.md) egy korábbi Azure-előfizetésből, amelyet a partner megvásárolt.</span><span class="sxs-lookup"><span data-stu-id="04f32-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="04f32-130">Azure Reservations az ügyfelek számára a virtualizáció rugalmasságát számos számítástechnikai megoldás esetében, beleértve a fejlesztést és tesztelést, az alkalmazások futtatását és az adatközpont kiterjesztését.</span><span class="sxs-lookup"><span data-stu-id="04f32-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="04f32-131">A [Azure Reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) például a kereskedelmi ügyfeleink akár 72%-ot is megtakarítanak, és az utólagos elszámolású Azure-beli virtuális gépek díjszabását egyszerűen megvásárolhatja, vagy "lefoglalhatja" a virtuális gépet egy 1 vagy 3 éves időszakra.</span><span class="sxs-lookup"><span data-stu-id="04f32-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="04f32-132">A frissítési garanciával rendelkező Windows Server rendszerű ügyfelek a Azure Hybrid Benefit akár 80%-ot is megtakarítanak, az utólagos elszámolású díjszabást is beleértve.</span><span class="sxs-lookup"><span data-stu-id="04f32-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="04f32-133">A kényszerített árképzés és a páratlan üzembe helyezési rugalmasság páratlan kombinációja esetén az ügyfelek a legjobb általános értéket fogják látni, amikor a Azure Reservations választják:</span><span class="sxs-lookup"><span data-stu-id="04f32-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="04f32-134">Azure Reserved Virtual Machine Instances</span><span class="sxs-lookup"><span data-stu-id="04f32-134">Azure reservations</span></span>

- <span data-ttu-id="04f32-135">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="04f32-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="04f32-136">SQL DB-foglalások</span><span class="sxs-lookup"><span data-stu-id="04f32-136">SQL DB Reservations</span></span>
- <span data-ttu-id="04f32-137">SQL Managed Instance</span><span class="sxs-lookup"><span data-stu-id="04f32-137">SQL Managed Instance</span></span>
- <span data-ttu-id="04f32-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="04f32-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="04f32-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="04f32-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="04f32-140">App Services</span><span class="sxs-lookup"><span data-stu-id="04f32-140">App Services</span></span>
- <span data-ttu-id="04f32-141">Azure Databricks egység foglalásai</span><span class="sxs-lookup"><span data-stu-id="04f32-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="04f32-142">Felügyelt lemez</span><span class="sxs-lookup"><span data-stu-id="04f32-142">Managed Disk</span></span>
- <span data-ttu-id="04f32-143">Blokkblob</span><span class="sxs-lookup"><span data-stu-id="04f32-143">Block blob</span></span>
- <span data-ttu-id="04f32-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="04f32-144">MySQL</span></span>
- <span data-ttu-id="04f32-145">Azure-adatkezelő</span><span class="sxs-lookup"><span data-stu-id="04f32-145">Azure Data explorer</span></span>
- <span data-ttu-id="04f32-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="04f32-146">MariaDB</span></span>
- <span data-ttu-id="04f32-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="04f32-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="04f32-148">Kiszolgálói előfizetések</span><span class="sxs-lookup"><span data-stu-id="04f32-148">Server subscriptions</span></span>

- <span data-ttu-id="04f32-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="04f32-149">Windows Server</span></span>
- <span data-ttu-id="04f32-150">Távoli asztali szolgáltatások (RDS) ügyféllicencek</span><span class="sxs-lookup"><span data-stu-id="04f32-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="04f32-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="04f32-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="04f32-152">Linuxos ISV éves előfizetések</span><span class="sxs-lookup"><span data-stu-id="04f32-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="04f32-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="04f32-153">SUSE Linux</span></span>
- <span data-ttu-id="04f32-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="04f32-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="04f32-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="04f32-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="04f32-156">ISV éves előfizetések</span><span class="sxs-lookup"><span data-stu-id="04f32-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="04f32-157">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="04f32-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="04f32-158">Első lépések</span><span class="sxs-lookup"><span data-stu-id="04f32-158">Getting started</span></span>

<span data-ttu-id="04f32-159">Ha szeretné megtudni, hogy a lehető leggyorsabban hogyan helyezheti el a Azure Reservationst az ügyfelekkel, és hogyan kezdheti el működés közben a lehető leghamarabb, javasoljuk, hogy tekintse át a következő módszert a készültségi anyagok áttekintéséhez:</span><span class="sxs-lookup"><span data-stu-id="04f32-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="04f32-160">Tekintse át az áttekintő bemutatókat és a kapcsolódó webes előadásokat az ügyfél értékének kiosztásához és elhelyezéséhez</span><span class="sxs-lookup"><span data-stu-id="04f32-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="04f32-161">Tekintse át és Ismerje meg a modern kereskedelmi üzemeltetési útmutatót</span><span class="sxs-lookup"><span data-stu-id="04f32-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="04f32-162">Tekintse át az Azure RI és a kiszolgáló előfizetéseit – gyakori kérdések</span><span class="sxs-lookup"><span data-stu-id="04f32-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="04f32-163">A Azure Reservations-és kiszolgálói előfizetések frissítéseinek megismerése a [partner Center API-ban (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="04f32-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="04f32-164">További források</span><span class="sxs-lookup"><span data-stu-id="04f32-164">Resources</span></span>

<span data-ttu-id="04f32-165">Az alábbiakban egy átfogó listát talál az erőforrásokról, amelyek segítségével gyorsan áttekintheti Azure Reservations a partner centeren keresztül:</span><span class="sxs-lookup"><span data-stu-id="04f32-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="04f32-166">Értékesítés készültsége</span><span class="sxs-lookup"><span data-stu-id="04f32-166">Sales readiness</span></span>

- [<span data-ttu-id="04f32-167">Azure Reservations és kiszolgálói előfizetések Azure Hybrid Benefit áttekintéssel</span><span class="sxs-lookup"><span data-stu-id="04f32-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="04f32-168">Értékesítési táblázat</span><span class="sxs-lookup"><span data-stu-id="04f32-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="04f32-169">Partneri gyakori kérdések Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="04f32-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="04f32-170">Partneri gyakori kérdések a Azure Reservations és az SQL-ADATBÁZIShoz</span><span class="sxs-lookup"><span data-stu-id="04f32-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="04f32-171">Távoli asztali szolgáltatások (RDS) ügyfél-hozzáférési licenc (CAL) (közlemény)</span><span class="sxs-lookup"><span data-stu-id="04f32-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="04f32-172">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="04f32-172">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="04f32-173">Kiszolgálói előfizetések</span><span class="sxs-lookup"><span data-stu-id="04f32-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="04f32-174">SQL-adatbázis az Azure-ban – áttekintés</span><span class="sxs-lookup"><span data-stu-id="04f32-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="04f32-175">SQL DB-foglalások (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="04f32-175">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="04f32-176">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="04f32-176">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="04f32-177">SQL felügyelt példánya (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="04f32-177">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="04f32-178">SUSE és Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="04f32-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="04f32-179">Red Hat Linux az Azure-on</span><span class="sxs-lookup"><span data-stu-id="04f32-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="04f32-180">SUSE Linux az Azure-on</span><span class="sxs-lookup"><span data-stu-id="04f32-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="04f32-181">Linux az Azure-ban</span><span class="sxs-lookup"><span data-stu-id="04f32-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="04f32-182">Az Azure díjszabásának áttekintése</span><span class="sxs-lookup"><span data-stu-id="04f32-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="04f32-183">Az Azure díjszabásának kalkulátora</span><span class="sxs-lookup"><span data-stu-id="04f32-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="04f32-184">Azure Databricks egység foglalásai</span><span class="sxs-lookup"><span data-stu-id="04f32-184">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="04f32-185">CSP-árlista: a **Microsoft Azure fenntartott példányok** és a **szoftveres előfizetések** árlista a Partner Center [díjszabási & ajánlatok](https://partner.microsoft.com/pcv/sales) oldalán találhatók.</span><span class="sxs-lookup"><span data-stu-id="04f32-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="04f32-186">Képzés</span><span class="sxs-lookup"><span data-stu-id="04f32-186">Training</span></span>

<span data-ttu-id="04f32-187">Regisztráljon a [kereskedelmi licencelés készültségét ismertető előadások](https://commercial-licensing.eventbuilder.com/FY2019_ALL) és az igény szerinti események megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="04f32-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="04f32-188">A licencelési készültség igény szerinti eseményei többek között a következő témákat tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="04f32-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="04f32-189">CSP Online Services, CSP Azure és általános licencelési frissítések, beleértve az Azure-t (november 2018)</span><span class="sxs-lookup"><span data-stu-id="04f32-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="04f32-190">SQL DB fenntartott kapacitás & példányának rugalmassága (2018. augusztus)</span><span class="sxs-lookup"><span data-stu-id="04f32-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="04f32-191">Kiszolgálói előfizetések a CSP-ben (július 2018)</span><span class="sxs-lookup"><span data-stu-id="04f32-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="04f32-192">Azure Reservations áttekintése a CSP-ben (május 2018)</span><span class="sxs-lookup"><span data-stu-id="04f32-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="04f32-193">Más hasznos képzés magában foglalja a [partner Egyetemen elérhető Azure licencelési modult](https://aka.ms/azure_partner_licensing)is.</span><span class="sxs-lookup"><span data-stu-id="04f32-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="04f32-194">Műveletek</span><span class="sxs-lookup"><span data-stu-id="04f32-194">Operations</span></span>

- <span data-ttu-id="04f32-195">[Modern kereskedelmi üzemeltetési útmutató](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (frissítve): átfogó útmutató A kulcsfontosságú házirendekkel és működési szempontokkal, mint például a szerződések, a partner Center, a számla, az árlista részletei, az ösztönzők, a megbékélési fájl, az API/SDK, a homokozó és az Azure partner megosztott szolgáltatásai.</span><span class="sxs-lookup"><span data-stu-id="04f32-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="04f32-196">A modern ajánlatok ország rendelkezésre állása és az ügyfél pénznemének mátrixa</span><span class="sxs-lookup"><span data-stu-id="04f32-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="04f32-197">Microsoft Azure fenntartott példányok eladása</span><span class="sxs-lookup"><span data-stu-id="04f32-197">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md)
- [<span data-ttu-id="04f32-198">Microsoft Azure foglalások vásárlása az ügyfelek nevében</span><span class="sxs-lookup"><span data-stu-id="04f32-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="04f32-199">Azure-foglalások kezelése az ügyfelek nevében</span><span class="sxs-lookup"><span data-stu-id="04f32-199">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)
- [<span data-ttu-id="04f32-200">Számlázás Azure-foglalásokhoz</span><span class="sxs-lookup"><span data-stu-id="04f32-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="04f32-201">Virtuális gép méretezése a maximális foglalási használathoz</span><span class="sxs-lookup"><span data-stu-id="04f32-201">VM sizing for maximum reservation usage</span></span>](azure-usage.md)
- [<span data-ttu-id="04f32-202">Partneri központ API (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="04f32-202">Partner Center API (API/SDK)</span></span>](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="04f32-203">Távoli asztali szolgáltatások</span><span class="sxs-lookup"><span data-stu-id="04f32-203">Remote Desktop Services</span></span>](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="04f32-204">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="04f32-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="04f32-205">A [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) segítségével több értéket érhet el a Windows Server-licencekben, és akár \* 47%-ot is megtakaríthat a virtuális gépeken.</span><span class="sxs-lookup"><span data-stu-id="04f32-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="04f32-206">A kedvezményt a frissítési garanciával rendelkező Windows Server Datacenter és Standard Edition licenccel is használhatja.</span><span class="sxs-lookup"><span data-stu-id="04f32-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="04f32-207">A kiadástól függően a licenceket a Windows Server rendszerű virtuális gépek Azure-ban való futtatására és az alacsonyabb számítási díj (a linuxos virtuális gépek díjszabása) alapján konvertálhatja vagy használhatja újra.</span><span class="sxs-lookup"><span data-stu-id="04f32-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="04f32-208">Lásd még [Azure Hybrid BENEFIT GYIK](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="04f32-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="04f32-209">\* A tényleges megtakarítás a régió, a példány típusa vagy a használat alapján változhat.</span><span class="sxs-lookup"><span data-stu-id="04f32-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
