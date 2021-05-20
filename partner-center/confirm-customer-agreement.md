---
title: Annak ellenőrzése, hogy az ügyfél elfogadta-e Microsoft Ügyfélszerződés CSP-programhoz
description: Felhőszolgáltató (CSP) partnereknek meg kell erősítenie az ügyfél általi Microsoft Ügyfélszerződés, mielőtt Microsoft-szolgáltatások az ügyfeleknek.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: c75f129ae5a0755833462138f60901cc7ff36732
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148516"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="6d541-103">Annak ellenőrzése, hogy az ügyfél elfogadta-e Microsoft Ügyfélszerződés CSP-programhoz</span><span class="sxs-lookup"><span data-stu-id="6d541-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="6d541-104">**Megfelelő szerepkörök:** Rendszergazdai ügynök | Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="6d541-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="6d541-105">Az ügyfelek két lehetőség közül választhatnak, hogy hogyan fogadják el a Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="6d541-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="6d541-106">**1. lehetőség:** Az ügyfél-elfogadás partneri igazolása – A partner az API/SDK használatával Partnerközpont ügyfél-elfogadást Partnerközpont meg.</span><span class="sxs-lookup"><span data-stu-id="6d541-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="6d541-107">**2. lehetőség:** Az ügyfél közvetlen elfogadása – A partner meghívhatja az ügyfelet egy URL-címen keresztül, hogy áttekintse és elfogadja a Microsoft 365 Felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="6d541-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="6d541-108">Hozzáférés Microsoft Ügyfélszerződés sablonhoz</span><span class="sxs-lookup"><span data-stu-id="6d541-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="6d541-109">A sablon legújabb verzióját manuálisan letöltheti innen Microsoft Ügyfélszerződés [sablont.](https://aka.ms/customeragreement)</span><span class="sxs-lookup"><span data-stu-id="6d541-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="6d541-110">A Microsoft Ügyfélszerződés országspecifikus.</span><span class="sxs-lookup"><span data-stu-id="6d541-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="6d541-111">A sablon Microsoft Ügyfélszerződés mindenképpen a megfelelő országot válassza ki az ügyfél helye alapján.</span><span class="sxs-lookup"><span data-stu-id="6d541-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="6d541-112">1. lehetőség: Az ügyfél elfogadásának megerősítése a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="6d541-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="6d541-113">A közvetlen számlázási partnerek megerősíthetik, hogy az ügyfelek elfogadják Microsoft Ügyfélszerződés-Partnerközpont új és meglévő ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="6d541-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="6d541-114">A közvetett viszonteladók nem igazolhatóak az ügyfeleik nevében, és a közvetett szolgáltatójukkal kell dolgozniuk az igazolás elvégzéséhez.</span><span class="sxs-lookup"><span data-stu-id="6d541-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="6d541-115">Az ügyfelek új ügyfelek általi elfogadásának megerősítése</span><span class="sxs-lookup"><span data-stu-id="6d541-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="6d541-116">Amikor új ügyfélbérlőt hoz létre a Partnerközpont, a következő lépésekkel erősítse meg, hogy az ügyfél elfogadta a Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="6d541-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="6d541-117">A lépések végrehajtásához rendszergazdai vagy értékesítési ügynöknek kell lennie.</span><span class="sxs-lookup"><span data-stu-id="6d541-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="6d541-118">Válassza **az Ügyfelek,** majd az **Új ügyfél lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6d541-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="6d541-119">A **Fiókadatok alatt** adja meg a vállalat és az elsődleges kapcsolattartó adatait.</span><span class="sxs-lookup"><span data-stu-id="6d541-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="6d541-120">A **Microsoft-szerződés** alatt jelölje be a jelölőnégyzetet, amely igazolja, hogy az ügyfél elfogadta a Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="6d541-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="6d541-121">A **Szerződés elfogadásának dátuma alatt** adja meg a megfelelő dátumot.</span><span class="sxs-lookup"><span data-stu-id="6d541-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="6d541-122">Ezt nem állíthatja be jövőbeli dátumra.</span><span class="sxs-lookup"><span data-stu-id="6d541-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="6d541-123">Győződjön meg arról, hogy az elsődleges felhasználó megjelenített kapcsolattartási adatai helyesek.</span><span class="sxs-lookup"><span data-stu-id="6d541-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="6d541-124">Ha helytelen, válassza a **Frissítés** lehetőséget, és adja meg a szerződést elfogadó személy pontos adatait.</span><span class="sxs-lookup"><span data-stu-id="6d541-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="6d541-125">Kattintson **a Tovább gombra** az ügyfélbérlő létrehozásának folytatásához.</span><span class="sxs-lookup"><span data-stu-id="6d541-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Új ügyfél":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="6d541-127">Az ügyfelek meglévő ügyfelek általi elfogadásának megerősítése</span><span class="sxs-lookup"><span data-stu-id="6d541-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="6d541-128">Ehhez rendszergazdai ügynöknek vagy értékesítési ügynöknek kell lennie:</span><span class="sxs-lookup"><span data-stu-id="6d541-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="6d541-129">Válassza az **Ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6d541-129">Select **Customers**.</span></span> <span data-ttu-id="6d541-130">Keresse meg és válassza ki az ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="6d541-130">Find and select the customer.</span></span>

