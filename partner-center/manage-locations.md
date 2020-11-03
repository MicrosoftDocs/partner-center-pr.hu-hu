---
title: Telephelyek kezelése a partneri fiókban
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Ismerje meg, hogyan vehet fel új helyet, és hogyan használják a Location MPN ID-t az ösztönző programok, a CSP-üzleti, az előfizetések és az egyéb tranzakciók során.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c6b0fc84636befedbc51aa0672ce19110eb4d9aa
ms.sourcegitcommit: 1719ff11409cd6953602b7798f8cfe821b8ea15e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/15/2020
ms.locfileid: "92530427"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="93ede-103">Az MPN-fiók helyeinek kezelése és új hely hozzáadása</span><span class="sxs-lookup"><span data-stu-id="93ede-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="93ede-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="93ede-104">**Applies to**</span></span>

- <span data-ttu-id="93ede-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="93ede-105">Partner Center</span></span>

<span data-ttu-id="93ede-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="93ede-106">**Appropriate roles**</span></span>

- <span data-ttu-id="93ede-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="93ede-107">Global admin</span></span>
- <span data-ttu-id="93ede-108">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="93ede-108">Account admin</span></span>

<span data-ttu-id="93ede-109">A hely MPN-azonosítója azonosítja a vállalat minden egyes helyét.</span><span class="sxs-lookup"><span data-stu-id="93ede-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="93ede-110">Az MPN-azonosítót a következő helyen regisztrálhatja az ösztönző programokban: a Cloud Solution Provider (CSP) üzletág és más üzleti tranzakciók.</span><span class="sxs-lookup"><span data-stu-id="93ede-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="93ede-111">A globális MPN-azonosító a nem tranzakciós tevékenységek, például a támogatási kérelmek esetében használatos.</span><span class="sxs-lookup"><span data-stu-id="93ede-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="93ede-112">A következő tipikus forgatókönyv:</span><span class="sxs-lookup"><span data-stu-id="93ede-112">The following is a typical scenario:</span></span>

<span data-ttu-id="93ede-113">A contoso az Egyesült királyságbeli partneri globális fiókkal (PGA) rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="93ede-113">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="93ede-114">Ez a regisztrált jogi üzleti tevékenység, globális MPN-azonosítója pedig az összes nem tranzakciós üzlet kezelésére szolgál.</span><span class="sxs-lookup"><span data-stu-id="93ede-114">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="93ede-115">A contoso az Egyesült Királyság, Franciaország és az Egyesült Államok területén is rendelkezik leányvállalatokkal vagy részlegekkel egyenértékű partneri hellyel (PLA).</span><span class="sxs-lookup"><span data-stu-id="93ede-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="93ede-116">Az MPN-fiók struktúrájában ezek a PLAsok egyedi Location MPN-azonosítóként jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="93ede-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="93ede-117">A PLAs a tranzakciós vállalkozások, például a CSP-vagy ösztönző programok esetében használatos.</span><span class="sxs-lookup"><span data-stu-id="93ede-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="93ede-118">A kifizetések adott helyszínekhez vannak kötve.</span><span class="sxs-lookup"><span data-stu-id="93ede-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="93ede-119">1-1 kapcsolat van a CSP-bérlő és az MPN-hely azonosítója között.</span><span class="sxs-lookup"><span data-stu-id="93ede-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN-helyszínek szerkezete":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="93ede-121">Előfeltételek egy új hely megadásához a CSP vállalat számára</span><span class="sxs-lookup"><span data-stu-id="93ede-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="93ede-122">Új CSP üzleti hely hozzáadásához több előfeltétel van:</span><span class="sxs-lookup"><span data-stu-id="93ede-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="93ede-123">Rendelkeznie kell egy Location MPN-AZONOSÍTÓval abban az országban, ahol üzleti tevékenységet kíván végezni.</span><span class="sxs-lookup"><span data-stu-id="93ede-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="93ede-124">Szüksége lesz egy új Azure AD-bérlőre a [vállalati régióban](regional-authorization-overview.md) , amely még nincs regisztrálva a CSP-ben.</span><span class="sxs-lookup"><span data-stu-id="93ede-124">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="93ede-125">Hozza létre ezt a tanúsítványt a CSP-ben való regisztráláskor.</span><span class="sxs-lookup"><span data-stu-id="93ede-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="93ede-126">Az új HRE-bérlő használatával regisztráljon a CSP programba a régióban.</span><span class="sxs-lookup"><span data-stu-id="93ede-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="93ede-127">Jogi cég adatainak megadása, beleértve a jogi cég nevét, a lakcímét, az elsődleges kapcsolattartási adatokat.</span><span class="sxs-lookup"><span data-stu-id="93ede-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="93ede-128">Ez a fiók ellenőrzés alá kerül, ezért mindenképpen adjon meg érvényes információt.</span><span class="sxs-lookup"><span data-stu-id="93ede-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="93ede-129">Ne felejtse el bejelentkezni az **új** Azure ad-bérlő **új** hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="93ede-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="93ede-130">Ne használja a meglévő hitelesítő adatait, mert a partneri központ már rendelkezik fiókkal.</span><span class="sxs-lookup"><span data-stu-id="93ede-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="93ede-131">Fogadja el a Microsoft partneri szerződést, és aktiválja a fiókot.</span><span class="sxs-lookup"><span data-stu-id="93ede-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="93ede-132">MPN-hely hozzáadása</span><span class="sxs-lookup"><span data-stu-id="93ede-132">Add an MPN location</span></span>

