---
title: CSP regionális engedélyezési bérlői konszolidáció
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezekkel az utasításokkal összevonhatja a bérlőket a különböző országokban/régiókban. Ez magában foglalja a felhasználói fiókok és az ügyfél-előfizetések áttelepíthető lépéseit.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2171e2b10101e99bdd8d415a936ba98af65c2a1b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502570"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="32d9c-104">Útmutató a CSP regionális engedélyezési bérlőösszevonáshoz</span><span class="sxs-lookup"><span data-stu-id="32d9c-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="32d9c-105">**A következőre érvényes:**</span><span class="sxs-lookup"><span data-stu-id="32d9c-105">**Applies to**</span></span>

- <span data-ttu-id="32d9c-106">A Microsoft Cloud for US Government Partnerközpontja</span><span class="sxs-lookup"><span data-stu-id="32d9c-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="32d9c-107">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="32d9c-107">**Appropriate roles**</span></span>

- <span data-ttu-id="32d9c-108">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="32d9c-108">Global admin</span></span>
- <span data-ttu-id="32d9c-109">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="32d9c-109">Admin agent</span></span>

<span data-ttu-id="32d9c-110">\[Néhány információ az előzetesen kiadott termékhez kapcsolódik, amely jelentősen módosítható a kereskedelmi forgalomba bocsátás előtt.</span><span class="sxs-lookup"><span data-stu-id="32d9c-110">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="32d9c-111">A Microsoft nem vállal kifejezett vagy törvényi garanciát az itt megjelenő információért.\]</span><span class="sxs-lookup"><span data-stu-id="32d9c-111">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="32d9c-112">A bérlőket összevonhatja a vállalata számára.</span><span class="sxs-lookup"><span data-stu-id="32d9c-112">You can consolidate tenants for your business.</span></span> <span data-ttu-id="32d9c-113">Ezekkel az utasításokkal összevonhatja a bérlőket a különböző országokban/régiókban.</span><span class="sxs-lookup"><span data-stu-id="32d9c-113">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="32d9c-114">Tisztában kell lennie az összes olyan kiosztott előfizetéssel és licenccel, amely az Ön által használt fiókban található ügyfelekre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="32d9c-114">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="32d9c-115">Az áttelepítési folyamat részeként ugyanezeket a pontos előfizetéseket fogja újból kiépíteni az új központi CSP-fiókban.</span><span class="sxs-lookup"><span data-stu-id="32d9c-115">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="32d9c-116">Az exportálási lista funkció segítségével létrehozhat egy listát azokról az ügyfelekről, amelyek áthelyezhetők a központi bérlőbe.</span><span class="sxs-lookup"><span data-stu-id="32d9c-116">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="32d9c-117">A konszolidáció befejezése után nem lehet visszaállítani az előző bérlői állapotot.</span><span class="sxs-lookup"><span data-stu-id="32d9c-117">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="32d9c-118">Az ügyfél beavatkozására is szükség lehet.</span><span class="sxs-lookup"><span data-stu-id="32d9c-118">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="32d9c-119">Előkészületek a migráláshoz</span><span class="sxs-lookup"><span data-stu-id="32d9c-119">Prepare for migration</span></span>

- <span data-ttu-id="32d9c-120">Jelentkezzen be a **partner Centerbe**  az **átváltási** fiók használatával (amely az új fiókra fog áttérni), és tekintse át az ügyfelek számára kiosztott összes ügyfelet és szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="32d9c-120">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="32d9c-121">Jelentkezzen ki ebből a fiókból.</span><span class="sxs-lookup"><span data-stu-id="32d9c-121">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="32d9c-122">Felhasználói fiókok áttelepíthetők</span><span class="sxs-lookup"><span data-stu-id="32d9c-122">Migrate customer accounts</span></span>

1. <span data-ttu-id="32d9c-123">Jelentkezzen be a **partner Centerbe**  az **áttérési** (új) fiókkal (amely az ügyfeleket áthelyezi).</span><span class="sxs-lookup"><span data-stu-id="32d9c-123">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="32d9c-124">Válassza az **Ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="32d9c-124">Select **Customers**.</span></span>

