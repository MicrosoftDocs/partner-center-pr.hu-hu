---
title: A megbékélési fájlok használata
ms.topic: article
ms.date: 06/08/2020
description: Ismerje meg a fiókpartner egyeztetési fájljait, valamint azt, hogy miként értelmezhető az adott számlázási időszakra vonatkozó díjak részletes, sorokra vonatkozó nézetei.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 98bfd9a9ce6f03ad62a830f05ba82f9b90268326
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528518"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="4cb56-103">Megtudhatja, hogyan olvashatja el a partner Center-egyeztetési fájlok sorát</span><span class="sxs-lookup"><span data-stu-id="4cb56-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="4cb56-104">A következőkre vonatkozik:</span><span class="sxs-lookup"><span data-stu-id="4cb56-104">Applies to:</span></span>

- <span data-ttu-id="4cb56-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="4cb56-105">Partner Center</span></span>
- <span data-ttu-id="4cb56-106">Az USA kormányzati szerveinek Microsoft Cloud a partneri központ</span><span class="sxs-lookup"><span data-stu-id="4cb56-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="4cb56-107">A partner Centerről letöltheti a megbékélési fájlokat a számlázási ciklusban minden egyes díj részletes, sorban álló nézetéhez.</span><span class="sxs-lookup"><span data-stu-id="4cb56-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="4cb56-108">A sor részletei közé tartoznak az egyes ügyfelek előfizetései, valamint a részletes események (például a licencek félidős hozzáadása az előfizetéshez).</span><span class="sxs-lookup"><span data-stu-id="4cb56-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="4cb56-109">Megfelelő szerepkörök:</span><span class="sxs-lookup"><span data-stu-id="4cb56-109">Appropriate roles:</span></span>

- <span data-ttu-id="4cb56-110">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="4cb56-110">Billing admin</span></span>
- <span data-ttu-id="4cb56-111">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="4cb56-111">Global admin</span></span>

