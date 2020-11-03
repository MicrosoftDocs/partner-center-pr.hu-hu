---
title: Cloudyn által Azure Cost Management CSP-ket
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan regisztrálhat a Cloudyn-webalkalmazást, és hogyan használhat titkos kulcsot a partner Centerben, így az alkalmazással nyomon követheti az ügyfelek Azure-használati adatait és költségeit.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/17/2020
ms.locfileid: "92528001"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="ea19c-103">A Customer Azure-beli használat és költségek nyomon követése a CSP-partnerek Azure Cost Management alkalmazásával</span><span class="sxs-lookup"><span data-stu-id="ea19c-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="ea19c-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="ea19c-104">**Applies to**</span></span>

- <span data-ttu-id="ea19c-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ea19c-105">Partner Center</span></span>
- <span data-ttu-id="ea19c-106">A Cloud Solution Provider program partnerei</span><span class="sxs-lookup"><span data-stu-id="ea19c-106">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="ea19c-107">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="ea19c-107">**Appropriate roles**</span></span>

- <span data-ttu-id="ea19c-108">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="ea19c-108">Global admin</span></span>
- <span data-ttu-id="ea19c-109">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="ea19c-109">Admin agent</span></span>

[<span data-ttu-id="ea19c-110">További információ a Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="ea19c-110">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="ea19c-111">Előkészületek</span><span class="sxs-lookup"><span data-stu-id="ea19c-111">Before you begin</span></span>
<span data-ttu-id="ea19c-112">A Azure Cost Management használata előtt győződjön meg arról, hogy megfelel a következő követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="ea19c-112">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="ea19c-113">Ön egy partner a Cloud Solution Provider programban.</span><span class="sxs-lookup"><span data-stu-id="ea19c-113">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="ea19c-114">Lehetőség van a partner Center API-webalkalmazás létrehozására.</span><span class="sxs-lookup"><span data-stu-id="ea19c-114">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="ea19c-115">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="ea19c-115">Overview</span></span>

<span data-ttu-id="ea19c-116">A Cloudyn egy webalkalmazás, amellyel nyomon követheti és kezelheti az Azure-t és a használat költségeit.</span><span class="sxs-lookup"><span data-stu-id="ea19c-116">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="ea19c-117">A partner Center API-n keresztül használja.</span><span class="sxs-lookup"><span data-stu-id="ea19c-117">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="ea19c-118">Webalkalmazás regisztrálása a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="ea19c-118">Register your web app in the Partner Center</span></span>
<span data-ttu-id="ea19c-119">Ha Azure Active Directory webalkalmazást regisztrál a partner Centerben, engedélyezze a hozzáférést a partner Center API-hoz.</span><span class="sxs-lookup"><span data-stu-id="ea19c-119">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="ea19c-120">Jelentkezzen be [a partner központjába](https://partnercenter.microsoft.com/pcv/dashboard/overview) egy [globális rendszergazdai vagy rendszergazdai ügynök fiók](create-user-accounts-and-set-permissions.md)használatával.</span><span class="sxs-lookup"><span data-stu-id="ea19c-120">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="ea19c-121">A **partner Centerben** válassza a **Fiókbeállítások** &gt; **[alkalmazás-kezelés](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ea19c-121">From the **Partner Center** , select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span></span>
3.  <span data-ttu-id="ea19c-122">A **webalkalmazás** szakaszban kattintson az **Add New Web App (új webalkalmazás hozzáadása** ) elemre.</span><span class="sxs-lookup"><span data-stu-id="ea19c-122">In the **Web App** section, click **Add new web app** .</span></span>
<br> <span data-ttu-id="ea19c-123">**Megjegyzés** : Ha korábban létrehozott egy webalkalmazást, kihagyhatja a 3. lépést.</span><span class="sxs-lookup"><span data-stu-id="ea19c-123">**Note** : If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="ea19c-124">Másolja és mentse a **kereskedelmi azonosító** GUID azonosítóját és az **alkalmazás azonosítójának** GUID azonosítóját a webalkalmazáshoz.</span><span class="sxs-lookup"><span data-stu-id="ea19c-124">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="ea19c-125">Az Azure Cost Management alkalmazás 30 napos ingyenes próbaverziójának használatához mindkét azonosítóra szüksége lesz.</span><span class="sxs-lookup"><span data-stu-id="ea19c-125">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="ea19c-126">Titkos kulcs hozzáadása az alkalmazáshoz</span><span class="sxs-lookup"><span data-stu-id="ea19c-126">Add a secret key to your app</span></span>
1. <span data-ttu-id="ea19c-127">A **Kulcs hozzáadása** gomb melletti legördülő listából válassza ki az 1 vagy 2 év időtartamát.</span><span class="sxs-lookup"><span data-stu-id="ea19c-127">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="ea19c-128">Kattintson a **Kulcs hozzáadása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="ea19c-128">Click **Add key** .</span></span> 
3. <span data-ttu-id="ea19c-129">Másolja ki és mentse a titkos kulcs értékét.</span><span class="sxs-lookup"><span data-stu-id="ea19c-129">Copy and save the secret key value.</span></span> <span data-ttu-id="ea19c-130">Erre szüksége lesz a 30 napos ingyenes próbaidőszakra.</span><span class="sxs-lookup"><span data-stu-id="ea19c-130">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="ea19c-131">Az alkalmazás titkos kulcsa a több lejárati dátummal rendelkező jelszavakhoz hasonló.</span><span class="sxs-lookup"><span data-stu-id="ea19c-131">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="ea19c-132">Mentse a kulcs értékét egy biztonságos helyre későbbi használatra.</span><span class="sxs-lookup"><span data-stu-id="ea19c-132">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ea19c-133">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ea19c-133">Next steps</span></span>
<span data-ttu-id="ea19c-134">Kezdjen el egy [30 napos ingyenes próbaverziót](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="ea19c-134">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="ea19c-135">A próbaverzió elindításához a következő adatokat kell megadnia:</span><span class="sxs-lookup"><span data-stu-id="ea19c-135">You need the following details to start the trial:</span></span>
- <span data-ttu-id="ea19c-136">A partner Center bejelentkezési hitelesítő adatai</span><span class="sxs-lookup"><span data-stu-id="ea19c-136">Partner Center sign in credentials</span></span>
- <span data-ttu-id="ea19c-137">Kereskedelmi azonosító GUID</span><span class="sxs-lookup"><span data-stu-id="ea19c-137">Commerce ID GUID</span></span>
- <span data-ttu-id="ea19c-138">Alkalmazás azonosítója GUID</span><span class="sxs-lookup"><span data-stu-id="ea19c-138">App ID GUID</span></span>
- <span data-ttu-id="ea19c-139">Alkalmazás titkos kulcsának értéke</span><span class="sxs-lookup"><span data-stu-id="ea19c-139">Application secret key value</span></span>
