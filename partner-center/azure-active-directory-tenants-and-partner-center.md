---
title: Munkahelyi fiók összekapcsolása a Partnerközpont
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hozzon létre egy munkahelyi fiókot, amely összeköti a vállalatát Partnerközpont fiókjával. Ez lehetővé teszi, hogy a vállalat alkalmazottai hozzáférjenek Partnerközpont.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: a06a38ef9d96b4c2a1e95328d510eb2fd71ff0e3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149842"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a><span data-ttu-id="e48a4-104">Hozzon létre egy munkahelyi fiókot, amely összeköti a vállalatot Partnerközpont fiókjával</span><span class="sxs-lookup"><span data-stu-id="e48a4-104">Create a work account that links your company to your Partner Center account</span></span>

<span data-ttu-id="e48a4-105">**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelő rendszergazda</span><span class="sxs-lookup"><span data-stu-id="e48a4-105">**Appropriate roles**: Global admin | User management admin</span></span>

## <a name="why-you-need-a-work-account"></a><span data-ttu-id="e48a4-106">Miért van szüksége munkahelyi fiókra?</span><span class="sxs-lookup"><span data-stu-id="e48a4-106">Why you need a work account</span></span>

<span data-ttu-id="e48a4-107">A Microsoft megköveteli, hogy a vállalat munkahelyi fiókját az új munkahelyi Partnerközpont hozzá.</span><span class="sxs-lookup"><span data-stu-id="e48a4-107">Microsoft requires you to link your company's work account to your new Partner Center account.</span></span> <span data-ttu-id="e48a4-108">A hivatkozással a fiók felhasználói bejelentkeznek Partnerközpont munkahelyi fiókjuk felhasználónevével és jelszavával.</span><span class="sxs-lookup"><span data-stu-id="e48a4-108">The link enables your account users to sign in to Partner Center with their work account user names and passwords.</span></span>

## <a name="the-work-account-email-address"></a><span data-ttu-id="e48a4-109">A munkahelyi fiók e-mail-címe</span><span class="sxs-lookup"><span data-stu-id="e48a4-109">The work account email address</span></span>

<span data-ttu-id="e48a4-110">Munkahelyi fiókja vagy munkahelyi e-mail-címe a vállalat által megadott e-mail-cím.</span><span class="sxs-lookup"><span data-stu-id="e48a4-110">Your work account or work email is the email address provided to you by your company.</span></span> <span data-ttu-id="e48a4-111">A munkahelyi fiók e-mail-címe általában formátumban `you@yourcompany.com` van.</span><span class="sxs-lookup"><span data-stu-id="e48a4-111">A work account email is usually in the format `you@yourcompany.com`.</span></span> <span data-ttu-id="e48a4-112">Az olyan személyes e-mail-címek, mint a Hotmail, a Gmail vagy a Yahoo, nem munkahelyi e-mail-címek, és nem használhatók Partnerközpont fiókjához.</span><span class="sxs-lookup"><span data-stu-id="e48a4-112">Personal email addresses such as Hotmail, Gmail, or Yahoo aren't work email and can't be used for your Partner Center account.</span></span>

<span data-ttu-id="e48a4-113">Ha több érvényes e-mail-címmel is dolgozik, használja azt, amely a regionális részleg helyett a vállalati főközponthoz van társítva, például használja az e-mail-címét a `contoso.com` cím `contoso.uk` helyett.</span><span class="sxs-lookup"><span data-stu-id="e48a4-113">If you have more than one valid work email address, use the one that is associated to your Corporate Headquarters rather than the regional department, for example, use your `contoso.com` email rather than the `contoso.uk` address.</span></span>

> [!NOTE]  
> <span data-ttu-id="e48a4-114">Mielőtt úgy dönt, hogy meglévő munkahelyi fiókot használ, gondolja át, hány felhasználónak kell a fiókban dolgoznia a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="e48a4-114">Before you decide to use an existing work account, think about how many users in the account will need to work in Partner Center.</span></span> <span data-ttu-id="e48a4-115">Ha vannak olyan felhasználói a fiókban, akiknek nem kell a Partnerközpont-ban dolgoznia, fontolja meg egy új fiók létrehozását csak azok számára, akiknek a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="e48a4-115">If you have users in the account who won't need to work in Partner Center, consider creating a new account for only those users who will need to work in the Partner Center.</span></span>

## <a name="not-sure-if-your-company-already-has-a-work-account"></a><span data-ttu-id="e48a4-116">Nem tudja, hogy a vállalata rendelkezik-e már munkahelyi fiókkal?</span><span class="sxs-lookup"><span data-stu-id="e48a4-116">Not sure if your company already has a work account?</span></span>

<span data-ttu-id="e48a4-117">Ha nem biztos abban, hogy a vállalata rendelkezik-e munkahelyi fiókkal, kövesse az alábbi lépéseket az ellenőrzéshez.</span><span class="sxs-lookup"><span data-stu-id="e48a4-117">If you're not sure whether your company has a work account, follow these steps to check.</span></span> <span data-ttu-id="e48a4-118">Ha aktív előfizetéssel rendelkezik egy Microsoft Azure Office 365-előfizetéssel, már rendelkezik munkahelyi fiókkal.</span><span class="sxs-lookup"><span data-stu-id="e48a4-118">If you have an active subscription to Microsoft Azure or Office 365, you already have a work account.</span></span>

