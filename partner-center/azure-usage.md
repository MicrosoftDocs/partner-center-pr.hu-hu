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
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="db27f-103">Microsoft Azure-beli virtuális gép méretezése a maximális foglalási kihasználtsághoz</span><span class="sxs-lookup"><span data-stu-id="db27f-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="db27f-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="db27f-104">**Applies to**</span></span>

- <span data-ttu-id="db27f-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="db27f-105">Partner Center</span></span>
- <span data-ttu-id="db27f-106">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="db27f-106">Azure portal</span></span>
- <span data-ttu-id="db27f-107">Partnerek a CSP programban</span><span class="sxs-lookup"><span data-stu-id="db27f-107">Partners in the CSP program</span></span>
 
> [!NOTE]
> <span data-ttu-id="db27f-108">Ez a cikk csak a Cloud Solution Provider (CSP) programban található partnerekre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="db27f-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="db27f-109">A más típusú előfizetéseket (például az utólagos elszámolású, az egyéni, a Microsoft-ügyféli szerződést vagy a Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek Ehelyett olvasniuk kell [Az Azure foglalási dokumentációját](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="db27f-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="db27f-110">A virtuális gép méretének meghatározása az ügyfél Azure-beli foglalásához</span><span class="sxs-lookup"><span data-stu-id="db27f-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="db27f-111">Microsoft Azure foglalásoknak az ügyfelek nevében történő megvásárlásakor ki kell választania egy virtuális gépet (VM), amely megfelel az ügyfél számítástechnikai igényeinek.</span><span class="sxs-lookup"><span data-stu-id="db27f-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="db27f-112">Ezeket az adatokat a következő módszerek egyikével keresheti meg:</span><span class="sxs-lookup"><span data-stu-id="db27f-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="db27f-113">Azure-kihasználtság API</span><span class="sxs-lookup"><span data-stu-id="db27f-113">Azure utilization API</span></span>
- <span data-ttu-id="db27f-114">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="db27f-114">The Azure portal</span></span>
- <span data-ttu-id="db27f-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="db27f-115">Azure PowerShell</span></span>
- <span data-ttu-id="db27f-116">A Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="db27f-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="db27f-117">Az egyes módszerek használatára vonatkozó utasítások alább láthatók.</span><span class="sxs-lookup"><span data-stu-id="db27f-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="db27f-118">A foglalás megvásárlása után a rendszer automatikusan alkalmazza a foglalási kedvezményt a foglalás attribútumait és mennyiségét megegyező virtuális gépekre.</span><span class="sxs-lookup"><span data-stu-id="db27f-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="db27f-119">Nem kell hozzárendelni a foglalást egy virtuális géphez.</span><span class="sxs-lookup"><span data-stu-id="db27f-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="db27f-120">A foglalási kedvezmények nem vonatkoznak a klasszikus és a promóciós virtuális gépekre.</span><span class="sxs-lookup"><span data-stu-id="db27f-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="db27f-121">Az ügyfél nevében megvásárolni kívánt virtuális gép típusának és méretének megfelelő azonosításához az alábbiakban ismertetett módszerek egyikét kell használnia, mivel a virtuálisgép-sorozat típusa nem megfelelően jelenik meg a partner Center egyeztetési fájljaiban.</span><span class="sxs-lookup"><span data-stu-id="db27f-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="db27f-122">VM-méretezési információk beolvasása az Azure-kihasználtság API használatával</span><span class="sxs-lookup"><span data-stu-id="db27f-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="db27f-123">A megvásárolni kívánt virtuálisgép-méret azonosításához használja a ServiceType attribútum értékét a additionalInfo elemben az API-válaszban.</span><span class="sxs-lookup"><span data-stu-id="db27f-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="db27f-124">További információ: [ügyfél kihasználtsági rekordjainak beszerzése az Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) -hoz a [partner Center API](/partner-center/develop/)-ban.</span><span class="sxs-lookup"><span data-stu-id="db27f-124">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="db27f-125">VM-méretezési információk beolvasása a Microsoft Azure Portal használatával</span><span class="sxs-lookup"><span data-stu-id="db27f-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="db27f-126">A partner Centerben lépjen az **ügyfelek** oldalra.</span><span class="sxs-lookup"><span data-stu-id="db27f-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="db27f-127">Keresse meg azt az ügyfelet, aki szeretné megvásárolni az Azure-beli virtuális gépek foglalását, majd a lefelé mutató nyílra kattintva bontsa ki az ügyfél adatait.</span><span class="sxs-lookup"><span data-stu-id="db27f-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="db27f-128">Válassza a **a Microsoft Azure felügyeleti portálja** lehetőséget az ügyfél rekordjának megnyitásához a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="db27f-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="db27f-129">Válassza a portál menüben a **virtuális gépek** lehetőséget, majd válassza ki azt a virtuális gépet, amelyhez foglalást szeretne vásárolni.</span><span class="sxs-lookup"><span data-stu-id="db27f-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="db27f-130">A virtuális gép részletei lapon keresse meg a méret és a régió adatait az alábbi ábrán látható módon, és használja ezt az információt a foglalás megvásárlásához a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="db27f-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="A méret és a régió adatai a Részletek lapon":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="db27f-132">VM-méretezési információk beolvasása Microsoft Azure PowerShell használatával</span><span class="sxs-lookup"><span data-stu-id="db27f-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="db27f-133">Az alábbi képen található információk segítségével megtekintheti annak a virtuális gépnek a helyét és méretét, amelyhez foglalást kíván vásárolni.</span><span class="sxs-lookup"><span data-stu-id="db27f-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Virtuális gép helye és mérete":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="db27f-135">VM-méretezési információk beolvasása a Azure Resource Manager (ARM) API használatával</span><span class="sxs-lookup"><span data-stu-id="db27f-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="db27f-136">A ARMClient vagy az ARM API-k használatával hívja meg az ARM-ügyfelet arra a virtuális gépre, amelyhez foglalást kíván vásárolni.</span><span class="sxs-lookup"><span data-stu-id="db27f-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="db27f-137">/Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-Version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="db27f-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="db27f-138">A hívás az alább látható módon visszaadja a **vmSize** és a **hely** értékét.</span><span class="sxs-lookup"><span data-stu-id="db27f-138">The call returns the values for **vmSize** and **location** , as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize érték":::
    :::image type="content" source="images/usage4.png" alt-text="hely értéke":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="db27f-141">Azure-beli virtuális gépek használatának és foglalási kedvezményének ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="db27f-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="db27f-142">Miután megvásárolta az Azure-beli fenntartott VM-példányt az ügyfél nevében, a rendszer automatikusan alkalmazza a virtuális gép területének kifizetésére vonatkozó kedvezményt az ügyfél foglalásának attribútumait és mennyiségét megegyező virtuális gépekre.</span><span class="sxs-lookup"><span data-stu-id="db27f-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="db27f-143">A következő módszerek egyikével ellenőrizheti az ügyfél foglalási használatát, és megtekintheti, hogy mely virtuális gépekre vonatkoznak a foglalási kedvezmények:</span><span class="sxs-lookup"><span data-stu-id="db27f-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="db27f-144">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="db27f-144">The Azure portal</span></span>