1. <span data-ttu-id="93ede-133">Jelentkezzen be az MPN-fiókkal a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="93ede-133">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="93ede-134">Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="93ede-134">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="93ede-135">A **beállítás ikonban** válassza ki a **partner beállításait** .</span><span class="sxs-lookup"><span data-stu-id="93ede-135">From the **Setting icon** , select the **Partner settings** .</span></span>

2. <span data-ttu-id="93ede-136">Válasszon **helyet.**</span><span class="sxs-lookup"><span data-stu-id="93ede-136">Select **Locations.**</span></span>

3. <span data-ttu-id="93ede-137">Válassza a **hely hozzáadása** lehetőséget, és szúrja be a vállalathoz hozzáadni kívánt hely, valamint a helyhez tartozó elsődleges kapcsolattartó címe adatait.</span><span class="sxs-lookup"><span data-stu-id="93ede-137">Select **Add a location** , and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="93ede-138">Miután hozzáadta a helyet a partner Centerben, nem távolítható el.</span><span class="sxs-lookup"><span data-stu-id="93ede-138">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="93ede-139">Ha a megfelelő MPN-azonosítót használta a bejelentkezéshez, az **MPN** a partner Center bal oldali menüjében jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="93ede-139">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="93ede-140">Globális partneri fiók helyének módosítása</span><span class="sxs-lookup"><span data-stu-id="93ede-140">Change Global partner account location</span></span>

1. <span data-ttu-id="93ede-141">A **[helyek](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** lapon tekintse meg a helyek listáját, és győződjön meg arról, hogy az a hely, ahol a jogi személy szerepel.</span><span class="sxs-lookup"><span data-stu-id="93ede-141">On the **[Locations](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="93ede-142">Ha nem, adja hozzá.</span><span class="sxs-lookup"><span data-stu-id="93ede-142">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="A partner Center-fiókok helyei lap képernyőképe az összes aktuális hely listájáról.":::

2. <span data-ttu-id="93ede-144">Válassza a **partner profil** lehetőséget, majd válassza a **jogi üzleti profil frissítése** elemet.</span><span class="sxs-lookup"><span data-stu-id="93ede-144">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Képernyőfelvétel: a partneri központ fiókpartner-profiljának adatai a választható frissítési lehetőséggel.":::

3. <span data-ttu-id="93ede-146">Válassza ki a régiót és a jogi személyt, és **küldje** el.</span><span class="sxs-lookup"><span data-stu-id="93ede-146">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Képernyőfelvétel: a partner jogi üzleti profiljának frissítése legördülő listát jelenít meg az ország vagy régió és a jogi személy frissítéséhez.":::

## <a name="next-steps"></a><span data-ttu-id="93ede-148">További lépések</span><span class="sxs-lookup"><span data-stu-id="93ede-148">Next steps</span></span>

- <span data-ttu-id="93ede-149">További információ az [ellenőrzési folyamatról](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="93ede-149">Learn about the [verification process](verification-responses.md).</span></span>