1. <span data-ttu-id="e48a4-119">Jelentkezzen be az [Azure Portalra](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="e48a4-119">Sign in to the [Azure portal](https://portal.azure.com).</span></span>

2. <span data-ttu-id="e48a4-120">Válassza Azure Active Directory a menüből, majd válassza a Tartománynevek lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e48a4-120">Select Azure Active Directory from the menu and then select Domain Names.</span></span>

3. <span data-ttu-id="e48a4-121">Ha már rendelkezik munkahelyi fiókkal, a tartománynév megjelenik a listában.</span><span class="sxs-lookup"><span data-stu-id="e48a4-121">If you already have a work account, your domain name will be listed.</span></span>

<span data-ttu-id="e48a4-122">Ha a vállalat még nem rendelkezik munkahelyi fiókkal, létrehozhat egyet a regisztrációs folyamat során.</span><span class="sxs-lookup"><span data-stu-id="e48a4-122">If your company doesn't already have a work account, you can create one during the enrollment process.</span></span>

<span data-ttu-id="e48a4-123">Az alábbi ábra számos tipikus forgatókönyv lépéseit mutatja be:</span><span class="sxs-lookup"><span data-stu-id="e48a4-123">The diagram below provides steps for several typical scenarios:</span></span>

- <span data-ttu-id="e48a4-124">állapítsa meg, hogy van-e munkahelyi fiókja</span><span class="sxs-lookup"><span data-stu-id="e48a4-124">determine if you have a work account</span></span>
- <span data-ttu-id="e48a4-125">a munkahelyi fiókba való bejelentkezés mikéntjének meghatározása</span><span class="sxs-lookup"><span data-stu-id="e48a4-125">determine how to sign into your work account</span></span>
- <span data-ttu-id="e48a4-126">annak meghatározása, hogy létre kell-e hoznia egy új munkahelyi fiókot</span><span class="sxs-lookup"><span data-stu-id="e48a4-126">determine if you need to create a new work account</span></span>

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Van munkahelyi fiókja, vagy létre kell hoznia egyet?":::

<span data-ttu-id="e48a4-128">További információ tartományok hozzáadásáról az Azure AD-ban: Tartomány hozzáadása vagy társítása az [Azure AD-ban.](/azure/active-directory/active-directory-add-domain)</span><span class="sxs-lookup"><span data-stu-id="e48a4-128">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="e48a4-129">A Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e48a4-129">About Microsoft Azure</span></span>

<span data-ttu-id="e48a4-130">Microsoft Azure egy nyilvános felhőplatform, amely segítségével a vállalatok alkalmazásokat építenek ki, helyezhetnek üzembe és kezelnek a Microsoft által felügyelt adatközpontok globális hálózatán.</span><span class="sxs-lookup"><span data-stu-id="e48a4-130">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="e48a4-131">A vállalatok az Azure-ral fizikai gépek helyett virtuális függvényekkel vagy szolgáltatásokkal működő virtuális it-infrastruktúrát építenek ki.</span><span class="sxs-lookup"><span data-stu-id="e48a4-131">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span>

<span data-ttu-id="e48a4-132">Amikor Azure-előfizetést vásárol, lényegében egy dedikált, biztonságos helyet bérel az Azure nyilvános felhőben, nem olyan különbözik attól, mintha egy irodaépületben bérel egy padlót a vállalat fizikai üzlete számára.</span><span class="sxs-lookup"><span data-stu-id="e48a4-132">When you purchase an Azure subscription, you're essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company's physical business.</span></span> <span data-ttu-id="e48a4-133">Az irodaépület tulajdonosa számára a vállalat bérlő.</span><span class="sxs-lookup"><span data-stu-id="e48a4-133">To the office building's owner, your company is a tenant.</span></span>

<span data-ttu-id="e48a4-134">Az Azure-beli munkahelyi fiók a vállalat dedikált és elkülönített virtuális reprezentációja az Azure nyilvános felhőben, amely akkor jön létre, amikor előfizet egy Microsoft-felhőszolgáltatásra, például az Azure-ra, az Microsoft Intune-re vagy az Office 365-re.</span><span class="sxs-lookup"><span data-stu-id="e48a4-134">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="e48a4-135">A munkahelyi fiókjában vannak az Azure AD-felhasználók, valamint a rájuk vonatkozó információk – a jelszavaik, profiladatok, engedélyek stb.</span><span class="sxs-lookup"><span data-stu-id="e48a4-135">Your work account hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="e48a4-136">A munkahelyi fiók csoportokat, alkalmazásokat és a vállalat biztonságával kapcsolatos egyéb információkat is tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="e48a4-136">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e48a4-137">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="e48a4-137">Next steps</span></span>

- [<span data-ttu-id="e48a4-138">Partnerközponti fiók kezelése</span><span class="sxs-lookup"><span data-stu-id="e48a4-138">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="e48a4-139">Ellenőrzési állapot nyomon követése</span><span class="sxs-lookup"><span data-stu-id="e48a4-139">Track verification status</span></span>](verification-responses.md)