- <span data-ttu-id="db27f-145">Azure-kihasználtság API</span><span class="sxs-lookup"><span data-stu-id="db27f-145">Azure utilization API</span></span>

<span data-ttu-id="db27f-146">Az egyes módszerek használatára vonatkozó utasítások alább láthatók.</span><span class="sxs-lookup"><span data-stu-id="db27f-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="db27f-147">Csak az Azure kihasználtsági API jeleníti meg, hogy a rendszer melyik virtuális gépre alkalmazza a kedvezményt.</span><span class="sxs-lookup"><span data-stu-id="db27f-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="db27f-148">Az ügyfél foglalási használatának ellenőrzése a Microsoft Azure Portalban</span><span class="sxs-lookup"><span data-stu-id="db27f-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="db27f-149">A partner Centerben lépjen az **ügyfelek** oldalra.</span><span class="sxs-lookup"><span data-stu-id="db27f-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="db27f-150">Keresse meg azt az ügyfelet, akinek a foglalási kedvezményét és felhasználását ellenőrizni szeretné, majd a lefelé mutató nyílra kattintva bontsa ki az ügyfél adatait.</span><span class="sxs-lookup"><span data-stu-id="db27f-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="db27f-151">Válassza a **a Microsoft Azure felügyeleti portálja** lehetőséget az ügyfél rekordjának megnyitásához a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="db27f-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="db27f-152">Válassza a portál menüben a **foglalások** lehetőséget, majd válassza ki azt a foglalást, amelynek a használatát ellenőriznie szeretné.</span><span class="sxs-lookup"><span data-stu-id="db27f-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="db27f-153">Az **Áttekintés** oldalon tekintse meg a foglalás kihasználtsága diagramot, amely azt mutatja, hogy a foglalás mekkora része lett alkalmazva a virtuális gépekre.</span><span class="sxs-lookup"><span data-stu-id="db27f-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="db27f-154">A kihasználtsági adatai akár 8 óráig is késleltethető.</span><span class="sxs-lookup"><span data-stu-id="db27f-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="db27f-155">a.</span><span class="sxs-lookup"><span data-stu-id="db27f-155">a.</span></span> <span data-ttu-id="db27f-156">Ha a foglalás kihasználtsága 100%, az ügyfél minden lehetséges megtakarítást biztosít, amelyet a foglalás megvásárlása tud biztosítani.</span><span class="sxs-lookup"><span data-stu-id="db27f-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="db27f-157">b.</span><span class="sxs-lookup"><span data-stu-id="db27f-157">b.</span></span> <span data-ttu-id="db27f-158">Ha a foglalás kihasználtsága 0%, a rendszer nem alkalmazza a kedvezményt egyetlen virtuális gépre sem.</span><span class="sxs-lookup"><span data-stu-id="db27f-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="db27f-159">c.</span><span class="sxs-lookup"><span data-stu-id="db27f-159">c.</span></span> <span data-ttu-id="db27f-160">Ha a foglalás kihasználtsága 1% és 99% között van, akkor nem használhatók előnyök.</span><span class="sxs-lookup"><span data-stu-id="db27f-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="db27f-161">Ennek elkerüléséhez határozza meg a megfelelő méretű virtuális gépet, hogy támogassa az ügyfél számítástechnikai igényeit a vásárlás előtt.</span><span class="sxs-lookup"><span data-stu-id="db27f-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="db27f-162">Az ügyfél foglalási használatának ellenőrzése az Azure kihasználtsági API-val</span><span class="sxs-lookup"><span data-stu-id="db27f-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="db27f-163">Csak az Azure kihasználtsági API jeleníti meg, hogy a rendszer melyik virtuális gépre alkalmazza a kedvezményt.</span><span class="sxs-lookup"><span data-stu-id="db27f-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="db27f-164">Lekérheti a foglalási használati adatokat az Azure kihasználtsági API-val annak ellenőrzéséhez, hogy az ügyfél beolvasta-e a foglalási kedvezményt, és hogy a rendszer mely virtuális gépeket (Virtual machines) alkalmazza a kedvezményre.</span><span class="sxs-lookup"><span data-stu-id="db27f-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="db27f-165">Hasonlítsa össze a példát a B példával, hogy megtekintse, hogyan ellenőrizheti az ügyfél foglalási felhasználását.</span><span class="sxs-lookup"><span data-stu-id="db27f-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="A foglalás használati példái":::

