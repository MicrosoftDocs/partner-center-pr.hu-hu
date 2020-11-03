---
title: Azure-csomag számlázása – & Recon-fájlok számlázása
ms.topic: article
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan érheti el és értelmezheti az Azure-csomag számlázásával kapcsolatos számlázási és egyeztetési adatstruktúrát.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5d8bb85357d796ae4917faf91c93db8fef4369c2
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528491"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="a0a05-103">Új kereskedelmi élmény a CSP-ben – Azure-számlázás</span><span class="sxs-lookup"><span data-stu-id="a0a05-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="a0a05-104">**Megfelelő szerepkörök:**</span><span class="sxs-lookup"><span data-stu-id="a0a05-104">**Appropriate roles:**</span></span>

- <span data-ttu-id="a0a05-105">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="a0a05-105">Admin agent</span></span>
- <span data-ttu-id="a0a05-106">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="a0a05-106">Billing admin</span></span>
- <span data-ttu-id="a0a05-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="a0a05-107">Global admin</span></span>

<span data-ttu-id="a0a05-108">Az Azure-csomag keretében történő számlázás egy egyszerűsített számlázási élmény, amely egy igazított, egyetlen számlázási dátummal és naptári hónapra alapuló számlázási időszakot használ.</span><span class="sxs-lookup"><span data-stu-id="a0a05-108">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="a0a05-109">A számlázási alapok összefoglalása</span><span class="sxs-lookup"><span data-stu-id="a0a05-109">Summary of billing essentials</span></span>

- <span data-ttu-id="a0a05-110">**Számla dátuma** : a számla-és egyeztetési fájl elérhető lesz a partner Center irányítópultján/API-ban (UTC szerint éjfélkor).</span><span class="sxs-lookup"><span data-stu-id="a0a05-110">**Invoice date** : Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="a0a05-111">**Számla számlázási időszaka** : a számlázási időszak a naptári hónapra van igazítva, például 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="a0a05-111">**Invoice billing period** : The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="a0a05-112">Díjszabási **szolgáltatási időszakok** : a díjak a naptári hónapra lesznek igazítva.</span><span class="sxs-lookup"><span data-stu-id="a0a05-112">**Charge service periods** : Charges will align to the calendar month.</span></span> <span data-ttu-id="a0a05-113">Ha például a számlázott partner Azure-szolgáltatásokat ad egy 10/15-es Azure-csomagon keresztül, és az ügyfél megkezdi az Azure-szolgáltatások az 10/15-on való felhasználását, akkor a számlázott partner a 11/8-as szolgáltatási 10/15-10/31 időszakra vonatkozó számlázást és felderítést is megkapja a-on.</span><span class="sxs-lookup"><span data-stu-id="a0a05-113">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="a0a05-114">A következő havi számla, amelyet a 12/8-es előállítás fog generálni, a 11/1-11/31-es szolgáltatási időszakra vonatkozó összes díjat tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="a0a05-114">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="a0a05-115">**Számla fizetési ideje** : nettó 60 nap.</span><span class="sxs-lookup"><span data-stu-id="a0a05-115">**Invoice payment term** : Net 60 days.</span></span>

