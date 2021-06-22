---
title: Az egyeztetési fájlok használata
ms.topic: article
ms.date: 03/26/2021
description: Megismerheti az egyeztetési fájlokat Partnerközpont és az adott számlázási ciklus díjtételek részletes, sortételes nézeteinek értelmezését.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431572"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="79719-103">Ismerje meg, hogyan olvashatja be az egyeztetési fájlokban Partnerközpont sorelemeket</span><span class="sxs-lookup"><span data-stu-id="79719-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="79719-104">**Megfelelő szerepkörök:** Számlázási rendszergazdai | Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="79719-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="79719-105">Az egyeztetési fájlokat letöltheti a Partnerközpont a számlázási ciklusban lévő egyes díjtételek részletes, sorelemnézetéhez.</span><span class="sxs-lookup"><span data-stu-id="79719-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="79719-106">A sortételek részletei tartalmazzák az egyes ügyfelek előfizetéseiért fizetendő díjakat és a részletes eseményeket (például a licencek előfizetéshez való rövid távú kiegészítését).</span><span class="sxs-lookup"><span data-stu-id="79719-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="79719-107">A számla beolvassa a (Számla olvasása) [adatokat.](read-your-bill.md) </span><span class="sxs-lookup"><span data-stu-id="79719-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="79719-108">Az egyeztetési fájlmezők</span><span class="sxs-lookup"><span data-stu-id="79719-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="79719-109">Licencalapú egyeztetési fájl mezői</span><span class="sxs-lookup"><span data-stu-id="79719-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="79719-110">Használatalapú egyeztetési fájl mezői</span><span class="sxs-lookup"><span data-stu-id="79719-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="79719-111">Napi névleges használatú egyeztetési fájl mezői</span><span class="sxs-lookup"><span data-stu-id="79719-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="79719-112">Egy alkalommal vásárolt CSP egyeztetési fájl mezői</span><span class="sxs-lookup"><span data-stu-id="79719-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="79719-113">Díjtípusok az egyeztetési fájlokban</span><span class="sxs-lookup"><span data-stu-id="79719-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="79719-114">Az egyeztetési fájlokban (a **ChargeType** oszlopban) található díjtípusokról az Egyeztetési fájl [díjtípusa tartalmaz további adatokat.](recon-file-charge-types.md)</span><span class="sxs-lookup"><span data-stu-id="79719-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="79719-115">Formázási problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="79719-115">Fix formatting issues</span></span>

