---
title: A Dynamics 365 CRM-partneri központ közös értékesítési összekötője
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Szinkronizálja a partner Centerben lévő hivatkozásokat a Dynamics 365 CRM-hez készült közös értékesítési összekötővel. Az értékesítők ezután a Microsofttal közösen értékesíthetők a CRM-rendszereken belül.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 18a54bf777cb987e8f486f85afcf277e04c1055c
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556361"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="ddfd3-104">Közös értékesítésű összekötő a Dynamics 365 CRM-hez – áttekintés</span><span class="sxs-lookup"><span data-stu-id="ddfd3-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="ddfd3-105">Megfelelő szerepkörök</span><span class="sxs-lookup"><span data-stu-id="ddfd3-105">Appropriate roles</span></span>

- <span data-ttu-id="ddfd3-106">Ajánlói rendszergazda</span><span class="sxs-lookup"><span data-stu-id="ddfd3-106">Referrals admin</span></span>
- <span data-ttu-id="ddfd3-107">Rendszerfelügyeleti webszolgáltatások vagy Rendszertestreszabó a CRM-ben</span><span class="sxs-lookup"><span data-stu-id="ddfd3-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="ddfd3-108">A partner Center közös értékesítési összekötője lehetővé teszi, hogy az értékesítők a Microsofttal közösen értékesítsenek a CRM-rendszereken belül.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="ddfd3-109">Nem kell kiképezniük, hogy a partner centerrel együtt kezeljék a közös értékesítési ajánlatokat.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="ddfd3-110">A közös értékesítésű összekötők használatával létrehozhat egy új, közösen értékesíthető hivatkozást a Microsoft-értékesítők bevonásához, a Microsoft-értékesítőtől kapott hivatkozásokat fogad, elfogadhatja/elutasíthatja az átirányítást, módosíthatja az ügyleti értékeket, például az üzlet értékét és a zárási dátumot.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="ddfd3-111">Ezeket a közös értékesítési ajánlatokat a Microsoft-értékesítők frissítései is megkapják.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="ddfd3-112">Az összes átirányítást megteheti a választott CRM-en belül, nem pedig a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="ddfd3-113">A megoldás a Microsoft Power automatizálási megoldásán alapul, és a partner Center API-kat használja.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="ddfd3-114">Az Előfeltételek telepítése előtt</span><span class="sxs-lookup"><span data-stu-id="ddfd3-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="ddfd3-115">**Témakörök**</span><span class="sxs-lookup"><span data-stu-id="ddfd3-115">**Topics**</span></span>   |<span data-ttu-id="ddfd3-116">**Részletek**</span><span class="sxs-lookup"><span data-stu-id="ddfd3-116">**Details**</span></span>   |<span data-ttu-id="ddfd3-117">**Hivatkozások**</span><span class="sxs-lookup"><span data-stu-id="ddfd3-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="ddfd3-118">Microsoft Partner Network azonosítója</span><span class="sxs-lookup"><span data-stu-id="ddfd3-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="ddfd3-119">Érvényes MPN-AZONOSÍTÓra van szüksége</span><span class="sxs-lookup"><span data-stu-id="ddfd3-119">You need a valid MPN ID</span></span>|<span data-ttu-id="ddfd3-120">Az [MPN](https://partner.microsoft.com/) csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="ddfd3-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="ddfd3-121">Értékesítésre kész</span><span class="sxs-lookup"><span data-stu-id="ddfd3-121">Cosell ready</span></span>|<span data-ttu-id="ddfd3-122">Az IP-/szolgáltatási megoldásnak közös értékesítéssel kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="ddfd3-123">Értékesítés a Microsofttal</span><span class="sxs-lookup"><span data-stu-id="ddfd3-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="ddfd3-124">Partnerközpont-fiók</span><span class="sxs-lookup"><span data-stu-id="ddfd3-124">Partner Center account</span></span>|<span data-ttu-id="ddfd3-125">A partner Center-bérlőhöz társított MPN-AZONOSÍTÓnak meg kell egyeznie a közös értékesítési megoldáshoz társított MPN-azonosítóval.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="ddfd3-126">Az összekötők üzembe helyezése előtt győződjön meg arról, hogy a partner Center portálon megtekintheti a közös értékesítéssel kapcsolatos hivatkozásokat.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="ddfd3-127">Saját fiók kezelése</span><span class="sxs-lookup"><span data-stu-id="ddfd3-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="ddfd3-128">A partner Center felhasználói szerepkörei</span><span class="sxs-lookup"><span data-stu-id="ddfd3-128">Partner Center user roles</span></span>|<span data-ttu-id="ddfd3-129">Az összekötőket telepítő és használó alkalmazottnak hivatkozói rendszergazdának kell lennie</span><span class="sxs-lookup"><span data-stu-id="ddfd3-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="ddfd3-130">Felhasználói szerepkörök és engedélyek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="ddfd3-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="ddfd3-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="ddfd3-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="ddfd3-132">A CRM-felhasználói szerepkör a rendszergazda vagy a rendszertestreszabó</span><span class="sxs-lookup"><span data-stu-id="ddfd3-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="ddfd3-133">Szerepkörök társítása a Dynamics 365-ben</span><span class="sxs-lookup"><span data-stu-id="ddfd3-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="ddfd3-134">Power automatizáló folyamat fiókja</span><span class="sxs-lookup"><span data-stu-id="ddfd3-134">Power Automate Flow Account</span></span>|<span data-ttu-id="ddfd3-135">Aktív [Power automatizáló](https://flow.microsoft.com) fiók a CRM rendszer-rendszergazda vagy Rendszertestreszabó számára.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="ddfd3-136">A telepítés előtt a felhasználónak legalább egyszer be kell jelentkeznie az [energiagazdálkodásba](https://flow.microsoft.com) .</span><span class="sxs-lookup"><span data-stu-id="ddfd3-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="ddfd3-137">A partneri központ átirányítási szinkronizálásának telepítése a Dynamics 365-hez (Power automatizáló megoldás)</span><span class="sxs-lookup"><span data-stu-id="ddfd3-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="ddfd3-138">Nyissa meg a [Power Automatet](https://flow.microsoft.com) , és válassza a **környezetek** lehetőséget a jobb felső sarokban.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="ddfd3-139">Ebben a lépésben az elérhető CRM-példányok jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="ddfd3-140">Válassza ki a megfelelő CRM-példányt a jobb felső sarokban lévő legördülő menüből.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="ddfd3-141">A bal oldali navigációs sávon válassza a **megoldások** elemet.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="ddfd3-142">Kattintson a felső menüben található **AppSource megnyitása** hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource megnyitása":::

5. <span data-ttu-id="ddfd3-144">Keressen rá a Dynamics365-hez készült **partner Center-összekötők** az előugró képernyőn.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="ddfd3-145">Kattintson a **Letöltés most** gombra, és **folytassa a művelettel**.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="ddfd3-146">Ekkor megnyílik a lap, amelyen kiválaszthatja az alkalmazás telepítéséhez szükséges CRM-környezetet (Dynamics 365).</span><span class="sxs-lookup"><span data-stu-id="ddfd3-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="ddfd3-147">Fogadja el a feltételeket és a kikötéseket.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="ddfd3-148">Ezután átirányítja a **megoldások kezelése** lapra.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="ddfd3-149">A lap alján található nyílgombok segítségével navigáljon a "partneri központhoz".</span><span class="sxs-lookup"><span data-stu-id="ddfd3-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="ddfd3-150">A **telepítés ütemezése** a partner Center Referrals megoldás mellett jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="ddfd3-151">A telepítés 10-15 percet vesz igénybe.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="ddfd3-152">A telepítés befejezése után váltson vissza a [Power automatizálás](https://flow.microsoft.com) szolgáltatásra, és válassza a bal oldali navigációs terület **megoldásait** .</span><span class="sxs-lookup"><span data-stu-id="ddfd3-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="ddfd3-153">Figyelje meg, hogy a **partneri központ a Dynamics 365-szinkronizálása** elérhető a megoldások listájában.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="ddfd3-154">Válassza **a partner Center-átirányítási szinkronizálás a Dynamics 365-hez** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="ddfd3-155">A következő energiagazdálkodási folyamatok és entitások érhetők el:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Rendelkezésre álló CRM":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="ddfd3-157">Ajánlott eljárás: tesztelés az élő indítás előtt</span><span class="sxs-lookup"><span data-stu-id="ddfd3-157">Best practice: test before you go live</span></span>

<span data-ttu-id="ddfd3-158">Mielőtt telepítené, konfigurálja és testreszabja az automatizálási megoldást az éles környezetben, mindenképpen tesztelje a megoldást egy átmeneti CRM-példányon.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="ddfd3-159">Telepítse a Microsoft Power automatizáló megoldást átmeneti környezetben vagy CRM-példányon.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="ddfd3-160">Készítsen másolatot a megoldásról, és futtassa a konfigurációt és a Power automatizálja a folyamatokat az átmeneti környezetben.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="ddfd3-161">Tesztelje a megoldást egy átmeneti vagy CRM-példányon.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="ddfd3-162">Sikeres, az importálás felügyelt megoldásként az éles példányra.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="ddfd3-163">A megoldás konfigurálása</span><span class="sxs-lookup"><span data-stu-id="ddfd3-163">Configure the solution</span></span>

1. <span data-ttu-id="ddfd3-164">Miután telepítette a megoldást a CRM-példányba, váltson vissza a [Power automatizálás](https://flow.microsoft.com/)szolgáltatásra.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="ddfd3-165">A jobb felső sarokban található **környezetek** legördülő listából válassza ki azt a CRM-példányt, amelyen az automatizálási megoldást telepítette.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="ddfd3-166">Olyan kapcsolatokat kell létrehoznia, amelyek a három felhasználói fiókot rendelik hozzá:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="ddfd3-167">A partner Center felhasználója az Ajánlói rendszergazdai hitelesítő adatokkal</span><span class="sxs-lookup"><span data-stu-id="ddfd3-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="ddfd3-168">Partnerközpont – események</span><span class="sxs-lookup"><span data-stu-id="ddfd3-168">Partner Center Events</span></span>

   - <span data-ttu-id="ddfd3-169">A CRM-rendszergazda a megoldásban a Power automatizálja a folyamatokat.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="ddfd3-170">Válassza a bal oldali navigációs sávon a **kapcsolatok** lehetőséget, majd a listából válassza ki a "partner-központra hivatkozó" megoldást.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="ddfd3-171">Hozzon létre egy kapcsolatokat a **kapcsolatok létrehozása** lehetőségre kattintva.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Kapcsolat létrehozása":::

      3. <span data-ttu-id="ddfd3-173">A jobb felső sarokban található keresési sávban keresse meg a **partneri központ hivatkozásait (előzetes verzió)** .</span><span class="sxs-lookup"><span data-stu-id="ddfd3-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="ddfd3-174">Hozzon létre kapcsolatot a fiókpartner-felhasználó számára az Ajánlói rendszergazda hitelesítő adatokkal kapcsolatos szerepkörével.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="ddfd3-175">Ezután hozzon létre egy partneri központ-esemény kapcsolatot a partner Center-felhasználó számára az Ajánlói rendszergazda hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="ddfd3-176">Hozzon létre egy Common Data Service (aktuális környezet) kapcsolatokat a CRM-rendszergazda felhasználó számára.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="ddfd3-177">Az összes hozzáadott kapcsolat után a következő kapcsolatokat kell látnia a környezetben:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Kapcsolatok":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="ddfd3-179">Kapcsolatok szerkesztése</span><span class="sxs-lookup"><span data-stu-id="ddfd3-179">Edit the connections</span></span>

1. <span data-ttu-id="ddfd3-180">Térjen vissza a **megoldások** lapra, és válassza az **alapértelmezett megoldás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="ddfd3-181">Válassza a **kapcsolatok referenciája (előzetes verzió)** lehetőséget az **összes** elemre kattintva.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Kapcsolódás":::

2. <span data-ttu-id="ddfd3-183">Szerkessze az egyes kapcsolatokat egyenként a három pont ikon kiválasztásával.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="ddfd3-184">Adja hozzá a megfelelő kapcsolatokat.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Felsorolt kapcsolatok"::: 

3.  <span data-ttu-id="ddfd3-186">Kapcsolja be a folyamatokat a következő sorozatban:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="ddfd3-187">A partner Center webhook-regisztrációja (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="ddfd3-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="ddfd3-188">Közös értékesítésre hivatkozó hivatkozás létrehozása – Dynamics 365 – partneri központ (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="ddfd3-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ddfd3-189">A partner Center Microsoft közös értékesítési hivatkozási frissítései a Dynamics 365-as verzióra (Insider előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="ddfd3-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="ddfd3-190">Partneri központ a Dynamics 365-hoz (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="ddfd3-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="ddfd3-191">Dynamics 365 a partneri központba (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="ddfd3-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ddfd3-192">Dynamics 365 lehetőség a partneri központhoz (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="ddfd3-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ddfd3-193">Dynamics 365 Microsoft-megoldások a partner Centerhez (Insider előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="ddfd3-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="ddfd3-194">A webhook API-k használata az Erőforrás-változási események regisztrálásához</span><span class="sxs-lookup"><span data-stu-id="ddfd3-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="ddfd3-195">A partner Center webhook API-k lehetővé teszik az Erőforrás-változási események regisztrálását.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="ddfd3-196">Ezeket a változási eseményeket a rendszer HTTP-bejegyzésekként küldi el az URL-címre.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="ddfd3-197">Az URL-cím regisztrálásához válassza a **partner Center webhook-regisztráció (belső előzetes verzió)** energiagazdálkodási folyamatát.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="ddfd3-198">Vegyen fel kapcsolatokat az (a.) partner Center-felhasználóhoz az Ajánlói rendszergazdai hitelesítő adatokkal (b.) a következő Kiemelt módon:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Eseményindító":::

3. <span data-ttu-id="ddfd3-200">Ha ezeket a frissítéseket végzi, a következőt fogja látni:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhookok":::

4. <span data-ttu-id="ddfd3-202">Mentse a módosításokat, és válassza **a bekapcsolás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="ddfd3-203">A következő lépésekkel engedélyezheti a partneri központ webhookok számára az események változásának figyelését:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="ddfd3-204">Válassza **a partner központ lehetőséget a Dynamics 365 (belső előzetes verzió)** elemre.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="ddfd3-205">Válassza a **Szerkesztés** ikont, és válassza ki a **http-kérés fogadásakor** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="ddfd3-206">Kattintson a **Másolás** ikonra a megadott http post URL-cím másolásához.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL-cím másolása":::

8. <span data-ttu-id="ddfd3-208">Most válassza ki a "partneri központ webhook-regisztráció (Insider előzetes verzió)" energiaellátás-automatizálási folyamat elemet, és válassza a **Futtatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="ddfd3-209">Győződjön meg arról, hogy a jobb oldali ablaktáblán megnyílik a "Futtatás folyamata" ablak, és kattintson a **Folytatás** gombra.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="ddfd3-210">Adja meg a következő részleteket:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-210">Enter the following details:</span></span>

    1. <span data-ttu-id="ddfd3-211">**Http-trigger végpontja**: a korábbi lépésből másolt URL-cím</span><span class="sxs-lookup"><span data-stu-id="ddfd3-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="ddfd3-212">**Regisztrálni kívánt események**: "referral-created" és "referral-frissítve"</span><span class="sxs-lookup"><span data-stu-id="ddfd3-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="ddfd3-213">**Meglévő trigger-végpontok felülírása (ha van**): igen (Ez felülírja a meglévő végpontokat.)</span><span class="sxs-lookup"><span data-stu-id="ddfd3-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="ddfd3-214">Válassza a **Futtatás** lehetőséget, majd kattintson a **Kész gombra.**</span><span class="sxs-lookup"><span data-stu-id="ddfd3-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="ddfd3-215">A webhook mostantól figyelheti az események létrehozását és frissítését.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="ddfd3-216">Szinkronizálási lépések testreszabása</span><span class="sxs-lookup"><span data-stu-id="ddfd3-216">Customize synchronization steps</span></span>

<span data-ttu-id="ddfd3-217">Ha a partneri központ és a CRM-rendszer között szinkronizálja a közös értékesítésre való átirányítást, akkor a partner Center-számítógépen szinkronizált mezők itt vannak felsorolva.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="ddfd3-218">A CRM-rendszerek gyakran testre szabottak.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="ddfd3-219">Testreszabhatja a Power automatizáló folyamatokat.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="ddfd3-220">Kövesse a mező-hozzárendelési útmutatót, és szükség esetén végezze el a megfelelő módosításokat a Power automatizáló folyamatok lépéseiben.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="ddfd3-221">A Microsoft-partneri központok a CRM-alapú hozzárendelésekhez vannak megadva, de a CRM-környezet alapján a mezők további testreszabására is lehetősége van.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="ddfd3-222">Az egyes energiagazdálkodási folyamatok több lépését az igényeinek megfelelően testre szabhatja.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="ddfd3-223">A következő példák az elérhető testreszabásokat szemléltetik:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="ddfd3-224">A partner központ létrehozási vagy frissítési eseményeihez tartozó mezők testreszabása a CRM-hivatkozó szinkronizálásához:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="ddfd3-225">a.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-225">a.</span></span> <span data-ttu-id="ddfd3-226">Válassza a partneri központ lehetőséget a Dynamics 365 (belső előzetes verzió) vagy a Salesforce (belső előzetes verzió) elemre.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="ddfd3-227">b.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-227">b.</span></span> <span data-ttu-id="ddfd3-228">Válassza a **Szerkesztés** lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="ddfd3-229">c.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-229">c.</span></span> <span data-ttu-id="ddfd3-230">Válassza **a (hatókör) lehetőséget az érdeklődő vagy a lehetőség szinkronizálásához**.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="ddfd3-231">Ha testre szeretné szabni a CRM-mezők hozzárendeléseit (a mező-hozzárendelések útmutatója alapján) az események létrehozásához, válassza ki, hogy **új megosztott lehetőség van-e, majd**.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="ddfd3-232">Válassza ki az allépést, **Ha igen** , majd bontsa ki az **új lehetőség létrehozása lehetőséget a CRM-ben**.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="ddfd3-233">Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató segítségével módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="ddfd3-234">d.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-234">d.</span></span> <span data-ttu-id="ddfd3-235">Ha testre szeretné szabni a CRM-mezők hozzárendeléseit (a mező-hozzárendelések útmutatója alapján) a frissítési események esetében, kattintson a "(hatókör)" lehetőségre az érdeklődő vagy a lehetőség szinkronizálásához.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="ddfd3-236">e.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-236">e.</span></span> <span data-ttu-id="ddfd3-237">Válassza ki **, hogy a lehetőség frissítése lehetséges-** e.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="ddfd3-238">**Ha igen** , akkor válassza ki az allépést, majd bontsa ki **, ha a partner Centerben és a CRM-ben a lehetőség-objektumok között van különbség**</span><span class="sxs-lookup"><span data-stu-id="ddfd3-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="ddfd3-239">f.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-239">f.</span></span> <span data-ttu-id="ddfd3-240">Jelölje be az **Igen** , majd a **meglévő frissítése lehetőséget** .</span><span class="sxs-lookup"><span data-stu-id="ddfd3-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="ddfd3-241">A CRM és a számítógép közötti átirányítási szinkronizálás mezőinek testreszabása a frissítési eseményekhez:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="ddfd3-242">a.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-242">a.</span></span> <span data-ttu-id="ddfd3-243">Válassza a **Szerkesztés**  lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="ddfd3-244">b.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-244">b.</span></span> <span data-ttu-id="ddfd3-245">Válassza **a (hatókör) lehetőséget a lehetőség szinkronizálásához**.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="ddfd3-246">c.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-246">c.</span></span> <span data-ttu-id="ddfd3-247">A frissítési események CRM-mezőkhöz való hozzárendelésének testreszabásához válassza ki, hogy van-e **különbség a partner Centerben és a CRM-ben lévő érdeklődő objektumok között**.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="ddfd3-248">d.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-248">d.</span></span> <span data-ttu-id="ddfd3-249">Válassza ki az allépést, **Ha igen** , majd bontsa ki az **átirányítási lehetőséget a lehetőségre vonatkozó adattal**.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="ddfd3-250">Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató alapján módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="ddfd3-251">A CRM és a számítógép közötti átirányítási szinkronizálás mezőinek testreszabása az események létrehozásához?</span><span class="sxs-lookup"><span data-stu-id="ddfd3-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="ddfd3-252">a.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-252">a.</span></span> <span data-ttu-id="ddfd3-253">Válassza a **Szerkesztés**  lehetőséget az automatizálási folyamat szerkesztéséhez/testreszabásához.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="ddfd3-254">b.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-254">b.</span></span> <span data-ttu-id="ddfd3-255">Válassza ki **(hatókör) az átirányítások szinkronizálását.**</span><span class="sxs-lookup"><span data-stu-id="ddfd3-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="ddfd3-256">c.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-256">c.</span></span> <span data-ttu-id="ddfd3-257">Ha testre kívánja szabni a CRM-mezők hozzárendeléseit (a mező-hozzárendelések útmutatója alapján) az események létrehozásához, válassza a **Microsoft ajánló létrehozása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="ddfd3-258">Az ebben a szakaszban található leképezéseket a mező-hozzárendelési útmutató alapján módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="ddfd3-259">Két környezeti változó lett létrehozva:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-259">There are two environment variables created:</span></span>

- <span data-ttu-id="ddfd3-260">Pipa: azt jelzi, hogy a partner központ és a Dynamics 365 CRM között kétirányú szinkronizálású lehetőségek mellett van-e pipa ikon.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="ddfd3-261">Csak közös értékesítési lehetőségek szinkronizálása: azt jelenti, hogy csak a közös értékesítési lehetőségeket kívánja szinkronizálni.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="ddfd3-262">A környezeti változók alapértelmezett értékének szerkesztését is választhatja.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Alapértelmezett értékekhez tartozó mező szerkesztése":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="ddfd3-264">Végpontok közötti kétirányú, közös értékesítésre hivatkozó átirányítás szinkronizálása</span><span class="sxs-lookup"><span data-stu-id="ddfd3-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="ddfd3-265">Miután telepítette, konfigurálta és testreszabta az automatizálási megoldást, tesztelheti a Dynamics 365 és a partner Center közötti összekapcsolási átirányítások szinkronizálását.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="ddfd3-266">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="ddfd3-266">Pre-requisites</span></span>

<span data-ttu-id="ddfd3-267">Ha szinkronizálni szeretné a partner központ és a Dynamics 365 CRM közötti átirányításokat, az automatizálási megoldás egyértelműen kijelölte a Microsoft-specifikus átirányítási mezőket.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="ddfd3-268">Ez az azonosítás lehetővé teszi az értékesítő csapatának, hogy eldöntse, hogy mely ajánlásokat szeretné megosztani a Microsofttal a közös értékesítéshez.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="ddfd3-269">Az egyéni mezők készlete a **lehetőség** entitás részeként érhető el.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="ddfd3-270">Egy CRM-rendszergazda felhasználónak külön CRM-szakaszt kell létrehoznia a **lehetőség** egyéni mezőivel.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="ddfd3-271">A következő egyéni mezők a CRM szakasz részét képezik:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="ddfd3-272">**Szinkronizálás a partner centerrel**: a lehetőség szinkronizálása a Microsoft partner centerrel</span><span class="sxs-lookup"><span data-stu-id="ddfd3-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="ddfd3-273">**Hivatkozási azonosító**: a Microsoft partner Center ajánlójának írásvédett azonosító mezője</span><span class="sxs-lookup"><span data-stu-id="ddfd3-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="ddfd3-274">**Referral link**: egy csak olvasható hivatkozás a Microsoft partner Centerben</span><span class="sxs-lookup"><span data-stu-id="ddfd3-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="ddfd3-275">**Hogyan segíthet a Microsoft súgója?**: Segítség szükséges a Microsoftnak az átirányításhoz</span><span class="sxs-lookup"><span data-stu-id="ddfd3-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="ddfd3-276">**Termékek**: a lehetőséghez társított termékek listája</span><span class="sxs-lookup"><span data-stu-id="ddfd3-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="ddfd3-277">**Naplózás**: írásvédett naplózási nyomvonal a partner Center-hivatkozásokkal való szinkronizáláshoz</span><span class="sxs-lookup"><span data-stu-id="ddfd3-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="ddfd3-278">Frissítse a lehetőség űrlapját a Dynamics 365 CRM-ben a termékek mezőhöz tartozó megoldások befoglalásához.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Lehetőség űrlapja":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a><span data-ttu-id="ddfd3-281">FORGATÓKÖNYVEK</span><span class="sxs-lookup"><span data-stu-id="ddfd3-281">SCENARIOS:</span></span>

1. <span data-ttu-id="ddfd3-282">Átirányítás szinkronizálása a CRM-ben való létrehozáskor vagy frissítésekor, valamint a partner Centerben szinkronizálva:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="ddfd3-283">Jelentkezzen be a Dynamics 365 CRM-környezetbe azokkal a felhasználókkal, akik a CRM **lehetőség** szakaszában láthatók.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="ddfd3-284">Győződjön meg arról, hogy a Dynamics 365 környezetben a következő szakasz jelenik meg, amikor létrehoz egy új lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="A Microsoft partner Center információinak a Dynamics 365-ben való megjelenítését bemutató példa lehetőség szakasza.":::

   3. <span data-ttu-id="ddfd3-286">Ha ezt a lehetőséget a Microsoft partner centerrel szeretné szinkronizálni, ügyeljen arra, hogy a következő mezőket adja meg a kártya nézetben:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="ddfd3-287">**Szinkronizálás a partner centerrel**: igen</span><span class="sxs-lookup"><span data-stu-id="ddfd3-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="ddfd3-288">**Hogyan segíthet a Microsoft súgója?**: válasszon a következők közül:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="A Dynamics 365-es minta lehetőség szakasza, amely a Microsoft-partneri központ súgóját mutatja be a hogyan tud a Microsoft Help? nevű mező mellett.":::

      - <span data-ttu-id="ddfd3-290">**Termékek**: a termék megoldás-azonosítói</span><span class="sxs-lookup"><span data-stu-id="ddfd3-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="ddfd3-291">Miután létrejött a lehetőség a Dynamics 365-ben a **partner centerrel való szinkronizálással** beállítás **Igen** értékre van állítva, várjon 10 percet, majd jelentkezzen be a partner Center-fiókjába.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="ddfd3-292">Az átirányítási adatokat a Dynamics 365-mel szinkronizálja a rendszer.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="ddfd3-293">Hasonlóképpen, ha a Dynamics 365 CRM-ben a lehetőség frissítésével "igen" értékre állította a "szinkronizálás a partneri központtal" beállítást, a rendszer szinkronizálja a módosításokat a partner Center-fiókban.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="ddfd3-294">A partner centerrel sikeresen szinkronizált lehetőségek a Dynamics 365-as ✔ ikonnal lesznek azonosítva.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="ddfd3-295">Az átirányítás szinkronizálása a Microsoft partner Centerben, a Dynamics 365 környezetben szinkronizálva:</span><span class="sxs-lookup"><span data-stu-id="ddfd3-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="ddfd3-296">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/home).</span><span class="sxs-lookup"><span data-stu-id="ddfd3-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="ddfd3-297">A bal oldali menüben válassza a **hivatkozók** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="ddfd3-298">Hozzon létre egy új, közös értékesítésre hivatkozó hivatkozást a partner Centerben az "új üzlet" lehetőségre kattintva.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="ddfd3-299">Jelentkezzen be a Dynamics 365 CRM-környezetbe.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="ddfd3-300">Navigáljon a **lehetőségek megnyitásához**.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="ddfd3-301">A Microsoft partner Centerben létrehozott hivatkozás mostantól szinkronizálva van a Dynamics 365 CRM-ben.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="ddfd3-302">Amikor kijelöl egy szinkronizált átirányítást, a rendszer feltölti a kártya nézetének részleteit.</span><span class="sxs-lookup"><span data-stu-id="ddfd3-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ddfd3-303">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ddfd3-303">Next steps</span></span>

- [<span data-ttu-id="ddfd3-304">Érdeklődők kezelése</span><span class="sxs-lookup"><span data-stu-id="ddfd3-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="ddfd3-305">Együttes értékesítési lehetőségek kezelése</span><span class="sxs-lookup"><span data-stu-id="ddfd3-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="ddfd3-306">További információ a Microsoft Power automatizáló platformról?</span><span class="sxs-lookup"><span data-stu-id="ddfd3-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="ddfd3-307">A partneri központ webhookai</span><span class="sxs-lookup"><span data-stu-id="ddfd3-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)