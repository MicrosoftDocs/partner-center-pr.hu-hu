---
title: A megbékélési fájlok használata
ms.topic: article
ms.date: 03/26/2021
description: Ismerje meg a fiókpartner egyeztetési fájljait, valamint azt, hogy miként értelmezhető az adott számlázási időszakra vonatkozó díjak részletes, sorokra vonatkozó nézetei.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633896"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="c8e67-103">Megtudhatja, hogyan olvashatja el a partner Center-egyeztetési fájlok sorát</span><span class="sxs-lookup"><span data-stu-id="c8e67-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="c8e67-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="c8e67-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c8e67-105">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="c8e67-105">Billing admin</span></span>
- <span data-ttu-id="c8e67-106">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="c8e67-106">Global admin</span></span>

<span data-ttu-id="c8e67-107">A partner Centerről letöltheti a megbékélési fájlokat a számlázási ciklusban minden egyes díj részletes, sorban álló nézetéhez.</span><span class="sxs-lookup"><span data-stu-id="c8e67-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="c8e67-108">A sor részletei közé tartoznak az egyes ügyfelek előfizetései, valamint a részletes események (például a licencek félidős hozzáadása az előfizetéshez).</span><span class="sxs-lookup"><span data-stu-id="c8e67-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="c8e67-109">A **számla** beolvasásával kapcsolatos információkért lásd: [a számla olvasása](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="c8e67-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="c8e67-110">Az egyeztetési fájl mezőinek megismerése</span><span class="sxs-lookup"><span data-stu-id="c8e67-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="c8e67-111">Licencalapú egyeztetési fájl mezői</span><span class="sxs-lookup"><span data-stu-id="c8e67-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="c8e67-112">Használatalapú egyeztetési fájl mezői</span><span class="sxs-lookup"><span data-stu-id="c8e67-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="c8e67-113">Napi névleges használatú egyeztetési fájl mezői</span><span class="sxs-lookup"><span data-stu-id="c8e67-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="c8e67-114">Egyszeri beszerzési CSP-egyeztetési fájl mezői</span><span class="sxs-lookup"><span data-stu-id="c8e67-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="c8e67-115">A díjszabási típusok megértése az egyeztetési fájlokban</span><span class="sxs-lookup"><span data-stu-id="c8e67-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="c8e67-116">Ha meg szeretné ismerni az egyeztetési fájlok (a **ChargeType** oszlop) használati feltételeit, tekintse meg a következőt: [egyeztetési](recon-file-charge-types.md)feltételek.</span><span class="sxs-lookup"><span data-stu-id="c8e67-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="c8e67-117">Formázási problémák javítása</span><span class="sxs-lookup"><span data-stu-id="c8e67-117">Fix formatting issues</span></span>

<span data-ttu-id="c8e67-118">Esetenként előfordulhat, hogy egy egyeztető fájl formázási problémákat tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="c8e67-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="c8e67-119">Ez a probléma például akkor fordulhat elő, ha az en-US területi beállítás nincs használatban.</span><span class="sxs-lookup"><span data-stu-id="c8e67-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="c8e67-120">A következő lépések végrehajtásával javítsa ki az egyeztetési fájlok formázási problémáit:</span><span class="sxs-lookup"><span data-stu-id="c8e67-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="c8e67-121">Nyissa meg az egyeztetési fájlt (. csv formátumban) a Microsoft Excelben.</span><span class="sxs-lookup"><span data-stu-id="c8e67-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="c8e67-122">Válassza ki a fájl első oszlopát.</span><span class="sxs-lookup"><span data-stu-id="c8e67-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="c8e67-123">Nyissa meg a **szöveg konvertálása oszlopokra varázslót**.</span><span class="sxs-lookup"><span data-stu-id="c8e67-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="c8e67-124">A menüszalagon válassza az adatelemet, majd válassza a **szöveg oszlopokra** **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c8e67-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="c8e67-125">A varázslóban válassza a **tagolt fájl típusa** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c8e67-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="c8e67-126">Ezután válassza a **tovább** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c8e67-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="c8e67-127">A **határolójelek** mezőben válassza a **vessző** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c8e67-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="c8e67-128">(Ha a **Tab** már be van jelölve, akkor ezt a lehetőséget kiválasztva hagyhatja.) Ezután válassza a **tovább** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c8e67-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="c8e67-129">Az **oszlop adatformátuma** mezőben válassza a **Date: MDY** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c8e67-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="c8e67-130">Ezután válassza a **tovább** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c8e67-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="c8e67-131">Az **oszlop adatformátuma** mezőben válassza a **szöveg** lehetőséget az összes oszlop értéknél.</span><span class="sxs-lookup"><span data-stu-id="c8e67-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="c8e67-132">Ezután válassza a **Befejezés** gombot.</span><span class="sxs-lookup"><span data-stu-id="c8e67-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="c8e67-133">Az egyeztetési fájlok programozott módon tölthetők le</span><span class="sxs-lookup"><span data-stu-id="c8e67-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="c8e67-134">Az egyeztetési fájlok nagyon nagy méretűek lehetnek, és időnként nehéz letölteni.</span><span class="sxs-lookup"><span data-stu-id="c8e67-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="c8e67-135">Ha programozott módon szeretné letölteni az egyeztetési fájlokat, tekintse meg a [Számlázási sorok beolvasása című cikket](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="c8e67-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="c8e67-136">Ha a fájl túllépi az Excelben megadott korlátot</span><span class="sxs-lookup"><span data-stu-id="c8e67-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="c8e67-137">Ha le tudja tölteni az egyeztetési fájlt, de nem nyitja meg a Microsoft Excelben, valószínűleg azt jelenti, hogy a fájl több sort is tartalmaz, mint amennyit az Excel engedélyez.</span><span class="sxs-lookup"><span data-stu-id="c8e67-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="c8e67-138">Ha ez történik, a fájl megnyitásához használhatja az alábbi eljárások egyikét.</span><span class="sxs-lookup"><span data-stu-id="c8e67-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="c8e67-139">Felderítési fájl megnyitása Power BI</span><span class="sxs-lookup"><span data-stu-id="c8e67-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="c8e67-140">Töltse le az egyeztetési fájlt a szokásos módon.</span><span class="sxs-lookup"><span data-stu-id="c8e67-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="c8e67-141">Power BI-példány letöltése, telepítése és megnyitása.</span><span class="sxs-lookup"><span data-stu-id="c8e67-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="c8e67-142">A Power BI **Kezdőlap** lapon válassza az **adatlekérdezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c8e67-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="c8e67-143">A **gyakori adatforrások** listájában válassza a **text/CSV** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c8e67-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="c8e67-144">Ha a rendszer kéri, nyissa meg a Recon-fájlt.</span><span class="sxs-lookup"><span data-stu-id="c8e67-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="c8e67-145">Egy Recon-fájl megnyitása egy Excel-pivot táblában</span><span class="sxs-lookup"><span data-stu-id="c8e67-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="c8e67-146">Töltse le az egyeztetési fájlt a szokásos módon.</span><span class="sxs-lookup"><span data-stu-id="c8e67-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="c8e67-147">Nyisson meg egy új fájlt a Microsoft Excelben.</span><span class="sxs-lookup"><span data-stu-id="c8e67-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="c8e67-148">Az **adatok** lapon válassza az **adatok lekérése** elemet, válassza a **fájlból** lehetőséget, majd válassza a **text/CSV** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c8e67-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="c8e67-149">Ha a rendszer kéri, nyissa meg a Recon-fájlt.</span><span class="sxs-lookup"><span data-stu-id="c8e67-149">When prompted, open your recon file.</span></span> <span data-ttu-id="c8e67-150">Ekkor megjelennek az adatai.</span><span class="sxs-lookup"><span data-stu-id="c8e67-150">Your data will appear.</span></span>
5. <span data-ttu-id="c8e67-151">A **Betöltés** legördülő menüben válassza a **Betöltés a** következőhöz lehetőséget, majd **az OK gombot**.</span><span class="sxs-lookup"><span data-stu-id="c8e67-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="c8e67-152">Az **adatimportálás** párbeszédpanelen válassza a **kimutatás jelentést** a fájl megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="c8e67-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="c8e67-153">Adók vagy ÁFA leképezése</span><span class="sxs-lookup"><span data-stu-id="c8e67-153">Map taxes or VAT</span></span>

<span data-ttu-id="c8e67-154">Adók vagy hozzáadottérték-adó (ÁFA) hozzárendelése a számlához:</span><span class="sxs-lookup"><span data-stu-id="c8e67-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="c8e67-155">Adja meg az **adó** oszlopot a licenc-alapú fájlból.</span><span class="sxs-lookup"><span data-stu-id="c8e67-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="c8e67-156">A **TaxAmount** oszlop összege a használaton alapuló fájlból.</span><span class="sxs-lookup"><span data-stu-id="c8e67-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="c8e67-157">Itemize-egyeztetési fájlok partner szerint</span><span class="sxs-lookup"><span data-stu-id="c8e67-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="c8e67-158">A **közvetett modellben** lévő partnerek ezeket a további mezőket használhatják a licenc-és a használati alapú egyeztetési fájlokban is, hogy itemize a fájlokat a viszonteladók által.</span><span class="sxs-lookup"><span data-stu-id="c8e67-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="c8e67-159">MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="c8e67-159">MPN ID</span></span> | <span data-ttu-id="c8e67-160">Description</span><span class="sxs-lookup"><span data-stu-id="c8e67-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="c8e67-161">MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="c8e67-161">MPN ID</span></span> | <span data-ttu-id="c8e67-162">A Cloud Solution Provider (CSP) partner (közvetlen vagy közvetett) Microsoft Partner Network (MPN) azonosítója.</span><span class="sxs-lookup"><span data-stu-id="c8e67-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="c8e67-163">Viszonteladói MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="c8e67-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="c8e67-164">Az [előfizetéshez tartozó rekord viszonteladójának MPN-azonosítója](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="c8e67-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="c8e67-165">Ez a mező az adott előfizetéshez tartozó, a partner Centerben megadott viszonteladói AZONOSÍTÓnak felel meg.</span><span class="sxs-lookup"><span data-stu-id="c8e67-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="c8e67-166">Csak a közvetett modellben lévő partnereknek szóló egyeztető fájlokban jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="c8e67-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="c8e67-167">Viszonteladói MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="c8e67-167">Reseller MPN ID</span></span>

<span data-ttu-id="c8e67-168">Ha egy CSP-partner közvetlenül az ügyfélnek adta el az előfizetést, az **MPN-azonosítójuk** kétszer jelenik meg, mint az **MPN-azonosító** és a **viszonteladói MPN-azonosító**.</span><span class="sxs-lookup"><span data-stu-id="c8e67-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="c8e67-169">Ha a CSP-partner rendelkezik **MPN-azonosító** nélküli viszonteladóval, akkor ez az érték a partner **MPN-azonosítóját** adja meg helyette.</span><span class="sxs-lookup"><span data-stu-id="c8e67-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="c8e67-170">Ha a CSP-partner eltávolít egy **viszonteladói MPN-azonosítót**, az érték *-1* lesz.</span><span class="sxs-lookup"><span data-stu-id="c8e67-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="c8e67-171">A **viszonteladói MPN-azonosító** megtekintése vagy frissítése:</span><span class="sxs-lookup"><span data-stu-id="c8e67-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="c8e67-172">Jelentkezzen be a Partnerközpontba.</span><span class="sxs-lookup"><span data-stu-id="c8e67-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="c8e67-173">A partner Center menüben válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c8e67-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="c8e67-174">Válassza ki az ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="c8e67-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="c8e67-175">Az ügyfél menüben válassza az **előfizetések** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c8e67-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="c8e67-176">Válassza ki az előfizetést a listából.</span><span class="sxs-lookup"><span data-stu-id="c8e67-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="c8e67-177">Válassza a **frissítés** lehetőséget a **viszonteladó (MPN-azonosító)** módosításához.</span><span class="sxs-lookup"><span data-stu-id="c8e67-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c8e67-178">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c8e67-178">Next steps</span></span>

- [<span data-ttu-id="c8e67-179">A Bill & Recon-fájl beolvasása</span><span class="sxs-lookup"><span data-stu-id="c8e67-179">How to read your bill & recon file</span></span>](read-your-bill.md) 