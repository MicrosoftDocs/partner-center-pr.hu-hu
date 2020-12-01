---
title: Azure-kiadások költségkeretének beállítása az ügyfelek számára
ms.topic: how-to
ms.date: 06/03/2020
description: Megtudhatja, hogyan állíthatja be vagy távolíthatja el az ügyfelek havi Azure-költségkeretét, valamint megtekintheti az Azure-kiadások adatait, és megadhatja a költségvetéssel kapcsolatos értesítéseket is.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e311af31bbce65ed38c20df12243d325c7a63d04
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/01/2020
ms.locfileid: "96438980"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="1421c-103">A partner Center ügyfelei számára havi Azure-költségkeretek beállítása, bejelölése vagy eltávolítása</span><span class="sxs-lookup"><span data-stu-id="1421c-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="1421c-104">A következőkre vonatkozik:</span><span class="sxs-lookup"><span data-stu-id="1421c-104">Applies to:</span></span>

- <span data-ttu-id="1421c-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="1421c-105">Partner Center</span></span>
- <span data-ttu-id="1421c-106">A Microsoft Cloud for US Government Partnerközpontja</span><span class="sxs-lookup"><span data-stu-id="1421c-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="1421c-107">Megadhatja a partner Center [ügyfeleinek havi Azure-költségkeretét](#set-azure-spending-budget) .</span><span class="sxs-lookup"><span data-stu-id="1421c-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="1421c-108">Ez segít az ügyfeleknek az Azure-kiadások kezelésében.</span><span class="sxs-lookup"><span data-stu-id="1421c-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="1421c-109">Ez a beállítás lehetővé teszi, hogy az ügyfelek Azure-kiadásait a hónap folyamán összehasonlítsa a költségvetésbe.</span><span class="sxs-lookup"><span data-stu-id="1421c-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="1421c-110">Emellett az ügyfelek számára is lehetővé teszi az Azure-kiadások költségvetését, így a havi számla nem nagyobb, mint amennyire várható.</span><span class="sxs-lookup"><span data-stu-id="1421c-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="1421c-111">Ez a funkció nem érhető el a homokozóban vagy a tesztelés éles (TIP) fiókokban.</span><span class="sxs-lookup"><span data-stu-id="1421c-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="1421c-112">Miután [beállította az Azure-költségkeretet az ügyfél (ek) számára](#set-azure-spending-budget), a következő módokon tekintheti át az ügyfelek használatát.</span><span class="sxs-lookup"><span data-stu-id="1421c-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="1421c-113">Ezek a lehetőségek segíthetnek a helytelenül konfigurált szolgáltatások vagy szokatlan, csalást okozó trendek felderítésében.</span><span class="sxs-lookup"><span data-stu-id="1421c-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="1421c-114">Ezután a felhasználó (k) használatával azonosíthatja a kiváltó okot, és kezelheti a költségeket.</span><span class="sxs-lookup"><span data-stu-id="1421c-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="1421c-115">Ha szükséges, [az ügyfél költségvetését is megváltoztathatja](#set-azure-spending-budget) magasabb értékre.</span><span class="sxs-lookup"><span data-stu-id="1421c-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="1421c-116">Aktuális Azure-kiadások keresése</span><span class="sxs-lookup"><span data-stu-id="1421c-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="1421c-117">E-mail-értesítések bekapcsolása, ha az ügyfél kiadásai közel vannak a költségvetési korláthoz</span><span class="sxs-lookup"><span data-stu-id="1421c-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="1421c-118">Részletezett költségek megtekintése szolgáltatás alapján a használaton alapuló előfizetésekhez</span><span class="sxs-lookup"><span data-stu-id="1421c-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="1421c-119">Az Azure- [költségkeretet bármikor el is távolíthatja](#remove-azure-spending-budget) az ügyfelekhez.</span><span class="sxs-lookup"><span data-stu-id="1421c-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="1421c-120">Az Azure kiadásai</span><span class="sxs-lookup"><span data-stu-id="1421c-120">Azure spending data</span></span>

<span data-ttu-id="1421c-121">Az Azure-kiadási adatok *becsültek* , a *tényleges számlázási összegek pedig eltérőek lehetnek*.</span><span class="sxs-lookup"><span data-stu-id="1421c-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="1421c-122">Az adatok értéke *nem tükrözi* az adókat, a krediteket, a beállításokat és az esetlegesen alkalmazandó egyéb díjakat.</span><span class="sxs-lookup"><span data-stu-id="1421c-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="1421c-123">A kiadási adat *naponta egyszer frissül*.</span><span class="sxs-lookup"><span data-stu-id="1421c-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="1421c-124">Az ügyfelek továbbra is használhatják az Azure-szolgáltatások és-erőforrások használatát (és díjat számítanak fel), hacsak nem módosítja a fiók beállításait a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="1421c-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="1421c-125">Az Azure-kiadások költségvetésének beállítása</span><span class="sxs-lookup"><span data-stu-id="1421c-125">Set Azure spending budget</span></span>

<span data-ttu-id="1421c-126">A partner Centerben több ügyfél számára is *beállíthat havi Azure-költségkeretet* :</span><span class="sxs-lookup"><span data-stu-id="1421c-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="1421c-127">Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="1421c-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="1421c-128">A bal oldali menü **CSP** területén válassza az Azure- **kiadások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1421c-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="1421c-129">Az **Azure-kiadások** oldalon Microsoft Azure- **előfizetéssel rendelkező ügyfelek** területen válassza ki azokat az ügyfeleket, akik számára költségvetést kíván beállítani.</span><span class="sxs-lookup"><span data-stu-id="1421c-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="1421c-130">Adja meg a **havi költségkeret** értékét.</span><span class="sxs-lookup"><span data-stu-id="1421c-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="1421c-131">A módosítások mentéséhez kattintson az **alkalmaz** gombra.</span><span class="sxs-lookup"><span data-stu-id="1421c-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="1421c-132">Megadhat *egy költségvetést is egy egyéni ügyfél* számára az előfizetési beállításokban:</span><span class="sxs-lookup"><span data-stu-id="1421c-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="1421c-133">Jelentkezzen be a partner Center irányítópultra.</span><span class="sxs-lookup"><span data-stu-id="1421c-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="1421c-134">A bal oldali menüben a **CSP** területen válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1421c-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="1421c-135">Az **ügyfelek** lapon válassza ki az ügyfél **vállalatának nevét**.</span><span class="sxs-lookup"><span data-stu-id="1421c-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="1421c-136">Az ügyfél **előfizetések** lapján, a **használaton alapuló előfizetés** területen válassza a **költségvetés módosítása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1421c-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="1421c-137">Adja meg a költségvetés értékét.</span><span class="sxs-lookup"><span data-stu-id="1421c-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="1421c-138">A módosítások mentéséhez kattintson az **alkalmaz** gombra.</span><span class="sxs-lookup"><span data-stu-id="1421c-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="1421c-139">Az Azure-kiadások költségvetésének eltávolítása</span><span class="sxs-lookup"><span data-stu-id="1421c-139">Remove Azure spending budget</span></span>

<span data-ttu-id="1421c-140">A partner Centerben a következő *havi Azure-költségkeretet távolíthatja el* ügyfeleinek:</span><span class="sxs-lookup"><span data-stu-id="1421c-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="1421c-141">Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="1421c-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="1421c-142">A bal oldali menü **CSP** területén válassza az Azure- **kiadások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1421c-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="1421c-143">Az **Azure-kiadások** oldalon Microsoft Azure- **előfizetéssel rendelkező ügyfelek** területen válassza ki azokat az ügyfeleket, akiknek a költségvetését el szeretné távolítani.</span><span class="sxs-lookup"><span data-stu-id="1421c-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="1421c-144">Válassza a **költségvetés eltávolítása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1421c-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="1421c-145">Aktuális Azure-kiadások keresése</span><span class="sxs-lookup"><span data-stu-id="1421c-145">Check current Azure spending</span></span>

<span data-ttu-id="1421c-146">*Az ügyfelek aktuális Azure-kiadásait és havi költségkereteit bármikor nyomon követheti* :</span><span class="sxs-lookup"><span data-stu-id="1421c-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="1421c-147">Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="1421c-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="1421c-148">A bal oldali menü **CSP** területén válassza az Azure- **kiadások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1421c-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="1421c-149">Az **Azure-kiadások** oldalon Microsoft Azure- **előfizetéssel rendelkező ügyfeleknél** tekintse meg az ügyfelek havi költségkeretét, a jelenlegi kiadási becsléseket és a felhasznált költségvetés százalékos arányát.</span><span class="sxs-lookup"><span data-stu-id="1421c-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="1421c-150">A költségvetési korlátokkal kapcsolatos értesítések</span><span class="sxs-lookup"><span data-stu-id="1421c-150">Notifications for budget limits</span></span>

<span data-ttu-id="1421c-151">*Bekapcsolhatja az e-mailes értesítéseket* , amikor az ügyfél havi kiadásai elérik a költségvetési korlátot.</span><span class="sxs-lookup"><span data-stu-id="1421c-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="1421c-152">Ha bekapcsolja ezt a beállítást, a rendszer értesítést küld, ha az ügyfelek a havi költségkeretük 80%-át használják.</span><span class="sxs-lookup"><span data-stu-id="1421c-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="1421c-153">Ez a beállítás segít megőrizni az Azure-számlázást.</span><span class="sxs-lookup"><span data-stu-id="1421c-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="1421c-154">E-mail-értesítések konfigurálása:</span><span class="sxs-lookup"><span data-stu-id="1421c-154">To configure email notifications:</span></span>

1. <span data-ttu-id="1421c-155">Jelentkezzen be a Partnerközpontba.</span><span class="sxs-lookup"><span data-stu-id="1421c-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="1421c-156">Válassza a **Beállítások lehetőséget**.</span><span class="sxs-lookup"><span data-stu-id="1421c-156">Go to **Settings**.</span></span>

3. <span data-ttu-id="1421c-157">Válassza **a saját beállítások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1421c-157">Select **My preferences**.</span></span>

4. <span data-ttu-id="1421c-158">Ha még nem tette meg, konfiguráljon egy előnyben részesített e-mail címet.</span><span class="sxs-lookup"><span data-stu-id="1421c-158">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="1421c-159">Adja meg az értesítéshez használni kívánt nyelvet.</span><span class="sxs-lookup"><span data-stu-id="1421c-159">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="1421c-160">Válassza a **CSP** fület az **értesítési beállítások** szakaszban.</span><span class="sxs-lookup"><span data-stu-id="1421c-160">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="1421c-161">Keresse meg az Azure- **kiadások** értesítése e-mailben lehetőséget, és **mentse** a következőt:.</span><span class="sxs-lookup"><span data-stu-id="1421c-161">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="1421c-162">Kitételi költségek szolgáltatás szerint</span><span class="sxs-lookup"><span data-stu-id="1421c-162">Itemized costs by service</span></span>

<span data-ttu-id="1421c-163">*A tételes költségeket (és a becsült használatot) a szolgáltatás alapján, a használaton alapuló előfizetések esetében tekintheti* meg:</span><span class="sxs-lookup"><span data-stu-id="1421c-163">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="1421c-164">Jelentkezzen be a Partnerközpontba.</span><span class="sxs-lookup"><span data-stu-id="1421c-164">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="1421c-165">A bal oldali menüben a **CSP** területen válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1421c-165">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="1421c-166">Az **ügyfelek** lapon válassza ki az ügyfél **vállalatának nevét**.</span><span class="sxs-lookup"><span data-stu-id="1421c-166">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="1421c-167">Az ügyfél **előfizetések** lapján, a **használat alapú előfizetések** területen válassza ki az **előfizetés** nevét.</span><span class="sxs-lookup"><span data-stu-id="1421c-167">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="1421c-168">Az előfizetés lapján áttekintheti a **részletezett költségeket** a szolgáltatás alapján, valamint az aktuális hónap **becsült felhasználását** .</span><span class="sxs-lookup"><span data-stu-id="1421c-168">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
