---
title: Egyeztetési fájlok díjtípusai
ms.topic: article
ms.date: 06/05/2020
description: Fedezze fel a (például licenc-alapú, használati és egyszeri), kreditek és kedvezmények típusát a partner Center egyeztetési fájljaiban.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f1fb7fdcc4ec56f0d5cf0eb26b62294235a5b908
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441596"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="351b8-103">A különböző díjszabási típusok ismertetése a partner Center egyeztetési fájljaiban</span><span class="sxs-lookup"><span data-stu-id="351b8-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="351b8-104">**A következőre érvényes:**</span><span class="sxs-lookup"><span data-stu-id="351b8-104">**Applies to**</span></span>

- <span data-ttu-id="351b8-105">A Microsoft Cloud for US Government Partnerközpontja</span><span class="sxs-lookup"><span data-stu-id="351b8-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="351b8-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="351b8-106">**Appropriate roles**</span></span>

- <span data-ttu-id="351b8-107">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="351b8-107">Admin agent</span></span>
- <span data-ttu-id="351b8-108">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="351b8-108">Billing admin</span></span>
- <span data-ttu-id="351b8-109">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="351b8-109">Global admin</span></span>

<span data-ttu-id="351b8-110">Ez a cikk a számla szakasz és a társított díjszabási típusok közötti leképezéseket ismerteti, amelyek lehetnek a megbékélési fájlban.</span><span class="sxs-lookup"><span data-stu-id="351b8-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="351b8-111">A számla a díjak összegzését tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="351b8-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="351b8-112">Az egyeztetési fájl részletesen részletezi a line-Item tranzakciókat, beleértve a díjszabási típusokat is.</span><span class="sxs-lookup"><span data-stu-id="351b8-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="351b8-113">Az egyeztetési fájlokkal kapcsolatos további információkért lásd: [a megbékélési fájlok használata](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="351b8-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="351b8-114">A [használaton alapuló egyeztetési fájlok](usage-based-recon-files.md) és a [licenc-alapú egyeztetési fájlok](license-based-recon-files.md) csak a használattal kapcsolatos tranzakciókat és díjakat (a felhasznált egységek és a kapcsolódó díjak) mutatják.</span><span class="sxs-lookup"><span data-stu-id="351b8-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="351b8-115">A számlán megjelenő egyszeri kreditek, kedvezmények vagy visszatérítések nem jelennek meg az egyeztetési fájlban. </span><span class="sxs-lookup"><span data-stu-id="351b8-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="351b8-116">Vegyesköltség-típusok hozzárendelése a számlázáshoz</span><span class="sxs-lookup"><span data-stu-id="351b8-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="351b8-117">A számla és a megbékélési fájl közötti Összevetéshez használja a Microsoft Excelben a szűrési lehetőségeket.</span><span class="sxs-lookup"><span data-stu-id="351b8-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="351b8-118">Az egyeztetési fájlban lévő vegyesköltség-típusok alapján szűkítse a számla díját a visszaegyeztetési fájlban lévő vegyesköltség-részletezési csoportba.</span><span class="sxs-lookup"><span data-stu-id="351b8-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="351b8-119">Licenc-alapú díjak</span><span class="sxs-lookup"><span data-stu-id="351b8-119">License-based charges</span></span>

