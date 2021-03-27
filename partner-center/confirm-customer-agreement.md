---
title: Annak ellenőrzése, hogy az ügyfél elfogadta-e a Microsoft ügyfél-szerződést a CSP programhoz
description: A Microsoft-szolgáltatások ügyfeleknek való megrendelése előtt a Cloud Solution Provider (CSP) partnereinek meg kell erősíteniük a Microsoft ügyfél-szerződését.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633778"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="8ed37-103">Annak ellenőrzése, hogy az ügyfél elfogadta-e a Microsoft ügyfél-szerződést a CSP programhoz</span><span class="sxs-lookup"><span data-stu-id="8ed37-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="8ed37-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="8ed37-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8ed37-105">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="8ed37-105">Admin agent</span></span>
- <span data-ttu-id="8ed37-106">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="8ed37-106">Sales agent</span></span>


<span data-ttu-id="8ed37-107">Az ügyfelek két lehetőség közül választhatnak, hogy elfogadják a Microsoft ügyfél-szerződését.</span><span class="sxs-lookup"><span data-stu-id="8ed37-107">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="8ed37-108">**1. lehetőség**: az ügyfél-hitelesítés partneri igazolása – a partner megerősítheti az ügyfelek elfogadását a partner Center API/SDK használatával vagy a partner Center irányítópultján.</span><span class="sxs-lookup"><span data-stu-id="8ed37-108">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="8ed37-109">**2. lehetőség**: közvetlen ügyfél-elfogadás – a partner meghívhatja az ügyfelet egy URL-címen keresztül, hogy áttekintse és elfogadja a szerződést a Microsoft 365 felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="8ed37-109">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="8ed37-110">Hozzáférés a Microsoft ügyfél-szerződési sablonhoz</span><span class="sxs-lookup"><span data-stu-id="8ed37-110">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="8ed37-111">A Microsoft Customer Agreement sablon legújabb verzióját manuálisan is letöltheti [innen.](https://aka.ms/customeragreement)</span><span class="sxs-lookup"><span data-stu-id="8ed37-111">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="8ed37-112">A Microsoft Customer szerződés országspecifikus.</span><span class="sxs-lookup"><span data-stu-id="8ed37-112">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="8ed37-113">A Microsoft ügyfél-szerződési sablon kérésekor a megfelelő országot válassza ki az ügyfél helye alapján.</span><span class="sxs-lookup"><span data-stu-id="8ed37-113">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="8ed37-114">1. lehetőség: az ügyfelek elfogadásának megerősítése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="8ed37-114">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="8ed37-115">A közvetlen számla partnerei megerősítik a Microsoft ügyfél-szerződését a partner Centerben az új és a meglévő ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="8ed37-115">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="8ed37-116">A közvetett viszonteladók nem tanúsítják az ügyfeleik nevében, és nem kell együttműködni a közvetett szolgáltatóval az igazolás befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="8ed37-116">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="8ed37-117">Az ügyfelek elfogadásának megerősítése új ügyfelek esetén</span><span class="sxs-lookup"><span data-stu-id="8ed37-117">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="8ed37-118">Amikor új ügyfél-bérlőt hoz létre a partner Centerben, kövesse az alábbi lépéseket a Microsoft ügyfél-szerződés elfogadásának megerősítéséhez.</span><span class="sxs-lookup"><span data-stu-id="8ed37-118">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="8ed37-119">A lépések végrehajtásához rendszergazdai vagy értékesítési ügynöknek kell tartoznia.</span><span class="sxs-lookup"><span data-stu-id="8ed37-119">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="8ed37-120">Válassza az **ügyfelek**, majd az **új ügyfél** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ed37-120">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="8ed37-121">A **fiók adatai** területen adja meg a vállalat és az elsődleges kapcsolattartó adatait.</span><span class="sxs-lookup"><span data-stu-id="8ed37-121">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="8ed37-122">A **Microsoft-szerződés** területen jelölje be a jelölőnégyzetet annak igazolására, hogy az ügyfél elfogadta a Microsoft ügyfél-szerződést.</span><span class="sxs-lookup"><span data-stu-id="8ed37-122">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="8ed37-123">A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot.</span><span class="sxs-lookup"><span data-stu-id="8ed37-123">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="8ed37-124">Ez nem állítható be jövőbeli dátumra.</span><span class="sxs-lookup"><span data-stu-id="8ed37-124">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="8ed37-125">Győződjön meg arról, hogy az elsődleges felhasználói kapcsolattartási adatok helyesek.</span><span class="sxs-lookup"><span data-stu-id="8ed37-125">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="8ed37-126">Ha nem megfelelő, válassza a **frissítés** lehetőséget, és adja meg a szerződést elfogadó személy pontos információit.</span><span class="sxs-lookup"><span data-stu-id="8ed37-126">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="8ed37-127">A **tovább** gombra kattintva folytathatja az ügyfél-bérlő létrehozását.</span><span class="sxs-lookup"><span data-stu-id="8ed37-127">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Új ügyfél":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="8ed37-129">Ügyfelek elfogadásának megerősítése meglévő ügyfelek esetén</span><span class="sxs-lookup"><span data-stu-id="8ed37-129">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="8ed37-130">Ennek elvégzéséhez rendszergazdai vagy értékesítési ügynöknek kell lennie:</span><span class="sxs-lookup"><span data-stu-id="8ed37-130">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="8ed37-131">Válassza az **Ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ed37-131">Select **Customers**.</span></span> <span data-ttu-id="8ed37-132">Keresse meg és válassza ki az ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="8ed37-132">Find and select the customer.</span></span>

2. <span data-ttu-id="8ed37-133">Válassza a **fiókadatok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ed37-133">Select **Account info**.</span></span>

3. <span data-ttu-id="8ed37-134">A **Microsoft ügyfél-szerződés** területen válassza a **frissítés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ed37-134">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="8ed37-135">Adja meg a szerződést elfogadó személy **utónevét**, **vezetéknevét**, **e-mail-címét** és **telefonszámát** (nem kötelező).</span><span class="sxs-lookup"><span data-stu-id="8ed37-135">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="8ed37-136">A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot.</span><span class="sxs-lookup"><span data-stu-id="8ed37-136">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="8ed37-137">Ez nem állítható be jövőbeli dátumra.</span><span class="sxs-lookup"><span data-stu-id="8ed37-137">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="8ed37-138">Válassza a **Mentés** és Folytatás lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ed37-138">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Meglévő ügyfél":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="8ed37-140">Az ügyfél-elfogadás megerősítésének beolvasása</span><span class="sxs-lookup"><span data-stu-id="8ed37-140">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="8ed37-141">A következő lépések végrehajtásával kérheti le, hogy egy meglévő ügyfél elfogadta a Microsoft ügyfél-szerződést.</span><span class="sxs-lookup"><span data-stu-id="8ed37-141">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="8ed37-142">Ehhez rendszergazdai ügynöknek vagy értékesítési ügynöknek kell lennie.</span><span class="sxs-lookup"><span data-stu-id="8ed37-142">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="8ed37-143">Válassza ki az **ügyfelek** lehetőséget, majd keresse meg és válassza ki a megtekinteni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="8ed37-143">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="8ed37-144">Válassza a **fiókadatok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ed37-144">Select **Account info**.</span></span>

3. <span data-ttu-id="8ed37-145">A **Microsoft ügyfél-szerződés** alatt tekintse meg, hogy az ügyfél nem adta-e meg a megerősítést.</span><span class="sxs-lookup"><span data-stu-id="8ed37-145">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="8ed37-146">Az ügyfelek elfogadásának megerősítése a partner Center API/SDK használatával</span><span class="sxs-lookup"><span data-stu-id="8ed37-146">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="8ed37-147">A partner Center API/SDK használatával megerősítheti a Microsoft-ügyfél szerződését.</span><span class="sxs-lookup"><span data-stu-id="8ed37-147">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="8ed37-148">Az API-val/SDK-val kapcsolatos részletekért tekintse meg a következőt:</span><span class="sxs-lookup"><span data-stu-id="8ed37-148">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="8ed37-149">A Microsoft Ügyfélszerződés szerződési metaadatainak lekérése</span><span class="sxs-lookup"><span data-stu-id="8ed37-149">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="8ed37-150">Annak megerősítése, hogy az ügyfél elfogadta a Microsoft Ügyfélszerződést</span><span class="sxs-lookup"><span data-stu-id="8ed37-150">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="8ed37-151">A Microsoft Ügyfélszerződés ügyfél általi elfogadási megerősítésének lekérése</span><span class="sxs-lookup"><span data-stu-id="8ed37-151">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="8ed37-152">Letöltési hivatkozás letöltése a Microsoft ügyfél-szerződési sablonhoz</span><span class="sxs-lookup"><span data-stu-id="8ed37-152">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="8ed37-153">2. lehetőség: az ügyfél elfogadottsága Microsoft 365 felügyeleti központban</span><span class="sxs-lookup"><span data-stu-id="8ed37-153">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="8ed37-154">A partnerek meghívhatnak új és meglévő ügyfeleket egy URL-címen keresztül, hogy áttekintsék és elfogadják a szerződést a Microsoft 365 felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="8ed37-154">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="8ed37-155">A következő néhány szakaszban bemutatjuk, hogyan végezheti el a következőket:</span><span class="sxs-lookup"><span data-stu-id="8ed37-155">The next few sections show you how to:</span></span>

- <span data-ttu-id="8ed37-156">Hozzon létre egy új ügyfelet, és kérje meg az ügyféltől a szerződés áttekintését és elfogadását.</span><span class="sxs-lookup"><span data-stu-id="8ed37-156">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="8ed37-157">Kérje meg az új ügyfelet, hogy tekintse át és fogadja el a viszonteladói kapcsolatot és szerződést.</span><span class="sxs-lookup"><span data-stu-id="8ed37-157">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="8ed37-158">Kérje meg a meglévő ügyfelet, hogy tekintse át és fogadja el a szerződést.</span><span class="sxs-lookup"><span data-stu-id="8ed37-158">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="8ed37-159">A [partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) használatával lekérheti a Microsoft ügyfél-szerződés közvetlen elfogadásának állapotát.</span><span class="sxs-lookup"><span data-stu-id="8ed37-159">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="8ed37-160">Hozzon létre egy új ügyfelet, és kérje meg az ügyfelet a szerződés áttekintésére és elfogadására</span><span class="sxs-lookup"><span data-stu-id="8ed37-160">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="8ed37-161">A következő lépésekkel hozzon létre egy új ügyfelet a partner Centerben, majd hívja meg őket, hogy tekintsék át és fogadják el a Microsoft Customer szerződést Microsoft 365 felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="8ed37-161">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="8ed37-162">A partner Center **ügyfelek** lapján válassza az **ügyfél hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ed37-162">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="8ed37-163">A **fiókadatok** területen adja meg az új ügyfél adatait az összes kötelező mezőben, beleértve az ügyfél vállalatának nevét és az elsődleges kapcsolattartót is.</span><span class="sxs-lookup"><span data-stu-id="8ed37-163">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="8ed37-164">Az **ügyfél szerződése** területen válassza **az ügyfél lehetőséget, hogy fogadja el a Microsoft Customer szerződést Microsoft 365 felügyeleti központban**.</span><span class="sxs-lookup"><span data-stu-id="8ed37-164">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="8ed37-165">Hajtsa végre az oldalon található egyéb kötelező mezőket.</span><span class="sxs-lookup"><span data-stu-id="8ed37-165">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="8ed37-166">Válassza a Next (tovább) lehetőséget **: Tekintse át** , majd folytassa az ügyfél-bérlő létrehozásához szükséges lépéseket.</span><span class="sxs-lookup"><span data-stu-id="8ed37-166">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="8ed37-167">Az új ügyfelek nem vásárolhatják meg a vásárlást, amíg el nem fogadják a Microsoft Customer szerződést.</span><span class="sxs-lookup"><span data-stu-id="8ed37-167">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Új ügyfél létrehozása":::

5. <span data-ttu-id="8ed37-169">Amikor eléri a **megerősítő** képernyőt az új ügyfél munkafolyamatban, mentse az ügyfél hitelesítő adatait.</span><span class="sxs-lookup"><span data-stu-id="8ed37-169">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="8ed37-170">Ezeket a hitelesítő adatokat később kell megadnia az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="8ed37-170">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="8ed37-171">A partner centeren kívül hozzon létre és küldjön egy e-mailt, amely meghívja az ügyfelet, hogy fogadja el a Microsoft Customer szerződést Microsoft 365 felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="8ed37-171">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="8ed37-172">Ügyeljen rá, hogy ezeket az elemeket az e-mailben adja meg:</span><span class="sxs-lookup"><span data-stu-id="8ed37-172">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="8ed37-173">Hivatkozás erre az [URL-címre](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (bejelentkezés szükséges)</span><span class="sxs-lookup"><span data-stu-id="8ed37-173">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="8ed37-174">Az ügyfél az 5. lépésben mentett hitelesítő adatai.</span><span class="sxs-lookup"><span data-stu-id="8ed37-174">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="8ed37-175">Az ügyfél ezután megkapja az e-mailes meghívót a partnertől, és kiválasztja az [URL-címet](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="8ed37-175">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="8ed37-176">Az ügyfél a megadott felhasználói hitelesítő adatokkal jelentkezik be Microsoft 365 felügyeleti központba.</span><span class="sxs-lookup"><span data-stu-id="8ed37-176">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="8ed37-177">Az ügyfél ellenőrzi a mezőt, hogy fogadja el a Microsoft ügyfél-szerződést.</span><span class="sxs-lookup"><span data-stu-id="8ed37-177">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="8ed37-178">Új ügyfél meghívása a viszonteladói kapcsolat és a Microsoft ügyfél-szerződés áttekintéséhez és elfogadásához</span><span class="sxs-lookup"><span data-stu-id="8ed37-178">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="8ed37-179">A következő lépésekkel meghívhat egy új ügyfelet a viszonteladói kapcsolat és a Microsoft ügyfél-szerződés áttekintésére és elfogadására.</span><span class="sxs-lookup"><span data-stu-id="8ed37-179">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="8ed37-180">A partner Center **ügyfelek** lapján válassza a **viszonteladói kapcsolat kérése** hivatkozást.</span><span class="sxs-lookup"><span data-stu-id="8ed37-180">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="8ed37-181">Létrejön egy automatikus e-mail sablon, amely tartalmazza a szöveget és egy paraméteres URL-címet, amely a Microsoft 365 felügyeleti központba irányítja az ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="8ed37-181">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="8ed37-182">Testreszabhatja az automatikusan létrehozott e-mail-sablont, majd kiválaszthatja a **Másolás a vágólapra** vagy **a Megnyitás e-mailben** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ed37-182">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="8ed37-183">Ezzel az e-mail sablonnal meghívhatja az ügyfelet, hogy fogadja el a **viszonteladói kapcsolatra** vonatkozó kérelmet és a **Microsoft Customer szerződést**.</span><span class="sxs-lookup"><span data-stu-id="8ed37-183">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="8ed37-184">(Megjegyzés: a meghívó e-mailben ellenőrizze, hogy a partner tartalmazza-e az automatikusan megadott URL-címet, valamint a nemrégiben létrehozott ügyfél-hitelesítő adatokat is.)</span><span class="sxs-lookup"><span data-stu-id="8ed37-184">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="kapcsolat létrehozása":::

5. <span data-ttu-id="8ed37-186">Az ügyfél e-mailben fogadja a meghívót, és rákattint a paraméteres URL-címre.</span><span class="sxs-lookup"><span data-stu-id="8ed37-186">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="8ed37-187">Az ügyfél az e-mailben megadott hitelesítő adatokat használja a Microsoft 365 felügyeleti központba való bejelentkezéshez.</span><span class="sxs-lookup"><span data-stu-id="8ed37-187">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="8ed37-188">Az ügyfél ellenőrzi a mezőt, hogy elfogadja a **viszonteladói kapcsolatot** és a **Microsoft ügyfél-szerződést**.</span><span class="sxs-lookup"><span data-stu-id="8ed37-188">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="8ed37-189">Ugyanazon az URL-címen belül az ügyfél megtekintheti a különböző partnerek összevont listáját, amelyekkel dolgozik.</span><span class="sxs-lookup"><span data-stu-id="8ed37-189">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="8ed37-190">Kijelölhetnek egy partnert a részletek megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="8ed37-190">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Szerződés elfogadása":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="8ed37-192">Meglévő ügyfél meghívása a szerződés áttekintéséhez és elfogadásához</span><span class="sxs-lookup"><span data-stu-id="8ed37-192">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="8ed37-193">A következő lépésekkel meghívhat egy meglévő ügyfelet a Microsoft Customer szerződés áttekintéséhez és elfogadásához.</span><span class="sxs-lookup"><span data-stu-id="8ed37-193">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="8ed37-194">Hozza létre az ügyfél e-mail-címét a beágyazott URL-címmel, amelyben meghívja ügyfeleit, hogy fogadja el a Microsoft Customer szerződést.</span><span class="sxs-lookup"><span data-stu-id="8ed37-194">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="8ed37-195">Az ügyfél e-mailben fogadja a meghívót, és rákattint az [URL-címre](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="8ed37-195">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="8ed37-196">Az ügyfél a hitelesítő adataikat Microsoft 365 felügyeleti központba írja be.</span><span class="sxs-lookup"><span data-stu-id="8ed37-196">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="8ed37-197">Az ügyfél ellenőrzi a mezőt, hogy fogadja el a Microsoft ügyfél-szerződést.</span><span class="sxs-lookup"><span data-stu-id="8ed37-197">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="8ed37-198">Ugyanezen az URL-címen az ügyfél láthatja a különböző partnerek összevont listáját, amelyekkel dolgozik.</span><span class="sxs-lookup"><span data-stu-id="8ed37-198">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="8ed37-199">Kijelölhetnek egy partnert a részletek megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="8ed37-199">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="ügyfél":::

>[!NOTE]
><span data-ttu-id="8ed37-201">Bizonyos esetekben előfordulhat, hogy az ügyfelek nem tudják közvetlenül elfogadni a Microsoft ügyfél-szerződést.</span><span class="sxs-lookup"><span data-stu-id="8ed37-201">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="8ed37-202">Ha többet szeretne megtudni ezekről a helyzetekről, olvassa el a következő két forgatókönyvet, ahol az ügyfél nevében kell tanúsítani az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="8ed37-202">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="8ed37-203">Két forgatókönyv, ahol az ügyfél nevében kell tanúsítani</span><span class="sxs-lookup"><span data-stu-id="8ed37-203">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="8ed37-204">Két forgatókönyv esetén előfordulhat, hogy az ügyfelek nem tudják közvetlenül elfogadni a Microsoft ügyfél-szerződést a Microsoft 365 felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="8ed37-204">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="8ed37-205">**1. eset**: egy meglévő ügyfél a következők bármelyikét vásárolta egy meglévő partneri kapcsolaton keresztül: ajánlatok, szoftver-vagy szoftver-előfizetések, fenntartott példányok vagy Azure-csomag.</span><span class="sxs-lookup"><span data-stu-id="8ed37-205">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="8ed37-206">Az ügyfél most megpróbál új vásárlást végezni (az automatikus megújítás kivételével).</span><span class="sxs-lookup"><span data-stu-id="8ed37-206">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="8ed37-207">Amikor az ügyfél az URL-címre kattint, a "Kérjük, forduljon a partneréhez, hogy erősítse meg a Microsoft-ügyfél szerződését."</span><span class="sxs-lookup"><span data-stu-id="8ed37-207">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="8ed37-208">**Megoldás**: az ügyfél nevében kell tanúsítani.</span><span class="sxs-lookup"><span data-stu-id="8ed37-208">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Képernyőkép a Microsoft 365 felügyeleti központ oldaláról, amely arra kéri, hogy forduljon a partnerhez a Microsoft ügyfél-szerződés elfogadásának megerősítéséhez.":::

<span data-ttu-id="8ed37-210">**2. forgatókönyv**: egy meglévő ügyfél megvásárolta a következő ajánlatok bármelyikét, a szoftver-és szoftver-előfizetéseket, a fenntartott példányokat és az Azure-csomagot.</span><span class="sxs-lookup"><span data-stu-id="8ed37-210">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="8ed37-211">Az ügyfél most megpróbál új partnert vásárolni.</span><span class="sxs-lookup"><span data-stu-id="8ed37-211">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="8ed37-212">Amikor az ügyfél az új partneri kapcsolat és a szerződés elfogadásához rákattint az Microsoft 365 felügyeleti központ URL-címére, a következő üzenet jelenik meg: "Kérjük, forduljon a partneréhez, hogy erősítse meg a Microsoft-ügyfél szerződését."</span><span class="sxs-lookup"><span data-stu-id="8ed37-212">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="8ed37-213">**Megoldás**: az ügyfél nevében kell tanúsítani.</span><span class="sxs-lookup"><span data-stu-id="8ed37-213">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="8ed37-214">Erősítse meg, hogy az ügyfél elfogadta a szerződést</span><span class="sxs-lookup"><span data-stu-id="8ed37-214">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="8ed37-215">Ha olyan meglévő ügyfélhez próbál új rendelést létrehozni, akit még nem erősített meg, a megerősítés befejezésére vonatkozó kérést kap.</span><span class="sxs-lookup"><span data-stu-id="8ed37-215">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="8ed37-216">Ezt a következő eljárással végezheti el.</span><span class="sxs-lookup"><span data-stu-id="8ed37-216">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="8ed37-217">Adja meg a szerződést elfogadó felhasználó **utónevét**, **vezetéknevét**, **e-mail címét** és **telefonszámát** (nem kötelező).</span><span class="sxs-lookup"><span data-stu-id="8ed37-217">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="8ed37-218">A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot.</span><span class="sxs-lookup"><span data-stu-id="8ed37-218">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="8ed37-219">Ez nem állítható be jövőbeli dátumra.</span><span class="sxs-lookup"><span data-stu-id="8ed37-219">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="8ed37-220">Válassza a **Mentés és folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ed37-220">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="8ed37-221">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="8ed37-221">Next steps</span></span>

- [<span data-ttu-id="8ed37-222">A vállalati profil adatainak ellenőrzése vagy frissítése</span><span class="sxs-lookup"><span data-stu-id="8ed37-222">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="8ed37-223">Microsoft Ügyfélszerződés (régió és nyelv szerint)</span><span class="sxs-lookup"><span data-stu-id="8ed37-223">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
