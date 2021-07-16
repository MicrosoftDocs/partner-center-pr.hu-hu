---
title: Az elemzési adatok programozott elérésének előfeltételei
description: Az elemzési adatok programozott elérésének előfeltételei
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376667"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="81271-103">Az elemzési adatok programozott elérésének előfeltételei</span><span class="sxs-lookup"><span data-stu-id="81271-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="81271-104">**Megfelelő szerepkörök:** Globális rendszergazdai | MPN-rendszergazda</span><span class="sxs-lookup"><span data-stu-id="81271-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="81271-105">Mielőtt programozott módon hozzáfér a partnerelemzési adatokhoz, teljesítenie kell az alábbi követelményeket.</span><span class="sxs-lookup"><span data-stu-id="81271-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="81271-106">MPN-program regisztrálása</span><span class="sxs-lookup"><span data-stu-id="81271-106">MPN Program enrollment</span></span>

<span data-ttu-id="81271-107">A partnerelemzési adatok programozott eléréséhez regisztrálni kell az MPN-programban, és létre kell Partnerközpont fiókkal.</span><span class="sxs-lookup"><span data-stu-id="81271-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="81271-108">További információ: [MPN-fiók létrehozása a Partnerközpont](mpn-create-a-partner-center-account.md)</span><span class="sxs-lookup"><span data-stu-id="81271-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="81271-109">Azure Active Directory (AAD) alkalmazás létrehozása</span><span class="sxs-lookup"><span data-stu-id="81271-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="81271-110">A partneradatok programozott eléréséhez nem használhatók normál felhasználói hitelesítő adatok Elemzések Analytics-adatokhoz.</span><span class="sxs-lookup"><span data-stu-id="81271-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="81271-111">A Azure Active Directory hozzáférési API-k eléréséhez létre kell Azure Active Directory (AAD) alkalmazást és egy titkos elérésű (alkalmazás + felhasználói hozzáférés) alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="81271-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="81271-112">Az AAD-alkalmazások és titkos információk létrehozásáról lásd: Rövid útmutató: Alkalmazás regisztrálása [a Microsoft Identitásplatform.](/azure/active-directory/develop/quickstart-register-app)   A Microsoft-fiók eléréséhez engedély Partner API.</span><span class="sxs-lookup"><span data-stu-id="81271-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="81271-113">Az engedélyek hozzáadásának elsajátításért lásd: Partner API [hitelesítés – Partner](/partner/develop/api-authentication#application-and-user-access)</span><span class="sxs-lookup"><span data-stu-id="81271-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="81271-114">Vezetői jelentésmegjelenítő (ERV) szerepkör hozzárendelése a felhasználóhoz</span><span class="sxs-lookup"><span data-stu-id="81271-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="81271-115">A partnerelemzési adatok programozott módon való eléréséhez az Executive Report Viewer (ERV) alkalmazással kell rendelkezésre lennie.</span><span class="sxs-lookup"><span data-stu-id="81271-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="81271-116">Az ERV szerepkör felhasználóhoz való hozzárendelésének elsajátításért lásd: Partnerközpont Elemzések hozzáférés hozzárendelése – [Partnerközpont](insights-roles.md)</span><span class="sxs-lookup"><span data-stu-id="81271-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="81271-117">AAD-jogkivonat létrehozása</span><span class="sxs-lookup"><span data-stu-id="81271-117">Generate an AAD token</span></span>

<span data-ttu-id="81271-118">Létre kell hoznia egy AAD-jogkivonatot az alkalmazás (ügyfél) azonosítójával, titkos ügyfél titkos kódjával, a felhasználói azonosítójával és jelszavával.   [Itt ellenőrizheti](insights-programmatic-first-api-call.md#token-generation) az AAD-jogkivonat létrehozásához szükséges lépéseket.</span><span class="sxs-lookup"><span data-stu-id="81271-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="81271-119">A jogkivonat egy óráig érvényes.</span><span class="sxs-lookup"><span data-stu-id="81271-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="81271-120">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="81271-120">Next steps</span></span>
[<span data-ttu-id="81271-121">Programozott hozzáférési paradigma</span><span class="sxs-lookup"><span data-stu-id="81271-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)