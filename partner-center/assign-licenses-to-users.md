---
title: Felhasználók kezelése az ügyfelek fiókjaihoz
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Felhasználók kezelése a partner Centerben – felhasználói fiókok létrehozása, felhasználói licencek hozzáadása vagy eltávolítása, jelszavak alaphelyzetbe állítása, valamint a felhasználói fiókok törlése vagy visszaállítása.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756085"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="dde22-103">Felhasználói fiókok és felhasználói licencek kezelése az ügyfelek fiókjaihoz</span><span class="sxs-lookup"><span data-stu-id="dde22-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="dde22-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="dde22-104">**Appropriate roles**</span></span>

- <span data-ttu-id="dde22-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="dde22-105">Global admin</span></span>
- <span data-ttu-id="dde22-106">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="dde22-106">User management admin</span></span>
- <span data-ttu-id="dde22-107">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="dde22-107">Admin agent</span></span>


<span data-ttu-id="dde22-108">Az ügyfél fiókjában új felhasználókat hozhat létre és törölhet.</span><span class="sxs-lookup"><span data-stu-id="dde22-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="dde22-109">A törléstől számított 30 napon belül egy vagy több olyan felhasználói fiókot is visszaállíthat, amelyet korábban törölt.</span><span class="sxs-lookup"><span data-stu-id="dde22-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="dde22-110">A felhasználó korábbi előfizetési hozzárendelései is vissza lesznek állítva (feltéve, hogy az előző foglalások elérhetők).</span><span class="sxs-lookup"><span data-stu-id="dde22-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="dde22-111">Amikor új előfizetést vásárol az ügyfél számára, az ügyfélnek meg kell adnia az összes olyan felhasználó listáját, akiknek szükségük van a fiókra, a felhasználói engedélyeire és az egyes felhasználók által igényelt szolgáltatásokra.</span><span class="sxs-lookup"><span data-stu-id="dde22-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="dde22-112">Az **ügyfél** lap **felhasználók és licencek** szakasza megjeleníti az adott ügyfél bérlője által létrehozott összes felhasználót, beleértve a más CSP-partnertől vagy egy másik beszerzési csatornától vásárolt licenccel rendelkező felhasználókat is.</span><span class="sxs-lookup"><span data-stu-id="dde22-112">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="dde22-113">Egyszerre [több felhasználóhoz is hozzárendelhet előfizetéseket](bulk-license-provisioning-for-multiple-users.md) úgy, hogy a neveket egy [Excel-kompatibilis. csv számolótábla-fájllal](adding-multiple-users-to-a-customer-account.md)importálja.</span><span class="sxs-lookup"><span data-stu-id="dde22-113">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="dde22-114">Felhasználói fiókok létrehozása egy ügyfélnél</span><span class="sxs-lookup"><span data-stu-id="dde22-114">Create user accounts for a customer</span></span>

1. <span data-ttu-id="dde22-115">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="dde22-115">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="dde22-116">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="dde22-116">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="dde22-117">Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="dde22-117">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="dde22-118">Minden hozzáadott felhasználónál Válassza az **előfizetés hozzáadása** lehetőséget, majd adja meg az adatokat, beleértve az engedélyeket és a licenceket is.</span><span class="sxs-lookup"><span data-stu-id="dde22-118">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="dde22-119">**Mentse** a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="dde22-119">**Save** your changes.</span></span>

