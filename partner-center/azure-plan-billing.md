---
title: Azure-csomag számlázása – számla & recon files
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan férhet hozzá és értheti meg az Azure-csomag számlázásával kapcsolatos számla- és egyeztetési fájlstruktúrát.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c7c06f5ed7b147625afb5020f63ead411ef58fa8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551520"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="df421-103">Új kereskedelmi felület a CSP-ben – Azure-számlázás</span><span class="sxs-lookup"><span data-stu-id="df421-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="df421-104">**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="df421-104">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="df421-105">Ez a cikk azt ismerteti, hogyan férhet hozzá az Azure-csomag számlázásához kapcsolódó számla- és egyeztetési fájlstruktúrához, és hogyan értheti meg azt.</span><span class="sxs-lookup"><span data-stu-id="df421-105">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="df421-106">Az Azure-csomag szerinti számlázás egy egyszerűsített számlázási élmény, amely egy igazított egyetlen számlázási dátumot és egy naptári hónapalapú számlázási időszakot használ.</span><span class="sxs-lookup"><span data-stu-id="df421-106">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="df421-107">A számlázással kapcsolatos alapvető információk összegzése</span><span class="sxs-lookup"><span data-stu-id="df421-107">Summary of billing essentials</span></span>

- <span data-ttu-id="df421-108">**Számla dátuma:** A számla és az egyeztetési fájl a következő időpontig Partnerközpont (UTC) éjfélig lesz elérhető a Partnerközpont irányítópultján/API-ján.</span><span class="sxs-lookup"><span data-stu-id="df421-108">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="df421-109">**Számlázási időszak:** A számla számlázási időszaka a naptári hónaphoz igazodik, például: 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="df421-109">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="df421-110">**Díjak szolgáltatási időszaka:** A díjak a naptári hónaphoz igazodnak.</span><span class="sxs-lookup"><span data-stu-id="df421-110">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="df421-111">Ha például a számlázott partner azure-szolgáltatásokat ad hozzá egy Azure-csomagon keresztül 10/15-én, és az ügyfél 10/15-én kezdi meg az Azure-szolgáltatások használatának elkezdét, akkor a kiszámlázott partner a 10/15–31 szolgáltatási időszakra vonatkozóan a 10/10/31-es szolgáltatási időszakra vonatkozóan a 11/8-as ügyfélfelhasználásra vonatkozóan kap számlát/recont.</span><span class="sxs-lookup"><span data-stu-id="df421-111">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="df421-112">A következő hónap 12/8-án generált számlája tartalmazza a 11/1–11/31 szolgáltatási időszakra vonatkozó díjakat.</span><span class="sxs-lookup"><span data-stu-id="df421-112">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="df421-113">**Számlás fizetési időszak:** 60 nap.</span><span class="sxs-lookup"><span data-stu-id="df421-113">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="df421-114">**Számla** pénzneme: 2021. január 28-tól kezdődően azok az EU-/EFTA- és Egyesült Királyság-régióban lévő partnerek, akik új ügyfelekkel és meglévő CSP-ügyfelekkel vásárolnak új kereskedelmi ajánlatokat 2020. május 11. előtt, a partneri hely pénznemében lesznek számlázva.</span><span class="sxs-lookup"><span data-stu-id="df421-114">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="df421-115">Az EU-n/EFTA-n és az Egyesült Királyságon kívül található partnerek számlázása továbbra is a partnerhely pénznemében történik.</span><span class="sxs-lookup"><span data-stu-id="df421-115">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="df421-116">**Partneri ösztönzők:** A számlázási hónap végével 45 nappal fizették ki.</span><span class="sxs-lookup"><span data-stu-id="df421-116">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="df421-117">Hozzáférés a számlákhoz és az egyeztetési fájlokhoz</span><span class="sxs-lookup"><span data-stu-id="df421-117">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="df421-118">A vállalat globális rendszergazdája vagy számlázási rendszergazdája e-mailt kap, ha a számla készen áll a megtekintésre.</span><span class="sxs-lookup"><span data-stu-id="df421-118">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="df421-119">A számla és az egyeztetési fájl elérése:</span><span class="sxs-lookup"><span data-stu-id="df421-119">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="df421-120">Jelentkezzen be a Partnerközpont [irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="df421-120">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="df421-121">A Partnerközpont válassza a Számlázás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="df421-121">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="df421-122">Válassza a Recurring (Ismétlődő) **és** **az One-time (Egyszeri) lapfület,** valamint a kívánt pénznemet.</span><span class="sxs-lookup"><span data-stu-id="df421-122">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="Számlázási.":::

4. <span data-ttu-id="df421-124">Válassza **a Számla** vagy az **Egyeztetési fájl lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="df421-124">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="df421-125">Az előzményszámlák és a recon-fájlok megtekintéséhez bontsa ki az alábbi Számlázási előzmények sort.</span><span class="sxs-lookup"><span data-stu-id="df421-125">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="df421-126">A használati adatok ismertetése</span><span class="sxs-lookup"><span data-stu-id="df421-126">Understanding usage data</span></span> 

1. <span data-ttu-id="df421-127">Az Azure-csomag a használat legfelső szintű vagy legfelső szintű tárolója.</span><span class="sxs-lookup"><span data-stu-id="df421-127">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="df421-128">Minden használat egyetlen Azure-csomaghoz kötődik.</span><span class="sxs-lookup"><span data-stu-id="df421-128">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="df421-129">Egy csomagon belül egy vagy több Azure-előfizetés lesz.</span><span class="sxs-lookup"><span data-stu-id="df421-129">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="df421-130">Ezek erőforrás-kezeléshez és üzembe helyezéshez használt tárolók.</span><span class="sxs-lookup"><span data-stu-id="df421-130">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="df421-131">Az előfizetésen belül az erőforráscsoportok hozzáadhatók az erőforrások csoportosításához.</span><span class="sxs-lookup"><span data-stu-id="df421-131">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="df421-132">Minden erőforrás egy erőforráscsoportba van telepítve.</span><span class="sxs-lookup"><span data-stu-id="df421-132">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="df421-133">Ilyen erőforrás például a virtuális gépek és a tárfiókok.</span><span class="sxs-lookup"><span data-stu-id="df421-133">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="df421-134">Erőforrás-kibocsátó mérők: A fogyasztásmérők egy erőforrás fogyasztásának mérései, és egy erőforrás több mérőre is kibocsáthat használatot.</span><span class="sxs-lookup"><span data-stu-id="df421-134">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="df421-135">A mérőket egy Termékazonosító, SKUId és AvailabilityId azonosítja.</span><span class="sxs-lookup"><span data-stu-id="df421-135">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="df421-136">Az előfizetési erőforráscsoportok és a mérés hierarchiája</span><span class="sxs-lookup"><span data-stu-id="df421-136">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="df421-137">**Azure-fiók (bérlő)**</span><span class="sxs-lookup"><span data-stu-id="df421-137">**Azure account (tenant)**</span></span>

- <span data-ttu-id="df421-138">A előfizetés</span><span class="sxs-lookup"><span data-stu-id="df421-138">Subscription A</span></span>
    - <span data-ttu-id="df421-139">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="df421-139">ResourceGroup 1</span></span>
        - <span data-ttu-id="df421-140">Virtuális gép (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="df421-140">Virtual machine (resource)</span></span>
            - <span data-ttu-id="df421-141">Számítási fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="df421-141">Compute meter</span></span>
        - <span data-ttu-id="df421-142">Virtuális hálózat (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="df421-142">Virtual network (resource)</span></span>
            - <span data-ttu-id="df421-143">Nincs számlázási mérő</span><span class="sxs-lookup"><span data-stu-id="df421-143">No billing meter</span></span>

    - <span data-ttu-id="df421-144">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="df421-144">ResourceGroup 2</span></span>
        - <span data-ttu-id="df421-145">Virtuális gép (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="df421-145">Virtual machine (resource)</span></span>
            - <span data-ttu-id="df421-146">Számítógép-fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="df421-146">Computer meter</span></span>
        - <span data-ttu-id="df421-147">prémium SSD lemez (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="df421-147">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="df421-148">Tárolókapacitás-mérő</span><span class="sxs-lookup"><span data-stu-id="df421-148">Storage capacity meter</span></span>
            - <span data-ttu-id="df421-149">Tárolási műveletek mérő</span><span class="sxs-lookup"><span data-stu-id="df421-149">Storage operations meter</span></span>

- <span data-ttu-id="df421-150">B előfizetés –ResourceGroup 1 – Azure SQL (erőforrás) – DTU-fogyasztásmérő – VPN Gateway (erőforrás) – VPN-átjáró mérő</span><span class="sxs-lookup"><span data-stu-id="df421-150">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="df421-151">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="df421-151">ResourceGroup 2</span></span>
        - <span data-ttu-id="df421-152">Virtual Network felület (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="df421-152">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="df421-153">Nincs számlázási mérő</span><span class="sxs-lookup"><span data-stu-id="df421-153">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="df421-154">A számla olvasása</span><span class="sxs-lookup"><span data-stu-id="df421-154">Read the invoice</span></span>

1. <span data-ttu-id="df421-155">A számla legkésőbb az egyes hónap végéig lesz elérhető.</span><span class="sxs-lookup"><span data-stu-id="df421-155">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="df421-156">A partnereknek 60 napjuk van a kifizetés visszafizetésére.</span><span class="sxs-lookup"><span data-stu-id="df421-156">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="df421-157">A számlázási időszak egy adott naptári hónapra vonatkozik, például: 10.1-10.31.</span><span class="sxs-lookup"><span data-stu-id="df421-157">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="df421-158">A díjak a kiigazítások nettó összegei (az összeg a "felügyelt szolgáltatások partneri jóváírásának nettó összege").</span><span class="sxs-lookup"><span data-stu-id="df421-158">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="df421-159">További számlázási részletekért tekintse át a számla recon fájlját és a napi névleges használati adatokat tartalmazó fájlt.</span><span class="sxs-lookup"><span data-stu-id="df421-159">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="Számla.":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="df421-161">A számla egyeztetési fájl olvasása</span><span class="sxs-lookup"><span data-stu-id="df421-161">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="df421-162">Az egyes Azure-csomag- és fogyasztásmérő-kombinációk legfeljebb két számlázási svonalat használhatnak a felderítési fájlban.</span><span class="sxs-lookup"><span data-stu-id="df421-162">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="df421-163">Ha a fogyasztásmérő bármilyen típusú kedvezményre vagy jóváírásra (például rétegzett kedvezményekre vagy felügyelt szolgáltatásokhoz kapott partneri jóváírásra) jogosult az egész naptári hónapban, akkor a recon fájl csak egy számlázási sort fog tartalmazni.</span><span class="sxs-lookup"><span data-stu-id="df421-163">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="df421-164">A **PriceAdjusmentDescription oszlop** a kedvezményre vagy a jóváírásra fog hivatkozni.</span><span class="sxs-lookup"><span data-stu-id="df421-164">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="df421-165">Ha egy adott fogyasztásmérőnek nincsenek kedvezményre vagy partneri jóváírásra jogosult erőforrásai, akkor a recon fájl csak egy számlázási sort fog tartalmazni, a tényleges egységár pedig a kiskereskedelmi ár lesz (amely az egységár).</span><span class="sxs-lookup"><span data-stu-id="df421-165">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="df421-166">Ha a fogyasztásmérő vagy az adott fogyasztásmérőt kibocsátó bármely erőforrás, amely a hónap egy részére felügyelt szolgáltatásokért kapott partneri jóváírásra van minősítve, a felderítési fájl két számlázási sort fog tartalmazni. </span><span class="sxs-lookup"><span data-stu-id="df421-166">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="df421-167">Az egyik vonal azokat a napokat jelenti, amelyekben a fogyasztásmérő minősített, a második pedig azokat a napokat jelenti, amelyek nem megfelelőek.</span><span class="sxs-lookup"><span data-stu-id="df421-167">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

>[!NOTE]
><span data-ttu-id="df421-168">Az Azure-használatot az egyszeres vásárlási recon fájlban egyeztetheti.</span><span class="sxs-lookup"><span data-stu-id="df421-168">You can reconcile your Azure consumption in your one-time purchase recon file.</span></span> <span data-ttu-id="df421-169">Ehhez keresse meg a napi rendszerességgel minősített használat felderítési fájlját, és keresse meg a SubscriptionID-t.</span><span class="sxs-lookup"><span data-stu-id="df421-169">To do this, go to your daily-rated usage recon file and search for your SubscriptionID.</span></span> <span data-ttu-id="df421-170">Ez megjeleníti az Azure-csomag azonosítójával kapcsolatos összes költséget.</span><span class="sxs-lookup"><span data-stu-id="df421-170">This will display all costs associated with your Azure Plan ID.</span></span> <span data-ttu-id="df421-171">Az Azure SubscriptionID jogosultságazonosítóként jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="df421-171">Your Azure SubscriptionID is shown as the EntitlementID.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="df421-172">A napi használati adatok fájl olvasása</span><span class="sxs-lookup"><span data-stu-id="df421-172">Read the daily usage file</span></span>

- <span data-ttu-id="df421-173">Az Azure-csomag előfizetési mérőszámai napi szinten vannak minősítve és összesülve.</span><span class="sxs-lookup"><span data-stu-id="df421-173">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="df421-174">**A felügyelt szolgáltatások partneri jóváírását** a rendszer naponta határozza meg és alkalmazza.</span><span class="sxs-lookup"><span data-stu-id="df421-174">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="df421-175">Minden előfizetés-mérőnek van egy sora annak a hónapnak minden naphoz, ahol volt használat.</span><span class="sxs-lookup"><span data-stu-id="df421-175">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="df421-176">Az alábbi példában:</span><span class="sxs-lookup"><span data-stu-id="df421-176">In the example below:</span></span>

  - <span data-ttu-id="df421-177">A 7/1 és 7/3 között kezelt szolgáltatások partneri jóváírásának mérői (vegye figyelembe, hogy a tényleges egységár a kiskereskedelmi ár és a partneri jóváírás. </span><span class="sxs-lookup"><span data-stu-id="df421-177">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="df421-178">A mérő nem  kapott partneri jóváírást a 7/4–7/7 között kezelt szolgáltatásokhoz (vegye figyelembe, hogy a tényleges egységár a kiskereskedelmi ár).</span><span class="sxs-lookup"><span data-stu-id="df421-178">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="df421-179">A 7/8-tól 7/31-ig felügyelt szolgáltatások partneri jóváírásának mérőja (vegye figyelembe, hogy a tényleges egységár a kiskereskedelmi ár és a partneri jóváírások összege). </span><span class="sxs-lookup"><span data-stu-id="df421-179">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="df421-181">Számla az ügyfél pénznemében</span><span class="sxs-lookup"><span data-stu-id="df421-181">Invoice in customer currency</span></span>

<span data-ttu-id="df421-182">Az Azure-csomagon keresztüli Azure-szolgáltatások díjszabása AMERIKAI DOLLÁRban történik, és a számlázás az ügyfél országának hozzárendelt pénznemében történik.</span><span class="sxs-lookup"><span data-stu-id="df421-182">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="df421-183">Ha a számlázási pénznem nem USD, akkor a felhasznált átváltási díj a számla utolsó oldalán jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="df421-183">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="df421-184">Az FX-árfolyamok meghatározása havonta történik, és az alábbi számlán lesz alkalmazva.</span><span class="sxs-lookup"><span data-stu-id="df421-184">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="df421-185">Az ország pénznemek teljes listájáért tekintse meg az új kereskedelmi ajánlatok országonkénti elérhetőségét és az ügyfél [pénznemmátrixát.](https://go.microsoft.com/fwlink/?linkid=2112354)</span><span class="sxs-lookup"><span data-stu-id="df421-185">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="df421-186">A Microsoft egy előre meghatározott átváltási árfolyamot alkalmaz az alap USD-árakra, hogy az egyes naptári hónapban megvásárolt vagy felhasznált Azure-szolgáltatások teljes díjára vonatkozzon.</span><span class="sxs-lookup"><span data-stu-id="df421-186">Microsoft applies a predetermined exchange rate to base USD prices to arrive at total charges incurred for Azure services purchased or consumed each calendar month.</span></span> <span data-ttu-id="df421-187">A havi átváltási árfolyam a Thomson Reuters által (általában) az előző hónap vége előtt két munkanap, 16:00-kor (GMT) közzétett árfolyam.</span><span class="sxs-lookup"><span data-stu-id="df421-187">The monthly exchange rate is the mid-rate published by Thomson Reuters (typically) two business days prior to the preceding month-end at 4:00 pm GMT.</span></span> 

<span data-ttu-id="df421-188">**Például:** A Microsoft decemberi árfolyama a Thomson Reuters középárfolyama november 29-én vagy körül lenne egy adott pénznemben.</span><span class="sxs-lookup"><span data-stu-id="df421-188">**For example,** Microsoft’s December exchange rate would be the Thomson Reuters mid-rate on or around November 29 for a given currency.</span></span> <span data-ttu-id="df421-189">Ez a díj az ebben a pénznemben történt összes vásárlásra alkalmazva lesz december 1-től december 31-ig.</span><span class="sxs-lookup"><span data-stu-id="df421-189">That rate will be applied to all purchases in that currency from December 1 to December 31.</span></span> 

## <a name="azure-reservations"></a><span data-ttu-id="df421-190">Azure Reserved Virtual Machine Instances</span><span class="sxs-lookup"><span data-stu-id="df421-190">Azure reservations</span></span>


<span data-ttu-id="df421-191">Ha [Azure-foglalásokat vásárol](azure-reservations.md) egy Azure-csomagon keresztül, választhat egy egyszeres vagy havi számlázást.</span><span class="sxs-lookup"><span data-stu-id="df421-191">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="df421-192">Azure-költség</span><span class="sxs-lookup"><span data-stu-id="df421-192">Azure spending</span></span>

<span data-ttu-id="df421-193">A rendszer frissíti a meglévő Azure-kiadásokat, hogy támogassa az új Azure-csomag számlázását a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="df421-193">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="df421-194">Ez lehetővé teszi a partnerek számára a következőt:</span><span class="sxs-lookup"><span data-stu-id="df421-194">This enables partners to:</span></span>

- <span data-ttu-id="df421-195">Az ügyfélszinten beállított költségvetéssel kapcsolatos riasztások megtekintése, kezelése és fogadása</span><span class="sxs-lookup"><span data-stu-id="df421-195">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="df421-196">Egy Azure-csomag összes becsült kiadásának megtekintése (erőforrás- és fogyasztásmérő-szint szerint bontva)</span><span class="sxs-lookup"><span data-stu-id="df421-196">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="df421-197">Mivel az Azure-szolgáltatások Azure-csomagon keresztüli számlázási modellje használat utáni használat, a vártnál nagyobb számla elkerülése érdekében a partnerek havi költségvetést alkalmazhatnak, és nyomon követhetik a használat százalékos arányát.</span><span class="sxs-lookup"><span data-stu-id="df421-197">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="df421-198">A költségvetés egyszerre egy ügyfélre vagy több ügyfélre is alkalmazható.</span><span class="sxs-lookup"><span data-stu-id="df421-198">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure-kiadások.":::

## <a name="next-steps"></a><span data-ttu-id="df421-200">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="df421-200">Next steps</span></span>

- <span data-ttu-id="df421-201">Tekintse meg a partneri jóváírás (PEC) kiszámításának módját.</span><span class="sxs-lookup"><span data-stu-id="df421-201">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="df421-202">Jelentkezzen be az Partnerközpont [irányítópultra,](https://partner.microsoft.com/dashboard/) és keresse meg az elérhető árlistát.</span><span class="sxs-lookup"><span data-stu-id="df421-202">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="df421-203">Tudnivalók az [Azure-csomag megvásárlásáról](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="df421-203">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="df421-204">Tekintse meg a CSP új kereskedelmi [élményének árlistát](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="df421-204">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
