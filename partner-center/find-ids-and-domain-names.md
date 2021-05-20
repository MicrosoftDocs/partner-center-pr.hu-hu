---
title: Bérlőazonosító, tartománynév, felhasználói objektumazonosító megkeresása
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan találhat azonosítókat a Azure Portal a szervezet Azure AD-bérlőazonosítóját, tartománynevét vagy adott felhasználói objektumazonosítóját. Néhány feladatnak szüksége van erre az információra.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150862"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="45ec4-104">Felhasználó fontos azonosítóinak megkereste</span><span class="sxs-lookup"><span data-stu-id="45ec4-104">Locate important IDs for a user</span></span>

<span data-ttu-id="45ec4-105">**Megfelelő szerepkörök:** Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="45ec4-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="45ec4-106">Ez a cikk bemutatja, hogyan keresheti meg [Azure Portal](https://portal.azure.com/) felhasználóra vonatkozó alábbi információkat a jelen témakörben:</span><span class="sxs-lookup"><span data-stu-id="45ec4-106">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="45ec4-107">A Microsoft Azure Active Directory szervezet vagy vállalat Microsoft Azure Active Directory (Azure AD) bérlőazonosítója</span><span class="sxs-lookup"><span data-stu-id="45ec4-107">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="45ec4-108">Az Azure AD-bérlőhöz társított szervezet vagy vállalat elsődleges tartományneve</span><span class="sxs-lookup"><span data-stu-id="45ec4-108">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="45ec4-109">A felhasználói objektum azonosítója</span><span class="sxs-lookup"><span data-stu-id="45ec4-109">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="45ec4-110">Keresse meg Microsoft Azure AD bérlőazonosítóját és elsődleges tartománynevét</span><span class="sxs-lookup"><span data-stu-id="45ec4-110">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="45ec4-111">Az alábbi lépésekkel keresheti meg az Azure AD-bérlőazonosítót vagy az elsődleges tartománynevet a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="45ec4-111">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="45ec4-112">(Ha programozott módon szeretné megtalálni a bérlőazonosítót, tekintse meg a bérlőazonosító PowerShell vagy parancssori felület használatával [történő megkeresését.)](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="45ec4-112">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="45ec4-113">A bérlőazonosító más néven is hívható a különböző alkalmazásokban vagy erőforrásokban.</span><span class="sxs-lookup"><span data-stu-id="45ec4-113">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="45ec4-114">A bérlőazonosítóra hivatkozhat például címtár-azonosítónak, Azure Active Directory-bérlőnek (Azure AD-bérlőnek), Microsoft-azonosítónak, vagy bizonyos jelentéseknek, még a *tenantguid-nak is.*</span><span class="sxs-lookup"><span data-stu-id="45ec4-114">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="45ec4-115">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="45ec4-115">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="45ec4-116">Válassza **Azure Active Directory** lehetőséget a menüből.</span><span class="sxs-lookup"><span data-stu-id="45ec4-116">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Megjeleníti Azure Portal menüben Azure Active Directory lehetőség kiválasztását.":::

3. <span data-ttu-id="45ec4-118">Megjelenik Azure Active Directory **Áttekintés** lap.</span><span class="sxs-lookup"><span data-stu-id="45ec4-118">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="45ec4-119">Az Azure AD-bérlőazonosító vagy az elsődleges  tartománynév megkereséhez keresse meg a Bérlőazonosító mezőt és az **Elsődleges tartomány** mezőt.</span><span class="sxs-lookup"><span data-stu-id="45ec4-119">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="45ec4-120">Ezek a mezők a Bérlő adatai szakaszban jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="45ec4-120">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Az Áttekintés oldalt jeleníti meg két kiemelt mezővel, a bérlőazonosítóval és az elsődleges tartománynévvel.":::

4. <span data-ttu-id="45ec4-122">A bérlőazonosítót a Azure Portal más módokon is megkeresheti.</span><span class="sxs-lookup"><span data-stu-id="45ec4-122">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="45ec4-123">Válassza **Azure Active Directory** lehetőséget a menüből.</span><span class="sxs-lookup"><span data-stu-id="45ec4-123">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="45ec4-124">Ezután keresse meg a **Kezelés szakaszt** a menüben, és válassza a **Tulajdonságok lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="45ec4-124">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="45ec4-125">A Tulajdonságok lapon a felhasználóhoz társított bérlőazonosító is megjelenik.</span><span class="sxs-lookup"><span data-stu-id="45ec4-125">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Megjeleníti a Tulajdonságok lapot a kiemelt Bérlőazonosító mezővel.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="45ec4-127">A felhasználói objektum azonosítójának megkeresása</span><span class="sxs-lookup"><span data-stu-id="45ec4-127">Find the user object ID</span></span>

<span data-ttu-id="45ec4-128">Előfordulhat, hogy a tartománynév és a bérlőazonosító megkeresása nem mindig elég.</span><span class="sxs-lookup"><span data-stu-id="45ec4-128">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="45ec4-129">Előfordulhat, hogy meg kell találnia a felhasználóhoz rendelt adott objektumazonosítót is.</span><span class="sxs-lookup"><span data-stu-id="45ec4-129">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="45ec4-130">Kövesse az alábbi lépéseket, hogy megtalálja a felhasználó objektumazonosítóját a Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="45ec4-130">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="45ec4-131">Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="45ec4-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="45ec4-132">Válassza **Azure Active Directory** lehetőséget a menüből.</span><span class="sxs-lookup"><span data-stu-id="45ec4-132">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="45ec4-133">Keresse meg **a Kezelés** szakaszt a menüben, majd válassza a **Felhasználók lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="45ec4-133">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Megjeleníti Azure Active Directory menüt a Kiemelt Felhasználók lehetőséggel.":::

4. <span data-ttu-id="45ec4-135">A Felhasználók lapon írja be a felhasználó nevét a keresőmezőbe.</span><span class="sxs-lookup"><span data-stu-id="45ec4-135">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Megjeleníti a Felhasználók lapot egy adott felhasználó keresésére vonatkozó keresőmezővel.":::

5. <span data-ttu-id="45ec4-137">Válassza ki a felhasználó nevét, ahol az megjelenik a listában.</span><span class="sxs-lookup"><span data-stu-id="45ec4-137">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Megjeleníti a Felhasználó lapot, amely megjelenít egy sort a keresett felhasználó számára.":::

6. <span data-ttu-id="45ec4-139">Keresse meg az Identitás szakaszt a felhasználó Profil lapján.</span><span class="sxs-lookup"><span data-stu-id="45ec4-139">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="45ec4-140">Itt megjelenik az Objektumazonosító mező a felhasználó egyedi objektumazonosítójával.</span><span class="sxs-lookup"><span data-stu-id="45ec4-140">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Megjeleníti a Felhasználói profil oldalt az Identitás szakaszsal, valamint egy kiemelt mezőt az objektumazonosítóhoz.":::

## <a name="next-steps"></a><span data-ttu-id="45ec4-142">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="45ec4-142">Next steps</span></span>

- [<span data-ttu-id="45ec4-143">A bérlőazonosító programozott módon történő megkeresés a PowerShell vagy a parancssori felület használatával</span><span class="sxs-lookup"><span data-stu-id="45ec4-143">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="45ec4-144">További információ a felhasználói profilokról a Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="45ec4-144">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="45ec4-145">Ismerje meg, hogyan láthatják vagy exportálják a partnerek az ügyfelek adatait a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="45ec4-145">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

