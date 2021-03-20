---
title: Azure-költségvetés beállítása az ügyfelek számára
ms.topic: how-to
ms.date: 03/17/2021
description: Megtudhatja, hogyan állíthatja be vagy távolíthatja el az ügyfelek havi Azure-költségkeretét, valamint megtekintheti az Azure-kiadások adatait, és megadhatja a költségvetéssel kapcsolatos értesítéseket is.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712749"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="7e464-103">A partner Center ügyfelei számára havi Azure-költségkeretek beállítása, bejelölése vagy eltávolítása</span><span class="sxs-lookup"><span data-stu-id="7e464-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="7e464-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="7e464-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7e464-105">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="7e464-105">Admin agent</span></span>

<span data-ttu-id="7e464-106">Megadhatja a partner Center [ügyfeleinek havi Azure-költségkeretét](#set-azure-spending-budget) .</span><span class="sxs-lookup"><span data-stu-id="7e464-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="7e464-107">Ez segít az ügyfeleknek az Azure-kiadások kezelésében.</span><span class="sxs-lookup"><span data-stu-id="7e464-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="7e464-108">Ez a beállítás lehetővé teszi, hogy az ügyfelek Azure-kiadásait a hónap folyamán összehasonlítsa a költségvetésbe.</span><span class="sxs-lookup"><span data-stu-id="7e464-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="7e464-109">Emellett az ügyfelek számára is lehetővé teszi az Azure-kiadások költségvetését, így a havi számla nem nagyobb, mint amennyire várható.</span><span class="sxs-lookup"><span data-stu-id="7e464-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="7e464-110">Ez a funkció nem érhető el a homokozóban vagy a tesztelés éles (TIP) fiókokban.</span><span class="sxs-lookup"><span data-stu-id="7e464-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="7e464-111">Miután [beállította az Azure-költségkeretet az ügyfél (ek) számára](#set-azure-spending-budget), a következő módokon tekintheti át az ügyfelek használatát.</span><span class="sxs-lookup"><span data-stu-id="7e464-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="7e464-112">Ezek a lehetőségek segíthetnek a helytelenül konfigurált szolgáltatások vagy szokatlan, csalást okozó trendek felderítésében.</span><span class="sxs-lookup"><span data-stu-id="7e464-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="7e464-113">Ezután a felhasználó (k) használatával azonosíthatja a kiváltó okot, és kezelheti a költségeket.</span><span class="sxs-lookup"><span data-stu-id="7e464-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="7e464-114">Ha szükséges, [az ügyfél költségvetését is megváltoztathatja](#set-azure-spending-budget) magasabb értékre.</span><span class="sxs-lookup"><span data-stu-id="7e464-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="7e464-115">Aktuális Azure-kiadások keresése</span><span class="sxs-lookup"><span data-stu-id="7e464-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="7e464-116">E-mail-értesítések bekapcsolása, ha az ügyfél kiadásai közel vannak a költségvetési korláthoz</span><span class="sxs-lookup"><span data-stu-id="7e464-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="7e464-117">Részletezett költségek megtekintése szolgáltatás alapján a használaton alapuló előfizetésekhez</span><span class="sxs-lookup"><span data-stu-id="7e464-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="7e464-118">Az Azure- [költségkeretet bármikor el is távolíthatja](#remove-azure-spending-budget) az ügyfelekhez.</span><span class="sxs-lookup"><span data-stu-id="7e464-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="7e464-119">Az Azure kiadásai</span><span class="sxs-lookup"><span data-stu-id="7e464-119">Azure spending data</span></span>

<span data-ttu-id="7e464-120">Az Azure-kiadási adatok *becsültek* , a *tényleges számlázási összegek pedig eltérőek lehetnek*.</span><span class="sxs-lookup"><span data-stu-id="7e464-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="7e464-121">Az adatok értéke *nem tükrözi* az adókat, a krediteket, a beállításokat és az esetlegesen alkalmazandó egyéb díjakat.</span><span class="sxs-lookup"><span data-stu-id="7e464-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="7e464-122">A kiadási adat *naponta egyszer frissül*.</span><span class="sxs-lookup"><span data-stu-id="7e464-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="7e464-123">Az ügyfelek továbbra is használhatják az Azure-szolgáltatások és-erőforrások használatát (és díjat számítanak fel), hacsak nem módosítja a fiók beállításait a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7e464-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="7e464-124">Az Azure-kiadások költségvetésének beállítása</span><span class="sxs-lookup"><span data-stu-id="7e464-124">Set Azure spending budget</span></span>

<span data-ttu-id="7e464-125">A partner Centerben több ügyfél számára is *beállíthat havi Azure-költségkeretet* :</span><span class="sxs-lookup"><span data-stu-id="7e464-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="7e464-126">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="7e464-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="7e464-127">A bal oldali menü **CSP** területén válassza az Azure- **kiadások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e464-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="7e464-128">Az **Azure-kiadások** oldalon Microsoft Azure- **előfizetéssel rendelkező ügyfelek** területen válassza ki azokat az ügyfeleket, akik számára költségvetést kíván beállítani.</span><span class="sxs-lookup"><span data-stu-id="7e464-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="7e464-129">Adja meg a **havi költségkeret** értékét.</span><span class="sxs-lookup"><span data-stu-id="7e464-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="7e464-130">A módosítások mentéséhez kattintson az **alkalmaz** gombra.</span><span class="sxs-lookup"><span data-stu-id="7e464-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="7e464-131">Megadhat *egy költségvetést is egy egyéni ügyfél* számára az előfizetési beállításokban:</span><span class="sxs-lookup"><span data-stu-id="7e464-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="7e464-132">Jelentkezzen be a Partnerközpont irányítópultjába.</span><span class="sxs-lookup"><span data-stu-id="7e464-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="7e464-133">A bal oldali menüben a **CSP** területen válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e464-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="7e464-134">Az **ügyfelek** lapon válassza ki az ügyfél **vállalatának nevét**.</span><span class="sxs-lookup"><span data-stu-id="7e464-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="7e464-135">Az ügyfél **előfizetések** lapján, a **használaton alapuló előfizetés** területen válassza a **költségvetés módosítása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e464-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="7e464-136">Adja meg a költségvetés értékét.</span><span class="sxs-lookup"><span data-stu-id="7e464-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="7e464-137">A módosítások mentéséhez kattintson az **alkalmaz** gombra.</span><span class="sxs-lookup"><span data-stu-id="7e464-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="7e464-138">Az Azure-kiadások költségvetésének eltávolítása</span><span class="sxs-lookup"><span data-stu-id="7e464-138">Remove Azure spending budget</span></span>

<span data-ttu-id="7e464-139">A partner Centerben a következő *havi Azure-költségkeretet távolíthatja el* ügyfeleinek:</span><span class="sxs-lookup"><span data-stu-id="7e464-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="7e464-140">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="7e464-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="7e464-141">A bal oldali menü **CSP** területén válassza az Azure- **kiadások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e464-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="7e464-142">Az **Azure-kiadások** oldalon Microsoft Azure- **előfizetéssel rendelkező ügyfelek** területen válassza ki azokat az ügyfeleket, akiknek a költségvetését el szeretné távolítani.</span><span class="sxs-lookup"><span data-stu-id="7e464-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="7e464-143">Válassza a **költségvetés eltávolítása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e464-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="7e464-144">Aktuális Azure-kiadások keresése</span><span class="sxs-lookup"><span data-stu-id="7e464-144">Check current Azure spending</span></span>

<span data-ttu-id="7e464-145">*Az ügyfelek aktuális Azure-kiadásait és havi költségkereteit bármikor nyomon követheti* :</span><span class="sxs-lookup"><span data-stu-id="7e464-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="7e464-146">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="7e464-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="7e464-147">A bal oldali menü **CSP** területén válassza az Azure- **kiadások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e464-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="7e464-148">Az **Azure-kiadások** oldalon Microsoft Azure- **előfizetéssel rendelkező ügyfeleknél** tekintse meg az ügyfelek havi költségkeretét, a jelenlegi kiadási becsléseket és a felhasznált költségvetés százalékos arányát.</span><span class="sxs-lookup"><span data-stu-id="7e464-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="7e464-149">A költségvetési korlátokkal kapcsolatos értesítések</span><span class="sxs-lookup"><span data-stu-id="7e464-149">Notifications for budget limits</span></span>

<span data-ttu-id="7e464-150">*Bekapcsolhatja az e-mailes értesítéseket* , amikor az ügyfél havi kiadásai elérik a költségvetési korlátot.</span><span class="sxs-lookup"><span data-stu-id="7e464-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="7e464-151">Ha bekapcsolja ezt a beállítást, a rendszer értesítést küld, ha az ügyfelek a havi költségkeretük 80%-át használják.</span><span class="sxs-lookup"><span data-stu-id="7e464-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="7e464-152">Ez a beállítás segít megőrizni az Azure-számlázást.</span><span class="sxs-lookup"><span data-stu-id="7e464-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="7e464-153">E-mail-értesítések konfigurálása:</span><span class="sxs-lookup"><span data-stu-id="7e464-153">To configure email notifications:</span></span>

1. <span data-ttu-id="7e464-154">Jelentkezzen be a Partnerközpontba.</span><span class="sxs-lookup"><span data-stu-id="7e464-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="7e464-155">Válassza a **Beállítások lehetőséget**.</span><span class="sxs-lookup"><span data-stu-id="7e464-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="7e464-156">Válassza **a saját beállítások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e464-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="7e464-157">Ha még nem tette meg, konfiguráljon egy előnyben részesített e-mail címet.</span><span class="sxs-lookup"><span data-stu-id="7e464-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="7e464-158">Adja meg az értesítéshez használni kívánt nyelvet.</span><span class="sxs-lookup"><span data-stu-id="7e464-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="7e464-159">Válassza a **CSP** fület az **értesítési beállítások** szakaszban.</span><span class="sxs-lookup"><span data-stu-id="7e464-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="7e464-160">Keresse meg az Azure- **kiadások** értesítése e-mailben lehetőséget, és **mentse** a következőt:.</span><span class="sxs-lookup"><span data-stu-id="7e464-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="7e464-161">Kitételi költségek szolgáltatás szerint</span><span class="sxs-lookup"><span data-stu-id="7e464-161">Itemized costs by service</span></span>

<span data-ttu-id="7e464-162">*A tételes költségeket (és a becsült használatot) a szolgáltatás alapján, a használaton alapuló előfizetések esetében tekintheti* meg:</span><span class="sxs-lookup"><span data-stu-id="7e464-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="7e464-163">Jelentkezzen be a Partnerközpontba.</span><span class="sxs-lookup"><span data-stu-id="7e464-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="7e464-164">A bal oldali menüben a **CSP** területen válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7e464-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="7e464-165">Az **ügyfelek** lapon válassza ki az ügyfél **vállalatának nevét**.</span><span class="sxs-lookup"><span data-stu-id="7e464-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="7e464-166">Az ügyfél **előfizetések** lapján, a **használat alapú előfizetések** területen válassza ki az **előfizetés** nevét.</span><span class="sxs-lookup"><span data-stu-id="7e464-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="7e464-167">Az előfizetés lapján áttekintheti a **részletezett költségeket** a szolgáltatás alapján, valamint az aktuális hónap **becsült felhasználását** .</span><span class="sxs-lookup"><span data-stu-id="7e464-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="7e464-168">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="7e464-168">Next steps</span></span>

- [<span data-ttu-id="7e464-169">Új kereskedelmi felület a CSP-ben – Azure-számlázás</span><span class="sxs-lookup"><span data-stu-id="7e464-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
