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
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a>Azure Reserved VM instances (RI) + kiszolgáló-előfizetések beolvasása, kiépítése, & kezelése

A következőkre vonatkozik:

- Partnerközpont

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Globális rendszergazda
- Segélyszolgálat ügynöke
- Értékesítési ügynök
- Felhasználói felügyeleti rendszergazda

> [!NOTE]
> Ez a cikk csak a Cloud Solution Provider (CSP) programban található partnerekre vonatkozik. A más típusú előfizetéseket (például az utólagos elszámolású, az egyéni, a Microsoft-ügyféli szerződést vagy a Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek Ehelyett olvasniuk kell [Az Azure foglalási dokumentációját](/azure/cost-management-billing/reservations).


## <a name="what-are-azure-reservations"></a>Mi az az Azure Reservations?

Azure Reservations a virtuális gép egy-vagy hároméves, SQL Database számítási kapacitásának, Azure Cosmos DB átviteli sebességének vagy más Azure-erőforrásoknak az előzetes kifizetésével segítheti a pénz megtakarítását. Az előzetes fizetés lehetővé teszi, hogy kedvezményt kapjon a felhasznált erőforrásokhoz. A foglalások jelentősen csökkenthetik a virtuális gépeket, az SQL Database számítási, Azure Cosmos DB és egyéb erőforrás-költségeit akár 72%-kal az utólagos elszámolású árakhoz képest. A Reservations számlázási kedvezményt nyújt, és nincs hatással az erőforrások futtatási állapotára. További információ: [Mi a Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)

## <a name="why-should-customers-buy-a-reservation"></a>Miért vásárolnak az ügyfelek foglalást?

Ha az ügyfelek olyan virtuális gépeket, Azure Cosmos DB vagy SQL-adatbázisokat foglalnak magukban, amelyek hosszú ideig futnak, a foglalás megvásárlása a leghatékonyabb megoldást kínálja. Ha például egy ügyfél a szolgáltatás négy példányát egy foglalás nélkül futtatja, akkor az utólagos elszámolású díjszabásban kell fizetni. Ha foglalást vásárol az adott erőforráshoz, azonnal megkapja a foglalási kedvezményt. Az erőforrásokért ezután nem használatalapú fizetéses díjakat kell fizetnie.

### <a name="compelling-new-azure-offer-in-csp"></a>Lenyűgöző új Azure-ajánlat a CSP-ben

A Azure Reservations-és kiszolgáló-előfizetések CSP programba való bevonásával a Microsoft jobb lehetőséget biztosít partnerei számára, hogy a gyors ütemben növekvő ügyfelek számára költséghatékony megoldásokat kínáljon a nagy mértékben kiszámítható, állandó Felhőbeli számítási feladatok támogatásához. A CSP program lehetővé teszi, hogy a partnerek a kereskedelmi ügyfelek nevében beszerezzék, kiépítsék és kezeljék Azure Reservations és kiszolgálói előfizetéseket a Microsoft partner Center és a Azure Portal használatával.

Az Azure-foglalások megvásárlásának módjáról is biztosítunk partnereket a CSP programban. A CSP-partnerek az [ügyfelek nevében vásárolhatnak Azure-foglalásokat](azure-reservations-buying.md) , és [lehetővé tehetik, hogy az ügyfél megvásárolja a saját foglalásait](give-customers-permission.md) egy korábbi Azure-előfizetésből, amelyet a partner megvásárolt.

Azure Reservations az ügyfelek számára a virtualizáció rugalmasságát számos számítástechnikai megoldás esetében, beleértve a fejlesztést és tesztelést, az alkalmazások futtatását és az adatközpont kiterjesztését.

A [Azure Reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) például a kereskedelmi ügyfeleink akár 72%-ot is megtakarítanak, és az utólagos elszámolású Azure-beli virtuális gépek díjszabását egyszerűen megvásárolhatja, vagy "lefoglalhatja" a virtuális gépet egy 1 vagy 3 éves időszakra. A frissítési garanciával rendelkező Windows Server rendszerű ügyfelek a Azure Hybrid Benefit akár 80%-ot is megtakarítanak, az utólagos elszámolású díjszabást is beleértve.

A kényszerített árképzés és a páratlan üzembe helyezési rugalmasság páratlan kombinációja esetén az ügyfelek a legjobb általános értéket fogják látni, amikor a Azure Reservations választják:

#### <a name="azure-reservations"></a>Azure Reserved Virtual Machine Instances

- Azure Reserved VM Instances
- SQL DB-foglalások
- SQL Managed Instance
- Azure Cosmos DB
- Azure SQL Data Warehouse
- App Services
- Azure Databricks egység foglalásai
- Felügyelt lemez
- Blokkblob
- MySQL
- Azure-adatkezelő
- MariaDB
- PostgreSQL

#### <a name="server-subscriptions"></a>Kiszolgálói előfizetések

- Windows Server
- Távoli asztali szolgáltatások (RDS) ügyféllicencek
- SQL Server

#### <a name="linux-isv-annual-subscriptions"></a>Linuxos ISV éves előfizetések

- SUSE Linux
- Red Hat Enterprise Linux
- Azure Red Hat OpenShift

#### <a name="isv-annual-subscriptions"></a>ISV éves előfizetések

- Azure VMware Solution by CloudSimple

## <a name="getting-started"></a>Első lépések

Ha szeretné megtudni, hogy a lehető leggyorsabban hogyan helyezheti el a Azure Reservationst az ügyfelekkel, és hogyan kezdheti el működés közben a lehető leghamarabb, javasoljuk, hogy tekintse át a következő módszert a készültségi anyagok áttekintéséhez:

1. Tekintse át az áttekintő bemutatókat és a kapcsolódó webes előadásokat az ügyfél értékének kiosztásához és elhelyezéséhez
2. Tekintse át és Ismerje meg a modern kereskedelmi üzemeltetési útmutatót
3. Tekintse át az Azure RI és a kiszolgáló előfizetéseit – gyakori kérdések
4. A Azure Reservations-és kiszolgálói előfizetések frissítéseinek megismerése a [partner Center API-ban (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)

## <a name="resources"></a>További források

Az alábbiakban egy átfogó listát talál az erőforrásokról, amelyek segítségével gyorsan áttekintheti Azure Reservations a partner centeren keresztül:

### <a name="sales-readiness"></a>Értékesítés készültsége

- [Azure Reservations és kiszolgálói előfizetések Azure Hybrid Benefit áttekintéssel](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [Értékesítési táblázat](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [Partneri gyakori kérdések Azure Reservations](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [Partneri gyakori kérdések a Azure Reservations és az SQL-ADATBÁZIShoz](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [Távoli asztali szolgáltatások (RDS) ügyfél-hozzáférési licenc (CAL) (közlemény)](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [Azure Reserved VM Instances (Azure Portal)](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [Kiszolgálói előfizetések](csp-software-subscriptions.md)
- [SQL-adatbázis az Azure-ban – áttekintés](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
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
- CSP-árlista: a **Microsoft Azure fenntartott példányok** és a **szoftveres előfizetések** árlista a Partner Center [díjszabási & ajánlatok](https://partner.microsoft.com/pcv/sales) oldalán találhatók.

### <a name="training"></a>Képzés

Regisztráljon a [kereskedelmi licencelés készültségét ismertető előadások](https://commercial-licensing.eventbuilder.com/FY2019_ALL) és az igény szerinti események megtekintéséhez.

A licencelési készültség igény szerinti eseményei többek között a következő témákat tartalmazzák:

- CSP Online Services, CSP Azure és általános licencelési frissítések, beleértve az Azure-t (november 2018)
- SQL DB fenntartott kapacitás & példányának rugalmassága (2018. augusztus)
- Kiszolgálói előfizetések a CSP-ben (július 2018)
- Azure Reservations áttekintése a CSP-ben (május 2018)

Más hasznos képzés magában foglalja a [partner Egyetemen elérhető Azure licencelési modult](https://aka.ms/azure_partner_licensing)is.

### <a name="operations"></a>Műveletek

- [Modern kereskedelmi üzemeltetési útmutató](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (frissítve): átfogó útmutató A kulcsfontosságú házirendekkel és működési szempontokkal, mint például a szerződések, a partner Center, a számla, az árlista részletei, az ösztönzők, a megbékélési fájl, az API/SDK, a homokozó és az Azure partner megosztott szolgáltatásai.
- [A modern ajánlatok ország rendelkezésre állása és az ügyfél pénznemének mátrixa](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [Microsoft Azure fenntartott példányok eladása](azure-reservations.md)
- [Microsoft Azure foglalások vásárlása az ügyfelek nevében](azure-reservations-buying.md)
- [Azure-foglalások kezelése az ügyfelek nevében](azure-reservations-manage.md)
- [Számlázás Azure-foglalásokhoz](azure-plan-billing.md)
- [Virtuális gép méretezése a maximális foglalási használathoz](azure-usage.md)
- [Partneri központ API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [Távoli asztali szolgáltatások](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a>Azure Hybrid Benefit

A [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) segítségével több értéket érhet el a Windows Server-licencekben, és akár * 47%-ot is megtakaríthat a virtuális gépeken. A kedvezményt a frissítési garanciával rendelkező Windows Server Datacenter és Standard Edition licenccel is használhatja. A kiadástól függően a licenceket a Windows Server rendszerű virtuális gépek Azure-ban való futtatására és az alacsonyabb számítási díj (a linuxos virtuális gépek díjszabása) alapján konvertálhatja vagy használhatja újra.

Lásd még [Azure Hybrid BENEFIT GYIK](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

* A tényleges megtakarítás a régió, a példány típusa vagy a használat alapján változhat.
