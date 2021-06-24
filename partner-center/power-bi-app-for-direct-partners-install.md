---
title: A Partnerközpont Analytics for Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A cikk lépéseit követve telepítheti és megtekintheti az Partnerközpont adatelemzési alkalmazás a Power BI-hoz (a CSP közvetlen partnerei számára).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ff95f989ac847bd2c17558d062c86a52110b2ddf
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565040"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="ef01b-103">A Partnerközpont adatelemzési alkalmazás a Microsoft Power BI-hoz telepítése és előzetes verziója</span><span class="sxs-lookup"><span data-stu-id="ef01b-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>


<span data-ttu-id="ef01b-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Értékesítési ügynök | Rendszergazdai ügynök</span><span class="sxs-lookup"><span data-stu-id="ef01b-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="ef01b-105">Előkészületek</span><span class="sxs-lookup"><span data-stu-id="ef01b-105">Before you begin</span></span>

<span data-ttu-id="ef01b-106">Válassza ki az üzlet szempontjából legfontosabb alkalmazást az elérhető Microsoft Power BI közül:</span><span class="sxs-lookup"><span data-stu-id="ef01b-106">Select the application that is most relevant to your business from the following list of available Microsoft Power BI apps:</span></span>

- [<span data-ttu-id="ef01b-107">Közvetlen szolgáltató</span><span class="sxs-lookup"><span data-stu-id="ef01b-107">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="ef01b-108">Közvetett szolgáltató</span><span class="sxs-lookup"><span data-stu-id="ef01b-108">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="ef01b-109">Közvetett viszonteladó</span><span class="sxs-lookup"><span data-stu-id="ef01b-109">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="ef01b-110">A Partnerközpont Analytics alkalmazás előzetes verziójának telepítése előtt győződjön meg arról, hogy megfelel az alábbi követelményeknek.</span><span class="sxs-lookup"><span data-stu-id="ef01b-110">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="ef01b-111">Válassza ki a Power BI megfelelő alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="ef01b-111">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="ef01b-112">Pro-licenccel Power BI rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="ef01b-112">You have a Power BI pro license.</span></span>

- <span data-ttu-id="ef01b-113">Rendelkezik a sablonalkalmazások bérlőn való telepítéséhez szükséges engedélyekkel.</span><span class="sxs-lookup"><span data-stu-id="ef01b-113">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="ef01b-114">Bejelentkezhet a Power BI.</span><span class="sxs-lookup"><span data-stu-id="ef01b-114">You can sign in to Power BI.</span></span>

- <span data-ttu-id="ef01b-115">Bejelentkezhet globális rendszergazdaként, rendszergazdai ügynökként vagy számlázási rendszergazdaként a vállalat Azure Active Directory [(Azure AD) bérlőjébe.](azure-active-directory-tenants-and-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="ef01b-115">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="ef01b-116">Az alkalmazás telepítése</span><span class="sxs-lookup"><span data-stu-id="ef01b-116">To install the app</span></span>

1. <span data-ttu-id="ef01b-117">Válassza ki a fenti szakaszban megadott alkalmazásforrás-hivatkozást (közvetlen szolgáltató/közvetett szolgáltató/közvetett viszonteladó).</span><span class="sxs-lookup"><span data-stu-id="ef01b-117">Select the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="ef01b-118">Válassza **a GET IT NOW (SZEREZZE BE MOST) lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ef01b-118">Select **GET IT NOW**.</span></span> 

3. <span data-ttu-id="ef01b-119">A Folytatás lehetőség kiválasztásával elfogadja a feltételeket és **a feltételeket.**</span><span class="sxs-lookup"><span data-stu-id="ef01b-119">Agree terms and conditions by selecting **Continue**.</span></span>

4. <span data-ttu-id="ef01b-120">A Már rendelkezik fiókkal? válassza **a Bejelentkezés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ef01b-120">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="ef01b-121">A következő lapon adja meg a Power BI felhasználónevét és jelszavát, majd válassza a **Bejelentkezés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ef01b-121">On the next page, enter your Power BI user name and password and then select **Sign In**.</span></span>

6. <span data-ttu-id="ef01b-122">Telepítse a munkaterületet a munkaterület nevének meg megszava.</span><span class="sxs-lookup"><span data-stu-id="ef01b-122">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="ef01b-123">A telepített sablonalkalmazásokat az Alkalmazások szakaszban találja.</span><span class="sxs-lookup"><span data-stu-id="ef01b-123">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="ef01b-124">Válassza **az Alkalmazások lehetőséget,** és válassza ki a telepített alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="ef01b-124">Select **Apps** and choose the installed apps.</span></span>

9. <span data-ttu-id="ef01b-125">Megnyílik az Új alkalmazás első lépések képernyője.</span><span class="sxs-lookup"><span data-stu-id="ef01b-125">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="ef01b-126">Az adatokhoz való csatlakozáshoz válassza a Csatlakozás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ef01b-126">To connect to the data, select **Connect**.</span></span>

11. <span data-ttu-id="ef01b-127">A **Csatlakozás az Partnerközpont Analyticshez** előugró ablakban  ellenőrizze, hogy a Hitelesítési módszer **beállítása oAuth2,** vagy ha nem, válassza az **oAuth2** lehetőséget a listából.</span><span class="sxs-lookup"><span data-stu-id="ef01b-127">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="ef01b-128">Az ablak megjelenése eltarthat néhány percig.</span><span class="sxs-lookup"><span data-stu-id="ef01b-128">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="ef01b-129">A **Partnerközpont Analytics-összekötő** lapon jelentkezzen be a vállalati Azure AD-bérlő globális rendszergazdai, rendszergazdai vagy számlázási rendszergazdai hitelesítő adataival, majd válassza a **Bejelentkezés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ef01b-129">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="ef01b-130">Amikor a rendszer hozzáférést kér, válassza az **Elfogadás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ef01b-130">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="ef01b-131">Miután az Partnerközpont Analytics szolgáltatás csatlakozott a Power BI, megkezdődik az adatok betöltése.</span><span class="sxs-lookup"><span data-stu-id="ef01b-131">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="ef01b-132">Az adatok mennyiségétől függően ez akár 10 percig is eltarthat.</span><span class="sxs-lookup"><span data-stu-id="ef01b-132">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="ef01b-133">Az adatok betöltését követően elkezdheti használni a Partnerközpont Analytics-alkalmazás irányítópultját és jelentéseit a Power BI.</span><span class="sxs-lookup"><span data-stu-id="ef01b-133">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ef01b-134">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ef01b-134">Next steps</span></span>

[<span data-ttu-id="ef01b-135">Üzleti adatok megtekintése a Microsoft Partnerközpont Analytics alkalmazással Power BI</span><span class="sxs-lookup"><span data-stu-id="ef01b-135">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
