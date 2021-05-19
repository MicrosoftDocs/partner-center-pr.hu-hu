---
title: Kreditkorlát kényszerítve
ms.topic: how-to
ms.date: 05/11/2021
description: Ismerje meg a kreditkorlátot és annak kiszámítását. Tartalmazza a gyakori kérdéseket.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148108"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="a173e-104">Kreditkorlát kényszerítési (CLE)</span><span class="sxs-lookup"><span data-stu-id="a173e-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="a173e-105">**Megfelelő szerepkörök:** Számlázási rendszergazda</span><span class="sxs-lookup"><span data-stu-id="a173e-105">**Appropriate roles**: Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="a173e-106">A kreditkeret és annak működése</span><span class="sxs-lookup"><span data-stu-id="a173e-106">Your credit limit and how it works</span></span>

<span data-ttu-id="a173e-107">A kreditkorlát az a maximális összeg (amerikai dollárban), amit partnerként elkölthet termékek vagy előfizetések vásárlására a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="a173e-107">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="a173e-108">Ha túllépi a kreditkorlátot, addig nem vásárolhat új vásárlásokat, amíg nem fizet ki elegendő összeget.</span><span class="sxs-lookup"><span data-stu-id="a173e-108">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="a173e-109">A meglévő előfizetések továbbra is zavartalanul maradnak.</span><span class="sxs-lookup"><span data-stu-id="a173e-109">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="a173e-110">A kreditkorlátok az Azure-csomagra, az Azure Reservationsre, a Szoftverre, a Marketplace-re, az Azure 145 P-re, az Office-re és a Dynamics-termékekre vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="a173e-110">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="a173e-111">A jóváírási korlátok nem vonatkoznak a megújításra és a folyamatos használatra.</span><span class="sxs-lookup"><span data-stu-id="a173e-111">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="a173e-112">A kreditkorlátot a bérlői szinten rendeljük hozzá az előfizetési időszak alatt.</span><span class="sxs-lookup"><span data-stu-id="a173e-112">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="a173e-113">Ezt az előre jelzett bevételre, a vásárlási lehetőségekre és a kifizetési előzményekre alapozjuk.</span><span class="sxs-lookup"><span data-stu-id="a173e-113">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="a173e-114">Ezután a következő képlettel számítjuk ki a rendelkezésre álló egyenleget:</span><span class="sxs-lookup"><span data-stu-id="a173e-114">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="a173e-115">**[Kreditkorlát – (Bejövő vásárlás + Ki nem fizetett számlák + ki nem számlázott díjak – túlfizetés)]**</span><span class="sxs-lookup"><span data-stu-id="a173e-115">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="a173e-116">Gyakori kérdések</span><span class="sxs-lookup"><span data-stu-id="a173e-116">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="a173e-117">A kreditkorlátom a bérlő vagy a globális szinten van beállítva?</span><span class="sxs-lookup"><span data-stu-id="a173e-117">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="a173e-118">A bérlői szint.</span><span class="sxs-lookup"><span data-stu-id="a173e-118">The tenant level.</span></span> <span data-ttu-id="a173e-119">Tegyük fel például, hogy az Egyesült Államokból, Kanadából és Japánból üzemeltet.</span><span class="sxs-lookup"><span data-stu-id="a173e-119">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="a173e-120">Ha a kanadai bérlő eléri a kreditkorlátot, akkor a bérlő értesítést kap, amikor megpróbál vásárolni a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="a173e-120">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="a173e-121">A többi bérlőre ez nem lesz hatással.</span><span class="sxs-lookup"><span data-stu-id="a173e-121">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="a173e-122">Ha túllépem a kreditkorlátomat, folytatható a meglévő ügyfelek és előfizetések teljes körű kiszolgálása?</span><span class="sxs-lookup"><span data-stu-id="a173e-122">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="a173e-123">Igen.</span><span class="sxs-lookup"><span data-stu-id="a173e-123">Yes.</span></span> <span data-ttu-id="a173e-124">Az ügyfelek meglévő előfizetései megszakítás nélkül folytatódnak.</span><span class="sxs-lookup"><span data-stu-id="a173e-124">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="a173e-125">Az ügyfelek számára azonban nem vásárolhat új előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="a173e-125">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="a173e-126">Vonatkozik a CLE a közvetlen számlázási partnerekre és a közvetett szolgáltatókra is?</span><span class="sxs-lookup"><span data-stu-id="a173e-126">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="a173e-127">Igen, mindkettőre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="a173e-127">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="a173e-128">Miután beküldtem a kifizetésemet a fiók visszaállításához, mikor vásárolhatok további előfizetéseket?</span><span class="sxs-lookup"><span data-stu-id="a173e-128">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="a173e-129">A vásárlást a kifizetést követő 24 órán belül folytathatja, feltéve, hogy a Microsoft megkapta a hitelkeret-ellenőrzés folyamatának folytatásához szükséges összes követelményt.</span><span class="sxs-lookup"><span data-stu-id="a173e-129">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="a173e-130">Hogyan tudom ellenőrizni a kreditkorlátomat?</span><span class="sxs-lookup"><span data-stu-id="a173e-130">How can I check my credit limit?</span></span>

