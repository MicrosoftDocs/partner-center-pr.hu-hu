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
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a>Azure-beli fenntartott virtuálisgép& példányok (RI) és kiszolgáló-előfizetések vásárlása, kiépítése és kezelése az ügyfelek számára


**Megfelelő szerepkörök:** Rendszergazdai ügynök | Globális rendszergazdai | Az | Értékesítési ügynök | Felhasználókezelő rendszergazda


## <a name="what-are-azure-reservations"></a>Mi az az Azure Reservations?

Az Azure Reservations segítségével pénzt takaríthat meg, ha előre fizet egy vagy három évnyi virtuális gépért, SQL Database számítási kapacitásért, Azure Cosmos DB átviteli sebességért vagy más Azure-erőforrásokért. Az előzetes fizetés lehetővé teszi, hogy kedvezményt kap a használt erőforrásokra. A Reservations jelentősen csökkentheti a virtuális gép, az SQL Database számítási, Azure Cosmos DB- és egyéb erőforrások költségeit akár 72%-kal a használat alapján fizetett árakhoz képest. A Reservations számlázási kedvezményt nyújt, és nincs hatással az erőforrások futtatási állapotára. További információ: [Mi az az Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)

## <a name="why-should-customers-buy-a-reservation"></a>Miért érdemes az ügyfeleknek foglalást vásárolniuk?

Ha az ügyfelek olyan virtuális gépekkel, Azure Cosmos DB vagy SQL-adatbázisokkal futnak, amelyek hosszú ideig futnak, a foglalás megvásárlása biztosítja számukra a legköltséghatékosabb megoldást. Ha például egy ügyfél folyamatosan futtatja egy szolgáltatás négy példányát foglalás nélkül, használat alapján kell fizetnie. Ha ezekhez az erőforrásokhoz vásárolnak foglalást, azonnal kapják meg a foglalási kedvezményt. Az erőforrásokért ezután nem használatalapú fizetéses díjakat kell fizetnie.

### <a name="compelling-new-azure-offer-in-csp"></a>Lenyűgöző új Azure-ajánlat a CSP-ban

Azáltal, hogy az Azure Reservationst és a Kiszolgáló-előfizetéseket a CSP-programba teszi, a Microsoft jobban teszi lehetővé a partnerek számára, hogy a rendkívül kiszámítható, állandó felhőalapú számítási feladatok támogatásához költséghatékonyabb megoldások iránti egyre növekvő ügyféligényeket elégednek ki. A CSP-program lehetővé teszi a partnerek számára az Azure Reservations- és Server-előfizetések a Kereskedelmi ügyfelek nevében történő megszerzését, üzembe Partnerközpont és Azure Portal.
Még azt is megadjuk a CSP-programunk partnereinek, hogy hogyan vásárolhatók meg az Azure-foglalások. A CSP-partnerek [vásárolhatnak Azure-foglalásokat](azure-reservations-buying.md) egy [](give-customers-permission.md) ügyfél nevében, vagy engedélyezhetik, hogy az ügyfél megvásárolja a saját foglalását egy korábbi Azure-előfizetésből, amit a partner megvásárolt számukra.

Az Azure Reservations rugalmasságot biztosít az ügyfeleknek a különböző számítástechnikai megoldások virtualizálásában, beleértve a fejlesztést és tesztelést, az alkalmazások futtatását és az adatközpont kibővítését.

A [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) esetében például a kereskedelmi ügyfelek akár 72%-ot is megtakaríthatnak a használat alapján fizetett Azure-beli virtuális gépek díjszabásával szemben, ha egy 1 vagy 3 éves időszakra megvásárolják a virtuális gépet . A windowsos Azure Hybrid Benefit és Frissítési Garancia ügyfelek akár 80%-kal is pénzt takaríthatnak meg a fizetéses díjszabással szemben.

A lenyűgöző díjszabás és a nem egyező üzembe helyezési rugalmasság egyedülálló kombinációjával az ügyfelek az Azure Reservations kiválasztásakor a legjobb általános értéket látják.

- Lásd: [Foglalások vásárlása](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) az Azure Portalon.