- <span data-ttu-id="a0a05-116">**Számla pénzneme** : a partnerek továbbra is az ügyfél country's rendelt pénznemében lesznek számlázva.</span><span class="sxs-lookup"><span data-stu-id="a0a05-116">**Invoice currency** : Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="a0a05-117">Ha például a számlázott partner Írországban, az Egyesült Királyságban, Norvégiában és Németországban található ügyfelekkel, akkor a számlázott partner GBP, NOK és EUR számla/Recon összegű számlát kap.</span><span class="sxs-lookup"><span data-stu-id="a0a05-117">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="a0a05-118">**Partneri ösztönzők** : a számlázási hónap végétől számított 45 nappal.</span><span class="sxs-lookup"><span data-stu-id="a0a05-118">**Partner incentives** : Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="a0a05-119">A számlák és a megbékélési fájlok elérése</span><span class="sxs-lookup"><span data-stu-id="a0a05-119">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="a0a05-120">A vállalat globális rendszergazdája vagy számlázási rendszergazdája e-mailt fog kapni, ha a számla készen áll a megtekintésre.</span><span class="sxs-lookup"><span data-stu-id="a0a05-120">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="a0a05-121">A számla és a megbékélési fájl elérése:</span><span class="sxs-lookup"><span data-stu-id="a0a05-121">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="a0a05-122">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="a0a05-122">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="a0a05-123">A partner Center menüben válassza a **számlázás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a0a05-123">From the Partner Center menu, select **Billing** .</span></span>

3. <span data-ttu-id="a0a05-124">Válassza ki az **ismétlődő** és az **egyszeri** , valamint a pénznemhez tartozó lapot.</span><span class="sxs-lookup"><span data-stu-id="a0a05-124">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="számlázási":::

4. <span data-ttu-id="a0a05-126">Válassza a **számla** vagy a **megbékélési fájl** elemet.</span><span class="sxs-lookup"><span data-stu-id="a0a05-126">Select **Invoice** or **Reconciliation file** .</span></span>  

   <span data-ttu-id="a0a05-127">A korábbi számlák és a felderítési fájlok megtekintéséhez bontsa ki az alábbi számlázási előzmények sort.</span><span class="sxs-lookup"><span data-stu-id="a0a05-127">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="a0a05-128">A használati adatok ismertetése</span><span class="sxs-lookup"><span data-stu-id="a0a05-128">Understanding usage data</span></span> 

1. <span data-ttu-id="a0a05-129">Az Azure-csomag a legfelső szintű vagy legfelső szintű tároló a használathoz.</span><span class="sxs-lookup"><span data-stu-id="a0a05-129">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="a0a05-130">Minden használat egyetlen Azure-csomaghoz van kötve.</span><span class="sxs-lookup"><span data-stu-id="a0a05-130">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="a0a05-131">Egy csomagon belül egy vagy több Azure-előfizetés lesz.</span><span class="sxs-lookup"><span data-stu-id="a0a05-131">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="a0a05-132">Ezek az erőforrások kezeléséhez és üzembe helyezéséhez használt tárolók.</span><span class="sxs-lookup"><span data-stu-id="a0a05-132">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="a0a05-133">Egy előfizetésen belül erőforráscsoportok hozzáadásával csoportosíthatja az erőforrásokat.</span><span class="sxs-lookup"><span data-stu-id="a0a05-133">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="a0a05-134">Minden erőforrás üzembe helyezése egy erőforráscsoporthoz történik.</span><span class="sxs-lookup"><span data-stu-id="a0a05-134">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="a0a05-135">Ilyenek például a virtuális gépek és a Storage-fiókok.</span><span class="sxs-lookup"><span data-stu-id="a0a05-135">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="a0a05-136">Erőforrás-kibocsátó mérőszámok: a mérőórák egy erőforrás felhasználásának mérései, és egy erőforrás több fogyasztásmérőn is kibocsáthatja a használatot.</span><span class="sxs-lookup"><span data-stu-id="a0a05-136">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="a0a05-137">A mérőórákat a termékkód, a SKUId és a AvailabilityId azonosítja.</span><span class="sxs-lookup"><span data-stu-id="a0a05-137">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="a0a05-138">Az előfizetési erőforráscsoportok és a mérések hierarchiája</span><span class="sxs-lookup"><span data-stu-id="a0a05-138">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="a0a05-139">**Azure-fiók (bérlő)**</span><span class="sxs-lookup"><span data-stu-id="a0a05-139">**Azure account (tenant)**</span></span>

