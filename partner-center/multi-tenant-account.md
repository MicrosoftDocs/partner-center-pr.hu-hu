---
title: További bérlők hozzáadása a partner Center-fiókhoz
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan adhat hozzá, összevonhat vagy kezelhet több Azure AD-bérlőt a partner Center-fiókban. Ismerje meg az egyes okokat is, amelyeket érdemes megtennie.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105552"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="085eb-104">Több bérlő hozzáadása és kezelése a partner Center-fiókban</span><span class="sxs-lookup"><span data-stu-id="085eb-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="085eb-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="085eb-105">**Appropriate roles**</span></span>

- <span data-ttu-id="085eb-106">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="085eb-106">Global admin</span></span>

<span data-ttu-id="085eb-107">Ez a funkció lehetővé teszi több, a vállalathoz tartozó bérlő kezelését és konszolidálását a Partnerközpont-fiókban.</span><span class="sxs-lookup"><span data-stu-id="085eb-107">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="085eb-108">Számos oka lehet annak, hogy több Azure AD-bérlőt kell kezelnie a partner Center-fiókjában.</span><span class="sxs-lookup"><span data-stu-id="085eb-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="085eb-109">Például:</span><span class="sxs-lookup"><span data-stu-id="085eb-109">For example:</span></span>

- <span data-ttu-id="085eb-110">A vállalat megvásárolhat egy másik vállalatot, és azt szeretné, hogy az új vállalat alkalmazottai használni tudják a partner centert.</span><span class="sxs-lookup"><span data-stu-id="085eb-110">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="085eb-111">Azonban azt szeretné, hogy a két vállalat külön maradjon.</span><span class="sxs-lookup"><span data-stu-id="085eb-111">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="085eb-112">Ebben az esetben az új vállalati Azure AD-bérlőt a partner globális fiókjával (PGA) társíthatja.</span><span class="sxs-lookup"><span data-stu-id="085eb-112">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="085eb-113">Ez a társítás azt teszi lehetővé, hogy mindkét vállalat felhasználói működjenek a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="085eb-113">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="085eb-114">Ha több Bérlővel is futtatja vállalkozását (pl.: contoso.com, contoso.uk, contoso.in), a több-bérlős használatával összekapcsolhatja őket ugyanazzal a PC-fiókkal.</span><span class="sxs-lookup"><span data-stu-id="085eb-114">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="085eb-115">Az egyesülések és a beszerzések esetében több bérlőt kell használni (például ha a contoso a Fabrikamt szerezte be, akkor mindkét Constoso.com és a Fabrikam.com megfelelő bérlőt kell használnia).</span><span class="sxs-lookup"><span data-stu-id="085eb-115">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="085eb-116">A bérlők bármelyikének a következőket kell tudnia:</span><span class="sxs-lookup"><span data-stu-id="085eb-116">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="085eb-117">Partneri központ elérése képzéshez, digitális letöltésekhez, MCP-társításhoz</span><span class="sxs-lookup"><span data-stu-id="085eb-117">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="085eb-118">Hozzá kell rendelni a partner Center-szerepköröket, például az MPN-rendszergazdát, az ösztönzők rendszergazdáját stb.</span><span class="sxs-lookup"><span data-stu-id="085eb-118">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="085eb-119">Másik Azure AD-bérlő hozzáadása a fiókhoz</span><span class="sxs-lookup"><span data-stu-id="085eb-119">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="085eb-120">Globális rendszergazdaként jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="085eb-120">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="085eb-121">A **Beállítások** ikonban válassza a **Fiókbeállítások** , majd a **bérlők** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="085eb-121">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="bérlők hozzárendelése"::: 

3. <span data-ttu-id="085eb-123">Válassza a **másik ad-bérlő hozzárendelése** lehetőséget, és jelölje ki a hozzárendelni kívánt bérlőt.</span><span class="sxs-lookup"><span data-stu-id="085eb-123">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="085eb-124">Globális rendszergazdaként jelentkezzen be a társítani kívánt bérlőbe, és erősítse meg a társítást.</span><span class="sxs-lookup"><span data-stu-id="085eb-124">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="bérlők hozzárendelésének megerősítése"::: 

5. <span data-ttu-id="085eb-126">A megerősítést követően megjelenik az **összes beállított** értesítés.</span><span class="sxs-lookup"><span data-stu-id="085eb-126">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="085eb-127">Válassza a **Visszatérés a bérlői felügyelethez** lehetőséget, majd megjelenik az újonnan hozzáadott bérlő.</span><span class="sxs-lookup"><span data-stu-id="085eb-127">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="085eb-128">Nem lehet bérlőt társítani egy fiókhoz, ha már társítva van egy másik partner Center-fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="085eb-128">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="085eb-129">Bérlő eltávolítása a fiókból</span><span class="sxs-lookup"><span data-stu-id="085eb-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="085eb-130">Globális rendszergazdaként jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="085eb-130">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="085eb-131">A **Beállítások** ikonban válassza a **Fiókbeállítások** – > bérlők lehetőséget, és kattintson a **partner** fülre.</span><span class="sxs-lookup"><span data-stu-id="085eb-131">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="085eb-132">Kattintson az **Eltávolítás** gombra a leválasztani kívánt bérlőhöz.</span><span class="sxs-lookup"><span data-stu-id="085eb-132">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="085eb-133">A bérlők leválasztása azt jelenti, hogy a bérlő felhasználóinak többé nem lesz hozzáférésük a partner Center-fiókhoz, és ez hatással lehet a kompetenciára.</span><span class="sxs-lookup"><span data-stu-id="085eb-133">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="085eb-134">Az **Eltávolítás** gomb minden társított bérlő esetében engedélyezve van, kivéve az elsődleges bérlőt és azt a bérlőt, amelyhez jelenleg be van jelentkezve.</span><span class="sxs-lookup"><span data-stu-id="085eb-134">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="az Eltávolítás gombbal rendelkező bérlők":::
 

## <a name="next-steps"></a><span data-ttu-id="085eb-136">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="085eb-136">Next steps</span></span>

- [<span data-ttu-id="085eb-137">Felhasználók hozzáadása</span><span class="sxs-lookup"><span data-stu-id="085eb-137">Add users</span></span>](create-user-accounts-and-set-permissions.md)






