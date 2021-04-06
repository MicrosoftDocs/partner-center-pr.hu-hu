---
title: Ügyfél-előfizetések létrehozása a partner Centerben
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan értékesítheti az ügyfeleknek a Microsoft által közzétett, valamint a harmadik féltől származó független szoftvergyártók által közzétett SaaS-termékek előfizetéseit.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 559d1fbd2efc1417ae89931279b9d3c9a1d67f7c
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502935"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="26ba2-103">Ügyfél-előfizetések létrehozása, felfüggesztése vagy lemondása</span><span class="sxs-lookup"><span data-stu-id="26ba2-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="26ba2-104">**A következőre érvényes:**</span><span class="sxs-lookup"><span data-stu-id="26ba2-104">**Applies to**</span></span>

- <span data-ttu-id="26ba2-105">A Microsoft Cloud for US Government Partnerközpontja</span><span class="sxs-lookup"><span data-stu-id="26ba2-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="26ba2-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="26ba2-106">**Appropriate roles**</span></span>

- <span data-ttu-id="26ba2-107">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="26ba2-107">Admin agent</span></span>
- <span data-ttu-id="26ba2-108">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="26ba2-108">Billing admin</span></span>
- <span data-ttu-id="26ba2-109">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="26ba2-109">Global admin</span></span>
- <span data-ttu-id="26ba2-110">Segélyszolgálat ügynöke</span><span class="sxs-lookup"><span data-stu-id="26ba2-110">Helpdesk agent</span></span>
- <span data-ttu-id="26ba2-111">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="26ba2-111">Sales agent</span></span>

