---
title: Érvényes egységár kiszámítása
ms.topic: how-to
ms.date: 11/10/2020
description: Ismerje meg a hatályos árat és a számítás módját. Egy minta számítást tartalmaz.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/11/2020
ms.locfileid: "94499137"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="e754f-104">Az Azure-csomag felhasználásának tényleges számítási egysége</span><span class="sxs-lookup"><span data-stu-id="e754f-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="e754f-105">A hatályos egység ára</span><span class="sxs-lookup"><span data-stu-id="e754f-105">The effective unit price</span></span>

<span data-ttu-id="e754f-106">A tényleges egység árát a mérési szint alapján számítjuk ki (az erőforrás szintjével szemben), és napi rendszerességgel korrigáljuk a mérési adatok alapján.</span><span class="sxs-lookup"><span data-stu-id="e754f-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="e754f-107">A következő három tényezővel számítjuk ki a hatályos egység árát:</span><span class="sxs-lookup"><span data-stu-id="e754f-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="e754f-108">A teljes számlázási ciklusban naponta figyelt felhasználás</span><span class="sxs-lookup"><span data-stu-id="e754f-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="e754f-109">A fogyasztásmérő számlázandó díja</span><span class="sxs-lookup"><span data-stu-id="e754f-109">Billable cost for the meter</span></span>
- <span data-ttu-id="e754f-110">Rétegek (ha alkalmazható)</span><span class="sxs-lookup"><span data-stu-id="e754f-110">Tiering (if applicable)</span></span>

<span data-ttu-id="e754f-111">Mivel napi rendszerességgel figyeli a használatot a számlázási időszakban, a hatályos egység ára ingadozni fog.</span><span class="sxs-lookup"><span data-stu-id="e754f-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="e754f-112">Az adott elszámolási időszakra vonatkozó végleges díj a felhasználás kiszámításának leállítása és a számlázási idő lezárása után lesz elérhető.</span><span class="sxs-lookup"><span data-stu-id="e754f-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="e754f-113">A legtöbb változást a negyedik vagy az ötödik tizedesjegy után fogja látni.</span><span class="sxs-lookup"><span data-stu-id="e754f-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="e754f-114">Megtudhatja, hogy a mérőszám a lépcsőzetes díjszabást használja-e</span><span class="sxs-lookup"><span data-stu-id="e754f-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="e754f-115">Ha nem tudja, hogy a mérőszáma a lépcsőzetes díjszabást használja-e, az alábbi eljárással derítheti ki.</span><span class="sxs-lookup"><span data-stu-id="e754f-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="e754f-116">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="e754f-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="e754f-117">Válassza az **értékesítés** lehetőséget, válassza a **díjszabás és ajánlatok** lehetőséget, majd válassza az **Azure-csomag díjszabása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e754f-117">Select **Sell** , select **Pricing and offers** , and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="e754f-118">Keresse meg a mérőt azonosító alapján, majd töltse le a díjszabási adatait.</span><span class="sxs-lookup"><span data-stu-id="e754f-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="e754f-119">Minta kiszámítása</span><span class="sxs-lookup"><span data-stu-id="e754f-119">Sample calculation</span></span>

<span data-ttu-id="e754f-120">Az alábbi táblázat bemutatja, hogyan számítjuk ki a hatályos egység árát a nyitott időszak alatt.</span><span class="sxs-lookup"><span data-stu-id="e754f-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="e754f-121">A táblázatban a következő értékek érvényesek:</span><span class="sxs-lookup"><span data-stu-id="e754f-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="e754f-122">**Up** = az erőforrás egységenkénti ára/óra = 0,868</span><span class="sxs-lookup"><span data-stu-id="e754f-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="e754f-123">**BCU** = a mérőhöz tartozó számlázható fogyasztási egység</span><span class="sxs-lookup"><span data-stu-id="e754f-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="e754f-124">**BC** = a mérőhöz tartozó számlázandó díj = BCU \* fel \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="e754f-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="e754f-125">Ez megfelel a 15%-os PEC kedvezmény beállításának.</span><span class="sxs-lookup"><span data-stu-id="e754f-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="e754f-126">Ezután a függvény alsó határát használjuk az értéknek a tizedesvessző utáni két számjegyre való korlátozásához a minimális mennyiség kiszámításához.</span><span class="sxs-lookup"><span data-stu-id="e754f-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="e754f-127">**Érvényes egységár** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="e754f-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="e754f-128">Megjegyzés: az ebben a példában szereplő mérőszám nem rendelkezik a díjszabási csomaggal.</span><span class="sxs-lookup"><span data-stu-id="e754f-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="e754f-129">Date</span><span class="sxs-lookup"><span data-stu-id="e754f-129">Date</span></span> | <span data-ttu-id="e754f-130">BCU (számlázható fogyasztási egység)</span><span class="sxs-lookup"><span data-stu-id="e754f-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="e754f-131">BC (számlázható díj)</span><span class="sxs-lookup"><span data-stu-id="e754f-131">BC (Billable cost)</span></span> | <span data-ttu-id="e754f-132">Érvényes Egységár</span><span class="sxs-lookup"><span data-stu-id="e754f-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="e754f-133">3 – augusztus</span><span class="sxs-lookup"><span data-stu-id="e754f-133">3-Aug</span></span> | <span data-ttu-id="e754f-134">29</span><span class="sxs-lookup"><span data-stu-id="e754f-134">29</span></span> | <span data-ttu-id="e754f-135">21,39</span><span class="sxs-lookup"><span data-stu-id="e754f-135">21.39</span></span> | <span data-ttu-id="e754f-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="e754f-136">0.737586206896552</span></span> |
| <span data-ttu-id="e754f-137">10 – augusztus</span><span class="sxs-lookup"><span data-stu-id="e754f-137">10-Aug</span></span> | <span data-ttu-id="e754f-138">210,950039</span><span class="sxs-lookup"><span data-stu-id="e754f-138">210.950039</span></span> | <span data-ttu-id="e754f-139">155,63</span><span class="sxs-lookup"><span data-stu-id="e754f-139">155.63</span></span> | <span data-ttu-id="e754f-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="e754f-140">0.737757626107858</span></span> |
| <span data-ttu-id="e754f-141">25 – augusztus</span><span class="sxs-lookup"><span data-stu-id="e754f-141">25-Aug</span></span> | <span data-ttu-id="e754f-142">555,950039</span><span class="sxs-lookup"><span data-stu-id="e754f-142">555.950039</span></span> | <span data-ttu-id="e754f-143">410,17</span><span class="sxs-lookup"><span data-stu-id="e754f-143">410.17</span></span> | <span data-ttu-id="e754f-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="e754f-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="e754f-145">További lépések</span><span class="sxs-lookup"><span data-stu-id="e754f-145">Next steps</span></span>

- [<span data-ttu-id="e754f-146">Számlázás és adók</span><span class="sxs-lookup"><span data-stu-id="e754f-146">Billing and taxes</span></span>](billing.md)
