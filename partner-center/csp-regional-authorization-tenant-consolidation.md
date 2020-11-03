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
ms.openlocfilehash: 0ae107c005eaf6b8ff8a6d99a91075ebc560cf81
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/13/2020
ms.locfileid: "92530252"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="486ee-104">Útmutató a CSP regionális engedélyezési bérlői összevonásához</span><span class="sxs-lookup"><span data-stu-id="486ee-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="486ee-105">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="486ee-105">**Applies to**</span></span>

-  <span data-ttu-id="486ee-106">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="486ee-106">Partner Center</span></span>
-  <span data-ttu-id="486ee-107">Az USA kormányzati szerveinek Microsoft Cloud a partneri központ</span><span class="sxs-lookup"><span data-stu-id="486ee-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="486ee-108">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="486ee-108">**Appropriate roles**</span></span>

- <span data-ttu-id="486ee-109">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="486ee-109">Global admin</span></span>
- <span data-ttu-id="486ee-110">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="486ee-110">Admin agent</span></span>

<span data-ttu-id="486ee-111">\[Néhány információ az előzetesen kiadott termékhez kapcsolódik, amely jelentősen módosítható a kereskedelmi forgalomba bocsátás előtt.</span><span class="sxs-lookup"><span data-stu-id="486ee-111">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="486ee-112">A Microsoft nem vállal kifejezett vagy törvényi garanciát az itt megjelenő információért.\]</span><span class="sxs-lookup"><span data-stu-id="486ee-112">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="486ee-113">A bérlőket összevonhatja a vállalata számára.</span><span class="sxs-lookup"><span data-stu-id="486ee-113">You can consolidate tenants for your business.</span></span> <span data-ttu-id="486ee-114">Ezekkel az utasításokkal összevonhatja a bérlőket a különböző országokban/régiókban.</span><span class="sxs-lookup"><span data-stu-id="486ee-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="486ee-115">Tisztában kell lennie az összes olyan kiosztott előfizetéssel és licenccel, amely az Ön által használt fiókban található ügyfelekre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="486ee-115">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="486ee-116">Az áttelepítési folyamat részeként ugyanezeket a pontos előfizetéseket fogja újból kiépíteni az új központi CSP-fiókban.</span><span class="sxs-lookup"><span data-stu-id="486ee-116">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="486ee-117">Az exportálási lista funkció segítségével létrehozhat egy listát azokról az ügyfelekről, amelyek áthelyezhetők a központi bérlőbe.</span><span class="sxs-lookup"><span data-stu-id="486ee-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="486ee-118">A konszolidáció befejezése után nem lehet visszaállítani az előző bérlői állapotot.</span><span class="sxs-lookup"><span data-stu-id="486ee-118">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="486ee-119">Az ügyfél beavatkozására is szükség lehet.</span><span class="sxs-lookup"><span data-stu-id="486ee-119">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="486ee-120">Előkészületek a migráláshoz</span><span class="sxs-lookup"><span data-stu-id="486ee-120">Prepare for migration</span></span>

- <span data-ttu-id="486ee-121">Jelentkezzen be a **partner Centerbe**  az **átváltási** fiók használatával (amely az új fiókra fog áttérni), és tekintse át az ügyfelek számára kiosztott összes ügyfelet és szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="486ee-121">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="486ee-122">Jelentkezzen ki ebből a fiókból.</span><span class="sxs-lookup"><span data-stu-id="486ee-122">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="486ee-123">Felhasználói fiókok áttelepíthetők</span><span class="sxs-lookup"><span data-stu-id="486ee-123">Migrate customer accounts</span></span>

1. <span data-ttu-id="486ee-124">Jelentkezzen be a **partner Centerbe**  az **áttérési** (új) fiókkal (amely az ügyfeleket áthelyezi).</span><span class="sxs-lookup"><span data-stu-id="486ee-124">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="486ee-125">Válassza az **Ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="486ee-125">Select **Customers** .</span></span>

