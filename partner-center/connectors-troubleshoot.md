---
title: A közös értékesítéssel való átirányítási összekötők hibáinak megoldása
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Válaszok a közös értékesítési összekötők használatával kapcsolatos gyakori kérdésekre. Olvassa el ezt a gyakori kérdéseket a közös értékesítési összekötők hibáinak megoldásához.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b8977f7c602b8587a619236b37a760a55bf87e53
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354542"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="fe775-104">A közös értékesítéssel való átirányítási összekötők hibáinak megoldása</span><span class="sxs-lookup"><span data-stu-id="fe775-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="fe775-105">**A következőkre vonatkozik:**</span><span class="sxs-lookup"><span data-stu-id="fe775-105">**Applies to:**</span></span>

- <span data-ttu-id="fe775-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="fe775-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="fe775-107">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="fe775-107">Salesforce CRM</span></span>

<span data-ttu-id="fe775-108">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="fe775-108">**Appropriate roles**</span></span>

- <span data-ttu-id="fe775-109">Ajánlói rendszergazda</span><span class="sxs-lookup"><span data-stu-id="fe775-109">Referrals admin</span></span>
- <span data-ttu-id="fe775-110">Rendszerfelügyeleti webszolgáltatások vagy Rendszertestreszabó a CRM-ben</span><span class="sxs-lookup"><span data-stu-id="fe775-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="fe775-111">Az előfeltételekkel kapcsolatos kérdések és válaszok</span><span class="sxs-lookup"><span data-stu-id="fe775-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="fe775-112">Használhat-e a környezetéhez egy próbaverziós, közös értékesítéssel kapcsolatos átirányítási megoldást?</span><span class="sxs-lookup"><span data-stu-id="fe775-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="fe775-113">Ha a tesztelési/előkészítési környezetben van, választhatja a próbaverziós megoldást.</span><span class="sxs-lookup"><span data-stu-id="fe775-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="fe775-114">Az összekötők fizetett verziója a AppSource-on érhető el az USA-ban 15 USD/hó.</span><span class="sxs-lookup"><span data-stu-id="fe775-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="fe775-115">A fizetős kapcsolatok napi 10K API-hívásokat tesznek szükségessé.</span><span class="sxs-lookup"><span data-stu-id="fe775-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="fe775-116">Az összekötők a partner Center Referral API-k tetején található burkolók.</span><span class="sxs-lookup"><span data-stu-id="fe775-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="fe775-117">Ha az összekötői megoldások a partner központ vagy a CRM-oldal lehetőségein a **létrehozási** vagy **frissítési** eseményekhez futnak, egy API-hívás történik.</span><span class="sxs-lookup"><span data-stu-id="fe775-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="fe775-118">Milyen szerepkörrel kell szakaszt létrehozni a CRM-környezetben?</span><span class="sxs-lookup"><span data-stu-id="fe775-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="fe775-119">Azok a felhasználók, akik rendszergazdák vagy rendszertestreszabók, mindenki számára módosíthatják a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="fe775-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="fe775-120">Az alkalmazás összes felhasználója azonban személyre szabhatja a rendszerállapotot, és másokkal is megoszthatja a testreszabásokat.</span><span class="sxs-lookup"><span data-stu-id="fe775-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="fe775-121">A partner-értékesítőknek speciális szerepkörökre van szükségük a partner Centerben való munkához?</span><span class="sxs-lookup"><span data-stu-id="fe775-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="fe775-122">A partner-értékesítőknek hozzá kell rendelniük az "Ajánlói rendszergazda" szerepkört.</span><span class="sxs-lookup"><span data-stu-id="fe775-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="fe775-123">További információkért tekintse meg a következő [engedélyek áttekintését) (create-User-accounts-and-set-permissions).</span><span class="sxs-lookup"><span data-stu-id="fe775-123">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="fe775-124">Mely mezőket kell elsőként beállítani a CRM-környezetben?</span><span class="sxs-lookup"><span data-stu-id="fe775-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="fe775-125">• Győződjön meg arról, hogy a pénznem megfelelő a tartózkodási helyéhez, és pontosan a CRM-környezetben van.</span><span class="sxs-lookup"><span data-stu-id="fe775-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="fe775-126">• Az értékesítési csapatnak CRM-felhasználóként kell szerepelnie a CRM-környezetben.</span><span class="sxs-lookup"><span data-stu-id="fe775-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="fe775-127">Milyen előfeltételek szükségesek a Power automatizáló környezet létrehozásához?</span><span class="sxs-lookup"><span data-stu-id="fe775-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="fe775-128">A Power automatizáló környezet használatához a következők szükségesek:</span><span class="sxs-lookup"><span data-stu-id="fe775-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="fe775-129">A rendszer automatizálja a szükséges energiagazdálkodási licencet.</span><span class="sxs-lookup"><span data-stu-id="fe775-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="fe775-130">Legalább 1 GB-nyi tárterület szükséges.</span><span class="sxs-lookup"><span data-stu-id="fe775-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="fe775-131">Szüksége van egy Dynamics 365-előfizetésre az Salesforce-összekötők megoldás használatához?</span><span class="sxs-lookup"><span data-stu-id="fe775-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="fe775-132">Az Salesforce-összekötő megoldás "Dynamics flow" típusú, amely támogatja a más CRM-rendszerekkel való szinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="fe775-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="fe775-133">A megoldáshoz nem szükséges Dynamics 365-példány vagy-előfizetés.</span><span class="sxs-lookup"><span data-stu-id="fe775-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="fe775-134">A Salesforce-megoldás telepítésekor előfordulhat, hogy a vállalat meglévő CDS-környezetének legördülő lista jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="fe775-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="fe775-135">Ezt a környezetet kell kiválasztania.</span><span class="sxs-lookup"><span data-stu-id="fe775-135">You need to select that environment.</span></span> <span data-ttu-id="fe775-136">Továbbá, ha "nem találtunk a bejelentkezett felhasználóhoz csatlakozó Dynamics 365-szervezetet" hibaüzenet jelenik meg, akkor új környezetet kell létrehoznia az összekötőhöz.</span><span class="sxs-lookup"><span data-stu-id="fe775-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="fe775-137">A konfigurációval kapcsolatos kérdések és válaszok</span><span class="sxs-lookup"><span data-stu-id="fe775-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="fe775-138">Mi a teendő, ha az alábbi hibába ütközne a folyamatok aktiválása a Power automatizáló platformon?</span><span class="sxs-lookup"><span data-stu-id="fe775-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="fe775-139">Hiba: a Azure Resource Manager kérése sikertelen volt, hiba: {"Error": {"code": "WorkflowTriggerNotFound", "Message": "a (z)" e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 "trigger" Manual "utasítása nem található."}} ".</span><span class="sxs-lookup"><span data-stu-id="fe775-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="fe775-140">Kövesse az alábbi hibaelhárítási lépéseket:</span><span class="sxs-lookup"><span data-stu-id="fe775-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="fe775-141">Törölje a CDS-kapcsolatot, majd hozza létre újból a CDS-kapcsolatokat.</span><span class="sxs-lookup"><span data-stu-id="fe775-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="fe775-142">A gyermek kikapcsolásának és bekapcsolása</span><span class="sxs-lookup"><span data-stu-id="fe775-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="fe775-143">Törölje a megoldást, majd telepítse újra a megoldást.</span><span class="sxs-lookup"><span data-stu-id="fe775-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="fe775-144">Mi a teendő, ha a "Bejelentkezés" hibaüzenet jelenik meg egy partneri központ-összekötőnek a Power automatizáló platformban való hozzáadásakor?</span><span class="sxs-lookup"><span data-stu-id="fe775-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Bejelentkezést igénylő hibaüzenet":::

