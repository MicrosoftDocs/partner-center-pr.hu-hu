---
title: Helyek kezelése a partnerfiókban
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Megtudhatja, hogyan adhat hozzá új helyet, és hogyan használja fel a hely MPN-azonosítóját az ösztönzőprogramokban, a CSP-üzletben, az előfizetésben és más tranzakciókban.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 13d6e7dc4722227035be2b24df48427f2008bb14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151780"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="ed4e8-103">Az MPN-fiók helyének kezelése és hely hozzáadása (törlése)</span><span class="sxs-lookup"><span data-stu-id="ed4e8-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="ed4e8-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Fiók rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="ed4e8-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="ed4e8-105">A hely MPN-azonosítója azonosítja a vállalat egyes helyeket.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-105">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="ed4e8-106">A hely MPN-azonosítójával regisztrálható az ösztönzőprogramokba, tranzakciókat Felhőszolgáltató (CSP) és egyéb üzleti tranzakciókat.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-106">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="ed4e8-107">A globális MPN-azonosítót nem tranzakciós tevékenységekhez, például támogatási kérelmekhez használjuk.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-107">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="ed4e8-108">A következő forgatókönyv jellemző:</span><span class="sxs-lookup"><span data-stu-id="ed4e8-108">The following scenario is typical:</span></span>

<span data-ttu-id="ed4e8-109">A Contoso globális partnerfiókkal (PGA) rendelkezik az Egyesült Királyságban.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-109">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="ed4e8-110">A PGA a regisztrált jogi vállalkozásuk, és annak globális MPN-azonosítóját az összes nem tranzakciós üzlet kezelésére használják.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-110">The PGA is their registered legal business, and its global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="ed4e8-111">A Contoso emellett partnerhelyi fiókokkal (PLA) is rendelkezik, amelyek egyenértékűek az Egyesült Királyság, Franciaország és az USA más helyén található leányvállalatokkal vagy részlegekkel.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-111">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="ed4e8-112">Az MPN-fiók struktúrájában ezek a PLA-k egyedi hely MPN-azonosítókként vannak ábrázolva.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-112">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="ed4e8-113">A PLA-k tranzakciós üzleti tevékenységhez, például CSP-khez vagy ösztönzőprogramokhoz használhatók.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-113">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="ed4e8-114">A kifizetések adott helyekhez vannak kötve.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-114">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="ed4e8-115">Egy CSP-bérlő és egy MPN-helyazonosító között 1–1 kapcsolat áll elő.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-115">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Az MPN-helyek struktúrája":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="ed4e8-117">Új fiók csp-vállalkozáshoz való hozzáadásának előfeltételei</span><span class="sxs-lookup"><span data-stu-id="ed4e8-117">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="ed4e8-118">Új VÁLLALATI CSP-fiók hozzáadásához először is meg kell bizonyosodni arról, hogy teljesülnek az előfeltételek.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-118">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="ed4e8-119">Egy hely MPN-azonosítóval kell lennie abban az országban, ahol CSP-vállalkozást szeretne.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-119">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="ed4e8-120">Új MPN-hely létrehozásához olvassa el alább az "MPN-hely hozzáadása" adatokat.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-120">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="ed4e8-121">Új regisztráció létrehozásához olvassa CSP Indirect Reseller [Közvetett szolgáltatókkal való munka részt.](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="ed4e8-121">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="ed4e8-122">Ne felejtsen el bejelentkezni az **új** CSP-fiók új hitelesítő adataival. </span><span class="sxs-lookup"><span data-stu-id="ed4e8-122">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="ed4e8-123">Ne használja a meglévő hitelesítő adatait, mert Partnerközpont a rendszer felismeri, hogy már rendelkezik fiókkal.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-123">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="ed4e8-124">Fogadja el Microsoft Partnerszerződés és aktiválja a fiókot.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-124">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="ed4e8-125">Ha közvetlen számlázási partnerként szeretne regisztrálni, olvassa el a Következőt: A közvetlen számlázási [partnerekre vonatkozó követelmények](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="ed4e8-125">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="ed4e8-126">MPN-helyek megtekintése és frissítése</span><span class="sxs-lookup"><span data-stu-id="ed4e8-126">View and update your MPN locations</span></span>

