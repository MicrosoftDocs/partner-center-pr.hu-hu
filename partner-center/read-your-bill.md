---
title: A Bill & Recon-fájl beolvasása
ms.topic: article
ms.date: 06/05/2020
description: További információ a számla & egyeztetési fájlokról. A számlán az adott havi időszakra vonatkozó, a programon, a termékeken és az ügyfeleknek felszámított partneri költségek szerepelnek.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 43c2605d750d35bc2e0095b1fed413ed91a1a28e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215815"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a><span data-ttu-id="34355-104">A számla és a megbékélési fájl megismerése – Ismerje meg, hogyan keresheti meg őket a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="34355-104">Understand your bill and reconciliation file - learn how to find them in Partner Center</span></span>


<span data-ttu-id="34355-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="34355-105">**Appropriate roles**</span></span>

- <span data-ttu-id="34355-106">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="34355-106">Global admin</span></span>
- <span data-ttu-id="34355-107">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="34355-107">Billing admin</span></span>
- <span data-ttu-id="34355-108">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="34355-108">Admin agent</span></span>


<span data-ttu-id="34355-109">A **számla** az **összes partner Center-díj** (a program, az összes termék és minden ügyfél) összefoglalása.</span><span class="sxs-lookup"><span data-stu-id="34355-109">Your **invoice** is a **summary of all your Partner Center charges** (across the program, all products, and all customers).</span></span> 

## <a name="invoice-types"></a><span data-ttu-id="34355-110">Számlák típusai</span><span class="sxs-lookup"><span data-stu-id="34355-110">Invoice types</span></span>

<span data-ttu-id="34355-111">A Microsoft egy számlát ad ki a licenc-alapú díjak (például az Office 365) és a használati díjak (például az Azure) számára, valamint egy külön számlát az egyszeri költségek (például az Azure RI, a piactér vagy az Azure-csomag) számára.</span><span class="sxs-lookup"><span data-stu-id="34355-111">Microsoft will issue one invoice for any license-based charges (such as Office 365) and usage-based charges (such as Azure) and a separate invoice for one-time charges (such as Azure RI, Marketplace, or Azure plan).</span></span>

<span data-ttu-id="34355-112">Példa:</span><span class="sxs-lookup"><span data-stu-id="34355-112">For example,</span></span>  

<span data-ttu-id="34355-113">**1. forgatókönyv [egyetlen pénznem]**: a partner 145P-ajánlatokat és O365-licenceket vásárol,</span><span class="sxs-lookup"><span data-stu-id="34355-113">**Scenario 1 [Single Currency]**: Partner has purchases for 145P offer and O365 licenses,</span></span>  

- <span data-ttu-id="34355-114">A partner egy számla PDF és 2 egyeztetési fájlt kap, amely a O365 és az Azure (145p) díjait is tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="34355-114">Partner will get one invoice PDF and 2 reconciliation files covering the charges for both O365 and Azure (145p).</span></span>  

<span data-ttu-id="34355-115">**2. forgatókönyv [egyetlen pénznem]**: a partner az Azure RI, a piactér és/vagy az Azure-csomag megvásárlásával, valamint a 145p-vásárlásokkal is rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="34355-115">**Scenario 2 [Single Currency]**: Partner has purchases for Azure RI, Marketplace and/or Azure plan along with 145p purchases.</span></span>

- <span data-ttu-id="34355-116">A partner egy számla PDF-fájlját és egy egyeztetési fájlt kap, amely az Azure (145p) díjait tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="34355-116">Partner will get one invoice PDF and a reconciliation file covering the charges for Azure (145p).</span></span> 

- <span data-ttu-id="34355-117">A partner egy másik számla PDF-fájlját és egy egyeztető fájlt fog kapni, amely az Azure RI, a piactér és az Azure-csomag díjaira vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="34355-117">Partner will receive another invoice PDF and a reconciliation file covering their charges for Azure RI, Marketplace, Azure plan.</span></span> 

<span data-ttu-id="34355-118">**3. forgatókönyv [többszörös pénznem]**: a partner az Azure ri-t a DKK-ben és az Azure-ban, a 145p-vásárlások esetében pedig euróban vásárolja meg.</span><span class="sxs-lookup"><span data-stu-id="34355-118">**Scenario 3 [Multi-Currency]**: Partner has purchases for Azure RI in DKK and Azure plan in EUR along with 145p purchases in EUR.</span></span>

- <span data-ttu-id="34355-119">A partner egy számla PDF-fájlját és egy egyeztető fájlt fog kapni, amely a DKK-ban található Azure RI díját tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="34355-119">Partner will receive one invoice PDF and a reconciliation file covering the charges for Azure RI in DKK.</span></span> 