<span data-ttu-id="fe775-146">Kövesse ezt a hibaelhárítási lépést:</span><span class="sxs-lookup"><span data-stu-id="fe775-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="fe775-147">A partner Center hitelesítő adataival egyszeri bejelentkezést használhat a flow-környezetbe (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="fe775-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="fe775-148">Mi a teendő, ha a következő hibaüzenetet kapja, amikor aktiválja a partneri központot a CRM-folyamatba a Power automatizáló platformon?</span><span class="sxs-lookup"><span data-stu-id="fe775-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="A frissítéseket igénylő hibaüzenet":::

<span data-ttu-id="fe775-150">Kövesse az alábbi hibaelhárítási lépéseket:</span><span class="sxs-lookup"><span data-stu-id="fe775-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="fe775-151">Először aktiválja a következő két alárendelt folyamatot a partner központ CRM-folyamatba való aktiválása előtt.</span><span class="sxs-lookup"><span data-stu-id="fe775-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="fe775-152">Partneri központ és CRM – Helper (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="fe775-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="fe775-153">A partner Center Microsoft közös értékesítési hivatkozási frissítései a CRM-ben (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="fe775-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="fe775-154">Mi a teendő, ha nem tud kapcsolatokat hozzáadni a folyamathoz, amikor megkísérli a folyamat szerkesztését?</span><span class="sxs-lookup"><span data-stu-id="fe775-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="fe775-155">Ha a folyamat futása közben kapcsolatokat ad hozzá a folyamathoz, akkor az egyes folyamatokhoz való hozzáadása külön történik.</span><span class="sxs-lookup"><span data-stu-id="fe775-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="fe775-156">Ha a kapcsolatok hozzáadására szolgáló párbeszédpanel nem nyílik meg automatikusan a folyamat szerkesztése közben, akkor a folyamatok egyes lépéseit és allépéseit egyenként is szerkesztheti.</span><span class="sxs-lookup"><span data-stu-id="fe775-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="fe775-157">Válassza ki az egyes folyamatokat, és szerkessze azokat egyenként.</span><span class="sxs-lookup"><span data-stu-id="fe775-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="fe775-158">A folyamat összes lépésének kibontása</span><span class="sxs-lookup"><span data-stu-id="fe775-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="A kapcsolatokat igénylő lépések":::

- <span data-ttu-id="fe775-160">Válassza ki azokat a lépéseket, amelyekben a rendszer figyelmeztető ikont kér a kapcsolatok hozzárendelésére, valamint kapcsolatok hozzáadására.</span><span class="sxs-lookup"><span data-stu-id="fe775-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Folyamat szerkesztése lépésről lépésre":::


5. <span data-ttu-id="fe775-162">Mi a teendő, ha a közös értékesítésre hivatkozó összekötők megoldásának folyamatai nem kapcsolják be?</span><span class="sxs-lookup"><span data-stu-id="fe775-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="fe775-163">A.</span><span class="sxs-lookup"><span data-stu-id="fe775-163">A.</span></span> <span data-ttu-id="fe775-164">A Power Gyorsbüféban a folyamatokat a következő sorrendben kell szerkesztenie, és frissítenie kell őket a megfelelő kapcsolatok használatára:</span><span class="sxs-lookup"><span data-stu-id="fe775-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="fe775-165">A partner Center webhook-regisztrációja (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="fe775-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="fe775-166">Közös értékesítéssel való hivatkozás létrehozása – Salesforce (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="fe775-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="fe775-167">Partneri központ a Microsoft közös értékesítési hivatkozási frissítései a Salesforce-be (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="fe775-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="fe775-168">Partneri központ – Salesforce (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="fe775-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="fe775-169">Salesforce (Insider előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="fe775-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="fe775-170">Salesforce lehetőség a partneri központhoz (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="fe775-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="fe775-171">Salesforce Microsoft-megoldások a partner Centerhez (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="fe775-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="fe775-172">B.</span><span class="sxs-lookup"><span data-stu-id="fe775-172">B.</span></span> <span data-ttu-id="fe775-173">Mindegyik folyamat esetében válassza a **csak a felhasználók futtatása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fe775-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="fe775-174">Válassza a **kapcsolatok használata** lehetőséget a **csak futtatást használó felhasználó** számára.</span><span class="sxs-lookup"><span data-stu-id="fe775-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Folyamat aktiválása":::


<span data-ttu-id="fe775-176">C.</span><span class="sxs-lookup"><span data-stu-id="fe775-176">C.</span></span> <span data-ttu-id="fe775-177">Aktiválja az alábbi említett folyamatokat:</span><span class="sxs-lookup"><span data-stu-id="fe775-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="fe775-178">Partneri központ a Microsoft közös értékesítési hivatkozási frissítései a Salesforce-be (belső előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="fe775-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="fe775-179">Salesforce (Insider előzetes verzió)</span><span class="sxs-lookup"><span data-stu-id="fe775-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="fe775-180">D.</span><span class="sxs-lookup"><span data-stu-id="fe775-180">D.</span></span> <span data-ttu-id="fe775-181">Aktiválja az összes fennmaradó folyamatot.</span><span class="sxs-lookup"><span data-stu-id="fe775-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="fe775-182">E.</span><span class="sxs-lookup"><span data-stu-id="fe775-182">E.</span></span> <span data-ttu-id="fe775-183">A flow-partneri központ webhookjának regisztrációja lapon válassza a **Futtatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fe775-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="fe775-184">Adja meg a Salesforce folyamathoz a **partner Center** első műveletének **http URL-címét** .</span><span class="sxs-lookup"><span data-stu-id="fe775-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="fe775-185">Válassza a mind a négy lehetőséget a **regisztráláshoz** , majd válassza az **Igen** lehetőséget a felülíráshoz.</span><span class="sxs-lookup"><span data-stu-id="fe775-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="fe775-186">A futtatással/karbantartással kapcsolatos kérdések és válaszok</span><span class="sxs-lookup"><span data-stu-id="fe775-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="fe775-187">Hogyan történik a hibák elhárítása a Power automatizálási folyamat végrehajtása során?</span><span class="sxs-lookup"><span data-stu-id="fe775-187">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="fe775-188">Ha biztosítani szeretné, hogy a teljesítmény-automatizálási folyamatok a várt módon fussanak, és a hibák elhárítása a végrehajtás során történik, tekintse meg a [folyamatok hibáinak](/power-automate/fix-flow-failures)elhárítása</span><span class="sxs-lookup"><span data-stu-id="fe775-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="fe775-189">Mi a teendő, ha olyan hivatkozásokat lát, amelyek nincsenek megfelelően szinkronizálva a partner Centerben vagy a CRM-környezetben?</span><span class="sxs-lookup"><span data-stu-id="fe775-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="fe775-190">Az átirányítási szinkronizálás állapotának meghatározásához válassza a **naplózás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fe775-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Az átirányítások szinkronizálása":::

<span data-ttu-id="fe775-192">Győződjön meg arról, hogy teljesülnek a következő feltételek:</span><span class="sxs-lookup"><span data-stu-id="fe775-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="fe775-193">A megoldás azonosítója a lehetőség részeként van megadva.</span><span class="sxs-lookup"><span data-stu-id="fe775-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="fe775-194">Két betűs országkód szükséges.</span><span class="sxs-lookup"><span data-stu-id="fe775-194">Two letter country code is required.</span></span>

- <span data-ttu-id="fe775-195">Ha a Microsoft segítségére van kiválasztva a lehetőségre, az ügyfél kapcsolattartási adatai szükségesek.</span><span class="sxs-lookup"><span data-stu-id="fe775-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="fe775-196">Hogyan lehet meggyőződni arról, hogy az átirányítások kétirányú szinkronizálást végeznek?</span><span class="sxs-lookup"><span data-stu-id="fe775-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="fe775-197">Hajtsa végre a következő lépéseket:</span><span class="sxs-lookup"><span data-stu-id="fe775-197">Do the following steps:</span></span>

- <span data-ttu-id="fe775-198">A partner-értékesítőknek biztosítaniuk kell, hogy engedélyezve legyenek a **partner centerrel való szinkronizálás** a CRM szakaszban.</span><span class="sxs-lookup"><span data-stu-id="fe775-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Győződjön meg arról, hogy engedélyezte a szinkronizálást":::

- <span data-ttu-id="fe775-200">Az értékesítőknek meg kell adniuk a bevételt és a zárási dátumot, amikor minősítést vezetnek be.</span><span class="sxs-lookup"><span data-stu-id="fe775-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="fe775-201">Ha a CRM-azonosító a közös értékesítés **létrehozása** vagy **frissítése** szakaszban van megadva, de a CRM-ben nem található az azonosítóhoz vezető lehetőség, akkor a frissítés vagy a létrehozás figyelmen kívül lesz hagyva.</span><span class="sxs-lookup"><span data-stu-id="fe775-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="fe775-202">Győződjön meg arról, hogy az átirányítási pénznem mező a Salesforce-környezetben van konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="fe775-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="fe775-203">Mi a teendő, ha az összekötő leválasztja a kapcsolatot, és kihagy egy hivatkozó szinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="fe775-203">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="fe775-204">A következő lehetőségek közül néhányat kipróbálhat:</span><span class="sxs-lookup"><span data-stu-id="fe775-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="fe775-205">Győződjön meg arról, hogy lejárt-e a Felhasználónév vagy a jelszó a fiókpartner felhasználói számára hivatkozó rendszergazdai szerepkörökkel.</span><span class="sxs-lookup"><span data-stu-id="fe775-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="fe775-206">Megtekintheti a nem szinkronizált lehetőséget, elvégezheti a másodlagos frissítést, és megfigyelheti, hogy az átirányítás szinkronizálva van-e.</span><span class="sxs-lookup"><span data-stu-id="fe775-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="fe775-207">Ha a folyamatok futnak, és sikertelenek voltak, válassza ki a folyamatot, és küldje el újra a sikertelen futtatást.</span><span class="sxs-lookup"><span data-stu-id="fe775-207">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="fe775-208">Mi a teendő, ha hozzáférés-megtagadási hibát kap?</span><span class="sxs-lookup"><span data-stu-id="fe775-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="fe775-209">Győződjön meg arról, hogy a megfelelő szerepkörök léteznek</span><span class="sxs-lookup"><span data-stu-id="fe775-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="fe775-210">Hivatkozó rendszergazdai szerepkör a partner Center-értékesítőhöz</span><span class="sxs-lookup"><span data-stu-id="fe775-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="fe775-211">Rendszergazda vagy Rendszertestreszabó szerepkör a CRM-példányon</span><span class="sxs-lookup"><span data-stu-id="fe775-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="fe775-212">Győződjön meg arról, hogy a Power automatizáló folyamat fiókjának felhasználói bejelentkezik https://flow.microsoft.com legalább egyszer</span><span class="sxs-lookup"><span data-stu-id="fe775-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="fe775-213">Ha azt látja, hogy az **ügyfél-fiók kódja** hiányzik a közös értékesítés lehetősége létrehozásakor?</span><span class="sxs-lookup"><span data-stu-id="fe775-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="fe775-214">A CRM-ben hozzá kell adnia a kétbetűs ISO-országkódot a felhasználói fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="fe775-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="fe775-215">Mi a teendő, ha úgy látja, hogy a **megoldás-azonosító** a közös értékesítési lehetőség létrehozásakor szükséges?</span><span class="sxs-lookup"><span data-stu-id="fe775-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="fe775-216">A közös értékesítéssel való hivatkozás létrehozásához szükség van egy Microsoft közös értékesítésre kész megoldásra.</span><span class="sxs-lookup"><span data-stu-id="fe775-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="fe775-217">Mi a teendő, ha a partnervállalat olyan közös értékesítési lehetőségeit látja, amelyek nincsenek szinkronizálva a CRM-be, bár nincs folyamattal kapcsolatos hiba:</span><span class="sxs-lookup"><span data-stu-id="fe775-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="fe775-218">Tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="fe775-218">Do the following:</span></span>

- <span data-ttu-id="fe775-219">Miután létrehozott egy új, közös értékesítéssel foglalkozó megállapodást a partner Centerben, ellenőrizze, hogy meghívja-e a partneri központot a Dynamics 365 flow-ba (többször is meghívható).</span><span class="sxs-lookup"><span data-stu-id="fe775-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="fe775-220">Ha a folyamat meghívja a folyamatot, ellenőrizze az összes meghívott folyamatot, és azonosítsa a folyamat futtatását, amely frissíti a CRM-t.</span><span class="sxs-lookup"><span data-stu-id="fe775-220">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="fe775-221">Követheti a műveleteket, és ellenőrizheti, hogy frissítette-e a CRM-t, vagy hibát észlelt.</span><span class="sxs-lookup"><span data-stu-id="fe775-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="fe775-222">Ellenőrizze, hogy az *új Deal*\* a partner Centerben van-e kitöltve a CRM-azonosítóval.</span><span class="sxs-lookup"><span data-stu-id="fe775-222">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="fe775-223">Győződjön meg arról, hogy az üzlet nem lett véletlenül lezárva "megnyert" vagy "elveszett" néven a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="fe775-223">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fe775-224">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="fe775-224">Next steps</span></span>

- [<span data-ttu-id="fe775-225">Érdeklődők kezelése</span><span class="sxs-lookup"><span data-stu-id="fe775-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="fe775-226">Együttes értékesítési lehetőségek kezelése</span><span class="sxs-lookup"><span data-stu-id="fe775-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
