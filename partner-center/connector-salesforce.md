---
title: A Salesforce CRM-összekötő Partnerközpont
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Szinkronizálja a hivatkozásokat Partnerközpont Salesforce CRM-mel. Az értékesítők ezután együtt értékesíthet a Microsofttal az Ön CRM-rendszereiből.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148414"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="58e78-104">Salesforce CRM-hez készült közös értékesítési összekötő – áttekintés</span><span class="sxs-lookup"><span data-stu-id="58e78-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="58e78-105">**Megfelelő szerepkörök:** Ajánlói rendszergazdai | Rendszergazda vagy rendszer-testreszabó a CRM-ben</span><span class="sxs-lookup"><span data-stu-id="58e78-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="58e78-106">Partnerközpont összekötő lehetővé teszi az értékesítők számára, hogy az Ön CRM-rendszereiből együtt értékesítsen a Microsofttal.</span><span class="sxs-lookup"><span data-stu-id="58e78-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="58e78-107">Nem kell betanítanunk őket ahhoz, hogy az Partnerközpont az értékesítések kezeléséhez.</span><span class="sxs-lookup"><span data-stu-id="58e78-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="58e78-108">Az együttműködési összekötők használatával létrehozhat egy új közös értékesítésre vonatkozó ajánlást, amely egy Microsoft-értékesítőt vesz fel, használhatja a Microsoft-értékesítőtől származó terjesztéseket, elfogadhatja/elutasíthatja az ajánlati adatokat, például módosíthatja az üzlet értékét és a záródátumokat.</span><span class="sxs-lookup"><span data-stu-id="58e78-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="58e78-109">Emellett a Microsoft értékesítőitől is kaphat frissítéseket ezekről az együttműködési ügyletekről.</span><span class="sxs-lookup"><span data-stu-id="58e78-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="58e78-110">Az összes ajánlását a választott CRM-ben, és nem a saját Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="58e78-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="58e78-111">A megoldás a Microsoft Power Automate Solution-alapú, és Partnerközpont API-kat használ.</span><span class="sxs-lookup"><span data-stu-id="58e78-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="58e78-112">Telepítés előtt – előfeltételek</span><span class="sxs-lookup"><span data-stu-id="58e78-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="58e78-113">**Témakörök**</span><span class="sxs-lookup"><span data-stu-id="58e78-113">**Topics**</span></span>   |<span data-ttu-id="58e78-114">**Részletek**</span><span class="sxs-lookup"><span data-stu-id="58e78-114">**Details**</span></span>   |<span data-ttu-id="58e78-115">**Hivatkozások**</span><span class="sxs-lookup"><span data-stu-id="58e78-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="58e78-116">Microsoft Partner Network azonosítója</span><span class="sxs-lookup"><span data-stu-id="58e78-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="58e78-117">Érvényes MPN-azonosítóra van szüksége</span><span class="sxs-lookup"><span data-stu-id="58e78-117">You need a valid MPN ID</span></span>|<span data-ttu-id="58e78-118">Csatlakozás az [MPN-hez](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="58e78-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="58e78-119">Készen áll az értékesítésre</span><span class="sxs-lookup"><span data-stu-id="58e78-119">Co-sell ready</span></span>|<span data-ttu-id="58e78-120">Az IP-/szolgáltatási megoldásnak készen kell állnia az értékesítésre.</span><span class="sxs-lookup"><span data-stu-id="58e78-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="58e78-121">Értékesítés a Microsofttal</span><span class="sxs-lookup"><span data-stu-id="58e78-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="58e78-122">Partnerközpont-fiók</span><span class="sxs-lookup"><span data-stu-id="58e78-122">Partner Center account</span></span>|<span data-ttu-id="58e78-123">A Partnerközpont bérlőhöz társított MPN-azonosítónak meg kell egynie az együttműködési megoldáshoz társított MPN-azonosítóval.</span><span class="sxs-lookup"><span data-stu-id="58e78-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="58e78-124">Az összekötők üzembe helyezése előtt ellenőrizze, hogy látja-e az Partnerközpont-hez kapcsolódó hivatkozásokat.</span><span class="sxs-lookup"><span data-stu-id="58e78-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="58e78-125">Saját fiók kezelése</span><span class="sxs-lookup"><span data-stu-id="58e78-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="58e78-126">Partnerközpont felhasználói szerepkörök</span><span class="sxs-lookup"><span data-stu-id="58e78-126">Partner Center user roles</span></span>|<span data-ttu-id="58e78-127">Az összekötőket telepítő és azt felhasználó alkalmazottnak ajánlói rendszergazdának kell lennie</span><span class="sxs-lookup"><span data-stu-id="58e78-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="58e78-128">Felhasználói szerepkörök és engedélyek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="58e78-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="58e78-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="58e78-129">Salesforce CRM</span></span>|<span data-ttu-id="58e78-130">A CRM felhasználói szerepkör a rendszergazda vagy a rendszer testre szabója</span><span class="sxs-lookup"><span data-stu-id="58e78-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="58e78-131">Szerepkörök hozzárendelése a Salesforce CRM-ben</span><span class="sxs-lookup"><span data-stu-id="58e78-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="58e78-132">Power Automate Flow-fiók</span><span class="sxs-lookup"><span data-stu-id="58e78-132">Power Automate Flow Account</span></span>|<span data-ttu-id="58e78-133">Aktív fiók [Power Automate](https://flow.microsoft.com) CRM-rendszerrendszergazdának vagy rendszer-testreszabónak.</span><span class="sxs-lookup"><span data-stu-id="58e78-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="58e78-134">A felhasználónak legalább [Power Automate](https://flow.microsoft.com) be kell jelentkeznie az alkalmazásba.</span><span class="sxs-lookup"><span data-stu-id="58e78-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="58e78-135">A Salesforce-csomag telepítése a Microsoft Custom Fieldshez</span><span class="sxs-lookup"><span data-stu-id="58e78-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="58e78-136">A Partnerközpont és a Salesforce CRM Power Automate megoldásnak egyértelműen azonosítania kell a Microsoft-specifikus javaslatmezőket.</span><span class="sxs-lookup"><span data-stu-id="58e78-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="58e78-137">Ez a demarkáció lehetővé teszi a partner értékesítői csapatok számára, hogy eldöntsék, mely terjesztéseket szeretnék megosztani a Microsofttal az közös értékesítéshez.</span><span class="sxs-lookup"><span data-stu-id="58e78-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="58e78-138">A Salesforce-ban aktiválja a **Jegyzeteket,** és adja hozzá a lehetőségekhez kapcsolódó listához.</span><span class="sxs-lookup"><span data-stu-id="58e78-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="58e78-139">Referencia</span><span class="sxs-lookup"><span data-stu-id="58e78-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="58e78-140">A **lehetőségcsapatok aktiválásához** kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="58e78-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="58e78-141">A Telepítőben a **Gyors keresés mezőben** keresse meg a Lehetőségcsoport beállításait.</span><span class="sxs-lookup"><span data-stu-id="58e78-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="58e78-142">Szükség szerint adja meg a beállításokat.</span><span class="sxs-lookup"><span data-stu-id="58e78-142">Define the settings as needed.</span></span>
[<span data-ttu-id="58e78-143">Referencia</span><span class="sxs-lookup"><span data-stu-id="58e78-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="58e78-144">A Salesforce-ban telepítsen egyéni mezőket és objektumokat a [csomagtelepítővel.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)</span><span class="sxs-lookup"><span data-stu-id="58e78-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="58e78-145">Ezzel bármely vállalatnál telepítheti a csomagot.</span><span class="sxs-lookup"><span data-stu-id="58e78-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="58e78-146">Ha a telepítést egy védőfalba telepíti, az URL-cím kezdeti részét a következőre kell cserélnie: http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="58e78-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="58e78-147">A Salesforce-ban adja hozzá a Microsoft-megoldásokat a **Lehetőséggel** kapcsolatos listához.</span><span class="sxs-lookup"><span data-stu-id="58e78-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="58e78-148">A hozzáadás után válassza a **csavarkulcs ikont,** és frissítse a tulajdonságokat</span><span class="sxs-lookup"><span data-stu-id="58e78-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="58e78-149">Ajánlott eljárás: Tesztelés az élő adás előtt</span><span class="sxs-lookup"><span data-stu-id="58e78-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="58e78-150">Mielőtt telepíti, konfigurálja és testreszabja az Power Automate-megoldást az éles környezetben, mindenképpen tesztelje a megoldást egy átmeneti CRM-példányon.</span><span class="sxs-lookup"><span data-stu-id="58e78-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="58e78-151">Telepítse a Microsoft Power Automate megoldást egy átmeneti környezetbe/CRM-példányba.</span><span class="sxs-lookup"><span data-stu-id="58e78-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="58e78-152">Másolatot készítsen a megoldásról, futtassa a konfigurációt, Power Automate folyamat testreszabását az átmeneti környezetben.</span><span class="sxs-lookup"><span data-stu-id="58e78-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="58e78-153">Tesztelje a megoldást egy átmeneti/CRM-példányon.</span><span class="sxs-lookup"><span data-stu-id="58e78-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="58e78-154">Sikeresség után importálja felügyelt megoldásként az éles példányba.</span><span class="sxs-lookup"><span data-stu-id="58e78-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="58e78-155">A Partnerközpont szinkronizálásának telepítése a Salesforce CRM-hez</span><span class="sxs-lookup"><span data-stu-id="58e78-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="58e78-156">A jobb [felső Power Automate](https://flow.microsoft.com) válassza a **Környezetek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="58e78-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="58e78-157">Itt érhetők el az elérhető CRM-példányok.</span><span class="sxs-lookup"><span data-stu-id="58e78-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="58e78-158">Válassza ki a megfelelő CRM-példányt a jobb felső sarokban található legördülő menüből.</span><span class="sxs-lookup"><span data-stu-id="58e78-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="58e78-159">A **bal oldali** navigációs sávon válassza a Megoldások lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="58e78-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="58e78-160">Válassza a **felső menü Open AppSource (AppSource** megnyitása) hivatkozását.</span><span class="sxs-lookup"><span data-stu-id="58e78-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Az AppSource megnyitása":::

5. <span data-ttu-id="58e78-162">Az **előugró Partnerközpont keresse meg a Salesforce-hez** használható ajánlói összekötőket.</span><span class="sxs-lookup"><span data-stu-id="58e78-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="58e78-164">Kattintson a **Get it now (Lekért most) gombra,** majd a **Continue (Folytatás) gombra.**</span><span class="sxs-lookup"><span data-stu-id="58e78-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="58e78-165">Ez megnyitja az oldalt, ahol kiválaszthatja a Salesforce CRM-környezetet az alkalmazás telepítéséhez.</span><span class="sxs-lookup"><span data-stu-id="58e78-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="58e78-166">A használati feltételeket és feltételeket elfogadja.</span><span class="sxs-lookup"><span data-stu-id="58e78-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Elérhető CRM-ek":::

8. <span data-ttu-id="58e78-168">Ezután a Megoldás kezelése **lapra irányítja** át.</span><span class="sxs-lookup"><span data-stu-id="58e78-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="58e78-169">Navigáljon a "Partnerközpont" elemhez az oldal alján található nyílgombokkal.</span><span class="sxs-lookup"><span data-stu-id="58e78-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="58e78-170">**Az ütemezett telepítésnek** a javaslati megoldás Partnerközpont kell megjelennie.</span><span class="sxs-lookup"><span data-stu-id="58e78-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="58e78-171">A telepítés 10–15 percet fog igénybe venni.</span><span class="sxs-lookup"><span data-stu-id="58e78-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="58e78-172">A telepítés befejezése után lépjen vissza az Power Automate, [és](https://flow.microsoft.com) válassza a **Megoldások** lehetőséget a bal oldali navigációs területen.</span><span class="sxs-lookup"><span data-stu-id="58e78-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="58e78-173">Figyelje **Partnerközpont, hogy a Salesforce-hez való** hivatkozásszinkronizálás elérhető a Megoldások listában.</span><span class="sxs-lookup"><span data-stu-id="58e78-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="58e78-174">Válassza **Partnerközpont a Salesforce-hez való hivatkozásszinkronizálás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="58e78-175">A következő Power Automate folyamatok és entitások érhetők el:</span><span class="sxs-lookup"><span data-stu-id="58e78-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce-folyamatok":::



## <a name="configure-the-solution"></a><span data-ttu-id="58e78-177">A megoldás konfigurálása</span><span class="sxs-lookup"><span data-stu-id="58e78-177">Configure the solution</span></span>

1. <span data-ttu-id="58e78-178">Miután telepítette a megoldást a CRM-példányban, lépjen vissza a [Power Automate.](https://flow.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="58e78-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="58e78-179">A jobb **felső** sarokban található Környezetek legördülő menüből válassza ki azt a CRM-példányt, ahová a Power Automate telepítette.</span><span class="sxs-lookup"><span data-stu-id="58e78-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="58e78-180">A három felhasználói fiókot társító kapcsolatokat kell létrehoznia:</span><span class="sxs-lookup"><span data-stu-id="58e78-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="58e78-181">Partnerközpont rendszergazdai hitelesítő adatok megadása a felhasználónak</span><span class="sxs-lookup"><span data-stu-id="58e78-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="58e78-182">Partnerközpont – események</span><span class="sxs-lookup"><span data-stu-id="58e78-182">Partner Center Events</span></span>
    - <span data-ttu-id="58e78-183">CRM-rendszergazda a Power Automate folyamatokkal a megoldásban.</span><span class="sxs-lookup"><span data-stu-id="58e78-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="58e78-184">A **bal oldali** navigációs sávon válassza a Kapcsolatok lehetőséget, majd válassza a "Partnerközpont" megoldást a listából.</span><span class="sxs-lookup"><span data-stu-id="58e78-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="58e78-185">A Kapcsolat létrehozása gombra **kattintva hozzon létre egy kapcsolatot.**</span><span class="sxs-lookup"><span data-stu-id="58e78-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Kapcsolat létrehozása":::

- <span data-ttu-id="58e78-187">Keressen a Partnerközpont (előzetes verzió) kifejezésre a jobb felső sarokban található keresősávban.</span><span class="sxs-lookup"><span data-stu-id="58e78-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="58e78-188">Hozzon létre egy kapcsolatot a Partnerközpont a ajánlói rendszergazda hitelesítőadat-szerepkörében.</span><span class="sxs-lookup"><span data-stu-id="58e78-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="58e78-189">Ezután hozzon létre egy Partnerközpont Események kapcsolatot a Partnerközpont a ajánlói rendszergazda hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="58e78-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="58e78-190">Hozzon létre egy kapcsolatot a Salesforce számára a CRM-rendszergazdai felhasználó számára.</span><span class="sxs-lookup"><span data-stu-id="58e78-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="58e78-191">Miután hozzáadta az összes kapcsolatot, a következő kapcsolatoknak kell látszani a környezetében:</span><span class="sxs-lookup"><span data-stu-id="58e78-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Kapcsolatok megfigyelése":::

### <a name="edit-the-connections"></a><span data-ttu-id="58e78-193">A kapcsolatok szerkesztése</span><span class="sxs-lookup"><span data-stu-id="58e78-193">Edit the connections</span></span>

1. <span data-ttu-id="58e78-194">Térjen vissza a Megoldások lapra, és válassza az **Alapértelmezett megoldás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="58e78-195">A Minden elemre kattintva válassza a Kapcsolati **referencia (előzetes verzió)** **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Összekötő szerkesztésének megkezdése":::

2. <span data-ttu-id="58e78-197">Szerkessze egyenként a kapcsolatokat a három pont ikon kiválasztásával.</span><span class="sxs-lookup"><span data-stu-id="58e78-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="58e78-198">Adja hozzá a megfelelő kapcsolatokat.</span><span class="sxs-lookup"><span data-stu-id="58e78-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Összekötők szerkesztése":::

3. <span data-ttu-id="58e78-200">Kapcsolja be a folyamatokat a következő sorrendben:</span><span class="sxs-lookup"><span data-stu-id="58e78-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="58e78-201">Partnerközpont regisztrációja (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="58e78-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="58e78-202">Közös értékesítési ajánlás létrehozása – Salesforce Partnerközpont (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="58e78-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="58e78-203">Partnerközpont Microsoft Co-sell Referral Updates to Salesforce (Insider Preview) (Microsoft Co-sell referral Updates to Salesforce (Insider Preview) (A Salesforce (Belső előzetes verzió) frissítései)</span><span class="sxs-lookup"><span data-stu-id="58e78-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="58e78-204">Partnerközpont Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="58e78-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="58e78-205">A Salesforce Partnerközpont (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="58e78-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="58e78-206">Salesforce Opportunity to Partnerközpont (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="58e78-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="58e78-207">A Salesforce Microsoft Solutions Partnerközpont (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="58e78-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="58e78-208">Webhook API-k használata erőforrás-módosítási eseményekre való regisztrációhoz</span><span class="sxs-lookup"><span data-stu-id="58e78-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="58e78-209">A Partnerközpont Webhook API-k lehetővé teszik, hogy regisztráljon az erőforrás-módosítási eseményekre.</span><span class="sxs-lookup"><span data-stu-id="58e78-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="58e78-210">Ezeket a módosítási eseményeket a rendszer HTTP-bejegyzésekként küldi el az URL-címére.</span><span class="sxs-lookup"><span data-stu-id="58e78-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="58e78-211">Az URL-cím regisztráláshoz válassza Partnerközpont **webhookregisztráció (Insider Preview)** lehetőséget a Power Automate folyamathoz.</span><span class="sxs-lookup"><span data-stu-id="58e78-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="58e78-212">Adjon hozzá kapcsolatokat (a.) Partnerközpont felhasználóhoz a hivatkozások rendszergazdai hitelesítő adataival (b.) Partnerközpont eseményekhez az alább kiemelt módon</span><span class="sxs-lookup"><span data-stu-id="58e78-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Eseményindító":::

3. <span data-ttu-id="58e78-214">A frissítések során a következőt fogja látni:</span><span class="sxs-lookup"><span data-stu-id="58e78-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhookok":::

4. <span data-ttu-id="58e78-216">Mentse a módosításokat, és válassza **a Bekapcsolás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="58e78-217">Ha engedélyezni Partnerközpont, hogy a webhookok figyeljék az események változásait, hajtsa végre a következő lépéseket:</span><span class="sxs-lookup"><span data-stu-id="58e78-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="58e78-218">Válassza **Partnerközpont Salesforce CRM (Insider Preview)** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="58e78-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="58e78-219">Válassza a **Szerkesztés ikont,** majd **a HTTP-kérések esetén lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="58e78-220">Kattintson a **Másolás ikonra** a megadott HTTP POST URL-cím másoláshoz.</span><span class="sxs-lookup"><span data-stu-id="58e78-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL-cím másolása":::

8. <span data-ttu-id="58e78-222">Válassza ki a "Partnerközpont Regisztráció (Insider Preview)" folyamatot, Power Automate futtatás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="58e78-223">Győződjön meg arról, hogy a jobb oldali panelen megnyílik a "Folyamat futtatása" ablak, és válassza a **Folytatás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="58e78-224">Adja meg a következő részleteket:</span><span class="sxs-lookup"><span data-stu-id="58e78-224">Enter the following details:</span></span>

    1. <span data-ttu-id="58e78-225">**HTTP-eseményindító végpontja:** Az URL-cím kimásolható a korábbi lépésből</span><span class="sxs-lookup"><span data-stu-id="58e78-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="58e78-226">**Regisztrálni szükséges események:**"referral-created" és "referral-updated"</span><span class="sxs-lookup"><span data-stu-id="58e78-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="58e78-227">**Meglévő triggervégpont felülírása, ha van:** Igen (Ez felülírja a meglévő végpontokat.)</span><span class="sxs-lookup"><span data-stu-id="58e78-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="58e78-228">Válassza a **Futtatás,** majd a Kész **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="58e78-229">A webhook most már képes figyelni az események létrehozására és frissítésére.</span><span class="sxs-lookup"><span data-stu-id="58e78-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="58e78-230">Szinkronizálási lépések testreszabása</span><span class="sxs-lookup"><span data-stu-id="58e78-230">Customize synchronization steps</span></span>

<span data-ttu-id="58e78-231">Ha az értékesítésre vonatkozó hivatkozásokat a Partnerközpont és a CRM-rendszer szinkronizálja, itt megjelenik az Partnerközpont számítógépen szinkronizált mezők listája.</span><span class="sxs-lookup"><span data-stu-id="58e78-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="58e78-232">A CRM-rendszerek gyakran nagymértékben testre vannak szabva.</span><span class="sxs-lookup"><span data-stu-id="58e78-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="58e78-233">A folyamatokat testre Power Automate testreszabhatja.</span><span class="sxs-lookup"><span data-stu-id="58e78-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="58e78-234">Kövesse a mezőleképezési útmutatót, és szükség esetén hajtsa végre a megfelelő módosításokat a Power Automate lépésekben.</span><span class="sxs-lookup"><span data-stu-id="58e78-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="58e78-235">A Microsoft Partnerközpontok és CRM-leképezések is rendelkezésre állnak, de az Ön CRM-környezete alapján további testreszabási beállításokat is választhat a mezőkhöz.</span><span class="sxs-lookup"><span data-stu-id="58e78-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="58e78-236">Az egyes folyamatfolyamatok Power Automate az igényeinek megfelelően testre szabhatók.</span><span class="sxs-lookup"><span data-stu-id="58e78-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="58e78-237">Az alábbiakban példákat talál az elérhető testreszabási lehetőségekre:</span><span class="sxs-lookup"><span data-stu-id="58e78-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="58e78-238">A létrehozási vagy frissítési események mezőinek testreszabása a Partnerközpont CRM-hivatkozásszinkronizáláshoz:</span><span class="sxs-lookup"><span data-stu-id="58e78-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="58e78-239">Válassza Partnerközpont Salesforce CRM (Insider Preview) lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="58e78-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="58e78-240">Válassza **a Szerkesztés** lehetőséget a folyamat szerkesztéséhez Power Automate testreszabásához.</span><span class="sxs-lookup"><span data-stu-id="58e78-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="58e78-241">Válassza **a (Hatókör) Érdeklődő vagy lehetőség szinkronizálása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="58e78-242">A CRM-mezőleképezések létrehozási eseményekhez való testreszabásához válassza az Új Megosztott lehetőség **lehetőséget, majd a lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="58e78-243">Ha igen,  válassza az allépést, majd bontsa ki **az Új lehetőség létrehozása a CRM-ben lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="58e78-244">Az ebben a szakaszban található leképezéseket a Mezőleképezés útmutatója segítségével szerkesztheti.</span><span class="sxs-lookup"><span data-stu-id="58e78-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="58e78-245">A CRM-mezőleképezések frissítési eseményekhez való testreszabásához válassza a "(Hatókör) Az érdeklődő vagy lehetőség szinkronizálása" lépést.</span><span class="sxs-lookup"><span data-stu-id="58e78-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="58e78-246">Válassza az If it's update to an opportunity (Lehetőség **frissítése) lehetőséget, majd a lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="58e78-247">Ha igen,  jelölje ki az allépést, majd bontsa ki a Lehetőségobjektumok közötti különbség az ügyfélben és **a CRM Partnerközpont, majd a et.**</span><span class="sxs-lookup"><span data-stu-id="58e78-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="58e78-248">Válassza a **Ha igen,** majd a **Meglévő lehetőség frissítése lehetőséget**</span><span class="sxs-lookup"><span data-stu-id="58e78-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="58e78-249">A CRM-számítógépekre történő hivatkozásszinkronizálás mezőinek testreszabása a frissítési eseményekhez:</span><span class="sxs-lookup"><span data-stu-id="58e78-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="58e78-250">Válassza **a Szerkesztés**  lehetőséget a folyamat szerkesztéséhez Power Automate testreszabásához.</span><span class="sxs-lookup"><span data-stu-id="58e78-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="58e78-251">Válassza **a (Hatókör) Lehetőség szinkronizálása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="58e78-252">A frissítési események CRM-mezőleképezésének (mezőleképezési útmutató alapján) való testreszabásához válassza a Ha van különbség a crm és a Partnerközpont érdeklődőobjektumai között, akkor **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="58e78-253">Ha igen,  válassza az allépést, majd bontsa ki **a Hivatkozás frissítése lehetőségadatokkal lépést.**</span><span class="sxs-lookup"><span data-stu-id="58e78-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="58e78-254">Az ebben a szakaszban található leképezéseket a Mezőleképezési útmutató alapján szerkesztheti.</span><span class="sxs-lookup"><span data-stu-id="58e78-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="58e78-255">A CRM-számítógépekre történő hivatkozásszinkronizálás mezőinek testreszabása az események létrehozásához?</span><span class="sxs-lookup"><span data-stu-id="58e78-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="58e78-256">Válassza **a Szerkesztés**  lehetőséget a folyamat szerkesztéséhez Power Automate testreszabásához.</span><span class="sxs-lookup"><span data-stu-id="58e78-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="58e78-257">Válassza **a (Hatókör) Javaslatszinkronizálás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="58e78-258">A CRM-mezőleképezések (mezőleképezések útmutatója alapján) események létrehozásához való testreszabásához válassza a **Microsoft-ajánlás létrehozása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58e78-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="58e78-259">Az ebben a szakaszban található leképezéseket a Mezőleképezési útmutató alapján szerkesztheti.</span><span class="sxs-lookup"><span data-stu-id="58e78-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="58e78-260">Kétirányú kétirányú kétirányú hivatkozásszinkronizálás</span><span class="sxs-lookup"><span data-stu-id="58e78-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="58e78-261">Miután telepítette, konfigurálta és testre szabta a Power Automate megoldást, tesztelheti a Salesforce CRM és a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="58e78-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="58e78-262">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="58e78-262">Pre-requisites</span></span>

<span data-ttu-id="58e78-263">A microsoftos és Partnerközpont Salesforce CRM közötti szinkronizáláshoz a Power Automate megoldásnak egyértelműen el kell különítenének Microsoft-specifikus javaslati mezőket.</span><span class="sxs-lookup"><span data-stu-id="58e78-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="58e78-264">Ez az azonosítás lehetővé teszi az értékesítő csapatok számára, hogy eldöntsék, mely terjesztéseket szeretnék megosztani a Microsofttal közös értékesítés céljából.</span><span class="sxs-lookup"><span data-stu-id="58e78-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="58e78-265">Egyéni mezők egy készlete érhető el a Partnerközpont a Salesforce CRM megoldás lehetőség **entitásának** részeként.</span><span class="sxs-lookup"><span data-stu-id="58e78-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="58e78-266">A CRM rendszergazdának létre kell hoznia egy külön CRM-szakaszt a **Lehetőség egyéni mezőkkel.**</span><span class="sxs-lookup"><span data-stu-id="58e78-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="58e78-267">Az alábbi egyéni mezőknek a CRM szakasz részeinek kell lennie:</span><span class="sxs-lookup"><span data-stu-id="58e78-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="58e78-268">**Szinkronizálás Partnerközpont:** A lehetőség szinkronizálása a Microsoft Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="58e78-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="58e78-269">**Hivatkozásazonosító:** Egy csak olvasható azonosító mező a Microsoft Partnerközpont számára</span><span class="sxs-lookup"><span data-stu-id="58e78-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="58e78-270">**Hivatkozás:** A Microsoft Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="58e78-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="58e78-271">**Hogyan segíthet a Microsoft:** A Microsofttól a hivatkozáshoz szükséges segítség</span><span class="sxs-lookup"><span data-stu-id="58e78-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="58e78-272">**Termékek:** A lehetőséghez társított termékek listája</span><span class="sxs-lookup"><span data-stu-id="58e78-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="58e78-273">**Naplózás:** Csak olvasható auditálási napló a Partnerközpont való szinkronizáláshoz</span><span class="sxs-lookup"><span data-stu-id="58e78-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="58e78-274">Forgatókönyvek:</span><span class="sxs-lookup"><span data-stu-id="58e78-274">SCENARIOS:</span></span>

1. <span data-ttu-id="58e78-275">Hivatkozásszinkronizálás a CRM-ben történő hivatkozás létrehozásakor vagy frissítésekor, majd az Partnerközpont:</span><span class="sxs-lookup"><span data-stu-id="58e78-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="58e78-276">Jelentkezzen be a Salesforce CRM-környezetbe a CRM **Lehetőség** szakaszában látható felhasználóval.</span><span class="sxs-lookup"><span data-stu-id="58e78-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="58e78-277">Ellenőrizze, hogy a következő szakasz jelen van-e az "Új lehetőség" Salesforce CRM-környezetben való létrehozásakor</span><span class="sxs-lookup"><span data-stu-id="58e78-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-környezet":::

   3. <span data-ttu-id="58e78-279">Ha szinkronizálni szeretné ezt a lehetőséget a Microsoft Partnerközpont, állítsa be a következő mezőket a kártyanézetben:</span><span class="sxs-lookup"><span data-stu-id="58e78-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="58e78-280">"Szinkronizálás a Partnerközpont": Igen</span><span class="sxs-lookup"><span data-stu-id="58e78-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="58e78-281">"Hogyan segíthet a Microsoft?": Válasszon az alábbi lehetőségek közül:</span><span class="sxs-lookup"><span data-stu-id="58e78-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="58e78-282">Termékek: A termék megoldás-számai</span><span class="sxs-lookup"><span data-stu-id="58e78-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="58e78-283">Miután beállította a Szinkronizálás a következővel  **lehetőséget Partnerközpont** **igen,** várjon 10 percet, jelentkezzen be a Partnerközpont fiókjába.</span><span class="sxs-lookup"><span data-stu-id="58e78-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="58e78-284">A rendszer szinkronizálja a hivatkozásokat a Salesforce CRM-mel.</span><span class="sxs-lookup"><span data-stu-id="58e78-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="58e78-285">Ha a "Szinkronizálás Partnerközpont" beállítás "Igen" van beállítva, akkor ha frissíti a lehetőséget a Salesforce CRM-ben, a módosítások szinkronizálva lesznek az Partnerközpont fiókkal.</span><span class="sxs-lookup"><span data-stu-id="58e78-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="58e78-286">A Salesforce CRM-ben a Partnerközpont sikeresen szinkronizált lehetőségeket a ✔ azonosítja.</span><span class="sxs-lookup"><span data-stu-id="58e78-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="58e78-287">Hivatkozásszinkronizálás a Microsoft-ügyfélben létrehozott vagy frissített hivatkozások Partnerközpont Salesforce CRM-környezetben való szinkronizálása esetén:</span><span class="sxs-lookup"><span data-stu-id="58e78-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="58e78-288">Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="58e78-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="58e78-289">A **bal oldali menüben** válassza a Hivatkozások lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="58e78-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="58e78-290">Hozzon létre egy új közös értékesítésre vonatkozó ajánlást a Partnerközpont "Új üzlet" lehetőségre kattintva.</span><span class="sxs-lookup"><span data-stu-id="58e78-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="58e78-291">Jelentkezzen be a Salesforce CRM-környezetbe.</span><span class="sxs-lookup"><span data-stu-id="58e78-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="58e78-292">Lépjen a **Megnyitási lehetőségek lapra.**</span><span class="sxs-lookup"><span data-stu-id="58e78-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="58e78-293">A Microsoft Partnerközpont létrehozott hivatkozás most már szinkronizálva van a Salesforce CRM-ben.</span><span class="sxs-lookup"><span data-stu-id="58e78-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="A Salesforce lehetőség képernyője":::

    6. <span data-ttu-id="58e78-295">Szinkronizált hivatkozás kiválasztásakor a kártyanézet részletei ki lesznek töltve.</span><span class="sxs-lookup"><span data-stu-id="58e78-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="58e78-296">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="58e78-296">Next steps</span></span>

- [<span data-ttu-id="58e78-297">Érdeklődők kezelése</span><span class="sxs-lookup"><span data-stu-id="58e78-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="58e78-298">Együttes értékesítési lehetőségek kezelése</span><span class="sxs-lookup"><span data-stu-id="58e78-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="58e78-299">Partnerközpont – webhookok</span><span class="sxs-lookup"><span data-stu-id="58e78-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
