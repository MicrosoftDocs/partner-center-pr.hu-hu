---
title: Tényleges egységár kiszámítása
ms.topic: how-to
ms.date: 04/02/2021
description: Ismerje meg a hatályos egység árát és a számítás módját. Ez a cikk egy minta számítást is tartalmaz.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a662e0b815c979b3454762c5b35eb510887c96ad
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374392"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="8ae16-104">Az Azure-csomag felhasználásának tényleges számítási egysége</span><span class="sxs-lookup"><span data-stu-id="8ae16-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="8ae16-105">A hatályos egység ára</span><span class="sxs-lookup"><span data-stu-id="8ae16-105">The effective unit price</span></span>

<span data-ttu-id="8ae16-106">A tényleges egység árát a mérési szint alapján számítjuk ki (az erőforrás szintjével szemben), és napi rendszerességgel korrigáljuk a mérési adatok alapján.</span><span class="sxs-lookup"><span data-stu-id="8ae16-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="8ae16-107">A következő három tényezővel számítjuk ki a hatályos egység árát:</span><span class="sxs-lookup"><span data-stu-id="8ae16-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="8ae16-108">A teljes számlázási ciklusban naponta figyelt felhasználás</span><span class="sxs-lookup"><span data-stu-id="8ae16-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="8ae16-109">A fogyasztásmérő számlázandó díja</span><span class="sxs-lookup"><span data-stu-id="8ae16-109">Billable cost for the meter</span></span>
- <span data-ttu-id="8ae16-110">Rétegek (ha alkalmazható)</span><span class="sxs-lookup"><span data-stu-id="8ae16-110">Tiering (if applicable)</span></span>

<span data-ttu-id="8ae16-111">Mivel napi rendszerességgel figyeli a használatot a számlázási időszakban, a hatályos egység ára ingadozni fog.</span><span class="sxs-lookup"><span data-stu-id="8ae16-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="8ae16-112">Az adott elszámolási időszakra vonatkozó végleges díj a felhasználás kiszámításának leállítása és a számlázási idő lezárása után lesz elérhető.</span><span class="sxs-lookup"><span data-stu-id="8ae16-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="8ae16-113">A legtöbb változást a negyedik vagy az ötödik tizedesjegy után fogja látni.</span><span class="sxs-lookup"><span data-stu-id="8ae16-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="8ae16-114">Megtudhatja, hogy a mérőszám a lépcsőzetes díjszabást használja-e</span><span class="sxs-lookup"><span data-stu-id="8ae16-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="8ae16-115">Ha nem tudja, hogy a mérőszáma a lépcsőzetes díjszabást használja-e, az alábbi eljárással derítheti ki.</span><span class="sxs-lookup"><span data-stu-id="8ae16-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="8ae16-116">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8ae16-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="8ae16-117">Válassza az **értékesítés** lehetőséget, válassza a **díjszabás és ajánlatok** lehetőséget, majd válassza az **Azure-csomag díjszabása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ae16-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="8ae16-118">Keresse meg a mérőt azonosító alapján, majd töltse le a díjszabási adatait.</span><span class="sxs-lookup"><span data-stu-id="8ae16-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="8ae16-119">Minta kiszámítása</span><span class="sxs-lookup"><span data-stu-id="8ae16-119">Sample calculation</span></span>

<span data-ttu-id="8ae16-120">Az alábbi táblázat bemutatja, hogyan számítjuk ki a hatályos egység árát a nyitott időszak alatt.</span><span class="sxs-lookup"><span data-stu-id="8ae16-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="8ae16-121">A táblázatban a következő értékek érvényesek:</span><span class="sxs-lookup"><span data-stu-id="8ae16-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="8ae16-122">**Up** = az erőforrás egységenkénti ára/óra = 0,868</span><span class="sxs-lookup"><span data-stu-id="8ae16-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="8ae16-123">**BCU** = a mérőhöz tartozó számlázható fogyasztási egység</span><span class="sxs-lookup"><span data-stu-id="8ae16-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="8ae16-124">**BC** = a mérőhöz tartozó számlázandó díj = BCU \* fel \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="8ae16-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="8ae16-125">Ez megfelel a 15%-os PEC kedvezmény beállításának.</span><span class="sxs-lookup"><span data-stu-id="8ae16-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="8ae16-126">Ezután a függvény alsó határát használjuk az értéknek a tizedesvessző utáni két számjegyre való korlátozásához a minimális mennyiség kiszámításához.</span><span class="sxs-lookup"><span data-stu-id="8ae16-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="8ae16-127">**Érvényes egységár** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="8ae16-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="8ae16-128">Az ebben a példában szereplő mérőszámhoz nem tartoznak díjszabási szintek.</span><span class="sxs-lookup"><span data-stu-id="8ae16-128">The meter in this example does not have tiers in pricing.</span></span> <span data-ttu-id="8ae16-129">A hatályos egység díjszabása a kedvezmények százalékában és egyéb beállításokban.</span><span class="sxs-lookup"><span data-stu-id="8ae16-129">The Effective Unit Price factors in discount percentages and other adjustments.</span></span>

| <span data-ttu-id="8ae16-130">Date</span><span class="sxs-lookup"><span data-stu-id="8ae16-130">Date</span></span> | <span data-ttu-id="8ae16-131">BCU (számlázható fogyasztási egység)</span><span class="sxs-lookup"><span data-stu-id="8ae16-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="8ae16-132">BC (számlázható díj)</span><span class="sxs-lookup"><span data-stu-id="8ae16-132">BC (Billable cost)</span></span> | <span data-ttu-id="8ae16-133">Érvényes Egységár</span><span class="sxs-lookup"><span data-stu-id="8ae16-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="8ae16-134">3 – augusztus</span><span class="sxs-lookup"><span data-stu-id="8ae16-134">3-Aug</span></span> | <span data-ttu-id="8ae16-135">29</span><span class="sxs-lookup"><span data-stu-id="8ae16-135">29</span></span> | <span data-ttu-id="8ae16-136">21,39</span><span class="sxs-lookup"><span data-stu-id="8ae16-136">21.39</span></span> | <span data-ttu-id="8ae16-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="8ae16-137">0.737586206896552</span></span> |
| <span data-ttu-id="8ae16-138">10 – augusztus</span><span class="sxs-lookup"><span data-stu-id="8ae16-138">10-Aug</span></span> | <span data-ttu-id="8ae16-139">210,950039</span><span class="sxs-lookup"><span data-stu-id="8ae16-139">210.950039</span></span> | <span data-ttu-id="8ae16-140">155,63</span><span class="sxs-lookup"><span data-stu-id="8ae16-140">155.63</span></span> | <span data-ttu-id="8ae16-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="8ae16-141">0.737757626107858</span></span> |
| <span data-ttu-id="8ae16-142">25 – augusztus</span><span class="sxs-lookup"><span data-stu-id="8ae16-142">25-Aug</span></span> | <span data-ttu-id="8ae16-143">555,950039</span><span class="sxs-lookup"><span data-stu-id="8ae16-143">555.950039</span></span> | <span data-ttu-id="8ae16-144">410,17</span><span class="sxs-lookup"><span data-stu-id="8ae16-144">410.17</span></span> | <span data-ttu-id="8ae16-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="8ae16-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="8ae16-146">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="8ae16-146">Next steps</span></span>

- [<span data-ttu-id="8ae16-147">Számlázás és adók</span><span class="sxs-lookup"><span data-stu-id="8ae16-147">Billing and taxes</span></span>](billing.md)
