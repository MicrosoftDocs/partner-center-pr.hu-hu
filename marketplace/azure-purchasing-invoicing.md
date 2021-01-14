---
title: Szoftverek és megoldások vásárlása az Azure Marketplace-ről
description: Ismerje meg azokat az eszközöket, amelyek egyszerűbbé és egyszerűbbé teszik a szoftverek vásárlását és felügyeletét az Azure Marketplace-en.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 8f7962b1b040be90f7dc1b2696a2ced3830d25b9
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182477"
---
# <a name="azure-marketplace-purchasing"></a><span data-ttu-id="0c88f-103">Az Azure Marketplace megvásárlása</span><span class="sxs-lookup"><span data-stu-id="0c88f-103">Azure Marketplace purchasing</span></span>

<span data-ttu-id="0c88f-104">Az Azure Marketplace számos olyan eszközzel és funkcióval rendelkezik, amely egyszerűbbé és egyszerűbbé teszi a vásárlási házirend megvásárlását, számlázását és kezelését.</span><span class="sxs-lookup"><span data-stu-id="0c88f-104">Azure Marketplace has numerous tools and features that simplify and streamline the process of purchasing, invoicing, and managing purchasing policy.</span></span>

## <a name="simplified-procurement"></a><span data-ttu-id="0c88f-105">Egyszerűsített beszerzés</span><span class="sxs-lookup"><span data-stu-id="0c88f-105">Simplified procurement</span></span>

<span data-ttu-id="0c88f-106">Az Azure Marketplace-en különböző vásárlási lehetőségek állnak rendelkezésére, amelyekkel leegyszerűsítheti a beszerzési folyamatot.</span><span class="sxs-lookup"><span data-stu-id="0c88f-106">Azure Marketplace helps you simplify the procurement process through different purchasing options.</span></span> <span data-ttu-id="0c88f-107">Ha az Azure-fiókjához társított bankkártyát használ, az összes vásárlás konszolidálva lesz egyetlen számlán, és a választott bankkártyára kerül.</span><span class="sxs-lookup"><span data-stu-id="0c88f-107">If you purchase products using a credit card associated with your Azure account, all purchases will be consolidated on a single invoice and billed to the credit card of choice.</span></span> <span data-ttu-id="0c88f-108">Ha Ön nagy ügyfél, megvásárolhatja Nagyvállalati Szerződés használatával.</span><span class="sxs-lookup"><span data-stu-id="0c88f-108">If you are a large customer, you can purchase using an Enterprise Agreement.</span></span> <span data-ttu-id="0c88f-109">A nagyvállalati szerződéssel rendelkező szoftvereket a rendszer automatikusan felveszi az Azure-számlába.</span><span class="sxs-lookup"><span data-stu-id="0c88f-109">With an EA, any software purchases are automatically included in your Azure invoice.</span></span> <span data-ttu-id="0c88f-110">A számla elején az Azure használati díjai jelennek meg, amelyeket az Azure Marketplace díjai követnek.</span><span class="sxs-lookup"><span data-stu-id="0c88f-110">Your invoice will contain Azure usage charges first, followed by Azure Marketplace charges.</span></span>

<span data-ttu-id="0c88f-111">Az Azure Marketplace-en való vásárlás során nem kell az egyes szállítói kapcsolatok és számlák kezelésének összetettségét kizárni.</span><span class="sxs-lookup"><span data-stu-id="0c88f-111">When you purchase through Azure Marketplace, you eliminate the complexity of managing individual vendor relationships and invoices.</span></span> <span data-ttu-id="0c88f-112">A Microsoft egyetlen, összevont havi számlát kap, amely az Azure Marketplace-vásárlásokat és az Azure-díjakat is tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="0c88f-112">You get a single, consolidated monthly bill from Microsoft that includes both your Azure Marketplace purchases and your Azure charges.</span></span>

## <a name="permission-to-purchase"></a><span data-ttu-id="0c88f-113">A vásárláshoz szükséges engedély</span><span class="sxs-lookup"><span data-stu-id="0c88f-113">Permission to purchase</span></span>