- <span data-ttu-id="db27f-167">A reservationId azonosítja azt az Azure-foglalást, amelyet a kedvezmény a virtuális gépre való alkalmazásához használt.</span><span class="sxs-lookup"><span data-stu-id="db27f-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="db27f-168">a consumptionMeter annak a virtuális gépnek a MeterId, amelyhez a foglalási kedvezmény vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="db27f-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="db27f-169">A ReservationMeter a foglalási kedvezmény alkalmazása óta $0 költségeket mutat.</span><span class="sxs-lookup"><span data-stu-id="db27f-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="db27f-170">További információ: [ügyfél kihasználtsági rekordjainak beszerzése az Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) -hoz a [partner Center API](/partner-center/develop/)-ban.</span><span class="sxs-lookup"><span data-stu-id="db27f-170">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="db27f-171">A szoftveres költségek, mint például a Microsoft Windows Server, jelenleg nem szerepelnek a virtuális gépek foglalásának árán, és külön sorokként jelennek meg a rendelési rekordban és a számlán.</span><span class="sxs-lookup"><span data-stu-id="db27f-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="db27f-172">Ha azonban az ügyfél rendelkezik a Azure Hybrid Use Benefitval, a rendszer nem alkalmazza a szoftverre vonatkozó költségeket.</span><span class="sxs-lookup"><span data-stu-id="db27f-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="db27f-173">További információ: [a Windows-szoftverek nem tartalmazzák a fenntartott példányokat](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="db27f-173">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="db27f-174">Azure-foglalások erőforrásai</span><span class="sxs-lookup"><span data-stu-id="db27f-174">Azure reservations resources</span></span>

