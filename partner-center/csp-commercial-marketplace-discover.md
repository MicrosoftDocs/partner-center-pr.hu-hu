---
title: Ajánlatok felderítése – kereskedelmi piactér
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy a CSP-partnerek hogyan használhatják a partner centert a piactéren az SaaS-ajánlatok vagy a független szoftvergyártók (ISV-EK) díjszabásának megtekintéséhez vagy kereséséhez.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f741ef4e44632e1d239285b58e99fbb38a8f37e7
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979600"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a><span data-ttu-id="e27c6-103">Fedezze fel az ajánlatokat és a díjszabást a partner Center kereskedelmi piactéren</span><span class="sxs-lookup"><span data-stu-id="e27c6-103">Discover offers and pricing in Partner Center commercial marketplace</span></span>

<span data-ttu-id="e27c6-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="e27c6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e27c6-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="e27c6-105">Global admin</span></span>
- <span data-ttu-id="e27c6-106">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="e27c6-106">Admin agent</span></span>

<span data-ttu-id="e27c6-107">Ha a független szoftvergyártók (ISV-ket) úgy döntenek, hogy közzétesznek egy ajánlatot a kereskedelmi piactéren, dönthetnek arról is, hogy az ajánlatot elérhetővé kívánják-e tenni a CSP programban.</span><span class="sxs-lookup"><span data-stu-id="e27c6-107">When Independent Software Vendors (ISVs) choose to publish an offer in the commercial marketplace, they can also decide if they want the offer to be made available in the CSP program.</span></span> <span data-ttu-id="e27c6-108">Ha úgy dönt, hogy eladja az ajánlatot a CSP programon keresztül, a CSP-partnereknek az ajánlatot a partner Center Marketplace területen kell látniuk.</span><span class="sxs-lookup"><span data-stu-id="e27c6-108">If they choose to sell the offer through the CSP program, CSP partners should see the offer in Partner Center Marketplace area.</span></span>

<span data-ttu-id="e27c6-109">Ha egy ISV-ajánlat nem jelenik meg a partner Centerben elvárt módon, az a következők miatt fordulhat elő:</span><span class="sxs-lookup"><span data-stu-id="e27c6-109">If an ISV offer does not appear as you expect in Partner Center, it may be because:</span></span>