<span data-ttu-id="26ba2-112">Miután létrehozott egy rekordot az ügyfélről a partner Centerben, a katalógusban lévő termékek előfizetéseit is értékesítheti.</span><span class="sxs-lookup"><span data-stu-id="26ba2-112">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="26ba2-113">Ide tartoznak a Microsoft és a szolgáltatott szoftverek (SaaS) által közzétett, harmadik féltől származó független szoftvergyártók által közzétett termékek a [kereskedelmi piactéren](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="26ba2-113">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="26ba2-114">Egyes ajánlatok felhasználónként egy előfizetésre korlátozódnak.</span><span class="sxs-lookup"><span data-stu-id="26ba2-114">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="26ba2-115">Ha szeretné megtekinteni, hogy mely ajánlatok vannak korlátozva, látogasson el a partner Center díjszabási és ajánlatok oldalára.</span><span class="sxs-lookup"><span data-stu-id="26ba2-115">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="26ba2-116">A CSP programban partnerként vásárolhat **licenc-alapú** vagy **mért** SaaS-előfizetéseket a partner centeren belüli ISV-közzétevők közül.</span><span class="sxs-lookup"><span data-stu-id="26ba2-116">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="26ba2-117">Ez azt jelenti, hogy vásárolhat bármilyen **licenccel** vagy **mért** SaaS-ajánlatot, amelyet az ISV közzétevő elérhetővé tett, beleértve az [exkluzív ajánlatokat](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) is, amelyekhez hozzáféréssel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="26ba2-117">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="26ba2-118">Ha más, kereskedelmi Piactéri ajánlatokat szeretne megvásárolni vagy kezelni (például Azure-alkalmazásokat,-tárolókat vagy virtuális gépeket érintő használaton alapuló ajánlatokat), akkor a [Azure Portalra](https://portal.azure.com/)kell lépnie.</span><span class="sxs-lookup"><span data-stu-id="26ba2-118">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="26ba2-119">Új előfizetés létrehozása</span><span class="sxs-lookup"><span data-stu-id="26ba2-119">Create a new subscription</span></span>

1. <span data-ttu-id="26ba2-120">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="26ba2-120">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="26ba2-121">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="26ba2-121">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="26ba2-122">Válassza az **előfizetés hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="26ba2-122">Select **Add subscription**.</span></span> <span data-ttu-id="26ba2-123">Az **online szolgáltatások** lapon megjelenik az összes elérhető Piactéri SaaS-ajánlat.</span><span class="sxs-lookup"><span data-stu-id="26ba2-123">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="26ba2-124">Ha csak bizonyos típusú előfizetéseket szeretne látni, a választható szűrők közül választhat:</span><span class="sxs-lookup"><span data-stu-id="26ba2-124">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="26ba2-125">**Közzétevő**: válassza a **Microsoft** lehetőséget, hogy csak a Microsoft által kínált ajánlatokat vagy a **partnert** tekintse meg a független szoftvergyártók által közzétett kereskedelmi Piactéri termékeket.</span><span class="sxs-lookup"><span data-stu-id="26ba2-125">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="26ba2-126">**Számlázási típus**: válassza ki a használni kívánt előfizetés-számlázás típusát: **licenc** vagy **használat**.</span><span class="sxs-lookup"><span data-stu-id="26ba2-126">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="26ba2-127">A havi és éves számlázási gyakorisággal kapcsolatos információkért tekintse meg a [licenc alapú számlázást](license-based-billing.md) ismertető témakört.</span><span class="sxs-lookup"><span data-stu-id="26ba2-127">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="26ba2-128">**Kategória**: válassza a **vállalat**, a **kisvállalat vagy** a **próbaverzió** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="26ba2-128">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="26ba2-129">A próbaverziós előfizetésekkel kapcsolatos információkért tekintse [meg az ügyfelek Microsoft-termékekkel kapcsolatos próbaverzióit](offer-your-customers-trials-of-microsoft-products.md)ismertető témakört.</span><span class="sxs-lookup"><span data-stu-id="26ba2-129">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="26ba2-130">Válassza ki az ügyfél számára megvásárolni kívánt termék-előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="26ba2-130">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="26ba2-131">A megjelenő termékek a vásárlói szegmens típusától (oktatási, kormányzati stb.) és az alkalmazott szűrőktől függenek.</span><span class="sxs-lookup"><span data-stu-id="26ba2-131">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="26ba2-132">Előfordulhat, hogy a piactéren látható egyes ajánlatok nem mindig lesznek elérhetők egy adott ügyfél vagy egy adott CSP-partner számára.</span><span class="sxs-lookup"><span data-stu-id="26ba2-132">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="26ba2-133">Ennek oka a következő lehet:</span><span class="sxs-lookup"><span data-stu-id="26ba2-133">This can be because:</span></span>

   - <span data-ttu-id="26ba2-134">Az ügyfél már rendelkezik előfizetéssel a termékre, és csak egy</span><span class="sxs-lookup"><span data-stu-id="26ba2-134">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="26ba2-135">Előfordulhat, hogy az ügyfél előfizetését felfüggesztették (ebben az esetben újra kell aktiválni az előfizetést, és nem kell újat megvásárolnia.)</span><span class="sxs-lookup"><span data-stu-id="26ba2-135">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="26ba2-136">Az ISV SaaS-ajánlatok esetében előfordulhat, hogy az ajánlat nem érhető el a vásárláshoz: az ISV nem támogatja az ügyfél számlázási országát vagy régióját; lehetséges, hogy az ISV úgy döntött, hogy nem teszi elérhetővé az ajánlatot a CSP programon keresztül; a független szoftvergyártók azonban kizárólag bizonyos CSP- [partnerek számára is](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) elvégezték az ajánlatot.</span><span class="sxs-lookup"><span data-stu-id="26ba2-136">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="26ba2-137">Előfordulhat, hogy az ISV-ajánlat nem hívható le a partneri központon keresztül (például tárolók vagy használaton alapuló ajánlatok).</span><span class="sxs-lookup"><span data-stu-id="26ba2-137">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="26ba2-138">Minden hozzáadni kívánt előfizetéshez adja meg a licencek számát (ha szükséges), és válassza a **Hozzáadás a kosárhoz** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="26ba2-138">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="26ba2-139">Ha elkészült az előfizetések hozzáadásával, válassza a **felülvizsgálat** lehetőséget, és tekintse át a rendelését.</span><span class="sxs-lookup"><span data-stu-id="26ba2-139">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="26ba2-140">Miután áttekintette a rendeléseit, és készen áll az előfizetések megvásárlására, válassza a **vásárlás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="26ba2-140">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="26ba2-141">Miután megvásárolt egy előfizetést az ügyfél számára, a következők történnek:</span><span class="sxs-lookup"><span data-stu-id="26ba2-141">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="26ba2-142">Az előfizetés áttekintéséhez vagy szerkesztéséhez válassza ki az előfizetés nevét az ügyfél **előfizetések** lapján.</span><span class="sxs-lookup"><span data-stu-id="26ba2-142">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="26ba2-143">Innen kiválaszthatja a kiegészítő licenceket, ha vannak ilyenek, módosíthatja a licencek mennyiségét, vagy felfüggesztheti az előfizetést.</span><span class="sxs-lookup"><span data-stu-id="26ba2-143">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="26ba2-144">**ISV SaaS (licenc-alapú és mért) előfizetések esetén:**</span><span class="sxs-lookup"><span data-stu-id="26ba2-144">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="26ba2-145">Az ISV-közzétevő webhelyére mutató hivatkozást fog kapni.</span><span class="sxs-lookup"><span data-stu-id="26ba2-145">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="26ba2-146">Ez a hivatkozás segítséget nyújt az ügyfél előfizetésének üzembe helyezéséhez vagy a fiók beállításának befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="26ba2-146">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="26ba2-147">Sem Ön, sem az ügyfél nem kap e-mailt a fiók beállítása/kiépítés az ilyen típusú ISV-előfizetésben való elvégzéséhez szükséges utasításokkal.)</span><span class="sxs-lookup"><span data-stu-id="26ba2-147">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="26ba2-148">Ha az előfizetése 30 napos ingyenes próbaidőszakot tartalmaz, a rendszer automatikusan alkalmazza az ingyenes próbaidőszakot.</span><span class="sxs-lookup"><span data-stu-id="26ba2-148">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="26ba2-149">A CSP programban partnerként nem lehet lemondani az ingyenes próbaidőszakot az ügyfeleknek megvásárolt ajánlatokról.</span><span class="sxs-lookup"><span data-stu-id="26ba2-149">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="26ba2-150">Az ingyenes próbaidőszak lejárta után megkezdődik az előfizetés időtartama, és az előfizetés fizetett állapotba lesz konvertálva.</span><span class="sxs-lookup"><span data-stu-id="26ba2-150">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="26ba2-151">Az előfizetés ekkor automatikusan megújítható az adott ütemterv szerint.</span><span class="sxs-lookup"><span data-stu-id="26ba2-151">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="26ba2-152">Előfizetések frissítése bővítményekkel</span><span class="sxs-lookup"><span data-stu-id="26ba2-152">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="26ba2-153">Egy bővítmény megvásárlásához az ügyfélnek először aktív alapszintű előfizetéssel kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="26ba2-153">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="26ba2-154">A katalóguson keresztül nem vásárolhat bővítményeket.</span><span class="sxs-lookup"><span data-stu-id="26ba2-154">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="26ba2-155">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="26ba2-155">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="26ba2-156">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="26ba2-156">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="26ba2-157">Válassza ki a kezelni kívánt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="26ba2-157">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="26ba2-158">Az **állapot** szakaszban az előfizetés elérhető bővítményeinek listája látható.</span><span class="sxs-lookup"><span data-stu-id="26ba2-158">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="26ba2-159">Frissítse a licencek mennyiségét az egyes szükséges bővítményekhez.</span><span class="sxs-lookup"><span data-stu-id="26ba2-159">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="26ba2-160">Küldje el a módosításokat a **Küldés** gombbal.</span><span class="sxs-lookup"><span data-stu-id="26ba2-160">Then **Submit** your changes.</span></span>

<span data-ttu-id="26ba2-161">A partnerek központon keresztüli megvásárlásának lehetősége csak a közvetlen számla és a közvetett szolgáltatók számára érhető el.</span><span class="sxs-lookup"><span data-stu-id="26ba2-161">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="26ba2-162">Csak a jogosult bővítmények jelennek meg az alapkövetelmények és a regionális elérhetőség alapján.</span><span class="sxs-lookup"><span data-stu-id="26ba2-162">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="26ba2-163">A díjszabással és ajánlatokkal kapcsolatos további információkért tekintse meg a felhőalapú viszonteladói ajánlat mátrixát.</span><span class="sxs-lookup"><span data-stu-id="26ba2-163">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="26ba2-164">Az alapszintű előfizetés felfüggesztése a kapcsolódó bővítményeket is felfüggeszti.</span><span class="sxs-lookup"><span data-stu-id="26ba2-164">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="26ba2-165">A bővítmények kezdő dátuma az alapszintű előfizetéshez igazodik, és a díjakat a díj kezdő dátuma és a díj befejezési dátuma alapján számítjuk ki, az első számlán pedig arányosított díjak szerepelnek.</span><span class="sxs-lookup"><span data-stu-id="26ba2-165">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="26ba2-166">További információ: [licenc alapú számlázás](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="26ba2-166">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="26ba2-167">Előfizetés felfüggesztése vagy megszakítása</span><span class="sxs-lookup"><span data-stu-id="26ba2-167">Suspend or cancel a subscription</span></span>

<span data-ttu-id="26ba2-168">A partnerek felfüggesztheti vagy lemondhatja az előfizetést, ha az ügyfél kéri, vagy nem fizetés vagy csalás esetén.</span><span class="sxs-lookup"><span data-stu-id="26ba2-168">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="26ba2-169">Előfizetés felfüggesztése</span><span class="sxs-lookup"><span data-stu-id="26ba2-169">Suspend a subscription</span></span>

<span data-ttu-id="26ba2-170">Ha a **felfüggesztett** előfizetés állapotát módosítja, a felhasználók nem tudnak bejelentkezni vagy elérni szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="26ba2-170">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="26ba2-171">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="26ba2-171">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="26ba2-172">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="26ba2-172">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="26ba2-173">Válassza ki a kezelni kívánt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="26ba2-173">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="26ba2-174">Az **Állapot** szakaszban válassza a **Felfüggesztve** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="26ba2-174">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="26ba2-175">Küldje el a módosításokat a **Küldés** gombbal.</span><span class="sxs-lookup"><span data-stu-id="26ba2-175">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="26ba2-176">A rendszer minden adatmennyiséget töröl, kivéve, ha az előfizetés újraaktiválása 90 napon belül történik, vagy 90 nap, valamint a fiók megnyitása és az első számlázási időszak (maximális 120 nap) közötti napok száma.</span><span class="sxs-lookup"><span data-stu-id="26ba2-176">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="26ba2-177">Egy előfizetés felfüggesztése esetén a **felfüggesztett** gomb alatt látható dátum azt jelzi, hogy az előfizetés automatikusan lejár-e, ha nem aktiválja újra.</span><span class="sxs-lookup"><span data-stu-id="26ba2-177">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="26ba2-178">Előfizetés megszakítása</span><span class="sxs-lookup"><span data-stu-id="26ba2-178">Cancel a subscription</span></span>

<span data-ttu-id="26ba2-179">A licenc-alapú SaaS-előfizetéseket a partner Center [kereskedelmi piactéren](csp-commercial-marketplace-overview.md)található külső gyártóktól származó ISV-gyártóktól is megszakíthatja.</span><span class="sxs-lookup"><span data-stu-id="26ba2-179">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="26ba2-180">Ha a lemondási időszakon belül megszakítja a megszakítást, teljes visszatérítést fog kapni.</span><span class="sxs-lookup"><span data-stu-id="26ba2-180">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="26ba2-181">Az ISV-ajánlatokhoz havonta számlázunk:</span><span class="sxs-lookup"><span data-stu-id="26ba2-181">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="26ba2-182">Ha kevesebb, mint 24 órával később megszakítja a rendelést, akkor a következő számlán teljes jóváírást fog kapni.</span><span class="sxs-lookup"><span data-stu-id="26ba2-182">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="26ba2-183">Ha a megrendelés után 24 órával később megszakítja a lemondást, a rendszer a Megújításkor ütemezi a megszakítást.</span><span class="sxs-lookup"><span data-stu-id="26ba2-183">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="26ba2-184">Évente számlázott ajánlatok esetén:</span><span class="sxs-lookup"><span data-stu-id="26ba2-184">For offers billed annually:</span></span>

- <span data-ttu-id="26ba2-185">Ha kevesebb mint 14 nappal megszakítja a rendelést, akkor a következő számlán teljes jóváírást fog kapni.</span><span class="sxs-lookup"><span data-stu-id="26ba2-185">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="26ba2-186">Ha a megrendelés elvégzése után 14 napon belül megszakítja a megszakítást, a rendszer a Megújításkor ütemezi a lemondást.</span><span class="sxs-lookup"><span data-stu-id="26ba2-186">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="26ba2-187">Ezen időszakok átadása után már nem jelenik meg az előfizetés megszakításának lehetősége.</span><span class="sxs-lookup"><span data-stu-id="26ba2-187">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="26ba2-188">A használaton alapuló és mért, külső gyártótól származó ISV-szolgáltatások (például a virtuális gépeket vagy tárolókat használó) nem jogosultak a visszatérésre.</span><span class="sxs-lookup"><span data-stu-id="26ba2-188">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="26ba2-189">A használaton alapuló szolgáltatások visszavonási módszerként is kihelyezhetők.</span><span class="sxs-lookup"><span data-stu-id="26ba2-189">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="26ba2-190">Mivel a díjak számlázása használat után történik, ezek a szolgáltatások nem jogosultak visszatérítésre.</span><span class="sxs-lookup"><span data-stu-id="26ba2-190">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="26ba2-191">Ha törölni szeretne egy licencalapú SaaS-előfizetést egy ISV-kiadóból, tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="26ba2-191">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="26ba2-192">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="26ba2-192">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="26ba2-193">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="26ba2-193">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="26ba2-194">Keresse meg a megszüntetni kívánt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="26ba2-194">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="26ba2-195">Az **állapot** oszlopban válassza a **Mégse** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="26ba2-195">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="26ba2-196">Küldje el a módosításokat a **Küldés** gombbal.</span><span class="sxs-lookup"><span data-stu-id="26ba2-196">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="26ba2-197">Ha megjelenik egy párbeszédpanel, töltse ki a megfelelő részleteket, majd válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="26ba2-197">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="26ba2-198">A törlés megerősítéséhez válassza az **Igen,** majd a Mégse gombot.</span><span class="sxs-lookup"><span data-stu-id="26ba2-198">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="26ba2-199">Dönthet úgy is, hogy megszakítja az Azure Marketplace-előfizetést API-k használatával.</span><span class="sxs-lookup"><span data-stu-id="26ba2-199">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="26ba2-200">Ehhez tekintse meg [Az Azure Marketplace-előfizetés megszakítása](/partner-center/develop/cancel-an-azure-marketplace-subscription)című témakört.</span><span class="sxs-lookup"><span data-stu-id="26ba2-200">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="26ba2-201">Válassza ki, hogy a kereskedelmi piactér-előfizetés automatikusan megújuljon-e</span><span class="sxs-lookup"><span data-stu-id="26ba2-201">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="26ba2-202">Alapértelmezés szerint az aktív előfizetések úgy vannak beállítva, hogy az előfizetési időszak lejáratakor automatikusan megújuljanak.</span><span class="sxs-lookup"><span data-stu-id="26ba2-202">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="26ba2-203">A [kereskedelmi piactér termékeire való előfizetések](csp-commercial-marketplace-overview.md)esetén dönthet úgy is, hogy nem újítja meg automatikusan az előfizetést.</span><span class="sxs-lookup"><span data-stu-id="26ba2-203">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="26ba2-204">Aktív kereskedelmi piactér-előfizetés leállítása automatikus megújítással:</span><span class="sxs-lookup"><span data-stu-id="26ba2-204">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="26ba2-205">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="26ba2-205">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="26ba2-206">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="26ba2-206">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="26ba2-207">Válassza az **Előfizetések** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="26ba2-207">Select **Subscriptions**.</span></span> <span data-ttu-id="26ba2-208">Ez felsorolja az ügyfél számára megvásárolt licenc-alapú előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="26ba2-208">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="26ba2-209">Az **előfizetés** oszlopban válassza ki a módosítani kívánt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="26ba2-209">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="26ba2-210">Az előfizetés részletei oldalon keresse meg az **állapot** szakaszt, és törölje az **automatikus megújítás** jelölőnégyzet jelölését.</span><span class="sxs-lookup"><span data-stu-id="26ba2-210">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="26ba2-211">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="26ba2-211">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="26ba2-212">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="26ba2-212">Next steps</span></span>

- [<span data-ttu-id="26ba2-213">Kereskedelmi piactéren vásárolt termékek vásárlása ügyfelei számára</span><span class="sxs-lookup"><span data-stu-id="26ba2-213">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="26ba2-214">Kereskedelmi piactér-termékek kezelése ügyfelei számára</span><span class="sxs-lookup"><span data-stu-id="26ba2-214">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="26ba2-215">Kereskedelmi piactér áttekintése</span><span class="sxs-lookup"><span data-stu-id="26ba2-215">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)