---
title: Telephelyek kezelése a partneri fiókban
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Ismerje meg, hogyan vehet fel új helyet, és hogyan használják a Location MPN ID-t az ösztönző programok, a CSP-üzleti, az előfizetések és az egyéb tranzakciók során.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925005"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="94f2f-103">Az MPN-fiók helyeinek kezelése és új hely hozzáadása</span><span class="sxs-lookup"><span data-stu-id="94f2f-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="94f2f-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="94f2f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="94f2f-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="94f2f-105">Global admin</span></span>
- <span data-ttu-id="94f2f-106">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="94f2f-106">Account admin</span></span>

<span data-ttu-id="94f2f-107">A hely MPN-azonosítója azonosítja a vállalat minden egyes helyét.</span><span class="sxs-lookup"><span data-stu-id="94f2f-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="94f2f-108">Az MPN-azonosítót a következő helyen regisztrálhatja az ösztönző programokban: a Cloud Solution Provider (CSP) üzletág és más üzleti tranzakciók.</span><span class="sxs-lookup"><span data-stu-id="94f2f-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="94f2f-109">A globális MPN-azonosító a nem tranzakciós tevékenységek, például a támogatási kérelmek esetében használatos.</span><span class="sxs-lookup"><span data-stu-id="94f2f-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="94f2f-110">A következő tipikus forgatókönyv:</span><span class="sxs-lookup"><span data-stu-id="94f2f-110">The following is a typical scenario:</span></span>