- <span data-ttu-id="a0a05-140">Előfizetés A</span><span class="sxs-lookup"><span data-stu-id="a0a05-140">Subscription A</span></span>
    - <span data-ttu-id="a0a05-141">1. ResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a0a05-141">ResourceGroup 1</span></span>
        - <span data-ttu-id="a0a05-142">Virtuális gép (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="a0a05-142">Virtual machine (resource)</span></span>
            - <span data-ttu-id="a0a05-143">Számítási fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="a0a05-143">Compute meter</span></span>
        - <span data-ttu-id="a0a05-144">Virtuális hálózat (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="a0a05-144">Virtual network (resource)</span></span>
            - <span data-ttu-id="a0a05-145">Nincs számlázási fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="a0a05-145">No billing meter</span></span>

    - <span data-ttu-id="a0a05-146">2. ResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a0a05-146">ResourceGroup 2</span></span>
        - <span data-ttu-id="a0a05-147">Virtuális gép (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="a0a05-147">Virtual machine (resource)</span></span>
            - <span data-ttu-id="a0a05-148">Számítógép-fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="a0a05-148">Computer meter</span></span>
        - <span data-ttu-id="a0a05-149">Prémium SSD felügyelt lemez (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="a0a05-149">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="a0a05-150">Tárolási kapacitás mérője</span><span class="sxs-lookup"><span data-stu-id="a0a05-150">Storage capacity meter</span></span>
            - <span data-ttu-id="a0a05-151">Tárolási műveleti fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="a0a05-151">Storage operations meter</span></span>

- <span data-ttu-id="a0a05-152">Előfizetés B-ResourceGroup 1 – Azure SQL (erőforrás) – DTU-mérő-VPN Gateway (erőforrás) – VPN Gateway-mérő</span><span class="sxs-lookup"><span data-stu-id="a0a05-152">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="a0a05-153">2. ResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a0a05-153">ResourceGroup 2</span></span>
        - <span data-ttu-id="a0a05-154">Virtual Network csatoló (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="a0a05-154">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="a0a05-155">Nincs számlázási fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="a0a05-155">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="a0a05-156">A számla elolvasása</span><span class="sxs-lookup"><span data-stu-id="a0a05-156">Read the invoice</span></span>

1. <span data-ttu-id="a0a05-157">A számla az egyes hónapok nyolcadik napján nem lesz elérhető.</span><span class="sxs-lookup"><span data-stu-id="a0a05-157">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="a0a05-158">A partnereknek 60 napja van a fizetésre.</span><span class="sxs-lookup"><span data-stu-id="a0a05-158">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="a0a05-159">A számlázási időszak egy adott naptári hónapra vonatkozni fog, például 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="a0a05-159">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="a0a05-160">A díjak nettó kiigazítások (az összeg a "partner által felügyelt szolgáltatások által kezelt kreditek" nettó mennyisége).</span><span class="sxs-lookup"><span data-stu-id="a0a05-160">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="a0a05-161">További számlázási részletekért tekintse át a számla-felderítési fájlt és a napi minősítésű használati fájlt.</span><span class="sxs-lookup"><span data-stu-id="a0a05-161">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="számla":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="a0a05-163">A számlázási egyeztetési fájl elolvasása</span><span class="sxs-lookup"><span data-stu-id="a0a05-163">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="a0a05-164">Minden egyes Azure-csomag és-mérési kombináció legfeljebb két számlázási sorral rendelkezhet a Recon-fájlban.</span><span class="sxs-lookup"><span data-stu-id="a0a05-164">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="a0a05-165">Ha a mérőszám a teljes naptári hónapban bármilyen típusú kedvezményt vagy kreditet (például a többrétegű kedvezményeket vagy a partner által kezelt szolgáltatások kreditjét) minősítette, akkor a felderítési fájl csak egy számlázási sort fog tartalmazni.</span><span class="sxs-lookup"><span data-stu-id="a0a05-165">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="a0a05-166">A **PriceAdjusmentDescription** oszlop a kedvezményre vagy a keresett kreditre hivatkozik.</span><span class="sxs-lookup"><span data-stu-id="a0a05-166">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="a0a05-167">Ha nincs olyan erőforrás egy adott mérőszámhoz, amely kedvezményre vagy partner által felhasználható kreditre van kiértékelve, akkor a felderítési fájl csak egy számlázási sort fog tartalmazni, és a hatályos egység ára a kiskereskedelmi díj (amely az egység díja).</span><span class="sxs-lookup"><span data-stu-id="a0a05-167">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="a0a05-168">Ha a mérő, vagy bármely olyan erőforrás, amely az adott mérőszámot kibocsátja, a partner által a hónap egy részében **kezelt szolgáltatásokra vonatkozó jóváírásra** jogosult, a Recon-fájl két számlázási sort fog tartalmazni.</span><span class="sxs-lookup"><span data-stu-id="a0a05-168">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="a0a05-169">Az egyik sor azokat a napokat jelöli, amelyeknek a mérőszáma minősített, a második sor pedig azon napokat jelöli, amelyeknek a mérőszáma nem volt</span><span class="sxs-lookup"><span data-stu-id="a0a05-169">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="a0a05-170">A napi használati fájl elolvasása</span><span class="sxs-lookup"><span data-stu-id="a0a05-170">Read the daily usage file</span></span>

- <span data-ttu-id="a0a05-171">Az előfizetési mérőszámok az Azure-csomag keretében vannak értékelve, és naponta halmozódnak.</span><span class="sxs-lookup"><span data-stu-id="a0a05-171">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="a0a05-172">A **felügyelt szolgáltatásokhoz tartozó partner által létrehozott kreditek** napi rendszerességgel vannak meghatározva és alkalmazva.</span><span class="sxs-lookup"><span data-stu-id="a0a05-172">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="a0a05-173">Minden előfizetési fogyasztásmérőnek van egy sora a hónap minden napján, amelyben használatban volt.</span><span class="sxs-lookup"><span data-stu-id="a0a05-173">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="a0a05-174">Az alábbi példában:</span><span class="sxs-lookup"><span data-stu-id="a0a05-174">In the example below:</span></span>

  - <span data-ttu-id="a0a05-175">A 7/1-7/3-től **felügyelt szolgáltatások esetében a partner által szerzett kreditek** díja</span><span class="sxs-lookup"><span data-stu-id="a0a05-175">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="a0a05-176">A mérő nem felelt meg a partner által a 7/4-7/7-től **felügyelt szolgáltatásokra vonatkozó kreditért** (a tényleges egység ára a kiskereskedelmi díj).</span><span class="sxs-lookup"><span data-stu-id="a0a05-176">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="a0a05-177">A 7/8-7/31-től **felügyelt szolgáltatások esetében a partner által szerzett kreditek** díja (a tényleges egység ára a kiskereskedelmi ár, a partner által szerzett kredit).</span><span class="sxs-lookup"><span data-stu-id="a0a05-177">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="a0a05-179">Számla az ügyfél pénznemében</span><span class="sxs-lookup"><span data-stu-id="a0a05-179">Invoice in customer currency</span></span>

<span data-ttu-id="a0a05-180">Az Azure-csomagokon keresztül az Azure-szolgáltatások díja USD lesz, és az ügyfél-országhoz rendelt pénznemben kell fizetni.</span><span class="sxs-lookup"><span data-stu-id="a0a05-180">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="a0a05-181">Ha a számlázási pénznem nem USD, akkor a számla utolsó oldalán a használt deviza-(FX-) díj is megjelenik.</span><span class="sxs-lookup"><span data-stu-id="a0a05-181">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="a0a05-182">Az FX díjszabását havonta határozzák meg, és a következő számlára kell alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="a0a05-182">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="a0a05-183">Az ország pénznemek teljes listájáért tekintse meg az [új kereskedelmi ajánlatok ország rendelkezésre állását és az ügyfél pénznemének mátrixát](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="a0a05-183">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="a0a05-184">A Microsoft a Thomson Reuters használatával határozza meg, hogy milyen FX-díjakat kell kiszámítani az árképzés pénznemének számlázására.</span><span class="sxs-lookup"><span data-stu-id="a0a05-184">Microsoft will use Thomson Reuters to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="a0a05-185">Az FX díjszabása a hónap első előtti napján frissül és elérhető lesz.</span><span class="sxs-lookup"><span data-stu-id="a0a05-185">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="a0a05-186">**Példa** : a szolgáltatási időszak augusztus 1-től augusztus 31-ig érvényes használati díjait a számlázás a július 31-ig közzétett FX-díj alapján számoljuk el.</span><span class="sxs-lookup"><span data-stu-id="a0a05-186">**Example** :  Usage charges for the service period August 1 - August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="a0a05-187">Ezek a díjak a szeptember számlán jelennek meg, és az FX-díjat a számla utolsó oldalán fogjuk feltüntetni.</span><span class="sxs-lookup"><span data-stu-id="a0a05-187">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="a0a05-188">Azure Reserved Virtual Machine Instances</span><span class="sxs-lookup"><span data-stu-id="a0a05-188">Azure reservations</span></span>


<span data-ttu-id="a0a05-189">Az Azure- [foglalások](azure-reservations.md) Azure-csomagon keresztüli megvásárlásakor egyszeri vagy havi számlázást is választhat.</span><span class="sxs-lookup"><span data-stu-id="a0a05-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="a0a05-190">Azure-költség</span><span class="sxs-lookup"><span data-stu-id="a0a05-190">Azure spending</span></span>

<span data-ttu-id="a0a05-191">A meglévő Azure-kiadások a partner Centerben új Azure-csomag számlázásának támogatásához frissülnek.</span><span class="sxs-lookup"><span data-stu-id="a0a05-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="a0a05-192">Ez lehetővé teszi a partnerek számára a következőket:</span><span class="sxs-lookup"><span data-stu-id="a0a05-192">This enables partners to:</span></span>

- <span data-ttu-id="a0a05-193">A költségvetési készletre vonatkozó riasztások megtekintése, kezelése és fogadása az ügyfél szintjén</span><span class="sxs-lookup"><span data-stu-id="a0a05-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="a0a05-194">Az Azure-csomag becsült összes kiadásának megtekintése (erőforrás-és mérési szint szerinti bontásban)</span><span class="sxs-lookup"><span data-stu-id="a0a05-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="a0a05-195">Mivel az Azure-szolgáltatások számlázási modellje az Azure-csomagon keresztüli fizetés utáni használatot jelent, hogy a vártnál nagyobb mennyiségű számla elkerülhető legyen, a partnerek havi költségvetést alkalmazhatnak, és nyomon követhetik a használat százalékos arányát.</span><span class="sxs-lookup"><span data-stu-id="a0a05-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="a0a05-196">Egy költségvetést egyszerre csak egy vagy több ügyfélre lehet alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="a0a05-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure-költség":::

## <a name="next-steps"></a><span data-ttu-id="a0a05-198">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="a0a05-198">Next steps</span></span>

- <span data-ttu-id="a0a05-199">Megtudhatja, hogyan számítja ki a partner által létrehozott kreditet (PEC).</span><span class="sxs-lookup"><span data-stu-id="a0a05-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="a0a05-200">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/) , és keresse meg az elérhető árlista listáját.</span><span class="sxs-lookup"><span data-stu-id="a0a05-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="a0a05-201">További információ [Az Azure-csomag megvásárlásáról](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="a0a05-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="a0a05-202">Tekintse meg a [CSP új kereskedelmi élményét ismertető árlistát](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="a0a05-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