- A **szoftver-előfizetésekért** és a Linux ISV éves előfizetéseiért tekintse meg az Azure RI CSP kereskedelmi árlistát a **Microsoft Azure Reserved Instances** (Fenntartott példányok) kategória Partnerközpont Díjszabás és ajánlatok lapján. [](https://partner.microsoft.com/dashboard/sell/pricingandoffers)


 
**Linux ISV éves előfizetések**

- SUSE Linux
- Red Hat Enterprise Linux
- Azure Red Hat OpenShift

**ISV éves előfizetések**

- Azure VMware Solution by CloudSimple

## <a name="getting-started"></a>Első lépések

Annak érdekében, hogy megértsük, hogyan tudja az Azure Reservationst az ügyfelekkel együtt helyezze el, és hogyan tud a lehető leggyorsabban üzemelni, a következő megközelítést javasoljuk a készültségi anyagok áttekintésére:

1. Tekintse át és Partnerközpont [új kereskedelmi műveletek útmutatóját.](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)

2. Az Azure Reservations és a Server Subscriptions frissítéseit az [Partnerközpont API(API/SDK) szolgáltatásban értheti](/partner-center/develop/purchase-azure-reserved-vm-instances)meg.


### <a name="sales-readiness"></a>Értékesítési készenlét

- [Távoli asztali szolgáltatások (RDS) ügyfél-hozzáférési licenc (CAL) (közlemény)](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [Azure Reserved VM Instances (Azure Portal)](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [Kiszolgáló-előfizetések](./csp-software-subscriptions.md)

- [SQL DB Reservations (Azure Portal)](/azure/sql-database/sql-database-reserved-capacity)

- [Azure Cosmos DB (Azure Portal)](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [SQL Managed Instance (Azure Portal)](/azure/sql-database/sql-database-managed-instance)

- [SUSE és Red Hat Enterprise Linux (Azure Portal)](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [Red Hat Linux az Azure-ban](https://azure.com/redhat)

- [SUSE Linux az Azure-on](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [Linux az Azure-ban](https://azure.microsoft.com/overview/linux-on-azure/)

- [Az Azure díjszabásának áttekintése](https://azure.microsoft.com/pricing/)

- [Azure díjkalkulátor](https://azure.microsoft.com/pricing/calculator)

- [Azure Databricks egységfoglalások](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a>Oktatás

Regisztráljon a kereskedelmi [licencelési készenlét webináriumok és](https://commercial-licensing.eventbuilder.com/FY2019_ALL) igény szerinti események megtekintéséhez.
A korábban rögzített, igény szerinti licencelésre való készenlétről szóló események a következő témaköröket tartalmazzák:

- CSP Online Services, CSP Azure és általános licencelési frissítések, beleértve az Azure-t (2018. november)

- Fenntartott SQL DB-& példányméret-rugalmasság (2018. augusztus)

- Kiszolgáló-előfizetések a CSP-ben (2018. július)

- Az Azure Reservations áttekintése a CSP-ben (2018. május)

## <a name="operations"></a>Üzemeltetés

[Partnerközpont](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)új kereskedelmi műveletek útmutatója: Átfogó útmutató az olyan kulcsfontosságú szabályzatokról és működési szempontokról, mint a szerződések, a rendelés Partnerközpont, a számla, az árlista részletei, az ösztönzők, az egyeztetési fájl, az API/SDK, a Azure Partner Shared Services.

## <a name="azure-hybrid-benefit"></a>Azure Hybrid Benefit

A [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) az Frissítési Garancia-licenccel rendelkező ügyfelek számára díjszabási kedvezmény, amely segít maximalizálni a meglévő helyszíni Windows Server- és/vagy SQL Server-licencbefektetések értékét az Azure-ba való miálás során. A jogosult ügyfelek akár 40%-ot* is megtakaríthat az Azure Virtual Machines-ban (szolgáltatásként elérhető infrastruktúra vagy IaaS), és akár 55%-ot is megtakaríthat Azure SQL Database-ban (szolgáltatásként elérhető platform vagy PaaS) és SQL Server-t az Azure Virtual Machines-ben (IaaS) az Azure Hybrid Benefit-sel, ami akár 80%-kal is nő az Azure-beli fenntartott példányokkal együtt.

## <a name="next-steps"></a>Következő lépések

- [Azure Hybrid Benefit – GYIK](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

*A tényleges megtakarítás régiónként, példánytípustól vagy használattól függően változhat.