<span data-ttu-id="94f2f-111">A contoso az Egyesült királyságbeli partneri globális fiókkal (PGA) rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="94f2f-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="94f2f-112">Ez a regisztrált jogi üzleti tevékenység, globális MPN-azonosítója pedig az összes nem tranzakciós üzlet kezelésére szolgál.</span><span class="sxs-lookup"><span data-stu-id="94f2f-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="94f2f-113">A contoso az Egyesült Királyság, Franciaország és az Egyesült Államok területén is rendelkezik leányvállalatokkal vagy részlegekkel egyenértékű partneri hellyel (PLA).</span><span class="sxs-lookup"><span data-stu-id="94f2f-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="94f2f-114">Az MPN-fiók struktúrájában ezek a PLAsok egyedi Location MPN-azonosítóként jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="94f2f-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="94f2f-115">A PLAs a tranzakciós vállalkozások, például a CSP-vagy ösztönző programok esetében használatos.</span><span class="sxs-lookup"><span data-stu-id="94f2f-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="94f2f-116">A kifizetések adott helyszínekhez vannak kötve.</span><span class="sxs-lookup"><span data-stu-id="94f2f-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="94f2f-117">1-1 kapcsolat van a CSP-bérlő és az MPN-hely azonosítója között.</span><span class="sxs-lookup"><span data-stu-id="94f2f-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN-helyszínek szerkezete":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="94f2f-119">Előfeltételek új fiók hozzáadásához a CSP vállalat számára</span><span class="sxs-lookup"><span data-stu-id="94f2f-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="94f2f-120">Új CSP üzleti fiók hozzáadásához először győződjön meg arról, hogy teljesítette az előfeltételeket.</span><span class="sxs-lookup"><span data-stu-id="94f2f-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="94f2f-121">Rendelkeznie kell egy Location MPN-AZONOSÍTÓval abban az országban, ahol a CSP vállalatot szeretné elvégezni.</span><span class="sxs-lookup"><span data-stu-id="94f2f-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="94f2f-122">Új MPN-hely létrehozásához olvassa el az alábbi "MPN-hely hozzáadása" című szakaszt.</span><span class="sxs-lookup"><span data-stu-id="94f2f-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="94f2f-123">Új CSP közvetett viszonteladói regisztrációjának létrehozásához olvassa el a [közvetett szolgáltatók használata](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="94f2f-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="94f2f-124">Ne felejtse el bejelentkezni az **új** CSP-fiók **új** hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="94f2f-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="94f2f-125">Ne használja a meglévő hitelesítő adatait, mert a partneri központ már rendelkezik fiókkal.</span><span class="sxs-lookup"><span data-stu-id="94f2f-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="94f2f-126">Fogadja el a Microsoft partneri szerződést, és aktiválja a fiókot.</span><span class="sxs-lookup"><span data-stu-id="94f2f-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="94f2f-127">MPN-hely hozzáadása</span><span class="sxs-lookup"><span data-stu-id="94f2f-127">Add an MPN location</span></span>

1. <span data-ttu-id="94f2f-128">Jelentkezzen be az MPN-fiókkal a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="94f2f-128">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="94f2f-129">(Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól).</span><span class="sxs-lookup"><span data-stu-id="94f2f-129">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="94f2f-130">Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="94f2f-130">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="94f2f-131">A **Beállítások ikonban** válassza ki a **Fiókbeállítások** elemet, majd válassza a **szervezeti profil** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="94f2f-131">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="94f2f-132">Válassza a **jogi** lehetőséget, majd a **partner** lapon válassza az **üzleti helyek lehetőséget,** majd kattintson a **hely hozzáadása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="94f2f-132">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="94f2f-133">Adja meg a szükséges adatokat, beleértve az üzleti nevet, a lakcímet és a kapcsolattartót a vállalatához hozzáadni kívánt helyhez.</span><span class="sxs-lookup"><span data-stu-id="94f2f-133">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="94f2f-134">Kattintson a **hely hozzáadása** gombra.</span><span class="sxs-lookup"><span data-stu-id="94f2f-134">Click **Add location**.</span></span> <span data-ttu-id="94f2f-135">Ekkor létrejön egy új MPN-azonosító az új helyhez, amelyet a CSP-tranzakciókhoz és-ösztönzőkhöz használhat.</span><span class="sxs-lookup"><span data-stu-id="94f2f-135">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Új jogi üzleti tevékenység hozzáadása":::

> [!NOTE]
> <span data-ttu-id="94f2f-137">Miután hozzáadta a helyet a partner Centerben, nem távolítható el.</span><span class="sxs-lookup"><span data-stu-id="94f2f-137">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="94f2f-138">Ha a megfelelő MPN-azonosítót használta a bejelentkezéshez, az **MPN** a partner Center bal oldali menüjében jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="94f2f-138">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="94f2f-139">Partner globális fiók országának módosítása</span><span class="sxs-lookup"><span data-stu-id="94f2f-139">Change country of Partner global account</span></span> 

1. <span data-ttu-id="94f2f-140">Jelentkezzen be az MPN-fiókkal a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="94f2f-140">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="94f2f-141">(Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól).</span><span class="sxs-lookup"><span data-stu-id="94f2f-141">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="94f2f-142">Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="94f2f-142">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="94f2f-143">A **partner** lapon lépjen az **üzleti helyek** elemre, és ellenőrizze a helyek listáját, és győződjön meg arról, hogy az Ön által használt hely szerepel a jogi személy listáján.</span><span class="sxs-lookup"><span data-stu-id="94f2f-143">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="94f2f-144">Hely hozzáadásához kattintson a **hely hozzáadása** lehetőségre, és a kilépéskor adja meg a szükséges adatokat, beleértve az üzleti nevét, a lakcímét és az elsődleges kapcsolattartót a vállalatához hozzáadni kívánt helyhez.</span><span class="sxs-lookup"><span data-stu-id="94f2f-144">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="94f2f-145">Válassza az ország **/régió** legördülő lista melletti **ország módosítása** lehetőséget, és kövesse a lépéseket.</span><span class="sxs-lookup"><span data-stu-id="94f2f-145">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Jogi üzleti profilra vonatkozó adatvesztés":::

5. <span data-ttu-id="94f2f-147">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="94f2f-147">Click **Save**.</span></span>

6. <span data-ttu-id="94f2f-148">Az MPN globális fiók országa az új jogi országra lesz módosítva.</span><span class="sxs-lookup"><span data-stu-id="94f2f-148">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="94f2f-149">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="94f2f-149">Next steps</span></span>

- <span data-ttu-id="94f2f-150">További információ az [ellenőrzési folyamatról](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="94f2f-150">Learn about the [verification process](verification-responses.md).</span></span>
