---
title: Telephelyek kezelése a partneri fiókban
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Ismerje meg, hogyan vehet fel új helyet, és hogyan használják a Location MPN ID-t az ösztönző programok, a CSP-üzleti, az előfizetések és az egyéb tranzakciók során.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005902"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="e5985-103">Az MPN-fiók helyeinek kezelése és hely hozzáadása (törlése)</span><span class="sxs-lookup"><span data-stu-id="e5985-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="e5985-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="e5985-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e5985-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="e5985-105">Global admin</span></span>
- <span data-ttu-id="e5985-106">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="e5985-106">Account admin</span></span>

<span data-ttu-id="e5985-107">A hely MPN-azonosítója azonosítja a vállalat minden egyes helyét.</span><span class="sxs-lookup"><span data-stu-id="e5985-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="e5985-108">Az MPN-azonosítót a következő helyen regisztrálhatja az ösztönző programokban: a Cloud Solution Provider (CSP) üzletág és más üzleti tranzakciók.</span><span class="sxs-lookup"><span data-stu-id="e5985-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="e5985-109">A globális MPN-azonosító a nem tranzakciós tevékenységek, például a támogatási kérelmek esetében használatos.</span><span class="sxs-lookup"><span data-stu-id="e5985-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="e5985-110">A következő tipikus forgatókönyv:</span><span class="sxs-lookup"><span data-stu-id="e5985-110">The following is a typical scenario:</span></span>

