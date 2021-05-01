---
title: Licencelés kezelése a Marketplace-ajánlatokban
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan állíthatja be és kezelheti az ISV kereskedelmi piactéri ajánlatok licencelését.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284888"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="76bcd-103">Licencelés kezelése a Marketplace-ajánlatokban</span><span class="sxs-lookup"><span data-stu-id="76bcd-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="76bcd-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="76bcd-104">**Appropriate roles**</span></span>

- <span data-ttu-id="76bcd-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="76bcd-105">Global admin</span></span>
- <span data-ttu-id="76bcd-106">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="76bcd-106">Account admin</span></span>

<span data-ttu-id="76bcd-107">Ez a cikk végigvezeti az ajánlat Partnerközpont- és Microsoft AppSource- és licenckezelés folyamatán.</span><span class="sxs-lookup"><span data-stu-id="76bcd-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="76bcd-108">A cikkben lévő képességek jelenleg nyilvános előzetes verzióban állnak rendelkezésre.</span><span class="sxs-lookup"><span data-stu-id="76bcd-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="76bcd-109">Előkészületek</span><span class="sxs-lookup"><span data-stu-id="76bcd-109">Before you begin</span></span>

<span data-ttu-id="76bcd-110">A folyamat megkezdése előtt ismerkedjen meg az alábbi információkkal.</span><span class="sxs-lookup"><span data-stu-id="76bcd-110">Before beginning this process, you should familiarize yourself with the information below.</span></span>

### <a name="review-the-azure-marketplace-documentation"></a><span data-ttu-id="76bcd-111">Tekintse át a Azure Marketplace dokumentációját</span><span class="sxs-lookup"><span data-stu-id="76bcd-111">Review the Azure Marketplace documentation</span></span>

<span data-ttu-id="76bcd-112">Az alábbi cikkek olyan információkat tartalmaznak, amelyekről a folytatás előtt tudnia kell.</span><span class="sxs-lookup"><span data-stu-id="76bcd-112">The articles below contain information you should know before continuing.</span></span> 

