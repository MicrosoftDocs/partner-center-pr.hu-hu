---
title: Bérlők hozzáadása a partner Center-fiókhoz
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan adhat hozzá, összevonhat vagy kezelhet több Azure AD-bérlőt a partner Center-fiókban, és megtudhatja, miért érdemes ezt megtenni.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124805"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="ced8b-103">Több bérlő hozzáadása és kezelése a partner Center-fiókban</span><span class="sxs-lookup"><span data-stu-id="ced8b-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="ced8b-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="ced8b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ced8b-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="ced8b-105">Global admin</span></span>
- <span data-ttu-id="ced8b-106">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="ced8b-106">Account admin</span></span>

<span data-ttu-id="ced8b-107">Ez a cikk azt ismerteti, hogyan lehet összevonni több Azure Active Directory (Azure AD) bérlőt a vállalat számára, majd a partner Center-fiókban felvenni és felügyelni azokat.</span><span class="sxs-lookup"><span data-stu-id="ced8b-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="ced8b-108">Ennek számos oka van.</span><span class="sxs-lookup"><span data-stu-id="ced8b-108">There are many reasons to do so.</span></span> <span data-ttu-id="ced8b-109">Például:</span><span class="sxs-lookup"><span data-stu-id="ced8b-109">For example:</span></span>

- <span data-ttu-id="ced8b-110">Tegyük fel, hogy vállalata, a contoso, megszerezte a fabrikam egy másik vállalatát.</span><span class="sxs-lookup"><span data-stu-id="ced8b-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="ced8b-111">Azt szeretné, hogy a két vállalat külön maradjon, de azt szeretné, hogy az új alkalmazottak használni tudják a partner centert.</span><span class="sxs-lookup"><span data-stu-id="ced8b-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="ced8b-112">Ebben az esetben az új vállalati Azure AD-bérlőt a partner globális fiókjával (PGA) társítja.</span><span class="sxs-lookup"><span data-stu-id="ced8b-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="ced8b-113">Ez a társítás lehetővé teszi, hogy mindkét vállalat felhasználói működjenek a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="ced8b-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="ced8b-114">Ha több Bérlővel is futtatja vállalkozását (például *contoso.com*, *contoso.uk* és *contoso.in*), a bérlős segítségével csoportosíthatja azokat ugyanazon a számítógép-fiókban.</span><span class="sxs-lookup"><span data-stu-id="ced8b-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="ced8b-115">Ha az összeolvadások és a beszerzések irányelvei megkövetelik, hogy mindkét vállalat bérlői is működjenek, akkor a *constoso.com* és a *fabrikam.com* bérlőket is használni fogja.</span><span class="sxs-lookup"><span data-stu-id="ced8b-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="ced8b-116">A bérlők felhasználói számára a következőket kell tudnia:</span><span class="sxs-lookup"><span data-stu-id="ced8b-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="ced8b-117">A Microsoft Certified Professional (MCP) társításának elérése a partner centerrel.</span><span class="sxs-lookup"><span data-stu-id="ced8b-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="ced8b-118">Társítsa a partner Center-szerepköröket, például a Microsoft Partner Network (MPN) rendszergazdai vagy ösztönző rendszergazdát.</span><span class="sxs-lookup"><span data-stu-id="ced8b-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="ced8b-119">Azure AD-bérlő hozzáadása a fiókjához</span><span class="sxs-lookup"><span data-stu-id="ced8b-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="ced8b-120">Jelentkezzen be globális rendszergazdaként a [Microsoft partner Centerbe](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="ced8b-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="ced8b-121">A jobb felső sarokban válassza a **Beállítások** lehetőséget, válassza a **Fiókbeállítások** lehetőséget, majd válassza a **bérlők** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ced8b-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Képernyőkép az Azure AD-profil ablaktábla hozzárendelés gombjáról."::: 

1. <span data-ttu-id="ced8b-123">Válassza a **hozzárendelés** lehetőséget, majd adja meg a hozzárendelni kívánt bérlőt.</span><span class="sxs-lookup"><span data-stu-id="ced8b-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="ced8b-124">A parancssorban jelentkezzen be globális rendszergazdaként a hozzárendelni kívánt bérlőre, majd válassza a **Confirm (megerősítés**) lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ced8b-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Képernyőkép az új Azure AD-társítás megerősítése panel megerősítés gombjáról."::: 

   <span data-ttu-id="ced8b-126">Miután megerősítette a társítást, megjelenik az **összes beállított** üzenet.</span><span class="sxs-lookup"><span data-stu-id="ced8b-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="ced8b-127">Az újonnan hozzáadott bérlő megtekintéséhez válassza a **Visszatérés a bérlői felügyeletbe** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ced8b-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="ced8b-128">Ha már társítva van egy másik partner Center-fiókkal, akkor nem lehet bérlőt társítani a fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="ced8b-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="ced8b-129">Bérlő eltávolítása a fiókból</span><span class="sxs-lookup"><span data-stu-id="ced8b-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="ced8b-130">Jelentkezzen be globális rendszergazdaként a [Microsoft partner Centerbe](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="ced8b-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="ced8b-131">A jobb felső sarokban válassza a **Beállítások** ikont, majd válassza a **Fiókbeállítások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ced8b-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="ced8b-132">A bal oldali ablaktáblán válassza a **bérlők** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ced8b-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="ced8b-133">Az **Azure ad-bérlők kezelése** területen válassza a **partner** lapot.</span><span class="sxs-lookup"><span data-stu-id="ced8b-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="ced8b-134">Válassza az **Eltávolítás** lehetőséget azon bérlő mellett, amelynek társítását el szeretné távolítani.</span><span class="sxs-lookup"><span data-stu-id="ced8b-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Képernyőkép az aktuális bérlői társításokról és azok eltávolítási kapcsolatairól.":::

   <span data-ttu-id="ced8b-136">Ahogy az előző képernyőképen is látható, az **eltávolítási** hivatkozások minden társított bérlőhöz engedélyezve vannak, kivéve az elsődleges bérlőt és a bérlőt, amelyre jelenleg bejelentkezett.</span><span class="sxs-lookup"><span data-stu-id="ced8b-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="ced8b-137">Ha eltávolít egy bérlőt, az adott bérlő felhasználói már nem férnek hozzá a partner Center-fiókhoz, és az Eltávolítás hatással lehet a kompetenciára.</span><span class="sxs-lookup"><span data-stu-id="ced8b-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="ced8b-138">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ced8b-138">Next steps</span></span>

- [<span data-ttu-id="ced8b-139">Felhasználói fiókok létrehozása</span><span class="sxs-lookup"><span data-stu-id="ced8b-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






