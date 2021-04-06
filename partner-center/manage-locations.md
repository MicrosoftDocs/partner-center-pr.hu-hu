---
title: Telephelyek kezelése a partneri fiókban
ms.topic: how-to
ms.date: 04/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Ismerje meg, hogyan vehet fel új helyet, és hogyan használják a Location MPN ID-t az ösztönző programok, a CSP-üzleti, az előfizetések és az egyéb tranzakciók során.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ca8c866479fbe153c1e0192edd33e8258b9d6e7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441327"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="fb4e6-103">Az MPN-fiók helyeinek kezelése és hely hozzáadása (törlése)</span><span class="sxs-lookup"><span data-stu-id="fb4e6-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="fb4e6-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="fb4e6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fb4e6-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="fb4e6-105">Global admin</span></span>
- <span data-ttu-id="fb4e6-106">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="fb4e6-106">Account admin</span></span>

<span data-ttu-id="fb4e6-107">A hely MPN-azonosítója azonosítja a vállalat minden egyes helyét.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="fb4e6-108">Az MPN-azonosítót a következő helyen regisztrálhatja az ösztönző programokban: a Cloud Solution Provider (CSP) üzletág és más üzleti tranzakciók.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="fb4e6-109">A globális MPN-azonosító a nem tranzakciós tevékenységek, például a támogatási kérelmek esetében használatos.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="fb4e6-110">A következő forgatókönyv tipikus:</span><span class="sxs-lookup"><span data-stu-id="fb4e6-110">The following scenario is typical:</span></span>

<span data-ttu-id="fb4e6-111">A contoso az Egyesült királyságbeli partneri globális fiókkal (PGA) rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="fb4e6-112">A PGA a regisztrált jogi üzleti tevékenység, a globális MPN-azonosító pedig az összes nem tranzakciós üzlet kezelésére szolgál.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="fb4e6-113">A contoso az Egyesült Királyság, Franciaország és az Egyesült Államok területén is rendelkezik leányvállalatokkal vagy részlegekkel egyenértékű partneri hellyel (PLA).</span><span class="sxs-lookup"><span data-stu-id="fb4e6-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="fb4e6-114">Az MPN-fiók struktúrájában ezek a PLAsok egyedi Location MPN-azonosítóként jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="fb4e6-115">A PLAs a tranzakciós vállalkozások, például a CSP-vagy ösztönző programok esetében használatos.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="fb4e6-116">A kifizetések adott helyszínekhez vannak kötve.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="fb4e6-117">1-1 kapcsolat van a CSP-bérlő és az MPN-hely azonosítója között.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN-helyszínek szerkezete":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="fb4e6-119">Előfeltételek új fiók hozzáadásához a CSP vállalat számára</span><span class="sxs-lookup"><span data-stu-id="fb4e6-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="fb4e6-120">Új CSP üzleti fiók hozzáadásához először győződjön meg arról, hogy teljesítette az előfeltételeket.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="fb4e6-121">Rendelkeznie kell egy Location MPN-AZONOSÍTÓval abban az országban, ahol a CSP vállalatot szeretné elvégezni.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="fb4e6-122">Új MPN-hely létrehozásához olvassa el az alábbi "MPN-hely hozzáadása" című szakaszt.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="fb4e6-123">Új CSP közvetett viszonteladói regisztrációjának létrehozásához olvassa el a [közvetett szolgáltatók használata](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="fb4e6-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="fb4e6-124">Ne felejtse el bejelentkezni az **új** CSP-fiók **új** hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="fb4e6-125">Ne használja a meglévő hitelesítő adatait, mert a partneri központ már rendelkezik fiókkal.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="fb4e6-126">Fogadja el a Microsoft partneri szerződést, és aktiválja a fiókot.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="fb4e6-127">Ha közvetlen számlás partnerként szeretne regisztrálni, olvassa el [a közvetlen számlázási partnereinkre vonatkozó követelményeket](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="fb4e6-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="fb4e6-128">MPN-hely megtekintése</span><span class="sxs-lookup"><span data-stu-id="fb4e6-128">View your MPN locations</span></span>

1. <span data-ttu-id="fb4e6-129">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/home) az MPN-fiókja hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="fb4e6-130">(Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól)</span><span class="sxs-lookup"><span data-stu-id="fb4e6-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="fb4e6-131">A **Beállítások** ikonban válassza a **Fiókbeállítások**, **szervezeti profil**, **jogi** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="fb4e6-132">A **partner** lapon ellenőrizze, hogy nincs-e szalagcím-hibaüzenet, amely arra kéri, hogy javítsa az áttelepített helyet a PMC-ból.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="fb4e6-133">Ha a helyük nincsenek helyesen beállítva a PMC-ben, és még nem váltották át a SZÁMÍTÓGÉPekre, frissítenie kell ezeket a helyeket.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="A screencap bemutatja, hogyan lehet frissíteni a helyet.":::
 
