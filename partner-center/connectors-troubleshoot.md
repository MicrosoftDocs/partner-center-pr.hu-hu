---
title: Az közös értékesítésre vonatkozó ajánló összekötők hibaelhárítása
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg az együttműködési összekötők használatával kapcsolatos gyakori kérdésekre adott válaszokat. Olvassa el ezt a gyakori kérdéseket az együttműködési összekötők hibaelhárításáról.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 939654202a370f6d9ba15d9e62a11be44884b613
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284213"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="17ce5-104">Az közös értékesítésre vonatkozó ajánló összekötők hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="17ce5-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="17ce5-105">**A következőre érvényes:**</span><span class="sxs-lookup"><span data-stu-id="17ce5-105">**Applies to**</span></span>

- <span data-ttu-id="17ce5-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="17ce5-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="17ce5-107">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="17ce5-107">Salesforce CRM</span></span>

<span data-ttu-id="17ce5-108">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="17ce5-108">**Appropriate roles**</span></span>

- <span data-ttu-id="17ce5-109">Ajánlói rendszergazda</span><span class="sxs-lookup"><span data-stu-id="17ce5-109">Referrals admin</span></span>
- <span data-ttu-id="17ce5-110">Rendszergazda vagy rendszer testreszabó a CRM-ben</span><span class="sxs-lookup"><span data-stu-id="17ce5-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="17ce5-111">Előfeltételekre és válaszokra adott kérdések és válaszok</span><span class="sxs-lookup"><span data-stu-id="17ce5-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="17ce5-112">Használhat az Ön környezetében próbaverziós, közös értékesítésre vonatkozó javaslati összekötő megoldást?</span><span class="sxs-lookup"><span data-stu-id="17ce5-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="17ce5-113">Ha a tesztelési/előkészítési környezetben van, választhatja a próbaverziós megoldást.</span><span class="sxs-lookup"><span data-stu-id="17ce5-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="17ce5-114">Az összekötők fizetős verziója havonta 15 USD összegben érhető el az AppSource-ban.</span><span class="sxs-lookup"><span data-stu-id="17ce5-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="17ce5-115">A fizetős kapcsolattal naponta 10 000 API-hívást kap.</span><span class="sxs-lookup"><span data-stu-id="17ce5-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="17ce5-116">Az összekötők a hivatkozási API-k Partnerközpont burkolók.</span><span class="sxs-lookup"><span data-stu-id="17ce5-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="17ce5-117">Amikor az összekötő-megoldások létrehozási vagy frissítési eseményen futnak **a** Partnerközpont vagy a CRM oldalán található lehetőségeken, a rendszer API-hívást hoz létre. </span><span class="sxs-lookup"><span data-stu-id="17ce5-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="17ce5-118">Milyen szerepkörre van szüksége szakaszok létrehozásához a CRM-környezetben?</span><span class="sxs-lookup"><span data-stu-id="17ce5-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="17ce5-119">Azok a felhasználók, akik rendszergazdai vagy rendszer-testreszabók, mindenkire alkalmazhatják a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="17ce5-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="17ce5-120">Az alkalmazás minden felhasználója azonban személyre szabhatja a rendszert, és akár a testreszabások egy részét megoszthatja másokkal.</span><span class="sxs-lookup"><span data-stu-id="17ce5-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="17ce5-121">A partner értékesítőknek speciális szerepkörökre van szükségük a Partnerközpont?</span><span class="sxs-lookup"><span data-stu-id="17ce5-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="17ce5-122">A partner értékesítőknek a "Ajánlói rendszergazda" szerepkört kell hozzárendelni.</span><span class="sxs-lookup"><span data-stu-id="17ce5-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="17ce5-123">További információ: [Engedélyek áttekintése.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="17ce5-123">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="17ce5-124">Milyen mezőket kell először beállítani a CRM-környezetben?</span><span class="sxs-lookup"><span data-stu-id="17ce5-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="17ce5-125">• Győződjön meg arról, hogy a pénzneme megfelelő az Ön tartózkodási helyének, és hogy pontosan a CRM-környezetben van.</span><span class="sxs-lookup"><span data-stu-id="17ce5-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="17ce5-126">• Az értékesítési csapatnak CRM-felhasználóként kell szerepelve lennie a CRM-környezetben.</span><span class="sxs-lookup"><span data-stu-id="17ce5-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="17ce5-127">Milyen előfeltételek szükségesek a Power Automate létrehozásához?</span><span class="sxs-lookup"><span data-stu-id="17ce5-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="17ce5-128">A Power Automate a következőre lesz szüksége:</span><span class="sxs-lookup"><span data-stu-id="17ce5-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="17ce5-129">Egy Power Automate licenc szükséges.</span><span class="sxs-lookup"><span data-stu-id="17ce5-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="17ce5-130">Legalább 1 GB tárhely szükséges.</span><span class="sxs-lookup"><span data-stu-id="17ce5-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="17ce5-131">Dynamics 365-előfizetésre van szüksége a Salesforce-összekötők megoldásához?</span><span class="sxs-lookup"><span data-stu-id="17ce5-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="17ce5-132">A Salesforce Connector megoldás típusa "Dynamics Flow", amely támogatja a más CRM-rendszerekkel való szinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="17ce5-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="17ce5-133">A megoldáshoz nem szükséges Dynamics 365-példány vagy -előfizetés.</span><span class="sxs-lookup"><span data-stu-id="17ce5-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="17ce5-134">A Salesforce-megoldás telepítésekor megjelenik egy legördülő lista a vállalat meglévő CDS-környezetéről.</span><span class="sxs-lookup"><span data-stu-id="17ce5-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="17ce5-135">Ki kell választania ezt a környezetet.</span><span class="sxs-lookup"><span data-stu-id="17ce5-135">You need to select that environment.</span></span> <span data-ttu-id="17ce5-136">Emellett ha a "Nem található bejelentkezett felhasználóhoz csatlakoztatott Dynamics 365-szervezet" hibaüzenet jelenik meg, akkor új környezetet kell létrehoznia az összekötőhöz.</span><span class="sxs-lookup"><span data-stu-id="17ce5-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="17ce5-137">Konfigurációval kapcsolatos kérdések és válaszok</span><span class="sxs-lookup"><span data-stu-id="17ce5-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="17ce5-138">Mit kell tenni, ha a következő hibaüzenet jelenik meg a folyamatok aktiválása során az Power Automate Platformon?</span><span class="sxs-lookup"><span data-stu-id="17ce5-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="17ce5-139">Hiba: A(z) Azure Resource Manager kérése a következő hibával meghiúsult: {"error":{"code":"WorkflowTriggerNotFound","message":"Az "e14d00f1-1fdf-4b1b-aaac-54a5064093d3" eseményindító "manuális" eseményindítója nem található."}}".</span><span class="sxs-lookup"><span data-stu-id="17ce5-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="17ce5-140">Kövesse az alábbi hibaelhárítási lépéseket:</span><span class="sxs-lookup"><span data-stu-id="17ce5-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="17ce5-141">Törölje a CDS-kapcsolatot, majd hozza létre újra a CDS-kapcsolatokat.</span><span class="sxs-lookup"><span data-stu-id="17ce5-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="17ce5-142">A gyermekfolyam ki- és bekapcsolás</span><span class="sxs-lookup"><span data-stu-id="17ce5-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="17ce5-143">Törölje a megoldást, majd telepítse újra a megoldást.</span><span class="sxs-lookup"><span data-stu-id="17ce5-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="17ce5-144">Mit kell tenni, ha a "Bejelentkezés" hibával szembesül, amikor hozzáad egy Partnerközpont-összekötőt a Power Automate Platformhoz?</span><span class="sxs-lookup"><span data-stu-id="17ce5-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Bejelentkezést igénylő hibaüzenet":::

