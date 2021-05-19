---
title: Bérlők hozzáadása a Partnerközpont fiókjához
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan adhat hozzá, konszolidálhat vagy kezelhet több Azure AD-bérlőt Partnerközpont-fiókjában, és megtudhatja, miért érdemes ezt megtennie.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151202"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="bfd8d-103">Több bérlő hozzáadása és kezelése a Partnerközpont fiókjában</span><span class="sxs-lookup"><span data-stu-id="bfd8d-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="bfd8d-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Fiók adminisztrátora</span><span class="sxs-lookup"><span data-stu-id="bfd8d-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="bfd8d-105">Ez a cikk azt ismerteti, hogyan konszolidálhat több Azure Active Directory -bérlőt (Azure AD-bérlőt) a vállalat számára, majd hogyan adjuk hozzá és felügyelhetjük őket a Partnerközpont fiókjában.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="bfd8d-106">Ennek számos oka lehet.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-106">There are many reasons to do so.</span></span> <span data-ttu-id="bfd8d-107">Például:</span><span class="sxs-lookup"><span data-stu-id="bfd8d-107">For example:</span></span>

- <span data-ttu-id="bfd8d-108">Tegyük fel, hogy vállalata, a Contoso megvásárolt egy másik vállalatot, a Fabrikamot.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="bfd8d-109">Azt szeretné, hogy a két vállalat elkülönülő maradjon, de azt szeretné, hogy az új alkalmazottak használni tudják a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="bfd8d-110">Ebben az esetben az új vállalat Azure AD-bérlőjéhez társítja a globális partnerfiókját (PGA).</span><span class="sxs-lookup"><span data-stu-id="bfd8d-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="bfd8d-111">Ez a társítás lehetővé teszi, hogy a felhasználók mindkét vállalatnál a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="bfd8d-112">Ha a vállalkozását több bérlővel (például *contoso.com,* *contoso.uk* és *contoso.in)* futtatja, több-bérlős rendszerekkel csoportosíthatja őket ugyanabban a számítógépfiókban.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="bfd8d-113">Ha az összeolvadással és felvásárlással kapcsolatos irányelvek megkövetelik, hogy  mindkét vállalat bérlőivel dolgozzon, akkor a constoso.com és fabrikam.com *bérlőket* is használnia kell.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="bfd8d-114">Bármely bérlő felhasználóinak képesnek kell lennie a következőre:</span><span class="sxs-lookup"><span data-stu-id="bfd8d-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="bfd8d-115">Hozzáférés Partnerközpont képzéshez, digitális letöltéshez vagy Microsoft Certified Professional (MCP) társításhoz.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="bfd8d-116">Olyan szerepkörhöz Partnerközpont, mint Microsoft Partner Network (MPN) rendszergazda vagy ösztönzők rendszergazdája.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="bfd8d-117">Azure AD-bérlő hozzáadása a fiókhoz</span><span class="sxs-lookup"><span data-stu-id="bfd8d-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="bfd8d-118">Jelentkezzen be globális rendszergazdaként a [Microsoft Partnerközpont.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="bfd8d-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="bfd8d-119">A jobb felső sarokban válassza a **Beállítások,** a **Fiókbeállítások** lehetőséget, majd a **Bérlők lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="bfd8d-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Képernyőkép az Azure AD-profil panel Társítás gombjáról."::: 

1. <span data-ttu-id="bfd8d-121">Válassza **a Társítás** lehetőséget, majd jelölje ki a társítani kívánt bérlőt.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="bfd8d-122">Amikor a rendszer kéri, jelentkezzen be globális rendszergazdaként a társítani kívánt bérlőbe, majd válassza a **Megerősítés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="bfd8d-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Képernyőkép a Confirm (Megerősítés) gombról a Confirm new Azure AD association (Új Azure AD társítás megerősítése) panelen."::: 

   <span data-ttu-id="bfd8d-124">Miután megerősítette a társítást, megjelenik a **Minden beállítva** üzenet.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="bfd8d-125">Az újonnan hozzáadott bérlő megtekintéséhez válassza a Visszatérés a **bérlőkezeléshez lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="bfd8d-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="bfd8d-126">Nem társíthat bérlőt egy fiókhoz, ha már társítva van egy másik Partnerközpont fiókkal.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="bfd8d-127">Bérlő eltávolítása a fiókból</span><span class="sxs-lookup"><span data-stu-id="bfd8d-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="bfd8d-128">Jelentkezzen be globális rendszergazdaként a [Microsoft Partnerközpont.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="bfd8d-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="bfd8d-129">A jobb felső sarokban válassza a **Beállítások ikont,** majd a **Fiókbeállítások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="bfd8d-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="bfd8d-130">A bal oldali panelen válassza a **Bérlők lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="bfd8d-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="bfd8d-131">Az **Azure AD-bérlők kezelése alatt** válassza a **Partner** lapot.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="bfd8d-132">Válassza **az Eltávolítás** lehetőséget azon bérlő mellett, amelynek társítását el szeretné távolítani.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Képernyőkép az aktuális bérlői társításról és azok Eltávolítás hivatkozásairól.":::

   <span data-ttu-id="bfd8d-134">Ahogy az előző képernyőképen  is látható, a Hivatkozások eltávolítása lehetőség engedélyezve van az összes társított bérlőn, kivéve az elsődleges bérlőt és azt a bérlőt, amelybe jelenleg be van jelentkezve.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="bfd8d-135">Bérlő eltávolításakor a bérlő felhasználói már nem férhetnek hozzá a Partnerközpont-fiókhoz, és az eltávolítás hatással lehet a kompetenciákra.</span><span class="sxs-lookup"><span data-stu-id="bfd8d-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="bfd8d-136">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="bfd8d-136">Next steps</span></span>

- [<span data-ttu-id="bfd8d-137">Felhasználói fiókok létrehozása</span><span class="sxs-lookup"><span data-stu-id="bfd8d-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