- <span data-ttu-id="34355-120">A partner egyetlen számla PDF-fájlját és egy egyeztető fájlt kap, amely az Azure-csomag díjait tartalmazza EUR-ban.</span><span class="sxs-lookup"><span data-stu-id="34355-120">Partner will receive one invoice PDF and a reconciliation file covering the charges for Azure plan in EUR.</span></span> 

- <span data-ttu-id="34355-121">A partner egy másik számla PDF-fájlját és egy egyeztetési fájlt fog kapni, amely az 145p ajánlat díjait (vagy a partner számlázási pénznemét) tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="34355-121">Partner will receive another invoice PDF and a reconciliation file covering their charges for 145p offer in EUR (or partner billing currency).</span></span> 

## <a name="find-your-bill"></a><span data-ttu-id="34355-122">Számla megkeresése</span><span class="sxs-lookup"><span data-stu-id="34355-122">Find your bill</span></span> 

<span data-ttu-id="34355-123">A számla a partner Center irányítópultjának számlázási lapján található.</span><span class="sxs-lookup"><span data-stu-id="34355-123">You can find your invoice on the Billing page of the dashboard in Partner Center.</span></span> <span data-ttu-id="34355-124">Ezen a lapon megtekintheti a számlázási előzményeit, a kiadások trendjét és a fájlok egyeztetését.</span><span class="sxs-lookup"><span data-stu-id="34355-124">You can also find your billing history, spending trends, and reconciliation files on this page.</span></span> 

