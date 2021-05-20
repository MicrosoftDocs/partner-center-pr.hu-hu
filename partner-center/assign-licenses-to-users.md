---
title: Ügyfélfiókok felhasználóinak kezelése
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Az ügyfelek felhasználóinak kezelése a Partnerközpont – felhasználói fiókokat hozhat létre, felhasználói licenceket adhat hozzá vagy távolíthat el, új jelszavakat állíthat vissza, valamint törölheti vagy visszaállíthatja a felhasználói fiókokat.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149893"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="4a639-103">Az ügyfélfiókok felhasználói és felhasználói licenceinek kezelése</span><span class="sxs-lookup"><span data-stu-id="4a639-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="4a639-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Rendszergazdai ügynök</span><span class="sxs-lookup"><span data-stu-id="4a639-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="4a639-105">Új felhasználókat hozhat létre és törölhet az ügyfél fiókjában.</span><span class="sxs-lookup"><span data-stu-id="4a639-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="4a639-106">Egy vagy több olyan felhasználói fiókot is visszaállíthat, amelyet a törlést követő 30 napon belül törölt.</span><span class="sxs-lookup"><span data-stu-id="4a639-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="4a639-107">A felhasználó korábbi előfizetés-hozzárendelései szintén visszaállnak (feltéve, hogy a korábbi foglalások elérhetők).</span><span class="sxs-lookup"><span data-stu-id="4a639-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="4a639-108">Amikor új előfizetéseket vásárol egy ügyfélnek, az ügyfélnek meg kell adni egy listát az összes felhasználóról, akiknek fiókra van szüksége, a felhasználói engedélyeiket, valamint az egyes felhasználóknak szükséges szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="4a639-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="4a639-109">Az **Ügyfél lap** Felhasználók  és licencek szakasza az adott ügyfél bérlője által létrehozott összes felhasználót megjeleníti, beleértve azokat a felhasználókat is, akik más CSP-partnertől vagy más vásárlási csatornáról vásárolt licenccel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="4a639-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="4a639-110">Az [előfizetéseket egyszerre](bulk-license-provisioning-for-multiple-users.md) több felhasználóhoz is hozzárendelheti, ha a neveket [egy Excel-kompatibilis .csv-táblázatfájllal importálja.](adding-multiple-users-to-a-customer-account.md)</span><span class="sxs-lookup"><span data-stu-id="4a639-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="4a639-111">Felhasználói fiókok létrehozása egy ügyfélnél</span><span class="sxs-lookup"><span data-stu-id="4a639-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="4a639-112">Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="4a639-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="4a639-113">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="4a639-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="4a639-114">Az ügyfélmenüben válassza a **Felhasználók és licencek lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4a639-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="4a639-115">Minden egyes felhasználónál válassza az **Előfizetés** hozzáadása lehetőséget, majd töltse ki az adatokat, beleértve az engedélyeket és a licenceket.</span><span class="sxs-lookup"><span data-stu-id="4a639-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="4a639-116">**Mentse a** módosításokat.</span><span class="sxs-lookup"><span data-stu-id="4a639-116">**Save** your changes.</span></span>

