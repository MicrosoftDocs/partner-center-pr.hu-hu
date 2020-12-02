---
title: Felhasználói fiókok és felhasználói licencek kezelése az ügyfelek fiókjaihoz
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan kezelheti az ügyfelek felhasználói számára a partner Centerben, például felhasználói fiókok létrehozását, felhasználói licencek hozzáadását vagy eltávolítását, felhasználói jelszavak visszaállítását, valamint felhasználói fiókok törlését vagy visszaállítását.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fb7906b006540ef939e443a21855488e9d2c36f9
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474070"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="3b2f3-103">Felhasználói fiókok és felhasználói licencek kezelése az ügyfelek fiókjaihoz</span><span class="sxs-lookup"><span data-stu-id="3b2f3-103">Manage users and user licenses for customer accounts</span></span>

<span data-ttu-id="3b2f3-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="3b2f3-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3b2f3-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="3b2f3-105">Global admin</span></span>
- <span data-ttu-id="3b2f3-106">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="3b2f3-106">User management admin</span></span>
- <span data-ttu-id="3b2f3-107">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="3b2f3-107">Admin agent</span></span>


<span data-ttu-id="3b2f3-108">Az ügyfél fiókjában új felhasználókat hozhat létre és törölhet.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="3b2f3-109">A törléstől számított 30 napon belül egy vagy több olyan felhasználói fiókot is visszaállíthat, amelyet korábban törölt.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="3b2f3-110">A felhasználó korábbi előfizetési hozzárendelései is vissza lesznek állítva (feltéve, hogy az előző foglalások elérhetők).</span><span class="sxs-lookup"><span data-stu-id="3b2f3-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="3b2f3-111">Amikor új előfizetést vásárol az ügyfél számára, az ügyfélnek meg kell adnia az összes olyan felhasználó listáját, akiknek szükségük van a fiókra, a felhasználói engedélyeire és az egyes felhasználók által igényelt szolgáltatásokra.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="3b2f3-112">Egyszerre [több felhasználóhoz is hozzárendelhet előfizetéseket](bulk-license-provisioning-for-multiple-users.md) úgy, hogy a neveket egy [Excel-kompatibilis. csv számolótábla-fájllal](adding-multiple-users-to-a-customer-account.md)importálja.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-112">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="3b2f3-113">Felhasználói fiókok létrehozása az ügyfelek számára</span><span class="sxs-lookup"><span data-stu-id="3b2f3-113">Create user accounts for a customer</span></span>

1. <span data-ttu-id="3b2f3-114">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="3b2f3-114">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3b2f3-115">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3b2f3-116">Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-116">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="3b2f3-117">Minden hozzáadott felhasználónál Válassza az **előfizetés hozzáadása** lehetőséget, majd adja meg az adatokat, beleértve az engedélyeket és a licenceket is.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-117">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="3b2f3-118">**Mentse** a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-118">**Save** your changes.</span></span>

