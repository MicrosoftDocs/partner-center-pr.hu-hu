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
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2020
ms.locfileid: "92528154"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="c838c-104">Azure AD-alkalmazás (egyszerű szolgáltatásnév) hozzáadása a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="c838c-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="c838c-105">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="c838c-105">**Applies to**</span></span>

- <span data-ttu-id="c838c-106">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="c838c-106">Partner Center</span></span>

<span data-ttu-id="c838c-107">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="c838c-107">**Appropriate roles**</span></span>

- <span data-ttu-id="c838c-108">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="c838c-108">Global admin</span></span>

<span data-ttu-id="c838c-109">A partner Center kereskedelmi piactér programjában mostantól hozzáadhat egy Azure AD-alkalmazást (egyszerű szolgáltatásnév) a partner Center-fiókjában.</span><span class="sxs-lookup"><span data-stu-id="c838c-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="c838c-110">(Korábban már megtehette a Cloud Partner Portalban, vagy a CPP-ben, a fiókban.</span><span class="sxs-lookup"><span data-stu-id="c838c-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="c838c-111">Most, hogy áttelepítette a partner központba, a CPP-fiók írásvédett.)</span><span class="sxs-lookup"><span data-stu-id="c838c-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="c838c-112">Az egyszerű szolgáltatásnév az Azure AD-alkalmazás szinonimája.</span><span class="sxs-lookup"><span data-stu-id="c838c-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="c838c-113">Azure AD-alkalmazás hozzáadása (egyszerű szolgáltatásnév)</span><span class="sxs-lookup"><span data-stu-id="c838c-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="c838c-114">A partner Center irányítópultján válassza a **Beállítások** , majd a **fejlesztői beállítások** elemet.</span><span class="sxs-lookup"><span data-stu-id="c838c-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings** .</span></span>

2. <span data-ttu-id="c838c-115">Válassza a **felhasználók** , majd az **Azure ad-alkalmazások hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c838c-115">Select **Users** and then select **Add Azure AD Applications** .</span></span>

3. <span data-ttu-id="c838c-116">Válasszon ki egy meglévő Azure AD-alkalmazást, vagy hozzon létre egy újat.</span><span class="sxs-lookup"><span data-stu-id="c838c-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="c838c-117">Ha új Azure AD-alkalmazást hoz létre, a következő információkat kell tartalmaznia:</span><span class="sxs-lookup"><span data-stu-id="c838c-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="c838c-118">**Válasz URL-címe** : az az URL-cím, amelyben a felhasználók bejelentkezhetnek az Azure ad-alkalmazás használatára.</span><span class="sxs-lookup"><span data-stu-id="c838c-118">**Reply URL** : The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="c838c-119">**Alkalmazás-azonosító URI** : az Azure ad-alkalmazáshoz tartozó logikai azonosító, amely akkor jelenik meg, amikor egyszeri bejelentkezésre vonatkozó kérést küld az Azure ad-nek.</span><span class="sxs-lookup"><span data-stu-id="c838c-119">**App ID URI** : A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="c838c-120">**Biztonsági szerepkörök** : a szerepkörök **kezelője** (ugyanaz, mint a "tulajdonos" szerepkör a CPP-ben) és a **fejlesztő** (ugyanaz, mint a "közreműködői" szerepkör a CPP-ben) a partner Center kereskedelmi piactér programjára vonatkozik, és társítható ehhez az Azure ad-alkalmazáshoz.</span><span class="sxs-lookup"><span data-stu-id="c838c-120">**Security roles** : The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="c838c-121">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c838c-121">Next steps</span></span>

- [<span data-ttu-id="c838c-122">A partneri központ kereskedelmi piactérének áttekintése</span><span class="sxs-lookup"><span data-stu-id="c838c-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)