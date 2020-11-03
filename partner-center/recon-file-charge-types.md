---
title: Egyeztetési felszámított fájlok típusai
ms.topic: article
ms.date: 06/05/2020
description: Fedezze fel a (például licenc-alapú, használati és egyszeri), kreditek és kedvezmények típusát a partner Center egyeztetési fájljaiban.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/31/2020
ms.locfileid: "92528061"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="b5290-103">A különböző díjszabási típusok ismertetése a partner Center egyeztetési fájljaiban</span><span class="sxs-lookup"><span data-stu-id="b5290-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="b5290-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="b5290-104">**Applies to**</span></span>

- <span data-ttu-id="b5290-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="b5290-105">Partner Center</span></span>
- <span data-ttu-id="b5290-106">Az USA kormányzati szerveinek Microsoft Cloud a partneri központ</span><span class="sxs-lookup"><span data-stu-id="b5290-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="b5290-107">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="b5290-107">**Appropriate roles**</span></span>

- <span data-ttu-id="b5290-108">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="b5290-108">Admin agent</span></span>
- <span data-ttu-id="b5290-109">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="b5290-109">Billing admin</span></span>
- <span data-ttu-id="b5290-110">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="b5290-110">Global admin</span></span>

<span data-ttu-id="b5290-111">Ez a témakör a számla szakasz és a társított díjszabási típusok közötti leképezéseket ismerteti, amelyek lehetnek a megbékélési fájlban.</span><span class="sxs-lookup"><span data-stu-id="b5290-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="b5290-112">A számla a díjak összegzését tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="b5290-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="b5290-113">Az egyeztetési fájl részletesen részletezi a line-Item tranzakciókat, beleértve a díjszabási típusokat is.</span><span class="sxs-lookup"><span data-stu-id="b5290-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="b5290-114">Az egyeztetési fájlokkal kapcsolatos további információkért lásd: [a megbékélési fájlok használata](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="b5290-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="b5290-115">A [használaton alapuló egyeztetési fájlok](usage-based-recon-files.md) és a [licenc-alapú egyeztetési fájlok](license-based-recon-files.md) csak a használattal kapcsolatos tranzakciókat és díjakat (a felhasznált egységek és a kapcsolódó díjak) mutatják.</span><span class="sxs-lookup"><span data-stu-id="b5290-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="b5290-116">A számlán megjelenő egyszeri kreditek, kedvezmények vagy visszatérítések nem jelennek meg az egyeztetési fájlban. **Adjustments**</span><span class="sxs-lookup"><span data-stu-id="b5290-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="b5290-117">Vegyesköltség-típusok hozzárendelése a számlázáshoz</span><span class="sxs-lookup"><span data-stu-id="b5290-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="b5290-118">A számla és a megbékélési fájl közötti Összevetéshez használja a Microsoft Excelben a szűrési lehetőségeket.</span><span class="sxs-lookup"><span data-stu-id="b5290-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="b5290-119">Az egyeztetési fájlban lévő vegyesköltség-típusok alapján szűkítse a számla díját a visszaegyeztetési fájlban lévő vegyesköltség-részletezési csoportba.</span><span class="sxs-lookup"><span data-stu-id="b5290-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="b5290-120">Licenc-alapú díjak</span><span class="sxs-lookup"><span data-stu-id="b5290-120">License-based charges</span></span>

