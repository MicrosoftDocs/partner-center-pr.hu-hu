---
title: Azure AD-szolgáltatásnév
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan adhat hozzá szolgáltatásnévt az Azure AD-bérlőhöz. Ez egy Azure AD-alkalmazás (szolgáltatásnév) hozzáadását jelenti a Partnerközpont.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551554"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="92193-104">Azure AD-alkalmazás (szolgáltatásnév) hozzáadása a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="92193-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="92193-105">**Megfelelő szerepkörök:** Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="92193-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="92193-106">A Partnerközpont kereskedelmi piactéri programjában most már hozzáadhat egy Microsoft Azure Active Directory-alkalmazást (Azure AD)-alkalmazást (szolgáltatásnév) az Partnerközpont fiókjában.</span><span class="sxs-lookup"><span data-stu-id="92193-106">In the Commercial Marketplace program in Partner Center, you are now able to add a Microsoft Azure Active Directory (Azure AD) application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="92193-107">(Ezt korábban már meg tudta tenni a Cloud Partner Portal (CPP) fiókjában.</span><span class="sxs-lookup"><span data-stu-id="92193-107">(You were able to do so previously in your Cloud Partner Portal (CPP) account.</span></span> <span data-ttu-id="92193-108">Most, hogy migrált a Partnerközpont, a CPP-fiók csak olvasható.)</span><span class="sxs-lookup"><span data-stu-id="92193-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="92193-109">A szolgáltatásnév az Azure AD-alkalmazás szinonimája.</span><span class="sxs-lookup"><span data-stu-id="92193-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="92193-110">Azure AD-alkalmazás hozzáadása (szolgáltatásnév)</span><span class="sxs-lookup"><span data-stu-id="92193-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="92193-111">A Partnerközpont válassza a **Beállítások,** majd a Fejlesztői **beállítások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="92193-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="92193-112">Válassza **a Felhasználók,** majd az **Azure AD-alkalmazások hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="92193-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="92193-113">Válasszon ki egy meglévő Azure AD-alkalmazást, vagy hozzon létre egy újat.</span><span class="sxs-lookup"><span data-stu-id="92193-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="92193-114">Ha új Azure AD-alkalmazást hoz létre, a következő információkat kell tartalmaznia:</span><span class="sxs-lookup"><span data-stu-id="92193-114">If you create a new Azure AD application, include the following information:</span></span>  

   - <span data-ttu-id="92193-115">**Válasz URL-cím:** Az AZ URL-cím, ahová a felhasználók bejelentkeznek az Azure AD-alkalmazás használata érdekében.</span><span class="sxs-lookup"><span data-stu-id="92193-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="92193-116">**Alkalmazásazonosító URI:** Az Azure AD-alkalmazás logikai azonosítója, amely akkor lesz bemutatva, amikor egyszeri bejelentkezési kérelmet küld az Azure AD-nek.</span><span class="sxs-lookup"><span data-stu-id="92193-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="92193-117">**Biztonsági szerepkörök:**  A szerepkörkezelő (ugyanaz, mint a CPP tulajdonosi szerepköre) és a fejlesztő **(ugyanaz,** mint a CPP közreműködői szerepköre) a Partnerközpont kereskedelmi piactéri programjában érvényesek, és társíthatóak ehhez az Azure AD-alkalmazáshoz.</span><span class="sxs-lookup"><span data-stu-id="92193-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="92193-118">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="92193-118">Next steps</span></span>

- [<span data-ttu-id="92193-119">A kereskedelmi piactér áttekintése a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="92193-119">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)