2. <span data-ttu-id="6d541-131">Válassza **a Fiókadatok lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6d541-131">Select **Account info**.</span></span>

3. <span data-ttu-id="6d541-132">A **Microsoft Ügyfélszerződés** válassza a **Frissítés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6d541-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="6d541-133">Adja meg **a** szerződést elfogadó személy vezetéknevét, vezetéknevét, e-mail-címét és telefonszámát **(nem** kötelező).</span><span class="sxs-lookup"><span data-stu-id="6d541-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="6d541-134">A **Szerződés elfogadásának dátuma alatt** adja meg a megfelelő dátumot.</span><span class="sxs-lookup"><span data-stu-id="6d541-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="6d541-135">Ezt nem állíthatja be jövőbeli dátumra.</span><span class="sxs-lookup"><span data-stu-id="6d541-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="6d541-136">Válassza **a Mentés és** folytatás lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6d541-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Meglévő ügyfél":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="6d541-138">Ügyfél-elfogadás megerősítésének lekérése</span><span class="sxs-lookup"><span data-stu-id="6d541-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="6d541-139">Annak megerősítéséhez, hogy egy meglévő ügyfél elfogadta a Microsoft Ügyfélszerződés, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="6d541-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="6d541-140">Ehhez rendszergazdai ügynöknek vagy értékesítési ügynöknek kell lennie.</span><span class="sxs-lookup"><span data-stu-id="6d541-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="6d541-141">Válassza **az Ügyfelek** lehetőséget, majd keresse meg és válassza ki a látni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="6d541-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="6d541-142">Válassza a **Fiókadatok lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6d541-142">Select **Account info**.</span></span>