3. <span data-ttu-id="32d9c-125">Válassza **a viszonteladói kapcsolat kérése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="32d9c-125">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="32d9c-126">Az ügyfeleknek küldött alapértelmezett e-mail-üzenet jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="32d9c-126">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="32d9c-127">Ez az üzenet egy olyan URL-címet tartalmaz, amely az új partner Center-fiókban egyedi szervezeti AZONOSÍTÓval rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="32d9c-127">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="32d9c-128">**Ügyfél-művelet:** Győződjön meg arról, hogy az áttelepíteni kívánt összes aktív ügyfél meglátogatja ezt az URL-címet.</span><span class="sxs-lookup"><span data-stu-id="32d9c-128">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="32d9c-129">Az URL megnyitásakor a rendszer felszólítja az ügyfelet, hogy jelentkezzen be az Office 365 portálra.</span><span class="sxs-lookup"><span data-stu-id="32d9c-129">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="32d9c-130">Az ügyfél ugyanazzal a szervezeti AZONOSÍTÓval jelentkezik be, amelyet az Azure-és Office 365 felügyeleti portálok elérésére használ.</span><span class="sxs-lookup"><span data-stu-id="32d9c-130">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="32d9c-131">Bejelentkezés után az **ügyfél fiókjának** globális rendszergazdája megkéri, hogy küldjön be egy szerződést, amely delegált rendszergazdai jogosultságokat biztosít az új CSP-fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="32d9c-131">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="32d9c-132">Ha elfogadják, az ügyfél kiválasztja a jelölőnégyzetet, és elfogadja a kapcsolat engedélyezését.</span><span class="sxs-lookup"><span data-stu-id="32d9c-132">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="32d9c-133">Az ügyfelek a partner ügyfeleinek listájában jelennek meg, miután elküldték a szerződést, egyenként.</span><span class="sxs-lookup"><span data-stu-id="32d9c-133">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="32d9c-134">Office 365-és nem Azure-alapú használati előfizetés áttelepítése</span><span class="sxs-lookup"><span data-stu-id="32d9c-134">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="32d9c-135">Miután az ügyfél aláírta a szerződést, újra létrehozhatja előfizetéseit a központi partner bérlője alatt.</span><span class="sxs-lookup"><span data-stu-id="32d9c-135">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="32d9c-136">A **partner Centerben** válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="32d9c-136">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="32d9c-137">Nyissa meg az áttelepíteni kívánt ügyfél vállalatának nevét.</span><span class="sxs-lookup"><span data-stu-id="32d9c-137">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="32d9c-138">Válassza az **előfizetés hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="32d9c-138">Select **Add subscription**.</span></span>

5. <span data-ttu-id="32d9c-139">Adja hozzá a megfelelő előfizetéseket és a licencek számát a katalógusból.</span><span class="sxs-lookup"><span data-stu-id="32d9c-139">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="32d9c-140">Győződjön meg arról, hogy az **áttérés** partneri fiókokból című témakörben szereplő információk szerepelnek.</span><span class="sxs-lookup"><span data-stu-id="32d9c-140">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="ügyfelek listája":::

