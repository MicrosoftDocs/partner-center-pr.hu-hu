---
title: Partnerközpontfiók létrehozása
ms.topic: article
ms.date: 08/07/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Ismerje meg, hogy Microsoft Partner Network tagok hogyan hozhatnak létre partneri központot a hálózati előnyeiknek és kompetenciáinak kezeléséhez.
author: ParthP
ms.author: ParthP
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: e3f04708d3b7e2c86c88541931c120a6649674fb
ms.sourcegitcommit: 6b03ff400d1350db9696f9b457fcfe710310c5d3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/03/2020
ms.locfileid: "96570790"
---
# <a name="create-a-partner-center-account-to-manage-network-benefits-and-competencies"></a><span data-ttu-id="7a851-103">Partner Center-fiók létrehozása hálózati előnyök és kompetenciák kezeléséhez</span><span class="sxs-lookup"><span data-stu-id="7a851-103">Create a Partner Center account to manage network benefits and competencies</span></span>

<span data-ttu-id="7a851-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="7a851-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7a851-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="7a851-105">Global admin</span></span>
- <span data-ttu-id="7a851-106">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="7a851-106">Admin agent</span></span>

<span data-ttu-id="7a851-107">Ahhoz, hogy fiókot hozzon létre a partner Centerben, a vállalatnak a Microsoft Partner Network tagjának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="7a851-107">Before you can create an account on Partner Center, your company must be a member of the Microsoft Partner Network.</span></span> <span data-ttu-id="7a851-108">Ha még nem tagja a hálózatnak, [csatlakozhat most](https://partner.microsoft.com/commercial#).</span><span class="sxs-lookup"><span data-stu-id="7a851-108">If you're not already a member of the network, you can [join now](https://partner.microsoft.com/commercial#).</span></span> <span data-ttu-id="7a851-109">A partner Center-fiók létrehozása után tekintse meg ezt a rövid videót [az irányítópulton](https://vimeo.com/290338211).</span><span class="sxs-lookup"><span data-stu-id="7a851-109">After you create a Partner Center account, watch this short video [Discover your dashboard](https://vimeo.com/290338211).</span></span>

## <a name="get-a-work-email-address-before-setting-up-a-partner-center-account"></a><span data-ttu-id="7a851-110">Munkahelyi e-mail-cím beszerzése a partner Center-fiók beállítása előtt</span><span class="sxs-lookup"><span data-stu-id="7a851-110">Get a work email address before setting up a Partner Center account</span></span>

<span data-ttu-id="7a851-111">A vállalatnak egy e-mail-tartományt kell megvásárolnia ahhoz, hogy be tudja állítani a munkahelyi e-mail-címeket az alkalmazottak számára.</span><span class="sxs-lookup"><span data-stu-id="7a851-111">Your company needs to purchase an email domain in order for you to be able to set up work email addresses for your employees.</span></span> <span data-ttu-id="7a851-112">Működjön együtt az informatikai részleggel egy e-mail-tartomány megvásárlásához, mivel ez egy technikai folyamat.</span><span class="sxs-lookup"><span data-stu-id="7a851-112">Work with your IT department to buy an email domain since this is a technical process.</span></span> <span data-ttu-id="7a851-113">Az új e-mail-cím használatával beállíthatja az Azure AD-bérlőt és a partner Center-fiókját.</span><span class="sxs-lookup"><span data-stu-id="7a851-113">Use the new email to set up your Azure AD tenant and your Partner Center account.</span></span>

## <a name="get-started"></a><span data-ttu-id="7a851-114">Bevezetés</span><span class="sxs-lookup"><span data-stu-id="7a851-114">Get started</span></span>

<span data-ttu-id="7a851-115">Ahhoz, hogy fiókot hozzon létre a partner Centerben, a következő információkat kell megadnia.</span><span class="sxs-lookup"><span data-stu-id="7a851-115">To create an account on Partner Center, you'll need to have on hand the following information.</span></span> <span data-ttu-id="7a851-116">Az első lépések megkezdése előtt érdemes lehet néhány percet igénybe venni:</span><span class="sxs-lookup"><span data-stu-id="7a851-116">You may want to take a few minutes to gather these items before you get started:</span></span>

- <span data-ttu-id="7a851-117">Globális rendszergazdai munkahelyi e-mail cím.</span><span class="sxs-lookup"><span data-stu-id="7a851-117">Global administrator work email.</span></span>

- <span data-ttu-id="7a851-118">Ha nem biztos abban, hogy mi a munkahelyi fiókja, tekintse [meg a munkahelyi fiókját és a partneri központot](azure-active-directory-tenants-and-partner-center.md) , ha a vállalat nem rendelkezik munkahelyi fiókkal, létrehozhat egyet a fiók létrehozási folyamata során.</span><span class="sxs-lookup"><span data-stu-id="7a851-118">If you're not sure what your company's work account is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md) If your company doesn't have a work account, you can create one during the account creation process.</span></span> 