<span data-ttu-id="0c88f-114">Miután megtalálta a megfelelő szoftvert, a vásárlás befejezése egyszerű.</span><span class="sxs-lookup"><span data-stu-id="0c88f-114">After you've found the right software application, completing the purchase is simple.</span></span> <span data-ttu-id="0c88f-115">Az Azure-előfizetésben azonban megfelelő engedélyekkel kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="0c88f-115">You will, however, need suitable permissions within the Azure subscription.</span></span> <span data-ttu-id="0c88f-116">Mivel az Azure [szerepköralapú Access Control](/azure/role-based-access-control/overview) (RBAC) modellen működik, a fióknak **előfizetés-tulajdonosi** vagy **közreműködői** engedélyekkel kell rendelkeznie a vásárláshoz.</span><span class="sxs-lookup"><span data-stu-id="0c88f-116">Since Azure operates on a [Role Based Access Control](/azure/role-based-access-control/overview) (RBAC) model, your account needs **subscription owner** or **contributor** permissions to make a purchase.</span></span>

<span data-ttu-id="0c88f-117">A vásárlás befejezése előtt ellenőrizze, hogy a felhasználó rendelkezik-e a megfelelő konfigurációval az Azure-bérlőben.</span><span class="sxs-lookup"><span data-stu-id="0c88f-117">Before completing a purchase, make sure the user has the correct configuration in the Azure tenant.</span></span> <span data-ttu-id="0c88f-118">Ez segít megelőzni a hibák megvásárlását.</span><span class="sxs-lookup"><span data-stu-id="0c88f-118">This will help prevent errors during purchase.</span></span>

<span data-ttu-id="0c88f-119">Az Azure Marketplace-en a Azure Portalban keresse meg a megvásárolni kívánt alkalmazást, majd válassza a **Létrehozás** vagy **beállítás + előfizetés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0c88f-119">In the Azure Marketplace experience in the Azure portal, find the application you want to buy and select **Create** or **Set up + subscribe**.</span></span> <span data-ttu-id="0c88f-120">A rendszer kérni fogja, hogy az új megoldás használata előtt végezzen el néhány információt.</span><span class="sxs-lookup"><span data-stu-id="0c88f-120">You'll be prompted to complete some information before being able to use your new solution.</span></span>

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Az ajánlat létrehozása gomb.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="A beállítás + előfizetés gomb.":::

<span data-ttu-id="0c88f-123">Ha az Azure Marketplace online áruházból szeretne megoldást telepíteni, válassza a **Letöltés most** lehetőséget a termékleírás lapon, majd jelentkezzen be az Azure-fiókja hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="0c88f-123">If you want to deploy a solution from the Azure Marketplace online store, select **Get it now** on the product description page and then sign in with your Azure account credentials.</span></span>

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Az Azure Marketplace bejelentkezési párbeszédpanelje.":::

<span data-ttu-id="0c88f-125">A bejelentkezés után a rendszer átirányítja a termékre a Azure Portal a vásárlás befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="0c88f-125">Once you sign in, you will be redirected to the product in the Azure portal to complete your purchase.</span></span>

## <a name="purchase-policy-management"></a><span data-ttu-id="0c88f-126">A házirend-kezelés megvásárlása</span><span class="sxs-lookup"><span data-stu-id="0c88f-126">Purchase policy management</span></span>

<span data-ttu-id="0c88f-127">A Microsoft lehetővé teszi a felhasználói vásárlások kezelését a számlázási profilon keresztül az Azure-előfizetés rendszergazdájaként.</span><span class="sxs-lookup"><span data-stu-id="0c88f-127">Microsoft lets you manage user purchases through your billing profile as the Azure subscription administrator.</span></span> <span data-ttu-id="0c88f-128">Három lehetőség közül választhat:</span><span class="sxs-lookup"><span data-stu-id="0c88f-128">Choose from three options:</span></span>

