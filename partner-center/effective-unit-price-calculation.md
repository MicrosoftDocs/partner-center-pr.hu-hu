---
title: Tényleges egységár kiszámítása
ms.topic: how-to
ms.date: 04/02/2021
description: Megismeri a tényleges egységárat és számítását. Ez a cikk egy mintaszámítást is tartalmaz.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172217"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="9a4ee-104">Az Azure-csomagfelhasználás tényleges egységárának kiszámítása</span><span class="sxs-lookup"><span data-stu-id="9a4ee-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="9a4ee-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="9a4ee-105">**Appropriate roles**</span></span>

- <span data-ttu-id="9a4ee-106">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="9a4ee-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="9a4ee-107">A tényleges egységár</span><span class="sxs-lookup"><span data-stu-id="9a4ee-107">The effective unit price</span></span>

<span data-ttu-id="9a4ee-108">A tényleges egységár számítása a fogyasztásmérő szintjén történik (nem az erőforrás szintjén), és a mérőhasználat alapján naponta lesz módosítva.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="9a4ee-109">A tényleges egységárat az alábbi három tényező alapján számítjuk ki:</span><span class="sxs-lookup"><span data-stu-id="9a4ee-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="9a4ee-110">Felhasználás, amelyet naponta figyelnek a számlázási ciklus során</span><span class="sxs-lookup"><span data-stu-id="9a4ee-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="9a4ee-111">A fogyasztásmérő számlázható költsége</span><span class="sxs-lookup"><span data-stu-id="9a4ee-111">Billable cost for the meter</span></span>
- <span data-ttu-id="9a4ee-112">Rétegezés (ha van)</span><span class="sxs-lookup"><span data-stu-id="9a4ee-112">Tiering (if applicable)</span></span>

<span data-ttu-id="9a4ee-113">Mivel a használatot naponta monitorozni fogjuk a számlázási ciklusban, a tényleges egységár ingadozni fog.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="9a4ee-114">Az adott számlázási ciklus végső ára a használat kiszámításának leállítása és a számlázási időszak bezárása után lesz elérhető.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="9a4ee-115">A használat legtöbb változását a negyedik vagy ötödik tizedesjegy után fogja látni.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="9a4ee-116">Annak kiderítése, hogy a fogyasztásmérő rétegzett díjszabást használ-e</span><span class="sxs-lookup"><span data-stu-id="9a4ee-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="9a4ee-117">Ha nem tudja, hogy a fogyasztásmérő rétegzett díjszabást használ-e, az alábbi eljárással derítse ki.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="9a4ee-118">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="9a4ee-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="9a4ee-119">Válassza **az Értékesítés** lehetőséget, válassza a Díjszabás és **ajánlatok** lehetőséget, majd az **Azure-csomag díjszabása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="9a4ee-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="9a4ee-120">Keresse meg a fogyasztásmérőt azonosító alapján, majd töltse le a díjszabási adatokat.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="9a4ee-121">Mintaszámítás</span><span class="sxs-lookup"><span data-stu-id="9a4ee-121">Sample calculation</span></span>

<span data-ttu-id="9a4ee-122">Az alábbi táblázat egy példát mutat be arra, hogyan számítjuk ki a tényleges egységárat a nyitott időszakban.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="9a4ee-123">A táblázatban a következő értékek érvényesek:</span><span class="sxs-lookup"><span data-stu-id="9a4ee-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="9a4ee-124">**UP** = az erőforrás óránkénti egységára = 0,868</span><span class="sxs-lookup"><span data-stu-id="9a4ee-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="9a4ee-125">**BCU** = A fogyasztásmérő számlázható fogyasztási egysége</span><span class="sxs-lookup"><span data-stu-id="9a4ee-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="9a4ee-126">**BC** = a fogyasztásmérő számlázható költsége = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="9a4ee-127">Ez a 15%-os PEC-kedvezmény kiigazítását tükrözi.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="9a4ee-128">Ezután a függvény alsó korlátját használva a tizedesvessző utáni két számjegyre korlátozjuk az értéket a minimális összeg felszámizálása érdekében.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="9a4ee-129">**Tényleges egységár** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="9a4ee-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="9a4ee-130">Megjegyzés: Az ebben a példában található fogyasztásmérő nem rendelkezik tarifacsomagokkal vagy egyéb kedvezményekkel – a tényleges egységár a kedvezmény százalékos arányait és egyéb módosításokat is figyelembe veszi.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="9a4ee-131">Date</span><span class="sxs-lookup"><span data-stu-id="9a4ee-131">Date</span></span> | <span data-ttu-id="9a4ee-132">BCU (számlázható fogyasztási egység)</span><span class="sxs-lookup"><span data-stu-id="9a4ee-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="9a4ee-133">BC (számlázható költség)</span><span class="sxs-lookup"><span data-stu-id="9a4ee-133">BC (Billable cost)</span></span> | <span data-ttu-id="9a4ee-134">Tényleges egységár</span><span class="sxs-lookup"><span data-stu-id="9a4ee-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="9a4ee-135">3–Aug.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-135">3-Aug</span></span> | <span data-ttu-id="9a4ee-136">29</span><span class="sxs-lookup"><span data-stu-id="9a4ee-136">29</span></span> | <span data-ttu-id="9a4ee-137">21.39</span><span class="sxs-lookup"><span data-stu-id="9a4ee-137">21.39</span></span> | <span data-ttu-id="9a4ee-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="9a4ee-138">0.737586206896552</span></span> |
| <span data-ttu-id="9a4ee-139">10-Aug.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-139">10-Aug</span></span> | <span data-ttu-id="9a4ee-140">210.950039</span><span class="sxs-lookup"><span data-stu-id="9a4ee-140">210.950039</span></span> | <span data-ttu-id="9a4ee-141">155.63</span><span class="sxs-lookup"><span data-stu-id="9a4ee-141">155.63</span></span> | <span data-ttu-id="9a4ee-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="9a4ee-142">0.737757626107858</span></span> |
| <span data-ttu-id="9a4ee-143">25-Aug.</span><span class="sxs-lookup"><span data-stu-id="9a4ee-143">25-Aug</span></span> | <span data-ttu-id="9a4ee-144">555.950039</span><span class="sxs-lookup"><span data-stu-id="9a4ee-144">555.950039</span></span> | <span data-ttu-id="9a4ee-145">410.17</span><span class="sxs-lookup"><span data-stu-id="9a4ee-145">410.17</span></span> | <span data-ttu-id="9a4ee-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="9a4ee-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="9a4ee-147">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="9a4ee-147">Next steps</span></span>

- [<span data-ttu-id="9a4ee-148">Számlázás és adók</span><span class="sxs-lookup"><span data-stu-id="9a4ee-148">Billing and taxes</span></span>](billing.md)
