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
ms.openlocfilehash: 1d5386dd4b2b19e641cc9d731d4a3d0f44ab5ad6
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182494"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a>Azure Reserved VM instances (RI) + kiszolgáló-előfizetések beolvasása, kiépítése, & kezelése


**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Globális rendszergazda
- Segélyszolgálat ügynöke
- Értékesítési ügynök
- Felhasználói felügyeleti rendszergazda


## <a name="what-are-azure-reservations"></a>Mi az az Azure Reservations?

Azure Reservations a virtuális gép egy-vagy hároméves, SQL Database számítási kapacitásának, Azure Cosmos DB átviteli sebességének vagy más Azure-erőforrásoknak az előzetes kifizetésével segítheti a pénz megtakarítását. Az előzetes fizetés lehetővé teszi, hogy kedvezményt kapjon a felhasznált erőforrásokhoz. A foglalások jelentősen csökkenthetik a virtuális gépeket, az SQL Database számítási, Azure Cosmos DB és egyéb erőforrás-költségeit akár 72%-kal az utólagos elszámolású árakhoz képest. A Reservations számlázási kedvezményt nyújt, és nincs hatással az erőforrások futtatási állapotára. További információ: [Mi a Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)

## <a name="why-should-customers-buy-a-reservation"></a>Miért vásárolnak az ügyfelek foglalást?

Ha az ügyfelek olyan virtuális gépeket, Azure Cosmos DB vagy SQL-adatbázisokat foglalnak magukban, amelyek hosszú ideig futnak, a foglalás megvásárlása a leghatékonyabb megoldást kínálja. Ha például egy ügyfél a szolgáltatás négy példányát egy foglalás nélkül futtatja, akkor az utólagos elszámolású díjszabásban kell fizetni. Ha foglalást vásárol az adott erőforráshoz, azonnal megkapja a foglalási kedvezményt. Az erőforrásokért ezután nem használatalapú fizetéses díjakat kell fizetnie.

### <a name="compelling-new-azure-offer-in-csp"></a>Lenyűgöző új Azure-ajánlat a CSP-ben

A Azure Reservations-és kiszolgáló-előfizetések CSP programba való bevonásával a Microsoft jobb lehetőséget biztosít partnerei számára, hogy a gyors ütemben növekvő ügyfelek számára költséghatékony megoldásokat kínáljon a nagy mértékben kiszámítható, állandó Felhőbeli számítási feladatok támogatásához. A CSP program lehetővé teszi, hogy a partnerek a kereskedelmi ügyfelek nevében beszerezzék, kiépítsék és kezeljék Azure Reservations és kiszolgálói előfizetéseket a Microsoft partner Center és a Azure Portal használatával.
Az Azure-foglalások megvásárlásának módjáról is biztosítunk partnereket a CSP programban. A CSP-partnerek az [ügyfelek nevében vásárolhatnak Azure-foglalásokat](azure-reservations-buying.md) , és [lehetővé tehetik, hogy az ügyfél megvásárolja a saját foglalásait](give-customers-permission.md) egy korábbi Azure-előfizetésből, amelyet a partner megvásárolt.

Azure Reservations az ügyfelek számára a virtualizáció rugalmasságát számos számítástechnikai megoldás esetében, beleértve a fejlesztést és tesztelést, az alkalmazások futtatását és az adatközpont kiterjesztését.

A [Azure Reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) például a kereskedelmi ügyfeleink akár 72%-ot is megtakarítanak, és az utólagos elszámolású Azure-beli virtuális gépek díjszabását egyszerűen megvásárolhatja, vagy "lefoglalhatja" a virtuális gépet egy 1 vagy 3 éves időszakra. A frissítési garanciával rendelkező Windows Server rendszerű ügyfelek a Azure Hybrid Benefit akár 80%-ot is megtakarítanak, az utólagos elszámolású díjszabást is beleértve.

A kényszerített árképzés és a páratlan üzembe helyezési rugalmasság páratlan kombinációja esetén az ügyfelek a legjobb általános értéket fogják látni, amikor kiválasztják Azure Reservations.

- Az Azure Portalon megjelenő [vásárlási foglalások](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) .