- <span data-ttu-id="7a851-119">A vállalat jogi üzleti neve és címe.</span><span class="sxs-lookup"><span data-stu-id="7a851-119">Your company's legal business name and address.</span></span>  

- <span data-ttu-id="7a851-120">Jogi szerződések aláírására szolgáló hatóság.</span><span class="sxs-lookup"><span data-stu-id="7a851-120">Authority to sign legal agreements.</span></span> <span data-ttu-id="7a851-121">Győződjön meg arról, hogy jogosult a jogi szerződések aláírására a vállalat nevében, mivel ezt a beléptetési folyamat során meg kell adnia.</span><span class="sxs-lookup"><span data-stu-id="7a851-121">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

- <span data-ttu-id="7a851-122">Az elsődleges kapcsolattartóként használni kívánt személy neve és vállalati e-mail-címe.</span><span class="sxs-lookup"><span data-stu-id="7a851-122">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="7a851-123">A vállalat biztonságának és adatvédelmének biztosítása érdekében e-mailben értesítjük az elsődleges kapcsolattartót annak ellenőrzéséhez, hogy (1) bejelentkezett-e a partner Center-fiókra, és hogy (2) Ez az e-mail-cím a vállalathoz tartozik-e.</span><span class="sxs-lookup"><span data-stu-id="7a851-123">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and that (2) this email address belongs to your company.</span></span> <span data-ttu-id="7a851-124">Miután az elsődleges kapcsolat ellenőrzi a saját e-mail-címét, folytatjuk a megadott információk áttekintését.</span><span class="sxs-lookup"><span data-stu-id="7a851-124">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

<span data-ttu-id="7a851-125">Ezt az információt a fiók létrehozási folyamata során ellenőrizzük.</span><span class="sxs-lookup"><span data-stu-id="7a851-125">We'll verify this information during the account creation process.</span></span> <span data-ttu-id="7a851-126">Az ellenőrzési folyamattal kapcsolatos információkért lásd: [Fiók ellenőrzése](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="7a851-126">For information on the verification process, see [Account verification](verification-responses.md)</span></span>
 
## <a name="create-a-partner-center-account"></a><span data-ttu-id="7a851-127">Partnerközpontfiók létrehozása</span><span class="sxs-lookup"><span data-stu-id="7a851-127">Create a Partner Center account</span></span>

1.  <span data-ttu-id="7a851-128">Tekintse át az **üdvözlőlapon** az információkat, majd kattintson a **tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="7a851-128">Review the information on the **Welcome** page and then select **Next**.</span></span>

2.  <span data-ttu-id="7a851-129">Jelentkezzen be globális rendszergazdaként a vállalata munkahelyi fiókjába.</span><span class="sxs-lookup"><span data-stu-id="7a851-129">Sign in as a global admin to your company's work account.</span></span> <span data-ttu-id="7a851-130">Ha nem biztos benne, hogy mi a vállalat munkahelyi fiókja, tekintse [meg a munkahelyi fiók és a partner központ](azure-active-directory-tenants-and-partner-center.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="7a851-130">If you're not sure what your company's work account   is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span>

    <span data-ttu-id="7a851-131">Ha tudja, hogy a vállalata munkahelyi e-mail-fiókkal rendelkezik, válassza **a bejelentkezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7a851-131">Select **Sign in** if you know your company has a work email account.</span></span> <span data-ttu-id="7a851-132">A következő lapon adja meg a vállalati munkahelyi fiók globális rendszergazdai hitelesítő adatait.</span><span class="sxs-lookup"><span data-stu-id="7a851-132">On the next page, enter global admin credentials for your company's work account.</span></span> 

    <span data-ttu-id="7a851-133">Ha a vállalat nem rendelkezik munkahelyi fiókkal, válassza a **Létrehozás** lehetőséget, ha most szeretné beállítani.</span><span class="sxs-lookup"><span data-stu-id="7a851-133">If your company doesn't have a work account, select **Create one** to set one up now.</span></span> <span data-ttu-id="7a851-134">A munkahelyi fiók létrehozása után jelentkezzen be az imént létrehozott munkahelyi fiók globális rendszergazdai hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="7a851-134">After creating a work account, sign in using your global admin credentials for the work account you just created.</span></span>