3. <span data-ttu-id="486ee-126">Kattintson **a viszonteladói kapcsolat kérése** elemre.</span><span class="sxs-lookup"><span data-stu-id="486ee-126">Click **Request a reseller relationship** .</span></span> <span data-ttu-id="486ee-127">Az ügyfeleknek küldött alapértelmezett e-mail-üzenet jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="486ee-127">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="486ee-128">Ez az üzenet egy olyan URL-címet tartalmaz, amely az új partner Center-fiókban egyedi szervezeti AZONOSÍTÓval rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="486ee-128">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="486ee-129">**Ügyfél-művelet:** Győződjön meg arról, hogy az áttelepíteni kívánt összes aktív ügyfél meglátogatja ezt az URL-címet.</span><span class="sxs-lookup"><span data-stu-id="486ee-129">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="486ee-130">Az URL megnyitásakor a rendszer felszólítja az ügyfelet, hogy jelentkezzen be az Office 365 portálra.</span><span class="sxs-lookup"><span data-stu-id="486ee-130">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="486ee-131">Az ügyfél ugyanazzal a szervezeti AZONOSÍTÓval jelentkezik be, amelyet az Azure-és Office 365 felügyeleti portálok elérésére használ.</span><span class="sxs-lookup"><span data-stu-id="486ee-131">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="486ee-132">Bejelentkezés után az **ügyfél fiókjának** globális rendszergazdája megkéri, hogy küldjön be egy szerződést, amely delegált rendszergazdai jogosultságokat biztosít az új CSP-fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="486ee-132">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="486ee-133">Ha elfogadják, az ügyfél kiválasztja a jelölőnégyzetet, és elfogadja a kapcsolat engedélyezését.</span><span class="sxs-lookup"><span data-stu-id="486ee-133">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="486ee-134">Az ügyfelek a partner ügyfeleinek listájában jelennek meg, miután elküldték a szerződést, egyenként.</span><span class="sxs-lookup"><span data-stu-id="486ee-134">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="486ee-135">Office 365-és nem Azure-alapú használati előfizetés áttelepítése</span><span class="sxs-lookup"><span data-stu-id="486ee-135">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="486ee-136">Miután az ügyfél aláírta a szerződést, újra létrehozhatja előfizetéseit a központi partner bérlője alatt.</span><span class="sxs-lookup"><span data-stu-id="486ee-136">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="486ee-137">A **partner Centerben** válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="486ee-137">From **Partner Center** select **Customers** .</span></span>

3. <span data-ttu-id="486ee-138">Nyissa meg az áttelepíteni kívánt ügyfél vállalatának nevét.</span><span class="sxs-lookup"><span data-stu-id="486ee-138">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="486ee-139">Válassza az **előfizetés hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="486ee-139">Select **Add subscription** .</span></span>

5. <span data-ttu-id="486ee-140">Adja hozzá a megfelelő előfizetéseket és a licencek számát a katalógusból.</span><span class="sxs-lookup"><span data-stu-id="486ee-140">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="486ee-141">Győződjön meg arról, hogy az **áttérés** partneri fiókokból című témakörben szereplő információk szerepelnek.</span><span class="sxs-lookup"><span data-stu-id="486ee-141">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="ügyfelek listája":::

