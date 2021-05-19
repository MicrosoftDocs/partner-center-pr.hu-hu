---
title: Regisztráció a felhőszolgáltatói programba
titleSuffix: Microsoft Cloud for US Government - Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg a CSP-program követelményeit az olyan partnerek számára, akik regisztrálni Felhőszolgáltató programba a Microsoft Cloud for US Government.
author: mowrim
ms.author: mowrim
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.date: 10/05/2020
ms.openlocfilehash: e2b206b049050efa520099d74230d8535ac93793
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147173"
---
# <a name="enroll-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a><span data-ttu-id="18eb2-103">Regisztrálás a Felhőszolgáltató programba Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="18eb2-103">Enroll in the Cloud Solution Provider program for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="18eb2-104">**A következőkre vonatkozik:** Partnerközpont Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="18eb2-104">**Applies to**: Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="18eb2-105">**Megfelelő szerepkörök:** Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="18eb2-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="18eb2-106">A Microsoft partnerei mostantól az Felhőszolgáltató program (CSP) keretében az USA szövetségi, állami, helyi és törzsi entitásai számára értékesítik a Microsoft felhőalapú megoldásait Microsoft Cloud for US Government.</span><span class="sxs-lookup"><span data-stu-id="18eb2-106">Microsoft partners can now sell Microsoft's cloud solutions and services to US federal, state, local, and tribal entities through the Cloud Solution Provider program (CSP) for Microsoft Cloud for US Government.</span></span>

<span data-ttu-id="18eb2-107">Microsoft Cloud for US Government a Microsoft Azure egy privát, dedikált és elkülönített példányát biztosítja, amely megfelel az Egyesült Államok kormányának adatbiztonságra, adatvédelemre és megfelelőségre vonatkozó követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="18eb2-107">Microsoft Cloud for US Government provides a private, dedicated, and isolated instance of Microsoft Azure that meets the US government's requirements for data security, privacy, and compliance.</span></span> <span data-ttu-id="18eb2-108">A vállalatnak meg kell felelnie a Microsoft jogosultsági követelményeinek ahhoz, hogy részt vehessenek a felhőszolgáltatói programban az Microsoft Cloud for US Government.</span><span class="sxs-lookup"><span data-stu-id="18eb2-108">Your company must meet Microsoft's eligibility requirements to participate in the CSP program for Microsoft Cloud for US Government.</span></span> <span data-ttu-id="18eb2-109">További információ: Partnerközpont [a Microsoft Cloud for US Government.](partner-center-for-microsoft-us-govt-cloud.md)</span><span class="sxs-lookup"><span data-stu-id="18eb2-109">For more information, see [Partner Center for Microsoft Cloud for US Government](partner-center-for-microsoft-us-govt-cloud.md).</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="18eb2-110">Előkészületek</span><span class="sxs-lookup"><span data-stu-id="18eb2-110">Before you begin</span></span>

