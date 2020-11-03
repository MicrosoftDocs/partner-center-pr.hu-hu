---
title: Felhasználói fiókok létrehozása és szerepkörök társítása
description: Minden alkalmazottnak hozzá kell rendelnie egy szerepkört, mielőtt hozzá tudnak férni a partner központhoz. Megtudhatja, hogyan hozhat létre felhasználói fiókokat, rendelhet hozzá szerepköröket és állíthat be engedélyeket.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/13/2020
ms.locfileid: "92530247"
---
# <a name="create-user-accounts"></a><span data-ttu-id="559db-104">Felhasználói fiókok létrehozása</span><span class="sxs-lookup"><span data-stu-id="559db-104">Create user accounts</span></span>  

<span data-ttu-id="559db-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="559db-105">**Appropriate roles**</span></span>

- <span data-ttu-id="559db-106">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="559db-106">Account admin</span></span>
- <span data-ttu-id="559db-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="559db-107">Global admin</span></span>
- <span data-ttu-id="559db-108">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="559db-108">User management admin</span></span>

<span data-ttu-id="559db-109">Hozzon létre felhasználói fiókokat azon alkalmazottak számára, akiknek hozzáférésre van szükségük a partner központhoz.</span><span class="sxs-lookup"><span data-stu-id="559db-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="559db-110">Ezeket a feladatokat a felhasználói felügyeleti rendszergazdának, a fiókok rendszergazdájának vagy a globális rendszergazdának kell elvégeznie. A feladatokat végrehajtó felhasználónak hozzá kell rendelnie a felhasználói rendszergazda vagy a globális rendszergazda Azure Active Directory (HRE) szerepkörét is.</span><span class="sxs-lookup"><span data-stu-id="559db-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="559db-111">További információ a HRE szerepköreiről: [rendszergazdai szerepkör engedélyei Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="559db-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="559db-112">Új felhasználó hozzáadása</span><span class="sxs-lookup"><span data-stu-id="559db-112">Add a new user</span></span>

1. <span data-ttu-id="559db-113">A partner központ jobb felső részén található **Beállítások** ikonban válassza a **Fiókbeállítások** , majd a **felhasználói kezelés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="559db-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management** .</span></span>

2. <span data-ttu-id="559db-114">Válassza a **Felhasználó hozzáadása** elemet.</span><span class="sxs-lookup"><span data-stu-id="559db-114">Select **Add user** .</span></span>

3. <span data-ttu-id="559db-115">Adja meg a felhasználó teljes nevét és egyedi e-mail-címét.</span><span class="sxs-lookup"><span data-stu-id="559db-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="559db-116">Válassza ki az ügynök típusát és/vagy a felhasználóhoz hozzárendelni kívánt rendszergazda típusát.</span><span class="sxs-lookup"><span data-stu-id="559db-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="559db-117">A fiókpartner-hozzáférés szerepköralapú, így engedélyeket rendelhet a felhasználó nézetének testreszabásához, hogy csak azok a funkciók jelenjenek meg, amelyekre a felhasználónak szüksége van az adott feladatok elvégzéséhez.</span><span class="sxs-lookup"><span data-stu-id="559db-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="559db-118">Ha a felhasználók szerepkör-hozzárendelést kívánnak, a globális adminisztrátorok **és a** globális rendszergazda szűrése lehetőségre kattintva megtalálhatják a kapcsolattartáshoz szükséges globális rendszergazdákat.</span><span class="sxs-lookup"><span data-stu-id="559db-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="559db-119">Kattintson a **Hozzáadás** gombra a felhasználói fiók létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="559db-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="559db-120">Erősítse meg a felhasználó adatait a következő oldalon.</span><span class="sxs-lookup"><span data-stu-id="559db-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="559db-121">Jegyezze fel az új felhasználó bejelentkezési információit ezen az oldalon.</span><span class="sxs-lookup"><span data-stu-id="559db-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="559db-122">Ügyeljen arra, hogy ezeket az adatokat az új felhasználónak másolja és küldje el, mivel később nem fogja tudni elérni.</span><span class="sxs-lookup"><span data-stu-id="559db-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="559db-123">A felhasználónak felhasználónevével és ideiglenes jelszavával be kell jelentkeznie a partner központba.</span><span class="sxs-lookup"><span data-stu-id="559db-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="559db-124">Amikor a felhasználó első alkalommal jelentkezik be a partner központba, a rendszer felszólítja a jelszó módosítására.</span><span class="sxs-lookup"><span data-stu-id="559db-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="559db-125">Felhasználói szerepkörök kiosztása</span><span class="sxs-lookup"><span data-stu-id="559db-125">Assign user roles</span></span>

<span data-ttu-id="559db-126">A partner Centerben való működéshez hozzárendelt szerepkörrel kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="559db-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="559db-127">A szerepkörök jelenleg Azure Active Directory bérlői szerepköröket, a Cloud Solution Provider (CSP) szerepköröket, valamint a nem HRE vállalati szerepköröket tartalmazzák.</span><span class="sxs-lookup"><span data-stu-id="559db-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="559db-128">Az egyes vállalatok igénybe vehetik az összes ilyen szerepkört.</span><span class="sxs-lookup"><span data-stu-id="559db-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="559db-129">A partneri központ eléréséhez a bérlőnek szerepelnie kell az egyéni felhasználók listáján.</span><span class="sxs-lookup"><span data-stu-id="559db-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="559db-130">A szerepkör-hozzárendelések további hozzáférést biztosítanak.</span><span class="sxs-lookup"><span data-stu-id="559db-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="559db-131">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="559db-131">Next steps</span></span>

- [<span data-ttu-id="559db-132">Felhasználói szerepkörök és engedélyek kiosztása a partner Centerben való működéshez szükséges alkalmazottak számára</span><span class="sxs-lookup"><span data-stu-id="559db-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