- <span data-ttu-id="e27c6-110">Az ISV úgy döntött, hogy nem értékesíti az ajánlatot a CSP programon keresztül.</span><span class="sxs-lookup"><span data-stu-id="e27c6-110">The ISV decided not to sell the offer through the CSP program.</span></span> <span data-ttu-id="e27c6-111">Előfordulhat például, hogy egyes ISV-termékek elérhetővé válnak a kereskedelmi piactér más területein (például a [Microsoft AppSource](https://appsource.microsoft.com/) és az [Azure piactéren](https://azuremarketplace.microsoft.com/)), de előfordulhat, hogy nem jelennek meg a partnerek számára a partnervállalat programban a partner Center piactéren.</span><span class="sxs-lookup"><span data-stu-id="e27c6-111">For example, some ISV products may have been made available in other areas of the commercial marketplace (such as in [Microsoft AppSource](https://appsource.microsoft.com/) and [Azure Marketplace](https://azuremarketplace.microsoft.com/)), but may not appear for partners in the CSP program in Partner Center marketplace.</span></span>

- <span data-ttu-id="e27c6-112">Az ISV úgy döntött, hogy az ajánlatot kizárólag kiválasztott számú CSP-partnernek teszi ki.</span><span class="sxs-lookup"><span data-stu-id="e27c6-112">The ISV decided to make the offer exclusive to only a select number of CSP partners.</span></span> <span data-ttu-id="e27c6-113">Az exkluzív ajánlatokról további információt a jelen témakör későbbi, című szakaszában talál.</span><span class="sxs-lookup"><span data-stu-id="e27c6-113">For more information about exclusive offers, see later in this help topic.</span></span>

- <span data-ttu-id="e27c6-114">Előfordulhat, hogy az ajánlat típusa nem hívható meg a partnervállalat vagy a Azure Portal (például tárolók vagy valamilyen használaton alapuló ajánlatok) segítségével.</span><span class="sxs-lookup"><span data-stu-id="e27c6-114">The offer type may not be transactable through Partner Center or Azure portal (e.g. Containers or some usage-based offers).</span></span>

- <span data-ttu-id="e27c6-115">Előfordulhat, hogy a társított ügyfél (ek) számlázási országa nem támogatott ezen az ISV-ajánlaton.</span><span class="sxs-lookup"><span data-stu-id="e27c6-115">The billing country of your associated customer(s) may not be supported for this ISV offer.</span></span>

## <a name="view-marketplace-offers-in-partner-center"></a><span data-ttu-id="e27c6-116">Piactéri ajánlatok megtekintése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="e27c6-116">View Marketplace offers in Partner Center</span></span>

<span data-ttu-id="e27c6-117">Az elérhető kereskedelmi Piactéri ajánlatok megtekintése a CSP programban:</span><span class="sxs-lookup"><span data-stu-id="e27c6-117">To view available commercial marketplace offers in the CSP program:</span></span>

1. <span data-ttu-id="e27c6-118">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard), majd a bal oldali navigációs menüben válassza a **CSP** elemet.</span><span class="sxs-lookup"><span data-stu-id="e27c6-118">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="e27c6-119">Válassza az **értékesítés**, majd a **piactér** elemet.</span><span class="sxs-lookup"><span data-stu-id="e27c6-119">Select **Sell**, followed by **Marketplace**.</span></span> <span data-ttu-id="e27c6-120">Alapértelmezés szerint minden típusú és kategóriájú terméket látni fog.</span><span class="sxs-lookup"><span data-stu-id="e27c6-120">By default, you will see products of all types and categories.</span></span>

3. <span data-ttu-id="e27c6-121">Válasszon egy szűrőt típus vagy kategória alapján.</span><span class="sxs-lookup"><span data-stu-id="e27c6-121">Select a filter by type or category.</span></span> <span data-ttu-id="e27c6-122">A **kereséssel** konkrét kulcsszavakat, ajánlat-NEVEKET vagy ISV-közzétevők nevét is megkeresheti.</span><span class="sxs-lookup"><span data-stu-id="e27c6-122">You can also use **Search** to find specific keywords, offer names or the names of ISV publishers.</span></span>

4. <span data-ttu-id="e27c6-123">Válasszon ki egy adott terméket a listából.</span><span class="sxs-lookup"><span data-stu-id="e27c6-123">Select a specific product offer from the list.</span></span> <span data-ttu-id="e27c6-124">Ekkor megjelenik a Product Overview (termék áttekintése) lap, ahol többet is megtudhat az ajánlatról.</span><span class="sxs-lookup"><span data-stu-id="e27c6-124">This will take you to a product Overview tab where you can learn more about the offer.</span></span> <span data-ttu-id="e27c6-125">Az ezen a lapon található információk a következők lehetnek:</span><span class="sxs-lookup"><span data-stu-id="e27c6-125">Information on this tab might include:</span></span> 

    - <span data-ttu-id="e27c6-126">A termék vagy ajánlat leírása</span><span class="sxs-lookup"><span data-stu-id="e27c6-126">A description of the product or offer</span></span>

    - <span data-ttu-id="e27c6-127">További információ az ISV-közzétevőről</span><span class="sxs-lookup"><span data-stu-id="e27c6-127">More information about the ISV publisher</span></span>

    - <span data-ttu-id="e27c6-128">Az ISV-közzétevő által feltöltött dokumentációra vagy marketinganyagokra mutató hivatkozások</span><span class="sxs-lookup"><span data-stu-id="e27c6-128">Links to documentation or marketing materials uploaded by the ISV publisher</span></span>

    - <span data-ttu-id="e27c6-129">Egyéb lehetséges ISV-kapcsolatok az ügyfélszolgálathoz, a mérnöki tevékenységhez vagy a CSP-programhoz való kapcsolattartáshoz</span><span class="sxs-lookup"><span data-stu-id="e27c6-129">Other possible ISV contacts for customer support, engineering, or a contact for the CSP program</span></span>

5. <span data-ttu-id="e27c6-130">Ha többet szeretne megtudni az ajánlat rendelkezésre álló csomagjairól, SKU-ról vagy díjszabásáról, válassza a **csomagok + díjszabás** lapot. Ezen a lapon a következő jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="e27c6-130">To see more information about an offer's available plans, SKUs, or pricing, select the **Plans + Pricing** tab. This tab will show you:</span></span>

    - <span data-ttu-id="e27c6-131">Azok a piacok, amelyeken elérhető az ajánlat</span><span class="sxs-lookup"><span data-stu-id="e27c6-131">The markets where this offer is available to you</span></span>

    - <span data-ttu-id="e27c6-132">Az ajánlathoz elérhető SKU-i vagy csomagok listája</span><span class="sxs-lookup"><span data-stu-id="e27c6-132">A list of SKUs or plans available for the offer</span></span>

    - <span data-ttu-id="e27c6-133">Az egyes SKU-vagy díjcsomag díjszabása</span><span class="sxs-lookup"><span data-stu-id="e27c6-133">Pricing for each SKU or Plan available</span></span>

## <a name="view-marketplace-offers-via-partner-center-apis"></a><span data-ttu-id="e27c6-134">Piactéri ajánlatok megtekintése a partner Center API-kon keresztül</span><span class="sxs-lookup"><span data-stu-id="e27c6-134">View Marketplace offers via Partner Center APIs</span></span>

<span data-ttu-id="e27c6-135">A CSP program partnerei API-kat is használhatnak a jogosult ajánlatok listájának visszaküldéséhez.</span><span class="sxs-lookup"><span data-stu-id="e27c6-135">CSP program partners can also use APIs to return a list of eligible offers.</span></span> <span data-ttu-id="e27c6-136">A jogosult ajánlatok csak azokra a SaaS ISV-ajánlatokra lesznek elérhetők, amelyek a partner Center Marketplace-en keresztül értékesíthetők.</span><span class="sxs-lookup"><span data-stu-id="e27c6-136">Eligible offers will be only those SaaS ISV offers available for the partner to sell via Partner Center marketplace.</span></span> <span data-ttu-id="e27c6-137">A katalógusban található ajánlatok azonosítására szolgáló API-kat használó partnereink számára tekintse meg az útmutatót, amely a [piacon elérhető ajánlatok listáját tartalmazza](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span><span class="sxs-lookup"><span data-stu-id="e27c6-137">For partners using APIs to identify offers in the catalog, refer to the guidance to [obtain a list of offers for a market](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span></span>

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a><span data-ttu-id="e27c6-138">Tekintse meg a piactér legújabb ajánlatának díjszabását a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="e27c6-138">View the latest Marketplace offer pricing in Partner Center</span></span>

<span data-ttu-id="e27c6-139">Az ajánlatokkal kapcsolatos legújabb díjszabási részletekért kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="e27c6-139">Follow these steps for the latest pricing details associated with an offer:</span></span>

1. <span data-ttu-id="e27c6-140">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard), majd a bal oldali navigációs menüben válassza a **CSP** elemet.</span><span class="sxs-lookup"><span data-stu-id="e27c6-140">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="e27c6-141">Válassza az **értékesítés** lehetőséget, majd a **díjszabást és az ajánlatokat**.</span><span class="sxs-lookup"><span data-stu-id="e27c6-141">Select **Sell**, followed by **Pricing and offers**.</span></span>

3. <span data-ttu-id="e27c6-142">Görgessen le a **piactér** szakaszhoz, válasszon egy helyet, és töltse le a **piactér díjszabását**.</span><span class="sxs-lookup"><span data-stu-id="e27c6-142">Scroll down to the **Marketplace** section, select a location and download **Marketplace pricing**.</span></span> <span data-ttu-id="e27c6-143">Ez egy táblázatot hoz létre az SaaS-, licenc-alapú ajánlatok és az ISV-közzétevők által elérhető díjszabású ajánlatok legújabb díjszabási adataival.</span><span class="sxs-lookup"><span data-stu-id="e27c6-143">This generates a spreadsheet with the latest pricing data for SaaS, license-based offers and metered offers available from ISV publishers.</span></span> <span data-ttu-id="e27c6-144">Néhány Azure-alkalmazás díjszabása is itt jelenhet meg.</span><span class="sxs-lookup"><span data-stu-id="e27c6-144">Some Azure application pricing may also appear here.</span></span> <span data-ttu-id="e27c6-145">A rendszer naponta frissíti ezeket az információkat, így a választott gyakorisággal a jelenlegi árakon is megtekintheti.</span><span class="sxs-lookup"><span data-stu-id="e27c6-145">This information is updated daily, so you can check it for current prices as often as you choose.</span></span>

4. <span data-ttu-id="e27c6-146">Ha egy ISV-termék ingyenes próbaidőszakot tartalmaz, a táblázat két sort fog megjeleníteni a termékhez:</span><span class="sxs-lookup"><span data-stu-id="e27c6-146">If an ISV product includes a free trial period, the spreadsheet will display two rows for that product:</span></span>

    - <span data-ttu-id="e27c6-147">Az egyik sor a nulla ingyenes próba árát mutatja.</span><span class="sxs-lookup"><span data-stu-id="e27c6-147">One row shows the free trial price of zero.</span></span> <span data-ttu-id="e27c6-148">Ez azt jelenti, hogy az ingyenes próbaidőszak elérhető.</span><span class="sxs-lookup"><span data-stu-id="e27c6-148">This means a free trial period is available.</span></span>

    - <span data-ttu-id="e27c6-149">A másik sor az ingyenes próbaidőszak lejárta után alkalmazandó árat és feltételeket mutatja.</span><span class="sxs-lookup"><span data-stu-id="e27c6-149">The other row shows the price and terms that will apply after the free trial period is over.</span></span>

<span data-ttu-id="e27c6-150">A CSP program partnereként jogosult lehet az egyes kereskedelmi Piactéri ajánlatokhoz kapcsolódó egyéb ösztönzőkre.</span><span class="sxs-lookup"><span data-stu-id="e27c6-150">As a CSP program partner, you may be eligible for other incentives associated with certain commercial marketplace offers.</span></span> <span data-ttu-id="e27c6-151">További információ az egyéb ösztönzőkről: CSP- [ösztönző útmutató](https://aka.ms/partnerincentives) (CSP-bejelentkezést igényel).</span><span class="sxs-lookup"><span data-stu-id="e27c6-151">For more information about other incentives, see the [CSP incentive guide](https://aka.ms/partnerincentives) (requires CSP login).</span></span>

## <a name="learn-about-marketplace-exclusive-offers"></a><span data-ttu-id="e27c6-152">Ismerje meg a Marketplace exkluzív ajánlatait</span><span class="sxs-lookup"><span data-stu-id="e27c6-152">Learn about marketplace exclusive offers</span></span>

<span data-ttu-id="e27c6-153">Az ISV-ket lehetőségük van arra, hogy az ajánlatait csak bizonyos partnereknek lehessen elérhetővé tenni a CSP programban.</span><span class="sxs-lookup"><span data-stu-id="e27c6-153">ISVs have the option to make their offers available only to specific partners in the CSP program.</span></span> <span data-ttu-id="e27c6-154">Ezt exkluzív ajánlatnak nevezzük.</span><span class="sxs-lookup"><span data-stu-id="e27c6-154">This is known as an Exclusive offer.</span></span> <span data-ttu-id="e27c6-155">A CSP program összes partnere továbbra is megtekintheti a partner Center kereskedelmi piactéren található összes ISV-ajánlatot, beleértve az exkluzív jelölésű ajánlatokat is.</span><span class="sxs-lookup"><span data-stu-id="e27c6-155">All partners in the CSP program can still view all ISV offers in Partner Center commercial marketplace, including those offers marked Exclusive.</span></span>

<span data-ttu-id="e27c6-156">Ha egy ajánlat **nem** kizárólagos jelölésű, az összes partner megvásárolhatja az ajánlatot (feltéve, hogy a kiválasztott ügyfél számlázási országa megfelel az ISV-k ajánlatának országa számára elérhetőnek).</span><span class="sxs-lookup"><span data-stu-id="e27c6-156">If an offer is **not** marked Exclusive, all partners can purchase that offer (assuming the selected customer’s billing country matches the country availability of the ISV's offer).</span></span>

<span data-ttu-id="e27c6-157">Az exkluzív jelölésű ajánlatok esetében azonban csak az ISV által kiválasztott partnerek vásárolhatják meg az ajánlatot.</span><span class="sxs-lookup"><span data-stu-id="e27c6-157">For any offer marked Exclusive, however, only those partners selected by the ISV will be able to purchase that offer.</span></span>

> [!NOTE]
> <span data-ttu-id="e27c6-158">Ha olyan exkluzív ajánlat jelenik meg, amelyet szeretne értékesíteni az ügyfeleknek, forduljon közvetlenül az ISV-hoz, és kérjen engedélyt az exkluzív ajánlat eladására.</span><span class="sxs-lookup"><span data-stu-id="e27c6-158">If you see an offer marked Exclusive that you would like to sell to your customers, reach out to the ISV directly and ask for permission to sell the Exclusive offer.</span></span> <span data-ttu-id="e27c6-159">Ha megtekinti egy exkluzív ajánlat részleteit, megjelenhet egy **partneri ISV** -hivatkozás, amelyet kiválaszthat.</span><span class="sxs-lookup"><span data-stu-id="e27c6-159">When you view the details of an Exclusive offer, you may see a **Contact ISV** link that you can select.</span></span>

<span data-ttu-id="e27c6-160">Ha többet szeretne megtudni a kereskedelmi piactéren található ISV-ról, olvassa el a [Cloud Solution Providers szolgáltatást](/azure/marketplace/cloud-solution-providers).</span><span class="sxs-lookup"><span data-stu-id="e27c6-160">To learn more about the ISV experience in the commercial marketplace, read [Cloud Solution Providers](/azure/marketplace/cloud-solution-providers).</span></span>

<span data-ttu-id="e27c6-161">A piactéren elérhető CSP-vel kapcsolatos további információkért olvassa el a [kereskedelmi piactér – áttekintés](csp-commercial-marketplace-overview.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="e27c6-161">For more information on the CSP experience in the marketplace, read [Commercial marketplace overview](csp-commercial-marketplace-overview.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="e27c6-162">További lépések</span><span class="sxs-lookup"><span data-stu-id="e27c6-162">Next steps</span></span>

- [<span data-ttu-id="e27c6-163">Kereskedelmi Piactéri ajánlatok vásárlása</span><span class="sxs-lookup"><span data-stu-id="e27c6-163">Purchase commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)