---
title: A Power BI a partner Center Analytics telepítése
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A cikk lépéseit követve telepítse és tekintse meg a partner Center Analytics alkalmazást a Power BIhoz (közvetlen partnerek számára a CSP-ben).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 64467ec608c2ca87dbc2b7d5dfb02adb08f13c18
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/14/2020
ms.locfileid: "92527975"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="6fb9b-103">A Partnerközpont adatelemzési alkalmazás a Microsoft Power BI-hoz telepítése és előzetes verziója</span><span class="sxs-lookup"><span data-stu-id="6fb9b-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="6fb9b-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="6fb9b-104">**Applies to**</span></span>

- <span data-ttu-id="6fb9b-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="6fb9b-105">Partner Center</span></span>

<span data-ttu-id="6fb9b-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="6fb9b-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="6fb9b-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="6fb9b-107">Global admin</span></span>
-   <span data-ttu-id="6fb9b-108">Felhasználói rendszergazda</span><span class="sxs-lookup"><span data-stu-id="6fb9b-108">User admin</span></span>
-   <span data-ttu-id="6fb9b-109">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="6fb9b-109">Sales agent</span></span>
-   <span data-ttu-id="6fb9b-110">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="6fb9b-110">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="6fb9b-111">Előkészületek</span><span class="sxs-lookup"><span data-stu-id="6fb9b-111">Before you begin</span></span>

<span data-ttu-id="6fb9b-112">Válassza ki a vállalata számára leginkább megfelelő alkalmazást az elérhető Power BI alkalmazások alábbi listájából:</span><span class="sxs-lookup"><span data-stu-id="6fb9b-112">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>
- [<span data-ttu-id="6fb9b-113">Közvetlen szolgáltató</span><span class="sxs-lookup"><span data-stu-id="6fb9b-113">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="6fb9b-114">Közvetett szolgáltató</span><span class="sxs-lookup"><span data-stu-id="6fb9b-114">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="6fb9b-115">Közvetett viszonteladó</span><span class="sxs-lookup"><span data-stu-id="6fb9b-115">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="6fb9b-116">A partner Center Analytics-alkalmazás előzetes verziójának telepítése előtt győződjön meg arról, hogy megfelel az alábbi követelményeknek.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-116">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="6fb9b-117">Kiválaszthatja a vállalata számára megfelelő Power BI alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-117">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="6fb9b-118">Power BI Pro-licenccel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-118">You have a Power BI pro license.</span></span>

- <span data-ttu-id="6fb9b-119">Rendelkezik a sablon alkalmazásainak a bérlőre való telepítéséhez szükséges engedélyekkel.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-119">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="6fb9b-120">Bejelentkezhet Power BIba.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-120">You can sign in to Power BI.</span></span>

- <span data-ttu-id="6fb9b-121">A [vállalat Azure Active Directory (Azure ad) bérlője](azure-active-directory-tenants-and-partner-center.md)globális rendszergazdaként, rendszergazdai ügynökként vagy számlázási rendszergazdaként is bejelentkezhet.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-121">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="6fb9b-122">Az alkalmazás telepítése</span><span class="sxs-lookup"><span data-stu-id="6fb9b-122">To install the app</span></span>

1. <span data-ttu-id="6fb9b-123">Kattintson az adott alkalmazás forrás hivatkozására (közvetlen szolgáltató/közvetett szolgáltató/közvetett viszonteladó) a fenti szakaszban.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-123">Click on the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="6fb9b-124">Kattintson a **Letöltés most** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-124">Click on **GET IT NOW** .</span></span> 

3. <span data-ttu-id="6fb9b-125">A **Folytatás** gombra kattintva fogadja el a feltételeket és a kikötéseket.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-125">Agree terms and conditions by clicking **Continue** .</span></span>

4. <span data-ttu-id="6fb9b-126">Már van fiókja? válassza **a bejelentkezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-126">Under Already have an account? select **Sign In** .</span></span>

5. <span data-ttu-id="6fb9b-127">A következő lapon adja meg Power BI felhasználónevét és jelszavát, majd válassza a bejelentkezés lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-127">On the next page, enter your Power BI user name and password and then select Sign In.</span></span>

6. <span data-ttu-id="6fb9b-128">A munkaterület nevének megadásával telepítse a munkaterületet.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-128">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="6fb9b-129">Megtalálhatja az alkalmazások szakaszban telepített sablonok alkalmazásait.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-129">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="6fb9b-130">Kattintson az alkalmazások elemre, és válassza ki a telepített alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-130">Click on Apps and choose the installed apps.</span></span>

9. <span data-ttu-id="6fb9b-131">Megnyílik az új alkalmazás képernyője.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-131">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="6fb9b-132">Az adatkapcsolathoz kattintson a **Kapcsolódás** gombra.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-132">To connect to the data Click **Connect** .</span></span>

11. <span data-ttu-id="6fb9b-133">A **Kapcsolódás a partneri központ Analytics** előugró ablakhoz lapon ellenőrizze, hogy a **hitelesítési módszer** a **oAuth2** értékre van-e állítva, vagy válassza a **oAuth2** lehetőséget a listából, ha nem.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-133">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="6fb9b-134">Ez az ablak néhány percig is eltarthat.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-134">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="6fb9b-135">A **partner Center Analytics-összekötő** lapon jelentkezzen be a vállalati Azure ad-bérlőhöz a globális rendszergazda, a rendszergazdai ügynök vagy a számlázási rendszergazdai hitelesítő adatokkal, majd válassza a **Bejelentkezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-135">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In** .</span></span>
 
13. <span data-ttu-id="6fb9b-136">Amikor a rendszer kéri a hozzáférést, válassza az **elfogadás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-136">When prompted for access, select **Accept** .</span></span> 

<span data-ttu-id="6fb9b-137">Miután a partner Center Analytics szolgáltatás csatlakozott a Power BIhoz, a rendszer betölti az adatgyűjtést.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-137">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="6fb9b-138">Az adatmennyiségtől függően ez akár 10 percet is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-138">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="6fb9b-139">Az adatbetöltések befejezése után elkezdheti a partner Center Analytics alkalmazás irányítópultjának és jelentéseinek használatát Power BI.</span><span class="sxs-lookup"><span data-stu-id="6fb9b-139">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6fb9b-140">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="6fb9b-140">Next steps</span></span>

[<span data-ttu-id="6fb9b-141">Üzleti adatai megtekinthetők a Microsoft Power BI partner Center Analytics alkalmazásával</span><span class="sxs-lookup"><span data-stu-id="6fb9b-141">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
