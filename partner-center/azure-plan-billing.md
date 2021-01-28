---
title: Azure-csomag számlázása – & Recon-fájlok számlázása
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan érheti el és értelmezheti az Azure-csomag számlázásával kapcsolatos számlázási és egyeztetési adatstruktúrát.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 819f90ca9a8467de4a8001a1b10f8409d3fb1b81
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/28/2021
ms.locfileid: "98924997"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="9708d-103">Új kereskedelmi felület a CSP-ben – Azure-számlázás</span><span class="sxs-lookup"><span data-stu-id="9708d-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="9708d-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="9708d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9708d-105">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="9708d-105">Admin agent</span></span>
- <span data-ttu-id="9708d-106">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="9708d-106">Billing admin</span></span>
- <span data-ttu-id="9708d-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="9708d-107">Global admin</span></span>

<span data-ttu-id="9708d-108">Ez a cikk azt ismerteti, hogyan érheti el és értelmezheti az Azure-csomag számlázásával kapcsolatos számlázási és egyeztetési fájlrendszert.</span><span class="sxs-lookup"><span data-stu-id="9708d-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="9708d-109">Az Azure-csomag keretében történő számlázás egy egyszerűsített számlázási élmény, amely egy igazított, egyetlen számlázási dátummal és naptári hónapra alapuló számlázási időszakot használ.</span><span class="sxs-lookup"><span data-stu-id="9708d-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="9708d-110">A számlázási alapok összefoglalása</span><span class="sxs-lookup"><span data-stu-id="9708d-110">Summary of billing essentials</span></span>