<span data-ttu-id="351b8-120">Ha ezeket a licencfeltételeket szeretné feltérképezni a számlán, a licenc-alapú fájl **összeg** oszlopát adja meg.</span><span class="sxs-lookup"><span data-stu-id="351b8-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="351b8-121">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="351b8-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="351b8-122">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="351b8-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="351b8-123">Aktiválási díj</span><span class="sxs-lookup"><span data-stu-id="351b8-123">Activation fee</span></span> | <span data-ttu-id="351b8-124">Az ügyfélnek a vásárlás után az előfizetés használatakor felszámított összeg.</span><span class="sxs-lookup"><span data-stu-id="351b8-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="351b8-125">Megszakított díj</span><span class="sxs-lookup"><span data-stu-id="351b8-125">Cancel fee</span></span> | <span data-ttu-id="351b8-126">A hozzárendelt licencek megváltozásakor a rendszer visszafizeti az előfizetést az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="351b8-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="351b8-127">Példány-arány megszakítása</span><span class="sxs-lookup"><span data-stu-id="351b8-127">Cancel instance prorate</span></span> | <span data-ttu-id="351b8-128">Az elszámolási díjak megszakadtak, ha a havi előfizetéssel rendelkező ügyfél felfüggesztette az előfizetést, és a társított licencek egy hónapon belül változnak</span><span class="sxs-lookup"><span data-stu-id="351b8-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="351b8-129">Ciklus díja</span><span class="sxs-lookup"><span data-stu-id="351b8-129">Cycle fee</span></span> | <span data-ttu-id="351b8-130">Egy előfizetés rendszeres díjai.</span><span class="sxs-lookup"><span data-stu-id="351b8-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="351b8-131">Ciklus példányának gyakorisága</span><span class="sxs-lookup"><span data-stu-id="351b8-131">Cycle instance prorate</span></span> | <span data-ttu-id="351b8-132">Az ügyfél által a társított licencek megváltozásakor kiértékelt arányban elszámolt díjak.</span><span class="sxs-lookup"><span data-stu-id="351b8-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="351b8-133">A megszakítás díja</span><span class="sxs-lookup"><span data-stu-id="351b8-133">Prorate fees when cancel</span></span> | <span data-ttu-id="351b8-134">A szolgáltatás fel nem használt részének elszámolási aránya a lemondás után.</span><span class="sxs-lookup"><span data-stu-id="351b8-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="351b8-135">Az aktuális ajánlatból való áttéréskor felmerülő díjak</span><span class="sxs-lookup"><span data-stu-id="351b8-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="351b8-136">Arányos díjak az aktuális havi előfizetésből egy éves előfizetésre való áttérés után.</span><span class="sxs-lookup"><span data-stu-id="351b8-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="351b8-137">Az új ajánlatra való áttéréskor felmerülő díjak</span><span class="sxs-lookup"><span data-stu-id="351b8-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="351b8-138">A havi előfizetés új éves előfizetésre való konvertálása után eltelt díjak.</span><span class="sxs-lookup"><span data-stu-id="351b8-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="351b8-139">Díjszabási díjak a vásárláskor</span><span class="sxs-lookup"><span data-stu-id="351b8-139">Prorate fees when purchase</span></span> | <span data-ttu-id="351b8-140">Az előfizetés díja, ha havi vagy éves számlázást is használ.</span><span class="sxs-lookup"><span data-stu-id="351b8-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="351b8-141">A megújítás díjszabása</span><span class="sxs-lookup"><span data-stu-id="351b8-141">Prorate fee when renew</span></span> | <span data-ttu-id="351b8-142">Az Előfizetés megújítása után elszámolt díjak.</span><span class="sxs-lookup"><span data-stu-id="351b8-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="351b8-143">Megújítás díja</span><span class="sxs-lookup"><span data-stu-id="351b8-143">Renew fee</span></span> | <span data-ttu-id="351b8-144">Előfizetés megújításának díja</span><span class="sxs-lookup"><span data-stu-id="351b8-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="351b8-145">Díjszabási díjak aktiváláskor</span><span class="sxs-lookup"><span data-stu-id="351b8-145">Prorate fees when activate</span></span> | <span data-ttu-id="351b8-146">Elszámolási díjak az aktiválástól egészen a számlázási időszak végéig.</span><span class="sxs-lookup"><span data-stu-id="351b8-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="351b8-147">Egyszeri díj</span><span class="sxs-lookup"><span data-stu-id="351b8-147">One-time charges</span></span>

<span data-ttu-id="351b8-148">Ha ezeket az egyszeri díjakat szeretné leképezni a számlára, akkor a licenc-alapú fájl **összeg** oszlopát adja meg.</span><span class="sxs-lookup"><span data-stu-id="351b8-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="351b8-149">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="351b8-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="351b8-150">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="351b8-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="351b8-151">Új</span><span class="sxs-lookup"><span data-stu-id="351b8-151">New</span></span> | <span data-ttu-id="351b8-152">Új vásárlás létrehozásakor használatos.</span><span class="sxs-lookup"><span data-stu-id="351b8-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="351b8-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="351b8-153">addQuantity</span></span> | <span data-ttu-id="351b8-154">Az eredeti vásárlás és az új mennyiség visszatérítése után is használatos.</span><span class="sxs-lookup"><span data-stu-id="351b8-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="351b8-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="351b8-155">removeQuantity</span></span> | <span data-ttu-id="351b8-156">Az eredeti vásárlás visszatérítésében és az új mennyiség csökkenése után is használatos.</span><span class="sxs-lookup"><span data-stu-id="351b8-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="351b8-157">Mégse</span><span class="sxs-lookup"><span data-stu-id="351b8-157">Cancel</span></span> | <span data-ttu-id="351b8-158">Előfizetés megszakadása esetén használatos.</span><span class="sxs-lookup"><span data-stu-id="351b8-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="351b8-159">Konvertálás</span><span class="sxs-lookup"><span data-stu-id="351b8-159">Convert</span></span> | <span data-ttu-id="351b8-160">A licenc frissítésekor használatos, de a licencek száma változatlan marad.</span><span class="sxs-lookup"><span data-stu-id="351b8-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="351b8-161">Használati díjak</span><span class="sxs-lookup"><span data-stu-id="351b8-161">Usage charges</span></span>