<span data-ttu-id="18eb2-111">Mielőtt regisztrálhat a csp-programba az Microsoft Cloud for US Government, ellenőriznie kell, hogy a vállalata megfelel-e az USA kormányzati entitásai számára való értékesítés követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="18eb2-111">Before you can enroll in the CSP program for Microsoft Cloud for US Government, we need to verify that your company meets the requirements to sell to US government entities.</span></span> <span data-ttu-id="18eb2-112">A regisztrációs folyamat befejezése előtt töltse ki a [Microsoft Government](https://azuregov.microsoft.com/csp) Felhőérvényesítési űrlapját, hogy ellenőrizhetjük vállalata jogosultságát.</span><span class="sxs-lookup"><span data-stu-id="18eb2-112">Before you kick off the enrollment process, complete the [Microsoft Government Cloud Validation form](https://azuregov.microsoft.com/csp) so we can verify your company's eligibility.</span></span> <span data-ttu-id="18eb2-113">Miután ellenőrizjük a vállalat jogosultságát, egy, a vállalatra vonatkozó Azure Active Directory-bérlőt (Azure AD-bérlőt) Microsoft Cloud for US Government.</span><span class="sxs-lookup"><span data-stu-id="18eb2-113">After we verify your company's eligibility, we'll provide you with an Azure Active Directory (Azure AD) tenant specific to the Microsoft Cloud for US Government.</span></span>  

<span data-ttu-id="18eb2-114">Ha egy Partnerközpont-fiókot szeretne létrehozni, és regisztrálni szeretne a Microsoft Cloud for US Government-hoz a CSP-be, meg kell adnunk a következő információkat (előfordulhat, hogy a regisztrációs folyamat igénylése előtt össze kell gyűjtenie ezt az információt):</span><span class="sxs-lookup"><span data-stu-id="18eb2-114">To create a Partner Center account and enroll in CSP for Microsoft Cloud for US Government, you'll need to supply the following information (you may want to gather this information before you kick off the enrollment process):</span></span>

- <span data-ttu-id="18eb2-115">Globális rendszergazdai hitelesítő adatok a szervezet új Azure AD-bérlőjéhez Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="18eb2-115">Global admin credentials for your organization's new Azure AD tenant for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="18eb2-116">A szervezet felügyeleti Microsoft Partner Network (MPN) azonosítója</span><span class="sxs-lookup"><span data-stu-id="18eb2-116">Your organization's Microsoft Partner Network (MPN) ID</span></span>
- <span data-ttu-id="18eb2-117">Egy üzleti cím a Egyesült Államok</span><span class="sxs-lookup"><span data-stu-id="18eb2-117">A business address in the United States</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="18eb2-118">Ha már van fiókja a Partnerközpont, és csp-fiókkal szeretne regisztrálni az Microsoft Cloud for US Government-hoz, létre kell hoznia egy új, külön fiókot kifejezetten az USA kormányzati piaca számára.</span><span class="sxs-lookup"><span data-stu-id="18eb2-118">If you have an existing account in Partner Center and you want to enroll in CSP for Microsoft Cloud for US Government, you must create a new, separate account specifically for the US Government market.</span></span>

## <a name="how-to-enroll"></a><span data-ttu-id="18eb2-119">Regisztrálás</span><span class="sxs-lookup"><span data-stu-id="18eb2-119">How to enroll</span></span>

### <a name="step-1---create-a-partner-center-account-for-microsoft-cloud-for-us-government"></a><span data-ttu-id="18eb2-120">1. lépés – Hozzon létre egy Partnerközpont-fiókot a Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="18eb2-120">Step 1 - Create a Partner Center account for Microsoft Cloud for US Government</span></span>

1. <span data-ttu-id="18eb2-121">Itt kezdd el a regisztrációs [folyamatot.](https://partnercenter.microsoft.com/register/resellerusgjoinnow)</span><span class="sxs-lookup"><span data-stu-id="18eb2-121">Kick off the enrollment process [here](https://partnercenter.microsoft.com/register/resellerusgjoinnow).</span></span>

2. <span data-ttu-id="18eb2-122">Jelentkezzen be a szervezet Azure AD-bérlőjéhez globális rendszergazdai hitelesítő Microsoft Cloud for US Government.</span><span class="sxs-lookup"><span data-stu-id="18eb2-122">Sign in with global admin credentials for your organization's Azure AD tenant for Microsoft Cloud for US Government.</span></span> <span data-ttu-id="18eb2-123">Ha a szervezete nem tud fiókot ehhez a portálhoz, a Microsoft Government Cloud Validation űrlap kitöltésével kérhet [egyet.](https://azuregov.microsoft.com/csp)</span><span class="sxs-lookup"><span data-stu-id="18eb2-123">If your organization doesn't have an account for this portal, you can request one by completing the [Microsoft Government Cloud Validation form](https://azuregov.microsoft.com/csp).</span></span>

### <a name="step-2---apply-to-participate-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a><span data-ttu-id="18eb2-124">2. lépés – Alkalmazás a Felhőszolgáltató programjában való részvételhez Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="18eb2-124">Step 2 - Apply to participate in the Cloud Solution Provider program for Microsoft Cloud for US Government</span></span>

1. <span data-ttu-id="18eb2-125">Adja meg a regisztrációs űrlap hiányzó adatait, beleértve a Microsoft Partner Network azonosítóját és a szervezet ügyfélszolgálati adatait.</span><span class="sxs-lookup"><span data-stu-id="18eb2-125">Fill in any missing information on the enrollment form, including your Microsoft Partner Network ID and your organization's customer support details.</span></span>

2. <span data-ttu-id="18eb2-126">Válassza **az Elfogadás lehetőséget, és folytassa a gombra.**</span><span class="sxs-lookup"><span data-stu-id="18eb2-126">Select **Accept and continue**.</span></span> <span data-ttu-id="18eb2-127">Az alkalmazás áttekintése több napot is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="18eb2-127">Reviewing your application may take us several days.</span></span> <span data-ttu-id="18eb2-128">A felülvizsgálat befejezése után e-mailben értesítjük.</span><span class="sxs-lookup"><span data-stu-id="18eb2-128">We'll email you when we've completed our review.</span></span>

   > [!IMPORTANT]
   > <span data-ttu-id="18eb2-129">Az **Elfogadás** és folytatás lehetőség kiválasztásával megerősíti, hogy jogosult a szervezet nevében cselekedni, és elfogadja, hogy engedélyezi a Microsoftnak a háttérhitel-ellenőrzés futtatását a szervezet Felhőszolgáltató-alkalmazásának áttekintése előtt.</span><span class="sxs-lookup"><span data-stu-id="18eb2-129">By selecting **Accept and continue**, you're confirming that you're authorized to act on your organization's behalf, and you're agreeing to allow Microsoft to run a background credit check before reviewing your organization's Cloud Solution Provider application.</span></span>

### <a name="step-3---sign-the-reseller-agreement-for-microsoft-cloud-for-us-government"></a><span data-ttu-id="18eb2-130">3. lépés – A viszonteladói szerződés Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="18eb2-130">Step 3 - Sign the reseller agreement for Microsoft Cloud for US Government</span></span>

1. <span data-ttu-id="18eb2-131">Jelentkezzen be a Partnerközpont-Microsoft Cloud for US Government az alkalmazás jóváhagyási e-mailben megadott hivatkozásával.</span><span class="sxs-lookup"><span data-stu-id="18eb2-131">Sign in to Partner Center for Microsoft Cloud for US Government using the link provided in the application approval email.</span></span>

2. <span data-ttu-id="18eb2-132">A Szerződés **lapon olvassa** el a feltételeket, és ha elfogadja, válassza az **Elfogadás** lehetőséget, és folytassa a viszonteladói szerződés digitális Microsoft Cloud for US Government.</span><span class="sxs-lookup"><span data-stu-id="18eb2-132">On the **Agreement** page, read the terms, and if you agree, select **Accept and continue** to digitally sign the reseller agreement for Microsoft Cloud for US Government.</span></span> <span data-ttu-id="18eb2-133">A fiók létrehozása több órát is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="18eb2-133">Creating your account may take several hours.</span></span> <span data-ttu-id="18eb2-134">Kijelentkezhet a Partnerközpont, Microsoft Cloud for US Government később újra bejelentkezhet.</span><span class="sxs-lookup"><span data-stu-id="18eb2-134">You can sign out of Partner Center for Microsoft Cloud for US Government and then sign back in later.</span></span>

### <a name="step-4---assign-users-to-the-admin-agent-role-in-the-microsoft-azure-admin-portal-for-microsoft-cloud-for-us-government"></a><span data-ttu-id="18eb2-135">4. lépés – Felhasználók hozzárendelése a rendszergazdai ügynök szerepkörhöz a Microsoft Azure felügyeleti portálján Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="18eb2-135">Step 4 - Assign users to the Admin Agent role in the Microsoft Azure admin portal for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="18eb2-136">Microsoft Cloud for US Government a kormányzati megfelelőségi, biztonsági és adatvédelmi szabványoknak Microsoft Azure külön példányát biztosítja.</span><span class="sxs-lookup"><span data-stu-id="18eb2-136">Microsoft Cloud for US Government provides a separate instance of Microsoft Azure that meets government compliance, security, and privacy standards.</span></span> <span data-ttu-id="18eb2-137">Ahhoz, hogy a rendszergazdák felügyelni tudjanak felhasználókat és licenceket a Microsoft Azure Portal, manuálisan hozzá kell rendelnie a Rendszergazdai ügynök szerepkört.</span><span class="sxs-lookup"><span data-stu-id="18eb2-137">To allow admins to manage users and licenses in the Microsoft Azure portal, you'll need to manually assign the Admin Agent role to them.</span></span>

> [!NOTE]
> <span data-ttu-id="18eb2-138">Miután hozzárendelt felhasználókat a rendszergazdai ügynök szerepkörhöz, hozzáférhetnek az  Ügyfelek lapon található ügyféllistához, és új [ügyfeleket adhatnak hozzá.](add-a-new-customer.md)</span><span class="sxs-lookup"><span data-stu-id="18eb2-138">After you assign users to the Admin Agent role, they'll be able to access your customer list on the **Customers** page and [add new customers](add-a-new-customer.md).</span></span>

1. <span data-ttu-id="18eb2-139">Jelentkezzen be a Microsoft Azure portálra a [https://portal.azure.us/](https://portal.azure.us/) webhelyen.</span><span class="sxs-lookup"><span data-stu-id="18eb2-139">Sign in to the Microsoft Azure admin portal at [https://portal.azure.us/](https://portal.azure.us/).</span></span>

2. <span data-ttu-id="18eb2-140">Rendelje hozzá a Rendszergazdai ügynök szerepkört a szervezet megfelelő felhasználóihoz.</span><span class="sxs-lookup"><span data-stu-id="18eb2-140">Assign the Admin Agent role to the appropriate users in your organization.</span></span> <span data-ttu-id="18eb2-141">Ehhez hozzá kell adni ezeket a felhasználókat a beépített **AdminAgent csoporthoz.**</span><span class="sxs-lookup"><span data-stu-id="18eb2-141">To do this, you'll need to add these users to the built-in **AdminAgent** group.</span></span> <span data-ttu-id="18eb2-142">A [csoport tagjainak kezelése a](/azure/active-directory/active-directory-groups-members-azure-portal) Azure Active Directory a csoport tagjainak kezeléséhez.</span><span class="sxs-lookup"><span data-stu-id="18eb2-142">See [Manage the members for a group in Azure Active Directory](/azure/active-directory/active-directory-groups-members-azure-portal) for information about how to do this.</span></span>

## <a name="connect-with-us"></a><span data-ttu-id="18eb2-143">Lépjen velünk kapcsolatba</span><span class="sxs-lookup"><span data-stu-id="18eb2-143">Connect with us</span></span>

- <span data-ttu-id="18eb2-144">Kérdése van?</span><span class="sxs-lookup"><span data-stu-id="18eb2-144">Questions?</span></span> <span data-ttu-id="18eb2-145">Küldjön e-mailt a címre azgovcsp@microsoft.com</span><span class="sxs-lookup"><span data-stu-id="18eb2-145">Email us at azgovcsp@microsoft.com</span></span>

- <span data-ttu-id="18eb2-146">Csatlakozás a [Yammerhez](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=11509777)</span><span class="sxs-lookup"><span data-stu-id="18eb2-146">Join us on [Yammer](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=11509777)</span></span>

## <a name="next-steps"></a><span data-ttu-id="18eb2-147">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="18eb2-147">Next steps</span></span>

- [<span data-ttu-id="18eb2-148">A Microsoft Cloud for US Government Partnerközpontja</span><span class="sxs-lookup"><span data-stu-id="18eb2-148">Partner Center for Microsoft Cloud for US Government</span></span>](partner-center-for-microsoft-us-govt-cloud.md)

- [<span data-ttu-id="18eb2-149">Felhasználók és licencek kezelése Partnerközpont a Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="18eb2-149">User and license management in Partner Center for Microsoft Cloud for US Government</span></span>](user-management-in-partner-center-for-microsoft-us-govt-cloud.md)