- Tekintse meg az **Azure ri CSP kereskedelmi díjszabását** a **Microsoft Azure fenntartott példányok** kategóriájában a következő témakörben: a partner Center [díjszabási és ajánlatok](https://partner.microsoft.com/dashboard/sell/pricingandoffers) lapján a szoftveres előfizetések és a Linux ISV éves előfizetések


 
**Linuxos ISV éves előfizetések**

- SUSE Linux
- Red Hat Enterprise Linux
- Azure Red Hat OpenShift

**ISV éves előfizetések**

- Azure VMware Solution by CloudSimple

## <a name="getting-started"></a>Első lépések

Ha szeretné megtudni, hogy a lehető leggyorsabban hogyan helyezheti el a Azure Reservationst az ügyfelekkel, és hogyan kezdheti el működés közben a lehető leghamarabb, javasoljuk, hogy tekintse át a következő módszert a készültségi anyagok áttekintéséhez:

1. Tekintse át és Ismerje meg a [partner Center új kereskedelmi üzemeltetési útmutatóját](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).

2. A Azure Reservations-és kiszolgálói előfizetések frissítéseinek megismerése a [partner Center API-ban (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).


### <a name="sales-readiness"></a>Értékesítés készültsége

- [Távoli asztali szolgáltatások (RDS) ügyfél-hozzáférési licenc (CAL) (közlemény)](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [Azure Reserved VM Instances (Azure Portal)](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [Kiszolgálói előfizetések](./csp-software-subscriptions.md)

- [SQL DB-foglalások (Azure Portal)](/azure/sql-database/sql-database-reserved-capacity)

- [Azure Cosmos DB (Azure Portal)](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [SQL felügyelt példánya (Azure Portal)](/azure/sql-database/sql-database-managed-instance)

- [SUSE és Red Hat Enterprise Linux (Azure Portal)](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [Red Hat Linux az Azure-on](https://azure.com/redhat)

- [SUSE Linux az Azure-on](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [Linux az Azure-ban](https://azure.microsoft.com/overview/linux-on-azure/)

- [Az Azure díjszabásának áttekintése](https://azure.microsoft.com/pricing/)

- [Az Azure díjszabásának kalkulátora](https://azure.microsoft.com/pricing/calculator)

- [Azure Databricks egység foglalásai](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a>Képzés

Regisztráljon a [kereskedelmi licencelés készültségét ismertető előadások](https://commercial-licensing.eventbuilder.com/FY2019_ALL) és az igény szerinti események megtekintéséhez.
A korábban rögzített licencelési készültség az igény szerinti eseményeknél többek között a következő témaköröket tartalmazza:

- CSP Online Services, CSP Azure és általános licencelési frissítések, beleértve az Azure-t (november 2018)

- SQL DB fenntartott kapacitás & példányának rugalmassága (2018. augusztus)

- Kiszolgálói előfizetések a CSP-ben (július 2018)

- Azure Reservations áttekintése a CSP-ben (május 2018)

## <a name="operations"></a>Műveletek

A [partner Center új kereskedelmi üzemeltetési útmutatója](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf): átfogó útmutató, amely tartalmazza a legfontosabb házirendeket és üzemeltetési szempontokat, például a szerződések, a partneri központ, a számla, az árlista részletei, az ösztönzők, a megbékélési fájl, az API/SDK, a homokozó és az Azure partner megosztott szolgáltatásait.

## <a name="azure-hybrid-benefit"></a>Azure Hybrid Benefit

A [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) a frissítési garanciával rendelkező ügyfeleinknek szóló díjszabási kedvezmény, amely segít maximalizálni a meglévő helyszíni Windows Server-és/vagy SQL Server-licencek értékét az Azure-ba való Migrálás során. A jogosult ügyfeleknek akár 40%-ot is megtakaríthat az Azure Virtual Machines (infrastruktúra-szolgáltatásként vagy IaaS), és akár 55%-ot is megtakaríthat Azure SQL Database (platform as szolgáltatásként vagy Péterként), és SQL Server az Azure Virtual Machines (IaaS Azure Hybrid Benefit) szolgáltatással, amely az Azure-beli fenntartott példányokkal együtt akár 80%-ra is nő.

## <a name="next-steps"></a>Következő lépések

- [Azure Hybrid Benefit – GYIK](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

* A tényleges megtakarítás a régió, a példány típusa vagy a használat alapján változhat.