<span data-ttu-id="79719-116">Az egyeztetési fájlok esetenként formázási problémákat is tartalmazhatnak.</span><span class="sxs-lookup"><span data-stu-id="79719-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="79719-117">Ez a probléma például akkor fordulhat elő, ha az en-US területi et nem használja.</span><span class="sxs-lookup"><span data-stu-id="79719-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="79719-118">Az egyeztetési fájlok formázási problémáinak megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="79719-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="79719-119">Nyissa meg az egyeztetési fájlt (.csv formátumban) a Microsoft Excelben.</span><span class="sxs-lookup"><span data-stu-id="79719-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="79719-120">Válassza ki a fájl első oszlopát.</span><span class="sxs-lookup"><span data-stu-id="79719-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="79719-121">Nyissa meg **a Szöveg átalakítása oszlopokká varázslót.**</span><span class="sxs-lookup"><span data-stu-id="79719-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="79719-122">A menüszalagon válassza az **Adatok** lehetőséget, majd a **Szövegből oszlopokba lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="79719-123">A varázslóban válassza a **Tagolt fájltípus lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="79719-124">Ezután válassza a **Tovább lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="79719-125">Az **Elválasztó mezőkben** válassza a **Vessző lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="79719-126">(Ha **a Tab** már ki van jelölve, ezt a beállítást hagyja bejelölve.) Ezután válassza a **Tovább lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="79719-127">Az Oszlop **adatformátuma mezőben** válassza a **Date:MDY lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="79719-128">Ezután válassza a **Tovább lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="79719-129">Az Oszlop **adatformátuma mezőben** válassza a **Szöveg lehetőséget** minden összegoszlophoz.</span><span class="sxs-lookup"><span data-stu-id="79719-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="79719-130">Ezután válassza a **Befejezés** gombot.</span><span class="sxs-lookup"><span data-stu-id="79719-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="79719-131">Egyeztetési fájlok letöltése programozott módon</span><span class="sxs-lookup"><span data-stu-id="79719-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="79719-132">Az egyeztetési fájlok nagyon nagy méretűek, és néha nehezen tölthetők le.</span><span class="sxs-lookup"><span data-stu-id="79719-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="79719-133">Az egyeztetési fájlok programozott letöltéséhez lásd: [Számlasorelemek betöltése.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="79719-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="79719-134">Ha a fájl túllépi a sorkorlátot az Excelben</span><span class="sxs-lookup"><span data-stu-id="79719-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="79719-135">Ha le tud tölteni egy egyeztetési fájlt, de nem nyitja meg a Microsoft Excelben, az valószínűleg azt jelenti, hogy a fájl több sort tartalmaz, mint amennyit az Excel engedélyez.</span><span class="sxs-lookup"><span data-stu-id="79719-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="79719-136">Ebben az esetben az alábbi eljárások bármelyikével megnyithatja a fájlt.</span><span class="sxs-lookup"><span data-stu-id="79719-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="79719-137">Nyisson meg egy recon fájlt a Power BI</span><span class="sxs-lookup"><span data-stu-id="79719-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="79719-138">Töltse le az egyeztetési fájlt a szokásos módon.</span><span class="sxs-lookup"><span data-stu-id="79719-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="79719-139">Töltse le, telepítse és nyissa meg a Microsoft Power BI.</span><span class="sxs-lookup"><span data-stu-id="79719-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="79719-140">A Power BI **lapon** válassza az Adatok **lekérte lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="79719-141">A Gyakori adatforrások **listájában válassza** a **Szöveg/CSV lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="79719-142">Amikor a rendszer kéri, nyissa meg a recon fájlt.</span><span class="sxs-lookup"><span data-stu-id="79719-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="79719-143">Felderítési fájl megnyitása Excel-kimutatástáblában</span><span class="sxs-lookup"><span data-stu-id="79719-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="79719-144">Töltse le az egyeztetési fájlt a szokásos módon.</span><span class="sxs-lookup"><span data-stu-id="79719-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="79719-145">Nyisson meg egy új fájlt a Microsoft Excelben.</span><span class="sxs-lookup"><span data-stu-id="79719-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="79719-146">Az Adatok **lapon** válassza az Adatok **lekérte** lehetőséget, válassza a **Fájlból,** majd a **Szöveg/CSV lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="79719-147">Amikor a rendszer kéri, nyissa meg a recon fájlt.</span><span class="sxs-lookup"><span data-stu-id="79719-147">When prompted, open your recon file.</span></span> <span data-ttu-id="79719-148">Megjelennek az adatok.</span><span class="sxs-lookup"><span data-stu-id="79719-148">Your data will appear.</span></span>
5. <span data-ttu-id="79719-149">A **Betöltés legördülő** menüben válassza **a** Betöltés ide, majd az **OK gombot.**</span><span class="sxs-lookup"><span data-stu-id="79719-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="79719-150">Az Adatok **importálása párbeszédpanelen** válassza a **Kimutatás jelentés lehetőséget** a fájl megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="79719-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="79719-151">Megjelenített negatív összeg</span><span class="sxs-lookup"><span data-stu-id="79719-151">Negative amount displayed</span></span>

<span data-ttu-id="79719-152">Előfordulhat, hogy negatív összeget lát az egyeztetési fájlban.</span><span class="sxs-lookup"><span data-stu-id="79719-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="79719-153">Ezt valószínűleg az alábbiak valamelyike okozza:</span><span class="sxs-lookup"><span data-stu-id="79719-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="79719-154">Nemrég lemondta vagy csökkentette a licencek számát</span><span class="sxs-lookup"><span data-stu-id="79719-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="79719-155">Jóváírást kapott egy szolgáltatáslicenc-szerződés (SLA) vagy az Azure-használat alapján</span><span class="sxs-lookup"><span data-stu-id="79719-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="79719-156">Ha további információt szeretne kapni erről a tranzakcióról, tekintse meg a díjtípus attribútumát az egyeztetési fájlban.</span><span class="sxs-lookup"><span data-stu-id="79719-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="79719-157">Adó- vagy áfaleképés térképe</span><span class="sxs-lookup"><span data-stu-id="79719-157">Map taxes or VAT</span></span>

<span data-ttu-id="79719-158">Adó- vagy értékadó (ÁFA) leképezése a számlára:</span><span class="sxs-lookup"><span data-stu-id="79719-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="79719-159">Összegezve **a licencalapú** fájl Adó oszlopát.</span><span class="sxs-lookup"><span data-stu-id="79719-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="79719-160">Összegezve **a TaxAmount oszlopot** a használatalapú fájlból.</span><span class="sxs-lookup"><span data-stu-id="79719-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="79719-161">Egyeztetési fájlok elemet ad meg partner szerint</span><span class="sxs-lookup"><span data-stu-id="79719-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="79719-162">A közvetett **modellben lévő partnerek** ezeket a további mezőket licencalapú és használatalapú egyeztetési fájlokban is felhasználhatjak a fájlok viszonteladó szerint való elemztetéséhez.</span><span class="sxs-lookup"><span data-stu-id="79719-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="79719-163">MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="79719-163">MPN ID</span></span> | <span data-ttu-id="79719-164">Leírás</span><span class="sxs-lookup"><span data-stu-id="79719-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="79719-165">MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="79719-165">MPN ID</span></span> | <span data-ttu-id="79719-166">A Microsoft Partner Network (közvetlen vagy közvetett) partner Felhőszolgáltató (MPN) azonosítója.</span><span class="sxs-lookup"><span data-stu-id="79719-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="79719-167">Viszonteladói MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="79719-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="79719-168">Az [előfizetés rekordjának viszonteladójának MPN-azonosítója.](#reseller-mpn-id)</span><span class="sxs-lookup"><span data-stu-id="79719-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="79719-169">Ez a mező az adott előfizetéshez felsorolt viszonteladói azonosítónak felel meg a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="79719-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="79719-170">Csak a közvetett modellben lévő partnerek egyeztetési fájljaiban jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="79719-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="79719-171">Viszonteladói MPN-azonosító</span><span class="sxs-lookup"><span data-stu-id="79719-171">Reseller MPN ID</span></span>

<span data-ttu-id="79719-172">Ha egy CSP-partner közvetlenül az ügyfélnek adta el az előfizetést, az **MPN-azonosítója** kétszer lesz listázva, mind **MPN-azonosítóként,** mind **viszonteladói MPN-azonosítóként.**</span><span class="sxs-lookup"><span data-stu-id="79719-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="79719-173">Ha egy CSP-partner egy **MPN-azonosítóval** nem rendelkezik viszonteladóval, akkor ez az érték a partner **MPN-azonosítójára van beállítva.**</span><span class="sxs-lookup"><span data-stu-id="79719-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="79719-174">Ha a CSP-partner eltávolít egy **viszonteladói MPN-azonosítót,** ez az érték *-1* lesz.</span><span class="sxs-lookup"><span data-stu-id="79719-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="79719-175">A Viszonteladói **MPN-azonosító megtekintése** vagy frissítése:</span><span class="sxs-lookup"><span data-stu-id="79719-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="79719-176">Jelentkezzen be a Partnerközpontba.</span><span class="sxs-lookup"><span data-stu-id="79719-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="79719-177">A Partnerközpont válassza az Ügyfelek **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="79719-178">Válassza ki az ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="79719-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="79719-179">Az ügyfélmenüben válassza az **Előfizetések lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="79719-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="79719-180">Válassza ki az előfizetést a listából.</span><span class="sxs-lookup"><span data-stu-id="79719-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="79719-181">Válassza **a Frissítés** lehetőséget a viszonteladó **(MPN-azonosító) módosításhoz.**</span><span class="sxs-lookup"><span data-stu-id="79719-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="79719-182">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="79719-182">Next steps</span></span>

- [<span data-ttu-id="79719-183">A számla olvasása & recon fájlban</span><span class="sxs-lookup"><span data-stu-id="79719-183">How to read your bill & recon file</span></span>](read-your-bill.md) 