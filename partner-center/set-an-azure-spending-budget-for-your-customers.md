---
title: Azure-költségvetés beállítása az ügyfelek számára
ms.topic: how-to
ms.date: 03/17/2021
description: Megtudhatja, hogyan állíthat be vagy távolíthat el havi Azure-költségkereteket az ügyfelek számára, valamint megtekintheti az Azure-költségadatokat, és hogyan állíthat be költségvetéssel kapcsolatos értesítéseket.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855352"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="00dee-103">Havi Azure-költségvetések beállítása, ellenőrzése vagy eltávolítása a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="00dee-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="00dee-104">**Megfelelő szerepkörök:** Rendszergazdai ügynök</span><span class="sxs-lookup"><span data-stu-id="00dee-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="00dee-105">Havi [Azure-költségkeretet állíthat](#set-azure-spending-budget) be az ügyfelek számára a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="00dee-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="00dee-106">Ez segít az ügyfeleknek az Azure-kiadások kezelésében.</span><span class="sxs-lookup"><span data-stu-id="00dee-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="00dee-107">Ezzel a lehetőséggel összehasonlíthatja az ügyfelek Azure-kiadásait a költségvetéssel a hónap során.</span><span class="sxs-lookup"><span data-stu-id="00dee-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="00dee-108">Emellett segít az ügyfeleknek az Azure-kiadások költségvetésében is, hogy a havi számla ne magasabb, mint amit várnak.</span><span class="sxs-lookup"><span data-stu-id="00dee-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="00dee-109">Ez a funkció nem érhető el a tesztboxban vagy a Tesztelés éles környezetben (TIP) fiókokban.</span><span class="sxs-lookup"><span data-stu-id="00dee-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="00dee-110">Miután [beállította az Azure-költségvetést az ügyfél(ök)hez,](#set-azure-spending-budget)a következő módokon is áttekintheti az ügyfélhasználatot.</span><span class="sxs-lookup"><span data-stu-id="00dee-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="00dee-111">Ezek a lehetőségek segíthetnek a helytelenül konfigurált szolgáltatások vagy szokatlan trendek felderítésében, amelyek csalásra utalhatnak.</span><span class="sxs-lookup"><span data-stu-id="00dee-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="00dee-112">Ezután az ügyfél(ök) segítségével azonosíthatja a kiváltó okot és kezelheti a költségeket.</span><span class="sxs-lookup"><span data-stu-id="00dee-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="00dee-113">Szükség esetén magasabb [összegre](#set-azure-spending-budget) is módosíthatja az ügyfél költségvetését.</span><span class="sxs-lookup"><span data-stu-id="00dee-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="00dee-114">Az aktuális Azure-kiadások ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="00dee-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="00dee-115">E-mail-értesítéseket kapcsol be arra az értesítésre, amikor egy ügyfél költségkerete közeledik</span><span class="sxs-lookup"><span data-stu-id="00dee-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="00dee-116">Elemi költségek megtekintése szolgáltatás szerint a használatalapú előfizetések esetén</span><span class="sxs-lookup"><span data-stu-id="00dee-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="00dee-117">Az [ügyfelekre vonatkozó Azure-költségkeretet](#remove-azure-spending-budget) bármikor eltávolíthatja.</span><span class="sxs-lookup"><span data-stu-id="00dee-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="00dee-118">Azure-beli kiadási adatok</span><span class="sxs-lookup"><span data-stu-id="00dee-118">Azure spending data</span></span>

<span data-ttu-id="00dee-119">Az Azure-költségadatok becsült *összegek,* és a *tényleges számlázási összegek eltérőek lehetnek.*</span><span class="sxs-lookup"><span data-stu-id="00dee-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="00dee-120">Az adatok értéke *nem* tükrözi az adókat, jóváírásokat, helyesbítéseket és az esetlegesen fizetendő egyéb díjakat.</span><span class="sxs-lookup"><span data-stu-id="00dee-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="00dee-121">A költési adatok *naponta egyszer frissülnek.*</span><span class="sxs-lookup"><span data-stu-id="00dee-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="00dee-122">Az ügyfelek továbbra is használhatnak (és díjat számolunk fel) az Azure-szolgáltatások és -erőforrások használata esetén, ha nem módosítja a fiókbeállításokat a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="00dee-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="00dee-123">Az Azure-költségvetés beállítása</span><span class="sxs-lookup"><span data-stu-id="00dee-123">Set Azure spending budget</span></span>

<span data-ttu-id="00dee-124">Havi *Azure-költségkeretet állíthat* be több ügyfélhez a Partnerközpont:</span><span class="sxs-lookup"><span data-stu-id="00dee-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="00dee-125">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="00dee-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="00dee-126">A bal oldali menü **CSP** menüjében válassza az **Azure-kiadások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="00dee-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="00dee-127">Az **Azure-kiadások oldal** Ügyfelek Microsoft Azure **előfizetéssel** alatt válassza ki azokat az ügyfeleket, akiknek költségvetést szeretne beállítani.</span><span class="sxs-lookup"><span data-stu-id="00dee-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="00dee-128">Adjon meg egy értéket a **Havi költségvetés mezőben.**</span><span class="sxs-lookup"><span data-stu-id="00dee-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="00dee-129">A **módosítások mentéshez** válassza az Alkalmaz lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="00dee-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="00dee-130">Egyéni ügyfél *előfizetési beállításaiban is* beállíthatja a költségvetést:</span><span class="sxs-lookup"><span data-stu-id="00dee-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="00dee-131">Jelentkezzen be a Partnerközpont irányítópultjába.</span><span class="sxs-lookup"><span data-stu-id="00dee-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="00dee-132">A bal oldali menü **CSP** menüjében válassza az Ügyfelek **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="00dee-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="00dee-133">Az Ügyfelek **lapon** válassza ki az ügyfél **cégnevét.**</span><span class="sxs-lookup"><span data-stu-id="00dee-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="00dee-134">Az ügyfél Előfizetések **lapján,** a **Használatalapú előfizetés** alatt válassza a **Költségvetés módosítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="00dee-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="00dee-135">Adja meg a költségvetés értékét.</span><span class="sxs-lookup"><span data-stu-id="00dee-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="00dee-136">A **módosítások mentéshez** válassza az Alkalmaz lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="00dee-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="00dee-137">Azure-költségvetés eltávolítása</span><span class="sxs-lookup"><span data-stu-id="00dee-137">Remove Azure spending budget</span></span>

<span data-ttu-id="00dee-138">Az ügyfelek *havi Azure-költségkeretét* a következő Partnerközpont:</span><span class="sxs-lookup"><span data-stu-id="00dee-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="00dee-139">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="00dee-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="00dee-140">A bal oldali menü **CSP** menüjében válassza az **Azure-kiadások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="00dee-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="00dee-141">Az **Azure-kiadások oldal** Ügyfelek Microsoft Azure **előfizetéssel** területén válassza ki azokat az ügyfeleket, akiknek a költségvetését el szeretné távolítani.</span><span class="sxs-lookup"><span data-stu-id="00dee-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="00dee-142">Válassza a **Költségvetés eltávolítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="00dee-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="00dee-143">Az aktuális Azure-kiadások ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="00dee-143">Check current Azure spending</span></span>

<span data-ttu-id="00dee-144">Az ügyfelek *aktuális Azure-kiadásait* és havi költségkeretét bármikor nyomon követheti:</span><span class="sxs-lookup"><span data-stu-id="00dee-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="00dee-145">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="00dee-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="00dee-146">A bal oldali menü **CSP** menüjében válassza az **Azure-kiadások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="00dee-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="00dee-147">Az **Azure-kiadások** oldalon a Customers **with Microsoft Azure subscriptions**(Ügyfelek Microsoft Azure-előfizetéssel) alatt áttekintheti az ügyfelek havi költségvetését, az aktuális költségbecsléseket és a felhasznált költségvetés százalékos arányát.</span><span class="sxs-lookup"><span data-stu-id="00dee-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="00dee-148">Költségvetési korlátokra vonatkozó értesítések</span><span class="sxs-lookup"><span data-stu-id="00dee-148">Notifications for budget limits</span></span>

<span data-ttu-id="00dee-149">Bekapcsolhatja *az e-mail-értesítéseket,* ha az ügyfél havi költségkerete a költségkerethez közeledik.</span><span class="sxs-lookup"><span data-stu-id="00dee-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="00dee-150">Ha bekapcsolja ezt a beállítást, értesítést kap, ha az ügyfelek a havi költségkeretük 80%-át vagy többet használják ki.</span><span class="sxs-lookup"><span data-stu-id="00dee-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="00dee-151">Ezzel a lehetőséggel nyomon tudja tartani az Azure-számlát.</span><span class="sxs-lookup"><span data-stu-id="00dee-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="00dee-152">E-mail-értesítések konfigurálása:</span><span class="sxs-lookup"><span data-stu-id="00dee-152">To configure email notifications:</span></span>

1. <span data-ttu-id="00dee-153">Jelentkezzen be a Partnerközpontba.</span><span class="sxs-lookup"><span data-stu-id="00dee-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="00dee-154">Ugrás a **Beállítások lapra.**</span><span class="sxs-lookup"><span data-stu-id="00dee-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="00dee-155">Válassza **a Saját beállítások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="00dee-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="00dee-156">Ha még nem, konfigurálja az előnyben részesített e-mail-címet.</span><span class="sxs-lookup"><span data-stu-id="00dee-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="00dee-157">Konfigurálja az értesítés előnyben részesített nyelvét.</span><span class="sxs-lookup"><span data-stu-id="00dee-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="00dee-158">Az **Értesítési beállítások** szakaszban válassza a CSP **lapot.**</span><span class="sxs-lookup"><span data-stu-id="00dee-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="00dee-159">Jelölje be az Azure-beli **költési értesítés e-mailes beállítását,** majd a **Mentés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="00dee-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="00dee-160">Elemi költségek szolgáltatás szerint</span><span class="sxs-lookup"><span data-stu-id="00dee-160">Itemized costs by service</span></span>

<span data-ttu-id="00dee-161">A *használatalapú előfizetések* tételes költségeit (és becsült használatát) szolgáltatás szerint is megtekintheti:</span><span class="sxs-lookup"><span data-stu-id="00dee-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="00dee-162">Jelentkezzen be a Partnerközpontba.</span><span class="sxs-lookup"><span data-stu-id="00dee-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="00dee-163">A bal oldali menü **CSP** menüjében válassza az Ügyfelek **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="00dee-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="00dee-164">Az Ügyfelek **lapon** válassza ki az ügyfél **Cégnevét.**</span><span class="sxs-lookup"><span data-stu-id="00dee-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="00dee-165">Az ügyfél Előfizetések **lapján,** a **Használatalapú** előfizetések alatt válassza ki az Előfizetés **nevét.**</span><span class="sxs-lookup"><span data-stu-id="00dee-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="00dee-166">Az előfizetés oldalán áttekintheti a  tételes költségeket szolgáltatás  szerint, valamint a Becsült használatot az aktuális hónapra.</span><span class="sxs-lookup"><span data-stu-id="00dee-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="00dee-167">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="00dee-167">Next steps</span></span>

- [<span data-ttu-id="00dee-168">Új kereskedelmi felület a CSP-ben – Azure-számlázás</span><span class="sxs-lookup"><span data-stu-id="00dee-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