1. <span data-ttu-id="ed4e8-127">Jelentkezzen be az Partnerközpont [irányítópultra](https://partner.microsoft.com/dashboard/home) az MPN-fiókja hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="ed4e8-128">(Az MPN hitelesítő adatai különbözhetnek a CSP hitelesítő adataitól)</span><span class="sxs-lookup"><span data-stu-id="ed4e8-128">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="ed4e8-129">A Beállítások **ikonon** válassza a **Fiókbeállítások,** Szervezeti **profil,** **Jogi lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ed4e8-129">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="ed4e8-130">A **Partner lapon** ellenőrizze, hogy nincs-e szalagcím-hibaüzenet, amely arra kéri, hogy javítsa ki a PMC-ről migrált helyeket.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-130">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="ed4e8-131">Ha a helyek nem megfelelően voltak beállítva a PMC-n, és még nem voltak pc-re állítva, frissítenie kell ezeket a helyeket.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-131">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="A képernyőkép bemutatja, hogyan frissítheti a helyet.":::
 
4.  <span data-ttu-id="ed4e8-133">A **PMC-helyek áttekintése képernyőn** válassza a Frissítés **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ed4e8-133">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="ed4e8-134">Frissítse a következő mezőket:</span><span class="sxs-lookup"><span data-stu-id="ed4e8-134">Update the following fields:</span></span>

- <span data-ttu-id="ed4e8-135">**Név mező:** Győződjön meg arról, hogy a vállalat helyének neve helyes.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-135">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="ed4e8-136">Ha duplikált hiba jelenik meg, próbáljon meg például Contoso-ről Contoso, Inc-re vált.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-136">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="ed4e8-137">**Jogi személy mező:** Győződjön meg arról, hogy azt a jogi entitást választotta ki, amelyhez a hely kötődik</span><span class="sxs-lookup"><span data-stu-id="ed4e8-137">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="ed4e8-138">**Az 1. & 2 mező:** Ellenőrizze, hogy a cím helyes-e</span><span class="sxs-lookup"><span data-stu-id="ed4e8-138">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="ed4e8-139">**City & State/Province (Állam/Tartomány)** mezők: Győződjön meg arról, hogy a város és az állam/tartomány közötti kombináció helyes.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-139">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="ed4e8-140">Vannak országok, ahol az Állam/Tartomány kiválasztására vonatkozó legördülő menü érvényes, és más országokban a mezőt manuálisan kell beszúrni.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-140">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="ed4e8-141">**IRÁNYÍTÓSZÁM mező:** Győződjön meg arról, hogy az Irányítószám mező megfelel a megadott országnak, régiónak, városnak vagy címnek.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-141">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="ed4e8-142">**Elsődleges kapcsolattartási adatok mezői:** Győződjön meg arról, hogy az első és a vezetéknév mező ki van töltve, és hogy a megadott e-mail-cím munkahelyi e-mail-cím, nem pedig személyes cím (például @outlook.com , @live.com stb.)</span><span class="sxs-lookup"><span data-stu-id="ed4e8-142">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="ed4e8-143">**Telefonszám mező:** Győződjön meg arról, hogy a Telefonszám NEM tartalmaz speciális karaktereket, szóközöket vagy országkódot.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-143">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="ed4e8-144">A Telefonszám mezőben megadott érték mindig legfeljebb 10 karaktert tartalmazhat.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-144">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="ed4e8-145">Ha nem jelenik meg hibaüzenet, akkor a Beállítások lapon válassza a Fiókbeállítások, a Szervezeti **profil,** az **Azonosítók lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ed4e8-145">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="ed4e8-146">Keresse meg a "Hely" típusú MPN-azonosítót, amely megfelel a CSP-fiók országának, és használja a társítás befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-146">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="ed4e8-147">Ha nem találja a használni kívánt CSP-fióknak megfelelő hely MPN-azonosítót, hozzáadhat egy új helyet, amely létrehoz egy új MPN-azonosítót.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-147">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="ed4e8-148">Lásd **alább az MPN-hely hozzáadását.**</span><span class="sxs-lookup"><span data-stu-id="ed4e8-148">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="ed4e8-149">MPN-hely hozzáadása</span><span class="sxs-lookup"><span data-stu-id="ed4e8-149">Add an MPN location</span></span>

1. <span data-ttu-id="ed4e8-150">Jelentkezzen be az MPN-fiókkal a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="ed4e8-151">(Az MPN hitelesítő adatai különbözhetnek a CSP hitelesítő adataitól.) Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultsággal kell lennie.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-151">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="ed4e8-152">A Beállítások **ikonra kattintva** válassza a **Fiókbeállítások,** majd a Szervezeti **profil lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ed4e8-152">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="ed4e8-153">Válassza **a Jogi** lehetőséget, majd a Partner **lapon** válassza az Üzleti **helyek,** majd a Hely **hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ed4e8-153">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and select **Add a location.**</span></span>

3. <span data-ttu-id="ed4e8-154">Adja meg a szükséges adatokat, beleértve a vállalathoz hozzáadni kívánt hely nevét, címét és kapcsolattartóját.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-154">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="ed4e8-155">Válassza **a Hely hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ed4e8-155">Select **Add location**.</span></span> <span data-ttu-id="ed4e8-156">Ezzel létrehoz egy új MPN-azonosítót az új helyhez, amely a CSP-tranzakciókhoz és -ösztönzőkhez használható.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-156">This will create a new MPN ID for the new location that you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Új jogi vállalkozás hozzáadása":::

> [!NOTE]
> <span data-ttu-id="ed4e8-158">Miután hozzáadott egy helyet a Partnerközpont, nem távolíthatja el.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-158">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="ed4e8-159">Ha a megfelelő **MPN-azonosítót** használta a bejelentkezéshez Partnerközpont az MPN megjelenik a bal oldali menüben.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-159">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="ed4e8-160">A regisztrációs szám azonosítójának hozzáadása</span><span class="sxs-lookup"><span data-stu-id="ed4e8-160">Add the registration number ID</span></span>

<span data-ttu-id="ed4e8-161">Ha Ön közvetett szolgáltató, közvetlen számlázási partner vagy közvetett viszonteladó, és a következő országokban új vagy meglévő ügyfelekkel üzleti kapcsolatban áll, meg kell adnia a vállalat regisztrációs azonosítószámait.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-161">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="ed4e8-162">Ha az alábbi listán nem szerepel az üzleti tevékenység országa, a regisztrációs azonosító megadása nem kötelező.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-162">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="ed4e8-163">Örményország</span><span class="sxs-lookup"><span data-stu-id="ed4e8-163">Armenia</span></span> 
- <span data-ttu-id="ed4e8-164">Azerbajdzsán</span><span class="sxs-lookup"><span data-stu-id="ed4e8-164">Azerbaijan</span></span> 
- <span data-ttu-id="ed4e8-165">Belarusz</span><span class="sxs-lookup"><span data-stu-id="ed4e8-165">Belarus</span></span> 
- <span data-ttu-id="ed4e8-166">Brazília</span><span class="sxs-lookup"><span data-stu-id="ed4e8-166">Brazil</span></span> 
- <span data-ttu-id="ed4e8-167">Magyarország</span><span class="sxs-lookup"><span data-stu-id="ed4e8-167">Hungary</span></span> 
- <span data-ttu-id="ed4e8-168">India</span><span class="sxs-lookup"><span data-stu-id="ed4e8-168">India</span></span> 
- <span data-ttu-id="ed4e8-169">Irak</span><span class="sxs-lookup"><span data-stu-id="ed4e8-169">Iraq</span></span> 
- <span data-ttu-id="ed4e8-170">Kazahsztán</span><span class="sxs-lookup"><span data-stu-id="ed4e8-170">Kazakhstan</span></span> 
- <span data-ttu-id="ed4e8-171">Kirgizisztán</span><span class="sxs-lookup"><span data-stu-id="ed4e8-171">Kyrgyzstan</span></span> 
- <span data-ttu-id="ed4e8-172">Moldova</span><span class="sxs-lookup"><span data-stu-id="ed4e8-172">Moldova</span></span> 
- <span data-ttu-id="ed4e8-173">Mianmar</span><span class="sxs-lookup"><span data-stu-id="ed4e8-173">Myanmar</span></span> 
- <span data-ttu-id="ed4e8-174">Lengyelország</span><span class="sxs-lookup"><span data-stu-id="ed4e8-174">Poland</span></span> 
- <span data-ttu-id="ed4e8-175">Oroszország</span><span class="sxs-lookup"><span data-stu-id="ed4e8-175">Russia</span></span> 
- <span data-ttu-id="ed4e8-176">Szaúd-Arábia</span><span class="sxs-lookup"><span data-stu-id="ed4e8-176">Saudi Arabia</span></span> 
- <span data-ttu-id="ed4e8-177">Dél-afrikai Köztársaság</span><span class="sxs-lookup"><span data-stu-id="ed4e8-177">South Africa</span></span> 
- <span data-ttu-id="ed4e8-178">Dél-Szudán</span><span class="sxs-lookup"><span data-stu-id="ed4e8-178">South Sudan</span></span>  
- <span data-ttu-id="ed4e8-179">Tádzsikisztán</span><span class="sxs-lookup"><span data-stu-id="ed4e8-179">Tajikistan</span></span> 
- <span data-ttu-id="ed4e8-180">Thaiföld</span><span class="sxs-lookup"><span data-stu-id="ed4e8-180">Thailand</span></span>
- <span data-ttu-id="ed4e8-181">Törökország</span><span class="sxs-lookup"><span data-stu-id="ed4e8-181">Turkey</span></span> 
- <span data-ttu-id="ed4e8-182">Ukrajna</span><span class="sxs-lookup"><span data-stu-id="ed4e8-182">Ukraine</span></span> 
- <span data-ttu-id="ed4e8-183">Egyesült Arab Emírségek</span><span class="sxs-lookup"><span data-stu-id="ed4e8-183">United Arab Emirates</span></span> 
- <span data-ttu-id="ed4e8-184">Üzbegisztán</span><span class="sxs-lookup"><span data-stu-id="ed4e8-184">Uzbekistan</span></span> 
- <span data-ttu-id="ed4e8-185">Venezuela</span><span class="sxs-lookup"><span data-stu-id="ed4e8-185">Venezuela</span></span>
- <span data-ttu-id="ed4e8-186">Vietnam</span><span class="sxs-lookup"><span data-stu-id="ed4e8-186">Vietnam</span></span> 


<span data-ttu-id="ed4e8-187">További információkért olvassa el a [regisztrációs azonosító száminformációját.](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="ed4e8-187">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="ed4e8-188">Hely törlése</span><span class="sxs-lookup"><span data-stu-id="ed4e8-188">Delete a location</span></span>

<span data-ttu-id="ed4e8-189">Egy hely fiókból való törléséhez fel kell vennie a kapcsolatot a [partnertámogatással.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)</span><span class="sxs-lookup"><span data-stu-id="ed4e8-189">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="ed4e8-190">Győződjön meg arról, hogy megértette ennek a műveletnek a hatását.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-190">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="ed4e8-191">Törölt helyek nem olvashatók be, és az adott MPN-azonosítóhoz kötődő adatokat a rendszer többé nem ismeri fel vagy nem aktív a vállalatnál.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-191">Deleted locations cannot be retrieved and anything tied to that specific MPN ID will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="ed4e8-192">Partner globális fiókjának országának módosítása</span><span class="sxs-lookup"><span data-stu-id="ed4e8-192">Change country of Partner global account</span></span> 

1. <span data-ttu-id="ed4e8-193">Jelentkezzen be az MPN-fiókkal a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-193">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="ed4e8-194">(Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól.) Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell lennie.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-194">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="ed4e8-195">A **Partner lapon** válassza az Üzleti **helyek** lapot, és ellenőrizze a helyek listáját, és ellenőrizze, hogy a jogi személyként kívánt hely szerepel-e a listán.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-195">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="ed4e8-196">Hely hozzáadásához kattintson **az Add a location**(Hely hozzáadása) elemre, majd a úszó menüben adja meg a szükséges adatokat, beleértve a vállalathoz hozzáadni kívánt hely üzleti nevét, címét és elsődleges kapcsolattartóját.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-196">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="ed4e8-197">Válassza **az Ország/régió** legördülő lista melletti Ország **módosítása** lehetőséget, és kövesse a lépéseket.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-197">Select **Change your country** next to the **Country/region** drop-down list and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Jogi üzleti profil adatainak úszó panele":::

5. <span data-ttu-id="ed4e8-199">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-199">Select **Save**.</span></span>

6. <span data-ttu-id="ed4e8-200">Az MPN globális fiók országa az új jogi országra változik.</span><span class="sxs-lookup"><span data-stu-id="ed4e8-200">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="ed4e8-201">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ed4e8-201">Next steps</span></span>

- <span data-ttu-id="ed4e8-202">Ismerje meg az [ellenőrzési folyamatot.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="ed4e8-202">Learn about the [verification process](verification-responses.md).</span></span>