6. <span data-ttu-id="32d9c-142">Válassza a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="32d9c-142">Select **Submit.**</span></span>

   <span data-ttu-id="32d9c-143">A szolgáltatásokat mostantól a partner fiókba való **áttéréssel** biztosítjuk az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="32d9c-143">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="32d9c-144">Ismételje meg ezeket a lépéseket az előfizetések áttelepíteni az összes további ügyfélre.</span><span class="sxs-lookup"><span data-stu-id="32d9c-144">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="32d9c-145">Mielőtt továbblép a következő szakaszra, gondoskodjon arról, hogy a partneri fiókokba **való áttérés** alatt meglévő összes ügyfél-előfizetés újra kiépítve legyen a partner fiókba való **áttérés** alatt.</span><span class="sxs-lookup"><span data-stu-id="32d9c-145">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="32d9c-146">A partnereknek meg kell függeszteniük **az előfizetéseket a fiókpartner** partner bérlői fiókjából a partner Centerben, hogy az előfizetések átkerülnek **a partner központ partner** bérlői fiókjába, hogy a kettős számlázás ne történjen meg.</span><span class="sxs-lookup"><span data-stu-id="32d9c-146">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="32d9c-147">A támogatási kérelmeket a rendszer megtagadja a jóváírások miatt, mert a számlázás olyan átfedésben van, amely nem megfelelően tiltja le az előfizetések közötti **váltást** .</span><span class="sxs-lookup"><span data-stu-id="32d9c-147">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="32d9c-148">Az Office 365-előfizetések letiltása a partneri fiókból való áttérés alatt</span><span class="sxs-lookup"><span data-stu-id="32d9c-148">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="32d9c-149">Ha letiltja a CSP-előfizetést a partneri fiókokból **való áttérés alatt,** a jövőben nem számítunk fel díjat</span><span class="sxs-lookup"><span data-stu-id="32d9c-149">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="32d9c-150">Nem kell manuálisan letiltania az Azure-előfizetéseket, mert az Azure-előfizetések automatikusan le vannak tiltva az áttelepítési folyamat során.</span><span class="sxs-lookup"><span data-stu-id="32d9c-150">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="32d9c-151">Jelentkezzen be a **partner Centerbe** az **áttérés CSP-** fiókjából, és navigáljon az ügyfél listához.</span><span class="sxs-lookup"><span data-stu-id="32d9c-151">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="32d9c-152">Nyissa meg a letiltani kívánt előfizetésekkel rendelkező ügyfelet, majd válassza ki az első letiltani ajánlatot.</span><span class="sxs-lookup"><span data-stu-id="32d9c-152">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="32d9c-153">Állítsa az előfizetést **felfüggesztve** értékre, majd válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="32d9c-153">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="32d9c-154">Az előfizetés felfüggesztése biztosítja a kettős számlázást.</span><span class="sxs-lookup"><span data-stu-id="32d9c-154">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="32d9c-155">Az előfizetés fel van **függesztve** az előfizetések listáján.</span><span class="sxs-lookup"><span data-stu-id="32d9c-155">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="32d9c-156">Ismételje meg ezeket a lépéseket az ügyfélhez tartozó összes előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="32d9c-156">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="32d9c-157">Ellenőrizze az összes **felfüggesztett** megjelenítést.</span><span class="sxs-lookup"><span data-stu-id="32d9c-157">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="32d9c-158">Válassza ki a következő ügyfelet a listán, és ismételje meg az összes előfizetés letiltásának folyamatát.</span><span class="sxs-lookup"><span data-stu-id="32d9c-158">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="32d9c-159">Azure-alapú használati előfizetés áttelepítése</span><span class="sxs-lookup"><span data-stu-id="32d9c-159">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="32d9c-160">Az Office 365 CSP-előfizetésekkel ellentétben az Azure-ban nem kell manuálisan áttelepíteni a használati alapú CSP-előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="32d9c-160">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="32d9c-161">Microsoft Azure támogatás áttelepíti az Azure-előfizetéseket **és az összes** telepített szolgáltatást vagy erőforrást a CSP-viszonteladói fiókoktól a CSP viszonteladói fiókra **való áttéréstől** .</span><span class="sxs-lookup"><span data-stu-id="32d9c-161">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="32d9c-162">Az áttelepítés során az ügyfél nem zavarja a szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="32d9c-162">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="32d9c-163">Győződjön meg arról, hogy az Azure-előfizetésekkel rendelkező felhasználói fiókok elfogadták az új, CSP-re **való áttéréssel** kapcsolatos szerződést.</span><span class="sxs-lookup"><span data-stu-id="32d9c-163">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="32d9c-164">Értesíteni fogja a Microsoftot arról, hogy mely ügyfél-fiókok állnak készen az áttelepítésre, és adja meg az ügyfél vállalatának nevét.</span><span class="sxs-lookup"><span data-stu-id="32d9c-164">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="32d9c-165">A Microsoft áttelepíti az Azure-beli használaton alapuló előfizetéseket, és értesíti az áttelepítés befejezésekor.</span><span class="sxs-lookup"><span data-stu-id="32d9c-165">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="32d9c-166">Győződjön meg arról, hogy az Azure-előfizetés a CSP-viszonteladói fiókra történő **áttérés** alatt most már fel van **függesztve** a partner Centerben az ügyfél-előfizetések szakaszban.</span><span class="sxs-lookup"><span data-stu-id="32d9c-166">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="32d9c-167">Győződjön meg arról, hogy az Azure **-** előfizetés a CSP-viszonteladói fiókra történő áttérés alatt most az ügyfél-előfizetések szakaszban az **aktív** a partneri központban állapotot jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="32d9c-167">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="32d9c-168">Az ügyfél-előfizetések letiltása nem módosítja az ügyfél megjelenését az ügyfelek listájában.</span><span class="sxs-lookup"><span data-stu-id="32d9c-168">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="32d9c-169">Jelenleg nincs lehetőség az ügyfelek eltávolítására a listából.</span><span class="sxs-lookup"><span data-stu-id="32d9c-169">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="32d9c-170">A partnereknek kerülniük kell az előfizetések hozzáadását az ügyfeleknek **a fiókból a jövőben** .</span><span class="sxs-lookup"><span data-stu-id="32d9c-170">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="32d9c-171">Ismételje meg ezeket a lépéseket az összes ügyfél összes előfizetése számára, hogy leállítsa a jövőbeli díjakat a fiók (ok) **ról való áttéréskor** .</span><span class="sxs-lookup"><span data-stu-id="32d9c-171">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="32d9c-172">A partner a lemondás napja és a számlázási időszak utolsó napján a használaton kívüli napok száma után egy végső számlát kap.</span><span class="sxs-lookup"><span data-stu-id="32d9c-172">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="32d9c-173">A végső számlázási időszak után nem fog létrejönni jövőbeli számla.</span><span class="sxs-lookup"><span data-stu-id="32d9c-173">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="32d9c-174">További információ</span><span class="sxs-lookup"><span data-stu-id="32d9c-174">Additional information</span></span>