<span data-ttu-id="b5290-121">Ha ezeket a licencfeltételeket szeretné feltérképezni a számlán, a licenc-alapú fájl **összeg** oszlopát adja meg.</span><span class="sxs-lookup"><span data-stu-id="b5290-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="b5290-122">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="b5290-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b5290-123">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="b5290-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b5290-124">Aktiválási díj</span><span class="sxs-lookup"><span data-stu-id="b5290-124">Activation fee</span></span> | <span data-ttu-id="b5290-125">Az ügyfélnek a vásárlás után az előfizetés használatakor felszámított összeg.</span><span class="sxs-lookup"><span data-stu-id="b5290-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="b5290-126">Megszakított díj</span><span class="sxs-lookup"><span data-stu-id="b5290-126">Cancel fee</span></span> | <span data-ttu-id="b5290-127">A hozzárendelt licencek megváltozásakor a rendszer visszafizeti az előfizetést az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="b5290-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="b5290-128">Példány-arány megszakítása</span><span class="sxs-lookup"><span data-stu-id="b5290-128">Cancel instance prorate</span></span> | <span data-ttu-id="b5290-129">Az elszámolási díjak megszakadtak, ha a havi előfizetéssel rendelkező ügyfél felfüggesztette az előfizetést, és a társított licencek egy hónapon belül változnak</span><span class="sxs-lookup"><span data-stu-id="b5290-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="b5290-130">Ciklus díja</span><span class="sxs-lookup"><span data-stu-id="b5290-130">Cycle fee</span></span> | <span data-ttu-id="b5290-131">Egy előfizetés rendszeres díjai.</span><span class="sxs-lookup"><span data-stu-id="b5290-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="b5290-132">Ciklus példányának gyakorisága</span><span class="sxs-lookup"><span data-stu-id="b5290-132">Cycle instance prorate</span></span> | <span data-ttu-id="b5290-133">Az ügyfél által a társított licencek megváltozásakor kiértékelt arányban elszámolt díjak.</span><span class="sxs-lookup"><span data-stu-id="b5290-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="b5290-134">A megszakítás díja</span><span class="sxs-lookup"><span data-stu-id="b5290-134">Prorate fees when cancel</span></span> | <span data-ttu-id="b5290-135">A szolgáltatás fel nem használt részének elszámolási aránya a lemondás után.</span><span class="sxs-lookup"><span data-stu-id="b5290-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="b5290-136">Az aktuális ajánlatból való áttéréskor felmerülő díjak</span><span class="sxs-lookup"><span data-stu-id="b5290-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="b5290-137">Arányos díjak az aktuális havi előfizetésből egy éves előfizetésre való áttérés után.</span><span class="sxs-lookup"><span data-stu-id="b5290-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="b5290-138">Az új ajánlatra való áttéréskor felmerülő díjak</span><span class="sxs-lookup"><span data-stu-id="b5290-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="b5290-139">A havi előfizetés új éves előfizetésre való konvertálása után eltelt díjak.</span><span class="sxs-lookup"><span data-stu-id="b5290-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="b5290-140">Díjszabási díjak a vásárláskor</span><span class="sxs-lookup"><span data-stu-id="b5290-140">Prorate fees when purchase</span></span> | <span data-ttu-id="b5290-141">Az előfizetés díja, ha havi vagy éves számlázást is használ.</span><span class="sxs-lookup"><span data-stu-id="b5290-141">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="b5290-142">A megújítás díjszabása</span><span class="sxs-lookup"><span data-stu-id="b5290-142">Prorate fee when renew</span></span> | <span data-ttu-id="b5290-143">Az Előfizetés megújítása után elszámolt díjak.</span><span class="sxs-lookup"><span data-stu-id="b5290-143">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="b5290-144">Megújítás díja</span><span class="sxs-lookup"><span data-stu-id="b5290-144">Renew fee</span></span> | <span data-ttu-id="b5290-145">Előfizetés megújításának díja</span><span class="sxs-lookup"><span data-stu-id="b5290-145">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="b5290-146">Díjszabási díjak aktiváláskor</span><span class="sxs-lookup"><span data-stu-id="b5290-146">Prorate fees when activate</span></span> | <span data-ttu-id="b5290-147">Elszámolási díjak az aktiválástól egészen a számlázási időszak végéig.</span><span class="sxs-lookup"><span data-stu-id="b5290-147">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="b5290-148">Egyszeri díj</span><span class="sxs-lookup"><span data-stu-id="b5290-148">One-time charges</span></span>

<span data-ttu-id="b5290-149">Ha ezeket az egyszeri díjakat szeretné leképezni a számlára, akkor a licenc-alapú fájl **összeg** oszlopát adja meg.</span><span class="sxs-lookup"><span data-stu-id="b5290-149">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="b5290-150">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="b5290-150">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b5290-151">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="b5290-151">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b5290-152">Új</span><span class="sxs-lookup"><span data-stu-id="b5290-152">New</span></span> | <span data-ttu-id="b5290-153">Új vásárlás létrehozásakor használatos.</span><span class="sxs-lookup"><span data-stu-id="b5290-153">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="b5290-154">addQuantity</span><span class="sxs-lookup"><span data-stu-id="b5290-154">addQuantity</span></span> | <span data-ttu-id="b5290-155">Az eredeti vásárlás és az új mennyiség visszatérítése után is használatos.</span><span class="sxs-lookup"><span data-stu-id="b5290-155">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="b5290-156">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="b5290-156">removeQuantity</span></span> | <span data-ttu-id="b5290-157">Az eredeti vásárlás visszatérítésében és az új mennyiség csökkenése után is használatos.</span><span class="sxs-lookup"><span data-stu-id="b5290-157">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="b5290-158">Mégse</span><span class="sxs-lookup"><span data-stu-id="b5290-158">Cancel</span></span> | <span data-ttu-id="b5290-159">Előfizetés megszakadása esetén használatos.</span><span class="sxs-lookup"><span data-stu-id="b5290-159">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="b5290-160">Konvertálás</span><span class="sxs-lookup"><span data-stu-id="b5290-160">Convert</span></span> | <span data-ttu-id="b5290-161">A licenc frissítésekor használatos, de a licencek száma változatlan marad.</span><span class="sxs-lookup"><span data-stu-id="b5290-161">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="b5290-162">Használati díjak</span><span class="sxs-lookup"><span data-stu-id="b5290-162">Usage charges</span></span>

