---
title: Ügyfél-előfizetések létrehozása a Partnerközpont
ms.topic: how-to
ms.date: 05/17/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan értékesítsen előfizetéseket az ügyfeleinek a Microsoft által közzétett termékekre, valamint a harmadik féltől származó isv-k által közzétett SaaS-termékekre.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3269fa994d704c0a0dae067087bad8589a7ce031
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148198"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="04732-103">Ügyfél-előfizetések létrehozása, felfüggesztése vagy lemondása</span><span class="sxs-lookup"><span data-stu-id="04732-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="04732-104">**A következőkre vonatkozik:** Partnerközpont | Partnerközpont a Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="04732-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="04732-105">**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Globális rendszergazdai | Az | Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="04732-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="04732-106">Miután létrehozta az ügyfél rekordját a Partnerközpont, előfizetéseket értékesíthet a katalógusban található termékekhez.</span><span class="sxs-lookup"><span data-stu-id="04732-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="04732-107">Ide tartoznak a Microsoft által közzétett termékek és a külső független szoftverszállítók (ISV-k) által a kereskedelmi piactéren közzétett Szolgáltatott szoftver (SaaS) [termékek.](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="04732-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="04732-108">Egyes ajánlatok ügyfelenként egy előfizetésre vannak korlátozva.</span><span class="sxs-lookup"><span data-stu-id="04732-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="04732-109">A korlátozott ajánlatok listáját a Díjszabás és ajánlatok Partnerközpont oldalon láthatja.</span><span class="sxs-lookup"><span data-stu-id="04732-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="04732-110">A CSP-programban partnerként licencalapú **vagy** forgalmi díjas SaaS-előfizetéseket vásárolhat az isV-közzétevőktől a Partnerközpont. </span><span class="sxs-lookup"><span data-stu-id="04732-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="04732-111">Ez azt jelenti, hogy bármilyen licencalapú vagy forgalmi díjas  SaaS-ajánlatot [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) megvásárolhat, amelyet az ISV közzétevő tett elérhetővé az Ön számára, beleértve azokat az ajánlatokat is, amelyekhez Hozzáféréssel rendelkezik. </span><span class="sxs-lookup"><span data-stu-id="04732-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="04732-112">Az ISV-k (például Azure-alkalmazásokat, tárolókat vagy virtuális gépeket érintő használatalapú ajánlatok) kereskedelmi piactéri ajánlatának megvásárlásához vagy kezeléséhez meg kell [Azure Portal.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="04732-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="04732-113">Új előfizetés létrehozása</span><span class="sxs-lookup"><span data-stu-id="04732-113">Create a new subscription</span></span>

1. <span data-ttu-id="04732-114">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="04732-114">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="04732-115">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="04732-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="04732-116">Válassza **az Előfizetés hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="04732-116">Select **Add subscription**.</span></span> <span data-ttu-id="04732-117">Az **Online szolgáltatások lapon** érhetők el az összes elérhető Marketplace SaaS-ajánlat.</span><span class="sxs-lookup"><span data-stu-id="04732-117">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="04732-118">Ha csak bizonyos típusú előfizetéseket kell látnia, az elérhető szűrők között tegye a következőt:</span><span class="sxs-lookup"><span data-stu-id="04732-118">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="04732-119">**Közzétevő:** Válassza a **Microsoft** lehetőséget, ha csak a Microsoft ajánlatai vagy a **Partner** ajánlatai közül kíváncsi az ISV-k által közzétett kereskedelmi piactéri termékekre.</span><span class="sxs-lookup"><span data-stu-id="04732-119">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="04732-120">**Számlázási típus:** Válassza ki a használni kívánt előfizetés-számlázás típusát: **Licenc vagy** **Használat.**</span><span class="sxs-lookup"><span data-stu-id="04732-120">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="04732-121">A [havi és az éves számlázási](license-based-billing.md) gyakoriság közötti döntéshez szükséges információkért tekintse meg a licencalapú számlázást.</span><span class="sxs-lookup"><span data-stu-id="04732-121">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="04732-122">**Kategória:** Válassza a **Vállalati,** **a Kisvállalati vagy** a **Próbaverzió lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="04732-122">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="04732-123">A próbaverziós előfizetésekkel kapcsolatos információkért lásd: [Ajánlat az ügyfeleknek próbaverziós Microsoft-termékekre.](offer-your-customers-trials-of-microsoft-products.md)</span><span class="sxs-lookup"><span data-stu-id="04732-123">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="04732-124">Válassza ki az ügyfél számára megvásárolni kívánt termék-előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="04732-124">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="04732-125">A látható termékek az ügyfélszegmens típusától (oktatás, kormányzat stb.) és az alkalmazott szűrőktől függenek.</span><span class="sxs-lookup"><span data-stu-id="04732-125">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="04732-126">Előfordulhat, hogy a Marketplace-en megjelenő egyes ajánlatok nem mindig érhetők el egy adott ügyfél vagy egy adott CSP-partner számára.</span><span class="sxs-lookup"><span data-stu-id="04732-126">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="04732-127">Ennek oka a következő lehet:</span><span class="sxs-lookup"><span data-stu-id="04732-127">This can be because:</span></span>

   - <span data-ttu-id="04732-128">Az ügyfél már rendelkezik előfizetéssel az adott termékre, és csak egy engedélyezett</span><span class="sxs-lookup"><span data-stu-id="04732-128">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="04732-129">Előfordulhat, hogy az ügyfél előfizetése fel lett függesztve (ebben az esetben újraaktiválhatja az előfizetést ahelyett, hogy újat vásárol.</span><span class="sxs-lookup"><span data-stu-id="04732-129">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="04732-130">IsV SaaS-ajánlatok esetén több oka is lehet annak, hogy az ajánlat nem vásárolható meg: Előfordulhat, hogy az ISV nem támogatja az ügyfél számlázási országát vagy régióját; lehetséges, hogy a szoftverszolgáltató úgy döntött, hogy nem teszi elérhetővé az ajánlatot a CSP-programon keresztül; vagy az is előfordulhat, hogy [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) az is csak bizonyos CSP-partnerek számára tette kizárólagosként az ajánlatot.</span><span class="sxs-lookup"><span data-stu-id="04732-130">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="04732-131">Előfordulhat, hogy az ISV-ajánlat nem kezelhető a Partnerközpont (például tárolókon vagy használatalapú ajánlatokon) keresztül.</span><span class="sxs-lookup"><span data-stu-id="04732-131">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="04732-132">Minden hozzáadni kívánt előfizetéshez adja meg a licencek számát (ha szükséges), majd válassza a **Hozzáadás a kosárhoz lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="04732-132">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="04732-133">Ha befejezte az előfizetések hozzáadását, válassza az **Áttekintés és** a rendelés áttekintése lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04732-133">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="04732-134">Miután áttekintte a rendeléseket, és készen áll az előfizetések megvásárlására, válassza a **Vásárlás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="04732-134">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="04732-135">Miután előfizetést vásárol egy ügyfélnek, a következő történik:</span><span class="sxs-lookup"><span data-stu-id="04732-135">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="04732-136">Az előfizetés áttekintéséhez vagy szerkesztéséhez válassza ki az előfizetés nevét az ügyfél **Előfizetések oldalán.**</span><span class="sxs-lookup"><span data-stu-id="04732-136">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="04732-137">Innen kiválaszthatja a bővítménylicenceket, ha van ilyen, módosíthatja a licencek mennyiségét, vagy felfüggesztheti az előfizetést.</span><span class="sxs-lookup"><span data-stu-id="04732-137">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="04732-138">**ISV SaaS- (licencalapú és forgalmi díjas) előfizetések esetén:**</span><span class="sxs-lookup"><span data-stu-id="04732-138">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="04732-139">Egy, az ISV-közzétevő webhelyére mutató hivatkozást fog kapni.</span><span class="sxs-lookup"><span data-stu-id="04732-139">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="04732-140">Ez a hivatkozás segíthet az ügyfél előfizetésének üzembe helyezésében vagy fiókbeállításában.</span><span class="sxs-lookup"><span data-stu-id="04732-140">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="04732-141">Sem Ön, sem az ügyfele nem kap e-mailt, amely utasításokat tartalmaz az ilyen típusú ISV-előfizetéshez beállított/kiépítési fiók befejezésére vonatkozó utasításokkal.)</span><span class="sxs-lookup"><span data-stu-id="04732-141">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="04732-142">Ha az előfizetése 30 napos ingyenes próbaverzióval rendelkezik, az ingyenes próbaidőszak automatikusan alkalmazva lesz.</span><span class="sxs-lookup"><span data-stu-id="04732-142">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="04732-143">A CSP-programban partnerként nem hagyhatja ki az ingyenes próbaidőszakot az ügyfelek számára vásárolt ajánlatok esetében.</span><span class="sxs-lookup"><span data-stu-id="04732-143">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="04732-144">Az ingyenes próbaidőszak végén megkezdődik az előfizetési időszak, és az előfizetés fizetős állapotra vált.</span><span class="sxs-lookup"><span data-stu-id="04732-144">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="04732-145">Az előfizetés ekkor automatikusan megújul ugyanezen ütemezés szerint.</span><span class="sxs-lookup"><span data-stu-id="04732-145">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="04732-146">Előfizetések frissítése bővítményekkel</span><span class="sxs-lookup"><span data-stu-id="04732-146">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="04732-147">Bővítmény vásárlásához az ügyfélnek először aktív alap-előfizetéssel kell lennie.</span><span class="sxs-lookup"><span data-stu-id="04732-147">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="04732-148">A katalóguson keresztül nem vásárolhat bővítményeket.</span><span class="sxs-lookup"><span data-stu-id="04732-148">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="04732-149">Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="04732-149">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="04732-150">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="04732-150">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="04732-151">Válassza ki a kezelni kívánt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="04732-151">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="04732-152">Az Állapot **szakasz** alatt az előfizetéshez elérhető bővítmények listája látható.</span><span class="sxs-lookup"><span data-stu-id="04732-152">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="04732-153">Frissítse az egyes szükséges bővítmények licencmennyiségét.</span><span class="sxs-lookup"><span data-stu-id="04732-153">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="04732-154">Küldje el a módosításokat a **Küldés** gombbal.</span><span class="sxs-lookup"><span data-stu-id="04732-154">Then **Submit** your changes.</span></span>

<span data-ttu-id="04732-155">A bővítmények vásárlásának lehetősége Partnerközpont csak a közvetlen számlázási és közvetett szolgáltatók számára érhető el.</span><span class="sxs-lookup"><span data-stu-id="04732-155">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="04732-156">Csak a jogosult bővítmények jelennek meg az alapkövetelmények és a regionális rendelkezésre állás alapján.</span><span class="sxs-lookup"><span data-stu-id="04732-156">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="04732-157">További információ a díjszabásról és az ajánlatokról: Felhő viszonteladói ajánlat mátrixa.</span><span class="sxs-lookup"><span data-stu-id="04732-157">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="04732-158">Az alapszintű előfizetés felfüggesztése a kapcsolódó bővítményeket is felfüggeszti.</span><span class="sxs-lookup"><span data-stu-id="04732-158">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="04732-159">A bővítmények kezdő dátuma az alapszintű előfizetéshez igazodik, és a díjakat a díj kezdő dátuma és a díj befejezési dátuma alapján számítjuk ki, az első számlán pedig arányosított díjak szerepelnek.</span><span class="sxs-lookup"><span data-stu-id="04732-159">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="04732-160">További információ: [Licencalapú számlázás.](license-based-billing.md)</span><span class="sxs-lookup"><span data-stu-id="04732-160">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="04732-161">Előfizetés felfüggesztése vagy lemondása</span><span class="sxs-lookup"><span data-stu-id="04732-161">Suspend or cancel a subscription</span></span>

<span data-ttu-id="04732-162">A partnerek felfüggeszthetik vagy megszüntethetik az előfizetést, ha az ügyfél ezt kéri, illetve fizetés elmaradása vagy csalás esetén.</span><span class="sxs-lookup"><span data-stu-id="04732-162">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="04732-163">Előfizetés felfüggesztése</span><span class="sxs-lookup"><span data-stu-id="04732-163">Suspend a subscription</span></span>

<span data-ttu-id="04732-164">Ha egy előfizetés állapotát Felfüggesztve állapotra **módosítja,** a felhasználók nem tudnak bejelentkezni vagy hozzáférni a szolgáltatásokhoz.</span><span class="sxs-lookup"><span data-stu-id="04732-164">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="04732-165">Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="04732-165">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="04732-166">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="04732-166">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="04732-167">Válassza ki a kezelni kívánt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="04732-167">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="04732-168">Az **Állapot** szakaszban válassza a **Felfüggesztve** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04732-168">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="04732-169">Küldje el a módosításokat a **Küldés** gombbal.</span><span class="sxs-lookup"><span data-stu-id="04732-169">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="04732-170">Az összes adat törlődik, kivéve, ha az előfizetést 90 napon belül újraaktiválják, vagy a fiók megnyitása és az első számlázási időszak közötti napok száma (legfeljebb 120 nap).</span><span class="sxs-lookup"><span data-stu-id="04732-170">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="04732-171">Ha felfüggeszt egy előfizetést, a  Felfüggesztve gomb alatt látható dátum jelzi, hogy mikor jár le automatikusan az előfizetés, ha nem aktiválja újra.</span><span class="sxs-lookup"><span data-stu-id="04732-171">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="04732-172">A CSP-előfizetések nem lejártak (ahogyan a webes előfizetések is), amely alatt a szolgáltatások továbbra is működnek, de az előfizetés nem hoz létre számlázási díjakat.</span><span class="sxs-lookup"><span data-stu-id="04732-172">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="04732-173">A CSP-előfizetések aktívak vagy fel vannak függesztve (vagy teljesen törölve vannak).</span><span class="sxs-lookup"><span data-stu-id="04732-173">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="04732-174">Előfizetés lemondása</span><span class="sxs-lookup"><span data-stu-id="04732-174">Cancel a subscription</span></span>

<span data-ttu-id="04732-175">A licencalapú SaaS-előfizetéseket a kereskedelmi piactéren található külső isV-közzétevőktől Partnerközpont [le.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="04732-175">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="04732-176">A lemondási időszakon belül teljes visszatérítést kap.</span><span class="sxs-lookup"><span data-stu-id="04732-176">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="04732-177">Az ISV-ajánlatok számlázása havonta történik:</span><span class="sxs-lookup"><span data-stu-id="04732-177">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="04732-178">Ha a rendelést kevesebb mint 24 órával lemondja, a következő számlán teljes jóváírást fog kapni.</span><span class="sxs-lookup"><span data-stu-id="04732-178">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="04732-179">Ha a rendelést 24 óránál később mondja le, a lemondás a megújításkor lesz ütemezve.</span><span class="sxs-lookup"><span data-stu-id="04732-179">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="04732-180">Az évente számlázható ajánlatokhoz:</span><span class="sxs-lookup"><span data-stu-id="04732-180">For offers billed annually:</span></span>

- <span data-ttu-id="04732-181">Ha a rendelést kevesebb, mint 14 nappal lemondja, a következő számlán teljes jóváírást fog kapni.</span><span class="sxs-lookup"><span data-stu-id="04732-181">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="04732-182">Ha a rendelést a rendelést követően 14 napnál később mondja le, a lemondás a megújításkor lesz ütemezve.</span><span class="sxs-lookup"><span data-stu-id="04732-182">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="04732-183">Ha ezek az időszakok véget érnek, többé nem lesz lehetősége megszüntetni az előfizetést.</span><span class="sxs-lookup"><span data-stu-id="04732-183">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="04732-184">A használatalapú és forgalmi díjas, külső isV-szolgáltatások (amelyek például virtuális gépeket vagy tárolókat használnak) nem jogosultak a visszaküldésre.</span><span class="sxs-lookup"><span data-stu-id="04732-184">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="04732-185">A használatalapú szolgáltatások kiépítve megszakítási módszerként is fel lehet szabad használni.</span><span class="sxs-lookup"><span data-stu-id="04732-185">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="04732-186">Mivel a díjakat használat után számlázjuk, ezek a szolgáltatások nem jogosultak visszatérítésre.</span><span class="sxs-lookup"><span data-stu-id="04732-186">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="04732-187">Ha törölni szeretne egy licencalapú SaaS-előfizetést egy ISV-kiadóból, tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="04732-187">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="04732-188">Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="04732-188">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="04732-189">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="04732-189">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="04732-190">Keresse meg a megszüntetni kívánt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="04732-190">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="04732-191">Az Állapot **oszlopban** válassza a **Mégse lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="04732-191">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="04732-192">Küldje el a módosításokat a **Küldés** gombbal.</span><span class="sxs-lookup"><span data-stu-id="04732-192">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="04732-193">Ha megjelenik egy párbeszédpanel, adja meg a vonatkozó adatokat, majd válassza a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="04732-193">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="04732-194">A lemondás megerősítéséhez válassza az **Igen, lemondás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="04732-194">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="04732-195">Dönthet úgy is, hogy API-Azure Marketplace lemond egy előfizetést.</span><span class="sxs-lookup"><span data-stu-id="04732-195">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="04732-196">Lásd: Előfizetés [lemondása Azure Marketplace.](/partner-center/develop/cancel-an-azure-marketplace-subscription)</span><span class="sxs-lookup"><span data-stu-id="04732-196">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="04732-197">Annak kiválasztása, hogy a rendszer automatikusan megújítsa-e a kereskedelmi piactér-előfizetést</span><span class="sxs-lookup"><span data-stu-id="04732-197">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="04732-198">Alapértelmezés szerint az aktív előfizetések úgy vannak beállítva, hogy az előfizetési időszak lejáratakor automatikusan megújuljanak.</span><span class="sxs-lookup"><span data-stu-id="04732-198">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="04732-199">A [kereskedelmi piactéri termékekre való előfizetések esetén](csp-commercial-marketplace-overview.md)dönthet úgy is, hogy nem újítja meg automatikusan az előfizetést.</span><span class="sxs-lookup"><span data-stu-id="04732-199">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="04732-200">Egy aktív kereskedelmi piactér-előfizetés automatikus megújításának megállítása:</span><span class="sxs-lookup"><span data-stu-id="04732-200">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="04732-201">Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="04732-201">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="04732-202">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="04732-202">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="04732-203">Válassza az **Előfizetések** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04732-203">Select **Subscriptions**.</span></span> <span data-ttu-id="04732-204">Ez felsorolja az ügyfél számára megvásárolt licencalapú előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="04732-204">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="04732-205">Az Előfizetés **oszlopban** válassza ki a módosítani kívánt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="04732-205">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="04732-206">Az előfizetés részleteit tartalmazó lapon keresse meg az **Állapot szakaszt,** és törölje a jelölést az **Automatikus megújítás jelölőnégyzetből.**</span><span class="sxs-lookup"><span data-stu-id="04732-206">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="04732-207">Válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="04732-207">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="04732-208">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="04732-208">Next steps</span></span>

- [<span data-ttu-id="04732-209">Kereskedelmi piactéri termékek vásárlása az ügyfelek számára</span><span class="sxs-lookup"><span data-stu-id="04732-209">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="04732-210">Kereskedelmi piactéri termékek kezelése az ügyfelek számára</span><span class="sxs-lookup"><span data-stu-id="04732-210">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="04732-211">Kereskedelmi piactér áttekintése</span><span class="sxs-lookup"><span data-stu-id="04732-211">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)