<span data-ttu-id="e5985-111">A contoso az Egyesült királyságbeli partneri globális fiókkal (PGA) rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="e5985-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="e5985-112">Ez a regisztrált jogi üzleti tevékenység, globális MPN-azonosítója pedig az összes nem tranzakciós üzlet kezelésére szolgál.</span><span class="sxs-lookup"><span data-stu-id="e5985-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="e5985-113">A contoso az Egyesült Királyság, Franciaország és az Egyesült Államok területén is rendelkezik leányvállalatokkal vagy részlegekkel egyenértékű partneri hellyel (PLA).</span><span class="sxs-lookup"><span data-stu-id="e5985-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="e5985-114">Az MPN-fiók struktúrájában ezek a PLAsok egyedi Location MPN-azonosítóként jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="e5985-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="e5985-115">A PLAs a tranzakciós vállalkozások, például a CSP-vagy ösztönző programok esetében használatos.</span><span class="sxs-lookup"><span data-stu-id="e5985-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="e5985-116">A kifizetések adott helyszínekhez vannak kötve.</span><span class="sxs-lookup"><span data-stu-id="e5985-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="e5985-117">1-1 kapcsolat van a CSP-bérlő és az MPN-hely azonosítója között.</span><span class="sxs-lookup"><span data-stu-id="e5985-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN-helyszínek szerkezete":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="e5985-119">Előfeltételek új fiók hozzáadásához a CSP vállalat számára</span><span class="sxs-lookup"><span data-stu-id="e5985-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="e5985-120">Új CSP üzleti fiók hozzáadásához először győződjön meg arról, hogy teljesítette az előfeltételeket.</span><span class="sxs-lookup"><span data-stu-id="e5985-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="e5985-121">Rendelkeznie kell egy Location MPN-AZONOSÍTÓval abban az országban, ahol a CSP vállalatot szeretné elvégezni.</span><span class="sxs-lookup"><span data-stu-id="e5985-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="e5985-122">Új MPN-hely létrehozásához olvassa el az alábbi "MPN-hely hozzáadása" című szakaszt.</span><span class="sxs-lookup"><span data-stu-id="e5985-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="e5985-123">Új CSP közvetett viszonteladói regisztrációjának létrehozásához olvassa el a [közvetett szolgáltatók használata](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="e5985-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="e5985-124">Ne felejtse el bejelentkezni az **új** CSP-fiók **új** hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="e5985-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="e5985-125">Ne használja a meglévő hitelesítő adatait, mert a partneri központ már rendelkezik fiókkal.</span><span class="sxs-lookup"><span data-stu-id="e5985-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="e5985-126">Fogadja el a Microsoft partneri szerződést, és aktiválja a fiókot.</span><span class="sxs-lookup"><span data-stu-id="e5985-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="e5985-127">Ha közvetlen számlás partnerként szeretne regisztrálni, olvassa el [a közvetlen számlázási partnereinkre vonatkozó követelményeket](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="e5985-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="e5985-128">MPN-hely megtekintése</span><span class="sxs-lookup"><span data-stu-id="e5985-128">View your MPN locations</span></span>

1. <span data-ttu-id="e5985-129">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/home) az MPN-fiókja hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="e5985-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="e5985-130">(Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól)</span><span class="sxs-lookup"><span data-stu-id="e5985-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="e5985-131">A **Beállítások** ikonban válassza a **Fiókbeállítások**, **szervezeti profil**, **jogi** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e5985-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="e5985-132">A **partner** lapon ellenőrizze, hogy nincs-e szalagcím-hibaüzenet, amely arra kéri, hogy javítsa az áttelepített helyet a PMC-ból.</span><span class="sxs-lookup"><span data-stu-id="e5985-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="e5985-133">Ha van, kövesse az utasításokat, és javítsa ki ezeket a helyszíneket.</span><span class="sxs-lookup"><span data-stu-id="e5985-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="e5985-134">Ha nem jelenik meg hibaüzenet, a  **Beállítások** területen válassza a  **Fiókbeállítások**, **szervezeti profil**, **azonosítók** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e5985-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="e5985-135">Keresse meg a "location" típusú MPN-azonosítót, amely megfelel a CSP-fiók országának, és használja az alábbi kereséshez és a társítás befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="e5985-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="e5985-136">Ha nem találja a használni kívánt CSP-fióknak megfelelő Location MPN-azonosítót, új helyet is hozzáadhat, amely új MPN-azonosítót hoz létre.</span><span class="sxs-lookup"><span data-stu-id="e5985-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="e5985-137">Lásd: **MPN-hely hozzáadása** alább.</span><span class="sxs-lookup"><span data-stu-id="e5985-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="e5985-138">MPN-hely hozzáadása</span><span class="sxs-lookup"><span data-stu-id="e5985-138">Add an MPN location</span></span>

1. <span data-ttu-id="e5985-139">Jelentkezzen be az MPN-fiókkal a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="e5985-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="e5985-140">(Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól).</span><span class="sxs-lookup"><span data-stu-id="e5985-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="e5985-141">Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="e5985-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="e5985-142">A **Beállítások ikonban** válassza ki a **Fiókbeállítások** elemet, majd válassza a **szervezeti profil** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e5985-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="e5985-143">Válassza a **jogi** lehetőséget, majd a **partner** lapon válassza az **üzleti helyek lehetőséget,** majd kattintson a **hely hozzáadása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="e5985-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="e5985-144">Adja meg a szükséges adatokat, beleértve az üzleti nevet, a lakcímet és a kapcsolattartót a vállalatához hozzáadni kívánt helyhez.</span><span class="sxs-lookup"><span data-stu-id="e5985-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="e5985-145">Kattintson a **hely hozzáadása** gombra.</span><span class="sxs-lookup"><span data-stu-id="e5985-145">Click **Add location**.</span></span> <span data-ttu-id="e5985-146">Ekkor létrejön egy új MPN-azonosító az új helyhez, amelyet a CSP-tranzakciókhoz és-ösztönzőkhöz használhat.</span><span class="sxs-lookup"><span data-stu-id="e5985-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Új jogi üzleti tevékenység hozzáadása":::

> [!NOTE]
> <span data-ttu-id="e5985-148">Miután hozzáadta a helyet a partner Centerben, nem távolíthatja el.</span><span class="sxs-lookup"><span data-stu-id="e5985-148">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="e5985-149">Ha a megfelelő MPN-azonosítót használta a bejelentkezéshez, az **MPN** a partner Center bal oldali menüjében jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="e5985-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="e5985-150">Hely törlése</span><span class="sxs-lookup"><span data-stu-id="e5985-150">Delete a location</span></span>

<span data-ttu-id="e5985-151">Ha törölni szeretne egy helyet a fiókjából, kapcsolatba kell lépnie a [partner támogatási szolgálatával](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="e5985-151">To delete a location from your account you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="e5985-152">Győződjön meg arról, hogy tisztában van a művelet hatásával.</span><span class="sxs-lookup"><span data-stu-id="e5985-152">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="e5985-153">A törölt helyeket nem lehet beolvasni, és az adott MPN-azonosítóhoz kapcsolódó minden adat már nem ismerhető fel, vagy nem lesz aktív a vállalatnál.</span><span class="sxs-lookup"><span data-stu-id="e5985-153">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="e5985-154">Partner globális fiók országának módosítása</span><span class="sxs-lookup"><span data-stu-id="e5985-154">Change country of Partner global account</span></span> 

1. <span data-ttu-id="e5985-155">Jelentkezzen be az MPN-fiókkal a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="e5985-155">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="e5985-156">(Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól).</span><span class="sxs-lookup"><span data-stu-id="e5985-156">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="e5985-157">Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="e5985-157">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="e5985-158">A **partner** lapon lépjen az **üzleti helyek** elemre, és ellenőrizze a helyek listáját, és győződjön meg arról, hogy az Ön által használt hely szerepel a jogi személy listáján.</span><span class="sxs-lookup"><span data-stu-id="e5985-158">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="e5985-159">Hely hozzáadásához kattintson a **hely hozzáadása** lehetőségre, és a kilépéskor adja meg a szükséges adatokat, beleértve az üzleti nevét, a lakcímét és az elsődleges kapcsolattartót a vállalatához hozzáadni kívánt helyhez.</span><span class="sxs-lookup"><span data-stu-id="e5985-159">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="e5985-160">Válassza az ország **/régió** legördülő lista melletti **ország módosítása** lehetőséget, és kövesse a lépéseket.</span><span class="sxs-lookup"><span data-stu-id="e5985-160">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Jogi üzleti profilra vonatkozó adatvesztés":::

5. <span data-ttu-id="e5985-162">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="e5985-162">Click **Save**.</span></span>

6. <span data-ttu-id="e5985-163">Az MPN globális fiók országa az új jogi országra lesz módosítva.</span><span class="sxs-lookup"><span data-stu-id="e5985-163">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="e5985-164">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="e5985-164">Next steps</span></span>

- <span data-ttu-id="e5985-165">További információ az [ellenőrzési folyamatról](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="e5985-165">Learn about the [verification process](verification-responses.md).</span></span>
