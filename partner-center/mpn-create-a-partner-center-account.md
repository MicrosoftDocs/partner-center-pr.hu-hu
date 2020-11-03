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
ms.openlocfilehash: f94b11c4feb9cd1bedd97bebc537a504f9c4d127
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528482"
---
# <a name="create-a-partner-center-account-to-manage-network-benefits-and-competencies"></a><span data-ttu-id="1f6f7-103">Partner Center-fiók létrehozása hálózati előnyök és kompetenciák kezeléséhez</span><span class="sxs-lookup"><span data-stu-id="1f6f7-103">Create a Partner Center account to manage network benefits and competencies</span></span>

<span data-ttu-id="1f6f7-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="1f6f7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1f6f7-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="1f6f7-105">Global admin</span></span>
- <span data-ttu-id="1f6f7-106">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="1f6f7-106">Admin agent</span></span>

<span data-ttu-id="1f6f7-107">Ahhoz, hogy fiókot hozzon létre a partner Centerben, a vállalatnak a Microsoft Partner Network tagjának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-107">Before you can create an account on Partner Center, your company must be a member of the Microsoft Partner Network.</span></span> <span data-ttu-id="1f6f7-108">Ha még nem tagja a hálózatnak, [csatlakozhat most](https://partner.microsoft.com/commercial#).</span><span class="sxs-lookup"><span data-stu-id="1f6f7-108">If you're not already a member of the network, you can [join now](https://partner.microsoft.com/commercial#).</span></span> <span data-ttu-id="1f6f7-109">A partner Center-fiók létrehozása után tekintse meg ezt a rövid videót [az irányítópulton](https://vimeo.com/290338211).</span><span class="sxs-lookup"><span data-stu-id="1f6f7-109">After you create a Partner Center account, watch this short video [Discover your dashboard](https://vimeo.com/290338211).</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="1f6f7-110">Előkészületek</span><span class="sxs-lookup"><span data-stu-id="1f6f7-110">Before you begin</span></span>

<span data-ttu-id="1f6f7-111">Ahhoz, hogy fiókot hozzon létre a partner Centerben, a következő információkat kell megadnia.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-111">To create an account on Partner Center, you'll need to have on hand the following information.</span></span> <span data-ttu-id="1f6f7-112">Az első lépések megkezdése előtt érdemes lehet néhány percet igénybe venni:</span><span class="sxs-lookup"><span data-stu-id="1f6f7-112">You may want to take a few minutes to gather these items before you get started:</span></span>

-   <span data-ttu-id="1f6f7-113">Globális rendszergazdai munkahelyi e-mail cím.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-113">Global administrator work email.</span></span>

-   <span data-ttu-id="1f6f7-114">Ha nem biztos abban, hogy mi a munkahelyi fiókja, tekintse [meg a munkahelyi fiókját és a partneri központot](azure-active-directory-tenants-and-partner-center.md) , ha a vállalat nem rendelkezik munkahelyi fiókkal, létrehozhat egyet a fiók létrehozási folyamata során.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-114">If you're not sure what your company's work account is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md) If your company doesn't have a work account, you can create one during the account creation process.</span></span> 

-   <span data-ttu-id="1f6f7-115">A vállalat jogi üzleti neve és címe.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-115">Your company's legal business name and address.</span></span>  

-   <span data-ttu-id="1f6f7-116">Jogi szerződések aláírására szolgáló hatóság.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-116">Authority to sign legal agreements.</span></span> <span data-ttu-id="1f6f7-117">Győződjön meg arról, hogy jogosult a jogi szerződések aláírására a vállalat nevében, mivel ezt a beléptetési folyamat során meg kell adnia.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-117">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

-   <span data-ttu-id="1f6f7-118">Az elsődleges kapcsolattartóként használni kívánt személy neve és vállalati e-mail-címe.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-118">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="1f6f7-119">A vállalat biztonságának és adatvédelmének biztosítása érdekében e-mailben értesítjük az elsődleges kapcsolattartót annak ellenőrzéséhez, hogy (1) bejelentkezett-e a partner Center-fiókra, és hogy (2) Ez az e-mail-cím a vállalathoz tartozik-e.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-119">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and that (2) this email address belongs to your company.</span></span> <span data-ttu-id="1f6f7-120">Miután az elsődleges kapcsolat ellenőrzi a saját e-mail-címét, folytatjuk a megadott információk áttekintését.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-120">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