- <span data-ttu-id="9708d-111">**Számla dátuma**: a számla-és egyeztetési fájl elérhető lesz a partner Center irányítópultján/API-ban (UTC szerint éjfélkor).</span><span class="sxs-lookup"><span data-stu-id="9708d-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="9708d-112">**Számla számlázási időszaka**: a számlázási időszak a naptári hónapra van igazítva, például 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="9708d-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="9708d-113">Díjszabási **szolgáltatási időszakok**: a díjak a naptári hónapra lesznek igazítva.</span><span class="sxs-lookup"><span data-stu-id="9708d-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="9708d-114">Ha például a számlázott partner Azure-szolgáltatásokat ad egy 10/15-es Azure-csomagon keresztül, és az ügyfél megkezdi az Azure-szolgáltatások az 10/15-on való felhasználását, akkor a számlázott partner a 11/8-as szolgáltatási 10/15-10/31 időszakra vonatkozó számlázást és felderítést is megkapja a-on.</span><span class="sxs-lookup"><span data-stu-id="9708d-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="9708d-115">A következő havi számla, amelyet a 12/8-es előállítás fog generálni, a 11/1-11/31-es szolgáltatási időszakra vonatkozó összes díjat tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="9708d-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="9708d-116">**Számla fizetési ideje**: nettó 60 nap.</span><span class="sxs-lookup"><span data-stu-id="9708d-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="9708d-117">**Számla pénzneme**: január 28-ig 2021, az EU/EFTA és az Egyesült Királyság régiójában lévő partnereink, akik új ügyfelekkel és meglévő CSP-ügyfelekkel vásárolnak új kereskedelmi ajánlatokat az első alkalommal, amikor a bérlők a 2020. május 11. előtt jöttek létre, a partneri hely pénznemében megjelenő vásárlásért kell fizetni.</span><span class="sxs-lookup"><span data-stu-id="9708d-117">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="9708d-118">Az EU/EFTA és az Egyesült Királyság régióján kívüli partnerek továbbra is a partneri hely pénznemében lesznek számlázva.</span><span class="sxs-lookup"><span data-stu-id="9708d-118">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="9708d-119">**Partneri ösztönzők**: a számlázási hónap végétől számított 45 nappal.</span><span class="sxs-lookup"><span data-stu-id="9708d-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="9708d-120">A számlák és a megbékélési fájlok elérése</span><span class="sxs-lookup"><span data-stu-id="9708d-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="9708d-121">A vállalat globális rendszergazdája vagy számlázási rendszergazdája e-mailt fog kapni, ha a számla készen áll a megtekintésre.</span><span class="sxs-lookup"><span data-stu-id="9708d-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="9708d-122">A számla és a megbékélési fájl elérése:</span><span class="sxs-lookup"><span data-stu-id="9708d-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="9708d-123">Jelentkezzen be a Partnerközpont [irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="9708d-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="9708d-124">A partner Center menüben válassza a **számlázás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="9708d-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="9708d-125">Válassza ki az **ismétlődő** és az **egyszeri** , valamint a pénznemhez tartozó lapot.</span><span class="sxs-lookup"><span data-stu-id="9708d-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="számlázási":::

4. <span data-ttu-id="9708d-127">Válassza a **számla** vagy a **megbékélési fájl** elemet.</span><span class="sxs-lookup"><span data-stu-id="9708d-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="9708d-128">A korábbi számlák és a felderítési fájlok megtekintéséhez bontsa ki az alábbi számlázási előzmények sort.</span><span class="sxs-lookup"><span data-stu-id="9708d-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="9708d-129">A használati adatok ismertetése</span><span class="sxs-lookup"><span data-stu-id="9708d-129">Understanding usage data</span></span> 

1. <span data-ttu-id="9708d-130">Az Azure-csomag a legfelső szintű vagy legfelső szintű tároló a használathoz.</span><span class="sxs-lookup"><span data-stu-id="9708d-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="9708d-131">Minden használat egyetlen Azure-csomaghoz van kötve.</span><span class="sxs-lookup"><span data-stu-id="9708d-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="9708d-132">Egy csomagon belül egy vagy több Azure-előfizetés lesz.</span><span class="sxs-lookup"><span data-stu-id="9708d-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="9708d-133">Ezek az erőforrások kezeléséhez és üzembe helyezéséhez használt tárolók.</span><span class="sxs-lookup"><span data-stu-id="9708d-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="9708d-134">Egy előfizetésen belül erőforráscsoportok hozzáadásával csoportosíthatja az erőforrásokat.</span><span class="sxs-lookup"><span data-stu-id="9708d-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="9708d-135">Minden erőforrás üzembe helyezése egy erőforráscsoporthoz történik.</span><span class="sxs-lookup"><span data-stu-id="9708d-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="9708d-136">Ilyenek például a virtuális gépek és a Storage-fiókok.</span><span class="sxs-lookup"><span data-stu-id="9708d-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="9708d-137">Erőforrás-kibocsátó mérőszámok: a mérőórák egy erőforrás felhasználásának mérései, és egy erőforrás több fogyasztásmérőn is kibocsáthatja a használatot.</span><span class="sxs-lookup"><span data-stu-id="9708d-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="9708d-138">A mérőórákat a termékkód, a SKUId és a AvailabilityId azonosítja.</span><span class="sxs-lookup"><span data-stu-id="9708d-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="9708d-139">Az előfizetési erőforráscsoportok és a mérések hierarchiája</span><span class="sxs-lookup"><span data-stu-id="9708d-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="9708d-140">**Azure-fiók (bérlő)**</span><span class="sxs-lookup"><span data-stu-id="9708d-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="9708d-141">Előfizetés A</span><span class="sxs-lookup"><span data-stu-id="9708d-141">Subscription A</span></span>
    - <span data-ttu-id="9708d-142">1. ResourceGroup</span><span class="sxs-lookup"><span data-stu-id="9708d-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="9708d-143">Virtuális gép (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="9708d-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="9708d-144">Számítási fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="9708d-144">Compute meter</span></span>
        - <span data-ttu-id="9708d-145">Virtuális hálózat (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="9708d-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="9708d-146">Nincs számlázási fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="9708d-146">No billing meter</span></span>

    - <span data-ttu-id="9708d-147">2. ResourceGroup</span><span class="sxs-lookup"><span data-stu-id="9708d-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="9708d-148">Virtuális gép (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="9708d-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="9708d-149">Számítógép-fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="9708d-149">Computer meter</span></span>
        - <span data-ttu-id="9708d-150">Prémium SSD felügyelt lemez (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="9708d-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="9708d-151">Tárolási kapacitás mérője</span><span class="sxs-lookup"><span data-stu-id="9708d-151">Storage capacity meter</span></span>
            - <span data-ttu-id="9708d-152">Tárolási műveleti fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="9708d-152">Storage operations meter</span></span>

- <span data-ttu-id="9708d-153">Előfizetés B-ResourceGroup 1 – Azure SQL (erőforrás) – DTU-mérő-VPN Gateway (erőforrás) – VPN Gateway-mérő</span><span class="sxs-lookup"><span data-stu-id="9708d-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="9708d-154">2. ResourceGroup</span><span class="sxs-lookup"><span data-stu-id="9708d-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="9708d-155">Virtual Network csatoló (erőforrás)</span><span class="sxs-lookup"><span data-stu-id="9708d-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="9708d-156">Nincs számlázási fogyasztásmérő</span><span class="sxs-lookup"><span data-stu-id="9708d-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="9708d-157">A számla elolvasása</span><span class="sxs-lookup"><span data-stu-id="9708d-157">Read the invoice</span></span>

1. <span data-ttu-id="9708d-158">A számla az egyes hónapok nyolcadik napján nem lesz elérhető.</span><span class="sxs-lookup"><span data-stu-id="9708d-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="9708d-159">A partnereknek 60 napja van a fizetésre.</span><span class="sxs-lookup"><span data-stu-id="9708d-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="9708d-160">A számlázási időszak egy adott naptári hónapra vonatkozni fog, például 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="9708d-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="9708d-161">A díjak nettó kiigazítások (az összeg a "partner által felügyelt szolgáltatások által kezelt kreditek" nettó mennyisége).</span><span class="sxs-lookup"><span data-stu-id="9708d-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="9708d-162">További számlázási részletekért tekintse át a számla-felderítési fájlt és a napi minősítésű használati fájlt.</span><span class="sxs-lookup"><span data-stu-id="9708d-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="számla":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="9708d-164">A számlázási egyeztetési fájl elolvasása</span><span class="sxs-lookup"><span data-stu-id="9708d-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="9708d-165">Minden egyes Azure-csomag és-mérési kombináció legfeljebb két számlázási sorral rendelkezhet a Recon-fájlban.</span><span class="sxs-lookup"><span data-stu-id="9708d-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="9708d-166">Ha a mérőszám a teljes naptári hónapban bármilyen típusú kedvezményt vagy kreditet (például a többrétegű kedvezményeket vagy a partner által kezelt szolgáltatások kreditjét) minősítette, akkor a felderítési fájl csak egy számlázási sort fog tartalmazni.</span><span class="sxs-lookup"><span data-stu-id="9708d-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="9708d-167">A **PriceAdjusmentDescription** oszlop a kedvezményre vagy a keresett kreditre hivatkozik.</span><span class="sxs-lookup"><span data-stu-id="9708d-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="9708d-168">Ha nincs olyan erőforrás egy adott mérőszámhoz, amely kedvezményre vagy partner által felhasználható kreditre van kiértékelve, akkor a felderítési fájl csak egy számlázási sort fog tartalmazni, és a hatályos egység ára a kiskereskedelmi díj (amely az egység díja).</span><span class="sxs-lookup"><span data-stu-id="9708d-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="9708d-169">Ha a mérő, vagy bármely olyan erőforrás, amely az adott mérőszámot kibocsátja, a partner által a hónap egy részében **kezelt szolgáltatásokra vonatkozó jóváírásra** jogosult, a Recon-fájl két számlázási sort fog tartalmazni.</span><span class="sxs-lookup"><span data-stu-id="9708d-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="9708d-170">Az egyik sor azokat a napokat jelöli, amelyeknek a mérőszáma minősített, a második sor pedig azon napokat jelöli, amelyeknek a mérőszáma nem volt</span><span class="sxs-lookup"><span data-stu-id="9708d-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="9708d-171">A napi használati fájl elolvasása</span><span class="sxs-lookup"><span data-stu-id="9708d-171">Read the daily usage file</span></span>

- <span data-ttu-id="9708d-172">Az előfizetési mérőszámok az Azure-csomag keretében vannak értékelve, és naponta halmozódnak.</span><span class="sxs-lookup"><span data-stu-id="9708d-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="9708d-173">A **felügyelt szolgáltatásokhoz tartozó partner által létrehozott kreditek** napi rendszerességgel vannak meghatározva és alkalmazva.</span><span class="sxs-lookup"><span data-stu-id="9708d-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="9708d-174">Minden előfizetési fogyasztásmérőnek van egy sora a hónap minden napján, amelyben használatban volt.</span><span class="sxs-lookup"><span data-stu-id="9708d-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="9708d-175">Az alábbi példában:</span><span class="sxs-lookup"><span data-stu-id="9708d-175">In the example below:</span></span>

  - <span data-ttu-id="9708d-176">A 7/1-7/3-től **felügyelt szolgáltatások esetében a partner által szerzett kreditek** díja</span><span class="sxs-lookup"><span data-stu-id="9708d-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="9708d-177">A mérő nem felelt meg a partner által a 7/4-7/7-től **felügyelt szolgáltatásokra vonatkozó kreditért** (a tényleges egység ára a kiskereskedelmi díj).</span><span class="sxs-lookup"><span data-stu-id="9708d-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="9708d-178">A 7/8-7/31-től **felügyelt szolgáltatások esetében a partner által szerzett kreditek** díja (a tényleges egység ára a kiskereskedelmi ár, a partner által szerzett kredit).</span><span class="sxs-lookup"><span data-stu-id="9708d-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="9708d-180">Számla az ügyfél pénznemében</span><span class="sxs-lookup"><span data-stu-id="9708d-180">Invoice in customer currency</span></span>

<span data-ttu-id="9708d-181">Az Azure-csomagokon keresztül az Azure-szolgáltatások díja USD lesz, és az ügyfél-országhoz rendelt pénznemben kell fizetni.</span><span class="sxs-lookup"><span data-stu-id="9708d-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="9708d-182">Ha a számlázási pénznem nem USD, akkor a számla utolsó oldalán a használt deviza-(FX-) díj is megjelenik.</span><span class="sxs-lookup"><span data-stu-id="9708d-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="9708d-183">Az FX díjszabását havonta határozzák meg, és a következő számlára kell alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="9708d-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="9708d-184">Az ország pénznemek teljes listájáért tekintse meg az [új kereskedelmi ajánlatok ország rendelkezésre állását és az ügyfél pénznemének mátrixát](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="9708d-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="9708d-185">A Microsoft a londoni tőzsdei árfolyamot követi az átalakításhoz.</span><span class="sxs-lookup"><span data-stu-id="9708d-185">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="9708d-186">Az árfolyamot használjuk, amely a Londoni Értéktőzsdén a hónap utolsó munkanapján rögzített árfolyamot használja fel az utóbbi időben.</span><span class="sxs-lookup"><span data-stu-id="9708d-186">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="9708d-187">Az FX díjszabása a hónap első előtti napján frissül és elérhető lesz.</span><span class="sxs-lookup"><span data-stu-id="9708d-187">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="9708d-188">Azure Reserved Virtual Machine Instances</span><span class="sxs-lookup"><span data-stu-id="9708d-188">Azure reservations</span></span>


<span data-ttu-id="9708d-189">Az Azure- [foglalások](azure-reservations.md) Azure-csomagon keresztüli megvásárlásakor egyszeri vagy havi számlázást is választhat.</span><span class="sxs-lookup"><span data-stu-id="9708d-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="9708d-190">Azure-költség</span><span class="sxs-lookup"><span data-stu-id="9708d-190">Azure spending</span></span>

<span data-ttu-id="9708d-191">A meglévő Azure-kiadások a partner Centerben új Azure-csomag számlázásának támogatásához frissülnek.</span><span class="sxs-lookup"><span data-stu-id="9708d-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="9708d-192">Ez lehetővé teszi a partnerek számára a következőket:</span><span class="sxs-lookup"><span data-stu-id="9708d-192">This enables partners to:</span></span>

- <span data-ttu-id="9708d-193">A költségvetési készletre vonatkozó riasztások megtekintése, kezelése és fogadása az ügyfél szintjén</span><span class="sxs-lookup"><span data-stu-id="9708d-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="9708d-194">Az Azure-csomag becsült összes kiadásának megtekintése (erőforrás-és mérési szint szerinti bontásban)</span><span class="sxs-lookup"><span data-stu-id="9708d-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="9708d-195">Mivel az Azure-szolgáltatások számlázási modellje az Azure-csomagon keresztüli fizetés utáni használatot jelent, hogy a vártnál nagyobb mennyiségű számla elkerülhető legyen, a partnerek havi költségvetést alkalmazhatnak, és nyomon követhetik a használat százalékos arányát.</span><span class="sxs-lookup"><span data-stu-id="9708d-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="9708d-196">Egy költségvetést egyszerre csak egy vagy több ügyfélre lehet alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="9708d-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure-költség":::

## <a name="next-steps"></a><span data-ttu-id="9708d-198">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="9708d-198">Next steps</span></span>

- <span data-ttu-id="9708d-199">Megtudhatja, hogyan számítja ki a partner által létrehozott kreditet (PEC).</span><span class="sxs-lookup"><span data-stu-id="9708d-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="9708d-200">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/) , és keresse meg az elérhető árlista listáját.</span><span class="sxs-lookup"><span data-stu-id="9708d-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="9708d-201">További információ [Az Azure-csomag megvásárlásáról](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="9708d-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="9708d-202">Tekintse meg a [CSP új kereskedelmi élményét ismertető árlistát](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="9708d-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
