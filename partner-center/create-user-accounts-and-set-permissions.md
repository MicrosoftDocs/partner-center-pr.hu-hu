---
title: Felhasználói fiókok létrehozása és szerepkörök hozzárendelése
description: Minden alkalmazotthoz hozzá kell rendelni egy szerepkört, mielőtt hozzáférhet Partnerközpont. Megtudhatja, hogyan hozhat létre felhasználói fiókokat, hogyan rendelhet hozzá szerepköröket és állíthatja be az engedélyeket.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148142"
---
# <a name="create-user-accounts"></a><span data-ttu-id="c474a-104">Felhasználói fiókok létrehozása</span><span class="sxs-lookup"><span data-stu-id="c474a-104">Create user accounts</span></span>  

<span data-ttu-id="c474a-105">**Megfelelő szerepkörök:** Fiók-rendszergazdai | Globális rendszergazdai | Felhasználókezelő rendszergazda</span><span class="sxs-lookup"><span data-stu-id="c474a-105">**Appropriate roles**: Account admin | Global admin | User management admin</span></span>

<span data-ttu-id="c474a-106">Hozzon létre felhasználói fiókokat az olyan alkalmazottak számára, akiknek hozzáférésre van szükségük a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="c474a-106">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="c474a-107">Ezeket a feladatokat a felhasználókezelő rendszergazdának, a fiók rendszergazdának vagy a globális rendszergazdának kell elvégeznie. A feladatokat végző felhasználóhoz hozzá kell rendelni a felhasználói rendszergazda Azure Active Directory (AAD) szerepköreit is, globális rendszergazda.</span><span class="sxs-lookup"><span data-stu-id="c474a-107">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="c474a-108">További információ az AAD-szerepkörökről: Rendszergazdai szerepkör engedélyei a [Azure Active Directory.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)</span><span class="sxs-lookup"><span data-stu-id="c474a-108">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="c474a-109">Új felhasználó hozzáadása</span><span class="sxs-lookup"><span data-stu-id="c474a-109">Add a new user</span></span>

1. <span data-ttu-id="c474a-110">A jobb **felső sarokban** található Beállítások Partnerközpont válassza a Fiókbeállítások,  majd a **Felhasználókezelés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c474a-110">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="c474a-111">Válassza a **Felhasználó hozzáadása** elemet.</span><span class="sxs-lookup"><span data-stu-id="c474a-111">Select **Add user**.</span></span>

3. <span data-ttu-id="c474a-112">Adja meg a felhasználó teljes nevét és egyedi e-mail-címét.</span><span class="sxs-lookup"><span data-stu-id="c474a-112">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="c474a-113">Válassza ki az ügynök és/vagy a felhasználóhoz hozzárendelni kívánt rendszergazda típusát.</span><span class="sxs-lookup"><span data-stu-id="c474a-113">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="c474a-114">Partnerközpont hozzáférés szerepköralapú, így engedélyeket rendelhet a felhasználói nézet testreszabásához, hogy csak a felhasználó által meghatározott feladatok elvégzéséhez szükséges funkciókat mutassa.</span><span class="sxs-lookup"><span data-stu-id="c474a-114">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="c474a-115">Ha a felhasználók szerepkör-hozzárendelést keresnek, a Felhasználókezelés és szűrés a globális rendszergazda számára oldalon találhatják meg a kapcsolatot a globális rendszergazdákkal. </span><span class="sxs-lookup"><span data-stu-id="c474a-115">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="c474a-116">Kattintson a **Hozzáadás** gombra a felhasználói fiók létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="c474a-116">Select **Add** to create the user account.</span></span> <span data-ttu-id="c474a-117">A következő oldalon erősítse meg a felhasználó adatait.</span><span class="sxs-lookup"><span data-stu-id="c474a-117">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="c474a-118">Jegyezze fel az új felhasználó ezen az oldalon megjelenő bejelentkezési adatait.</span><span class="sxs-lookup"><span data-stu-id="c474a-118">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="c474a-119">Másolja ki és küldje el ezt az információt az új felhasználónak, mert később nem fogja tudni ismét elérni.</span><span class="sxs-lookup"><span data-stu-id="c474a-119">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="c474a-120">A felhasználónak be kell jelentkeznie a Partnerközpont a felhasználónevét és ideiglenes jelszavát.</span><span class="sxs-lookup"><span data-stu-id="c474a-120">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="c474a-121">Amikor a felhasználó először jelentkezik be a Partnerközpont, a rendszer kérni fogja, hogy változtassa meg a jelszavát.</span><span class="sxs-lookup"><span data-stu-id="c474a-121">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="c474a-122">Felhasználói szerepkörök hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="c474a-122">Assign user roles</span></span>

<span data-ttu-id="c474a-123">Ahhoz, hogy a Partnerközpont dolgoznia kell, egy hozzárendelt szerepkört kell hozzárendelnie.</span><span class="sxs-lookup"><span data-stu-id="c474a-123">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="c474a-124">A szerepkörök jelenleg Azure Active Directory bérlői, Felhőszolgáltató (CSP) és a nem AAD-hez használt vállalati szerepköröket foglalnak magukban.</span><span class="sxs-lookup"><span data-stu-id="c474a-124">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="c474a-125">Egy adott vállalatnak szüksége lehet az összes szerepkörre.</span><span class="sxs-lookup"><span data-stu-id="c474a-125">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="c474a-126">Az egyéni felhasználók csak akkor férhetnek hozzá a bérlőhöz, ha Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="c474a-126">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="c474a-127">A szerepkör-hozzárendelések további hozzáférést biztosítanak.</span><span class="sxs-lookup"><span data-stu-id="c474a-127">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c474a-128">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c474a-128">Next steps</span></span>

- [<span data-ttu-id="c474a-129">Felhasználói szerepkörök és engedélyek hozzárendelése olyan alkalmazottakhoz, akik a munkahelyi Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="c474a-129">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