<span data-ttu-id="1f6f7-121">Ezt az információt a fiók létrehozási folyamata során ellenőrizzük.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-121">We'll verify this information during the account creation process.</span></span> 
 
## <a name="create-a-partner-center-account"></a><span data-ttu-id="1f6f7-122">Partnerközpontfiók létrehozása</span><span class="sxs-lookup"><span data-stu-id="1f6f7-122">Create a Partner Center account</span></span>

1.  <span data-ttu-id="1f6f7-123">Tekintse át az **üdvözlőlapon** az információkat, majd kattintson a **tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-123">Review the information on the **Welcome** page and then select **Next** .</span></span>

2.  <span data-ttu-id="1f6f7-124">Jelentkezzen be globális rendszergazdaként a vállalata munkahelyi fiókjába.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-124">Sign in as a global admin to your company's work account.</span></span> <span data-ttu-id="1f6f7-125">Ha nem biztos benne, hogy mi a vállalat munkahelyi fiókja, tekintse [meg a munkahelyi fiók és a partner központ](azure-active-directory-tenants-and-partner-center.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-125">If you're not sure what your company's work account   is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span>

    <span data-ttu-id="1f6f7-126">Ha tudja, hogy a vállalata munkahelyi e-mail-fiókkal rendelkezik, válassza **a bejelentkezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-126">Select **Sign in** if you know your company has a work email account.</span></span> <span data-ttu-id="1f6f7-127">A következő lapon adja meg a vállalati munkahelyi fiók globális rendszergazdai hitelesítő adatait.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-127">On the next page, enter global admin credentials for your company's work account.</span></span> 

    <span data-ttu-id="1f6f7-128">Ha a vállalat nem rendelkezik munkahelyi fiókkal, válassza a **Létrehozás** lehetőséget, ha most szeretné beállítani.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-128">If your company doesn't have a work account, select **Create one** to set one up now.</span></span> <span data-ttu-id="1f6f7-129">A munkahelyi fiók létrehozása után jelentkezzen be az imént létrehozott munkahelyi fiók globális rendszergazdai hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-129">After creating a work account, sign in using your global admin credentials for the work account you just created.</span></span>

3.  <span data-ttu-id="1f6f7-130">Adja meg vagy frissítse a vállalata jogi üzleti profilját és az elsődleges kapcsolattartási adatait, majd válassza a **regisztrálás most** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-130">Provide or update your company's legal business profile and primary contact information and then select **Enroll now** .</span></span> 

    <span data-ttu-id="1f6f7-131">Az elsődleges kapcsolattartónak a vállalatban lévő személynek kell lennie, akivel kapcsolatba léphet az alkalmazással (ez lehet Ön vagy egy másik személy a cégnél).</span><span class="sxs-lookup"><span data-stu-id="1f6f7-131">The primary contact should be the person in your company we can contact about your application (this can be you or another person in your company).</span></span> <span data-ttu-id="1f6f7-132">Ezt az információt arra is felhasználjuk, hogy ellenőrizze, hogy ez a személy működik-e a cégnél, és regisztrált-e a partner Center-fiókra.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-132">We'll also use this information to verify that this person works at your company and has signed up for a Partner Center account.</span></span>

    > [!IMPORTANT]  
    > <span data-ttu-id="1f6f7-133">A vállalat biztonságának és adatvédelmének biztosítása érdekében e-mailben értesítjük az elsődleges kapcsolattartót annak ellenőrzéséhez, hogy (1) bejelentkezett-e a partner Center-fiókra, és (2) hogy ez az e-mail-cím a vállalathoz tartozik-e.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-133">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and (2) that this email address belongs to your company.</span></span> <span data-ttu-id="1f6f7-134">Miután az elsődleges kapcsolat ellenőrzi a saját e-mail-címét, folytatjuk a megadott információk áttekintését.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-134">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

4.  <span data-ttu-id="1f6f7-135">Olvassa el és fogadja el a feltételeket és kikötéseket a Microsoft Partner Network szerződésben.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-135">Read and accept the terms and conditions in the Microsoft Partner Network agreement.</span></span> 