4.  <span data-ttu-id="fb4e6-135">A **PMC-helyszínek áttekintése** képernyőn válassza a **frissítés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="fb4e6-136">Frissítse a következő mezőket:</span><span class="sxs-lookup"><span data-stu-id="fb4e6-136">Update the following fields:</span></span>

- <span data-ttu-id="fb4e6-137">**Név mező**: Ellenőrizze, hogy helyes-e a vállalati hely neve.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="fb4e6-138">Ha ismétlődő hiba jelenik meg, próbálkozzon a következővel:, például contoso – contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="fb4e6-139">**Jogi személy mező**: Győződjön meg arról, hogy a helyhez kötött jogi személyt választotta</span><span class="sxs-lookup"><span data-stu-id="fb4e6-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="fb4e6-140">**1. címtartomány & 2 mező**: Ellenőrizze, hogy helyes-e a címe.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="fb4e6-141">**Város & állam/megye mezők**: Ellenőrizze, hogy helyes-e a város és az állam/tartomány közötti kombináció.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="fb4e6-142">Vannak olyan országok, amelyekben az állam/megye kiválasztására szolgáló legördülő menü lesz érvényes, és más országokban is be kell szúrni a mezőt.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="fb4e6-143">**Irányítószám mező**: Győződjön meg arról, hogy az irányítószám mező megfelel a jelzett országnak, régiónak, városnak vagy címnek.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="fb4e6-144">**Elsődleges kapcsolattartási adatok mezői**: Győződjön meg arról, hogy az utónév és a vezetéknév mező ki van töltve, és hogy a megadott e-mail cím egy munkahelyi e-mail cím, és nem személyes (például @outlook.com @live.com stb.).</span><span class="sxs-lookup"><span data-stu-id="fb4e6-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="fb4e6-145">**Telefonszám mező**: Ügyeljen arra, hogy a telefonszám ne tartalmazzon speciális karaktereket, szóközöket vagy országkódot.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="fb4e6-146">A telefonszám mezőben megadott érték mindig legfeljebb 10 karaktert tartalmazhat.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="fb4e6-147">Ha nem jelenik meg hibaüzenet, a  **Beállítások** területen válassza a  **Fiókbeállítások**, **szervezeti profil**, **azonosítók** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="fb4e6-148">Keresse meg a "location" típusú MPN-azonosítót, amely megfelel a CSP-fiók országának, és használja a társítás befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="fb4e6-149">Ha nem találja a használni kívánt CSP-fióknak megfelelő Location MPN-azonosítót, új helyet adhat hozzá, amely létrehoz egy új MPN-azonosítót.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="fb4e6-150">Lásd: **MPN-hely hozzáadása** alább.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="fb4e6-151">MPN-hely hozzáadása</span><span class="sxs-lookup"><span data-stu-id="fb4e6-151">Add an MPN location</span></span>