5. <span data-ttu-id="4a639-117">Mindenképpen jegyezd fel a felhasználónak küldend el küldened a felhasználónevet és az ideiglenes jelszót.</span><span class="sxs-lookup"><span data-stu-id="4a639-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="4a639-118">Ha egyszerre több felhasználót ad hozzá, használja a **Másik felhasználó hozzáadása gombra.**</span><span class="sxs-lookup"><span data-stu-id="4a639-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="4a639-119">Egy Excel-kompatibilis .csv-számolótáblafájl importálása lehetővé teszi, hogy egyszerre több felhasználót [is hozzáadjon.](adding-multiple-users-to-a-customer-account.md)</span><span class="sxs-lookup"><span data-stu-id="4a639-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="4a639-120">Megvárhatja, amíg a teljes készlettel végzett, mielőtt e-mailt küld, vagy kinyomtatja a neveket és jelszavakat a megerősítési képernyőn.</span><span class="sxs-lookup"><span data-stu-id="4a639-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="4a639-121">Felhasználói licenc hozzáadása vagy eltávolítása egy ügyfélnél</span><span class="sxs-lookup"><span data-stu-id="4a639-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="4a639-122">Az alábbi lépések a Microsoft-termékek felhasználói licenceinek hozzáadására vagy eltávolítására vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="4a639-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="4a639-123">A licencalapú SaaS-előfizetések felhasználói licenceinek kereskedelmi piactéren való hozzáadásához vagy eltávolításához lásd: Licencek hozzáadása vagy [eltávolítása SaaS-előfizetéshez.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)</span><span class="sxs-lookup"><span data-stu-id="4a639-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="4a639-124">Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="4a639-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="4a639-125">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="4a639-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="4a639-126">Az ügyfélmenüben válassza a **Felhasználók és licencek lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4a639-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="4a639-127">Válasszon ki a listából egy vagy több felhasználót.</span><span class="sxs-lookup"><span data-stu-id="4a639-127">Choose one or more users from the list.</span></span> <span data-ttu-id="4a639-128">Ha például az ügyfél most vásárolt új licenceket, és olyan személyekhez kívánt hozzárendelni őket, akik még nem rendelkezik velük, a Felhasználók **szűrése...** lehetőséggel megkeresheti a megfelelő csoportot.</span><span class="sxs-lookup"><span data-stu-id="4a639-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="4a639-129">Válassza ki a **Licencek kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4a639-129">Select **Manage licenses**.</span></span> <span data-ttu-id="4a639-130">Módosításokat kell tenni, majd a **Mentés gombra.**</span><span class="sxs-lookup"><span data-stu-id="4a639-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="4a639-131">A [Azure Marketplace termékek](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)esetében a licenc-hozzárendelést és az aktiválást a terméket közzétevő független szoftverszállító (ISV) kezeli.</span><span class="sxs-lookup"><span data-stu-id="4a639-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="4a639-132">Felhasználó jelszavának visszaállítása egy ügyfélhez</span><span class="sxs-lookup"><span data-stu-id="4a639-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="4a639-133">Jelentkezzen be a Partnerközpont [irányítópultjába](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="4a639-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="4a639-134">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="4a639-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="4a639-135">Az ügyfélmenüben válassza a **Felhasználók és licencek lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4a639-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="4a639-136">Válassza ki a felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="4a639-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="4a639-137">A képernyő alján válassza a Jelszó **alaphelyzetbe állítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4a639-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="4a639-138">Küldje el az új ideiglenes jelszót a felhasználónak.</span><span class="sxs-lookup"><span data-stu-id="4a639-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="4a639-139">Ügyfél felhasználói fiókjainak törlése</span><span class="sxs-lookup"><span data-stu-id="4a639-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="4a639-140">A **Partnerközpont** válassza az Ügyfelek **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4a639-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="4a639-141">Válassza ki az ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="4a639-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="4a639-142">Az ügyfélmenüben válassza a **Felhasználók és licencek lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4a639-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="4a639-143">Válassza ki a felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="4a639-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="4a639-144">A képernyő alján válassza a **Felhasználói fiók törlése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4a639-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="4a639-145">Ha vissza kell állítania ezt a fiókot, az Ügyfél felhasználók és licencek listájának Törölt felhasználók lapján **találhatja** meg. </span><span class="sxs-lookup"><span data-stu-id="4a639-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="4a639-146">30 napja van a törölt felhasználók visszaállítására.</span><span class="sxs-lookup"><span data-stu-id="4a639-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="4a639-147">Törölt felhasználói fiókok visszaállítása</span><span class="sxs-lookup"><span data-stu-id="4a639-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="4a639-148">A **Partnerközpont** válassza az **Ügyfelek** lehetőséget, majd válassza ki az ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="4a639-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="4a639-149">Válassza **a Felhasználók és licencek lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4a639-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="4a639-150">Válassza a **Törölt felhasználók ( )** lapot. Ha vannak visszaállítható törölt felhasználók, akkor a következőt kell olvasnia: **(1)** vagy nagyobb.</span><span class="sxs-lookup"><span data-stu-id="4a639-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="4a639-151">Jelölje be a törölt felhasználók egy vagy több jelölőnégyzetét, majd válassza a Visszaállítás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4a639-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="4a639-152">Az összes kiválasztott felhasználói fiók megjelenik a Felhasználók és **licencek lapon.**</span><span class="sxs-lookup"><span data-stu-id="4a639-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4a639-153">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="4a639-153">Next steps</span></span>

- [<span data-ttu-id="4a639-154">Licencek hozzárendelése vagy visszavonása több felhasználó esetében</span><span class="sxs-lookup"><span data-stu-id="4a639-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="4a639-155">Több felhasználó létrehozása egy ügyfélfiókhoz</span><span class="sxs-lookup"><span data-stu-id="4a639-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)