---
title: Egyeztetési fájlok díjtípusai
ms.topic: article
ms.date: 06/05/2020
description: Megismerheti a díjtípusokat (például licencalapú, használatalapú és egyszeres), krediteket és kedvezményeket az egyeztetési Partnerközpont fájlokban.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855879"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="e28eb-103">Az egyeztetési fájlokban található különböző Partnerközpont típusainak</span><span class="sxs-lookup"><span data-stu-id="e28eb-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="e28eb-104">**A következőkre vonatkozik:** Partnerközpont | Partnerközpont a Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="e28eb-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="e28eb-105">**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="e28eb-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="e28eb-106">Ez a cikk a számlaszakaszok és a társított díjtípusok közötti leképezéseket ismerteti, amelyek az egyeztetési fájlban lehetnek.</span><span class="sxs-lookup"><span data-stu-id="e28eb-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="e28eb-107">A számla a díjak összegzését biztosítja.</span><span class="sxs-lookup"><span data-stu-id="e28eb-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="e28eb-108">Az egyeztetési fájl részletesen részletezi a sortétel-tranzakciókat, beleértve a díjtípusokat is.</span><span class="sxs-lookup"><span data-stu-id="e28eb-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="e28eb-109">Az egyeztetési fájlokkal kapcsolatos további információkért lásd az egyeztetési [fájlok használatát.](use-the-reconciliation-files.md)</span><span class="sxs-lookup"><span data-stu-id="e28eb-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="e28eb-110">Mind [a használatalapú egyeztetési](usage-based-recon-files.md) fájlok, mind a licencalapú egyeztetési fájlok [csak](license-based-recon-files.md) a használattal kapcsolatos tranzakciókat és díjakat (felhasznált egységeket és kapcsolódó díjakat) mutatják.</span><span class="sxs-lookup"><span data-stu-id="e28eb-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="e28eb-111">A számlán a Helyesbítésekként megjelenő egyszeres jóváírások, kedvezmények vagy visszatérítések nem jelennek meg az egyeztetési fájlban. </span><span class="sxs-lookup"><span data-stu-id="e28eb-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="e28eb-112">Díjtípusok leképezés a számlás díjakra</span><span class="sxs-lookup"><span data-stu-id="e28eb-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="e28eb-113">A díj összegeinek a számla és az egyeztetési fájl közötti kereszthivatkozáshoz használja a Microsoft Excel szűrési lehetőségeit.</span><span class="sxs-lookup"><span data-stu-id="e28eb-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="e28eb-114">Szűrhet díjtípusok szerint az egyeztetési fájlban, hogy a számlázási díjakat leképezheti az egyeztetési fájlban található költséglebontások készletére.</span><span class="sxs-lookup"><span data-stu-id="e28eb-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="e28eb-115">Licencalapú díjak</span><span class="sxs-lookup"><span data-stu-id="e28eb-115">License-based charges</span></span>