<span data-ttu-id="351b8-162">A használati díjaknak a számlára való hozzárendeléséhez a **PretaxCharges** oszlopot a használaton alapuló fájlból kell összegezni.</span><span class="sxs-lookup"><span data-stu-id="351b8-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="351b8-163">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="351b8-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="351b8-164">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="351b8-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="351b8-165">Használati díj kiértékelése megszakításkor</span><span class="sxs-lookup"><span data-stu-id="351b8-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="351b8-166">Az aktuális számlázási időszakban a nem fizetett használat megszüntetésére vonatkozó hozzáférési díj.</span><span class="sxs-lookup"><span data-stu-id="351b8-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="351b8-167">A jelenlegi ciklus használati díjának felmérése</span><span class="sxs-lookup"><span data-stu-id="351b8-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="351b8-168">Az aktuális számlázási időszakhoz való hozzáférés használati díja.</span><span class="sxs-lookup"><span data-stu-id="351b8-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="351b8-169">Kreditek</span><span class="sxs-lookup"><span data-stu-id="351b8-169">Credits</span></span>

<span data-ttu-id="351b8-170">A kreditek hozzárendelése a számlához:</span><span class="sxs-lookup"><span data-stu-id="351b8-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="351b8-171">Adja meg a **TotalForCustomer** a licenc-alapú fájlból.</span><span class="sxs-lookup"><span data-stu-id="351b8-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="351b8-172">A **PostTaxTotal** oszlop összege a használaton alapuló fájlból.</span><span class="sxs-lookup"><span data-stu-id="351b8-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="351b8-173">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="351b8-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="351b8-174">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="351b8-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="351b8-175">Egy tétel eltolása</span><span class="sxs-lookup"><span data-stu-id="351b8-175">Offset a line item</span></span> | <span data-ttu-id="351b8-176">Részleges vagy teljes visszatérítés egy sorra, beleértve az adókat is.</span><span class="sxs-lookup"><span data-stu-id="351b8-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="351b8-177">Használati alapú kedvezmények</span><span class="sxs-lookup"><span data-stu-id="351b8-177">Usage-based discounts</span></span>

<span data-ttu-id="351b8-178">A használati alapú kedvezmények a számlára való hozzárendeléséhez a **PretaxCharges** oszlopot a használaton alapuló fájlból kell összegezni.</span><span class="sxs-lookup"><span data-stu-id="351b8-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="351b8-179">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="351b8-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="351b8-180">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="351b8-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="351b8-181">Aktiválási kedvezmény</span><span class="sxs-lookup"><span data-stu-id="351b8-181">Activation discount</span></span> | <span data-ttu-id="351b8-182">Az előfizetés aktiválása esetén érvényes kedvezmény.</span><span class="sxs-lookup"><span data-stu-id="351b8-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="351b8-183">Ciklus kedvezménye</span><span class="sxs-lookup"><span data-stu-id="351b8-183">Cycle discount</span></span> | <span data-ttu-id="351b8-184">Az időszakos költségekre alkalmazott kedvezmény.</span><span class="sxs-lookup"><span data-stu-id="351b8-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="351b8-185">Kedvezmény megújítása</span><span class="sxs-lookup"><span data-stu-id="351b8-185">Renew discount</span></span> | <span data-ttu-id="351b8-186">Az előfizetés megújításakor alkalmazott kedvezmény.</span><span class="sxs-lookup"><span data-stu-id="351b8-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="351b8-187">Kedvezmény lemondása</span><span class="sxs-lookup"><span data-stu-id="351b8-187">Cancel discount</span></span> | <span data-ttu-id="351b8-188">A kedvezmények megszakításakor alkalmazott díjak.</span><span class="sxs-lookup"><span data-stu-id="351b8-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="351b8-189">Licenc-alapú kedvezmények</span><span class="sxs-lookup"><span data-stu-id="351b8-189">License-based discounts</span></span>

<span data-ttu-id="351b8-190">A licenc-alapú kedvezmények a számlára való leképezéséhez adja a **TotalOtherDiscount** oszlopot a licenc-alapú fájlból.</span><span class="sxs-lookup"><span data-stu-id="351b8-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="351b8-191">*A licenc-alapú kedvezmények több feltöltési típusra is alkalmazhatók.*</span><span class="sxs-lookup"><span data-stu-id="351b8-191">*License-based discounts may be applied to multiple charge types.*</span></span>
