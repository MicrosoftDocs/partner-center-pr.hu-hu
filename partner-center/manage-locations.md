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
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702892"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="c9da5-103">Az MPN-fiók helyének kezelése és hely hozzáadása (törlése)</span><span class="sxs-lookup"><span data-stu-id="c9da5-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="c9da5-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="c9da5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c9da5-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="c9da5-105">Global admin</span></span>
- <span data-ttu-id="c9da5-106">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="c9da5-106">Account admin</span></span>

<span data-ttu-id="c9da5-107">A hely MPN-azonosítója azonosítja a vállalat minden egyes helyét.</span><span class="sxs-lookup"><span data-stu-id="c9da5-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="c9da5-108">A hely MPN-azonosítójával regisztrál az ösztönzőprogramokba, tranzakciókat Felhőszolgáltató (CSP) és egyéb üzleti tranzakciókat.</span><span class="sxs-lookup"><span data-stu-id="c9da5-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="c9da5-109">A globális MPN-azonosítót nem tranzakciós tevékenységekhez, például támogatási kérelmekhez használjuk.</span><span class="sxs-lookup"><span data-stu-id="c9da5-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="c9da5-110">A következő forgatókönyv jellemző:</span><span class="sxs-lookup"><span data-stu-id="c9da5-110">The following scenario is typical:</span></span>