<span data-ttu-id="e28eb-116">Ezeknek a licencalapú díjaknak a számlán való leképezésén a **licencalapú** fájl Amount oszlopát összegezve kell összeadni.</span><span class="sxs-lookup"><span data-stu-id="e28eb-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e28eb-117">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="e28eb-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e28eb-118">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="e28eb-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e28eb-119">Aktiválási díj</span><span class="sxs-lookup"><span data-stu-id="e28eb-119">Activation fee</span></span> | <span data-ttu-id="e28eb-120">Az ügyfélnek a vásárlást követően az előfizetés használata után felszámított összeg.</span><span class="sxs-lookup"><span data-stu-id="e28eb-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="e28eb-121">Lemondási díj</span><span class="sxs-lookup"><span data-stu-id="e28eb-121">Cancel fee</span></span> | <span data-ttu-id="e28eb-122">Az ügyfélnek a társított licencek módosult díjának megfelelő visszatérítésekért.</span><span class="sxs-lookup"><span data-stu-id="e28eb-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="e28eb-123">Példány-prorate megszakítása</span><span class="sxs-lookup"><span data-stu-id="e28eb-123">Cancel instance prorate</span></span> | <span data-ttu-id="e28eb-124">A havi előfizetéssel rendelkező ügyfél előfizetésének felfüggesztése és a társított licencek ugyanabban a hónapban való módosult időszakában az időszakra vonatkozó, az időszakra vonatkozó díjakat az időszakban megszüntetjük.</span><span class="sxs-lookup"><span data-stu-id="e28eb-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="e28eb-125">Ciklus díja</span><span class="sxs-lookup"><span data-stu-id="e28eb-125">Cycle fee</span></span> | <span data-ttu-id="e28eb-126">Az előfizetések rendszeres díjai.</span><span class="sxs-lookup"><span data-stu-id="e28eb-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="e28eb-127">Ciklikus példány-prorate</span><span class="sxs-lookup"><span data-stu-id="e28eb-127">Cycle instance prorate</span></span> | <span data-ttu-id="e28eb-128">Az ügyféltől származó, a társított licencek módosulásával kapcsolatos, az igényeknek megfelelő díjakat kell megállapítani.</span><span class="sxs-lookup"><span data-stu-id="e28eb-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="e28eb-129">Díjfizetési díjak lemondáskor</span><span class="sxs-lookup"><span data-stu-id="e28eb-129">Prorate fees when cancel</span></span> | <span data-ttu-id="e28eb-130">A szolgáltatás fel nem használt részének időkorrekét visszatérítése lemondáskor.</span><span class="sxs-lookup"><span data-stu-id="e28eb-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="e28eb-131">Az aktuális ajánlatról való átváltás díjai</span><span class="sxs-lookup"><span data-stu-id="e28eb-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="e28eb-132">Az aktuális havi előfizetésről egy éves előfizetésre való átváltás után az időkorreklott díjak.</span><span class="sxs-lookup"><span data-stu-id="e28eb-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="e28eb-133">Az új ajánlatra való átváltás díjai</span><span class="sxs-lookup"><span data-stu-id="e28eb-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="e28eb-134">A havi előfizetés új éves előfizetésre való átváltása után fizetendő díjak.</span><span class="sxs-lookup"><span data-stu-id="e28eb-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="e28eb-135">Díjfizetés vásárláskor</span><span class="sxs-lookup"><span data-stu-id="e28eb-135">Prorate fees when purchase</span></span> | <span data-ttu-id="e28eb-136">Az előfizetés díjtípusa havi vagy éves számlázás esetén is.</span><span class="sxs-lookup"><span data-stu-id="e28eb-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="e28eb-137">Megújítás után fizetendő díj</span><span class="sxs-lookup"><span data-stu-id="e28eb-137">Prorate fee when renew</span></span> | <span data-ttu-id="e28eb-138">Az előfizetés megújítása után fizetendő díjak.</span><span class="sxs-lookup"><span data-stu-id="e28eb-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="e28eb-139">Díj megújítása</span><span class="sxs-lookup"><span data-stu-id="e28eb-139">Renew fee</span></span> | <span data-ttu-id="e28eb-140">Előfizetés megújításának díj</span><span class="sxs-lookup"><span data-stu-id="e28eb-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="e28eb-141">Az aktiválás díjai</span><span class="sxs-lookup"><span data-stu-id="e28eb-141">Prorate fees when activate</span></span> | <span data-ttu-id="e28eb-142">Az aktiválástól a számlázási időszak végéig fizetendő díjak.</span><span class="sxs-lookup"><span data-stu-id="e28eb-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="e28eb-143">Egyszer fizetendő díjak</span><span class="sxs-lookup"><span data-stu-id="e28eb-143">One-time charges</span></span>

<span data-ttu-id="e28eb-144">Ha ezeket az egyszeres díjakat le kell leképezni a számlájára, összegezve a licencalapú fájl **Amount** (Összeg) oszlopát.</span><span class="sxs-lookup"><span data-stu-id="e28eb-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e28eb-145">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="e28eb-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e28eb-146">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="e28eb-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e28eb-147">Új</span><span class="sxs-lookup"><span data-stu-id="e28eb-147">New</span></span> | <span data-ttu-id="e28eb-148">Új vásárlás létrehozásakor használatos.</span><span class="sxs-lookup"><span data-stu-id="e28eb-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="e28eb-149">addQuantity (Hozzáadásquantitás)</span><span class="sxs-lookup"><span data-stu-id="e28eb-149">addQuantity</span></span> | <span data-ttu-id="e28eb-150">Az eredeti vásárlás visszatérítésében és az új mennyiségben is felhasználható a növekedés után.</span><span class="sxs-lookup"><span data-stu-id="e28eb-150">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="e28eb-151">removeQuantity (Quantity eltávolítása)</span><span class="sxs-lookup"><span data-stu-id="e28eb-151">removeQuantity</span></span> | <span data-ttu-id="e28eb-152">Az eredeti vásárlás visszatérítésében és az új mennyiségben is felhasználható a csökkenést követően.</span><span class="sxs-lookup"><span data-stu-id="e28eb-152">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="e28eb-153">Mégse</span><span class="sxs-lookup"><span data-stu-id="e28eb-153">Cancel</span></span> | <span data-ttu-id="e28eb-154">Az előfizetés lemondása esetén használatos.</span><span class="sxs-lookup"><span data-stu-id="e28eb-154">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="e28eb-155">Konvertálás</span><span class="sxs-lookup"><span data-stu-id="e28eb-155">Convert</span></span> | <span data-ttu-id="e28eb-156">Akkor használatos, ha a licenc frissítve van, de a licencek száma változatlan marad.</span><span class="sxs-lookup"><span data-stu-id="e28eb-156">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="e28eb-157">Használati díjak</span><span class="sxs-lookup"><span data-stu-id="e28eb-157">Usage charges</span></span>