|<span data-ttu-id="db27f-175">**További információ**</span><span class="sxs-lookup"><span data-stu-id="db27f-175">**For information about**</span></span>   |<span data-ttu-id="db27f-176">**Olvassa el ezt**</span><span class="sxs-lookup"><span data-stu-id="db27f-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="db27f-177">Azure-foglalások a CSP-ben – áttekintés</span><span class="sxs-lookup"><span data-stu-id="db27f-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="db27f-178">Microsoft Azure fenntartott VM-példányok eladása</span><span class="sxs-lookup"><span data-stu-id="db27f-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="db27f-179">Azure-foglalások vásárlása az ügyfelek számára a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="db27f-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="db27f-180">Azure-foglalások vásárlása</span><span class="sxs-lookup"><span data-stu-id="db27f-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="db27f-181">Azure-foglalások kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="db27f-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="db27f-182">Azure-foglalások kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="db27f-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="db27f-183">Azure-foglalások megvásárlása a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="db27f-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="db27f-184">[Fizetős virtuális gépek esetén Azure Reserved VM instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) az Azure súgójában</span><span class="sxs-lookup"><span data-stu-id="db27f-184">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="db27f-185">Azure-foglalások kezelése a Azure Portalban</span><span class="sxs-lookup"><span data-stu-id="db27f-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="db27f-186">[Fenntartott VM-példányok kezelése](/azure/billing/billing-manage-reserved-vm-instance) az Azure súgójában</span><span class="sxs-lookup"><span data-stu-id="db27f-186">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="db27f-187">Azure-foglalások vásárlása a partner Center API használatával</span><span class="sxs-lookup"><span data-stu-id="db27f-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="db27f-188">[Vásárlás Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) a partner Center fejlesztői dokumentációjában</span><span class="sxs-lookup"><span data-stu-id="db27f-188">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="db27f-189">Lehetővé teszi, hogy az ügyfelek megvásárolják saját Azure-foglalásait a számukra megvásárolt előfizetésből.</span><span class="sxs-lookup"><span data-stu-id="db27f-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="db27f-190">Engedélyt ad az ügyfeleknek a saját Azure-foglalások megvásárlására</span><span class="sxs-lookup"><span data-stu-id="db27f-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |