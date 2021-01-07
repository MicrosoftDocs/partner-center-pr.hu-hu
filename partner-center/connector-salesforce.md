---
title: A Salesforce CRM-partneri központ közös értékesítési összekötője
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Szinkronizálja az átirányítási adatokat a Salesforce CRM-tel. Az értékesítők ezután a Microsofttal közösen értékesíthetők a CRM-rendszereken belül.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 68b8bdf7a88c1ca8d063cf3198fc49bf87552edb
ms.sourcegitcommit: de2ac2eea26426ae8f962d29ab50b68850318ce6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/07/2021
ms.locfileid: "97960951"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="f8c66-104">Közös értékesítési összekötő a Salesforce CRM-hez – áttekintés</span><span class="sxs-lookup"><span data-stu-id="f8c66-104">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="f8c66-105">Megfelelő szerepkörök</span><span class="sxs-lookup"><span data-stu-id="f8c66-105">Appropriate roles</span></span>

- <span data-ttu-id="f8c66-106">Ajánlói rendszergazda</span><span class="sxs-lookup"><span data-stu-id="f8c66-106">Referrals admin</span></span>
- <span data-ttu-id="f8c66-107">Rendszerfelügyeleti webszolgáltatások vagy Rendszertestreszabó a CRM-ben</span><span class="sxs-lookup"><span data-stu-id="f8c66-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="f8c66-108">A partner Center közös értékesítési összekötője lehetővé teszi, hogy az értékesítők a Microsofttal közösen értékesítsenek a CRM-rendszereken belül.</span><span class="sxs-lookup"><span data-stu-id="f8c66-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="f8c66-109">Nem kell kiképezniük, hogy a partner centerrel együtt kezeljék a közös értékesítési ajánlatokat.</span><span class="sxs-lookup"><span data-stu-id="f8c66-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="f8c66-110">A közös értékesítésű összekötők használatával új, közösen értékesíthető hivatkozást hozhat létre a Microsoft-értékesítők bevonásához, a Microsoft-értékesítőtől kapott hivatkozásokat, az átirányítások elfogadását/elutasítását, az ügyleti adatok módosítását, például az ügyleti értéket és a zárási dátumot.</span><span class="sxs-lookup"><span data-stu-id="f8c66-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="f8c66-111">Ezeket a közös értékesítési ajánlatokat a Microsoft-értékesítők frissítései is megkapják.</span><span class="sxs-lookup"><span data-stu-id="f8c66-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="f8c66-112">Az összes átirányítási munkát elvégezheti, miközben a választott CRM-en belül dolgozik, nem pedig a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="f8c66-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="f8c66-113">A megoldás a Microsoft Power automatizálási megoldásán alapul, és a partner Center API-kat használja.</span><span class="sxs-lookup"><span data-stu-id="f8c66-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="f8c66-114">Az Előfeltételek telepítése előtt</span><span class="sxs-lookup"><span data-stu-id="f8c66-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="f8c66-115">**Témakörök**</span><span class="sxs-lookup"><span data-stu-id="f8c66-115">**Topics**</span></span>   |<span data-ttu-id="f8c66-116">**Részletek**</span><span class="sxs-lookup"><span data-stu-id="f8c66-116">**Details**</span></span>   |<span data-ttu-id="f8c66-117">**Hivatkozások**</span><span class="sxs-lookup"><span data-stu-id="f8c66-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="f8c66-118">Microsoft Partner Network azonosítója</span><span class="sxs-lookup"><span data-stu-id="f8c66-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="f8c66-119">Érvényes MPN-AZONOSÍTÓra van szüksége</span><span class="sxs-lookup"><span data-stu-id="f8c66-119">You need a valid MPN ID</span></span>|<span data-ttu-id="f8c66-120">Az [MPN](https://partner.microsoft.com/) csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="f8c66-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="f8c66-121">Közös értékesítés kész</span><span class="sxs-lookup"><span data-stu-id="f8c66-121">Co-sell ready</span></span>|<span data-ttu-id="f8c66-122">Az IP-/szolgáltatási megoldásnak közös értékesítéssel kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="f8c66-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="f8c66-123">Értékesítés a Microsofttal</span><span class="sxs-lookup"><span data-stu-id="f8c66-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="f8c66-124">Partnerközpont-fiók</span><span class="sxs-lookup"><span data-stu-id="f8c66-124">Partner Center account</span></span>|<span data-ttu-id="f8c66-125">A partner Center-bérlőhöz társított MPN-AZONOSÍTÓnak meg kell egyeznie a közös értékesítési megoldáshoz társított MPN-azonosítóval.</span><span class="sxs-lookup"><span data-stu-id="f8c66-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="f8c66-126">Az összekötők üzembe helyezése előtt győződjön meg arról, hogy a partner Center portálon megtekintheti a közös értékesítéssel kapcsolatos hivatkozásokat.</span><span class="sxs-lookup"><span data-stu-id="f8c66-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="f8c66-127">Saját fiók kezelése</span><span class="sxs-lookup"><span data-stu-id="f8c66-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="f8c66-128">A partner Center felhasználói szerepkörei</span><span class="sxs-lookup"><span data-stu-id="f8c66-128">Partner Center user roles</span></span>|<span data-ttu-id="f8c66-129">Az összekötőket telepítő és használó alkalmazottnak hivatkozói rendszergazdának kell lennie</span><span class="sxs-lookup"><span data-stu-id="f8c66-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="f8c66-130">Felhasználói szerepkörök és engedélyek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="f8c66-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="f8c66-131">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="f8c66-131">Salesforce CRM</span></span>|<span data-ttu-id="f8c66-132">A CRM-felhasználói szerepkör a rendszergazda vagy a rendszertestreszabó</span><span class="sxs-lookup"><span data-stu-id="f8c66-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="f8c66-133">Szerepkörök társítása a Salesforce CRM-ben</span><span class="sxs-lookup"><span data-stu-id="f8c66-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="f8c66-134">Power automatizáló folyamat fiókja</span><span class="sxs-lookup"><span data-stu-id="f8c66-134">Power Automate Flow Account</span></span>|<span data-ttu-id="f8c66-135">Aktív [Power automatizáló](https://flow.microsoft.com) fiók a CRM rendszer-rendszergazda vagy Rendszertestreszabó számára.</span><span class="sxs-lookup"><span data-stu-id="f8c66-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="f8c66-136">A telepítés előtt a felhasználónak legalább egyszer be kell jelentkeznie az [energiagazdálkodásba](https://flow.microsoft.com) .</span><span class="sxs-lookup"><span data-stu-id="f8c66-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="f8c66-137">A Salesforce-csomag telepítése a Microsoft egyéni mezőihez</span><span class="sxs-lookup"><span data-stu-id="f8c66-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="f8c66-138">Ha szinkronizálni szeretné az átirányításokat a partner Center és a Salesforce CRM között, akkor az automatizálási megoldásnak egyértelműen azonosítania kell a Microsoft-specifikus átirányítási mezőket.</span><span class="sxs-lookup"><span data-stu-id="f8c66-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="f8c66-139">Ezzel a kijelöléssel a partner értékesítői csapatai eldönthetik, hogy mely ajánlásokat szeretnék megosztani a Microsofttal a közös értékesítéshez.</span><span class="sxs-lookup"><span data-stu-id="f8c66-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="f8c66-140">A Salesforce-ben aktiválja a **megjegyzéseket** , és adja hozzá a lehetőségek kapcsolódó listához.</span><span class="sxs-lookup"><span data-stu-id="f8c66-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="f8c66-141">Referencia</span><span class="sxs-lookup"><span data-stu-id="f8c66-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="f8c66-142">Aktiválja a **lehetőség csapatait** a következő lépések végrehajtásával:</span><span class="sxs-lookup"><span data-stu-id="f8c66-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="f8c66-143">A telepítőben a **gyors keresés** mező használatával keresse meg a lehetőség csapatának beállításait.</span><span class="sxs-lookup"><span data-stu-id="f8c66-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="f8c66-144">Szükség szerint adja meg a beállításokat.</span><span class="sxs-lookup"><span data-stu-id="f8c66-144">Define the settings as needed.</span></span>
[<span data-ttu-id="f8c66-145">Referencia</span><span class="sxs-lookup"><span data-stu-id="f8c66-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="f8c66-146">A Salesforce-ben telepítse az egyéni mezőket és objektumokat az alábbi Package Installer használatával.</span><span class="sxs-lookup"><span data-stu-id="f8c66-146">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="f8c66-147">[Ide](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) kattintva telepítheti a csomagot bármely vállalatra.</span><span class="sxs-lookup"><span data-stu-id="f8c66-147">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) to install the package into any company.</span></span>


<span data-ttu-id="f8c66-148">Megjegyzés: Ha egy sandbox-ba telepít, az URL kezdeti részét le kell cserélnie a http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="f8c66-148">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="f8c66-149">A Salesforce-ben adja hozzá a Microsoft-megoldásokat a **lehetőséghez** kapcsolódó listához.</span><span class="sxs-lookup"><span data-stu-id="f8c66-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="f8c66-150">A Hozzáadás után kattintson a **csavarkulcs** ikonra és a frissítés tulajdonságai elemre.</span><span class="sxs-lookup"><span data-stu-id="f8c66-150">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="f8c66-151">Ajánlott eljárás: tesztelés az élő indítás előtt</span><span class="sxs-lookup"><span data-stu-id="f8c66-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="f8c66-152">Mielőtt telepítené, konfigurálja és testreszabja az automatizálási megoldást az éles környezetben, mindenképpen tesztelje a megoldást egy átmeneti CRM-példányon.</span><span class="sxs-lookup"><span data-stu-id="f8c66-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="f8c66-153">Telepítse a Microsoft Power automatizáló megoldást átmeneti környezetben vagy CRM-példányon.</span><span class="sxs-lookup"><span data-stu-id="f8c66-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="f8c66-154">Készítsen másolatot a megoldásról, és futtassa a konfigurációt és a Power automatizálja a folyamatokat az átmeneti környezetben.</span><span class="sxs-lookup"><span data-stu-id="f8c66-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="f8c66-155">Tesztelje a megoldást egy átmeneti vagy CRM-példányon.</span><span class="sxs-lookup"><span data-stu-id="f8c66-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="f8c66-156">Sikeres, az importálás felügyelt megoldásként az üzemi példányra.</span><span class="sxs-lookup"><span data-stu-id="f8c66-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="f8c66-157">A Salesforce CRM-hez készült partner Center-átirányítási szinkronizálás telepítése</span><span class="sxs-lookup"><span data-stu-id="f8c66-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="f8c66-158">Nyissa meg a [Power Automatet](https://flow.microsoft.com) , és válassza a **környezetek** lehetőséget a jobb felső sarokban.</span><span class="sxs-lookup"><span data-stu-id="f8c66-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="f8c66-159">Ekkor megjelenik az elérhető CRM-példányok.</span><span class="sxs-lookup"><span data-stu-id="f8c66-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="f8c66-160">Válassza ki a megfelelő CRM-példányt a jobb felső sarokban lévő legördülő menüből.</span><span class="sxs-lookup"><span data-stu-id="f8c66-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="f8c66-161">A bal oldali navigációs sávon válassza a **megoldások** elemet.</span><span class="sxs-lookup"><span data-stu-id="f8c66-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="f8c66-162">Kattintson a felső menüben található **AppSource megnyitása** hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="f8c66-162">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource megnyitása":::

5. <span data-ttu-id="f8c66-164">Keressen rá a Salesforce-hez készült **partner Center-összekötők** az előugró képernyőn.</span><span class="sxs-lookup"><span data-stu-id="f8c66-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="f8c66-166">Kattintson a **Letöltés most** gombra, és **folytassa a művelettel**.</span><span class="sxs-lookup"><span data-stu-id="f8c66-166">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="f8c66-167">Ekkor megnyílik a lap, amelyen kiválaszthatja az Salesforce CRM-környezetet az alkalmazás telepítéséhez.</span><span class="sxs-lookup"><span data-stu-id="f8c66-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="f8c66-168">Fogadja el a feltételeket és a kikötéseket.</span><span class="sxs-lookup"><span data-stu-id="f8c66-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Rendelkezésre álló CRM":::

8. <span data-ttu-id="f8c66-170">Ezután átirányítja a **megoldások kezelése** lapra.</span><span class="sxs-lookup"><span data-stu-id="f8c66-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="f8c66-171">A lap alján található nyílgombok segítségével navigáljon a "partneri központhoz".</span><span class="sxs-lookup"><span data-stu-id="f8c66-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="f8c66-172">A **telepítés ütemezése** a partner Center Referrals megoldás mellett jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="f8c66-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="f8c66-173">A telepítés 10-15 percet vesz igénybe.</span><span class="sxs-lookup"><span data-stu-id="f8c66-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="f8c66-174">A telepítés befejezése után váltson vissza a [Power automatizálás](https://flow.microsoft.com) szolgáltatásra, és válassza a bal oldali navigációs terület **megoldásait** .</span><span class="sxs-lookup"><span data-stu-id="f8c66-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="f8c66-175">Figyelje meg, hogy a **Salesforce-hez készült fiókpartner-szinkronizálás** a megoldások listájában érhető el.</span><span class="sxs-lookup"><span data-stu-id="f8c66-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="f8c66-176">Válassza ki **a partneri központ átirányítási szinkronizálása Salesforce** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8c66-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="f8c66-177">A következő energiagazdálkodási folyamatok és entitások érhetők el:</span><span class="sxs-lookup"><span data-stu-id="f8c66-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce folyamatok":::



## <a name="configure-the-solution"></a><span data-ttu-id="f8c66-179">A megoldás konfigurálása</span><span class="sxs-lookup"><span data-stu-id="f8c66-179">Configure the solution</span></span>

1. <span data-ttu-id="f8c66-180">Miután telepítette a megoldást a CRM-példányba, váltson vissza a [Power automatizálás](https://flow.microsoft.com/)szolgáltatásra.</span><span class="sxs-lookup"><span data-stu-id="f8c66-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="f8c66-181">A jobb felső sarokban található **környezetek** legördülő listából válassza ki azt a CRM-példányt, amelyen az automatizálási megoldást telepítette.</span><span class="sxs-lookup"><span data-stu-id="f8c66-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="f8c66-182">A három felhasználói fiókot összekapcsoló kapcsolatokat kell létrehoznia:</span><span class="sxs-lookup"><span data-stu-id="f8c66-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="f8c66-183">A partner Center felhasználója az Ajánlói rendszergazdai hitelesítő adatokkal</span><span class="sxs-lookup"><span data-stu-id="f8c66-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="f8c66-184">Partnerközpont – események</span><span class="sxs-lookup"><span data-stu-id="f8c66-184">Partner Center Events</span></span>
    - <span data-ttu-id="f8c66-185">A CRM-rendszergazda a megoldásban a Power automatizálja a folyamatokat.</span><span class="sxs-lookup"><span data-stu-id="f8c66-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="f8c66-186">Válassza a bal oldali navigációs sávon a **kapcsolatok** lehetőséget, majd a listából válassza ki a "partner-központra hivatkozó" megoldást.</span><span class="sxs-lookup"><span data-stu-id="f8c66-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="f8c66-187">Hozzon létre egy kapcsolatokat a **kapcsolatok létrehozása** lehetőségre kattintva.</span><span class="sxs-lookup"><span data-stu-id="f8c66-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Kapcsolat létrehozása":::

- <span data-ttu-id="f8c66-189">A jobb felső sarokban található keresési sávban keresse meg a partner Center-hivatkozásokat (előzetes verzió).</span><span class="sxs-lookup"><span data-stu-id="f8c66-189">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="f8c66-190">Hozzon létre kapcsolatot a fiókpartner-felhasználó számára az Ajánlói rendszergazda hitelesítő adatokkal kapcsolatos szerepkörével.</span><span class="sxs-lookup"><span data-stu-id="f8c66-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="f8c66-191">Ezután hozzon létre egy partneri központ-esemény kapcsolatot a partner Center-felhasználó számára az Ajánlói rendszergazda hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="f8c66-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="f8c66-192">Hozzon létre egy Salesforce-kapcsolatokat a CRM-rendszergazda felhasználó számára.</span><span class="sxs-lookup"><span data-stu-id="f8c66-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="f8c66-193">Az összes hozzáadott kapcsolat után a következő kapcsolatokat kell látnia a környezetben:</span><span class="sxs-lookup"><span data-stu-id="f8c66-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Kapcsolatok megfigyelése":::

### <a name="edit-the-connections"></a><span data-ttu-id="f8c66-195">Kapcsolatok szerkesztése</span><span class="sxs-lookup"><span data-stu-id="f8c66-195">Edit the connections</span></span>

1. <span data-ttu-id="f8c66-196">Térjen vissza a megoldások lapra, és válassza az **alapértelmezett megoldás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8c66-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="f8c66-197">Válassza a **kapcsolatok referenciája (előzetes verzió)** lehetőséget az **összes** elemre kattintva.</span><span class="sxs-lookup"><span data-stu-id="f8c66-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Összekötők szerkesztésének megkezdése":::

2. <span data-ttu-id="f8c66-199">Szerkessze az egyes kapcsolatokat egyenként a három pont ikon kiválasztásával.</span><span class="sxs-lookup"><span data-stu-id="f8c66-199">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="f8c66-200">Adja hozzá a megfelelő kapcsolatokat.</span><span class="sxs-lookup"><span data-stu-id="f8c66-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Összekötők szerkesztése":::

3. <span data-ttu-id="f8c66-202">Kapcsolja be a folyamatokat a következő sorozatban:</span><span class="sxs-lookup"><span data-stu-id="f8c66-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="f8c66-203">A partner Center webhook-regisztrációja (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="f8c66-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="f8c66-204">Közös értékesítéssel való hivatkozás létrehozása – Salesforce (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="f8c66-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f8c66-205">Partneri központ a Microsoft közös értékesítési hivatkozási frissítései a Salesforce-be (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="f8c66-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="f8c66-206">Partneri központ – Salesforce (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="f8c66-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="f8c66-207">Salesforce (Insider előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="f8c66-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f8c66-208">Salesforce lehetőség a partneri központhoz (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="f8c66-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f8c66-209">Salesforce Microsoft-megoldások a partner Centerhez (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="f8c66-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="f8c66-210">A webhook API-k használata az Erőforrás-változási események regisztrálásához</span><span class="sxs-lookup"><span data-stu-id="f8c66-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="f8c66-211">A partner Center webhook API-k lehetővé teszik az Erőforrás-változási események regisztrálását.</span><span class="sxs-lookup"><span data-stu-id="f8c66-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="f8c66-212">Ezeket a változási eseményeket a rendszer HTTP-bejegyzésekként küldi el az URL-címre.</span><span class="sxs-lookup"><span data-stu-id="f8c66-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="f8c66-213">Az URL-cím regisztrálásához válassza a **partner Center webhook-regisztráció (belső előzetes verzió)** energiagazdálkodási folyamatát.</span><span class="sxs-lookup"><span data-stu-id="f8c66-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="f8c66-214">Vegyen fel kapcsolatokat az (a.) partner Center-felhasználóhoz az Ajánlói rendszergazdai hitelesítő adatokkal (b.) a következő Kiemelt módon:</span><span class="sxs-lookup"><span data-stu-id="f8c66-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Eseményindító":::

3. <span data-ttu-id="f8c66-216">Ha ezeket a frissítéseket végzi, a következőt fogja látni:</span><span class="sxs-lookup"><span data-stu-id="f8c66-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhookok":::

4. <span data-ttu-id="f8c66-218">Mentse a módosításokat, és válassza **a bekapcsolás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8c66-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="f8c66-219">A következő lépések végrehajtásával engedélyezheti a partneri központ webhookok számára az események változásának figyelését:</span><span class="sxs-lookup"><span data-stu-id="f8c66-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="f8c66-220">Válassza ki **a partneri központot a CRM Salesforce (belső előzetes verzió)**.</span><span class="sxs-lookup"><span data-stu-id="f8c66-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="f8c66-221">Válassza a **Szerkesztés** ikont, és válassza ki a **http-kérés fogadásakor** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8c66-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="f8c66-222">Kattintson a **Másolás** ikonra a megadott http post URL-cím másolásához.</span><span class="sxs-lookup"><span data-stu-id="f8c66-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL-cím másolása":::

8. <span data-ttu-id="f8c66-224">Most válassza ki a "partneri központ webhook-regisztráció (Insider előzetes verzió)" energiaellátás-automatizálási folyamat elemet, és válassza a **Futtatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8c66-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="f8c66-225">Győződjön meg arról, hogy a jobb oldali ablaktáblán megnyílik a "Futtatás folyamata" ablak, és kattintson a **Folytatás** gombra.</span><span class="sxs-lookup"><span data-stu-id="f8c66-225">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="f8c66-226">Adja meg a következő részleteket:</span><span class="sxs-lookup"><span data-stu-id="f8c66-226">Enter the following details:</span></span>

    1. <span data-ttu-id="f8c66-227">**Http-trigger végpontja**: a korábbi lépésből másolt URL-cím</span><span class="sxs-lookup"><span data-stu-id="f8c66-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="f8c66-228">**Regisztrálni kívánt események**: "referral-created" és "referral-frissítve"</span><span class="sxs-lookup"><span data-stu-id="f8c66-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="f8c66-229">**Meglévő trigger-végpontok felülírása (ha van**): igen (Ez felülírja a meglévő végpontokat.)</span><span class="sxs-lookup"><span data-stu-id="f8c66-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="f8c66-230">Válassza a **Futtatás** lehetőséget, majd kattintson a **Kész gombra.**</span><span class="sxs-lookup"><span data-stu-id="f8c66-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="f8c66-231">A webhook mostantól figyelheti az események létrehozását és frissítését.</span><span class="sxs-lookup"><span data-stu-id="f8c66-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="f8c66-232">Szinkronizálási lépések testreszabása</span><span class="sxs-lookup"><span data-stu-id="f8c66-232">Customize synchronization steps</span></span>

<span data-ttu-id="f8c66-233">Ha a partneri központ és a CRM-rendszer között szinkronizálja a közös értékesítésre való átirányítást, akkor a partner Center-számítógépen szinkronizált mezők itt vannak felsorolva.</span><span class="sxs-lookup"><span data-stu-id="f8c66-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="f8c66-234">A CRM-rendszerek gyakran testre szabottak.</span><span class="sxs-lookup"><span data-stu-id="f8c66-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="f8c66-235">Testreszabhatja a Power automatizáló folyamatokat.</span><span class="sxs-lookup"><span data-stu-id="f8c66-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="f8c66-236">Kövesse a mező-hozzárendelési útmutatót, és szükség esetén végezze el a megfelelő módosításokat a Power automatizáló folyamatok lépéseiben.</span><span class="sxs-lookup"><span data-stu-id="f8c66-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="f8c66-237">A Microsoft-partneri központok a CRM-alapú hozzárendelésekhez vannak megadva, de a CRM-környezet alapján a mezők további testreszabására is lehetősége van.</span><span class="sxs-lookup"><span data-stu-id="f8c66-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="f8c66-238">Az egyes energiagazdálkodási folyamatok több lépését az igényeinek megfelelően testre szabhatja.</span><span class="sxs-lookup"><span data-stu-id="f8c66-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="f8c66-239">A következő példák az elérhető testreszabásokat szemléltetik:</span><span class="sxs-lookup"><span data-stu-id="f8c66-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="f8c66-240">A partner központ létrehozási vagy frissítési eseményeihez tartozó mezők testreszabása a CRM-hivatkozó szinkronizálásához:</span><span class="sxs-lookup"><span data-stu-id="f8c66-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="f8c66-241">Válassza ki a partneri központot a CRM Salesforce (belső előzetes verzió).</span><span class="sxs-lookup"><span data-stu-id="f8c66-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="f8c66-242">Válassza a **Szerkesztés** lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.</span><span class="sxs-lookup"><span data-stu-id="f8c66-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="f8c66-243">Válassza **a (hatókör) lehetőséget az érdeklődő vagy a lehetőség szinkronizálásához**.</span><span class="sxs-lookup"><span data-stu-id="f8c66-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="f8c66-244">Ha testre szeretné szabni az események létrehozásához tartozó CRM-mezők leképezéseit, válassza ki, hogy **új megosztott lehetőség van-e, majd**.</span><span class="sxs-lookup"><span data-stu-id="f8c66-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="f8c66-245">Válassza ki az allépést, **Ha igen** , majd bontsa ki **az új lehetőség létrehozása lehetőséget a CRM-ben**.</span><span class="sxs-lookup"><span data-stu-id="f8c66-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="f8c66-246">Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató segítségével módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="f8c66-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="f8c66-247">A frissítési események CRM-mezőkhöz való hozzárendelésének testreszabásához kattintson a "(hatókör) – az érdeklődő vagy a lehetőség szinkronizálása" elemre.</span><span class="sxs-lookup"><span data-stu-id="f8c66-247">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="f8c66-248">Válassza ki **, hogy a lehetőség frissítése lehetséges-** e.</span><span class="sxs-lookup"><span data-stu-id="f8c66-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="f8c66-249">**Ha igen** , akkor válassza ki az allépést, majd bontsa ki **, ha a partner Centerben és a CRM-ben a lehetőség-objektumok között van különbség**</span><span class="sxs-lookup"><span data-stu-id="f8c66-249">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="f8c66-250">Jelölje be az **Igen** , majd a **meglévő frissítése lehetőséget** .</span><span class="sxs-lookup"><span data-stu-id="f8c66-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="f8c66-251">A CRM és a számítógép közötti átirányítási szinkronizálás mezőinek testreszabása a frissítési eseményekhez:</span><span class="sxs-lookup"><span data-stu-id="f8c66-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="f8c66-252">Válassza a **Szerkesztés**  lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.</span><span class="sxs-lookup"><span data-stu-id="f8c66-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="f8c66-253">Válassza **a (hatókör) lehetőséget a lehetőség szinkronizálásához**.</span><span class="sxs-lookup"><span data-stu-id="f8c66-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="f8c66-254">Ha a CRM-mezők hozzárendeléseit (mező-hozzárendelések útmutatója alapján) testreszabja a frissítési eseményekhez, akkor válassza ki, hogy van-e **különbség a partner Centerben és a CRM-ben lévő érdeklődő objektumok között**.</span><span class="sxs-lookup"><span data-stu-id="f8c66-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="f8c66-255">Válassza ki az allépést, **Ha igen** , majd bontsa ki az **átirányítási lehetőséget a lehetőségre vonatkozó adattal**.</span><span class="sxs-lookup"><span data-stu-id="f8c66-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="f8c66-256">Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató alapján módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="f8c66-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="f8c66-257">A CRM és a számítógép közötti átirányítási szinkronizálás mezőinek testreszabása az események létrehozásához?</span><span class="sxs-lookup"><span data-stu-id="f8c66-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="f8c66-258">Válassza a **Szerkesztés**  lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.</span><span class="sxs-lookup"><span data-stu-id="f8c66-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="f8c66-259">Válassza ki **(hatókör) az átirányítások szinkronizálását.**</span><span class="sxs-lookup"><span data-stu-id="f8c66-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="f8c66-260">Ha testre kívánja szabni a CRM-mezők hozzárendeléseit (a mező-hozzárendelések útmutatója alapján) az események létrehozásához, válassza a **Microsoft ajánló létrehozása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8c66-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="f8c66-261">Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató alapján módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="f8c66-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="f8c66-262">Végpontok közötti kétirányú, közös értékesítésre hivatkozó átirányítás szinkronizálása</span><span class="sxs-lookup"><span data-stu-id="f8c66-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="f8c66-263">Miután telepítette, konfigurálta és testreszabta az automatizálási megoldást, tesztelheti a Salesforce CRM és a partner Center közötti, közös értékesítéssel való átirányítások szinkronizálását.</span><span class="sxs-lookup"><span data-stu-id="f8c66-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="f8c66-264">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="f8c66-264">Pre-requisites</span></span>

<span data-ttu-id="f8c66-265">Ha szinkronizálni szeretné az átirányításokat a partner Center és a Salesforce CRM között, az automatizálási megoldásnak egyértelműen körzet határának kijelölésében kell a Microsoft-specifikus átirányítási mezőket.</span><span class="sxs-lookup"><span data-stu-id="f8c66-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="f8c66-266">Ez az azonosítás biztosítja az értékesítő csapatának, hogy eldöntse, hogy mely ajánlásokat szeretné megosztani a Microsofttal a közös értékesítéshez.</span><span class="sxs-lookup"><span data-stu-id="f8c66-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="f8c66-267">Az egyéni mezők készlete a Salesforce CRM-megoldási **lehetőség** entitásának partneri központhoz való átirányítási szinkronizálásának részeként érhető el.</span><span class="sxs-lookup"><span data-stu-id="f8c66-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="f8c66-268">Egy CRM-rendszergazda felhasználónak külön CRM-szakaszt kell létrehoznia a **lehetőség** egyéni mezőivel.</span><span class="sxs-lookup"><span data-stu-id="f8c66-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="f8c66-269">A következő egyéni mezők a CRM szakasz részét képezik:</span><span class="sxs-lookup"><span data-stu-id="f8c66-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="f8c66-270">**Szinkronizálás a partner centerrel**: a lehetőség szinkronizálása a Microsoft partner centerrel</span><span class="sxs-lookup"><span data-stu-id="f8c66-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="f8c66-271">**Hivatkozási azonosító**: a Microsoft partner Center ajánlójának írásvédett azonosító mezője</span><span class="sxs-lookup"><span data-stu-id="f8c66-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="f8c66-272">**Referral link**: egy csak olvasható hivatkozás a Microsoft partner Centerben</span><span class="sxs-lookup"><span data-stu-id="f8c66-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="f8c66-273">A **Microsoft súgója**: Segítség szükséges a Microsofttól az átirányításhoz</span><span class="sxs-lookup"><span data-stu-id="f8c66-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="f8c66-274">**Termékek**: a lehetőséghez társított termékek listája</span><span class="sxs-lookup"><span data-stu-id="f8c66-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="f8c66-275">**Naplózás**: írásvédett naplózási nyomvonal a partner Center-hivatkozásokkal való szinkronizáláshoz</span><span class="sxs-lookup"><span data-stu-id="f8c66-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="f8c66-276">FORGATÓKÖNYVEK</span><span class="sxs-lookup"><span data-stu-id="f8c66-276">SCENARIOS:</span></span>

1. <span data-ttu-id="f8c66-277">Átirányítás szinkronizálása a CRM-ben való létrehozáskor vagy frissítésekor, valamint a partner Centerben szinkronizálva:</span><span class="sxs-lookup"><span data-stu-id="f8c66-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="f8c66-278">Jelentkezzen be a Salesforce CRM-környezetbe olyan felhasználóval, aki rendelkezik a CRM **lehetőség** szakaszában láthatóval.</span><span class="sxs-lookup"><span data-stu-id="f8c66-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="f8c66-279">Győződjön meg arról, hogy a Salesforce CRM-környezet "új lehetőség" létrehozásakor a következő szakasz jelenik meg</span><span class="sxs-lookup"><span data-stu-id="f8c66-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-környezet":::

   3. <span data-ttu-id="f8c66-281">Ha ezt a lehetőséget a Microsoft partner centerrel szeretné szinkronizálni, ügyeljen arra, hogy a következő mezőket adja meg a kártya nézetben:</span><span class="sxs-lookup"><span data-stu-id="f8c66-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="f8c66-282">"Szinkronizálás a partner központtal": igen</span><span class="sxs-lookup"><span data-stu-id="f8c66-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="f8c66-283">"Hogyan lehet a Microsoft súgója?": válasszon a következő lehetőségek közül:</span><span class="sxs-lookup"><span data-stu-id="f8c66-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="f8c66-284">Termékek: a termék megoldás-azonosítói</span><span class="sxs-lookup"><span data-stu-id="f8c66-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="f8c66-285">Miután beállította a lehetőség  **szinkronizálását a partner Center** lehetőséggel **Igen**, várjon 10 percet, jelentkezzen be a partner Center-fiókjába.</span><span class="sxs-lookup"><span data-stu-id="f8c66-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="f8c66-286">Az átirányítási adatokat a Salesforce CRM-szel szinkronizálja a rendszer.</span><span class="sxs-lookup"><span data-stu-id="f8c66-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="f8c66-287">Ha a "szinkronizálás a partner központtal" beállítás értéke "yes", ha frissíti a lehetőséget a Salesforce CRM-ben, a módosítások szinkronizálva lesznek a partner Center-fiókjával.</span><span class="sxs-lookup"><span data-stu-id="f8c66-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="f8c66-288">A partner centerrel sikeresen szinkronizált lehetőségek a Salesforce CRM ✔ ikonjával lesznek azonosítva.</span><span class="sxs-lookup"><span data-stu-id="f8c66-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="f8c66-289">Az átirányítás szinkronizálása, ha a Microsoft partner Centerben létrehozták vagy frissítik az átirányítást, és szinkronizálva vannak a Salesforce CRM-környezetben:</span><span class="sxs-lookup"><span data-stu-id="f8c66-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="f8c66-290">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/home).</span><span class="sxs-lookup"><span data-stu-id="f8c66-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="f8c66-291">A bal oldali menüben válassza a **hivatkozók** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f8c66-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="f8c66-292">Hozzon létre egy új, közös értékesítésre hivatkozó hivatkozást a partner Centerben az "új üzlet" lehetőségre kattintva.</span><span class="sxs-lookup"><span data-stu-id="f8c66-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="f8c66-293">Jelentkezzen be a Salesforce CRM-környezetbe.</span><span class="sxs-lookup"><span data-stu-id="f8c66-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="f8c66-294">Navigáljon a **lehetőségek megnyitásához**.</span><span class="sxs-lookup"><span data-stu-id="f8c66-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="f8c66-295">A Microsoft partner Centerben létrehozott hivatkozás mostantól szinkronizálva van a Salesforce CRM-ben.</span><span class="sxs-lookup"><span data-stu-id="f8c66-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce lehetőség képernyő":::

    6. <span data-ttu-id="f8c66-297">Amikor kijelöl egy szinkronizált átirányítást, a rendszer feltölti a kártya nézetének részleteit.</span><span class="sxs-lookup"><span data-stu-id="f8c66-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f8c66-298">További lépések</span><span class="sxs-lookup"><span data-stu-id="f8c66-298">Next steps</span></span>

- [<span data-ttu-id="f8c66-299">Érdeklődők kezelése</span><span class="sxs-lookup"><span data-stu-id="f8c66-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="f8c66-300">Együttes értékesítési lehetőségek kezelése</span><span class="sxs-lookup"><span data-stu-id="f8c66-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="f8c66-301">A partneri központ webhookai</span><span class="sxs-lookup"><span data-stu-id="f8c66-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
