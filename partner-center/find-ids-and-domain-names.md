---
title: Bérlőazonosító, tartománynév, felhasználói objektumazonosító megkeresása
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan találhat azonosítókat a Azure Portal a szervezet Azure AD-bérlőazonosítóját, tartománynevét vagy adott felhasználói objektumazonosítóját. Egyes feladatoknak szüksége van erre az információra.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740284"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="e6a90-104">Felhasználó fontos azonosítóinak megkeresve</span><span class="sxs-lookup"><span data-stu-id="e6a90-104">Locate important IDs for a user</span></span>

<span data-ttu-id="e6a90-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="e6a90-105">**Appropriate roles**</span></span>

- <span data-ttu-id="e6a90-106">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="e6a90-106">Global admin</span></span>

<span data-ttu-id="e6a90-107">Ez a cikk azt ismerteti, hogyan használhatja [Azure Portal](https://portal.azure.com/) segítségével a következő információkat keresheti meg egy felhasználó számára:</span><span class="sxs-lookup"><span data-stu-id="e6a90-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="e6a90-108">A Microsoft Azure Active Directory szervezet vagy vállalat Microsoft Azure Active Directory (Azure AD) bérlőazonosítója</span><span class="sxs-lookup"><span data-stu-id="e6a90-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="e6a90-109">Az Azure AD-bérlőhöz társított szervezet vagy vállalat elsődleges tartományneve</span><span class="sxs-lookup"><span data-stu-id="e6a90-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="e6a90-110">A felhasználói objektum azonosítója</span><span class="sxs-lookup"><span data-stu-id="e6a90-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="e6a90-111">Keresse meg Microsoft Azure AD bérlőazonosítót és az elsődleges tartománynevet</span><span class="sxs-lookup"><span data-stu-id="e6a90-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="e6a90-112">Az alábbi lépéseket követve keresse meg az Azure AD-bérlőazonosítót vagy az elsődleges tartománynevet a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="e6a90-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="e6a90-113">(Ha programozott módon szeretné megtalálni a bérlőazonosítót, tekintse meg a bérlőazonosító PowerShell vagy parancssori felület használatával [történő keresését.)](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="e6a90-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="e6a90-114">A bérlőazonosító más neveket is nevezhet a különböző alkalmazásokban vagy erőforrásokban.</span><span class="sxs-lookup"><span data-stu-id="e6a90-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="e6a90-115">A bérlőazonosítóra hivatkozhat például címtár-azonosítónak, Azure Active Directory-bérlőnek (Azure AD-bérlőnek), Microsoft-azonosítónak, vagy bizonyos jelentéseknek, még a *tenantguid-nek is.*</span><span class="sxs-lookup"><span data-stu-id="e6a90-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="e6a90-116">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e6a90-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="e6a90-117">Válassza **Azure Active Directory** lehetőséget a menüből.</span><span class="sxs-lookup"><span data-stu-id="e6a90-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Megjeleníti Azure Portal menü Azure Active Directory lehetőség kiválasztását.":::

3. <span data-ttu-id="e6a90-119">Megjelenik Azure Active Directory **Áttekintés** lap.</span><span class="sxs-lookup"><span data-stu-id="e6a90-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="e6a90-120">Az Azure AD-bérlőazonosító vagy az elsődleges  tartománynév kereséséhez keresse meg a Bérlőazonosító mezőt és az **Elsődleges tartomány** mezőt.</span><span class="sxs-lookup"><span data-stu-id="e6a90-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="e6a90-121">Ezek a mezők a Bérlő adatai szakaszban jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="e6a90-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Az Áttekintés oldalt jeleníti meg két kiemelt mezővel, a bérlőazonosítóval és az elsődleges tartománynévvel.":::

4. <span data-ttu-id="e6a90-123">A bérlőazonosítót a Azure Portal más módokon is megkeresheti.</span><span class="sxs-lookup"><span data-stu-id="e6a90-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="e6a90-124">Válassza **Azure Active Directory** lehetőséget a menüből.</span><span class="sxs-lookup"><span data-stu-id="e6a90-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="e6a90-125">Ezután keresse meg a **Kezelés szakaszt** a menüben, és válassza a **Tulajdonságok lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e6a90-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="e6a90-126">A Tulajdonságok lapon a felhasználóhoz társított bérlőazonosító is megjelenik.</span><span class="sxs-lookup"><span data-stu-id="e6a90-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Megjeleníti a Tulajdonságok lapot a kiemelt Bérlőazonosító mezővel.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="e6a90-128">A felhasználói objektum azonosítójának megkeresása</span><span class="sxs-lookup"><span data-stu-id="e6a90-128">Find the user object ID</span></span>

<span data-ttu-id="e6a90-129">Előfordulhat, hogy a tartománynév és a bérlőazonosító megkeresása nem mindig elég.</span><span class="sxs-lookup"><span data-stu-id="e6a90-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="e6a90-130">Előfordulhat, hogy meg kell találnia a felhasználóhoz rendelt objektumazonosítót is.</span><span class="sxs-lookup"><span data-stu-id="e6a90-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="e6a90-131">Kövesse az alábbi lépéseket, hogy megtalálja a felhasználó objektumazonosítóját a Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="e6a90-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="e6a90-132">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e6a90-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="e6a90-133">Válassza **Azure Active Directory** lehetőséget a menüből.</span><span class="sxs-lookup"><span data-stu-id="e6a90-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="e6a90-134">Keresse meg **a Kezelés** szakaszt a menüben, majd válassza a **Felhasználók lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e6a90-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Megjeleníti Azure Active Directory menüt, kiemelt Felhasználók lehetőséggel.":::

4. <span data-ttu-id="e6a90-136">A Felhasználók lapon írja be a felhasználó nevét a keresőmezőbe.</span><span class="sxs-lookup"><span data-stu-id="e6a90-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Megjeleníti a Felhasználók lapot egy keresőmezővel, amely egy adott felhasználót keres.":::

5. <span data-ttu-id="e6a90-138">Válassza ki a felhasználó nevét, ahol az megjelenik a listában.</span><span class="sxs-lookup"><span data-stu-id="e6a90-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="A Keresett felhasználóhoz egy sort megjelenítő Felhasználó oldalt jelenít meg.":::

6. <span data-ttu-id="e6a90-140">Keresse meg az Identitás szakaszt a felhasználó Profil lapján.</span><span class="sxs-lookup"><span data-stu-id="e6a90-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="e6a90-141">Az Objektumazonosító mező itt jelenik meg a felhasználó egyedi objektumazonosítójával.</span><span class="sxs-lookup"><span data-stu-id="e6a90-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Megjeleníti a Felhasználói profil oldalt az Identitás szakaszsal és az objektumazonosító egy kiemelt mezőjével.":::

## <a name="next-steps"></a><span data-ttu-id="e6a90-143">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="e6a90-143">Next steps</span></span>

- [<span data-ttu-id="e6a90-144">A bérlőazonosító programozott módon történő megkeresés a PowerShell vagy a parancssori felület használatával</span><span class="sxs-lookup"><span data-stu-id="e6a90-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="e6a90-145">További információ a felhasználói profilokról a Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e6a90-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="e6a90-146">Ismerje meg, hogyan láthatják vagy exportálják a partnerek az ügyféladatokat a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="e6a90-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