<span data-ttu-id="a173e-131">Vegye [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) fel a kapcsolatot a hitelkerete és a legutóbbi vásárlásokkal kapcsolatos információk lekért információkért.</span><span class="sxs-lookup"><span data-stu-id="a173e-131">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="a173e-132">A vitatás alatt szereplő számlák beleszámnak a kreditkeretbe?</span><span class="sxs-lookup"><span data-stu-id="a173e-132">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="a173e-133">Igen.</span><span class="sxs-lookup"><span data-stu-id="a173e-133">Yes.</span></span> <span data-ttu-id="a173e-134">A probléma megoldásához azonban kapcsolatba léphet a Microsofttal [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) a következő elérhetőségen: .</span><span class="sxs-lookup"><span data-stu-id="a173e-134">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="a173e-135">Milyen hamar hallok majd, ha a-be írjuk ucmwrcsp@microsoft.com a-t?</span><span class="sxs-lookup"><span data-stu-id="a173e-135">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="a173e-136">Kevesebb mint 24 órán belül választ kell adnunk.</span><span class="sxs-lookup"><span data-stu-id="a173e-136">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="a173e-137">Milyen feltételeket használ a Microsoft egy partner hitelkeretének beállítására?</span><span class="sxs-lookup"><span data-stu-id="a173e-137">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="a173e-138">A kreditkorlátot az előre jelzett bevétel, a vásárlási lehetőségek és a fizetési előzmények alapján határozzuk meg.</span><span class="sxs-lookup"><span data-stu-id="a173e-138">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="a173e-139">A kreditkorlát jelenleg érvényben van az új kereskedelmi felhasználói élményben?</span><span class="sxs-lookup"><span data-stu-id="a173e-139">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="a173e-140">Igen.</span><span class="sxs-lookup"><span data-stu-id="a173e-140">Yes.</span></span> <span data-ttu-id="a173e-141">A kreditkorlátok az összes CSP-programra és -termékre érvényesek a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="a173e-141">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="a173e-142">Ki kapja meg az értesítést, amikor a szervezetem közeledik a kreditkorláthoz?</span><span class="sxs-lookup"><span data-stu-id="a173e-142">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="a173e-143">A szervezet pénzügyi kapcsolattartója megkapja az értesítést.</span><span class="sxs-lookup"><span data-stu-id="a173e-143">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a173e-144">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="a173e-144">Next steps</span></span>

[<span data-ttu-id="a173e-145">A számlázás alapjai</span><span class="sxs-lookup"><span data-stu-id="a173e-145">Billing basics</span></span>](./billing-basics.md)