5.  <span data-ttu-id="1f6f7-136">Ellenőrizze, hogy hozzá lett-e adva a felügyeleti ügynök csoportjához.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-136">Verify that you've been added to the admin agent group.</span></span> <span data-ttu-id="1f6f7-137">A fiók beállításának befejezéséhez, beleértve a más felhasználók hozzáadását is, rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-137">To finish setting up your account, including adding other users, you must have admin agent permissions.</span></span> <span data-ttu-id="1f6f7-138">Az engedélyek megtekintéséhez vagy frissítéséhez kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="1f6f7-138">Follow these steps to view or update your permissions:</span></span>

    <span data-ttu-id="1f6f7-139">a.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-139">a.</span></span> <span data-ttu-id="1f6f7-140">A partner Center [irányítópultján](https://partner.microsoft.com/dashboard/home**)kattintson a **Beállítások** ikonra, majd válassza a **felhasználói kezelés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-140">From the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home**), select the **Settings** icon and then select **User management** .</span></span>  

    <span data-ttu-id="1f6f7-141">b.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-141">b.</span></span> <span data-ttu-id="1f6f7-142">Válassza ki a nevét a felhasználók listából, majd válassza a **felügyeleti ügynök** lehetőséget, ha még nincs kiválasztva.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-142">Select your name from the users list and then select **Admin agent** if it's not already selected.</span></span> <span data-ttu-id="1f6f7-143">Válassza a **Frissítés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-143">Select **Update** .</span></span>  

## <a name="view-mpn-account-details"></a><span data-ttu-id="1f6f7-144">MPN-fiók részleteinek megtekintése</span><span class="sxs-lookup"><span data-stu-id="1f6f7-144">View MPN account details</span></span>

<span data-ttu-id="1f6f7-145">A partner Center-fiók létrehozása után visszatérhet a partneri központba, és megtekintheti a fiókadatok különböző adatait.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-145">Once you create a Partner Center account, you can return to Partner Center to see various account details.</span></span> <span data-ttu-id="1f6f7-146">Ezek közül sok a partneri központ [irányítópultjának](https://partner.microsoft.com/dashboard) **partner profil** lapján jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-146">Many of these appear on the **Partner profile** page in your Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

<span data-ttu-id="1f6f7-147">Ezek az adatok a következők:</span><span class="sxs-lookup"><span data-stu-id="1f6f7-147">Such details include:</span></span>

- <span data-ttu-id="1f6f7-148">Vállalata jogi üzleti profilja</span><span class="sxs-lookup"><span data-stu-id="1f6f7-148">Your company's legal business profile</span></span>

- <span data-ttu-id="1f6f7-149">Az MPN-AZONOSÍTÓval kapcsolatos információk</span><span class="sxs-lookup"><span data-stu-id="1f6f7-149">Information about your MPN ID</span></span>

- <span data-ttu-id="1f6f7-150">A regisztrált Microsoft-programhoz társított aktuális szerződésekre mutató hivatkozások</span><span class="sxs-lookup"><span data-stu-id="1f6f7-150">Links to current agreements associated with your enrolled Microsoft program</span></span>

  <span data-ttu-id="1f6f7-151">Ha például regisztrálva van az MPN programban, megjelenik az aktuális Microsoft Partner Network szerződésre mutató hivatkozás.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-151">For example, if you are enrolled in the MPN program, you'll see a link to the current Microsoft Partner Network agreement.</span></span> <span data-ttu-id="1f6f7-152">Ha más partneri programokban van regisztrálva, például a Cloud Solution Provider (CSP) programhoz, a más szerződésekre mutató hivatkozásokat is láthat, például a Microsoft partneri szerződést.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-152">If you're enrolled in other partner programs, like the Cloud Solution Provider (CSP) program, you may also see links to other agreements, such as the Microsoft Partner Agreement.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="1f6f7-153">Ezek a típusú hivatkozások akkor lehetnek hasznosak, ha szeretné áttekinteni, elérni vagy letölteni egy szerződést, vagy ellenőrizze az aláírásának dátumát.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-153">Seeing these types of links may be useful if you ever want to review, access, or download an agreement, or, check the date it was signed.</span></span>

### <a name="how-to-view-account-details-or-view-and-download-the-mpn-agreement"></a><span data-ttu-id="1f6f7-154">A fiók adatainak megtekintése, illetve az MPN-szerződés megtekintése és letöltése</span><span class="sxs-lookup"><span data-stu-id="1f6f7-154">How to view account details or view and download the MPN agreement</span></span>

<span data-ttu-id="1f6f7-155">Az alábbi lépéseket követve megtekintheti a fiók adatait, vagy megtekintheti és letöltheti az MPN-szerződést:</span><span class="sxs-lookup"><span data-stu-id="1f6f7-155">Follow these steps to view account details or view and download the MPN agreement:</span></span>