6. <span data-ttu-id="486ee-143">Kattintson a **Submit (küldés) gombra.**</span><span class="sxs-lookup"><span data-stu-id="486ee-143">Click **Submit.**</span></span>

   <span data-ttu-id="486ee-144">A szolgáltatásokat mostantól a partner fiókba való **áttéréssel** biztosítjuk az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="486ee-144">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="486ee-145">Ismételje meg ezeket a lépéseket az előfizetések áttelepíteni az összes további ügyfélre.</span><span class="sxs-lookup"><span data-stu-id="486ee-145">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="486ee-146">Mielőtt továbblép a következő szakaszra, gondoskodjon arról, hogy a partneri fiókokba **való áttérés** alatt meglévő összes ügyfél-előfizetés újra kiépítve legyen a partner fiókba való **áttérés** alatt.</span><span class="sxs-lookup"><span data-stu-id="486ee-146">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="486ee-147">A partnereknek meg kell függeszteniük **az előfizetéseket a fiókpartner** partner bérlői fiókjából a partner Centerben, hogy az előfizetések átkerülnek **a partner központ partner** bérlői fiókjába, hogy a kettős számlázás ne történjen meg.</span><span class="sxs-lookup"><span data-stu-id="486ee-147">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="486ee-148">A támogatási kérelmeket a rendszer megtagadja a jóváírások miatt, mert a számlázás olyan átfedésben van, amely nem megfelelően tiltja le az előfizetések közötti **váltást** .</span><span class="sxs-lookup"><span data-stu-id="486ee-148">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="486ee-149">Az Office 365-előfizetések letiltása a partneri fiókból való áttérés alatt</span><span class="sxs-lookup"><span data-stu-id="486ee-149">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="486ee-150">Ha letiltja a CSP-előfizetést a partneri fiókokból **való áttérés alatt,** a jövőben nem számítunk fel díjat</span><span class="sxs-lookup"><span data-stu-id="486ee-150">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="486ee-151">Nem kell manuálisan letiltania az Azure-előfizetéseket, mert az Azure-előfizetések automatikusan le vannak tiltva az áttelepítési folyamat során.</span><span class="sxs-lookup"><span data-stu-id="486ee-151">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="486ee-152">Jelentkezzen be a **partner Centerbe** az **áttérés CSP-** fiókjából, és navigáljon az ügyfél listához.</span><span class="sxs-lookup"><span data-stu-id="486ee-152">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="486ee-153">Nyissa meg a letiltani kívánt előfizetésekkel rendelkező ügyfelet, majd válassza ki az első letiltani ajánlatot.</span><span class="sxs-lookup"><span data-stu-id="486ee-153">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="486ee-154">Állítsa az előfizetést **felfüggesztve** értékre, majd kattintson a **Submit (Küldés** ) gombra.</span><span class="sxs-lookup"><span data-stu-id="486ee-154">Set the subscription to **suspended** , and then click **submit** .</span></span>

   >[!Note]
   ><span data-ttu-id="486ee-155">Az előfizetés felfüggesztése biztosítja a kettős számlázást.</span><span class="sxs-lookup"><span data-stu-id="486ee-155">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="486ee-156">Az előfizetés fel van **függesztve** az előfizetések listáján.</span><span class="sxs-lookup"><span data-stu-id="486ee-156">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="486ee-157">Ismételje meg ezeket a lépéseket az ügyfélhez tartozó összes előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="486ee-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="486ee-158">Ellenőrizze az összes **felfüggesztett** megjelenítést.</span><span class="sxs-lookup"><span data-stu-id="486ee-158">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="486ee-159">Válassza ki a következő ügyfelet a listán, és ismételje meg az összes előfizetés letiltásának folyamatát.</span><span class="sxs-lookup"><span data-stu-id="486ee-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="486ee-160">Azure-alapú használati előfizetés áttelepítése</span><span class="sxs-lookup"><span data-stu-id="486ee-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="486ee-161">Az Office 365 CSP-előfizetésekkel ellentétben az Azure-ban nem kell manuálisan áttelepíteni a használati alapú CSP-előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="486ee-161">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="486ee-162">Microsoft Azure támogatás áttelepíti az Azure-előfizetéseket, valamint az összes telepített szolgáltatást vagy erőforrást **a CSP-** viszonteladói fiókoktól a CSP-viszonteladói fiókra **való áttéréstől** .</span><span class="sxs-lookup"><span data-stu-id="486ee-162">Microsoft Azure Support will migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="486ee-163">Az áttelepítés során az ügyfél nem zavarja a szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="486ee-163">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="486ee-164">Győződjön meg arról, hogy az Azure-előfizetésekkel rendelkező felhasználói fiókok elfogadták az új, CSP-re **való áttéréssel** kapcsolatos szerződést.</span><span class="sxs-lookup"><span data-stu-id="486ee-164">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="486ee-165">Értesíteni fogja a Microsoftot arról, hogy mely ügyfél-fiókok állnak készen az áttelepítésre, és adja meg az ügyfél vállalatának nevét.</span><span class="sxs-lookup"><span data-stu-id="486ee-165">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="486ee-166">A Microsoft áttelepíti az Azure-beli használaton alapuló előfizetéseket, és értesíti az áttelepítés befejezésekor.</span><span class="sxs-lookup"><span data-stu-id="486ee-166">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="486ee-167">Győződjön meg arról, hogy az Azure-előfizetés a CSP-viszonteladói fiókra történő **áttérés** alatt most már fel van **függesztve** a partner Centerben az ügyfél-előfizetések szakaszban.</span><span class="sxs-lookup"><span data-stu-id="486ee-167">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="486ee-168">Győződjön meg arról, hogy az Azure **-** előfizetés a CSP-viszonteladói fiókra történő áttérés alatt most az ügyfél-előfizetések szakaszban az **aktív** a partneri központban állapotot jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="486ee-168">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="486ee-169">Az ügyfél-előfizetések letiltása nem módosítja az ügyfél megjelenését az ügyfelek listájában.</span><span class="sxs-lookup"><span data-stu-id="486ee-169">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="486ee-170">Jelenleg nincs lehetőség az ügyfelek eltávolítására a listából.</span><span class="sxs-lookup"><span data-stu-id="486ee-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="486ee-171">A partnereknek kerülniük kell az előfizetések hozzáadását az ügyfeleknek **a fiókból a jövőben** .</span><span class="sxs-lookup"><span data-stu-id="486ee-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="486ee-172">Ismételje meg ezeket a lépéseket az összes ügyfél összes előfizetése számára, hogy leállítsa a jövőbeli díjakat a fiók (ok) **ról való áttéréskor** .</span><span class="sxs-lookup"><span data-stu-id="486ee-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="486ee-173">A partner a lemondás napja és a számlázási időszak utolsó napján a használaton kívüli napok száma után egy végső számlát kap.</span><span class="sxs-lookup"><span data-stu-id="486ee-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="486ee-174">A végső számlázási időszak után nem fog létrejönni jövőbeli számla.</span><span class="sxs-lookup"><span data-stu-id="486ee-174">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="486ee-175">További információ</span><span class="sxs-lookup"><span data-stu-id="486ee-175">Additional information</span></span>