- [<span data-ttu-id="76bcd-113">Dynamics 365 for Customer Engagement- és PowerApps-ajánlat létrehozása</span><span class="sxs-lookup"><span data-stu-id="76bcd-113">Create a Dynamics 365 for Customer Engagement & PowerApps offer</span></span>](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [<span data-ttu-id="76bcd-114">Kereskedelmi piactéri fiók létrehozása a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="76bcd-114">Create a commercial marketplace account in Partner Center</span></span>](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a><span data-ttu-id="76bcd-115">Az ajánlatazonosító létrehozása</span><span class="sxs-lookup"><span data-stu-id="76bcd-115">Create your Offer ID</span></span>

<span data-ttu-id="76bcd-116">Az alábbi eljárásokban meg kell adnia egy ajánlatazonosítót.</span><span class="sxs-lookup"><span data-stu-id="76bcd-116">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="76bcd-117">Most egy kis idő alatt meg kell szereznie egy megfelelő ajánlatazonosítót, és vegye figyelembe a következő pontokat:</span><span class="sxs-lookup"><span data-stu-id="76bcd-117">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="76bcd-118">Ez az azonosító látható az ügyfelek számára a Marketplace-ajánlat webcímén, és Azure Resource Manager sablonokat, ha van ilyen.</span><span class="sxs-lookup"><span data-stu-id="76bcd-118">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="76bcd-119">Az ajánlatazonosítónak és a közzétevő azonosítójának 40 karakternél nem hosszabbnak kell lennie.</span><span class="sxs-lookup"><span data-stu-id="76bcd-119">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="76bcd-120">Csak kisbetűket és számokat használjon.</span><span class="sxs-lookup"><span data-stu-id="76bcd-120">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="76bcd-121">Az ajánlatazonosító tartalmazhat kötőjelet és aláhúzásjelet, de szóközt nem.</span><span class="sxs-lookup"><span data-stu-id="76bcd-121">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="76bcd-122">Ha például a közzétevő azonosítója testpublisherid, és a test-offer-1 címet adja meg, az ajánlat webcíme https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 lesz.</span><span class="sxs-lookup"><span data-stu-id="76bcd-122">For example, if your Publisher ID is testpublisherid and you enter test-offer-1, the offer web address will be https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1.</span></span>
- <span data-ttu-id="76bcd-123">Ez az azonosító a Létrehozás lehetőséget választva nem **módosítható.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-123">This ID can't be changed after you select **Create**.</span></span>

### <a name="create-your-offer-alias"></a><span data-ttu-id="76bcd-124">Ajánlat aliasának létrehozása</span><span class="sxs-lookup"><span data-stu-id="76bcd-124">Create your Offer alias</span></span>

<span data-ttu-id="76bcd-125">Az Ajánlat aliasa az ajánlathoz használt név a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="76bcd-125">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="76bcd-126">Szüksége lesz egy megfelelő Offer aliasra is, amely az alábbi irányelveket követi:</span><span class="sxs-lookup"><span data-stu-id="76bcd-126">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="76bcd-127">Ez a név nem használatos a piactéren, és eltér az ajánlat nevétől és az ügyfelek számára megjelenő egyéb értékektől.</span><span class="sxs-lookup"><span data-stu-id="76bcd-127">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="76bcd-128">Ez a név a Létrehozás kiválasztása után már nem módosítható.</span><span class="sxs-lookup"><span data-stu-id="76bcd-128">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="76bcd-129">Az ajánlat létrehozása</span><span class="sxs-lookup"><span data-stu-id="76bcd-129">Create your offer</span></span>

<span data-ttu-id="76bcd-130">A licencelési folyamat első lépése a kereskedelmi piactéri ajánlat létrehozása.</span><span class="sxs-lookup"><span data-stu-id="76bcd-130">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="76bcd-131">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="76bcd-131">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="76bcd-132">A bal oldali navigációs menüben válassza a **Kereskedelmi piactér/Áttekintés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-132">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="76bcd-133">Az Áttekintés oldal tetején válassza az Új ajánlat lehetőséget, majd a **Dynamics 365 for Customer Engagement & PowerApps lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-133">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="76bcd-134">Adja meg a korábban létrehozott **ajánlatazonosítót** és ajánlat aliast. </span><span class="sxs-lookup"><span data-stu-id="76bcd-134">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="76bcd-135">Válassza **a Létrehozás** lehetőséget az ajánlat létrehozásához és a folytatáshoz.</span><span class="sxs-lookup"><span data-stu-id="76bcd-135">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="76bcd-136">Válassza ki a licencelési beállításokat.</span><span class="sxs-lookup"><span data-stu-id="76bcd-136">Choose your licensing options.</span></span>

    - <span data-ttu-id="76bcd-137">Ha engedélyezni szeretné az ajánlat licenckezelését, válassza az **Alkalmazáslicenc-kezelés engedélyezése a Microsofton keresztül** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="76bcd-137">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="76bcd-138">Ez egy egyszeres beállítás, és nem módosíthatja az ajánlat közzététele után.</span><span class="sxs-lookup"><span data-stu-id="76bcd-138">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="76bcd-139">Azt is engedélyezheti, hogy az ügyfelek licenc nélkül futtatják az alkalmazás alapfunkcióit, és prémium szintű funkciókat futtassanak a licenc vásárlása után.</span><span class="sxs-lookup"><span data-stu-id="76bcd-139">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="76bcd-140">Ehhez jelölje be Az alkalmazás telepítésének engedélyezése az ügyfelek számára akkor is, ha nincs **licenc hozzárendelve jelölőnégyzetet.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-140">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="76bcd-141">Ha nem szeretné, hogy az ajánlatában engedélyezve legyen a licenckezelés, válassza a **Get it now (Free) (Szerezze be az ingyenes)** lehetőséget, az **Ingyenes** próbaverziót, vagy a Contact **me (Kapcsolatfelvétel) lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-141">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="76bcd-142">Csomag létrehozása</span><span class="sxs-lookup"><span data-stu-id="76bcd-142">Create your plan</span></span>

<span data-ttu-id="76bcd-143">Ezekben a lépésekben meghatározhatja az ajánlathoz engedélyezni kívánt csomagokat vagy csomagokat.</span><span class="sxs-lookup"><span data-stu-id="76bcd-143">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="76bcd-144">A bal oldali navigációs menüben válassza a **Csomag áttekintése,** majd az **Új csomag létrehozása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-144">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="76bcd-145">Adja meg a **csomagazonosítót** és a **csomag nevét,** majd válassza a **Létrehozás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-145">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="76bcd-146">A **Csomaglista lapon** adja meg a **csomag leírását.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-146">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="76bcd-147">A leírás mentéshez és a későbbi befejezéshez válassza a **Piszkozat mentése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-147">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="76bcd-148">Ha elkészült, válassza az Áttekintés **és közzététel lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-148">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="76bcd-149">A csomaginformációk mostantól megjelennek az ajánlatlistában appsource.microsoft.com (csomagok szakasz) alatt.</span><span class="sxs-lookup"><span data-stu-id="76bcd-149">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="76bcd-150">Miután létrehozta az ajánlat összes csomagját, ki kell másolnia az egyes csomagok szolgáltatásazonosítóját.</span><span class="sxs-lookup"><span data-stu-id="76bcd-150">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="76bcd-151">Válassza **a Plan overview (Csomag** áttekintése) lehetőséget a Plan listing (Csomaglista) lap tetején.</span><span class="sxs-lookup"><span data-stu-id="76bcd-151">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="76bcd-152">Másolja az egyes tervek szolgáltatásazonosítóját egy biztonságos helyre.</span><span class="sxs-lookup"><span data-stu-id="76bcd-152">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="76bcd-153">Szolgáltatás-idok hozzáadása a megoldáshoz</span><span class="sxs-lookup"><span data-stu-id="76bcd-153">Add Service IDs to your solution</span></span>

<span data-ttu-id="76bcd-154">A következő lépés a megoldás frissítése úgy, hogy hozzáadja a szolgáltatás-értékeket az összes másolt csomaghoz.</span><span class="sxs-lookup"><span data-stu-id="76bcd-154">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="76bcd-155">Ezzel kapcsolatos útmutatásért lásd: [Create an AppSource Package for your solution (AppSource-csomag létrehozása a megoldáshoz).](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)</span><span class="sxs-lookup"><span data-stu-id="76bcd-155">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="76bcd-156">Csomag feltöltése és az ajánlat közzététele</span><span class="sxs-lookup"><span data-stu-id="76bcd-156">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="76bcd-157">A bal oldali navigációs panelen válassza a **Kereskedelmi piactér** lehetőséget, majd a **Technikai konfiguráció lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-157">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="76bcd-158">Az **Alaplicenc-modell alatt válassza** a Felhasználó **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-158">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="76bcd-159">A **CRM-csomag alatt** adja meg a csomag helyének URL-címét.</span><span class="sxs-lookup"><span data-stu-id="76bcd-159">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="76bcd-160">A bal oldali navigációs ablaktábla többi lapjával adja meg az egyéb szükséges adatokat.</span><span class="sxs-lookup"><span data-stu-id="76bcd-160">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="76bcd-161">Ha végzett, válassza az Áttekintés **és közzététel lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-161">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="76bcd-162">Az ajánlat közzététele után áttekintjük és ellenőrizzük az adatait.</span><span class="sxs-lookup"><span data-stu-id="76bcd-162">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="76bcd-163">Ha bármilyen probléma van a folyamattal, értesítjük Önt.</span><span class="sxs-lookup"><span data-stu-id="76bcd-163">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="76bcd-164">Ha minden probléma megoldódott, értesítést kap arról, hogy az ajánlata elérhető az AppSource-ban.</span><span class="sxs-lookup"><span data-stu-id="76bcd-164">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="76bcd-165">Ezen a ponton élő adásra lehet képes.</span><span class="sxs-lookup"><span data-stu-id="76bcd-165">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="76bcd-166">Az ajánlat élő adásban Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="76bcd-166">Make your offer live in Partner Center</span></span>

<span data-ttu-id="76bcd-167">Az alábbi eljárás végigvezeti az ajánlat az AppSource-ban való élő készítés folyamatán.</span><span class="sxs-lookup"><span data-stu-id="76bcd-167">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="76bcd-168">A folyamattal kapcsolatos további információkért lásd: [Bevezetés a termékoldali lehetőségekbe.](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)</span><span class="sxs-lookup"><span data-stu-id="76bcd-168">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="76bcd-169">Az ajánlat közzététele után az élő adás 4–6 órát fog igénybe venni.</span><span class="sxs-lookup"><span data-stu-id="76bcd-169">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="76bcd-170">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="76bcd-170">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="76bcd-171">A bal oldali navigációs menüben válassza a **Kereskedelmi piactér/Áttekintés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-171">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="76bcd-172">Az Áttekintés **lapon** keresse meg a keresett ajánlatot.</span><span class="sxs-lookup"><span data-stu-id="76bcd-172">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="76bcd-173">A közzétételre kész ajánlatok előzetes verziójúak **lesznek.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-173">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="76bcd-174">Válassza ki az ajánlatot.</span><span class="sxs-lookup"><span data-stu-id="76bcd-174">Select the offer.</span></span>
4. <span data-ttu-id="76bcd-175">Az Ajánlat **áttekintése lapon** válassza az Élő **adásba lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-175">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="76bcd-176">Az ajánlat 4-6 óra múlva lesz élő.</span><span class="sxs-lookup"><span data-stu-id="76bcd-176">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="76bcd-177">Az ajánlatoldalt az AppSource-on az Ajánlat áttekintő oldalának alján található **AppSource** hivatkozásra **kattintva láthatja.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-177">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="76bcd-178">**Licenccel rendelkező ajánlatok** esetén: Ha az ajánlatához licencellenőrzés szükséges, a felhasználók csak a Kapcsolatfelvétel elemre kattintva léphetnek be az érdeklődőbe, hogy kommunikáljanak velük.</span><span class="sxs-lookup"><span data-stu-id="76bcd-178">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="76bcd-179">**Ingyenes telepítési lehetőséggel** rendelkező licenccel rendelkező ajánlatok esetén: Ha az ajánlathoz nincs szükség licencellenőrzésre, **a** rendszergazdai felhasználók a Kapcsolatfelvétel lehetőség mellett egy Azonnali lekért gombot is **láthatnak.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-179">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="76bcd-180">Azok a felhasználók, akik ki szeretnék próbálni az ingyenes telepítési lehetőséget, a **Get It Now**(Szerezze be most) gombra kattintva telepítik az ajánlatot a felügyeleti Power Platform központban.</span><span class="sxs-lookup"><span data-stu-id="76bcd-180">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="76bcd-181">A felhasználók továbbra is használhatjak a **Kapcsolatfelvétel a velem** kapcsolatot, ha kérdéseik vannak, vagy ha fizetős csomagra szeretnék frissíteni.</span><span class="sxs-lookup"><span data-stu-id="76bcd-181">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-dealreg"></a><span data-ttu-id="76bcd-182">ISV Connect-ajánlat regisztrálása a DealRegben</span><span class="sxs-lookup"><span data-stu-id="76bcd-182">Register ISV Connect deal in DealReg</span></span>

<span data-ttu-id="76bcd-183">A következő lépés az ajánlat regisztrálása.</span><span class="sxs-lookup"><span data-stu-id="76bcd-183">The next step is to register your deal.</span></span> <span data-ttu-id="76bcd-184">Ehhez lásd: [Az ügylet regisztrálása.](https://docs.microsoft.com/partner-center/register-deals)</span><span class="sxs-lookup"><span data-stu-id="76bcd-184">To do this, see [Register your deals](https://docs.microsoft.com/partner-center/register-deals).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="76bcd-185">Az ügyfél meghívása</span><span class="sxs-lookup"><span data-stu-id="76bcd-185">Invite the customer</span></span>

<span data-ttu-id="76bcd-186">Az alábbi eljárással hívatja meg az ügyfelet az ajánlatban való részvételre.</span><span class="sxs-lookup"><span data-stu-id="76bcd-186">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="76bcd-187">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="76bcd-187">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="76bcd-188">A bal oldali navigációs menüben válassza a **Kereskedelmi piactér/Áttekintés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-188">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="76bcd-189">Szűrjön **az Elküldött** ügyletekre, válassza a Folyamatban **lapot,** majd válassza ki a kívánt ügyletet.</span><span class="sxs-lookup"><span data-stu-id="76bcd-189">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
4. <span data-ttu-id="76bcd-190">Az ajánlat áttekintő oldalán válassza a **Licencek kezelése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-190">On the overview page for this deal, select **Manage licenses**.</span></span>
5. <span data-ttu-id="76bcd-191">A **Licencek kezelése ablakban** válassza ki az ügyfelet az Ügyfél **adatai** legördülő listából.</span><span class="sxs-lookup"><span data-stu-id="76bcd-191">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="76bcd-192">Ha az ügyfélkapcsolat még nem létezik, válassza a +Új ügyfél **meghívása a jóváhagyáshoz lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-192">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
6. <span data-ttu-id="76bcd-193">Másolja ki a megjelenő hivatkozást.</span><span class="sxs-lookup"><span data-stu-id="76bcd-193">Copy the link that is displayed.</span></span>
7. <span data-ttu-id="76bcd-194">Küldje el e-mailben ezt a hivatkozást az ügyfél számlázási rendszergazdája vagy globális rendszergazdája számára, és használja ezt a hivatkozást a admin.microsoft.com eléréséhez, valamint az Ön által létesított kapcsolat elfogadásához és elfogadásához.</span><span class="sxs-lookup"><span data-stu-id="76bcd-194">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="76bcd-195">A kapcsolat addig nem lesz létrejön, amíg az ügyfél el nem végzi ezt a lépést.</span><span class="sxs-lookup"><span data-stu-id="76bcd-195">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="76bcd-196">Licencek aktiválása, kezelése és eltávolítása</span><span class="sxs-lookup"><span data-stu-id="76bcd-196">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="76bcd-197">Miután az ügyfél létrejött, elkezdhet csomagokat hozzáadni az ajánlatból, és licenceket rendelni az egyes csomagokhoz.</span><span class="sxs-lookup"><span data-stu-id="76bcd-197">Once your customer has been established, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="76bcd-198">Az ajánlat Licencek kezelése ablakában válassza a **+Csomag hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-198">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="76bcd-199">Töltse ki **a Csomag ehhez a megoldáshoz és** a **Licencek száma** mezőket, majd válassza a **Licencek frissítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-199">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="76bcd-200">A licencek a következő admin.microsoft.com az ügyfelek kezelhetik és rendelhetik hozzá az alkalmazottakhoz.</span><span class="sxs-lookup"><span data-stu-id="76bcd-200">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="76bcd-201">Egy meglévő csomag licencszámának módosításához írja be az új számot a **Licencek** száma mezőbe, majd válassza a **Licencek frissítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-201">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="76bcd-202">Egy üzlet licencének inaktiválásához vagy eltávolításához  kattintson a Műveletek mezőben található kuka ikonra, majd válassza a **Licencek frissítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="76bcd-202">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>