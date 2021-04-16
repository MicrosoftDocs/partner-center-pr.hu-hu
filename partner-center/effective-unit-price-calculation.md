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
ms.openlocfilehash: 6c3c3a672de015c9f38fa0e34232da8d9913177c
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528569"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="45827-104">Az Azure-csomagfelhasználás tényleges egységárának kiszámítása</span><span class="sxs-lookup"><span data-stu-id="45827-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="45827-105">A tényleges egységár</span><span class="sxs-lookup"><span data-stu-id="45827-105">The effective unit price</span></span>

<span data-ttu-id="45827-106">A tényleges egységár számítása a fogyasztásmérő szintjén történik (nem az erőforrás szintjén), és a mérőhasználat alapján naponta lesz módosítva.</span><span class="sxs-lookup"><span data-stu-id="45827-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="45827-107">A tényleges egységárat az alábbi három tényező alapján számítjuk ki:</span><span class="sxs-lookup"><span data-stu-id="45827-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="45827-108">Felhasználás, amelyet naponta figyelnek a számlázási ciklus során</span><span class="sxs-lookup"><span data-stu-id="45827-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="45827-109">A fogyasztásmérő számlázható költsége</span><span class="sxs-lookup"><span data-stu-id="45827-109">Billable cost for the meter</span></span>
- <span data-ttu-id="45827-110">Rétegezés (ha van)</span><span class="sxs-lookup"><span data-stu-id="45827-110">Tiering (if applicable)</span></span>

<span data-ttu-id="45827-111">Mivel a használatot naponta monitorozni fogjuk a számlázási ciklusban, a tényleges egységár ingadozni fog.</span><span class="sxs-lookup"><span data-stu-id="45827-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="45827-112">Egy adott számlázási ciklus végső ára akkor lesz elérhető, ha leállítjuk a használat számítását, és lezárjuk a számlázási időszakot.</span><span class="sxs-lookup"><span data-stu-id="45827-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="45827-113">A használat legnagyobb változását a negyedik vagy ötödik tizedesjegy után fogja látni.</span><span class="sxs-lookup"><span data-stu-id="45827-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="45827-114">Annak kiderítése, hogy a fogyasztásmérő rétegzett díjszabást használ-e</span><span class="sxs-lookup"><span data-stu-id="45827-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="45827-115">Ha nem tudja, hogy a fogyasztásmérő rétegzett díjszabást használ-e, az alábbi eljárással derítse ki.</span><span class="sxs-lookup"><span data-stu-id="45827-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="45827-116">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="45827-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="45827-117">Válassza **az Értékesítés** lehetőséget, válassza a Díjszabás és **ajánlatok** lehetőséget, majd az **Azure-csomag díjszabása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="45827-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="45827-118">Keresse meg a fogyasztásmérőt azonosító alapján, majd töltse le a díjszabási adatokat.</span><span class="sxs-lookup"><span data-stu-id="45827-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="45827-119">Mintaszámítás</span><span class="sxs-lookup"><span data-stu-id="45827-119">Sample calculation</span></span>

<span data-ttu-id="45827-120">Az alábbi táblázat egy példát mutat be arra, hogyan számítjuk ki a tényleges egységárat a nyitott időszakban.</span><span class="sxs-lookup"><span data-stu-id="45827-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="45827-121">A táblázatban a következő értékek érvényesek:</span><span class="sxs-lookup"><span data-stu-id="45827-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="45827-122">**UP** = az erőforrás egységára óránként = 0,868</span><span class="sxs-lookup"><span data-stu-id="45827-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="45827-123">**BCU** = A fogyasztásmérő számlázható fogyasztási egysége</span><span class="sxs-lookup"><span data-stu-id="45827-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="45827-124">**BC** = a fogyasztásmérő számlázható költsége = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="45827-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="45827-125">Ez a 15%-os PEC-kedvezmény kiigazítását tükrözi.</span><span class="sxs-lookup"><span data-stu-id="45827-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="45827-126">Ezután a függvény alsó korlátját használva a tizedesvessző utáni két számjegyre korlátozjuk az értéket a minimális összeg felszámizálása érdekében.</span><span class="sxs-lookup"><span data-stu-id="45827-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="45827-127">**Tényleges egységár** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="45827-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="45827-128">Megjegyzés: A példában a fogyasztásmérő nem rendelkezik tarifacsomagokkal vagy egyéb kedvezményekkel – az Effective Unit Price a kedvezmény százalékos arányait és egyéb kiigazításokat is figyelembe veszi.</span><span class="sxs-lookup"><span data-stu-id="45827-128">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="45827-129">Date</span><span class="sxs-lookup"><span data-stu-id="45827-129">Date</span></span> | <span data-ttu-id="45827-130">BCU (számlázható fogyasztási egység)</span><span class="sxs-lookup"><span data-stu-id="45827-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="45827-131">BC (számlázható költség)</span><span class="sxs-lookup"><span data-stu-id="45827-131">BC (Billable cost)</span></span> | <span data-ttu-id="45827-132">Tényleges egységár</span><span class="sxs-lookup"><span data-stu-id="45827-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="45827-133">3–Aug.</span><span class="sxs-lookup"><span data-stu-id="45827-133">3-Aug</span></span> | <span data-ttu-id="45827-134">29</span><span class="sxs-lookup"><span data-stu-id="45827-134">29</span></span> | <span data-ttu-id="45827-135">21.39</span><span class="sxs-lookup"><span data-stu-id="45827-135">21.39</span></span> | <span data-ttu-id="45827-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="45827-136">0.737586206896552</span></span> |
| <span data-ttu-id="45827-137">10-Aug.</span><span class="sxs-lookup"><span data-stu-id="45827-137">10-Aug</span></span> | <span data-ttu-id="45827-138">210.950039</span><span class="sxs-lookup"><span data-stu-id="45827-138">210.950039</span></span> | <span data-ttu-id="45827-139">155.63</span><span class="sxs-lookup"><span data-stu-id="45827-139">155.63</span></span> | <span data-ttu-id="45827-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="45827-140">0.737757626107858</span></span> |
| <span data-ttu-id="45827-141">25-Aug.</span><span class="sxs-lookup"><span data-stu-id="45827-141">25-Aug</span></span> | <span data-ttu-id="45827-142">555.950039</span><span class="sxs-lookup"><span data-stu-id="45827-142">555.950039</span></span> | <span data-ttu-id="45827-143">410.17</span><span class="sxs-lookup"><span data-stu-id="45827-143">410.17</span></span> | <span data-ttu-id="45827-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="45827-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="45827-145">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="45827-145">Next steps</span></span>

- [<span data-ttu-id="45827-146">Számlázás és adók</span><span class="sxs-lookup"><span data-stu-id="45827-146">Billing and taxes</span></span>](billing.md)