- <span data-ttu-id="32d9c-175">Ha letiltotta az előfizetést a CSP-fiókból **való áttérésből** , az előfizetés letiltását megelőzően nem **befolyásolja a végfelhasználó** szolgáltatását.</span><span class="sxs-lookup"><span data-stu-id="32d9c-175">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="32d9c-176">Az ügyfelek nem használhatják az előfizetéseket, és nem hozhatnak fel díjat a felfüggesztés vagy a visszavonás után.</span><span class="sxs-lookup"><span data-stu-id="32d9c-176">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="32d9c-177">Jelenleg nem lehet teljesen eltávolítani az ügyfelet az **ügyfelek** listájáról.</span><span class="sxs-lookup"><span data-stu-id="32d9c-177">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="32d9c-178">A partnereknek meg kell függeszteniük az előfizetéseket a fiókpartner partner bérlői fiókjából való **áttéréskor** , az előfizetések pedig a fiókhoz való áttérés alatt **, a kettős** számlázás biztosításához pedig az áttelepítés alatt állnak.</span><span class="sxs-lookup"><span data-stu-id="32d9c-178">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="32d9c-179">A Microsoft nem támogatja a kreditek iránti kérelmeket, mert a számlázás olyan átfedésben van, amely nem megfelelően van beállítva az előfizetések felfüggesztésére való **áttéréskor** .</span><span class="sxs-lookup"><span data-stu-id="32d9c-179">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="32d9c-180">Az áttelepítés egyszerűbbé tétele az exportálással</span><span class="sxs-lookup"><span data-stu-id="32d9c-180">Simplify migration using Export</span></span>

<span data-ttu-id="32d9c-181">Az **Exportálás funkcióval** rögzítheti az új összevont struktúrában használni kívánt előfizetéseket:</span><span class="sxs-lookup"><span data-stu-id="32d9c-181">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="32d9c-182">Válassza ki az **ügyfeleket** a partner központban az ügyfelek listájának megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="32d9c-182">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="32d9c-183">Nyissa meg a kívánt ügyfél nevét.</span><span class="sxs-lookup"><span data-stu-id="32d9c-183">Open the desired customer name.</span></span>

3. <span data-ttu-id="32d9c-184">Az **előfizetések** lapon válassza az előfizetések **exportálása** lehetőséget, hogy egy Excel-fájlba exportálja az előfizetések részleteit.</span><span class="sxs-lookup"><span data-stu-id="32d9c-184">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="32d9c-185">Ezzel a listával újból létrehozhatja az előfizetéseket az új konszolidált bérlőben.</span><span class="sxs-lookup"><span data-stu-id="32d9c-185">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="32d9c-186">API-regisztráció</span><span class="sxs-lookup"><span data-stu-id="32d9c-186">API registration</span></span>

<span data-ttu-id="32d9c-187">Az API-regisztrációval kapcsolatos további információkért lásd: [API-hozzáférés beállítása a partner Centerben](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="32d9c-187">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="32d9c-188">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="32d9c-188">Next steps</span></span>

- [<span data-ttu-id="32d9c-189">A Cloud Solution Provider program regionális piacai és pénznemei, amelyekben a CSP-ajánlatok értékesíthetők</span><span class="sxs-lookup"><span data-stu-id="32d9c-189">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