- <span data-ttu-id="486ee-176">Ha letiltotta az előfizetést a CSP-fiókból **való áttérésből** , az előfizetés letiltását megelőzően nem **befolyásolja a végfelhasználó** szolgáltatását.</span><span class="sxs-lookup"><span data-stu-id="486ee-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="486ee-177">Az ügyfelek nem használhatják az előfizetéseket, és nem hozhatnak fel díjat a felfüggesztés vagy a visszavonás után.</span><span class="sxs-lookup"><span data-stu-id="486ee-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="486ee-178">Jelenleg nem lehet teljesen eltávolítani az ügyfelet az **ügyfelek** listájáról.</span><span class="sxs-lookup"><span data-stu-id="486ee-178">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="486ee-179">A partnereknek meg kell függeszteniük az előfizetéseket a fiókpartner partner bérlői fiókjából való **áttéréskor** , az előfizetések pedig a fiókhoz való áttérés alatt **, a kettős** számlázás biztosításához pedig az áttelepítés alatt állnak.</span><span class="sxs-lookup"><span data-stu-id="486ee-179">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="486ee-180">A Microsoft nem támogatja a kreditek iránti kérelmeket, mert a számlázás olyan átfedésben van, amely nem megfelelően van beállítva az előfizetések felfüggesztésére való **áttéréskor** .</span><span class="sxs-lookup"><span data-stu-id="486ee-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="486ee-181">Az áttelepítés egyszerűbbé tétele az exportálással</span><span class="sxs-lookup"><span data-stu-id="486ee-181">Simplify migration using Export</span></span>

<span data-ttu-id="486ee-182">Az **Exportálás funkcióval** rögzítheti az új összevont struktúrában használni kívánt előfizetéseket:</span><span class="sxs-lookup"><span data-stu-id="486ee-182">Using the **Export Function** , you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="486ee-183">Az ügyfelek listájának megtekintéséhez kattintson a partner központ **ügyfelei** elemére.</span><span class="sxs-lookup"><span data-stu-id="486ee-183">Click **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="486ee-184">Nyissa meg a kívánt ügyfél nevét.</span><span class="sxs-lookup"><span data-stu-id="486ee-184">Open the desired customer name.</span></span>

3. <span data-ttu-id="486ee-185">Az **előfizetések** lapon kattintson az **előfizetések exportálása** lehetőségre, hogy az előfizetések adatait egy Excel-fájlba exportálja.</span><span class="sxs-lookup"><span data-stu-id="486ee-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="486ee-186">Ezzel a listával újból létrehozhatja az előfizetéseket az új konszolidált bérlőben.</span><span class="sxs-lookup"><span data-stu-id="486ee-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="486ee-187">API-regisztráció</span><span class="sxs-lookup"><span data-stu-id="486ee-187">API registration</span></span>

<span data-ttu-id="486ee-188">Az API-regisztrációval kapcsolatos további információkért lásd: [API-hozzáférés beállítása a partner Centerben](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="486ee-188">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="486ee-189">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="486ee-189">Next steps</span></span>

- [<span data-ttu-id="486ee-190">A Cloud Solution Provider program regionális piacai és pénznemei, amelyekben a CSP-ajánlatok értékesíthetők</span><span class="sxs-lookup"><span data-stu-id="486ee-190">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