<span data-ttu-id="b5290-163">A használati díjaknak a számlára való hozzárendeléséhez a **PretaxCharges** oszlopot a használaton alapuló fájlból kell összegezni.</span><span class="sxs-lookup"><span data-stu-id="b5290-163">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="b5290-164">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="b5290-164">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b5290-165">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="b5290-165">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b5290-166">Használati díj kiértékelése megszakításkor</span><span class="sxs-lookup"><span data-stu-id="b5290-166">Assess usage fee when cancel</span></span> | <span data-ttu-id="b5290-167">Az aktuális számlázási időszakban a nem fizetett használat megszüntetésére vonatkozó hozzáférési díj.</span><span class="sxs-lookup"><span data-stu-id="b5290-167">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="b5290-168">A jelenlegi ciklus használati díjának felmérése</span><span class="sxs-lookup"><span data-stu-id="b5290-168">Assess usage fee for current cycle</span></span> | <span data-ttu-id="b5290-169">Az aktuális számlázási időszakhoz való hozzáférés használati díja.</span><span class="sxs-lookup"><span data-stu-id="b5290-169">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="b5290-170">Kreditek</span><span class="sxs-lookup"><span data-stu-id="b5290-170">Credits</span></span>

<span data-ttu-id="b5290-171">A kreditek hozzárendelése a számlához:</span><span class="sxs-lookup"><span data-stu-id="b5290-171">To map these credits to your invoice:</span></span>

- <span data-ttu-id="b5290-172">Adja meg a **TotalForCustomer** a licenc-alapú fájlból.</span><span class="sxs-lookup"><span data-stu-id="b5290-172">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="b5290-173">A **PostTaxTotal** oszlop összege a használaton alapuló fájlból.</span><span class="sxs-lookup"><span data-stu-id="b5290-173">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="b5290-174">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="b5290-174">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b5290-175">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="b5290-175">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b5290-176">Egy tétel eltolása</span><span class="sxs-lookup"><span data-stu-id="b5290-176">Offset a line item</span></span> | <span data-ttu-id="b5290-177">Részleges vagy teljes visszatérítés egy sorra, beleértve az adókat is.</span><span class="sxs-lookup"><span data-stu-id="b5290-177">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="b5290-178">Használati alapú kedvezmények</span><span class="sxs-lookup"><span data-stu-id="b5290-178">Usage-based discounts</span></span>

<span data-ttu-id="b5290-179">A használati alapú kedvezmények a számlára való hozzárendeléséhez a **PretaxCharges** oszlopot a használaton alapuló fájlból kell összegezni.</span><span class="sxs-lookup"><span data-stu-id="b5290-179">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="b5290-180">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="b5290-180">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b5290-181">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="b5290-181">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b5290-182">Aktiválási kedvezmény</span><span class="sxs-lookup"><span data-stu-id="b5290-182">Activation discount</span></span> | <span data-ttu-id="b5290-183">Az előfizetés aktiválása esetén érvényes kedvezmény.</span><span class="sxs-lookup"><span data-stu-id="b5290-183">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="b5290-184">Ciklus kedvezménye</span><span class="sxs-lookup"><span data-stu-id="b5290-184">Cycle discount</span></span> | <span data-ttu-id="b5290-185">Az időszakos költségekre alkalmazott kedvezmény.</span><span class="sxs-lookup"><span data-stu-id="b5290-185">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="b5290-186">Kedvezmény megújítása</span><span class="sxs-lookup"><span data-stu-id="b5290-186">Renew discount</span></span> | <span data-ttu-id="b5290-187">Az előfizetés megújításakor alkalmazott kedvezmény.</span><span class="sxs-lookup"><span data-stu-id="b5290-187">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="b5290-188">Kedvezmény lemondása</span><span class="sxs-lookup"><span data-stu-id="b5290-188">Cancel discount</span></span> | <span data-ttu-id="b5290-189">A kedvezmények megszakításakor alkalmazott díjak.</span><span class="sxs-lookup"><span data-stu-id="b5290-189">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="b5290-190">Licenc-alapú kedvezmények</span><span class="sxs-lookup"><span data-stu-id="b5290-190">License-based discounts</span></span>

<span data-ttu-id="b5290-191">A licenc-alapú kedvezmények a számlára való leképezéséhez adja a **TotalOtherDiscount** oszlopot a licenc-alapú fájlból.</span><span class="sxs-lookup"><span data-stu-id="b5290-191">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="b5290-192">*A licenc-alapú kedvezmények több feltöltési típusra is alkalmazhatók.*</span><span class="sxs-lookup"><span data-stu-id="b5290-192">*License-based discounts may be applied to multiple charge types.*</span></span>
