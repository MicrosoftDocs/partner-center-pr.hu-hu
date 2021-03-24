---
title: Azure AD egyszerű szolgáltatás
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan adhat hozzá egy egyszerű szolgáltatást az Azure AD-bérlőhöz. Ez azt jelenti, hogy hozzáad egy Azure AD-alkalmazást (egyszerű szolgáltatásnév) a partner Centerben.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ef5373fd9a606cd25345cbe80a55f28fc1f753f
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028468"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="6e9c8-104">Azure AD-alkalmazás (egyszerű szolgáltatásnév) hozzáadása a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="6e9c8-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="6e9c8-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="6e9c8-105">**Appropriate roles**</span></span>

- <span data-ttu-id="6e9c8-106">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="6e9c8-106">Global admin</span></span>

<span data-ttu-id="6e9c8-107">A partner Center kereskedelmi piactér programjában mostantól hozzáadhat egy Azure AD-alkalmazást (egyszerű szolgáltatásnév) a partner Center-fiókjában.</span><span class="sxs-lookup"><span data-stu-id="6e9c8-107">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="6e9c8-108">(Korábban már megtehette a Cloud Partner Portalban, vagy a CPP-ben, a fiókban.</span><span class="sxs-lookup"><span data-stu-id="6e9c8-108">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="6e9c8-109">Most, hogy áttelepítette a partner központba, a CPP-fiók írásvédett.)</span><span class="sxs-lookup"><span data-stu-id="6e9c8-109">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="6e9c8-110">Az egyszerű szolgáltatásnév az Azure AD-alkalmazás szinonimája.</span><span class="sxs-lookup"><span data-stu-id="6e9c8-110">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="6e9c8-111">Azure AD-alkalmazás hozzáadása (egyszerű szolgáltatásnév)</span><span class="sxs-lookup"><span data-stu-id="6e9c8-111">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="6e9c8-112">A partner Center irányítópultján válassza a **Beállítások** , majd a **fejlesztői beállítások** elemet.</span><span class="sxs-lookup"><span data-stu-id="6e9c8-112">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="6e9c8-113">Válassza a **felhasználók** , majd az **Azure ad-alkalmazások hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6e9c8-113">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="6e9c8-114">Válasszon ki egy meglévő Azure AD-alkalmazást, vagy hozzon létre egy újat.</span><span class="sxs-lookup"><span data-stu-id="6e9c8-114">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="6e9c8-115">Ha új Azure AD-alkalmazást hoz létre, a következő információkat kell tartalmaznia:</span><span class="sxs-lookup"><span data-stu-id="6e9c8-115">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="6e9c8-116">**Válasz URL-címe**: az az URL-cím, amelyben a felhasználók bejelentkezhetnek az Azure ad-alkalmazás használatára.</span><span class="sxs-lookup"><span data-stu-id="6e9c8-116">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="6e9c8-117">**Alkalmazás-azonosító URI**: az Azure ad-alkalmazáshoz tartozó logikai azonosító, amely akkor jelenik meg, amikor egyszeri bejelentkezésre vonatkozó kérést küld az Azure ad-nek.</span><span class="sxs-lookup"><span data-stu-id="6e9c8-117">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="6e9c8-118">**Biztonsági szerepkörök**: a szerepkörök **kezelője** (ugyanaz, mint a "tulajdonos" szerepkör a CPP-ben) és a **fejlesztő** (ugyanaz, mint a "közreműködői" szerepkör a CPP-ben) a partner Center kereskedelmi piactér programjára vonatkozik, és társítható ehhez az Azure ad-alkalmazáshoz.</span><span class="sxs-lookup"><span data-stu-id="6e9c8-118">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="6e9c8-119">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="6e9c8-119">Next steps</span></span>

- [<span data-ttu-id="6e9c8-120">A partneri központ kereskedelmi piactérének áttekintése</span><span class="sxs-lookup"><span data-stu-id="6e9c8-120">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)