- <span data-ttu-id="0c88f-129">**Ingyenes és fizetős** – lehetővé teszi, hogy a felhasználók bármilyen Azure Marketplace-alkalmazást szerezzenek be.</span><span class="sxs-lookup"><span data-stu-id="0c88f-129">**Free + Paid** – Allows users to acquire any Azure Marketplace software application.</span></span>
- <span data-ttu-id="0c88f-130">**Ingyenes** – lehetővé teszi a felhasználók számára, hogy csak az Azure piactéren telepítsenek ingyenes szoftvereket.</span><span class="sxs-lookup"><span data-stu-id="0c88f-130">**Free** – Allows users to deploy only free software from Azure Marketplace.</span></span>
- <span data-ttu-id="0c88f-131">**Nem** – megakadályozza, hogy a felhasználók szoftvert telepítsenek az Azure piactéren.</span><span class="sxs-lookup"><span data-stu-id="0c88f-131">**No** – Prevents users from deploying any software from Azure Marketplace.</span></span>

<span data-ttu-id="0c88f-132">Ezek a beállítások az Azure-előfizetéshez hozzáféréssel rendelkező összes felhasználóra érvényesek, amely lehetővé teszi az IT-beszerzések vezérlését a Azure Portalon keresztül.</span><span class="sxs-lookup"><span data-stu-id="0c88f-132">These settings apply to all users with access to your Azure subscription, which gives you the capability to control IT procurement through the Azure portal.</span></span>

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Az informatikai beszerzések szabályozása a Azure Portal":::

## <a name="cost-management"></a><span data-ttu-id="0c88f-134">Cost Management</span><span class="sxs-lookup"><span data-stu-id="0c88f-134">Cost management</span></span>

<span data-ttu-id="0c88f-135">Az Azure Marketplace-en vásárolt termékekhez olyan bepillantást szeretne kapni, amelyek segítenek a költségek kezelésében.</span><span class="sxs-lookup"><span data-stu-id="0c88f-135">As you purchase products from Azure Marketplace, you want to get insights that help you manage costs.</span></span> <span data-ttu-id="0c88f-136">Azure Cost Management a megvásárolt termékekkel kapcsolatos információk megtekintésére szolgáló ingyenes eszköz.</span><span class="sxs-lookup"><span data-stu-id="0c88f-136">Azure Cost Management is a free tool for viewing information on the products you've purchased.</span></span> <span data-ttu-id="0c88f-137">A Cost Management használatával megtekintheti, hogy milyen szolgáltatásokra költ pénzt, és hogyan követheti nyomon ezeket a költségeket a beállított költségkeretek alapján.</span><span class="sxs-lookup"><span data-stu-id="0c88f-137">You can use Cost Management to see details of what services you're spending money on over time and how those costs track against the budgets you've set.</span></span> <span data-ttu-id="0c88f-138">A költségvetések beállítása mellett a jelentések is ütemezhetők, és az előfizetési költségek is elemezhetők.</span><span class="sxs-lookup"><span data-stu-id="0c88f-138">In addition to setting budgets, you can schedule reports and analyze subscription costs.</span></span> <span data-ttu-id="0c88f-139">További információ a Azure Cost Managementről: a Microsoft Learn modul [elemzése a költségek elemzéséhez és a költségvetések létrehozása Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)használatával.</span><span class="sxs-lookup"><span data-stu-id="0c88f-139">Learn more about Azure Cost Management by completing the Microsoft Learn module on [Analyze costs and create budgets with Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).</span></span>

<span data-ttu-id="0c88f-140">Az Azure Cost Management költségelemző eszközével megtekintheti az Azure Marketplace-díjakat és a számlákat.</span><span class="sxs-lookup"><span data-stu-id="0c88f-140">You can view your Azure Marketplace charges and invoices on the cost analysis tool under Azure Cost Management.</span></span>

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="A Azure Cost Management használatával betekintést nyerhet a megvásárolt termékekbe.":::

## <a name="next-steps"></a><span data-ttu-id="0c88f-142">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="0c88f-142">Next steps</span></span>

- [<span data-ttu-id="0c88f-143">Számlázás és számlakiállítás</span><span class="sxs-lookup"><span data-stu-id="0c88f-143">Billing and invoicing</span></span>](billing-invoicing.md)