3.  <span data-ttu-id="7a851-135">Adja meg vagy frissítse a vállalata jogi üzleti profilját és az elsődleges kapcsolattartási adatait, majd válassza a **regisztrálás most** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7a851-135">Provide or update your company's legal business profile and primary contact information and then select **Enroll now**.</span></span> 

    <span data-ttu-id="7a851-136">Az elsődleges kapcsolattartónak a vállalatban lévő személynek kell lennie, akivel kapcsolatba léphet az alkalmazással (ez lehet Ön vagy egy másik személy a cégnél).</span><span class="sxs-lookup"><span data-stu-id="7a851-136">The primary contact should be the person in your company we can contact about your application (this can be you or another person in your company).</span></span> <span data-ttu-id="7a851-137">Ezt az információt arra is felhasználjuk, hogy ellenőrizze, hogy ez a személy működik-e a cégnél, és regisztrált-e a partner Center-fiókra.</span><span class="sxs-lookup"><span data-stu-id="7a851-137">We'll also use this information to verify that this person works at your company and has signed up for a Partner Center account.</span></span>

    > [!IMPORTANT]  
    > <span data-ttu-id="7a851-138">A vállalat biztonságának és adatvédelmének biztosítása érdekében e-mailben értesítjük az elsődleges kapcsolattartót annak ellenőrzéséhez, hogy (1) bejelentkezett-e a partner Center-fiókra, és (2) hogy ez az e-mail-cím a vállalathoz tartozik-e.</span><span class="sxs-lookup"><span data-stu-id="7a851-138">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and (2) that this email address belongs to your company.</span></span> <span data-ttu-id="7a851-139">Miután az elsődleges kapcsolat ellenőrzi a saját e-mail-címét, folytatjuk a megadott információk áttekintését.</span><span class="sxs-lookup"><span data-stu-id="7a851-139">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

4.  <span data-ttu-id="7a851-140">Olvassa el és fogadja el a feltételeket és kikötéseket a Microsoft Partner Network szerződésben.</span><span class="sxs-lookup"><span data-stu-id="7a851-140">Read and accept the terms and conditions in the Microsoft Partner Network agreement.</span></span> 

