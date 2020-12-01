---
title: Bérlő AZONOSÍTÓjának, tartománynevének, felhasználói objektum AZONOSÍTÓjának megkeresése
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan kereshet azonosítókat a Azure Portalban – egy szervezet Azure AD-bérlői AZONOSÍTÓjának, tartománynevének vagy adott felhasználói objektumának AZONOSÍTÓját. Néhány feladatnak szüksége van ezekre az adatokra.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: cb0325aae30fe57a4be2be3e37bca1ee6aa1eab8
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439232"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="108a3-104">Felhasználók fontos azonosítóinak megkeresése</span><span class="sxs-lookup"><span data-stu-id="108a3-104">Locate important IDs for a user</span></span>

<span data-ttu-id="108a3-105">Ez a cikk azt ismerteti, hogyan használható a [Azure Portal](https://portal.azure.com/) az alábbi információk megkereséséhez a felhasználó számára:</span><span class="sxs-lookup"><span data-stu-id="108a3-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="108a3-106">A felhasználó szervezetének vagy vállalatának Microsoft Azure Active Directory (Azure AD) bérlői azonosítója</span><span class="sxs-lookup"><span data-stu-id="108a3-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="108a3-107">Az Azure AD-bérlőhöz társított szervezet vagy vállalat elsődleges tartományneve</span><span class="sxs-lookup"><span data-stu-id="108a3-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="108a3-108">A felhasználói objektum azonosítója</span><span class="sxs-lookup"><span data-stu-id="108a3-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="108a3-109">A Microsoft Azure AD bérlő AZONOSÍTÓjának és elsődleges tartománynevének megkeresése</span><span class="sxs-lookup"><span data-stu-id="108a3-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="108a3-110">Az alábbi lépéseket követve megkeresheti az Azure AD-bérlő AZONOSÍTÓját vagy elsődleges tartománynevét a Azure Portalon belül.</span><span class="sxs-lookup"><span data-stu-id="108a3-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="108a3-111">(Ha a bérlői azonosítót programozottan szeretné megtalálni, tekintse meg a [bérlői azonosító keresése a PowerShell vagy a CLI használatával](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)című témakört.)</span><span class="sxs-lookup"><span data-stu-id="108a3-111">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="108a3-112">A bérlői azonosító neve eltérő lehet különböző alkalmazásokban vagy erőforrásokban.</span><span class="sxs-lookup"><span data-stu-id="108a3-112">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="108a3-113">Előfordulhat például, hogy a bérlő azonosítója a címtár-azonosító, a Azure Active Directory (Azure AD) bérlő, a Microsoft-azonosító, vagy bizonyos jelentések esetében még a *tenantguid* is hivatkozik.</span><span class="sxs-lookup"><span data-stu-id="108a3-113">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="108a3-114">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="108a3-114">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="108a3-115">A menüből válassza a **Azure Active Directory** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="108a3-115">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Megjeleníti Azure Portal a menüből válassza a Azure Active Directory lehetőséget.":::

3. <span data-ttu-id="108a3-117">Megjelenik egy Azure Active Directory **áttekintő** oldal.</span><span class="sxs-lookup"><span data-stu-id="108a3-117">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="108a3-118">Az Azure AD-bérlő AZONOSÍTÓjának vagy elsődleges tartománynevének megkereséséhez keresse meg a **bérlői azonosító** mezőt és az **elsődleges tartomány** mezőt.</span><span class="sxs-lookup"><span data-stu-id="108a3-118">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="108a3-119">Ezek a mezők a bérlői adatok szakaszban jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="108a3-119">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="A két Kiemelt mezőt, a bérlői azonosítót és az elsődleges tartománynevet tartalmazó áttekintő oldalt jeleníti meg.":::

4. <span data-ttu-id="108a3-121">A bérlői azonosítót többféleképpen is megtalálhatja a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="108a3-121">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="108a3-122">A menüből válassza a **Azure Active Directory** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="108a3-122">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="108a3-123">Ezután keresse meg a **kezelés** szakaszt a menüben, majd válassza a **Tulajdonságok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="108a3-123">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="108a3-124">A Tulajdonságok lap a felhasználó társított bérlői AZONOSÍTÓját is megjeleníti.</span><span class="sxs-lookup"><span data-stu-id="108a3-124">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Megjeleníti a tulajdonságok lapot a Kiemelt bérlői azonosító mezővel.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="108a3-126">A felhasználói objektum AZONOSÍTÓjának megkeresése</span><span class="sxs-lookup"><span data-stu-id="108a3-126">Find the user object ID</span></span>

<span data-ttu-id="108a3-127">Ha csak a tartománynevet és a bérlő AZONOSÍTÓját találja, nem mindig lehet elég.</span><span class="sxs-lookup"><span data-stu-id="108a3-127">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="108a3-128">Előfordulhat, hogy meg kell keresnie egy felhasználóhoz rendelt objektumazonosító-azonosítót is.</span><span class="sxs-lookup"><span data-stu-id="108a3-128">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="108a3-129">Az alábbi lépéseket követve megkeresheti a felhasználó objektumazonosítót a Azure Portalban:</span><span class="sxs-lookup"><span data-stu-id="108a3-129">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="108a3-130">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="108a3-130">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="108a3-131">A menüből válassza a **Azure Active Directory** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="108a3-131">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="108a3-132">Keresse meg a **kezelés** szakaszt a menüben, majd válassza a **felhasználók** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="108a3-132">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Megjeleníti Azure Active Directory menüt a Kiemelt felhasználók lehetőséggel.":::

4. <span data-ttu-id="108a3-134">A felhasználók lapon írja be a felhasználó nevét a keresőmezőbe.</span><span class="sxs-lookup"><span data-stu-id="108a3-134">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Megjeleníti a felhasználók lap keresési mezőjét egy adott felhasználó kereséséhez.":::

5. <span data-ttu-id="108a3-136">Válassza ki a felhasználó nevét, ahol megjelenik a listában.</span><span class="sxs-lookup"><span data-stu-id="108a3-136">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Megjeleníti a felhasználó oldalát, amely a keresett felhasználó sorát jeleníti meg.":::

6. <span data-ttu-id="108a3-138">Keresse meg az identitás szakaszt a felhasználó profilja oldalon.</span><span class="sxs-lookup"><span data-stu-id="108a3-138">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="108a3-139">Az objektumazonosító mező itt jelenik meg a felhasználó egyedi objektumazonosító-azonosítójával.</span><span class="sxs-lookup"><span data-stu-id="108a3-139">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Megjeleníti a felhasználói profil oldalt az identitás szakaszban, valamint egy kiemelt mezőt az objektumazonosító számára.":::

## <a name="next-steps"></a><span data-ttu-id="108a3-141">További lépések</span><span class="sxs-lookup"><span data-stu-id="108a3-141">Next steps</span></span>

- [<span data-ttu-id="108a3-142">A bérlői azonosító megkeresése programozott módon a PowerShell vagy a parancssori felület használatával</span><span class="sxs-lookup"><span data-stu-id="108a3-142">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="108a3-143">További információ a Azure Active Directory felhasználói profiljairól</span><span class="sxs-lookup"><span data-stu-id="108a3-143">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="108a3-144">Megtudhatja, hogyan láthatják vagy exportálják a partnereink a partneri központban lévő vásárlói adatokat</span><span class="sxs-lookup"><span data-stu-id="108a3-144">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

