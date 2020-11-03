---
title: További bérlők hozzáadása a partner Center-fiókhoz
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan adhat hozzá, összevonhat vagy kezelhet több Azure AD-bérlőt a partner Center-fiókban. Ismerje meg az egyes okokat is, amelyeket érdemes megtennie.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530511"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="7d729-104">Több bérlő hozzáadása és kezelése a partner Center-fiókban</span><span class="sxs-lookup"><span data-stu-id="7d729-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="7d729-105">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="7d729-105">**Applies to**</span></span>

- <span data-ttu-id="7d729-106">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="7d729-106">Partner Center</span></span>

<span data-ttu-id="7d729-107">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="7d729-107">**Appropriate roles**</span></span>

- <span data-ttu-id="7d729-108">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="7d729-108">Global admin</span></span>

<span data-ttu-id="7d729-109">Ez a funkció lehetővé teszi több, a vállalathoz tartozó bérlő kezelését és konszolidálását a Partnerközpont-fiókban.</span><span class="sxs-lookup"><span data-stu-id="7d729-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="7d729-110">Számos oka lehet annak, hogy több Azure AD-bérlőt kell kezelnie a partner Center-fiókjában.</span><span class="sxs-lookup"><span data-stu-id="7d729-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="7d729-111">Például:</span><span class="sxs-lookup"><span data-stu-id="7d729-111">For example:</span></span>

- <span data-ttu-id="7d729-112">A vállalat megvásárolhat egy másik vállalatot, és azt szeretné, hogy az új vállalat alkalmazottai használni tudják a partner centert.</span><span class="sxs-lookup"><span data-stu-id="7d729-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="7d729-113">Azonban azt szeretné, hogy a két vállalat külön maradjon.</span><span class="sxs-lookup"><span data-stu-id="7d729-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="7d729-114">Ebben az esetben az új vállalati Azure AD-bérlőt a partner globális fiókjával (PGA) társíthatja.</span><span class="sxs-lookup"><span data-stu-id="7d729-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="7d729-115">Ez a társítás azt teszi lehetővé, hogy mindkét vállalat felhasználói működjenek a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="7d729-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="7d729-116">Ha több Bérlővel is futtatja vállalkozását (pl.: contoso.com, contoso.uk, contoso.in), a több-bérlős használatával összekapcsolhatja őket ugyanazzal a PC-fiókkal.</span><span class="sxs-lookup"><span data-stu-id="7d729-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="7d729-117">Az egyesülések és a beszerzések esetében több bérlőt kell használni (például ha a contoso a Fabrikamt szerezte be, akkor mindkét Constoso.com és a Fabrikam.com megfelelő bérlőt kell használnia).</span><span class="sxs-lookup"><span data-stu-id="7d729-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="7d729-118">A bérlők bármelyikének a következőket kell tudnia:</span><span class="sxs-lookup"><span data-stu-id="7d729-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="7d729-119">Partneri központ elérése képzéshez, digitális letöltésekhez, MCP-társításhoz</span><span class="sxs-lookup"><span data-stu-id="7d729-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="7d729-120">Hozzá kell rendelni a partner Center-szerepköröket, például az MPN-rendszergazdát, az ösztönzők rendszergazdáját stb.</span><span class="sxs-lookup"><span data-stu-id="7d729-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="7d729-121">Másik Azure AD-bérlő hozzáadása a fiókhoz</span><span class="sxs-lookup"><span data-stu-id="7d729-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="7d729-122">Globális rendszergazdaként jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="7d729-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="7d729-123">A **Beállítások** ikonban válassza a **Fiókbeállítások** , majd a **bérlők** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7d729-123">From the **Settings** icon, select **Account settings** and then select **Tenants** .</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="bérlők hozzárendelése"::: 

3. <span data-ttu-id="7d729-125">Válassza a **másik ad-bérlő hozzárendelése** lehetőséget, és jelölje ki a hozzárendelni kívánt bérlőt.</span><span class="sxs-lookup"><span data-stu-id="7d729-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="7d729-126">Globális rendszergazdaként jelentkezzen be a társítani kívánt bérlőbe, és erősítse meg a társítást.</span><span class="sxs-lookup"><span data-stu-id="7d729-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="bérlők hozzárendelésének megerősítése"::: 

5. <span data-ttu-id="7d729-128">A megerősítést követően megjelenik az **összes beállított** értesítés.</span><span class="sxs-lookup"><span data-stu-id="7d729-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="7d729-129">Válassza a **Visszatérés a bérlői felügyelethez** lehetőséget, majd megjelenik az újonnan hozzáadott bérlő.</span><span class="sxs-lookup"><span data-stu-id="7d729-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="7d729-130">Nem lehet bérlőt társítani egy fiókhoz, ha már társítva van egy másik partner Center-fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="7d729-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="7d729-131">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="7d729-131">Next steps</span></span>

- [<span data-ttu-id="7d729-132">Felhasználók hozzáadása</span><span class="sxs-lookup"><span data-stu-id="7d729-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
