---
title: Credit limit enforcement
ms.topic: how-to
ms.date: 05/11/2021
description: Ismerje meg a kreditkorlátot és annak kiszámítását. Tartalmazza a gyakori kérdéseket.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819380"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="15381-104">Credit limit enforcement (CLE)</span><span class="sxs-lookup"><span data-stu-id="15381-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="15381-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="15381-105">**Appropriate roles**</span></span>

- <span data-ttu-id="15381-106">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="15381-106">Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="15381-107">A kreditkeret és annak működése</span><span class="sxs-lookup"><span data-stu-id="15381-107">Your credit limit and how it works</span></span>

<span data-ttu-id="15381-108">A kreditkorlát az a maximális összeg (amerikai dollárban), amit Partnerként elkölthet termékek vagy előfizetések vásárlására a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="15381-108">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="15381-109">Ha túllépi a kreditkeretét, addig nem vásárolhat új vásárlásokat, amíg nem fizet ki elegendő összeget.</span><span class="sxs-lookup"><span data-stu-id="15381-109">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="15381-110">A meglévő előfizetések továbbra is megszakítás nélkül maradnak.</span><span class="sxs-lookup"><span data-stu-id="15381-110">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="15381-111">A kreditkorlátok az Azure-csomag, az Azure Reservations, a Szoftver, a Marketplace, az Azure 145 P, az Office és a Dynamics termékek ajánlataira vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="15381-111">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="15381-112">A kreditkorlátok nem vonatkoznak a megújításra és a folyamatos használatra.</span><span class="sxs-lookup"><span data-stu-id="15381-112">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="15381-113">A kreditkorlátot a bérlői szinten rendeljük hozzá az előfizetési időszak alatt.</span><span class="sxs-lookup"><span data-stu-id="15381-113">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="15381-114">Ezt az előre jelzett bevételre, a vásárlási lehetőségekre és a fizetési előzményekre alapozjuk.</span><span class="sxs-lookup"><span data-stu-id="15381-114">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="15381-115">Ezután a következő képlettel számítjuk ki a rendelkezésre álló egyenleget:</span><span class="sxs-lookup"><span data-stu-id="15381-115">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="15381-116">**[Credit Limit – (Bejövő vásárlás + ki nem fizetett számlák + ki nem számlázott díjak – Túlfizetés)]**</span><span class="sxs-lookup"><span data-stu-id="15381-116">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="15381-117">Gyakori kérdések</span><span class="sxs-lookup"><span data-stu-id="15381-117">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="15381-118">A kreditkorlátom a bérlő vagy a globális szinten van beállítva?</span><span class="sxs-lookup"><span data-stu-id="15381-118">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="15381-119">A bérlői szint.</span><span class="sxs-lookup"><span data-stu-id="15381-119">The tenant level.</span></span> <span data-ttu-id="15381-120">Tegyük fel például, hogy az Egyesült Államokból, Kanadából és Japánból tevékenykedik.</span><span class="sxs-lookup"><span data-stu-id="15381-120">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="15381-121">Ha a kanadai bérlő eléri a kreditkorlátját, akkor a bérlő értesítést kap, amikor megpróbál vásárolni a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="15381-121">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="15381-122">A többi bérlőre ez nem lesz hatással.</span><span class="sxs-lookup"><span data-stu-id="15381-122">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="15381-123">Ha túllépem a kreditkorlátomat, folytatható a meglévő ügyfelek és előfizetések teljes körű kiszolgálása?</span><span class="sxs-lookup"><span data-stu-id="15381-123">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="15381-124">Igen.</span><span class="sxs-lookup"><span data-stu-id="15381-124">Yes.</span></span> <span data-ttu-id="15381-125">Az ügyfelek meglévő előfizetései megszakítás nélkül folytatódnak.</span><span class="sxs-lookup"><span data-stu-id="15381-125">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="15381-126">Azonban nem vásárolhat új előfizetéseket az ügyfelei számára.</span><span class="sxs-lookup"><span data-stu-id="15381-126">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="15381-127">Vonatkozik a CLE a közvetlen számlázási partnerekre és a közvetett szolgáltatókra is?</span><span class="sxs-lookup"><span data-stu-id="15381-127">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="15381-128">Igen, mindkettőre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="15381-128">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="15381-129">Miután beküldtem a kifizetésemet a fiók visszaállításához, mikor vásárolhatok további előfizetéseket?</span><span class="sxs-lookup"><span data-stu-id="15381-129">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="15381-130">A fizetést követő 24 órán belül folytathatja a vásárlást, feltéve, hogy a Microsoft megkapta a hitelkeret-ellenőrzés folyamatának folytatásához szükséges összes követelményt.</span><span class="sxs-lookup"><span data-stu-id="15381-130">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="15381-131">Hogyan tudom ellenőrizni a kreditkorlátomat?</span><span class="sxs-lookup"><span data-stu-id="15381-131">How can I check my credit limit?</span></span>

<span data-ttu-id="15381-132">Vegye [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) fel a kapcsolatot a kreditkorlátja és a legutóbbi vásárlások információinak lekért információkért.</span><span class="sxs-lookup"><span data-stu-id="15381-132">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="15381-133">A vitatás alatt szereplő számlák beleszámnak a kreditkeretbe?</span><span class="sxs-lookup"><span data-stu-id="15381-133">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="15381-134">Igen.</span><span class="sxs-lookup"><span data-stu-id="15381-134">Yes.</span></span> <span data-ttu-id="15381-135">A probléma megoldásához azonban kapcsolatba léphet a Microsofttal [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) a következő elérhetőségen: .</span><span class="sxs-lookup"><span data-stu-id="15381-135">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="15381-136">Milyen hamar hallok majd, ha a-be írjuk ucmwrcsp@microsoft.com a-t?</span><span class="sxs-lookup"><span data-stu-id="15381-136">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="15381-137">Kevesebb mint 24 órán belül választ kell adnunk.</span><span class="sxs-lookup"><span data-stu-id="15381-137">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="15381-138">Milyen feltételeket használ a Microsoft egy partner hitelkeretének beállítására?</span><span class="sxs-lookup"><span data-stu-id="15381-138">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="15381-139">A kreditkorlátot az előre jelzett bevétel, a vásárlási idő és a kifizetési előzmények alapján határozzuk meg.</span><span class="sxs-lookup"><span data-stu-id="15381-139">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="15381-140">A kreditkorlát jelenleg érvényben van az új kereskedelmi felhasználói élményben?</span><span class="sxs-lookup"><span data-stu-id="15381-140">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="15381-141">Igen.</span><span class="sxs-lookup"><span data-stu-id="15381-141">Yes.</span></span> <span data-ttu-id="15381-142">A kreditkorlátok az összes CSP-programra és termékre érvényesek a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="15381-142">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="15381-143">Ki kapja meg az értesítést, amikor a szervezetem a kreditkorlátja közeledik?</span><span class="sxs-lookup"><span data-stu-id="15381-143">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="15381-144">Az értesítést a szervezet pénzügyi kapcsolattartója kapja meg.</span><span class="sxs-lookup"><span data-stu-id="15381-144">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="15381-145">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="15381-145">Next steps</span></span>

[<span data-ttu-id="15381-146">A számlázás alapjai</span><span class="sxs-lookup"><span data-stu-id="15381-146">Billing basics</span></span>](./billing-basics.md)
