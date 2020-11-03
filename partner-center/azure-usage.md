---
title: Azure-beli virtuális gép méretezése a maximális foglalási kihasználtsághoz
description: Megtudhatja, hogyan méretezhető a virtuális gép (VM) az ügyfelek számítástechnikai igényeire, ha Microsoft Azure foglalásokat vásárol hozzájuk.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: e6c4e3e7a68de720f586754703308a447d7d30c1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529904"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Microsoft Azure-beli virtuális gép méretezése a maximális foglalási kihasználtsághoz

**A következőkre vonatkozik**

- Partnerközpont
- Azure Portal
- Partnerek a CSP programban
 
> [!NOTE]
> Ez a cikk csak a Cloud Solution Provider (CSP) programban található partnerekre vonatkozik. A más típusú előfizetéseket (például az utólagos elszámolású, az egyéni, a Microsoft-ügyféli szerződést vagy a Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek Ehelyett olvasniuk kell [Az Azure foglalási dokumentációját](/azure/cost-management-billing/reservations).

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>A virtuális gép méretének meghatározása az ügyfél Azure-beli foglalásához

Microsoft Azure foglalásoknak az ügyfelek nevében történő megvásárlásakor ki kell választania egy virtuális gépet (VM), amely megfelel az ügyfél számítástechnikai igényeinek. Ezeket az adatokat a következő módszerek egyikével keresheti meg:

- Azure-kihasználtság API
- Azure Portal
- Azure PowerShell
- A Azure Resource Manager (ARM) API

Az egyes módszerek használatára vonatkozó utasítások alább láthatók. A foglalás megvásárlása után a rendszer automatikusan alkalmazza a foglalási kedvezményt a foglalás attribútumait és mennyiségét megegyező virtuális gépekre. Nem kell hozzárendelni a foglalást egy virtuális géphez.

>[!NOTE]
>A foglalási kedvezmények nem vonatkoznak a klasszikus és a promóciós virtuális gépekre.

>[!IMPORTANT]
>Az ügyfél nevében megvásárolni kívánt virtuális gép típusának és méretének megfelelő azonosításához az alábbiakban ismertetett módszerek egyikét kell használnia, mivel a virtuálisgép-sorozat típusa nem megfelelően jelenik meg a partner Center egyeztetési fájljaiban.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>VM-méretezési információk beolvasása az Azure-kihasználtság API használatával

1. A megvásárolni kívánt virtuálisgép-méret azonosításához használja a ServiceType attribútum értékét a additionalInfo elemben az API-válaszban.

2. További információ: [ügyfél kihasználtsági rekordjainak beszerzése az Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) -hoz a [partner Center API](/partner-center/develop/)-ban.

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>VM-méretezési információk beolvasása a Microsoft Azure Portal használatával

1. A partner Centerben lépjen az **ügyfelek** oldalra.

2. Keresse meg azt az ügyfelet, aki szeretné megvásárolni az Azure-beli virtuális gépek foglalását, majd a lefelé mutató nyílra kattintva bontsa ki az ügyfél adatait. Válassza a **a Microsoft Azure felügyeleti portálja** lehetőséget az ügyfél rekordjának megnyitásához a Azure Portal.

3. Válassza a portál menüben a **virtuális gépek** lehetőséget, majd válassza ki azt a virtuális gépet, amelyhez foglalást szeretne vásárolni.

4. A virtuális gép részletei lapon keresse meg a méret és a régió adatait az alábbi ábrán látható módon, és használja ezt az információt a foglalás megvásárlásához a partner Centerben.  

   :::image type="content" source="images/usage1.png" alt-text="A méret és a régió adatai a Részletek lapon":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>VM-méretezési információk beolvasása Microsoft Azure PowerShell használatával

Az alábbi képen található információk segítségével megtekintheti annak a virtuális gépnek a helyét és méretét, amelyhez foglalást kíván vásárolni. 

:::image type="content" source="images/usage2.png" alt-text="A méret és a régió adatai a Részletek lapon":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>VM-méretezési információk beolvasása a Azure Resource Manager (ARM) API használatával

1. A ARMClient vagy az ARM API-k használatával hívja meg az ARM-ügyfelet arra a virtuális gépre, amelyhez foglalást kíván vásárolni.

2. /Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-Version = 2017-12-01

3. A hívás az alább látható módon visszaadja a **vmSize** és a **hely** értékét.

    :::image type="content" source="images/usage3.png" alt-text="A méret és a régió adatai a Részletek lapon":::
    :::image type="content" source="images/usage4.png" alt-text="A méret és a régió adatai a Részletek lapon":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Azure-beli virtuális gépek használatának és foglalási kedvezményének ellenőrzése

Miután megvásárolta az Azure-beli fenntartott VM-példányt az ügyfél nevében, a rendszer automatikusan alkalmazza a virtuális gép területének kifizetésére vonatkozó kedvezményt az ügyfél foglalásának attribútumait és mennyiségét megegyező virtuális gépekre.

A következő módszerek egyikével ellenőrizheti az ügyfél foglalási használatát, és megtekintheti, hogy mely virtuális gépekre vonatkoznak a foglalási kedvezmények:

- Azure Portal
- Azure-kihasználtság API

Az egyes módszerek használatára vonatkozó utasítások alább láthatók.

>[!NOTE]
>Csak az Azure kihasználtsági API jeleníti meg, hogy a rendszer melyik virtuális gépre alkalmazza a kedvezményt.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Az ügyfél foglalási használatának ellenőrzése a Microsoft Azure Portalban

1. A partner Centerben lépjen az **ügyfelek** oldalra.

2. Keresse meg azt az ügyfelet, akinek a foglalási kedvezményét és felhasználását ellenőrizni szeretné, majd a lefelé mutató nyílra kattintva bontsa ki az ügyfél adatait. Válassza a **a Microsoft Azure felügyeleti portálja** lehetőséget az ügyfél rekordjának megnyitásához a Azure Portal.
3. Válassza a portál menüben a **foglalások** lehetőséget, majd válassza ki azt a foglalást, amelynek a használatát ellenőriznie szeretné.
4. Az **Áttekintés** oldalon tekintse meg a foglalás kihasználtsága diagramot, amely azt mutatja, hogy a foglalás mekkora része lett alkalmazva a virtuális gépekre.

    >[!NOTE]
    >A kihasználtsági adatai akár 8 óráig is késleltethető.

    a. Ha a foglalás kihasználtsága 100%, az ügyfél minden lehetséges megtakarítást biztosít, amelyet a foglalás megvásárlása tud biztosítani.
    b. Ha a foglalás kihasználtsága 0%, a rendszer nem alkalmazza a kedvezményt egyetlen virtuális gépre sem.
    c. Ha a foglalás kihasználtsága 1% és 99% között van, akkor nem használhatók előnyök.

5. Ennek elkerüléséhez határozza meg a megfelelő méretű virtuális gépet, hogy támogassa az ügyfél számítástechnikai igényeit a vásárlás előtt.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Az ügyfél foglalási használatának ellenőrzése az Azure kihasználtsági API-val

>[!NOTE]
>Csak az Azure kihasználtsági API jeleníti meg, hogy a rendszer melyik virtuális gépre alkalmazza a kedvezményt.  

Lekérheti a foglalási használati adatokat az Azure kihasználtsági API-val annak ellenőrzéséhez, hogy az ügyfél beolvasta-e a foglalási kedvezményt, és hogy a rendszer mely virtuális gépeket (Virtual machines) alkalmazza a kedvezményre. Hasonlítsa össze a példát a B példával, hogy megtekintse, hogyan ellenőrizheti az ügyfél foglalási felhasználását.

:::image type="content" source="images/usage5.png" alt-text="A méret és a régió adatai a Részletek lapon":::

- A reservationId azonosítja azt az Azure-foglalást, amelyet a kedvezmény a virtuális gépre való alkalmazásához használt.
- a consumptionMeter annak a virtuális gépnek a MeterId, amelyhez a foglalási kedvezmény vonatkozik.
- A ReservationMeter a foglalási kedvezmény alkalmazása óta $0 költségeket mutat.

További információ: [ügyfél kihasználtsági rekordjainak beszerzése az Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) -hoz a [partner Center API](/partner-center/develop/)-ban.

>[!IMPORTANT]
>A szoftveres költségek, mint például a Microsoft Windows Server, jelenleg nem szerepelnek a virtuális gépek foglalásának árán, és külön sorokként jelennek meg a rendelési rekordban és a számlán. Ha azonban az ügyfél rendelkezik a Azure Hybrid Use Benefitval, a rendszer nem alkalmazza a szoftverre vonatkozó költségeket. További információ: [a Windows-szoftverek nem tartalmazzák a fenntartott példányokat](/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Azure-foglalások erőforrásai

|**További információ**   |**Olvassa el ezt**    |
|:-----------------------------|:-----------------|
|Azure-foglalások a CSP-ben – áttekintés  | [Microsoft Azure fenntartott VM-példányok eladása](azure-reservations.md)
|Azure-foglalások vásárlása az ügyfelek számára a partner Centerben   | [Azure-foglalások vásárlása](azure-reservations-buying.md)
|Azure-foglalások kezelése a partner Centerben | [Azure-foglalások kezelése a partner Centerben](azure-reservations-manage.md)
|Azure-foglalások megvásárlása a Azure Portal | [Fizetős virtuális gépek esetén Azure Reserved VM instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) az Azure súgójában |
|Azure-foglalások kezelése a Azure Portalban   | [Fenntartott VM-példányok kezelése](/azure/billing/billing-manage-reserved-vm-instance) az Azure súgójában  |
|Azure-foglalások vásárlása a partner Center API használatával | [Vásárlás Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) a partner Center fejlesztői dokumentációjában   |
|Lehetővé teszi, hogy az ügyfelek megvásárolják saját Azure-foglalásait a számukra megvásárolt előfizetésből. | [Engedélyt ad az ügyfeleknek a saját Azure-foglalások megvásárlására](give-customers-permission.md)   |