3. <span data-ttu-id="6d541-143">A **Microsoft-ügyfélszerződés alatt** megtekintheti, hogy az ügyfél nem adott-e meg megerősítést.</span><span class="sxs-lookup"><span data-stu-id="6d541-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="6d541-144">Ügyfél-elfogadás megerősítése Partnerközpont API/SDK használatával</span><span class="sxs-lookup"><span data-stu-id="6d541-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="6d541-145">A Partnerközpont API/SDK használatával megerősítheti, hogy az ügyfelek elfogadják a Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="6d541-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="6d541-146">Az API/SDK részleteiért tekintse meg a következőt:</span><span class="sxs-lookup"><span data-stu-id="6d541-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="6d541-147">A Microsoft Ügyfélszerződés szerződési metaadatainak lekérése</span><span class="sxs-lookup"><span data-stu-id="6d541-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="6d541-148">Annak megerősítése, hogy az ügyfél elfogadta a Microsoft Ügyfélszerződést</span><span class="sxs-lookup"><span data-stu-id="6d541-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="6d541-149">A Microsoft Ügyfélszerződés ügyfél általi elfogadási megerősítésének lekérése</span><span class="sxs-lookup"><span data-stu-id="6d541-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="6d541-150">A sablon letöltési hivatkozásának Microsoft Ügyfélszerződés letöltése</span><span class="sxs-lookup"><span data-stu-id="6d541-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="6d541-151">2. lehetőség: Ügyfél-elfogadás Microsoft 365 Felügyeleti központban</span><span class="sxs-lookup"><span data-stu-id="6d541-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="6d541-152">A partnerek meghívhatják az új és meglévő ügyfeleket egy URL-címen keresztül, hogy áttekintik és elfogadják a Microsoft 365 Felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="6d541-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="6d541-153">A következő néhány szakasz a következőt mutatja be:</span><span class="sxs-lookup"><span data-stu-id="6d541-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="6d541-154">Hozzon létre egy új ügyfelet, és hívja meg az ügyfelet, hogy tekintse át és fogadja el a szerződést.</span><span class="sxs-lookup"><span data-stu-id="6d541-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="6d541-155">Hívjon meg egy új ügyfelet, hogy tekintse át és fogadja el a viszonteladói kapcsolatot és szerződést.</span><span class="sxs-lookup"><span data-stu-id="6d541-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="6d541-156">Meghívhat egy meglévő ügyfelet, hogy tekintse át és fogadja el a szerződést.</span><span class="sxs-lookup"><span data-stu-id="6d541-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="6d541-157">A Partnerközpont [API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) használatával lekértheti az ügyfél közvetlen elfogadásának Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="6d541-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="6d541-158">Hozzon létre egy új ügyfelet, és hívja meg az ügyfelet, hogy tekintse át és fogadja el a szerződést</span><span class="sxs-lookup"><span data-stu-id="6d541-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="6d541-159">Az alábbi lépésekkel hozzon létre egy új ügyfelet a Partnerközpont, majd hívja meg őket, hogy fogadják el Microsoft Ügyfélszerződés felügyeleti Microsoft 365 felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="6d541-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="6d541-160">A lap **Ügyfelek lapján** válassza Partnerközpont Ügyfél **hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6d541-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="6d541-161">A **Fiókadatok területen** adja meg az új ügyfél adatait az összes kötelező mezőben, beleértve az ügyfél vállalatnevét és elsődleges kapcsolattartóját.</span><span class="sxs-lookup"><span data-stu-id="6d541-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="6d541-162">Az **Ügyfélszerződés alatt** válassza az Ügyfél lehetőséget, és fogadja el Microsoft Ügyfélszerződés felügyeleti **Microsoft 365 központban.**</span><span class="sxs-lookup"><span data-stu-id="6d541-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="6d541-163">Töltse ki az oldalon található összes többi kötelező mezőt.</span><span class="sxs-lookup"><span data-stu-id="6d541-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="6d541-164">Válassza **a Tovább: Áttekintés lehetőséget,** majd folytassa az ügyfélbérlő létrehozásához szükséges lépéseket.</span><span class="sxs-lookup"><span data-stu-id="6d541-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="6d541-165">Az új ügyfelek csak akkor vásárolhatnak, ha elfogadják a Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="6d541-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Új ügyfél létrehozása":::