1. <span data-ttu-id="1f6f7-156">A munkahelyi fiókja felhasználónevének és jelszavának használatával jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="1f6f7-156">Using your work account username and password, sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1f6f7-157">Megjelenik egy áttekintő oldal.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-157">An Overview page appears.</span></span> <span data-ttu-id="1f6f7-158">(Ha nem látja az Áttekintés lapot, válassza a bal oldali navigációs menü **Áttekintés** elemét.)</span><span class="sxs-lookup"><span data-stu-id="1f6f7-158">(If you do not see the Overview page, select **Overview** from the left-navigation menu.)</span></span>

3. <span data-ttu-id="1f6f7-159">Válassza a fogaskerék ikont az irányítópult jobb felső sarkában, majd válassza a **partner beállításai** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-159">Select the Gear icon in the top-right corner of the dashboard, then select **Partner settings** .</span></span> <span data-ttu-id="1f6f7-160">Ekkor megjelenik a partner profilja oldal.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-160">This takes you to the Partner profile page.</span></span>

4. <span data-ttu-id="1f6f7-161">A partner Profile lapon különböző területek jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-161">From the Partner profile page, you'll see different areas.</span></span> <span data-ttu-id="1f6f7-162">Ezek közé tartozik a **jogi üzleti profil** és a **program információs** részlege.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-162">These include a **Legal business profile** area and a **Program info** area.</span></span>

5. <span data-ttu-id="1f6f7-163">A **program adatai** területen keresse meg az **MPN program állapota** mezőt.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-163">Under **Program info** , locate the **MPN program status** field.</span></span> <span data-ttu-id="1f6f7-164">Ez megjeleníti a Microsoft Partner Network-szerződésre mutató hivatkozást.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-164">This displays a link to your Microsoft Partner Network agreement.</span></span> <span data-ttu-id="1f6f7-165">Emellett leírja a programban aktuális állapotát is.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-165">It also describes your current status in the program.</span></span>


   :::image type="content" source="images/accountsettings/mpn-program-info-download-mpn-agreement.png" alt-text="Kép: a partner profilja oldalon található program információi területe egy piros mező, amely az MPN program állapota mezőt emeli ki ezen a területen, valamint a hozzá tartozó hivatkozást a Microsoft Partner Network szerződéshez.":::

6. <span data-ttu-id="1f6f7-167">A szerződés megtekintéséhez vagy letöltéséhez válassza **Microsoft Partner Network szerződést** .</span><span class="sxs-lookup"><span data-stu-id="1f6f7-167">To view or download this agreement, select **Microsoft Partner Network agreement** .</span></span>  

> [!NOTE]
> <span data-ttu-id="1f6f7-168">A fenti lépésekkel más, regisztrált programok, például a Microsoft partneri szerződés esetében is megtekintheti és letöltheti a más szerződéseket, ha azok regisztrálva vannak a Cloud Solution Provider (CSP) programban.</span><span class="sxs-lookup"><span data-stu-id="1f6f7-168">You can also use the above steps to view or download other agreements for other, enrolled programs, such as the Microsoft Partner Agreement if you happen to be enrolled in the Cloud Solution Provider (CSP) program.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1f6f7-169">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="1f6f7-169">Next steps</span></span>

-   [<span data-ttu-id="1f6f7-170">Felhasználói fiókok hozzáadása és engedélyek kiosztása</span><span class="sxs-lookup"><span data-stu-id="1f6f7-170">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-   [<span data-ttu-id="1f6f7-171">Microsoft Action Pack-előfizetés vásárlása vagy megújítása</span><span class="sxs-lookup"><span data-stu-id="1f6f7-171">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-   [<span data-ttu-id="1f6f7-172">Tagsági előnyök kezelése</span><span class="sxs-lookup"><span data-stu-id="1f6f7-172">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-   [<span data-ttu-id="1f6f7-173">Ismerje meg az arany-és ezüst-tagságra vonatkozó kompetenciával kapcsolatos követelményeket</span><span class="sxs-lookup"><span data-stu-id="1f6f7-173">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-   [<span data-ttu-id="1f6f7-174">Üzleti profil létrehozása a potenciális vásárlók figyelmének felkeltéséhez a Microsofton keresztül</span><span class="sxs-lookup"><span data-stu-id="1f6f7-174">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-   [<span data-ttu-id="1f6f7-175">Értékesítési érdeklődők beszerzése és kezelése a Microsofttól</span><span class="sxs-lookup"><span data-stu-id="1f6f7-175">Get and manage sales leads from Microsoft</span></span>](manage-leads.md)