<span data-ttu-id="17ce5-146">Kövesse az alábbi hibaelhárítási lépést:</span><span class="sxs-lookup"><span data-stu-id="17ce5-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="17ce5-147">A Partnerközpont hitelesítő adataival jelentkezzen be egyszer a folyamatkörnyezetbe (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="17ce5-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="17ce5-148">Mit kell tenni, ha a következő hibaüzenetet kapja a CRM Partnerközpont-folyamat aktiválása közben a Power Automate Platformon?</span><span class="sxs-lookup"><span data-stu-id="17ce5-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Frissítést igénylő hibaüzenet":::

<span data-ttu-id="17ce5-150">Kövesse az alábbi hibaelhárítási lépéseket:</span><span class="sxs-lookup"><span data-stu-id="17ce5-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="17ce5-151">Először aktiválja a következő két gyermekfolyamatot, mielőtt aktiválja Partnerközpont CRM-folyamathoz.</span><span class="sxs-lookup"><span data-stu-id="17ce5-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="17ce5-152">Partnerközpont CRM – Segítő (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="17ce5-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="17ce5-153">Partnerközpont Crm (Insider Preview) microsoftos közös értékesítésre vonatkozó hivatkozási frissítései</span><span class="sxs-lookup"><span data-stu-id="17ce5-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="17ce5-154">Mit kell tenni, ha nem tud kapcsolatokat hozzáadni a folyamathoz, amikor megpróbálja szerkeszteni a folyamatot?</span><span class="sxs-lookup"><span data-stu-id="17ce5-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="17ce5-155">Amíg a folyamat fut, kapcsolatokat adhat hozzá a folyamathoz, és minden folyamatot külön-külön adhat hozzá.</span><span class="sxs-lookup"><span data-stu-id="17ce5-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="17ce5-156">Ha a kapcsolatok hozzáadására szolgáló párbeszédpanel nem nyílik meg automatikusan a folyamat szerkesztése közben, akkor külön-külön szerkesztheti a folyamatok egyes lépéseit és al lépéseit.</span><span class="sxs-lookup"><span data-stu-id="17ce5-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="17ce5-157">Jelölje ki az egyes folyamatokat, és szerkessze őket egyenként.</span><span class="sxs-lookup"><span data-stu-id="17ce5-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="17ce5-158">A folyamat összes lépésének kibontása</span><span class="sxs-lookup"><span data-stu-id="17ce5-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Kapcsolatokra van szükség":::

- <span data-ttu-id="17ce5-160">Válassza ki azokat a lépéseket, ahol megjelenik egy figyelmeztető ikon, amely a kapcsolatok társítását és a kapcsolatok hozzáadását kéri.</span><span class="sxs-lookup"><span data-stu-id="17ce5-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Folyamat szerkesztése lépésről lépésre":::


5. <span data-ttu-id="17ce5-162">Mit kell tenni, ha az együttműködési javaslati összekötők megoldásának folyamatai nem kapcsolnak be?</span><span class="sxs-lookup"><span data-stu-id="17ce5-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="17ce5-163">A.</span><span class="sxs-lookup"><span data-stu-id="17ce5-163">A.</span></span> <span data-ttu-id="17ce5-164">Ebben Power Automate a következő sorrendben kell szerkesztenie a folyamatokat, és frissítenie őket, hogy a megfelelő kapcsolatokat használják:</span><span class="sxs-lookup"><span data-stu-id="17ce5-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="17ce5-165">Partnerközpont webhookregisztráció (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="17ce5-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="17ce5-166">Közös értékesítési ajánlás létrehozása – Salesforce Partnerközpont (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="17ce5-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="17ce5-167">Partnerközpont Salesforce (Insider Preview) microsoftos közös értékesítési hivatkozási frissítései</span><span class="sxs-lookup"><span data-stu-id="17ce5-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="17ce5-168">Partnerközpont Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="17ce5-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="17ce5-169">Salesforce a Partnerközpont (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="17ce5-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="17ce5-170">Salesforce Opportunity to Partnerközpont (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="17ce5-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="17ce5-171">Salesforce Microsoft Solutions to Partnerközpont (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="17ce5-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="17ce5-172">B.</span><span class="sxs-lookup"><span data-stu-id="17ce5-172">B.</span></span> <span data-ttu-id="17ce5-173">Minden egyes folyamatnál válassza a **Csak felhasználók futtatása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="17ce5-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="17ce5-174">Válassza **a Kapcsolat használata** lehetőséget a Csak **futtatás felhasználója által biztosított helyett.**</span><span class="sxs-lookup"><span data-stu-id="17ce5-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Folyamat aktiválása":::


<span data-ttu-id="17ce5-176">C.</span><span class="sxs-lookup"><span data-stu-id="17ce5-176">C.</span></span> <span data-ttu-id="17ce5-177">Aktiválja az alábbi folyamatokat:</span><span class="sxs-lookup"><span data-stu-id="17ce5-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="17ce5-178">Partnerközpont Microsoft közös értékesítési hivatkozási frissítései a Salesforce-hoz (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="17ce5-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="17ce5-179">Salesforce a Partnerközpont (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="17ce5-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="17ce5-180">D.</span><span class="sxs-lookup"><span data-stu-id="17ce5-180">D.</span></span> <span data-ttu-id="17ce5-181">Aktiválja az összes többi folyamat.</span><span class="sxs-lookup"><span data-stu-id="17ce5-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="17ce5-182">E.</span><span class="sxs-lookup"><span data-stu-id="17ce5-182">E.</span></span> <span data-ttu-id="17ce5-183">A Folyamat Partnerközpont webhookregisztrációnál válassza a **Futtatás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="17ce5-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="17ce5-184">Adja meg **a http URL-címet** az első műveletből **a Partnerközpont Salesforce-folyamatba.**</span><span class="sxs-lookup"><span data-stu-id="17ce5-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="17ce5-185">Válassza ki mind a négy lehetőséget a Regisztrálni kívánt **események** alatt, majd válassza az **Igen** lehetőséget a Felülírás lehetőségnél.</span><span class="sxs-lookup"><span data-stu-id="17ce5-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="17ce5-186">Kérdések és válaszok a futtatásról/karbantartásról</span><span class="sxs-lookup"><span data-stu-id="17ce5-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="17ce5-187">Hogyan háríthatja el a folyamat végrehajtása során Power Automate hibákat?</span><span class="sxs-lookup"><span data-stu-id="17ce5-187">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="17ce5-188">Annak érdekében, hogy a Power Automate folyamat a vártnak megfelelő legyen, és elhárítsa a végrehajtás közbeni hibákat, tekintse meg a [Folyamathibák kijavítása témakört.](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="17ce5-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="17ce5-189">Mit kell tenni, ha olyan hivatkozásokat lát, amelyek nincsenek megfelelően szinkronizálva a Partnerközpont CRM-környezetben?</span><span class="sxs-lookup"><span data-stu-id="17ce5-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="17ce5-190">A hivatkozás-szinkronizálás állapotának meghatározásához válassza a Naplózás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="17ce5-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="A hivatkozások szinkronizálása":::

<span data-ttu-id="17ce5-192">Győződjön meg arról, hogy teljesülnek a következő feltételek:</span><span class="sxs-lookup"><span data-stu-id="17ce5-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="17ce5-193">A megoldásazonosító a lehetőség részeként van megtéve.</span><span class="sxs-lookup"><span data-stu-id="17ce5-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="17ce5-194">Kétbetűs országkód szükséges.</span><span class="sxs-lookup"><span data-stu-id="17ce5-194">Two letter country code is required.</span></span>

- <span data-ttu-id="17ce5-195">Ha a Microsofttól származó segítség van kiválasztva a lehetőséghez, az ügyfél kapcsolattartási adataira van szükség.</span><span class="sxs-lookup"><span data-stu-id="17ce5-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="17ce5-196">Hogyan biztosítható, hogy a hivatkozások kétirányú szinkronizálást biztosítsanak?</span><span class="sxs-lookup"><span data-stu-id="17ce5-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="17ce5-197">Tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="17ce5-197">Do the following steps:</span></span>

- <span data-ttu-id="17ce5-198">A partner értékesítőknek meg kell győződni arról, hogy engedélyezték a Szinkronizálás Partnerközpont **lehetőséget** a CRM szakaszban.</span><span class="sxs-lookup"><span data-stu-id="17ce5-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Győződjön meg arról, hogy engedélyezte a szinkronizálást":::

- <span data-ttu-id="17ce5-200">Az értékesítőknek meg kell adniuk a bevételt és a záró dátumot az érdeklődő minősítésekor.</span><span class="sxs-lookup"><span data-stu-id="17ce5-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="17ce5-201">Ha a CRM-azonosítót  az együttműködési lehetőség létrehozási vagy frissítési szakaszában adja meg, de az adott azonosítóval rendelkező érdeklődői lehetőség nem található a CRM-ben, akkor a rendszer figyelmen kívül hagyja a frissítést vagy létrehozást. </span><span class="sxs-lookup"><span data-stu-id="17ce5-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="17ce5-202">Győződjön meg arról, hogy a hivatkozás pénzneme mező be van állítva a Salesforce-környezetben.</span><span class="sxs-lookup"><span data-stu-id="17ce5-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="17ce5-203">Mit kell tenni, ha az összekötő le lesz választva, és nem rendelkezik hivatkozás-szinkronizálással?</span><span class="sxs-lookup"><span data-stu-id="17ce5-203">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="17ce5-204">Néhány lehetőség a kipróbált lehetőségek közül:</span><span class="sxs-lookup"><span data-stu-id="17ce5-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="17ce5-205">Ellenőrizze, hogy lejárt-e a felhasználónév vagy jelszó a Partnerközpont-rendszergazdai szerepkörökkel rendelkező felhasználó felhasználója számára.</span><span class="sxs-lookup"><span data-stu-id="17ce5-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="17ce5-206">A nem szinkronizált lehetőséggel kisebb frissítést is befejezhet, és megfigyelheti, hogy a hivatkozás szinkronizálva lett-e.</span><span class="sxs-lookup"><span data-stu-id="17ce5-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="17ce5-207">Ha a folyamatok lefuttak és sikertelenek, válassza ki a folyamatot, és küldje el újra a sikertelen futtatásokat.</span><span class="sxs-lookup"><span data-stu-id="17ce5-207">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="17ce5-208">Mit kell tenni, ha hozzáférés-megtagadásos hibákat kap?</span><span class="sxs-lookup"><span data-stu-id="17ce5-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="17ce5-209">Győződjön meg arról, hogy léteznek a megfelelő szerepkörök</span><span class="sxs-lookup"><span data-stu-id="17ce5-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="17ce5-210">Ajánlói rendszergazdai szerepkör Partnerközpont értékesítő számára</span><span class="sxs-lookup"><span data-stu-id="17ce5-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="17ce5-211">Rendszergazda vagy rendszer-testreszava szerepkör a CRM-példányon</span><span class="sxs-lookup"><span data-stu-id="17ce5-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="17ce5-212">Győződjön meg arról, Power Automate flow-fiók felhasználója legalább egyszer https://flow.microsoft.com előre bejelentkezik</span><span class="sxs-lookup"><span data-stu-id="17ce5-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="17ce5-213">Ha azt látja, hogy az **ügyfélfiók országkódja** hiányzik egy közös értékesítés létrehozása során, mit kell tennie?</span><span class="sxs-lookup"><span data-stu-id="17ce5-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="17ce5-214">Hozzá kell adni az ISO kétbetűs országkódját az Ügyfélfiókhoz a CRM-ben.</span><span class="sxs-lookup"><span data-stu-id="17ce5-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="17ce5-215">Mit kell tenni, ha azt  a hibaüzenetet látja, hogy a megoldásazonosítóra szükség van egy közös értékesítés létrehozása során?</span><span class="sxs-lookup"><span data-stu-id="17ce5-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="17ce5-216">Egy közös értékesítésre vonatkozó javaslat létrehozásához a Microsoft közös értékesítésre kész megoldásra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="17ce5-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="17ce5-217">Mit kell tenni, ha olyan, a crm-sel nem szinkronizált Partnerközpont-ban létrejött, közös értékesítést lehetővé tehetünk, annak ellenére, hogy nincsenek folyamathibák?</span><span class="sxs-lookup"><span data-stu-id="17ce5-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="17ce5-218">Tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="17ce5-218">Do the following:</span></span>

- <span data-ttu-id="17ce5-219">Miután létrehozott egy új közös értékesítést az Partnerközpont-ban, ellenőrizze, hogy meg lesz-e hívva Partnerközpont-e a Dynamics 365-folyamathoz való Partnerközpont (előfordulhat, hogy többször is meghívja).</span><span class="sxs-lookup"><span data-stu-id="17ce5-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="17ce5-220">Ha a folyamat meghívásra kerül, ellenőrizze az összes meghívott folyamatot, és azonosítsa a folyamat futását, amely frissíti a CRM-et.</span><span class="sxs-lookup"><span data-stu-id="17ce5-220">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="17ce5-221">A műveleteket követni tudja, és ellenőrizheti, hogy frissült-e a CRM,vagy tapasztalt-e problémát.</span><span class="sxs-lookup"><span data-stu-id="17ce5-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="17ce5-222">Tekintse **meg az Új üzlet** Partnerközpont, hogy feltöltődik-e a CRM-azonosítóval.</span><span class="sxs-lookup"><span data-stu-id="17ce5-222">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="17ce5-223">Győződjön meg arról, hogy az  üzlet nem záródik le véletlenül Won (Megnyert) vagy **Lost** (Elveszett) ként a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="17ce5-223">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="17ce5-224">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="17ce5-224">Next steps</span></span>

- [<span data-ttu-id="17ce5-225">Érdeklődők kezelése</span><span class="sxs-lookup"><span data-stu-id="17ce5-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="17ce5-226">Együttes értékesítési lehetőségek kezelése</span><span class="sxs-lookup"><span data-stu-id="17ce5-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