5. <span data-ttu-id="6d541-167">Amikor eléri a **Megerősítés** képernyőt az új ügyfél-munkafolyamatban, mentse az ügyfél hitelesítő adatait.</span><span class="sxs-lookup"><span data-stu-id="6d541-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="6d541-168">Ezeket a hitelesítő adatokat később meg kell adni az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="6d541-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="6d541-169">A Partnerközpont hozzon létre és küldjön egy e-mailt, amely meghívja az ügyfelet, hogy fogadja Microsoft Ügyfélszerződés felügyeleti Microsoft 365 felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="6d541-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="6d541-170">Ügyeljen arra, hogy az alábbi elemeket is tartalmazza az e-mailben:</span><span class="sxs-lookup"><span data-stu-id="6d541-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="6d541-171">Az URL-címre mutató [hivatkozás](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (bejelentkezés szükséges)</span><span class="sxs-lookup"><span data-stu-id="6d541-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="6d541-172">Az ügyfél 5. lépésben mentett hitelesítő adatai.</span><span class="sxs-lookup"><span data-stu-id="6d541-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="6d541-173">Az ügyfél ezután megkapja az e-mailes meghívót a partnertől, és kiválasztja a [URL-címet.](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)</span><span class="sxs-lookup"><span data-stu-id="6d541-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="6d541-174">Az ügyfél bejelentkezik Microsoft 365 Felügyeleti központba a megadott ügyfél-hitelesítő adatokkal.</span><span class="sxs-lookup"><span data-stu-id="6d541-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="6d541-175">Az ügyfél a microsoftos ügyfélszerződés elfogadásához ellenőrzi a jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="6d541-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="6d541-176">Hívjon meg egy új ügyfelet, hogy tekintse át és fogadja el a viszonteladói kapcsolatot, és Microsoft Ügyfélszerződés</span><span class="sxs-lookup"><span data-stu-id="6d541-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="6d541-177">Az alábbi lépésekkel meghívhat egy új ügyfelet, hogy tekintse át és fogadja el a viszonteladói kapcsolatot és a Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="6d541-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="6d541-178">A lap **Ügyfelek Partnerközpont** válassza **a Viszonteladói kapcsolat kérése hivatkozást.**</span><span class="sxs-lookup"><span data-stu-id="6d541-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="6d541-179">A rendszer létrehoz egy automatikus e-mail-sablont, amely szöveget és egy paraméteres URL-címet tartalmaz, amely az ügyfelet a felügyeleti Microsoft 365 irányítja.</span><span class="sxs-lookup"><span data-stu-id="6d541-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="6d541-180">Testreszabhatja az automatikusan létrehozott e-mail-sablont, majd kiválaszthatja a Másolás a **vágólapra** vagy **a Megnyitás e-mailben lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6d541-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="6d541-181">Ezzel az e-mail-sablonnal meghívhatja az ügyfelet, hogy fogadja el a **viszonteladói** kapcsolatkérést és a **Microsoft Ügyfélszerződés.**</span><span class="sxs-lookup"><span data-stu-id="6d541-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="6d541-182">(Megjegyzés: Az e-mailes meghívóban győződjön meg arról, hogy a partner tartalmazza az automatikusan megadott URL-címet, valamint a nemrég létrehozott ügyfél-hitelesítő adatokat.)</span><span class="sxs-lookup"><span data-stu-id="6d541-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="kapcsolat létrehozása":::

5. <span data-ttu-id="6d541-184">Az ügyfél e-mailben kap meghívót, és a paraméteres URL-címre kattint.</span><span class="sxs-lookup"><span data-stu-id="6d541-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="6d541-185">Az ügyfél az e-mailben megadott hitelesítő adatokat használja a felügyeleti Microsoft 365 való bejelentkezéshez.</span><span class="sxs-lookup"><span data-stu-id="6d541-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="6d541-186">Az ügyfél ellenőrzi a jelölőnégyzetet a **viszonteladói kapcsolat elfogadásához,** és **Microsoft Ügyfélszerződés.**</span><span class="sxs-lookup"><span data-stu-id="6d541-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="6d541-187">Ugyanazon az URL-címen belül az ügyfél láthatja azon partnerek összesített listáját, akiknél dolgozik.</span><span class="sxs-lookup"><span data-stu-id="6d541-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="6d541-188">Kiválaszthat egy partnert, hogy lássa a részleteket.</span><span class="sxs-lookup"><span data-stu-id="6d541-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Szerződés elfogadása":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="6d541-190">Meglévő ügyfél meghívása a szerződés felülvizsgálatára és elfogadására</span><span class="sxs-lookup"><span data-stu-id="6d541-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="6d541-191">Az alábbi lépésekkel meghívhat egy meglévő ügyfelet, hogy tekintse át és fogadja el Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="6d541-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="6d541-192">Hozza létre az ügyfél e-mail-címét a beágyazott URL-címmel, amely meghívja az ügyfelet, hogy fogadja Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="6d541-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="6d541-193">Az ügyfél e-mailben megkapja a meghívót, és a URL-címre [kattint.](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)</span><span class="sxs-lookup"><span data-stu-id="6d541-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="6d541-194">Az ügyfél a Felügyeleti központban adja meg Microsoft 365 hitelesítő adatait.</span><span class="sxs-lookup"><span data-stu-id="6d541-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="6d541-195">Az ügyfél a jelölőnégyzet be- és elfogadásával fogadja Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="6d541-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="6d541-196">Ugyanazon az URL-címen belül az ügyfél láthatja azon partnerek összesített listáját, akiknél dolgozik.</span><span class="sxs-lookup"><span data-stu-id="6d541-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="6d541-197">Kiválaszthat egy partnert, hogy lássa a részleteket.</span><span class="sxs-lookup"><span data-stu-id="6d541-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Ügyfél":::

>[!NOTE]
><span data-ttu-id="6d541-199">Bizonyos esetekben előfordulhat, hogy az ügyfelek nem tudják közvetlenül elfogadni a Microsoft Ügyfélszerződés.</span><span class="sxs-lookup"><span data-stu-id="6d541-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="6d541-200">Az ilyen helyzetekkel kapcsolatos további információkért olvassa el az alábbi két forgatókönyvet, ahol az ügyfél nevében kell igazolnia.</span><span class="sxs-lookup"><span data-stu-id="6d541-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="6d541-201">Két forgatókönyv, ahol az ügyfél nevében kell igazolnia</span><span class="sxs-lookup"><span data-stu-id="6d541-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="6d541-202">Két esetben előfordulhat, hogy az ügyfelek nem tudják közvetlenül elfogadni a Microsoft Ügyfélszerződés felügyeleti Microsoft 365 belül.</span><span class="sxs-lookup"><span data-stu-id="6d541-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="6d541-203">**1.** forgatókönyv: Egy meglévő ügyfél a következők bármelyikét megvásárolta egy meglévő partnerkapcsolaton keresztül: ajánlatok, szoftver- vagy szoftver-előfizetések, fenntartott példányok vagy Azure-csomag.</span><span class="sxs-lookup"><span data-stu-id="6d541-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="6d541-204">Az ügyfél most új vásárlást kísérel meg (kivéve az automatikus megújítást).</span><span class="sxs-lookup"><span data-stu-id="6d541-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="6d541-205">Amikor az ügyfél az URL-címre kattint, a következő üzenet jelenik meg: "Kérjük, forduljon a partneréhez, hogy erősítse meg a Microsoft Ügyfélszerződés."</span><span class="sxs-lookup"><span data-stu-id="6d541-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="6d541-206">**A megoldáshoz:** Az ügyfél nevében kell igazolnia.</span><span class="sxs-lookup"><span data-stu-id="6d541-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Képernyőkép Microsoft 365 Felügyeleti központ oldalról, amely arra kéri, hogy a partnerrel való partnerrel való megerősítést kérve erősítse meg a Microsoft Ügyfélszerződés.":::

<span data-ttu-id="6d541-208">**2. forgatókönyv:** Egy meglévő ügyfél az alábbi ajánlatok, szoftver- és szoftver-előfizetések, fenntartott példányok és Azure-csomag bármelyikét megvásárolta.</span><span class="sxs-lookup"><span data-stu-id="6d541-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="6d541-209">Az ügyfél most megpróbál új vásárlást vásárolni egy új partnerrel.</span><span class="sxs-lookup"><span data-stu-id="6d541-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="6d541-210">Amikor az ügyfél az Microsoft 365 Felügyeleti központ URL-címére kattint az új partnerkapcsolat és a szerződés elfogadásához, a következő üzenetet kapja: "Kérjük, forduljon a partneréhez, hogy erősítse meg az ügyfél Microsoft Ügyfélszerződés."</span><span class="sxs-lookup"><span data-stu-id="6d541-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="6d541-211">**A megoldáshoz:** Az ügyfél nevében kell igazolnia.</span><span class="sxs-lookup"><span data-stu-id="6d541-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="6d541-212">Annak ellenőrzése, hogy az ügyfél elfogadta-e a szerződést</span><span class="sxs-lookup"><span data-stu-id="6d541-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="6d541-213">Ha olyan meglévő ügyfél számára próbál új rendelést létrehozni, aki még nem erősítette meg korábban, a rendszer felszólítja, hogy töltse ki a megerősítést.</span><span class="sxs-lookup"><span data-stu-id="6d541-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="6d541-214">Ehhez a következő eljárást használhatja.</span><span class="sxs-lookup"><span data-stu-id="6d541-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="6d541-215">Adja meg **a** szerződést elfogadó felhasználó vezetéknevét, vezetéknevét, e-mail-címét és telefonszámát **(nem** kötelező). </span><span class="sxs-lookup"><span data-stu-id="6d541-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="6d541-216">A **Szerződés elfogadásának dátuma alatt** adja meg a megfelelő dátumot.</span><span class="sxs-lookup"><span data-stu-id="6d541-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="6d541-217">Ezt nem állíthatja be jövőbeli dátumra.</span><span class="sxs-lookup"><span data-stu-id="6d541-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="6d541-218">Válassza a **Mentés és folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6d541-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="6d541-219">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="6d541-219">Next steps</span></span>

- [<span data-ttu-id="6d541-220">A vállalati profil információinak ellenőrzése vagy frissítése</span><span class="sxs-lookup"><span data-stu-id="6d541-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="6d541-221">Microsoft Ügyfélszerződés (régió és nyelv szerint)</span><span class="sxs-lookup"><span data-stu-id="6d541-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