5.  <span data-ttu-id="7a851-141">Ellenőrizze, hogy hozzá lett-e adva a felügyeleti ügynök csoportjához.</span><span class="sxs-lookup"><span data-stu-id="7a851-141">Verify that you've been added to the admin agent group.</span></span> <span data-ttu-id="7a851-142">A fiók beállításának befejezéséhez, beleértve a más felhasználók hozzáadását is, rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="7a851-142">To finish setting up your account, including adding other users, you must have admin agent permissions.</span></span> <span data-ttu-id="7a851-143">Az engedélyek megtekintéséhez vagy frissítéséhez kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="7a851-143">Follow these steps to view or update your permissions:</span></span>

    <span data-ttu-id="7a851-144">a.</span><span class="sxs-lookup"><span data-stu-id="7a851-144">a.</span></span> <span data-ttu-id="7a851-145">A partner Center [irányítópultján](https://partner.microsoft.com/dashboard/home**)kattintson a **Beállítások** ikonra, majd válassza a **felhasználói kezelés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7a851-145">From the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home**), select the **Settings** icon and then select **User management**.</span></span>  

    <span data-ttu-id="7a851-146">b.</span><span class="sxs-lookup"><span data-stu-id="7a851-146">b.</span></span> <span data-ttu-id="7a851-147">Válassza ki a nevét a felhasználók listából, majd válassza a **felügyeleti ügynök** lehetőséget, ha még nincs kiválasztva.</span><span class="sxs-lookup"><span data-stu-id="7a851-147">Select your name from the users list and then select **Admin agent** if it's not already selected.</span></span> <span data-ttu-id="7a851-148">Válassza a **Frissítés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7a851-148">Select **Update**.</span></span>  

## <a name="view-mpn-account-details"></a><span data-ttu-id="7a851-149">MPN-fiók részleteinek megtekintése</span><span class="sxs-lookup"><span data-stu-id="7a851-149">View MPN account details</span></span>

<span data-ttu-id="7a851-150">A partner Center-fiók létrehozása után visszatérhet a partneri központba, és megtekintheti a fiókadatok különböző adatait.</span><span class="sxs-lookup"><span data-stu-id="7a851-150">Once you create a Partner Center account, you can return to Partner Center to see various account details.</span></span> <span data-ttu-id="7a851-151">Ezek közül sok a partneri központ [irányítópultjának](https://partner.microsoft.com/dashboard) **partner profil** lapján jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="7a851-151">Many of these appear on the **Partner profile** page in your Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

<span data-ttu-id="7a851-152">Ezek az adatok a következők:</span><span class="sxs-lookup"><span data-stu-id="7a851-152">Such details include:</span></span>

- <span data-ttu-id="7a851-153">Vállalata jogi üzleti profilja</span><span class="sxs-lookup"><span data-stu-id="7a851-153">Your company's legal business profile</span></span>

- <span data-ttu-id="7a851-154">Az MPN-AZONOSÍTÓval kapcsolatos információk</span><span class="sxs-lookup"><span data-stu-id="7a851-154">Information about your MPN ID</span></span>

- <span data-ttu-id="7a851-155">A regisztrált Microsoft-programhoz társított aktuális szerződésekre mutató hivatkozások</span><span class="sxs-lookup"><span data-stu-id="7a851-155">Links to current agreements associated with your enrolled Microsoft program</span></span>

  <span data-ttu-id="7a851-156">Ha például regisztrálva van az MPN programban, megjelenik az aktuális Microsoft Partner Network szerződésre mutató hivatkozás.</span><span class="sxs-lookup"><span data-stu-id="7a851-156">For example, if you are enrolled in the MPN program, you'll see a link to the current Microsoft Partner Network agreement.</span></span> <span data-ttu-id="7a851-157">Ha más partneri programokban van regisztrálva, például a Cloud Solution Provider (CSP) programhoz, a más szerződésekre mutató hivatkozásokat is láthat, például a Microsoft partneri szerződést.</span><span class="sxs-lookup"><span data-stu-id="7a851-157">If you're enrolled in other partner programs, like the Cloud Solution Provider (CSP) program, you may also see links to other agreements, such as the Microsoft Partner Agreement.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="7a851-158">Ezek a típusú hivatkozások akkor lehetnek hasznosak, ha szeretné áttekinteni, elérni vagy letölteni egy szerződést, vagy ellenőrizze az aláírásának dátumát.</span><span class="sxs-lookup"><span data-stu-id="7a851-158">Seeing these types of links may be useful if you ever want to review, access, or download an agreement, or, check the date it was signed.</span></span>

### <a name="how-to-view-account-details-or-view-and-download-the-mpn-agreement"></a><span data-ttu-id="7a851-159">A fiók adatainak megtekintése, illetve az MPN-szerződés megtekintése és letöltése</span><span class="sxs-lookup"><span data-stu-id="7a851-159">How to view account details or view and download the MPN agreement</span></span>

<span data-ttu-id="7a851-160">Az alábbi lépéseket követve megtekintheti a fiók adatait, vagy megtekintheti és letöltheti az MPN-szerződést:</span><span class="sxs-lookup"><span data-stu-id="7a851-160">Follow these steps to view account details or view and download the MPN agreement:</span></span>

1. <span data-ttu-id="7a851-161">A munkahelyi fiókja felhasználónevének és jelszavának használatával jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="7a851-161">Using your work account username and password, sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="7a851-162">Megjelenik egy áttekintő oldal.</span><span class="sxs-lookup"><span data-stu-id="7a851-162">An Overview page appears.</span></span> <span data-ttu-id="7a851-163">(Ha nem látja az Áttekintés lapot, válassza a bal oldali navigációs menü **Áttekintés** elemét.)</span><span class="sxs-lookup"><span data-stu-id="7a851-163">(If you do not see the Overview page, select **Overview** from the left-navigation menu.)</span></span>

3. <span data-ttu-id="7a851-164">Válassza a fogaskerék ikont az irányítópult jobb felső sarkában, majd válassza a **partner beállításai** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7a851-164">Select the Gear icon in the top-right corner of the dashboard, then select **Partner settings**.</span></span> <span data-ttu-id="7a851-165">Ekkor megjelenik a partner profilja oldal.</span><span class="sxs-lookup"><span data-stu-id="7a851-165">This takes you to the Partner profile page.</span></span>

4. <span data-ttu-id="7a851-166">A partner Profile lapon különböző területek jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="7a851-166">From the Partner profile page, you'll see different areas.</span></span> <span data-ttu-id="7a851-167">Ezek közé tartozik a **jogi üzleti profil** és a **program információs** részlege.</span><span class="sxs-lookup"><span data-stu-id="7a851-167">These include a **Legal business profile** area and a **Program info** area.</span></span>

5. <span data-ttu-id="7a851-168">A **program adatai** területen keresse meg az **MPN program állapota** mezőt.</span><span class="sxs-lookup"><span data-stu-id="7a851-168">Under **Program info**, locate the **MPN program status** field.</span></span> <span data-ttu-id="7a851-169">Ez megjeleníti a Microsoft Partner Network-szerződésre mutató hivatkozást.</span><span class="sxs-lookup"><span data-stu-id="7a851-169">This displays a link to your Microsoft Partner Network agreement.</span></span> <span data-ttu-id="7a851-170">Emellett leírja a programban aktuális állapotát is.</span><span class="sxs-lookup"><span data-stu-id="7a851-170">It also describes your current status in the program.</span></span>


   :::image type="content" source="images/accountsettings/mpn-program-info-download-mpn-agreement.png" alt-text="Kép: a partner profilja oldalon található program információi területe egy piros mező, amely az MPN program állapota mezőt emeli ki ezen a területen, valamint a hozzá tartozó hivatkozást a Microsoft Partner Network szerződéshez.":::

6. <span data-ttu-id="7a851-172">A szerződés megtekintéséhez vagy letöltéséhez válassza **Microsoft Partner Network szerződést**.</span><span class="sxs-lookup"><span data-stu-id="7a851-172">To view or download this agreement, select **Microsoft Partner Network agreement**.</span></span>  

> [!NOTE]
> <span data-ttu-id="7a851-173">A fenti lépésekkel más, regisztrált programok, például a Microsoft partneri szerződés esetében is megtekintheti és letöltheti a más szerződéseket, ha azok regisztrálva vannak a Cloud Solution Provider (CSP) programban.</span><span class="sxs-lookup"><span data-stu-id="7a851-173">You can also use the above steps to view or download other agreements for other, enrolled programs, such as the Microsoft Partner Agreement if you happen to be enrolled in the Cloud Solution Provider (CSP) program.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7a851-174">További lépések</span><span class="sxs-lookup"><span data-stu-id="7a851-174">Next steps</span></span>

-   [<span data-ttu-id="7a851-175">Felhasználói fiókok hozzáadása és engedélyek kiosztása</span><span class="sxs-lookup"><span data-stu-id="7a851-175">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-   [<span data-ttu-id="7a851-176">Microsoft Action Pack-előfizetés vásárlása vagy megújítása</span><span class="sxs-lookup"><span data-stu-id="7a851-176">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-   [<span data-ttu-id="7a851-177">Tagsági előnyök kezelése</span><span class="sxs-lookup"><span data-stu-id="7a851-177">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-   [<span data-ttu-id="7a851-178">Ismerje meg az arany-és ezüst-tagságra vonatkozó kompetenciával kapcsolatos követelményeket</span><span class="sxs-lookup"><span data-stu-id="7a851-178">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-   [<span data-ttu-id="7a851-179">Üzleti profil létrehozása a potenciális vásárlók figyelmének felkeltéséhez a Microsofton keresztül</span><span class="sxs-lookup"><span data-stu-id="7a851-179">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-   [<span data-ttu-id="7a851-180">Értékesítési érdeklődők beszerzése és kezelése a Microsofttól</span><span class="sxs-lookup"><span data-stu-id="7a851-180">Get and manage sales leads from Microsoft</span></span>](manage-leads.md)
