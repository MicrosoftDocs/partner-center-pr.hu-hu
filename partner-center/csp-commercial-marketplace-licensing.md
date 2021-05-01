---
title: Licencelés kezelése a Marketplace-ajánlatokban
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan állíthatja be és kezelheti az ISV kereskedelmi piactéri ajánlatok licencelését.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328015"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="ad4b4-103">Licencelés kezelése a Marketplace-ajánlatokban</span><span class="sxs-lookup"><span data-stu-id="ad4b4-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="ad4b4-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ad4b4-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="ad4b4-105">Global admin</span></span>
- <span data-ttu-id="ad4b4-106">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="ad4b4-106">Account admin</span></span>

<span data-ttu-id="ad4b4-107">Ez a cikk végigvezeti az ajánlat Partnerközpont- és Microsoft AppSource- és licenckezelésének folyamatán.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="ad4b4-108">A cikkben lévő képességek jelenleg nyilvános előzetes verzióban állnak rendelkezésre.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="ad4b4-109">Előkészületek</span><span class="sxs-lookup"><span data-stu-id="ad4b4-109">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="ad4b4-110">A kereskedelmi piactér alapjai</span><span class="sxs-lookup"><span data-stu-id="ad4b4-110">Commercial marketplace basics</span></span>

<span data-ttu-id="ad4b4-111">A folyamat megkezdése előtt ismerkedjen meg a kereskedelmi piactér alapjaival.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-111">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="ad4b4-112">Az alábbi táblázatban található cikkek segítenek az első lépésekben.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-112">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="ad4b4-113">Témakör</span><span class="sxs-lookup"><span data-stu-id="ad4b4-113">Topic</span></span>  | <span data-ttu-id="ad4b4-114">Cikk</span><span class="sxs-lookup"><span data-stu-id="ad4b4-114">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="ad4b4-115">Kereskedelmi piactéri csomagok</span><span class="sxs-lookup"><span data-stu-id="ad4b4-115">Commercial marketplace plans</span></span> | [<span data-ttu-id="ad4b4-116">A kereskedelmi piactéri ajánlatok csomagja és díjszabása</span><span class="sxs-lookup"><span data-stu-id="ad4b4-116">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="ad4b4-117">Kereskedelmi piactéri ajánlatok</span><span class="sxs-lookup"><span data-stu-id="ad4b4-117">Commercial marketplace offers</span></span>  | [<span data-ttu-id="ad4b4-118">Termékoldal-típusok</span><span class="sxs-lookup"><span data-stu-id="ad4b4-118">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="ad4b4-119">Kereskedelmi piactéri fiókok</span><span class="sxs-lookup"><span data-stu-id="ad4b4-119">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="ad4b4-120">Kereskedelmi piactéri fiók létrehozása a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ad4b4-120">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="ad4b4-121">Az ajánlatazonosító meghatározása</span><span class="sxs-lookup"><span data-stu-id="ad4b4-121">Determine your Offer ID</span></span>

<span data-ttu-id="ad4b4-122">Az alábbi eljárásokban meg kell adnia egy ajánlatazonosítót.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-122">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="ad4b4-123">Most egy kis idő alatt jöjjön ki egy megfelelő ajánlatazonosító, és vegye figyelembe a következőket:</span><span class="sxs-lookup"><span data-stu-id="ad4b4-123">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="ad4b4-124">Ez az azonosító látható az ügyfelek számára a marketplace-ajánlat webcímén, és Azure Resource Manager sablonokat, ha van ilyen.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-124">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="ad4b4-125">Az ajánlatazonosítónak és a közzétevő azonosítójának 40 karakternél nem hosszabbnak kell lennie.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-125">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="ad4b4-126">Csak kisbetűket és számokat használjon.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-126">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="ad4b4-127">Az ajánlatazonosító tartalmazhat kötőjelet és aláhúzásjelet, de szóközt nem.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-127">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="ad4b4-128">Ha például a közzétevő azonosítója , és a címet adja meg, `testpublisherid` `test-offer-1` az ajánlat webcíme `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` lesz.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-128">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="ad4b4-129">Ez az azonosító a Létrehozás lehetőséget választva nem **módosítható.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-129">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="ad4b4-130">Az ajánlat aliasának meghatározása</span><span class="sxs-lookup"><span data-stu-id="ad4b4-130">Determine your Offer alias</span></span>

<span data-ttu-id="ad4b4-131">Az Ajánlat aliasa az ajánlathoz használt név a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-131">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="ad4b4-132">Szüksége lesz egy megfelelő Offer aliasra is, amely az alábbi irányelveket követi:</span><span class="sxs-lookup"><span data-stu-id="ad4b4-132">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="ad4b4-133">Ez a név nem használatos a piactéren, és eltér az ajánlat nevétől és az ügyfelek számára megjelenő egyéb értékektől.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-133">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="ad4b4-134">Ez a név a Létrehozás kiválasztása után már nem módosítható.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-134">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="ad4b4-135">Ajánlat létrehozása</span><span class="sxs-lookup"><span data-stu-id="ad4b4-135">Create your offer</span></span>

<span data-ttu-id="ad4b4-136">A licencelési folyamat első lépése a kereskedelmi piactéri ajánlat létrehozása.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-136">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="ad4b4-137">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ad4b4-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="ad4b4-138">A bal oldali navigációs menüben válassza a **Kereskedelmi piactér/Áttekintés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-138">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="ad4b4-139">Az Áttekintés oldal tetején válassza az **Új** ajánlat lehetőséget, majd a **Dynamics 365 for Customer Engagement & PowerApps lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-139">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="ad4b4-140">Adja meg a  korábban létrehozott **Ajánlatazonosítót** és Ajánlat aliast.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-140">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="ad4b4-141">Válassza **a Létrehozás lehetőséget** az ajánlat létrehozásához és a folytatáshoz.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-141">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="ad4b4-142">Válassza ki a licencelési lehetőségeket.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-142">Choose your licensing options.</span></span>

    - <span data-ttu-id="ad4b4-143">Az ajánlat licenckezelésének engedélyezéséhez válassza az Alkalmazáslicenc-kezelés engedélyezése **a Microsofton keresztül lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-143">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="ad4b4-144">Ez egy egyszeres beállítás, és az ajánlat közzététele után nem módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-144">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="ad4b4-145">Azt is engedélyezheti, hogy az ügyfelek licenc nélkül futtatják az alkalmazás alapfunkcióit, és prémium szintű funkciókat futtassanak a licenc vásárlása után.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-145">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="ad4b4-146">Ehhez jelölje be Az alkalmazások telepítésének engedélyezése az ügyfelek számára akkor is, ha **nincsenek hozzárendelve licencek.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-146">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="ad4b4-147">Ha nem szeretné, hogy az ajánlatában engedélyezve legyen a licenckezelés, válassza a **Get it now (Free) (Szerezze be (ingyenes)**), **Az** ingyenes próbaverzió , vagy a Contact **me (Kapcsolatfelvétel) lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-147">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="ad4b4-148">Csomag létrehozása</span><span class="sxs-lookup"><span data-stu-id="ad4b4-148">Create your plan</span></span>

<span data-ttu-id="ad4b4-149">Ezekben a lépésekben meghatározhatja az ajánlathoz engedélyezni kívánt csomagokat vagy csomagokat.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-149">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="ad4b4-150">A bal oldali navigációs menüben válassza a **Csomag áttekintése,** majd az **Új csomag létrehozása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-150">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="ad4b4-151">Adja meg a **csomagazonosítót** és a **csomag nevét,** majd válassza a **Létrehozás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-151">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="ad4b4-152">A **Csomaglista lapon** adja meg a **csomag leírását.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-152">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="ad4b4-153">A leírás mentéshez és a későbbi befejezéshez válassza a **Piszkozat mentése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-153">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="ad4b4-154">Ha elkészült, válassza az Áttekintés **és közzététel lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-154">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="ad4b4-155">A csomaginformációk most már megjelennek a appsource.microsoft.com ajánlatlistában (csomagok szakaszban).</span><span class="sxs-lookup"><span data-stu-id="ad4b4-155">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="ad4b4-156">Miután létrehozta az ajánlat összes csomagját, ki kell másolnia az egyes csomagok szolgáltatásazonosítóját.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-156">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="ad4b4-157">Válassza **a Csomaglista** oldal tetején található Csomag áttekintése lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-157">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="ad4b4-158">Másolja az egyes tervek szolgáltatásazonosítóját egy biztonságos helyre.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-158">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="ad4b4-159">Szolgáltatás-önkiszolgálók hozzáadása a megoldáshoz</span><span class="sxs-lookup"><span data-stu-id="ad4b4-159">Add Service IDs to your solution</span></span>

<span data-ttu-id="ad4b4-160">A következő lépés a megoldás frissítése úgy, hogy hozzáadja a szolgáltatás-értékeket az összes másolt csomaghoz.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-160">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="ad4b4-161">Ezzel kapcsolatos útmutatásért lásd: [Create an AppSource Package for your solution (AppSource-csomag létrehozása a megoldáshoz).](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)</span><span class="sxs-lookup"><span data-stu-id="ad4b4-161">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="ad4b4-162">Csomag feltöltése és az ajánlat közzététele</span><span class="sxs-lookup"><span data-stu-id="ad4b4-162">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="ad4b4-163">A bal oldali navigációs panelen válassza a **Kereskedelmi piactér** lehetőséget, majd a **Technikai konfiguráció lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-163">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="ad4b4-164">Az **Alaplicenc-modell alatt válassza** a Felhasználó **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-164">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="ad4b4-165">A **CRM-csomag alatt** adja meg a csomag helyének URL-címét.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-165">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="ad4b4-166">A bal oldali navigációs panel többi lapját használva adja meg az egyéb szükséges adatokat.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-166">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="ad4b4-167">Ha végzett, válassza az Áttekintés **és közzététel lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-167">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="ad4b4-168">Az ajánlat közzététele után áttekintjük és ellenőrizzük az adatait.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-168">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="ad4b4-169">Ha bármilyen probléma van a folyamattal, értesítjük Önt.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-169">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="ad4b4-170">Ha minden probléma megoldódott, értesítést kap arról, hogy az ajánlata elérhető az AppSource-ban.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-170">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="ad4b4-171">Ezen a ponton élő adásra lehet képes.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-171">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="ad4b4-172">Az ajánlat élő adásban Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ad4b4-172">Make your offer live in Partner Center</span></span>

<span data-ttu-id="ad4b4-173">Az alábbi eljárás végigvezeti az ajánlat az AppSource-ban való élő készítés folyamatán.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-173">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="ad4b4-174">További információ erről a folyamatról: Bevezetés a [termékoldali lehetőségekbe.](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)</span><span class="sxs-lookup"><span data-stu-id="ad4b4-174">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="ad4b4-175">Az ajánlat közzététele után az élő adás 4–6 órát fog igénybe venni.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-175">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="ad4b4-176">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ad4b4-176">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="ad4b4-177">A bal oldali navigációs menüben válassza a **Kereskedelmi piactér/Áttekintés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-177">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="ad4b4-178">Az Áttekintés **lapon** keresse meg a keresett ajánlatot.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-178">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="ad4b4-179">A közzétételre kész ajánlatok előzetes verziójúak **lesznek.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-179">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="ad4b4-180">Válassza ki az ajánlatot.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-180">Select the offer.</span></span>
4. <span data-ttu-id="ad4b4-181">Az Ajánlat **áttekintése lapon** válassza az Élő **adása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-181">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="ad4b4-182">Az ajánlat 4-6 óra múlva lesz élő.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-182">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="ad4b4-183">Az ajánlatlista AppSource-on való áttekintéséhez kattintson az **AppSource** hivatkozásra az Ajánlat áttekintése **oldal alján.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-183">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="ad4b4-184">**Licenccel rendelkező ajánlatok** esetén: Ha az ajánlathoz licencellenőrzésre van szükség, a felhasználók csak a Kapcsolatfelvétel elemre kattintva léphetnek be érdeklődőt, hogy kommunikáljanak velük.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-184">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="ad4b4-185">**Ingyenes telepítési lehetőséggel** rendelkező licenccel rendelkező ajánlatok esetén: Ha az ajánlathoz nincs szükség licencellenőrzésre, a rendszergazdai felhasználók a Kapcsolatfelvétel lehetőség mellett a **Get It Now** (Azonnali lenyomás) gombot is látni **fogják.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-185">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="ad4b4-186">Azok a felhasználók, akik ki szeretnék próbálni az ingyenes telepítést, a **Get It Now**(Szerezze be most) gombra kattintva telepítik az ajánlatot a felügyeleti Power Platform központban.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-186">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="ad4b4-187">A felhasználók továbbra is használhatjak a **Kapcsolatfelvétel et,** ha kérdése van, vagy ha fizetős csomagra szeretne frissíteni.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-187">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="ad4b4-188">ISV Connect-ajánlat regisztrálása az ajánlatregisztrációban</span><span class="sxs-lookup"><span data-stu-id="ad4b4-188">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="ad4b4-189">Mielőtt licenceket rendelhet egy ügyfélhez, minden értékesítést regisztrálni kell a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-189">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="ad4b4-190">Ehhez lásd: [Az ügylet regisztrálása.](register-deals.md)</span><span class="sxs-lookup"><span data-stu-id="ad4b4-190">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="ad4b4-191">Az ügyfél meghívása</span><span class="sxs-lookup"><span data-stu-id="ad4b4-191">Invite the customer</span></span>

<span data-ttu-id="ad4b4-192">Az alábbi eljárással hívatja meg az ügyfelet az ajánlatban való részvételre.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-192">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="ad4b4-193">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ad4b4-193">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="ad4b4-194">A bal oldali navigációs menüben válassza a **Kereskedelmi piactér/Áttekintés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-194">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="ad4b4-195">A bal oldali navigációs menüben válassza a **Hivatkozások** lehetőséget, majd az **Ajánlatregisztráció lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-195">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="ad4b4-196">Szűrjön **az Elküldött** ügyletekre, válassza a Folyamatban **lapot,** majd válassza ki a kívánt ügyletet.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-196">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="ad4b4-197">Az ajánlat áttekintő oldalán válassza a **Licencek kezelése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-197">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="ad4b4-198">A **Licencek kezelése ablakban** válassza ki az ügyfelet az Ügyfél **adatai** legördülő listából.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-198">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="ad4b4-199">Ha az ügyfélkapcsolat még nem létezik, válassza a +Új ügyfél **meghívása a jóváhagyáshoz lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-199">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="ad4b4-200">Másolja ki a megjelenő hivatkozást.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-200">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="ad4b4-201">Küldje el e-mailben ezt a hivatkozást az ügyfél számlázási rendszergazdája vagy globális rendszergazdája számára, és ezt a hivatkozást használja a admin.microsoft.com eléréséhez és az Ön által létesított kapcsolat elfogadásához és elfogadásához.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-201">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="ad4b4-202">A kapcsolat addig nem lesz létrejön, amíg az ügyfél el nem végzi ezt a lépést.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-202">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="ad4b4-203">Licencek aktiválása, kezelése és eltávolítása</span><span class="sxs-lookup"><span data-stu-id="ad4b4-203">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="ad4b4-204">Miután az ügyfél engedélyezte a kapcsolatot Önvel, elkezdhet csomagokat hozzáadni az ajánlatból, és licenceket rendelni az egyes csomagokhoz.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-204">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="ad4b4-205">Az ajánlat Licencek kezelése ablakában válassza a **+Csomag hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-205">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="ad4b4-206">Töltse ki **a Csomag ehhez a megoldáshoz és** a **Licencek száma** mezőket, majd válassza a **Licencek frissítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-206">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="ad4b4-207">A licenceket az ügyfelek a admin.microsoft.com kezelhetik és hozzárendelhetik az alkalmazottakhoz.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-207">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="ad4b4-208">Egy meglévő csomag licencszámának módosításához írja be az  új számot a Licencek száma mezőbe, majd válassza a **Licencek frissítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-208">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="ad4b4-209">Az üzlet licencének inaktiválásához vagy eltávolításához  kattintson a Műveletek mezőben található kuka ikonra, majd válassza a **Licencek frissítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ad4b4-209">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ad4b4-210">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ad4b4-210">Next steps</span></span>

[<span data-ttu-id="ad4b4-211">Licencelési erőforrások</span><span class="sxs-lookup"><span data-stu-id="ad4b4-211">Licensing resources</span></span>](support-resources-licensing.md)
