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
ms.openlocfilehash: 14d488091227e30909b3d41af0684494a8b55de7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149451"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="ea7b3-103">Microsoft Azure-beli virtuális gép méretezése a maximális foglalási kihasználtsághoz</span><span class="sxs-lookup"><span data-stu-id="ea7b3-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="ea7b3-104">**Megfelelő szerepkörök:** Rendszergazdai ügynök | Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="ea7b3-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="ea7b3-105">Ez a cikk azt ismerteti, hogyan méretez egy virtuális gépet (VM) az ügyfelek számítási igényeihez, amikor Microsoft Azure vásárol számukra.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="ea7b3-106">Ez a cikk csak a Felhőszolgáltató (CSP) program partnereire vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="ea7b3-107">A más típusú előfizetéseket (például használat alapján fizetett, egyéni, Microsoft Ügyfélszerződés- vagy Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek érdemes elolvasni az [Azure Reservations dokumentációját.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="ea7b3-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="ea7b3-108">Az ügyfél Azure-foglalásának virtuálisgép-méretének meghatározása</span><span class="sxs-lookup"><span data-stu-id="ea7b3-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="ea7b3-109">Ha Microsoft Azure ügyfelek nevében vásárol foglalásokat, ki kell választania egy virtuális gépet, amely megfelel az ügyfél számítási igényeinek.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="ea7b3-110">Ezeket az információkat az alábbi módszerek egyikével találhatja meg:</span><span class="sxs-lookup"><span data-stu-id="ea7b3-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="ea7b3-111">Azure-kihasználtsági API</span><span class="sxs-lookup"><span data-stu-id="ea7b3-111">Azure utilization API</span></span>
- <span data-ttu-id="ea7b3-112">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="ea7b3-112">The Azure portal</span></span>
- <span data-ttu-id="ea7b3-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="ea7b3-113">Azure PowerShell</span></span>
- <span data-ttu-id="ea7b3-114">Az Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="ea7b3-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="ea7b3-115">Az egyes módszerek használatának utasításai alább olvashatók.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="ea7b3-116">A foglalás vásárlása után a foglalási kedvezmény automatikusan alkalmazva lesz a foglalás attribútumainak és mennyiségének megfelelő virtuális gépekre.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="ea7b3-117">Nem kell hozzárendelni a foglalást egy virtuális géphez.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="ea7b3-118">A foglalási kedvezmények nem vonatkoznak a klasszikus vagy promóciós virtuális gépekre.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="ea7b3-119">Az ügyfél nevében megvásárolni kívánt virtuális gép típusának és méretének helyes azonosításához az alább ismertetett módszerek egyikét kell használnia, mivel a virtuálisgép-sorozat típusa helytelenül jelenik meg az egyeztetési Partnerközpont fájlokban.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="ea7b3-120">Virtuális gépek méretezési információinak lekérte az Azure utilization API-val</span><span class="sxs-lookup"><span data-stu-id="ea7b3-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="ea7b3-121">Használja az additionalInfo attribútum ServiceType értékét az API-válaszban a megvásárolni kívánt virtuálisgép-méret azonosításához.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="ea7b3-122">További információkért lásd [az](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) ügyfél Azure-beli kihasználtsági rekordjainak le Partnerközpont [API-ban.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="ea7b3-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="ea7b3-123">Virtuális gép méretezési információinak lekért Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="ea7b3-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="ea7b3-124">A Partnerközpont az Ügyfelek **oldalra.**</span><span class="sxs-lookup"><span data-stu-id="ea7b3-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="ea7b3-125">Keresse meg azt az ügyfelet, aki Azure-beli virtuális gépek foglalását szeretné megvásárolni, majd válassza a lefelé mutató nyilat az ügyfél információinak kibontásához.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="ea7b3-126">Válassza **a Microsoft Azure felügyeleti portálja** az ügyfél rekordját a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="ea7b3-127">A **portál menüjében** válassza a Virtuális gépek lehetőséget, majd válassza ki azt a virtuális gépet, amelyhez foglalást szeretne vásárolni.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="ea7b3-128">A virtuális gép részletek lapján keresse meg a méretet és a régiót az alább látható módon, és ezen információk alapján vásárolja meg a foglalást a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Méret- és régióinformációk a részletek oldalán":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="ea7b3-130">Virtuális gép méretezési információinak lekért Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="ea7b3-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="ea7b3-131">Az alábbi képen látható információk alapján le tudja szerezni annak a virtuális gépnek a helyét és méretét, amelyhez foglalást szeretne vásárolni.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Virtuális gép helye és mérete":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="ea7b3-133">Virtuális gépek méretezési információinak lekérte az Azure Resource Manager (ARM) API-val</span><span class="sxs-lookup"><span data-stu-id="ea7b3-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="ea7b3-134">Az ARMClient vagy az ARM API-k használatával hívja meg az ARM-ügyfelet ahhoz a virtuális géphez, amelyhez foglalást szeretne vásárolni.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="ea7b3-135">/subscriptions/ <Subscription ID> /resourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="ea7b3-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="ea7b3-136">A hívás visszaadja a **vmSize** és **a location** értékeit az alább látható módon.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize value":::
    :::image type="content" source="images/usage4.png" alt-text="hely értéke":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="ea7b3-139">Azure-beli virtuális gépek használatának és foglalási kedvezményének ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="ea7b3-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="ea7b3-140">Miután megvásárolt egy Azure-beli fenntartott virtuálisgép-példányt egy ügyfél nevében, a virtuálisgép-területért előre fizetett kedvezmény automatikusan alkalmazva lesz az ügyfél foglalásának attribútumainak és mennyiségének megfelelő virtuális gépekre.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="ea7b3-141">Az alábbi módszerek egyikével ellenőrizheti az ügyfél foglaláshasználatát, és láthatja, hogy mely virtuális gépekre vonatkoznak a foglalási kedvezmények:</span><span class="sxs-lookup"><span data-stu-id="ea7b3-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="ea7b3-142">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="ea7b3-142">The Azure portal</span></span>
- <span data-ttu-id="ea7b3-143">Azure-kihasználtsági API</span><span class="sxs-lookup"><span data-stu-id="ea7b3-143">Azure utilization API</span></span>

<span data-ttu-id="ea7b3-144">Az alábbiakban az egyes metódusok használatának utasításait olvashatja.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="ea7b3-145">Csak az Azure utilization API mutatja meg, hogy a kedvezmény melyik virtuális gépre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="ea7b3-146">Ellenőrizze az ügyfél foglalási használatát a Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="ea7b3-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="ea7b3-147">A Partnerközpont az Ügyfelek **oldalra.**</span><span class="sxs-lookup"><span data-stu-id="ea7b3-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="ea7b3-148">Keresse meg azt az ügyfelet, akinek a foglalási kedvezményét és használati adatait ellenőrizni szeretné, majd válassza a lefelé mutató nyilat az ügyfél információinak kibontásához.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="ea7b3-149">Válassza **a Microsoft Azure felügyeleti portálja** az ügyfél rekordját a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="ea7b3-150">Válassza **a Foglalások** elemet a portál menüjében, majd válassza ki azt a foglalást, amelyről ellenőrizni szeretné a használatot.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="ea7b3-151">Az Áttekintés **lapon** ellenőrizze a foglalás kihasználtsági grafikonját, amely azt mutatja, hogy a foglalás mekkora része lett alkalmazva a virtuális gépekre.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="ea7b3-152">A kihasználtsági adatok akár 8 órával is késhetnek.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="ea7b3-153">a.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-153">a.</span></span> <span data-ttu-id="ea7b3-154">Ha a foglalás kihasználtsága 100%, az ügyfél minden lehetséges megtakarítást kap, amit a foglalás vásárlása biztosítani tud.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="ea7b3-155">b.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-155">b.</span></span> <span data-ttu-id="ea7b3-156">Ha a foglalás kihasználtsága 0%, a kedvezmény nem lesz alkalmazva egyetlen virtuális gépre sem.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="ea7b3-157">c.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-157">c.</span></span> <span data-ttu-id="ea7b3-158">Ha a foglalás kihasználtsága 1% és 99% között van, a használaton kívüli előnyök is vannak.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="ea7b3-159">Ennek elkerülése érdekében a vásárlás előtt határozza meg a megfelelő méretű virtuális gépet az ügyfél számítási igényeinek támogatásához.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="ea7b3-160">Az ügyfél foglalási kihasználtságának ellenőrzése az Azure utilization API-val</span><span class="sxs-lookup"><span data-stu-id="ea7b3-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="ea7b3-161">Csak az Azure utilization API mutatja meg, hogy melyik virtuális gépre vonatkozik a kedvezmény.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="ea7b3-162">Az Azure utilization API-val lekért foglalási használati adatok segítségével ellenőrizheti, hogy az ügyfél kap-e foglalási kedvezményt, és hogy mely virtuális gépekre (virtuális gépekre) érvényes a kedvezmény.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="ea7b3-163">Hasonlítsa össze az A példát a B példával, és tekintse meg, hogyan ellenőrizhető egy ügyfél foglalási kihasználtsága.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Foglaláshasználati példák":::

- <span data-ttu-id="ea7b3-165">A reservationId azonosítja a kedvezmény virtuális gépre való alkalmazáshoz használt Azure-foglalást.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="ea7b3-166">A consumptionMeter annak a virtuális gépnek a MeterId-e, amely a foglalási kedvezményt alkalmazza rá.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="ea7b3-167">A ReservationMeter 0 USD költséget mutat a foglalási kedvezmény alkalmazása óta.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="ea7b3-168">További információkért lásd [az](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) ügyfél Azure-beli kihasználtsági rekordjainak le Partnerközpont [API-ban.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="ea7b3-168">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="ea7b3-169">A szoftverköltségek, például a Microsoft Windows Server, jelenleg nem szerepelnek a virtuálisgép-foglalások árában, és külön sorelemekként jelennek meg a rendelési rekordban és a számlán.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="ea7b3-170">Ha azonban az ügyfél rendelkezik az Azure Hybrid Use Benefit kedvezményével, a szoftverköltségek nem lesznek alkalmazva.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="ea7b3-171">További információ: A Fenntartott példányok által nem [tartalmazott Windows-szoftverköltségek.](/azure/billing/billing-reserved-instance-windows-software-costs)</span><span class="sxs-lookup"><span data-stu-id="ea7b3-171">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="ea7b3-172">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ea7b3-172">Next steps</span></span>

|<span data-ttu-id="ea7b3-173">**További információ:**</span><span class="sxs-lookup"><span data-stu-id="ea7b3-173">**For information about**</span></span>   |<span data-ttu-id="ea7b3-174">**Olvassa el ezt**</span><span class="sxs-lookup"><span data-stu-id="ea7b3-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="ea7b3-175">Azure Reservations a CSP-ban – áttekintés</span><span class="sxs-lookup"><span data-stu-id="ea7b3-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="ea7b3-176">Fenntartott Microsoft Azure-példányok eladása</span><span class="sxs-lookup"><span data-stu-id="ea7b3-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="ea7b3-177">Azure-foglalások vásárlása az ügyfelek számára Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ea7b3-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="ea7b3-178">Azure Reservations vásárlása</span><span class="sxs-lookup"><span data-stu-id="ea7b3-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="ea7b3-179">Azure Reservations kezelése a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ea7b3-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="ea7b3-180">Azure Reservations kezelése a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ea7b3-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="ea7b3-181">Azure Reservations vásárlása a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="ea7b3-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="ea7b3-182">[Előre fizetés az Azure Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) virtuális gépekért</span><span class="sxs-lookup"><span data-stu-id="ea7b3-182">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="ea7b3-183">Azure Reservations kezelése a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="ea7b3-183">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="ea7b3-184">[Fenntartott virtuálisgép-példányok kezelése](/azure/billing/billing-manage-reserved-vm-instance) az Azure Súgóban</span><span class="sxs-lookup"><span data-stu-id="ea7b3-184">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="ea7b3-185">Azure-foglalások vásárlása a Partnerközpont API-val</span><span class="sxs-lookup"><span data-stu-id="ea7b3-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="ea7b3-186">[Vásárlás Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) a Partnerközpont fejlesztői dokumentációjában</span><span class="sxs-lookup"><span data-stu-id="ea7b3-186">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="ea7b3-187">Engedélyt ad az ügyfeleknek arra, hogy megvásárolják a saját Azure-foglalásukat a számukra megvásárolt előfizetésből.</span><span class="sxs-lookup"><span data-stu-id="ea7b3-187">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="ea7b3-188">Engedélyt adhat az ügyfeleknek a saját Azure-foglalásaik vásárlásra</span><span class="sxs-lookup"><span data-stu-id="ea7b3-188">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |