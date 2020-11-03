---
title: Munkahelyi fiók összekapcsolása a partner Center eléréséhez
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hozzon létre egy munkahelyi fiókot, amely összeköti a vállalatot a partner Center-fiókjával. Ez lehetővé teszi a vállalat alkalmazottai számára a partneri központ elérését.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: 2cc30c3681f0310f738ed937c15e0142b20cdc4c
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528495"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a><span data-ttu-id="4c957-104">Munkahelyi fiók létrehozása, amely összeköti a vállalatot a partner Center-fiókkal</span><span class="sxs-lookup"><span data-stu-id="4c957-104">Create a work account that links your company to your Partner Center account</span></span>

<span data-ttu-id="4c957-105">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="4c957-105">**Applies to**</span></span>

- <span data-ttu-id="4c957-106">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="4c957-106">Partner Center</span></span>

<span data-ttu-id="4c957-107">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="4c957-107">**Appropriate roles**</span></span>

- <span data-ttu-id="4c957-108">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="4c957-108">Global admin</span></span>
- <span data-ttu-id="4c957-109">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="4c957-109">User management admin</span></span>

## <a name="why-you-need-a-work-account"></a><span data-ttu-id="4c957-110">Miért van szüksége munkahelyi fiókra</span><span class="sxs-lookup"><span data-stu-id="4c957-110">Why you need a work account</span></span>

<span data-ttu-id="4c957-111">A Microsoft megköveteli, hogy a vállalati munkahelyi fiókot az új partner Center-fiókhoz kapcsolja.</span><span class="sxs-lookup"><span data-stu-id="4c957-111">Microsoft requires you to link your company's work account to your new Partner Center account.</span></span> <span data-ttu-id="4c957-112">A hivatkozás lehetővé teszi, hogy a fiók felhasználói bejelentkezzenek a partner központba a munkahelyi fiók felhasználónevével és jelszavával.</span><span class="sxs-lookup"><span data-stu-id="4c957-112">The link enables your account users to sign in to Partner Center with their work account user names and passwords.</span></span>

## <a name="the-work-account-email-address"></a><span data-ttu-id="4c957-113">A munkahelyi fiók e-mail-címe</span><span class="sxs-lookup"><span data-stu-id="4c957-113">The work account email address</span></span>

<span data-ttu-id="4c957-114">Munkahelyi fiókja vagy munkahelyi e-mail-címe a vállalata által megadott e-mail-cím.</span><span class="sxs-lookup"><span data-stu-id="4c957-114">Your work account or work email is the email address provided to you by your company.</span></span> <span data-ttu-id="4c957-115">A munkahelyi fiókhoz tartozó e-mailek formátuma általában `you@yourcompany.com` .</span><span class="sxs-lookup"><span data-stu-id="4c957-115">A work account email is usually in the format `you@yourcompany.com`.</span></span> <span data-ttu-id="4c957-116">A személyes e-mail-címek, például a Hotmail, a Gmail vagy a Yahoo nem működnek e-mailben, és nem használhatók a partner Center-fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="4c957-116">Personal email addresses such as Hotmail, Gmail, or Yahoo aren't work email and can't be used for your Partner Center account.</span></span>

<span data-ttu-id="4c957-117">Ha egynél több érvényes munkahelyi e-mail-címmel rendelkezik, használja a céges központhoz társított, nem pedig a regionális részleget, hanem a `contoso.com` cím helyett használja az e-mail-címét `contoso.uk` .</span><span class="sxs-lookup"><span data-stu-id="4c957-117">If you have more than one valid work email address, use the one that is associated to your Corporate Headquarters rather than the regional department, for example, use your `contoso.com` email rather than the `contoso.uk` address.</span></span>

> [!NOTE]  
> <span data-ttu-id="4c957-118">Mielőtt meglévő munkahelyi fiókot szeretne használni, gondolja át, hogy a fiók hány felhasználójának kell működnie a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="4c957-118">Before you decide to use an existing work account, think about how many users in the account will need to work in Partner Center.</span></span> <span data-ttu-id="4c957-119">Ha olyan fiókkal rendelkező felhasználókkal rendelkezik, akiknek nem kell a partner Centerben dolgoznia, érdemes lehet új fiókot létrehozni csak azokhoz a felhasználókhoz, akiknek a partner Centerben kell működniük.</span><span class="sxs-lookup"><span data-stu-id="4c957-119">If you have users in the account who won't need to work in Partner Center, consider creating a new account for only those users who will need to work in the Partner Center.</span></span>

## <a name="not-sure-if-your-company-already-has-a-work-account"></a><span data-ttu-id="4c957-120">Nem biztos abban, hogy a vállalata már rendelkezik munkahelyi fiókkal?</span><span class="sxs-lookup"><span data-stu-id="4c957-120">Not sure if your company already has a work account?</span></span>

<span data-ttu-id="4c957-121">Ha nem biztos abban, hogy munkahelyi fiókja van-e, kövesse az alábbi lépéseket az ellenőrzéshez.</span><span class="sxs-lookup"><span data-stu-id="4c957-121">If you're not sure whether your company has a work account, follow these steps to check.</span></span> <span data-ttu-id="4c957-122">Ha Microsoft Azure vagy Office 365-es aktív előfizetéssel rendelkezik, már van munkahelyi fiókja.</span><span class="sxs-lookup"><span data-stu-id="4c957-122">If you have an active subscription to Microsoft Azure or Office 365, you already have a work account.</span></span>

1. <span data-ttu-id="4c957-123">Jelentkezzen be az [Azure Portalra](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="4c957-123">Sign in to the [Azure portal](https://portal.azure.com).</span></span>

2. <span data-ttu-id="4c957-124">Válassza a menü Azure Active Directory elemét, majd válassza a tartománynevek lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4c957-124">Select Azure Active Directory from the menu and then select Domain Names.</span></span>

3. <span data-ttu-id="4c957-125">Ha már rendelkezik munkahelyi fiókkal, a rendszer a tartománynevet fogja listázni.</span><span class="sxs-lookup"><span data-stu-id="4c957-125">If you already have a work account, your domain name will be listed.</span></span>

<span data-ttu-id="4c957-126">Ha a vállalat még nem rendelkezik munkahelyi fiókkal, létrehozhat egyet a beléptetési folyamat során.</span><span class="sxs-lookup"><span data-stu-id="4c957-126">If your company doesn't already have a work account, you can create one during the enrollment process.</span></span>

<span data-ttu-id="4c957-127">Az alábbi ábra számos jellemző forgatókönyvhöz biztosít lépéseket:</span><span class="sxs-lookup"><span data-stu-id="4c957-127">The diagram below provides steps for several typical scenarios:</span></span>

- <span data-ttu-id="4c957-128">annak megállapítása, hogy van-e munkahelyi fiókja</span><span class="sxs-lookup"><span data-stu-id="4c957-128">determine if you have a work account</span></span>
- <span data-ttu-id="4c957-129">a munkahelyi fiókba való bejelentkezés módjának meghatározása</span><span class="sxs-lookup"><span data-stu-id="4c957-129">determine how to sign into your work account</span></span>
- <span data-ttu-id="4c957-130">annak megállapítása, hogy létre kell-e hoznia egy új munkahelyi fiókot</span><span class="sxs-lookup"><span data-stu-id="4c957-130">determine if you need to create a new work account</span></span>

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Van munkahelyi fiókja, vagy létre kell hoznia egyet?":::

<span data-ttu-id="4c957-132">További információ tartományok hozzáadásáról az Azure AD-ben: [tartomány hozzáadása vagy hozzárendelése az Azure ad](/azure/active-directory/active-directory-add-domain) -ben</span><span class="sxs-lookup"><span data-stu-id="4c957-132">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="4c957-133">Tudnivalók Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="4c957-133">About Microsoft Azure</span></span>

<span data-ttu-id="4c957-134">A Microsoft Azure egy nyilvános felhőalapú platform, amellyel a vállalatok a Microsoft által felügyelt adatközpontok globális hálózatán hozhatnak létre, helyezhetnek üzembe és kezelhetnek alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="4c957-134">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="4c957-135">A vállalatok az Azure-t használják virtuális informatikai infrastruktúra létrehozásához virtuális funkciókkal vagy szolgáltatásokkal fizikai gépek helyett.</span><span class="sxs-lookup"><span data-stu-id="4c957-135">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span>

<span data-ttu-id="4c957-136">Ha Azure-előfizetést vásárol, lényegében egy dedikált, biztonságos területet bérel az Azure nyilvános felhőben, nem egészen más, mint a vállalat fizikai üzleti tevékenységének elsajátításához.</span><span class="sxs-lookup"><span data-stu-id="4c957-136">When you purchase an Azure subscription, you're essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company's physical business.</span></span> <span data-ttu-id="4c957-137">Az irodaház tulajdonosának a vállalata bérlő.</span><span class="sxs-lookup"><span data-stu-id="4c957-137">To the office building's owner, your company is a tenant.</span></span>

<span data-ttu-id="4c957-138">Az Azure-beli munkahelyi fiók a vállalat dedikált és elszigetelt virtuális ábrázolása az Azure nyilvános felhőben, amely akkor jön létre, amikor előfizet egy Microsoft Cloud Service-re (például Azure, Microsoft Intune vagy Office 365).</span><span class="sxs-lookup"><span data-stu-id="4c957-138">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="4c957-139">Munkahelyi fiókja az Azure AD-felhasználókat és a rájuk vonatkozó információkat – a jelszavukat, a profil adatait, az engedélyeket stb. – tárolja.</span><span class="sxs-lookup"><span data-stu-id="4c957-139">Your work account hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="4c957-140">A munkahelyi fiók a vállalatra és annak biztonságára vonatkozó csoportokat, alkalmazásokat és egyéb információkat is tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="4c957-140">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span>