1. <span data-ttu-id="fb4e6-152">Jelentkezzen be az MPN-fiókkal a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="fb4e6-153">(Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól).</span><span class="sxs-lookup"><span data-stu-id="fb4e6-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="fb4e6-154">Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="fb4e6-155">A **Beállítások ikonban** válassza ki a **Fiókbeállítások** elemet, majd válassza a **szervezeti profil** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="fb4e6-156">Válassza a **jogi** lehetőséget, majd a **partner** lapon válassza az **üzleti helyek lehetőséget,** majd kattintson a **hely hozzáadása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="fb4e6-157">Adja meg a szükséges adatokat, beleértve az üzleti nevet, a lakcímet és a kapcsolattartót a vállalatához hozzáadni kívánt helyhez.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="fb4e6-158">Kattintson a **hely hozzáadása** gombra.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-158">Click **Add location**.</span></span> <span data-ttu-id="fb4e6-159">Ekkor létrejön egy új MPN-azonosító az új helyhez, amelyet a CSP-tranzakciókhoz és-ösztönzőkhöz használhat.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Új jogi üzleti tevékenység hozzáadása":::

> [!NOTE]
> <span data-ttu-id="fb4e6-161">Miután hozzáadta a helyet a partner Centerben, nem távolíthatja el.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="fb4e6-162">Ha a megfelelő MPN-azonosítót használta a bejelentkezéshez, az **MPN** a partner Center bal oldali menüjében jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>


## <a name="delete-a-location"></a><span data-ttu-id="fb4e6-163">Hely törlése</span><span class="sxs-lookup"><span data-stu-id="fb4e6-163">Delete a location</span></span>

<span data-ttu-id="fb4e6-164">Ha törölni szeretne egy helyet a fiókjából, kapcsolatba kell lépnie a [partner támogatási szolgálatával](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="fb4e6-164">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="fb4e6-165">Győződjön meg arról, hogy tisztában van a művelet hatásával.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-165">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="fb4e6-166">A törölt helyeket nem lehet beolvasni, és az adott MPN-azonosítóhoz kapcsolódó minden adat már nem ismerhető fel, vagy nem lesz aktív a vállalatnál.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-166">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="fb4e6-167">Partner globális fiók országának módosítása</span><span class="sxs-lookup"><span data-stu-id="fb4e6-167">Change country of Partner global account</span></span> 

1. <span data-ttu-id="fb4e6-168">Jelentkezzen be az MPN-fiókkal a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-168">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="fb4e6-169">(Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól).</span><span class="sxs-lookup"><span data-stu-id="fb4e6-169">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="fb4e6-170">Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-170">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="fb4e6-171">A **partner** lapon lépjen az **üzleti helyek** elemre, és ellenőrizze a helyek listáját, és győződjön meg arról, hogy az Ön által használt hely szerepel a jogi személy listáján.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-171">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="fb4e6-172">Hely hozzáadásához kattintson a **hely hozzáadása** lehetőségre, és a kilépéskor adja meg a szükséges adatokat, beleértve az üzleti nevét, a lakcímét és az elsődleges kapcsolattartót a vállalatához hozzáadni kívánt helyhez.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-172">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="fb4e6-173">Válassza az ország **/régió** legördülő lista melletti **ország módosítása** lehetőséget, és kövesse a lépéseket.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-173">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Jogi üzleti profilra vonatkozó adatvesztés":::

5. <span data-ttu-id="fb4e6-175">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-175">Click **Save**.</span></span>

6. <span data-ttu-id="fb4e6-176">Az MPN globális fiók országa az új jogi országra lesz módosítva.</span><span class="sxs-lookup"><span data-stu-id="fb4e6-176">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="fb4e6-177">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="fb4e6-177">Next steps</span></span>

- <span data-ttu-id="fb4e6-178">További információ az [ellenőrzési folyamatról](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="fb4e6-178">Learn about the [verification process](verification-responses.md).</span></span>