5. <span data-ttu-id="3b2f3-119">Ügyeljen arra, hogy a felhasználó számára küldendő felhasználónevet és ideiglenes jelszót jegyezze fel.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-119">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="3b2f3-120">Ha egyszerre több felhasználót ad hozzá, akkor használjon **másik felhasználót**.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-120">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="3b2f3-121">Egyszerre több felhasználót is hozzáadhat [egy Excel-kompatibilis. CSV formátumú számolótábla-fájl importálásával](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="3b2f3-121">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="3b2f3-122">Megvárhatja, amíg elkészült a teljes készlettel, mielőtt e-mailben vagy kinyomtatja a neveket és a jelszavakat a megerősítő képernyőn.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-122">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="3b2f3-123">Felhasználói licencek hozzáadása vagy eltávolítása az ügyfélhez</span><span class="sxs-lookup"><span data-stu-id="3b2f3-123">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="3b2f3-124">A következő lépések a Microsoft-termékekhez tartozó felhasználói licencek hozzáadására vagy eltávolítására vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-124">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="3b2f3-125">A licenc alapú SaaS-előfizetésekhez tartozó felhasználói licencek hozzáadásához vagy eltávolításához a kereskedelmi piactéren tekintse meg a [SaaS-előfizetés licencek hozzáadása vagy eltávolítása](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)című témakört.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-125">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="3b2f3-126">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="3b2f3-126">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3b2f3-127">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-127">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3b2f3-128">Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-128">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="3b2f3-129">Válasszon ki egy vagy több felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-129">Choose one or more users from the list.</span></span> <span data-ttu-id="3b2f3-130">Ha például az ügyfél csak új licenceket vásárolt, és azokat a felhasználók számára szeretné hozzárendelni, akik még nem rendelkeznek velük, akkor a megfelelő csoport megkereséséhez használhatja a **felhasználók szűrése...** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-130">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="3b2f3-131">Válassza a **licencek kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-131">Select **Manage licenses**.</span></span> <span data-ttu-id="3b2f3-132">Végezze el a módosításokat, majd **mentse**.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-132">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="3b2f3-133">Az [Azure Marketplace-termékek](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)esetében a licenc-hozzárendelést és az aktiválást a terméket közzétevő független SZOFTVERGYÁRTÓ (ISV) kezeli.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-133">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="3b2f3-134">Felhasználó jelszavának alaphelyzetbe állítása az ügyfél számára</span><span class="sxs-lookup"><span data-stu-id="3b2f3-134">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="3b2f3-135">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="3b2f3-135">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3b2f3-136">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-136">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="3b2f3-137">Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-137">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="3b2f3-138">Válassza ki a felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-138">Choose the user from the list.</span></span>

4.  <span data-ttu-id="3b2f3-139">A képernyő alján válassza a **jelszó alaphelyzetbe állítása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-139">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="3b2f3-140">Küldje el az új ideiglenes jelszót a felhasználónak.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-140">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="3b2f3-141">Ügyfelek felhasználói fiókjainak törlése</span><span class="sxs-lookup"><span data-stu-id="3b2f3-141">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="3b2f3-142">A **partner Center** menüben válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-142">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="3b2f3-143">Válassza ki az ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-143">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="3b2f3-144">Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-144">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="3b2f3-145">Válassza ki a felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-145">Choose the user from the list.</span></span>

3.  <span data-ttu-id="3b2f3-146">A képernyő alján válassza a **felhasználói fiók törlése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-146">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="3b2f3-147">Ha vissza kell állítania ezt a fiókot, az ügyfél **felhasználói és licencek** listája **törölt felhasználók** lapján található.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-147">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="3b2f3-148">A törölt felhasználó visszaállításának 30 napja van.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-148">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="3b2f3-149">Törölt felhasználói fiókok visszaállítása</span><span class="sxs-lookup"><span data-stu-id="3b2f3-149">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="3b2f3-150">A **partner Center** menüben válassza az **ügyfelek** lehetőséget, majd válassza ki az ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-150">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="3b2f3-151">Válassza **a felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-151">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="3b2f3-152">Válassza a **törölt felhasználók ()** lapot. Ha törölt felhasználók is visszaállíthatók, olvassa el **(1)** vagy annál nagyobb.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-152">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="3b2f3-153">Válasszon ki egy vagy több törölt felhasználó jelölőnégyzetet, majd válassza a **visszaállítás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-153">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="3b2f3-154">Az összes kiválasztott felhasználói fiók újra megjelenik a **felhasználók és licencek** lapon.</span><span class="sxs-lookup"><span data-stu-id="3b2f3-154">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="3b2f3-155">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="3b2f3-155">Related topics</span></span>


[<span data-ttu-id="3b2f3-156">Licencek hozzárendelése vagy visszavonása több felhasználó esetében</span><span class="sxs-lookup"><span data-stu-id="3b2f3-156">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="3b2f3-157">Több felhasználó létrehozása egy ügyfél-fiókhoz</span><span class="sxs-lookup"><span data-stu-id="3b2f3-157">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)