<span data-ttu-id="c9da5-111">A Contoso globális partnerfiókkal (PGA) rendelkezik az Egyesült Királyságban.</span><span class="sxs-lookup"><span data-stu-id="c9da5-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="c9da5-112">A PGA a regisztrált jogi vállalkozásuk, és globális MPN-azonosítóját az összes nem tranzakciós üzlet felügyeletére használják.</span><span class="sxs-lookup"><span data-stu-id="c9da5-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="c9da5-113">A Contoso emellett partnerihely-fiókokkal (PLA) is rendelkezik, amelyek egyenértékűek az Egyesült Királyság, Franciaország és az Egyesült Államok más helyeiben található leányvállalatokkal vagy részlegekkel.</span><span class="sxs-lookup"><span data-stu-id="c9da5-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="c9da5-114">Az MPN-fiók struktúrájában ezek a PLA-k egyedi hely MPN-azonosítókként vannak ábrázolva.</span><span class="sxs-lookup"><span data-stu-id="c9da5-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="c9da5-115">A PLA-k tranzakciós üzleti tevékenységhez, például CSP- vagy ösztönzőprogramokhoz használhatók.</span><span class="sxs-lookup"><span data-stu-id="c9da5-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="c9da5-116">A kifizetések adott helyekhez vannak kötve.</span><span class="sxs-lookup"><span data-stu-id="c9da5-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="c9da5-117">Egy CSP-bérlő és egy MPN-helyazonosító között 1–1 kapcsolat áll elő.</span><span class="sxs-lookup"><span data-stu-id="c9da5-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Az MPN-helyek szerkezete":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="c9da5-119">Új fiók csp-vállalkozáshoz való hozzáadásának előfeltételei</span><span class="sxs-lookup"><span data-stu-id="c9da5-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="c9da5-120">Új VÁLLALATI CSP-fiók hozzáadásához először is meg kell bizonyosodni arról, hogy teljesülnek az előfeltételek.</span><span class="sxs-lookup"><span data-stu-id="c9da5-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="c9da5-121">A CSP-üzletnek abban az országban kell lennie, ahol az MPN-azonosítót el szeretné látni.</span><span class="sxs-lookup"><span data-stu-id="c9da5-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="c9da5-122">Új MPN-hely létrehozásához olvassa el alább az "MPN-hely hozzáadása" adatokat.</span><span class="sxs-lookup"><span data-stu-id="c9da5-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="c9da5-123">Új regisztráció létrehozásához CSP Indirect Reseller: Közvetett [szolgáltatókkal való munka](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="c9da5-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="c9da5-124">Ne felejtsen el bejelentkezni az **új** CSP-fiók új hitelesítő adataival. </span><span class="sxs-lookup"><span data-stu-id="c9da5-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="c9da5-125">Ne használja a meglévő hitelesítő adatait, mert Partnerközpont a rendszer felismeri, hogy már rendelkezik fiókkal.</span><span class="sxs-lookup"><span data-stu-id="c9da5-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="c9da5-126">Fogadja el Microsoft Partnerszerződés és aktiválja a fiókot.</span><span class="sxs-lookup"><span data-stu-id="c9da5-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="c9da5-127">Ha közvetlen számlázási partnerként szeretne regisztrálni, olvassa el a [Következőt: A közvetlen számlázási partnerekre vonatkozó követelmények](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="c9da5-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="c9da5-128">MPN-helyek megtekintése és frissítése</span><span class="sxs-lookup"><span data-stu-id="c9da5-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="c9da5-129">Jelentkezzen be az Partnerközpont [irányítópultra](https://partner.microsoft.com/dashboard/home) az MPN-fiókja hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="c9da5-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="c9da5-130">(Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól)</span><span class="sxs-lookup"><span data-stu-id="c9da5-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="c9da5-131">A Beállítások **ikonon** válassza a **Fiókbeállítások,** Szervezeti **profil,** **Jogi lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c9da5-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="c9da5-132">A **Partner lapon** ellenőrizze, hogy nem jelenik-e meg szalagcímes hibaüzenet, amely a PMC-ről migrált helyek kijavításán kéri.</span><span class="sxs-lookup"><span data-stu-id="c9da5-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="c9da5-133">Ha a helyek nem megfelelően vannak beállítva a PMC-n, és még nem voltak pc-re állítva, frissítenie kell ezeket a helyeket.</span><span class="sxs-lookup"><span data-stu-id="c9da5-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="A képernyőkép bemutatja, hogyan frissítheti a helyet.":::
 
4.  <span data-ttu-id="c9da5-135">A **PMC-helyek áttekintése képernyőn** válassza a Frissítés **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c9da5-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="c9da5-136">Frissítse a következő mezőket:</span><span class="sxs-lookup"><span data-stu-id="c9da5-136">Update the following fields:</span></span>

- <span data-ttu-id="c9da5-137">**Név mező:** Győződjön meg arról, hogy a vállalat helyének neve helyes.</span><span class="sxs-lookup"><span data-stu-id="c9da5-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="c9da5-138">Ha duplikált hiba jelenik meg, próbáljon meg átváltást például a Contoso-ről a Contoso, Inc. fiókra.</span><span class="sxs-lookup"><span data-stu-id="c9da5-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="c9da5-139">**Jogi személy mező:** Győződjön meg arról, hogy azt a jogi entitást választotta ki, amelyhez a hely kötődik</span><span class="sxs-lookup"><span data-stu-id="c9da5-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="c9da5-140">**Az 1. & 2. mező:** Győződjön meg arról, hogy a cím helyes</span><span class="sxs-lookup"><span data-stu-id="c9da5-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="c9da5-141">**City & State/Province (Állam/Tartomány)** mezőkben: Győződjön meg arról, hogy a város és az állam/tartomány közötti kombináció helyes.</span><span class="sxs-lookup"><span data-stu-id="c9da5-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="c9da5-142">Vannak országok, ahol a State/Province (Állam/Tartomány) kiválasztására vonatkozó legördülő menüt kell alkalmazni, és más országokban a mezőt manuálisan kell beszúrni.</span><span class="sxs-lookup"><span data-stu-id="c9da5-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="c9da5-143">**IRÁNYÍTÓSZÁM mező:** Győződjön meg arról, hogy az Irányítószám mező megfelel a megadott országnak, régiónak, városnak vagy címnek.</span><span class="sxs-lookup"><span data-stu-id="c9da5-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="c9da5-144">**Elsődleges kapcsolattartási adatok mezői:** Győződjön meg arról, hogy az első és a vezetéknév mező ki van töltve, és hogy a megadott e-mail-cím munkahelyi e-mail-cím, nem pedig személyes cím (például @outlook.com , @live.com stb.)</span><span class="sxs-lookup"><span data-stu-id="c9da5-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="c9da5-145">**Telefonszám mező:** Győződjön meg arról, hogy a Telefonszám NEM tartalmaz speciális karaktereket, szóközöket vagy országkódot.</span><span class="sxs-lookup"><span data-stu-id="c9da5-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="c9da5-146">A Telefonszám mezőben megadott érték mindig legfeljebb 10 karaktert tartalmazhat.</span><span class="sxs-lookup"><span data-stu-id="c9da5-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="c9da5-147">Ha nem jelenik meg hibaüzenet, akkor a Beállítások lapon válassza a Fiókbeállítások, a Szervezeti **profil,** az **Azonosítók lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c9da5-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="c9da5-148">Keresse meg a "Hely" típusú MPN-azonosítót, amely megfelel a CSP-fiók országának, és használja a társítás befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="c9da5-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="c9da5-149">Ha nem találja a használni kívánt CSP-fióknak megfelelő hely MPN-azonosítót, hozzáadhat egy új helyet, amely létrehoz egy új MPN-azonosítót.</span><span class="sxs-lookup"><span data-stu-id="c9da5-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="c9da5-150">Lásd **alább az MPN-hely hozzáadását.**</span><span class="sxs-lookup"><span data-stu-id="c9da5-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="c9da5-151">MPN-hely hozzáadása</span><span class="sxs-lookup"><span data-stu-id="c9da5-151">Add an MPN location</span></span>

1. <span data-ttu-id="c9da5-152">Jelentkezzen be az MPN-fiókkal a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="c9da5-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="c9da5-153">(Az MPN hitelesítő adatai különbözhetnek a CSP hitelesítő adataitól) .</span><span class="sxs-lookup"><span data-stu-id="c9da5-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="c9da5-154">Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultsággal kell lennie.</span><span class="sxs-lookup"><span data-stu-id="c9da5-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="c9da5-155">A Beállítások **ikonra kattintva** válassza a **Fiókbeállítások,** majd a Szervezeti **profil lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c9da5-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="c9da5-156">Válassza **a Jogi** lehetőséget, majd a Partner **lapon** válassza az Üzleti **helyek lehetőséget,** majd kattintson a Hely **hozzáadása elemre.**</span><span class="sxs-lookup"><span data-stu-id="c9da5-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="c9da5-157">Adja meg a szükséges adatokat, beleértve a vállalathoz hozzáadni kívánt hely nevét, címét és kapcsolattartóját.</span><span class="sxs-lookup"><span data-stu-id="c9da5-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="c9da5-158">Kattintson **a Hely hozzáadása elemre.**</span><span class="sxs-lookup"><span data-stu-id="c9da5-158">Click **Add location**.</span></span> <span data-ttu-id="c9da5-159">Ezzel létrehoz egy új MPN-azonosítót az új helyhez, amelyet a CSP-tranzakciókhoz és -ösztönzőkhez használhat.</span><span class="sxs-lookup"><span data-stu-id="c9da5-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Új jogi vállalkozás hozzáadása":::

> [!NOTE]
> <span data-ttu-id="c9da5-161">Miután hozzáadott egy helyet a Partnerközpont, nem távolíthatja el.</span><span class="sxs-lookup"><span data-stu-id="c9da5-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="c9da5-162">Ha a megfelelő **MPN-azonosítót** használta a bejelentkezéshez Partnerközpont az MPN megjelenik a bal oldali menüben.</span><span class="sxs-lookup"><span data-stu-id="c9da5-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="c9da5-163">A regisztrációs szám azonosítójának hozzáadása</span><span class="sxs-lookup"><span data-stu-id="c9da5-163">Add the registration number ID</span></span>

<span data-ttu-id="c9da5-164">Ha Ön közvetett szolgáltató, közvetlen számlázási partner vagy közvetett viszonteladó, és a következő országokban új vagy meglévő ügyfelekkel üzleti kapcsolatban áll, meg kell adnia a vállalat regisztrációs azonosítószámait.</span><span class="sxs-lookup"><span data-stu-id="c9da5-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="c9da5-165">Ha az az ország, ahol a vállalkozása található, nem szerepel az alábbi listában, a regisztrációs azonosító megadása nem kötelező.</span><span class="sxs-lookup"><span data-stu-id="c9da5-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="c9da5-166">Örményország</span><span class="sxs-lookup"><span data-stu-id="c9da5-166">Armenia</span></span> 
- <span data-ttu-id="c9da5-167">Azerbajdzsán</span><span class="sxs-lookup"><span data-stu-id="c9da5-167">Azerbaijan</span></span> 
- <span data-ttu-id="c9da5-168">Belarusz</span><span class="sxs-lookup"><span data-stu-id="c9da5-168">Belarus</span></span> 
- <span data-ttu-id="c9da5-169">Brazília</span><span class="sxs-lookup"><span data-stu-id="c9da5-169">Brazil</span></span> 
- <span data-ttu-id="c9da5-170">Magyarország</span><span class="sxs-lookup"><span data-stu-id="c9da5-170">Hungary</span></span> 
- <span data-ttu-id="c9da5-171">India</span><span class="sxs-lookup"><span data-stu-id="c9da5-171">India</span></span> 
- <span data-ttu-id="c9da5-172">Irak</span><span class="sxs-lookup"><span data-stu-id="c9da5-172">Iraq</span></span> 
- <span data-ttu-id="c9da5-173">Kazahsztán</span><span class="sxs-lookup"><span data-stu-id="c9da5-173">Kazakhstan</span></span> 
- <span data-ttu-id="c9da5-174">Kirgizisztán</span><span class="sxs-lookup"><span data-stu-id="c9da5-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="c9da5-175">Moldova</span><span class="sxs-lookup"><span data-stu-id="c9da5-175">Moldova</span></span> 
- <span data-ttu-id="c9da5-176">Mianmar</span><span class="sxs-lookup"><span data-stu-id="c9da5-176">Myanmar</span></span> 
- <span data-ttu-id="c9da5-177">Lengyelország</span><span class="sxs-lookup"><span data-stu-id="c9da5-177">Poland</span></span> 
- <span data-ttu-id="c9da5-178">Oroszország</span><span class="sxs-lookup"><span data-stu-id="c9da5-178">Russia</span></span> 
- <span data-ttu-id="c9da5-179">Szaúd-Arábia</span><span class="sxs-lookup"><span data-stu-id="c9da5-179">Saudi Arabia</span></span> 
- <span data-ttu-id="c9da5-180">Dél-afrikai Köztársaság</span><span class="sxs-lookup"><span data-stu-id="c9da5-180">South Africa</span></span> 
- <span data-ttu-id="c9da5-181">Dél-Szudán</span><span class="sxs-lookup"><span data-stu-id="c9da5-181">South Sudan</span></span>  
- <span data-ttu-id="c9da5-182">Tádzsikisztán</span><span class="sxs-lookup"><span data-stu-id="c9da5-182">Tajikistan</span></span> 
- <span data-ttu-id="c9da5-183">Thaiföld</span><span class="sxs-lookup"><span data-stu-id="c9da5-183">Thailand</span></span>
- <span data-ttu-id="c9da5-184">Törökország</span><span class="sxs-lookup"><span data-stu-id="c9da5-184">Turkey</span></span> 
- <span data-ttu-id="c9da5-185">Ukrajna</span><span class="sxs-lookup"><span data-stu-id="c9da5-185">Ukraine</span></span> 
- <span data-ttu-id="c9da5-186">Egyesült Arab Emírségek</span><span class="sxs-lookup"><span data-stu-id="c9da5-186">United Arab Emirates</span></span> 
- <span data-ttu-id="c9da5-187">Üzbegisztán</span><span class="sxs-lookup"><span data-stu-id="c9da5-187">Uzbekistan</span></span> 
- <span data-ttu-id="c9da5-188">Venezuela</span><span class="sxs-lookup"><span data-stu-id="c9da5-188">Venezuela</span></span>
- <span data-ttu-id="c9da5-189">Vietnam</span><span class="sxs-lookup"><span data-stu-id="c9da5-189">Vietnam</span></span> 


<span data-ttu-id="c9da5-190">További információkért olvassa el a [regisztrációs azonosító száminformációját.](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="c9da5-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="c9da5-191">Hely törlése</span><span class="sxs-lookup"><span data-stu-id="c9da5-191">Delete a location</span></span>

<span data-ttu-id="c9da5-192">Egy hely fiókból való törléséhez fel kell vennie a kapcsolatot a [partnertámogatással.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)</span><span class="sxs-lookup"><span data-stu-id="c9da5-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="c9da5-193">Győződjön meg arról, hogy megértette ennek a műveletnek a hatását.</span><span class="sxs-lookup"><span data-stu-id="c9da5-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="c9da5-194">Törölt helyek nem olvashatók be, és az adott MPN-azonosítóhoz kötődő adatokat a rendszer nem ismeri fel és nem aktív a vállalatnál.</span><span class="sxs-lookup"><span data-stu-id="c9da5-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="c9da5-195">Partner globális fiókjának országának módosítása</span><span class="sxs-lookup"><span data-stu-id="c9da5-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="c9da5-196">Jelentkezzen be az MPN-fiókkal a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="c9da5-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="c9da5-197">(Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól) .</span><span class="sxs-lookup"><span data-stu-id="c9da5-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="c9da5-198">Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell lennie.</span><span class="sxs-lookup"><span data-stu-id="c9da5-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="c9da5-199">A **Partner lapon** válassza az Üzleti **helyek** lapot, és ellenőrizze a helyek listáját, és ellenőrizze, hogy a jogi személyként kívánt hely szerepel-e a listán.</span><span class="sxs-lookup"><span data-stu-id="c9da5-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="c9da5-200">Hely hozzáadásához kattintson **az Add a location**(Hely hozzáadása) elemre, majd a úszó menüben adja meg a szükséges adatokat, beleértve a vállalathoz hozzáadni kívánt hely üzleti nevét, címét és elsődleges kapcsolattartóját.</span><span class="sxs-lookup"><span data-stu-id="c9da5-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="c9da5-201">Válassza **az Ország/régió** legördülő lista Melletti Ország **módosítása** lehetőséget, és kövesse a lépéseket.</span><span class="sxs-lookup"><span data-stu-id="c9da5-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Jogi üzleti profil adatainak úszó panele":::

5. <span data-ttu-id="c9da5-203">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="c9da5-203">Click **Save**.</span></span>

6. <span data-ttu-id="c9da5-204">Az MPN globális fiók országa az új jogi országra változik.</span><span class="sxs-lookup"><span data-stu-id="c9da5-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="c9da5-205">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c9da5-205">Next steps</span></span>

- <span data-ttu-id="c9da5-206">Ismerje meg az [ellenőrzési folyamatot.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="c9da5-206">Learn about the [verification process](verification-responses.md).</span></span>