<span data-ttu-id="4cb56-112">A **számla** beolvasásával kapcsolatos információkért lásd: [a számla olvasása](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="4cb56-112">For information on how to read your **invoice** , see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="4cb56-113">Az egyeztetési fájl mezőinek megismerése</span><span class="sxs-lookup"><span data-stu-id="4cb56-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="4cb56-114">Licenc-alapú egyeztetési fájl mezői</span><span class="sxs-lookup"><span data-stu-id="4cb56-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="4cb56-115">Használaton alapuló egyeztetési fájl mezői</span><span class="sxs-lookup"><span data-stu-id="4cb56-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="4cb56-116">Napi besorolású használati egyeztetési fájl mezői</span><span class="sxs-lookup"><span data-stu-id="4cb56-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="4cb56-117">A díjszabási típusok megértése az egyeztetési fájlokban</span><span class="sxs-lookup"><span data-stu-id="4cb56-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="4cb56-118">Ha meg szeretné ismerni az egyeztetési fájlok (a **ChargeType** oszlop) használati feltételeit, tekintse meg a következőt: [egyeztetési](recon-file-charge-types.md)feltételek.</span><span class="sxs-lookup"><span data-stu-id="4cb56-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="4cb56-119">Formázási problémák javítása</span><span class="sxs-lookup"><span data-stu-id="4cb56-119">Fix formatting issues</span></span>

<span data-ttu-id="4cb56-120">Esetenként előfordulhat, hogy egy egyeztető fájl formázási problémákat tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="4cb56-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="4cb56-121">Ez a probléma például akkor fordulhat elő, ha az en-US területi beállítás nincs használatban.</span><span class="sxs-lookup"><span data-stu-id="4cb56-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="4cb56-122">A következő lépések végrehajtásával javítsa ki az egyeztetési fájlok formázási problémáit:</span><span class="sxs-lookup"><span data-stu-id="4cb56-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="4cb56-123">Nyissa meg az egyeztetési fájlt (. csv formátumban) a Microsoft Excelben.</span><span class="sxs-lookup"><span data-stu-id="4cb56-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="4cb56-124">Válassza ki a fájl első oszlopát.</span><span class="sxs-lookup"><span data-stu-id="4cb56-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="4cb56-125">Nyissa meg a **szöveg konvertálása oszlopokra varázslót** .</span><span class="sxs-lookup"><span data-stu-id="4cb56-125">Open the **Convert Text to Columns Wizard** .</span></span> <span data-ttu-id="4cb56-126">A menüszalagon válassza az adatelemet, majd válassza a **szöveg oszlopokra** **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4cb56-126">On the ribbon, select **Data** , then select **Text to Columns** .</span></span>
4. <span data-ttu-id="4cb56-127">A varázslóban válassza a **tagolt fájl típusa** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4cb56-127">In the wizard, select **Delimited file type** .</span></span> <span data-ttu-id="4cb56-128">Ezután válassza a **tovább** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4cb56-128">Then, select **Next** .</span></span>
5. <span data-ttu-id="4cb56-129">A **határolójelek** mezőben válassza a **vessző** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4cb56-129">In the **Delimiters** field, select **Comma** .</span></span> <span data-ttu-id="4cb56-130">(Ha a **Tab** már be van jelölve, akkor ezt a lehetőséget kiválasztva hagyhatja.) Ezután válassza a **tovább** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4cb56-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next** .</span></span>
6. <span data-ttu-id="4cb56-131">Az **oszlop adatformátuma** mezőben válassza a **Date: MDY** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4cb56-131">In the **Column data format** field, select **Date:MDY** .</span></span> <span data-ttu-id="4cb56-132">Ezután válassza a **tovább** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4cb56-132">Then, select **Next** .</span></span>
7. <span data-ttu-id="4cb56-133">Az **oszlop adatformátuma** mezőben válassza a **szöveg** lehetőséget az összes oszlop értéknél.</span><span class="sxs-lookup"><span data-stu-id="4cb56-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="4cb56-134">Ezután válassza a **Befejezés** gombot.</span><span class="sxs-lookup"><span data-stu-id="4cb56-134">Then, select **Finish** .</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="4cb56-135">Az egyeztetési fájlok programozott módon tölthetők le</span><span class="sxs-lookup"><span data-stu-id="4cb56-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="4cb56-136">Az egyeztetési fájlok nagyon nagy méretűek lehetnek, és időnként nehéz letölteni.</span><span class="sxs-lookup"><span data-stu-id="4cb56-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="4cb56-137">Ha programozott módon szeretné letölteni az egyeztetési fájlokat, tekintse meg a [Számlázási sorok beolvasása című cikket](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="4cb56-137">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="4cb56-138">Adók vagy ÁFA leképezése</span><span class="sxs-lookup"><span data-stu-id="4cb56-138">Map taxes or VAT</span></span>

<span data-ttu-id="4cb56-139">Adók vagy hozzáadottérték-adó (ÁFA) hozzárendelése a számlához:</span><span class="sxs-lookup"><span data-stu-id="4cb56-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="4cb56-140">Adja meg az **adó** oszlopot a licenc-alapú fájlból.</span><span class="sxs-lookup"><span data-stu-id="4cb56-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="4cb56-141">A **TaxAmount** oszlop összege a használaton alapuló fájlból.</span><span class="sxs-lookup"><span data-stu-id="4cb56-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="4cb56-142">Itemize-egyeztetési fájlok partner szerint</span><span class="sxs-lookup"><span data-stu-id="4cb56-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="4cb56-143">A **közvetett modellben** lévő partnerek ezeket a további mezőket használhatják a licenc-és a használati alapú egyeztetési fájlokban is, hogy itemize a fájlokat a viszonteladók által.</span><span class="sxs-lookup"><span data-stu-id="4cb56-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="4cb56-144">MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="4cb56-144">MPN ID</span></span> | <span data-ttu-id="4cb56-145">Description (Leírás)</span><span class="sxs-lookup"><span data-stu-id="4cb56-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="4cb56-146">MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="4cb56-146">MPN ID</span></span> | <span data-ttu-id="4cb56-147">A Cloud Solution Provider (CSP) partner (közvetlen vagy közvetett) Microsoft Partner Network (MPN) azonosítója.</span><span class="sxs-lookup"><span data-stu-id="4cb56-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="4cb56-148">Viszonteladói MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="4cb56-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="4cb56-149">Az [előfizetéshez tartozó rekord viszonteladójának MPN-azonosítója](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="4cb56-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="4cb56-150">Ez a mező az adott előfizetéshez tartozó, a partner Centerben megadott viszonteladói AZONOSÍTÓnak felel meg.</span><span class="sxs-lookup"><span data-stu-id="4cb56-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="4cb56-151">Csak a közvetett modellben lévő partnereknek szóló egyeztető fájlokban jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="4cb56-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="4cb56-152">Viszonteladói MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="4cb56-152">Reseller MPN ID</span></span>

<span data-ttu-id="4cb56-153">Ha egy CSP-partner közvetlenül az ügyfélnek adta el az előfizetést, az **MPN-azonosítójuk** kétszer jelenik meg, mint az **MPN-azonosító** és a **viszonteladói MPN-azonosító** .</span><span class="sxs-lookup"><span data-stu-id="4cb56-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID** .</span></span>

<span data-ttu-id="4cb56-154">Ha a CSP-partner rendelkezik **MPN-azonosító** nélküli viszonteladóval, akkor ez az érték a partner **MPN-azonosítóját** adja meg helyette.</span><span class="sxs-lookup"><span data-stu-id="4cb56-154">If a CSP partner has a reseller with no **MPN ID** , this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="4cb56-155">Ha a CSP-partner eltávolít egy **viszonteladói MPN-azonosítót** , az érték *-1* lesz.</span><span class="sxs-lookup"><span data-stu-id="4cb56-155">If the CSP partner removes a **Reseller MPN ID** , this value will be set to *-1* .</span></span>

<span data-ttu-id="4cb56-156">A **viszonteladói MPN-azonosító** megtekintése vagy frissítése:</span><span class="sxs-lookup"><span data-stu-id="4cb56-156">To view or update the **Reseller MPN ID** :</span></span>

1. <span data-ttu-id="4cb56-157">Jelentkezzen be a Partnerközpontba.</span><span class="sxs-lookup"><span data-stu-id="4cb56-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="4cb56-158">A partner Center menüben válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4cb56-158">In the Partner Center menu, select **Customers** .</span></span>
3. <span data-ttu-id="4cb56-159">Válassza ki az ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="4cb56-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="4cb56-160">Az ügyfél menüben válassza az **előfizetések** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4cb56-160">In the customer menu, select **Subscriptions** .</span></span>
5. <span data-ttu-id="4cb56-161">Válassza ki az előfizetést a listából.</span><span class="sxs-lookup"><span data-stu-id="4cb56-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="4cb56-162">Válassza a **frissítés** lehetőséget a **viszonteladó (MPN-azonosító)** módosításához.</span><span class="sxs-lookup"><span data-stu-id="4cb56-162">Select **update** to change the **Reseller (MPN ID)** .</span></span>