5. <span data-ttu-id="dde22-120">Ügyeljen arra, hogy a felhasználó számára küldendő felhasználónevet és ideiglenes jelszót jegyezze fel.</span><span class="sxs-lookup"><span data-stu-id="dde22-120">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="dde22-121">Ha egyszerre több felhasználót ad hozzá, akkor használjon **másik felhasználót**.</span><span class="sxs-lookup"><span data-stu-id="dde22-121">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="dde22-122">Egyszerre több felhasználót is hozzáadhat [egy Excel-kompatibilis. CSV formátumú számolótábla-fájl importálásával](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="dde22-122">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="dde22-123">Megvárhatja, amíg elkészült a teljes készlettel, mielőtt e-mailben vagy kinyomtatja a neveket és a jelszavakat a megerősítő képernyőn.</span><span class="sxs-lookup"><span data-stu-id="dde22-123">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="dde22-124">Felhasználói licencek hozzáadása vagy eltávolítása az ügyfélhez</span><span class="sxs-lookup"><span data-stu-id="dde22-124">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="dde22-125">A következő lépések a Microsoft-termékekhez tartozó felhasználói licencek hozzáadására vagy eltávolítására vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="dde22-125">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="dde22-126">A licenc alapú SaaS-előfizetésekhez tartozó felhasználói licencek hozzáadásához vagy eltávolításához a kereskedelmi piactéren tekintse meg a [SaaS-előfizetés licencek hozzáadása vagy eltávolítása](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)című témakört.</span><span class="sxs-lookup"><span data-stu-id="dde22-126">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="dde22-127">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="dde22-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="dde22-128">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="dde22-128">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="dde22-129">Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="dde22-129">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="dde22-130">Válasszon ki egy vagy több felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="dde22-130">Choose one or more users from the list.</span></span> <span data-ttu-id="dde22-131">Ha például az ügyfél csak új licenceket vásárolt, és azokat a felhasználók számára szeretné hozzárendelni, akik még nem rendelkeznek velük, akkor a megfelelő csoport megkereséséhez használhatja a **felhasználók szűrése...** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="dde22-131">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="dde22-132">Válassza a **licencek kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="dde22-132">Select **Manage licenses**.</span></span> <span data-ttu-id="dde22-133">Végezze el a módosításokat, majd **mentse**.</span><span class="sxs-lookup"><span data-stu-id="dde22-133">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="dde22-134">Az [Azure Marketplace-termékek](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)esetében a licenc-hozzárendelést és az aktiválást a terméket közzétevő független SZOFTVERGYÁRTÓ (ISV) kezeli.</span><span class="sxs-lookup"><span data-stu-id="dde22-134">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="dde22-135">Felhasználó jelszavának alaphelyzetbe állítása az ügyfél számára</span><span class="sxs-lookup"><span data-stu-id="dde22-135">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="dde22-136">Jelentkezzen be a Partnerközpont [irányítópultjába](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="dde22-136">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="dde22-137">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="dde22-137">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="dde22-138">Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="dde22-138">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="dde22-139">Válassza ki a felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="dde22-139">Choose the user from the list.</span></span>

4. <span data-ttu-id="dde22-140">A képernyő alján válassza a **jelszó alaphelyzetbe állítása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="dde22-140">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="dde22-141">Küldje el az új ideiglenes jelszót a felhasználónak.</span><span class="sxs-lookup"><span data-stu-id="dde22-141">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="dde22-142">Ügyfelek felhasználói fiókjainak törlése</span><span class="sxs-lookup"><span data-stu-id="dde22-142">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="dde22-143">A **partner Center** menüben válassza az **ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="dde22-143">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="dde22-144">Válassza ki az ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="dde22-144">Choose the customer from the list.</span></span>

2. <span data-ttu-id="dde22-145">Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="dde22-145">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="dde22-146">Válassza ki a felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="dde22-146">Choose the user from the list.</span></span>

3. <span data-ttu-id="dde22-147">A képernyő alján válassza a **felhasználói fiók törlése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="dde22-147">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="dde22-148">Ha vissza kell állítania ezt a fiókot, az ügyfél **felhasználói és licencek** listája **törölt felhasználók** lapján található.</span><span class="sxs-lookup"><span data-stu-id="dde22-148">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="dde22-149">A törölt felhasználó visszaállításának 30 napja van.</span><span class="sxs-lookup"><span data-stu-id="dde22-149">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="dde22-150">Törölt felhasználói fiókok visszaállítása</span><span class="sxs-lookup"><span data-stu-id="dde22-150">Restore deleted user accounts</span></span>

1. <span data-ttu-id="dde22-151">A **partner Center** menüben válassza az **ügyfelek** lehetőséget, majd válassza ki az ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="dde22-151">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="dde22-152">Válassza **a felhasználók és licencek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="dde22-152">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="dde22-153">Válassza a **törölt felhasználók ()** lapot. Ha törölt felhasználók is visszaállíthatók, olvassa el **(1)** vagy annál nagyobb.</span><span class="sxs-lookup"><span data-stu-id="dde22-153">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="dde22-154">Válasszon ki egy vagy több törölt felhasználó jelölőnégyzetet, majd válassza a **visszaállítás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="dde22-154">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="dde22-155">Az összes kiválasztott felhasználói fiók újra megjelenik a **felhasználók és licencek** lapon.</span><span class="sxs-lookup"><span data-stu-id="dde22-155">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="dde22-156">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="dde22-156">Next steps</span></span>

- [<span data-ttu-id="dde22-157">Licencek hozzárendelése vagy visszavonása több felhasználó esetében</span><span class="sxs-lookup"><span data-stu-id="dde22-157">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="dde22-158">Több felhasználó létrehozása egy ügyfél-fiókhoz</span><span class="sxs-lookup"><span data-stu-id="dde22-158">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)