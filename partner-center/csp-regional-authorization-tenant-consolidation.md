---
title: CSP regionális engedélyezési bérlők összevonása
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezekkel az utasításokkal konszolidálhatja a különböző országok/régiók bérlőit. Ez magában foglalja az ügyfélfiókok és ügyfél-előfizetések áttelepítésének lépéseit.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 84e5f7f2674e9b2f3c3c26ed2ea49f9bba0e96e0
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276875"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="575fc-104">Útmutató a CSP regionális engedélyezési bérlőösszevonáshoz</span><span class="sxs-lookup"><span data-stu-id="575fc-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="575fc-105">**A következőkre vonatkozik:** Partnerközpont | Partnerközpont a Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="575fc-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="575fc-106">**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök</span><span class="sxs-lookup"><span data-stu-id="575fc-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="575fc-107">\[Egyes információk az előre kiadott termékkel kapcsolatosak, amelyek a kereskedelmi forgalomban való nyilvánosságra kerül előtt jelentős mértékben módosíthatók.</span><span class="sxs-lookup"><span data-stu-id="575fc-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="575fc-108">A Microsoft nem vállal kifejezett vagy törvényi garanciát az itt megjelenő információért.\]</span><span class="sxs-lookup"><span data-stu-id="575fc-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="575fc-109">Összevonhatja a vállalat bérlőit.</span><span class="sxs-lookup"><span data-stu-id="575fc-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="575fc-110">Ezekkel az utasításokkal konszolidálhatja a különböző országok/régiók bérlőit.</span><span class="sxs-lookup"><span data-stu-id="575fc-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="575fc-111">Tisztában kell lennie az összes kiépített előfizetéssel és licencszámmal abban a fiókban, amelyről átvált.</span><span class="sxs-lookup"><span data-stu-id="575fc-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="575fc-112">A migrálási folyamat részeként újra kiépíti ugyanezeket az előfizetéseket ugyanazokkal a licencszámokkal az új központi CSP-fiókban.</span><span class="sxs-lookup"><span data-stu-id="575fc-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="575fc-113">Az exportálási lista funkcióval létrehozhatja azon ügyfelek listáját, akik átlépnek a központosított bérlőre.</span><span class="sxs-lookup"><span data-stu-id="575fc-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="575fc-114">A konszolidálás befejezése után nem lehet visszaállni az előző bérlői állapotra.</span><span class="sxs-lookup"><span data-stu-id="575fc-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="575fc-115">Szükség lehet az ügyfél beavatkozásra is.</span><span class="sxs-lookup"><span data-stu-id="575fc-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="575fc-116">Előkészületek a migráláshoz</span><span class="sxs-lookup"><span data-stu-id="575fc-116">Prepare for migration</span></span>

- <span data-ttu-id="575fc-117">Jelentkezzen be **Partnerközpont** fiókkal  (az új fiókra átváltáskor), és tekintse át az összes ügyfelet és az ezen ügyfelek számára kiépített szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="575fc-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="575fc-118">Jelentkezzen ki ebből a fiókból.</span><span class="sxs-lookup"><span data-stu-id="575fc-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="575fc-119">Ügyfélfiókok áttelepítése</span><span class="sxs-lookup"><span data-stu-id="575fc-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="575fc-120">Jelentkezzen be **a Partnerközpont**  az **Átmeneti** (új) fiókkal (arra, amelybe átveszi az ügyfeleket).</span><span class="sxs-lookup"><span data-stu-id="575fc-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="575fc-121">Válassza az **Ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="575fc-121">Select **Customers**.</span></span>

3. <span data-ttu-id="575fc-122">Válassza **a Viszonteladói kapcsolat kérése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="575fc-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="575fc-123">Megjelenik egy alapértelmezett e-mail-üzenet, amely elküldve lesz az ügyfeleknek.</span><span class="sxs-lookup"><span data-stu-id="575fc-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="575fc-124">Ez az üzenet egy URL-címet tartalmaz, amely az új fiók egyedi szervezeti Partnerközpont tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="575fc-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="575fc-125">**Ügyfél beavatkozása:** Győződjön meg arról, hogy az összes átemelni kívánt aktív ügyfél felkeresi ezt az URL-címet.</span><span class="sxs-lookup"><span data-stu-id="575fc-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="575fc-126">Az URL-cím megnyitásakor a rendszer felkéri az ügyfelet, hogy jelentkezzen be az Office 365 portálra.</span><span class="sxs-lookup"><span data-stu-id="575fc-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="575fc-127">Az ügyfél ugyanazokkal a szervezeti azonosítóval jelentkezik be, mint az Azure és az Office 365 felügyeleti portálok eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="575fc-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="575fc-128">Bejelentkezés után a rendszer felkéri  az ügyfélfiók globális rendszergazdáját, hogy küldjön be egy olyan szerződést, amely delegált rendszergazdai jogosultságokat biztosít az új CSP-fióknak.</span><span class="sxs-lookup"><span data-stu-id="575fc-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="575fc-129">Ha beleegyeznek, az ügyfél kiválasztja a jelölőnégyzetet, és engedélyezi a kapcsolatot.</span><span class="sxs-lookup"><span data-stu-id="575fc-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="575fc-130">Az ügyfelek a szerződés beküldtét követően jelennek meg a partner ügyféllistán, egyesével.</span><span class="sxs-lookup"><span data-stu-id="575fc-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="575fc-131">Office 365- és nem Azure-beli használatalapú előfizetések áttelepítése</span><span class="sxs-lookup"><span data-stu-id="575fc-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="575fc-132">Miután az ügyfél aláírta a szerződést, újra létrehozhatja az előfizetéseket a központi partnerbérlőben.</span><span class="sxs-lookup"><span data-stu-id="575fc-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="575fc-133">A **Partnerközpont** válassza a Customers (Ügyfelek) **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="575fc-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="575fc-134">Nyissa meg annak az ügyfélnek a cégnevét, akiről migelni szeretne.</span><span class="sxs-lookup"><span data-stu-id="575fc-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="575fc-135">Válassza **az Előfizetés hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="575fc-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="575fc-136">Adja hozzá a megfelelő előfizetéseket és licencszámokat a katalógusból.</span><span class="sxs-lookup"><span data-stu-id="575fc-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="575fc-137">Ellenőrizze a partnerfiókok váltása során **megadott** információkat.</span><span class="sxs-lookup"><span data-stu-id="575fc-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="ügyféllista.":::

6. <span data-ttu-id="575fc-139">Válassza a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="575fc-139">Select **Submit.**</span></span>

   <span data-ttu-id="575fc-140">A szolgáltatásokat most már a Váltás partnerfiókból biztosítja **az** ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="575fc-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="575fc-141">Ismételje meg ezeket a lépéseket az összes további ügyfél előfizetésének áttelepítéséhez.</span><span class="sxs-lookup"><span data-stu-id="575fc-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="575fc-142">Mielőtt továbblépne a következő szakaszra, győződjön  meg arról, hogy a Váltás partnerfiókból területen meglévő összes ügyfél-előfizetés újra ki van építve a **Váltás** partnerfiókra területen.</span><span class="sxs-lookup"><span data-stu-id="575fc-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="575fc-143">A partnereknek az  előfizetések váltása partnerbérlői fiókból fiókra való váltásának napján fel  kell függesztenie Partnerközpont előfizetéseket ugyanazon a napon, amikor az előfizetések át vannak állítva és be vannak állítva az Partnerközpont-ban a Váltás partnerbérlőre fiókban annak érdekében, hogy a kettős számlázás ne fordul elő.</span><span class="sxs-lookup"><span data-stu-id="575fc-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="575fc-144">A rendszer megtagadja a támogatási kéréseket a kreditekért, mert a számlázásban átfedés lép fel, és nem tiltja le megfelelően az előfizetésből **való váltást.**</span><span class="sxs-lookup"><span data-stu-id="575fc-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="575fc-145">Az Office 365-előfizetések letiltása a Váltás a partnerfiókból alatt</span><span class="sxs-lookup"><span data-stu-id="575fc-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="575fc-146">Ha letiltja a CSP-előfizetést a **Partnerfiókok** váltása alatt, azzal leállítja a jövőbeli számlázást.</span><span class="sxs-lookup"><span data-stu-id="575fc-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="575fc-147">Nem kell manuálisan letiltania az Azure-előfizetéseket, mert az Azure-előfizetések automatikusan le vannak tiltva a migrálási folyamat során.</span><span class="sxs-lookup"><span data-stu-id="575fc-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="575fc-148">Jelentkezzen be a **Partnerközpont** csp-fiókból való áttéréssel, és lépjen az ügyféllistára. </span><span class="sxs-lookup"><span data-stu-id="575fc-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="575fc-149">Nyissa meg az előfizetéseket a letiltásához, majd válassza ki az első letiltani kívánt ajánlatot.</span><span class="sxs-lookup"><span data-stu-id="575fc-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="575fc-150">Állítsa az előfizetést **felfüggesztettre,** majd válassza a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="575fc-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="575fc-151">Az előfizetés felfüggesztése biztosítja, hogy a dupla számlázás nem történik meg.</span><span class="sxs-lookup"><span data-stu-id="575fc-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="575fc-152">Az előfizetés fel **van függesztve** az előfizetések listájában.</span><span class="sxs-lookup"><span data-stu-id="575fc-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="575fc-153">Ismételje meg ezeket a lépéseket az ügyfél összes előfizetése esetén.</span><span class="sxs-lookup"><span data-stu-id="575fc-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="575fc-154">Ellenőrizze, hogy az összes fel **van-e függesztve.**</span><span class="sxs-lookup"><span data-stu-id="575fc-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="575fc-155">Válassza ki a listából a következő ügyfelet, és ismételje meg az összes előfizetés letiltásának folyamatát.</span><span class="sxs-lookup"><span data-stu-id="575fc-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="575fc-156">Használatalapú Azure-előfizetések áttelepítése</span><span class="sxs-lookup"><span data-stu-id="575fc-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="575fc-157">Az Office 365 CSP-előfizetésekkel ellentétben az Azure-beli használatalapú CSP-előfizetéseket nem kell manuálisan migrálni.</span><span class="sxs-lookup"><span data-stu-id="575fc-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="575fc-158">Microsoft Azure-támogatás át fogja telepíteni az Azure-előfizetéseket és az összes  üzembe helyezett szolgáltatást vagy erőforrást a CSP-viszonteladói fiókokról a **VÁLTÁS** CSP-re viszonteladói fiókra.</span><span class="sxs-lookup"><span data-stu-id="575fc-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="575fc-159">Az átállás során nem fog megszakadni az ügyfél kiszolgálása.</span><span class="sxs-lookup"><span data-stu-id="575fc-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="575fc-160">Győződjön meg arról, hogy a migrált Azure-előfizetésekkel rendelkező ügyfélfiókok elfogadták az új CSP-fiókra való áttérésre vonatkozó szerződést. </span><span class="sxs-lookup"><span data-stu-id="575fc-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="575fc-161">Értesítenie kell a Microsoftot arról, hogy mely ügyfélfiókok állnak készen az áttelepítésre, és meg kell adnia az ügyfél vállalatnevét.</span><span class="sxs-lookup"><span data-stu-id="575fc-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="575fc-162">A Microsoft migrálta az Azure használatalapú előfizetéseket, és értesíti, ha a migrálás befejeződött.</span><span class="sxs-lookup"><span data-stu-id="575fc-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="575fc-163">Meg kell erősítenie, hogy a CSP-viszonteladói fiókról váltás  alatt található Azure-előfizetés most fel van jelölve a Partnerközpont előfizetések szakaszban. </span><span class="sxs-lookup"><span data-stu-id="575fc-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="575fc-164">Győződjön meg arról, hogy a **Váltás** CSP-viszonteladói fiókra  területen lévő Azure-előfizetésnél az aktív állapot Partnerközpont az ügyfél-előfizetések szakaszban.</span><span class="sxs-lookup"><span data-stu-id="575fc-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="575fc-165">Az előfizetések ügyfél alatti letiltása nem módosítja az ügyfél megjelenését az Ügyfelek listában.</span><span class="sxs-lookup"><span data-stu-id="575fc-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="575fc-166">Jelenleg nincs lehetőség ügyfelek eltávolítására a listából.</span><span class="sxs-lookup"><span data-stu-id="575fc-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="575fc-167">A partnereknek el kell kerülniük,  hogy a jövőben előfizetéseket adjanak vissza ezekhez az ügyfelekhez a fiókjukból való áttérésből.</span><span class="sxs-lookup"><span data-stu-id="575fc-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="575fc-168">Ismételje meg ezeket a lépéseket az összes ügyfélhez elérhető  összes előfizetés esetében, hogy a jövőbeli díjakat leállítsa a váltás fiók(ak)on.</span><span class="sxs-lookup"><span data-stu-id="575fc-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="575fc-169">A partner egy utolsó számlát kap, amely a lemondás napja és a számlázási időszak utolsó napja közötti fel nem használt napok számára vonatkozó jóváírást is megkapja.</span><span class="sxs-lookup"><span data-stu-id="575fc-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="575fc-170">A végső számlázási időszak után nem fog számlát generálni.</span><span class="sxs-lookup"><span data-stu-id="575fc-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="575fc-171">További információ</span><span class="sxs-lookup"><span data-stu-id="575fc-171">Additional information</span></span>

- <span data-ttu-id="575fc-172">Ha letiltja az  előfizetést a CSP-fiókról való váltásról, az nem befolyásolja az ügyfél szolgáltatását, ha a szolgáltatást az előfizetés letiltása előtt kiépítik a Váltás  CSP-fiókra fiókból.</span><span class="sxs-lookup"><span data-stu-id="575fc-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="575fc-173">Az előfizetések nem használhatók az ügyfél által, és nem generálnak díjakat, ha fel vannak függesztve vagy törölve.</span><span class="sxs-lookup"><span data-stu-id="575fc-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="575fc-174">Jelenleg nincs mód arra, hogy teljesen eltávolítson egy ügyfelet az Ügyfelek **listából.**</span><span class="sxs-lookup"><span data-stu-id="575fc-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="575fc-175">A partnereknek ugyanazon  a napon fel kell függesztenie az előfizetéseket Partnerközpont partnerbérlői fiókról való váltásra, amikor az előfizetések át vannak állítva és be vannak állítva a Váltás fiókra, hogy a kettős számlázás ne fordul elő. </span><span class="sxs-lookup"><span data-stu-id="575fc-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="575fc-176">A Microsoft nem támogatja a kreditek kérését a számlázás bármilyen  átfedése miatt, amely abból ad vissza, hogy nem megfelelően beállította az előfizetésből való váltást felfüggesztettre.</span><span class="sxs-lookup"><span data-stu-id="575fc-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="575fc-177">A migrálás egyszerűsítése az Exportálás használatával</span><span class="sxs-lookup"><span data-stu-id="575fc-177">Simplify migration using Export</span></span>

<span data-ttu-id="575fc-178">Az **Export függvény használatával** rögzítheti az új konszolidált struktúrában használnia szükséges előfizetéseket:</span><span class="sxs-lookup"><span data-stu-id="575fc-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="575fc-179">Az **ügyfelek listájának** Partnerközpont válassza az Ügyfelek lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="575fc-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="575fc-180">Nyissa meg a kívánt ügyfélnevet.</span><span class="sxs-lookup"><span data-stu-id="575fc-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="575fc-181">Az **Előfizetések lapon** válassza az **Előfizetések exportálása** lehetőséget az előfizetések részleteinek Excel-fájlba való exportálásához.</span><span class="sxs-lookup"><span data-stu-id="575fc-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="575fc-182">Ezzel a listával újra létrehozhatja az előfizetéseket az új összevont bérlőben.</span><span class="sxs-lookup"><span data-stu-id="575fc-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="575fc-183">API-regisztráció</span><span class="sxs-lookup"><span data-stu-id="575fc-183">API registration</span></span>

<span data-ttu-id="575fc-184">További információ az API-regisztrációról: [API-hozzáférés beállítása a Partnerközpont.](/partner-center/develop/set-up-api-access-in-partner-center)</span><span class="sxs-lookup"><span data-stu-id="575fc-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="575fc-185">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="575fc-185">Next steps</span></span>

- [<span data-ttu-id="575fc-186">Felhőszolgáltató piacok és pénznemek, ahol CSP-ajánlatokat értékesíthet</span><span class="sxs-lookup"><span data-stu-id="575fc-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
