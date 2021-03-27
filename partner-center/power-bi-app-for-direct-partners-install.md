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
ms.openlocfilehash: ad0c2f3ee7d130c49dea6ba354e6794e29fd9e9f
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633692"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="796ce-103">A Partnerközpont adatelemzési alkalmazás a Microsoft Power BI-hoz telepítése és előzetes verziója</span><span class="sxs-lookup"><span data-stu-id="796ce-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>


<span data-ttu-id="796ce-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="796ce-104">**Appropriate roles**</span></span>

- <span data-ttu-id="796ce-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="796ce-105">Global admin</span></span>
- <span data-ttu-id="796ce-106">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="796ce-106">User management admin</span></span>
- <span data-ttu-id="796ce-107">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="796ce-107">Sales agent</span></span>
- <span data-ttu-id="796ce-108">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="796ce-108">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="796ce-109">Előkészületek</span><span class="sxs-lookup"><span data-stu-id="796ce-109">Before you begin</span></span>

<span data-ttu-id="796ce-110">Válassza ki a vállalata számára leginkább megfelelő alkalmazást az elérhető Power BI alkalmazások alábbi listájából:</span><span class="sxs-lookup"><span data-stu-id="796ce-110">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>

- [<span data-ttu-id="796ce-111">Közvetlen szolgáltató</span><span class="sxs-lookup"><span data-stu-id="796ce-111">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="796ce-112">Közvetett szolgáltató</span><span class="sxs-lookup"><span data-stu-id="796ce-112">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="796ce-113">Közvetett viszonteladó</span><span class="sxs-lookup"><span data-stu-id="796ce-113">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="796ce-114">A partner Center Analytics-alkalmazás előzetes verziójának telepítése előtt győződjön meg arról, hogy megfelel az alábbi követelményeknek.</span><span class="sxs-lookup"><span data-stu-id="796ce-114">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="796ce-115">Kiválaszthatja a vállalata számára megfelelő Power BI alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="796ce-115">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="796ce-116">Power BI Pro-licenccel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="796ce-116">You have a Power BI pro license.</span></span>

- <span data-ttu-id="796ce-117">Rendelkezik a sablon alkalmazásainak a bérlőre való telepítéséhez szükséges engedélyekkel.</span><span class="sxs-lookup"><span data-stu-id="796ce-117">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="796ce-118">Bejelentkezhet Power BIba.</span><span class="sxs-lookup"><span data-stu-id="796ce-118">You can sign in to Power BI.</span></span>

- <span data-ttu-id="796ce-119">A [vállalat Azure Active Directory (Azure ad) bérlője](azure-active-directory-tenants-and-partner-center.md)globális rendszergazdaként, rendszergazdai ügynökként vagy számlázási rendszergazdaként is bejelentkezhet.</span><span class="sxs-lookup"><span data-stu-id="796ce-119">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="796ce-120">Az alkalmazás telepítése</span><span class="sxs-lookup"><span data-stu-id="796ce-120">To install the app</span></span>

1. <span data-ttu-id="796ce-121">Válassza ki az adott alkalmazás forrásának hivatkozását (közvetlen szolgáltató/közvetett szolgáltató/közvetett viszonteladó) a fenti szakaszban.</span><span class="sxs-lookup"><span data-stu-id="796ce-121">Select the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="796ce-122">Válassza a **Letöltés most** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="796ce-122">Select **GET IT NOW**.</span></span> 

3. <span data-ttu-id="796ce-123">A **Folytatás** gombra kattintva fogadja el a feltételeket és a kikötéseket.</span><span class="sxs-lookup"><span data-stu-id="796ce-123">Agree terms and conditions by selecting **Continue**.</span></span>

4. <span data-ttu-id="796ce-124">Már van fiókja? válassza **a bejelentkezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="796ce-124">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="796ce-125">A következő lapon adja meg Power BI felhasználónevét és jelszavát, majd válassza a **Bejelentkezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="796ce-125">On the next page, enter your Power BI user name and password and then select **Sign In**.</span></span>

6. <span data-ttu-id="796ce-126">A munkaterület nevének megadásával telepítse a munkaterületet.</span><span class="sxs-lookup"><span data-stu-id="796ce-126">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="796ce-127">Megtalálhatja az alkalmazások szakaszban telepített sablonok alkalmazásait.</span><span class="sxs-lookup"><span data-stu-id="796ce-127">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="796ce-128">Válassza az **alkalmazások** lehetőséget, és válassza ki a telepített alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="796ce-128">Select **Apps** and choose the installed apps.</span></span>

9. <span data-ttu-id="796ce-129">Megnyílik az új alkalmazás képernyője.</span><span class="sxs-lookup"><span data-stu-id="796ce-129">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="796ce-130">Az adatkapcsolathoz válassza a **Kapcsolódás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="796ce-130">To connect to the data, select **Connect**.</span></span>

11. <span data-ttu-id="796ce-131">A **Kapcsolódás a partneri központ Analytics** előugró ablakhoz lapon ellenőrizze, hogy a **hitelesítési módszer** a **oAuth2** értékre van-e állítva, vagy válassza a **oAuth2** lehetőséget a listából, ha nem.</span><span class="sxs-lookup"><span data-stu-id="796ce-131">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="796ce-132">Ez az ablak néhány percig is eltarthat.</span><span class="sxs-lookup"><span data-stu-id="796ce-132">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="796ce-133">A **partner Center Analytics-összekötő** lapon jelentkezzen be a vállalati Azure ad-bérlőhöz a globális rendszergazda, a rendszergazdai ügynök vagy a számlázási rendszergazdai hitelesítő adatokkal, majd válassza a **Bejelentkezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="796ce-133">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="796ce-134">Amikor a rendszer kéri a hozzáférést, válassza az **elfogadás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="796ce-134">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="796ce-135">Miután a partner Center Analytics szolgáltatás csatlakozott a Power BIhoz, a rendszer betölti az adatgyűjtést.</span><span class="sxs-lookup"><span data-stu-id="796ce-135">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="796ce-136">Az adatmennyiségtől függően ez akár 10 percet is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="796ce-136">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="796ce-137">Az adatbetöltések befejezése után elkezdheti a partner Center Analytics alkalmazás irányítópultjának és jelentéseinek használatát Power BI.</span><span class="sxs-lookup"><span data-stu-id="796ce-137">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="796ce-138">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="796ce-138">Next steps</span></span>

[<span data-ttu-id="796ce-139">Üzleti adatai megtekinthetők a Microsoft Power BI partner Center Analytics alkalmazásával</span><span class="sxs-lookup"><span data-stu-id="796ce-139">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
