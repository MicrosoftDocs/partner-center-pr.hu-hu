---
title: Azure-beli virtuális gép méretezése a maximális foglalási kihasználtsághoz
description: Megtudhatja, hogyan méretez egy virtuális gépet (VM) az ügyfelek számítási igényei szerint, amikor Microsoft Azure vásárol számukra.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 2d8bc76e0da51abf433e49028445b398c6a1db31
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276994"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Microsoft Azure-beli virtuális gép méretezése a maximális foglalási kihasználtsághoz

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Értékesítési ügynök

Ez a cikk azt ismerteti, hogyan méretez egy virtuális gépet (VM) az ügyfelek számítási igényeihez, amikor Microsoft Azure vásárol számukra.
 
> [!NOTE]
> Ez a cikk csak a Felhőszolgáltató (CSP) program partnereire vonatkozik. A más típusú előfizetéseket (például használat alapján fizetett, egyéni, Microsoft Ügyfélszerződés- vagy Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek érdemes elolvasni az [Azure Reservations dokumentációját.](/azure/cost-management-billing/reservations)

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Az ügyfél Azure-foglalásának virtuálisgép-méretének meghatározása

Ha Microsoft Azure ügyfelek nevében vásárol foglalásokat, ki kell választania egy virtuális gépet, amely megfelel az ügyfél számítási igényeinek. Ezeket az információkat az alábbi módszerek egyikével találhatja meg:

- Azure-kihasználtsági API
- Azure Portal
- Azure PowerShell
- Az Azure Resource Manager (ARM) API

Az egyes módszerek használatának utasításai alább olvashatók. A foglalás vásárlása után a foglalási kedvezmény automatikusan alkalmazva lesz a foglalás attribútumainak és mennyiségének megfelelő virtuális gépekre. Nem kell hozzárendelni a foglalást egy virtuális géphez.

>[!NOTE]
>A foglalási kedvezmények nem vonatkoznak a klasszikus vagy promóciós virtuális gépekre.

>[!IMPORTANT]
>Az ügyfél nevében megvásárolni kívánt virtuális gép típusának és méretének helyes azonosításához az alább ismertetett módszerek egyikét kell használnia, mivel a virtuálisgép-sorozat típusa helytelenül jelenik meg az egyeztetési Partnerközpont fájlokban.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Virtuális gépek méretezési információinak lekérte az Azure utilization API-val

1. Használja az additionalInfo attribútum ServiceType értékét az API-válaszban a megvásárolni kívánt virtuálisgép-méret azonosításához.

2. További információkért lásd [az](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) ügyfél Azure-beli kihasználtsági rekordjainak le Partnerközpont [API-ban.](/partner-center/develop/)

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Virtuális gép méretezési információinak lekért Microsoft Azure Portal

1. A Partnerközpont az Ügyfelek **oldalra.**

2. Keresse meg azt az ügyfelet, aki Azure-beli virtuális gépek foglalását szeretné megvásárolni, majd válassza a lefelé mutató nyilat az ügyfél információinak kibontásához. Válassza **a Microsoft Azure felügyeleti portálja** az ügyfél rekordját a Azure Portal.

3. A **portál menüjében** válassza a Virtuális gépek lehetőséget, majd válassza ki azt a virtuális gépet, amelyhez foglalást szeretne vásárolni.

4. A virtuális gép részletek lapján keresse meg a méretre és a régióra vonatkozó információkat az alább látható módon, és használja ezeket az információkat a foglalás megvásárlásához a Partnerközpont.  

   :::image type="content" source="images/usage1.png" alt-text="Méret- és régióinformációk a részletek oldalán.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Virtuális gép méretezési információinak lekért Microsoft Azure PowerShell

Az alábbi képen látható információk alapján le tudja szerezni annak a virtuális gépnek a helyét és méretét, amelyhez foglalást szeretne vásárolni. 

:::image type="content" source="images/usage2.png" alt-text="A virtuális gép helye és mérete.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Virtuális gépek méretezési információinak le Azure Resource Manager (ARM) API-val

1. Az ARMClient vagy az ARM API-k használatával hívja meg az ARM-ügyfelet ahhoz a virtuális géphez, amelyhez foglalást szeretne vásárolni.

2. /subscriptions/ <Subscription ID> /resourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ?api-version=2017-12-01

3. A hívás visszaadja a **vmSize** és **a hely** értékeit az alább látható módon.

    :::image type="content" source="images/usage3.png" alt-text="vmSize value.":::
    :::image type="content" source="images/usage4.png" alt-text="hely értéke.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Azure-beli virtuális gép használatának és foglalási kedvezményének ellenőrzése

Miután megvásárolt egy Azure-beli fenntartott virtuálisgép-példányt egy ügyfél nevében, a rendszer automatikusan alkalmazza a virtuálisgép-területért előre fizetett kedvezményt az ügyfél foglalásának attribútumainak és mennyiségének megfelelő virtuális gépekre.

Az alábbi módszerek egyikével ellenőrizheti az ügyfél foglalási használatát, és láthatja, hogy mely virtuális gépekre vonatkoznak a foglalási kedvezmények:

- Azure Portal
- Azure-kihasználtsági API

Az egyes módszerek használatának utasításai alább olvashatók.

>[!NOTE]
>Csak az Azure utilization API mutatja meg, hogy melyik virtuális gépre vonatkozik a kedvezmény.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Ellenőrizze az ügyfél foglalási használatát a Microsoft Azure Portal

1. A Partnerközpont az Ügyfelek **oldalra.**

2. Keresse meg azt az ügyfelet, akinek a foglalási kedvezményét és használati adatait ellenőrizni szeretné, majd válassza a lefelé mutató nyilat az ügyfél információinak kibontásához. Válassza **a Microsoft Azure felügyeleti portálja** az ügyfél rekordját a Azure Portal.
3. Válassza **a Foglalások** elemet a portál menüjében, majd válassza ki azt a foglalást, amelyről ellenőrizni szeretné a használatot.
4. Az Áttekintés **lapon** ellenőrizze a foglalás kihasználtsági grafikonját, amely azt mutatja, hogy a foglalás mekkora része lett alkalmazva a virtuális gépekre.

    >[!NOTE]
    >A kihasználtsági adatok akár 8 órával is késhetnek.

    a. Ha a foglalás kihasználtsága 100%, az ügyfél minden lehetséges megtakarítást kap, amit a foglalás vásárlása biztosítani tud.
    b. Ha a foglalás kihasználtsága 0%, a kedvezmény nem lesz alkalmazva egyetlen virtuális gépre sem.
    c. Ha a foglalás kihasználtsága 1% és 99% között van, a használaton kívüli előnyök is vannak.

5. Ennek elkerülése érdekében a vásárlás előtt határozza meg a megfelelő méretű virtuális gépet az ügyfél számítási igényeinek támogatásához.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Az ügyfél foglalási kihasználtságának ellenőrzése az Azure utilization API-val

>[!NOTE]
>Csak az Azure utilization API mutatja meg, hogy melyik virtuális gépre vonatkozik a kedvezmény.  

Az Azure utilization API-val lekért foglalási használati adatok segítségével ellenőrizheti, hogy az ügyfél kap-e foglalási kedvezményt, és hogy mely virtuális gépekre (virtuális gépekre) érvényes a kedvezmény. Hasonlítsa össze az A példát a B példával, és tekintse meg, hogyan ellenőrizhető egy ügyfél foglalási kihasználtsága.

:::image type="content" source="images/usage5.png" alt-text="Foglaláshasználati példák.":::

- A reservationId azonosítja a kedvezmény virtuális gépre való alkalmazáshoz használt Azure-foglalást.
- A consumptionMeter annak a virtuális gépnek a MeterId-e, amely a foglalási kedvezményt alkalmazza rá.
- A ReservationMeter 0 USD költséget mutat a foglalási kedvezmény alkalmazása óta.

További információkért lásd [az](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) ügyfél Azure-beli kihasználtsági rekordjainak le Partnerközpont [API-ban.](/partner-center/develop/)

>[!IMPORTANT]
>A szoftverköltségek, például a Microsoft Windows Server, jelenleg nem szerepelnek a virtuálisgép-foglalások árában, és külön sorelemekként jelennek meg a rendelési rekordban és a számlán. Ha azonban egy ügyfél rendelkezik az Azure Hybrid Use Benefit kedvezményével, a szoftverköltségek nem lesznek alkalmazva. További információ: A Fenntartott példányok által nem [tartalmazott Windows-szoftverköltségek.](/azure/billing/billing-reserved-instance-windows-software-costs)  

## <a name="next-steps"></a>Következő lépések

|**További információ:**   |**Olvassa el ezt**    |
|:-----------------------------|:-----------------|
|Azure Reservations a CSP-ban – áttekintés  | [Fenntartott Microsoft Azure példányok eladása](azure-reservations.md)
|Azure-foglalások vásárlása az ügyfelek számára Partnerközpont   | [Azure Reservations vásárlása](azure-reservations-buying.md)
|Azure Reservations kezelése a Partnerközpont | [Azure Reservations kezelése a Partnerközpont](azure-reservations-manage.md)
|Azure Reservations vásárlása a Azure Portal | [Előre fizetés azure-Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) virtuális gépekért |
|Azure Reservations kezelése a Azure Portal   | [Fenntartott virtuálisgép-példányok kezelése](/azure/billing/billing-manage-reserved-vm-instance) az Azure súgóban  |
|Azure Reservations vásárlása az Partnerközpont API-val | [Vásárlási Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) az Partnerközpont fejlesztői dokumentációjában   |
|Engedélyt ad az ügyfeleknek arra, hogy megvásárolják saját Azure-foglalásukat egy számukra megvásárolt előfizetésből. | [Engedélyt adhat az ügyfeleknek a saját Azure-foglalásaik vásárlásra](give-customers-permission.md)   |