1. <span data-ttu-id="34355-125">Jelentkezzen be a Partnerközpont [irányítópultjába](https://partner.microsoft.com/dashboard/home).</span><span class="sxs-lookup"><span data-stu-id="34355-125">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span> 

2. <span data-ttu-id="34355-126">A bal oldali menüben válassza a **számlázás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="34355-126">In the left-hand menu, select **Billing**.</span></span> 

3. <span data-ttu-id="34355-127">A számlázás lapon válassza ki a letölteni kívánt számlát.</span><span class="sxs-lookup"><span data-stu-id="34355-127">On the Billing page, select the invoice you want to download.</span></span> 

<span data-ttu-id="34355-128">Az oldal tetején található utolsó számlára mutató hivatkozást a számla egyenlege a legutóbbi számlázási dátum alapján lehetőségre kattintva találja.</span><span class="sxs-lookup"><span data-stu-id="34355-128">You can find a link to your latest invoice at the top of the page under Account balance as of last invoice date.</span></span> 

<span data-ttu-id="34355-129">A korábbi számlákat a számlázási előzmények szakaszban találja.</span><span class="sxs-lookup"><span data-stu-id="34355-129">You can find previous invoices in the Billing history section.</span></span> <span data-ttu-id="34355-130">Válassza ki a megfelelő évet, majd válassza a megfelelő számlázási időszak melletti legördülő nyilat.</span><span class="sxs-lookup"><span data-stu-id="34355-130">Choose the appropriate year, then select the drop-down arrow next to the appropriate Billing period.</span></span> <span data-ttu-id="34355-131">Válassza a számlák melletti hivatkozást (. pdf) az adott időszak számlájának letöltéséhez.</span><span class="sxs-lookup"><span data-stu-id="34355-131">Select the link next to Invoices (.pdf) to download that period's invoice.</span></span> 

## <a name="understanding-invoice-pdf"></a><span data-ttu-id="34355-132">A számla PDF-fájljának ismertetése</span><span class="sxs-lookup"><span data-stu-id="34355-132">Understanding invoice PDF</span></span> 

<span data-ttu-id="34355-133">**Használati és licenc-alapú díjakra vonatkozó számlák**: az Office 365-es és Azure-szolgáltatások díjainak számlázása két (2) napon belül elérhető lesz a kiválasztott számlázási dátum [UTC] alapján.</span><span class="sxs-lookup"><span data-stu-id="34355-133">**Invoices for Usage and license-based charges**: Invoices for charges for services such as Office 365 and Azure will be available within two (2) days of your selected billing date [UTC].</span></span>  

<span data-ttu-id="34355-134">**Egyszeri és ismétlődő díjakkal kapcsolatos számlák**: az Azure RI, az Azure-csomag és a piactér díjainak számlázása minden hónap 8. után lesz elérhető.</span><span class="sxs-lookup"><span data-stu-id="34355-134">**Invoices for onetime and recurring charges**: Invoices for charges for services such as Azure RI, Azure plan, Marketplace will be available not later than 8th of every month.</span></span>  

<span data-ttu-id="34355-135">Az alábbiakban a számla PDF-dokumentumának legfontosabb mezői találhatók:</span><span class="sxs-lookup"><span data-stu-id="34355-135">Below are some of the key fields on the Invoice PDF document –</span></span>

<span data-ttu-id="34355-136">**Számla száma**: a megfelelő számlázási időszakra vonatkozóan generált számla dokumentum egyedi azonosítója.</span><span class="sxs-lookup"><span data-stu-id="34355-136">**Invoice number**: Unique identifier for the invoice document generated for the respective billing period.</span></span> 

<span data-ttu-id="34355-137">**Számlázási időszak**: ez az az időszak, amely alatt a használati és a licenc-alapú szolgáltatásokat használhatja.</span><span class="sxs-lookup"><span data-stu-id="34355-137">**Billing period**: This is the period during which you have usages and license-based services.</span></span> 

<span data-ttu-id="34355-138">**Számla dátuma**: az a számlázási dátum vagy évfordulós dátum, amikor a számla generálása havonta történik.</span><span class="sxs-lookup"><span data-stu-id="34355-138">**Invoice date**: The billing date or anniversary date on which your invoice is generated each month.</span></span> 

<span data-ttu-id="34355-139">**Fizetési** határidő: az a dátum, ameddig a fizetést meg kell kapni.</span><span class="sxs-lookup"><span data-stu-id="34355-139">**Payment due date**: The date by which your payment must be received.</span></span> 

<span data-ttu-id="34355-140">**Díjak**: a megfelelő számlázási időszakra vonatkozó számlázási pénznemben esedékes összeg.</span><span class="sxs-lookup"><span data-stu-id="34355-140">**Charges**: The amount due in your billing currency for the respective billing period.</span></span> 

<span data-ttu-id="34355-141">**Kreditek**: kreditek (SLA) vagy az előfizetések módosításaira vonatkozó módosítások (például a licenc növekedése vagy csökkentése).</span><span class="sxs-lookup"><span data-stu-id="34355-141">**Credits**: Credits (such as SLA) or adjustments for changes made to subscriptions (for example, license increases or decreases).</span></span> 

<span data-ttu-id="34355-142">**Fizetési utasítások**: a számla fizetésének leírása a régió alapján.</span><span class="sxs-lookup"><span data-stu-id="34355-142">**Payment instructions**: Description of how to pay your invoice, based on your region.</span></span> <span data-ttu-id="34355-143">A számla számát mindig adja meg a fizetéskor.</span><span class="sxs-lookup"><span data-stu-id="34355-143">Always be sure to include your invoice number when making a payment.</span></span> 

<span data-ttu-id="34355-144">A számlázási fájlban lévő összes mező részletes ismertetését (beleértve az egyszeri költségekkel kapcsolatos mezőket is) lásd: [számlasorok mezői](invoice-file.md).</span><span class="sxs-lookup"><span data-stu-id="34355-144">For a detailed description of all the fields in your invoice file (including fields for one-time charges), see [Invoice file fields](invoice-file.md).</span></span> 

## <a name="understand-reconciliation-files"></a><span data-ttu-id="34355-145">Az egyeztetési fájlok ismertetése</span><span class="sxs-lookup"><span data-stu-id="34355-145">Understand reconciliation files</span></span>

 <span data-ttu-id="34355-146">Az egyeztetési fájlok, amelyek részletezik és részletezik a díjak részleteit, letölthetők a számla PDF-fájljával együtt.</span><span class="sxs-lookup"><span data-stu-id="34355-146">Reconciliation files, which provides a drill down/itemized details of your charges, are available to download along with the Invoice PDF.</span></span> <span data-ttu-id="34355-147">Az egyeztetési fájlok közé tartoznak az ügyfél-azonosítók és az előfizetés-azonosítók, amelyeket az ügyfél-számlák létrehozásához használhat.</span><span class="sxs-lookup"><span data-stu-id="34355-147">The reconciliation files include customer identifiers and subscription identifiers that you can use to create customer invoices.</span></span> <span data-ttu-id="34355-148">A felderítési fájlokkal kapcsolatos további részletekért tekintse meg az  [egyeztetési fájlok használatát ismertető](use-the-reconciliation-files.md) témakört.</span><span class="sxs-lookup"><span data-stu-id="34355-148">Please refer to  [How to use the reconciliation files](use-the-reconciliation-files.md) to get more details on the recon files.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="34355-149">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="34355-149">Next steps</span></span>

- [<span data-ttu-id="34355-150">A megbékélési fájlok használata</span><span class="sxs-lookup"><span data-stu-id="34355-150">How to use the reconciliation files</span></span>](use-the-reconciliation-files.md)