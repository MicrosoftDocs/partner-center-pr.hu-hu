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
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147122"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="5c9a3-104">Az Azure-csomag tényleges egységárának kiszámítása</span><span class="sxs-lookup"><span data-stu-id="5c9a3-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="5c9a3-105">**Megfelelő szerepkörök:** Számlázási rendszergazda</span><span class="sxs-lookup"><span data-stu-id="5c9a3-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="5c9a3-106">A tényleges egységár</span><span class="sxs-lookup"><span data-stu-id="5c9a3-106">The effective unit price</span></span>

<span data-ttu-id="5c9a3-107">A tényleges egységár kiszámítása a fogyasztásmérő szintjén történik (nem az erőforrás szintjén), és naponta lesz módosítva a fogyasztásmérő használata alapján.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="5c9a3-108">A tényleges egységárat az alábbi három tényező alapján számítjuk ki:</span><span class="sxs-lookup"><span data-stu-id="5c9a3-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="5c9a3-109">A számlázási ciklusban naponta monitorozás alatt áll felhasználás</span><span class="sxs-lookup"><span data-stu-id="5c9a3-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="5c9a3-110">A fogyasztásmérő számlázható költsége</span><span class="sxs-lookup"><span data-stu-id="5c9a3-110">Billable cost for the meter</span></span>
- <span data-ttu-id="5c9a3-111">Rétegezés (ha van)</span><span class="sxs-lookup"><span data-stu-id="5c9a3-111">Tiering (if applicable)</span></span>

<span data-ttu-id="5c9a3-112">Mivel a használatot naponta monitorozni fogjuk a számlázási ciklus során, a tényleges egységár ingadozni fog.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="5c9a3-113">Az adott számlázási ciklus végső ára a használat kiszámításának leállítása és a számlázási időszak bezárása után lesz elérhető.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="5c9a3-114">A használat legtöbb változását a negyedik vagy ötödik tizedesjegy után fogja látni.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="5c9a3-115">Annak kiderítése, hogy a fogyasztásmérő rétegzett díjszabást használ-e</span><span class="sxs-lookup"><span data-stu-id="5c9a3-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="5c9a3-116">Ha nem tudja, hogy a fogyasztásmérő rétegzett díjszabást használ-e, az alábbi eljárással derítse ki.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="5c9a3-117">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="5c9a3-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="5c9a3-118">Válassza **az Értékesítés** lehetőséget, válassza a Díjszabás és **ajánlatok** lehetőséget, majd válassza az **Azure-csomag díjszabása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="5c9a3-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="5c9a3-119">Keresse meg a fogyasztásmérőt azonosító alapján, majd töltse le a díjszabási adatokat.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="5c9a3-120">Mintaszámítás</span><span class="sxs-lookup"><span data-stu-id="5c9a3-120">Sample calculation</span></span>

<span data-ttu-id="5c9a3-121">Az alábbi táblázat egy példát mutat be arra, hogyan számítjuk ki a tényleges egységárat a nyitott időszakban.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="5c9a3-122">A táblázatban a következő értékek érvényesek:</span><span class="sxs-lookup"><span data-stu-id="5c9a3-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="5c9a3-123">**UP** = az erőforrás óránkénti egységára = 0,868</span><span class="sxs-lookup"><span data-stu-id="5c9a3-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="5c9a3-124">**BCU** = A fogyasztásmérő számlázható fogyasztási egysége</span><span class="sxs-lookup"><span data-stu-id="5c9a3-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="5c9a3-125">**BC** = a fogyasztásmérő számlázható költsége = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="5c9a3-126">Ez a 15%-os PEC-kedvezmény kiigazítását tükrözi.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="5c9a3-127">Ezután a függvény alsó korlátját használva a tizedesvessző utáni két számjegyre korlátozjuk az értéket a minimális összeg felszámizálása érdekében.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="5c9a3-128">**Tényleges egységár** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="5c9a3-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="5c9a3-129">Megjegyzés: Az ebben a példában található fogyasztásmérő nem rendelkezik tarifacsomagokkal vagy egyéb kedvezményekkel – a tényleges egységár a kedvezmény százalékos arányait és egyéb módosításokat is figyelembe veszi.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="5c9a3-130">Date</span><span class="sxs-lookup"><span data-stu-id="5c9a3-130">Date</span></span> | <span data-ttu-id="5c9a3-131">BCU (számlázható fogyasztási egység)</span><span class="sxs-lookup"><span data-stu-id="5c9a3-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="5c9a3-132">BC (számlázható költség)</span><span class="sxs-lookup"><span data-stu-id="5c9a3-132">BC (Billable cost)</span></span> | <span data-ttu-id="5c9a3-133">Tényleges egységár</span><span class="sxs-lookup"><span data-stu-id="5c9a3-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="5c9a3-134">3–Aug.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-134">3-Aug</span></span> | <span data-ttu-id="5c9a3-135">29</span><span class="sxs-lookup"><span data-stu-id="5c9a3-135">29</span></span> | <span data-ttu-id="5c9a3-136">21.39</span><span class="sxs-lookup"><span data-stu-id="5c9a3-136">21.39</span></span> | <span data-ttu-id="5c9a3-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="5c9a3-137">0.737586206896552</span></span> |
| <span data-ttu-id="5c9a3-138">10-Aug.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-138">10-Aug</span></span> | <span data-ttu-id="5c9a3-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="5c9a3-139">210.950039</span></span> | <span data-ttu-id="5c9a3-140">155.63</span><span class="sxs-lookup"><span data-stu-id="5c9a3-140">155.63</span></span> | <span data-ttu-id="5c9a3-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="5c9a3-141">0.737757626107858</span></span> |
| <span data-ttu-id="5c9a3-142">25-Aug.</span><span class="sxs-lookup"><span data-stu-id="5c9a3-142">25-Aug</span></span> | <span data-ttu-id="5c9a3-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="5c9a3-143">555.950039</span></span> | <span data-ttu-id="5c9a3-144">410.17</span><span class="sxs-lookup"><span data-stu-id="5c9a3-144">410.17</span></span> | <span data-ttu-id="5c9a3-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="5c9a3-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="5c9a3-146">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="5c9a3-146">Next steps</span></span>

- [<span data-ttu-id="5c9a3-147">Számlázás és adók</span><span class="sxs-lookup"><span data-stu-id="5c9a3-147">Billing and taxes</span></span>](billing.md)