<span data-ttu-id="e28eb-158">Ezeknek a használati díjaknak a számlán való leképezésén a Használatalapú fájl **PretaxCharges** oszlopát összegezve kell összeadni.</span><span class="sxs-lookup"><span data-stu-id="e28eb-158">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e28eb-159">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="e28eb-159">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e28eb-160">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="e28eb-160">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e28eb-161">Használati díj értékelése lemondáskor</span><span class="sxs-lookup"><span data-stu-id="e28eb-161">Assess usage fee when cancel</span></span> | <span data-ttu-id="e28eb-162">A ki nem fizetett használat lemondása után a jelenlegi számlázási időszakra vonatkozó használati díj elérése.</span><span class="sxs-lookup"><span data-stu-id="e28eb-162">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="e28eb-163">A jelenlegi ciklus használati díjának felmérése</span><span class="sxs-lookup"><span data-stu-id="e28eb-163">Assess usage fee for current cycle</span></span> | <span data-ttu-id="e28eb-164">Az aktuális számlázási időszak használati díjának elérése.</span><span class="sxs-lookup"><span data-stu-id="e28eb-164">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="e28eb-165">Kreditek</span><span class="sxs-lookup"><span data-stu-id="e28eb-165">Credits</span></span>

<span data-ttu-id="e28eb-166">A kreditek a számlán való leképezésén a következőt kell látni:</span><span class="sxs-lookup"><span data-stu-id="e28eb-166">To map these credits to your invoice:</span></span>

- <span data-ttu-id="e28eb-167">Összegezve **a TotalForCustomer a** licencalapú fájlból.</span><span class="sxs-lookup"><span data-stu-id="e28eb-167">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="e28eb-168">Összegezve **a PostTaxTotal** oszlopot a használatalapú fájlból.</span><span class="sxs-lookup"><span data-stu-id="e28eb-168">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="e28eb-169">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="e28eb-169">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e28eb-170">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="e28eb-170">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e28eb-171">Sorelem eltolása</span><span class="sxs-lookup"><span data-stu-id="e28eb-171">Offset a line item</span></span> | <span data-ttu-id="e28eb-172">Részleges vagy teljes visszatérítés egy sortételre, az adókkal együtt.</span><span class="sxs-lookup"><span data-stu-id="e28eb-172">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="e28eb-173">Használatalapú kedvezmények</span><span class="sxs-lookup"><span data-stu-id="e28eb-173">Usage-based discounts</span></span>

<span data-ttu-id="e28eb-174">Ezeknek a használatalapú kedvezményeknek a számlán való leképezésén a Használatalapú fájl **PretaxCharges** oszlopát összegezve adatokat kaphat.</span><span class="sxs-lookup"><span data-stu-id="e28eb-174">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e28eb-175">Díj leírása (ChargeType oszlop az egyeztetési fájlban)</span><span class="sxs-lookup"><span data-stu-id="e28eb-175">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e28eb-176">Díj magyarázata</span><span class="sxs-lookup"><span data-stu-id="e28eb-176">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e28eb-177">Aktiválási kedvezmény</span><span class="sxs-lookup"><span data-stu-id="e28eb-177">Activation discount</span></span> | <span data-ttu-id="e28eb-178">Az előfizetés aktiválásakor alkalmazott kedvezmény.</span><span class="sxs-lookup"><span data-stu-id="e28eb-178">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="e28eb-179">Ciklusra kedvezményes</span><span class="sxs-lookup"><span data-stu-id="e28eb-179">Cycle discount</span></span> | <span data-ttu-id="e28eb-180">Az időszakos díjakra alkalmazott kedvezmény.</span><span class="sxs-lookup"><span data-stu-id="e28eb-180">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="e28eb-181">Kedvezmény megújítása</span><span class="sxs-lookup"><span data-stu-id="e28eb-181">Renew discount</span></span> | <span data-ttu-id="e28eb-182">Az előfizetés megújításakor alkalmazott kedvezmény.</span><span class="sxs-lookup"><span data-stu-id="e28eb-182">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="e28eb-183">Kedvezmény lemondása</span><span class="sxs-lookup"><span data-stu-id="e28eb-183">Cancel discount</span></span> | <span data-ttu-id="e28eb-184">A kedvezmények törlésekor alkalmazott díjak.</span><span class="sxs-lookup"><span data-stu-id="e28eb-184">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="e28eb-185">Licencalapú kedvezmények</span><span class="sxs-lookup"><span data-stu-id="e28eb-185">License-based discounts</span></span>

<span data-ttu-id="e28eb-186">Ha licencalapú kedvezményeket kell leképezni a számlára, összesítenünk kell a **TotalOtherDiscount** oszlopot a licencalapú fájlból.</span><span class="sxs-lookup"><span data-stu-id="e28eb-186">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="e28eb-187">*A licencalapú kedvezmények több díjtípusra is alkalmazhatók.*</span><span class="sxs-lookup"><span data-stu-id="e28eb-187">*License-based discounts may be applied to multiple charge types.*</span></span>
