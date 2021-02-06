---
title: Kifizetések és adóprofilok a Partnerközpontban
ms.topic: how-to
ms.date: 11/12/2020
description: Létrehozhatja és kezelheti a kifizetési és az adózási profilt, így Ön fizethet az ösztönzőkért. Ide tartozik a különböző profilok létrehozása, kezelése és használata.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 282fdacc8689ff71e885a2f0ea01ce9570611707
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624238"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="7152b-104">Ösztönzők létrehozása és kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="7152b-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>


<span data-ttu-id="7152b-105">**Megfelelő szerepkörök:**</span><span class="sxs-lookup"><span data-stu-id="7152b-105">**Appropriate roles:**</span></span>

- <span data-ttu-id="7152b-106">Ösztönzők rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="7152b-106">Incentives admin</span></span>
- <span data-ttu-id="7152b-107">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="7152b-107">Account admin</span></span>
- <span data-ttu-id="7152b-108">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="7152b-108">Global admin</span></span>

<span data-ttu-id="7152b-109">Ahhoz, hogy megkaphassa az egy adott MPN-helyhez tartozó ösztönzőprogramok kifizetését, be kell fejeznie a regisztrációt úgy, hogy a programhoz és az MPN-helyhez egy érvényes kifizetési és adóprofilt társít.</span><span class="sxs-lookup"><span data-stu-id="7152b-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="7152b-110">A Microsoft ezt a kifizetési és adóprofilt a kifizetésekhez fogja használni.</span><span class="sxs-lookup"><span data-stu-id="7152b-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="7152b-111">Az ösztönzőprogram szabályaitól függően lehetséges elektronikus banki átutalás vagy jóváírási értesítés használata is a kifizetéshez.</span><span class="sxs-lookup"><span data-stu-id="7152b-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="7152b-112">Szerepkörök, pénznemek és egyéb Microsoft-programok</span><span class="sxs-lookup"><span data-stu-id="7152b-112">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="7152b-113">Fontos megérteni az alábbi információkat, mielőtt megkezdi a befizetést és az adózási profilt.</span><span class="sxs-lookup"><span data-stu-id="7152b-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="7152b-114">Szerepkörök és engedélyek</span><span class="sxs-lookup"><span data-stu-id="7152b-114">Roles and permissions</span></span>

<span data-ttu-id="7152b-115">Az ösztönző befizetések esetén a banki és adózási információk megadásához ösztönző rendszergazdának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="7152b-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="7152b-116">Ha Ön MPN/fiók rendszergazdája, rendeljen hozzá önmagát és/vagy kollégáját, hogy az ösztönözze a rendszergazdát.</span><span class="sxs-lookup"><span data-stu-id="7152b-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="7152b-117">Ha ösztönző rendszergazdai jogosultságokat kell kérnie, forduljon az MPN-rendszergazdához vagy a globális rendszergazdához. A [partner Center irányítópultra](https://partner.microsoft.com/dashboard/)való bejelentkezéssel megállapíthatja, hogy kik a vállalatnál vannak ezek a szerepkörök.</span><span class="sxs-lookup"><span data-stu-id="7152b-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="7152b-118">Kattintson a jobb felső sarokban található **Beállítások** ikonra, válassza a **felhasználói kezelés** , majd a globális rendszergazda szűrése lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7152b-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="7152b-119">Ösztönzők a felhasználók megtekinthetik az ösztönző bevételeket és a fizetési adatokat és jelentéseket, de nem szerkeszthetik a bank és az adó adatait.</span><span class="sxs-lookup"><span data-stu-id="7152b-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="7152b-120">Válassza ki a kifizetés pénznemét</span><span class="sxs-lookup"><span data-stu-id="7152b-120">Choose your disbursement currency</span></span>

<span data-ttu-id="7152b-121">Az ösztönző kifizetések a fizetési profil beállításakor kiválasztott pénznemben történnek.</span><span class="sxs-lookup"><span data-stu-id="7152b-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="7152b-122">A fizetések kiszámítása a Microsoft által havonta beállított árfolyamon történik.</span><span class="sxs-lookup"><span data-stu-id="7152b-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="7152b-123">A kiválasztott pénznem miatt az érték változásaiért felelős lesz.</span><span class="sxs-lookup"><span data-stu-id="7152b-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="7152b-124">Különböző profilok használata különböző Microsoft-programokhoz</span><span class="sxs-lookup"><span data-stu-id="7152b-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="7152b-125">Ha a vállalata több ösztönző programban is regisztrálva van, használhatja ugyanazt a fizetési fiókot, vagy választhat, hogy különböző fizetési fiókokat szeretne használni a különböző programokhoz.</span><span class="sxs-lookup"><span data-stu-id="7152b-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="7152b-126">Kifizetési és adózási profilok létrehozása és kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="7152b-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="7152b-127">Az alábbi szakasz végigvezeti a fizetési és adózási profilok a partner Centerben való létrehozásának és kezelésének folyamatán.</span><span class="sxs-lookup"><span data-stu-id="7152b-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="7152b-128">A fizetési profilok a partner Centerben való létrehozásához és kezeléséhez ösztönző rendszergazdának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="7152b-128">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="7152b-129">Az ösztönző szerepköröket minden egyes, az egyes ösztönző programok alá tartozó MPN-helyhez hozzá kell rendelni.</span><span class="sxs-lookup"><span data-stu-id="7152b-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="7152b-130">Az ösztönző rendszergazdák a partner Centerben való hozzáadásával kapcsolatos további információkért lásd: [felhasználói fiókok létrehozása](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="7152b-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="7152b-131">A partner Center kifizetési és adózási szakaszának elérése</span><span class="sxs-lookup"><span data-stu-id="7152b-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="7152b-132">Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard/) a Azure Active Directory-(Azure ad-) fiókkal (vállalati fiókkal) vagy a megfelelő e-mail-címmel, ha az egyik hozzá lett rendelve.</span><span class="sxs-lookup"><span data-stu-id="7152b-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="7152b-133">Egy Azure AD-fiókban több tartomány is regisztrálható.</span><span class="sxs-lookup"><span data-stu-id="7152b-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="7152b-134">Forduljon a globális rendszergazdához, és állapítsa meg, hogy mely tartományok vannak társítva.</span><span class="sxs-lookup"><span data-stu-id="7152b-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="7152b-135">Ha csak a tartományba tud bejelentkezni @onmicrosoft.com , lépjen kapcsolatba a fiók rendszergazdájával, és adjon hozzá további tartományokat az Azure ad-fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="7152b-135">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="7152b-136">Ha a rendszer kéri, hogy válassza a munkahelyi vagy **iskolai fiók** vagy a **személyes fiók** lehetőséget, válassza a **munkahelyi vagy iskolai fiók** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7152b-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="7152b-137">Kattintson a fogaskerék ikonra a **Beállítások** menü megnyitásához, majd válassza a **Fiókbeállítások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7152b-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="7152b-138">A **Fiókbeállítások** menüben válassza a **kifizetés és az adó** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7152b-138">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="7152b-139">Kifizetési és adózási profilok társítása az egyes programokhoz</span><span class="sxs-lookup"><span data-stu-id="7152b-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="7152b-140">Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard/), majd kattintson a fogaskerék ikonra a **Beállítások** menü megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="7152b-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="7152b-141">Válassza ki a **Fiókbeállítások** lehetőséget, bontsa ki a **kifizetés és adó szakaszt**, majd válassza a **kifizetés és az adó profil hozzárendelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7152b-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="7152b-142">Ekkor megjelenik a programok listája.</span><span class="sxs-lookup"><span data-stu-id="7152b-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="7152b-143">A profil részleteinek megtekintéséhez kattintson a program melletti nyílra.</span><span class="sxs-lookup"><span data-stu-id="7152b-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="7152b-144">Az **adó-profil** legördülő menüben válassza ki a kívánt adózási profilt, vagy válassza az új profil létrehozása lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7152b-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="7152b-145">Ha új profil létrehozását választja, akkor a megfelelő módon lesz átirányítva.</span><span class="sxs-lookup"><span data-stu-id="7152b-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="7152b-146">Válassza a Folytatás lehetőséget az előugró ablakban.</span><span class="sxs-lookup"><span data-stu-id="7152b-146">Select Continue in the pop-up window.</span></span> <span data-ttu-id="7152b-147">Az új adózási profil létrehozásának folyamata alább látható.</span><span class="sxs-lookup"><span data-stu-id="7152b-147">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="7152b-148">Válassza a **fizetési mód** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7152b-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="7152b-149">Ha az **elektronikus banki átutalást** fizetési módként választotta, válassza ki a kívánt fizetési profilt, vagy válassza az új profil létrehozása lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7152b-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="7152b-150">Ha új profil létrehozását választja, akkor a megfelelő módon lesz átirányítva.</span><span class="sxs-lookup"><span data-stu-id="7152b-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="7152b-151">Válassza a Folytatás lehetőséget az előugró ablakban.</span><span class="sxs-lookup"><span data-stu-id="7152b-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="7152b-152">Az új fizetési profil létrehozásának folyamata alább látható.</span><span class="sxs-lookup"><span data-stu-id="7152b-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="7152b-153">Ha a fizetési mód mezőben a **jóváírási Megjegyzés** lehetőséget választotta, akkor végezze el az ellenőrzést.</span><span class="sxs-lookup"><span data-stu-id="7152b-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="7152b-154">Ezzel megerősíti, hogy a hivatkozott SAP-szám a szervezethez tartozik.</span><span class="sxs-lookup"><span data-stu-id="7152b-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="7152b-155">Ha több Microsoft üzleti entitás van felsorolva, ki kell választania egy fizetési profilt az egyes entitásokhoz.</span><span class="sxs-lookup"><span data-stu-id="7152b-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="7152b-156">A fizetési mód rendelkezésre állása az ösztönző program szabályaitól függ.</span><span class="sxs-lookup"><span data-stu-id="7152b-156">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="7152b-157">Válassza ki a **pénznemet**.</span><span class="sxs-lookup"><span data-stu-id="7152b-157">Select the **Currency**.</span></span>

6. <span data-ttu-id="7152b-158">Az összes fizetési mező kitöltése után válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7152b-158">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="7152b-159">A bank profiljának létrehozása</span><span class="sxs-lookup"><span data-stu-id="7152b-159">Create your bank profile</span></span>

<span data-ttu-id="7152b-160">A banki profilok szervezeti szinten jönnek létre.</span><span class="sxs-lookup"><span data-stu-id="7152b-160">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="7152b-161">Ez lehetővé teszi, hogy az egyik bank profilja több MPN-azonosító és egy szervezeten belüli ösztönző program között legyen hozzárendelve.</span><span class="sxs-lookup"><span data-stu-id="7152b-161">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="7152b-162">A banki profil különböző országokban való alkalmazása kivételeket okozhat, mivel a különböző banki és adózási szabályok érvényesek.</span><span class="sxs-lookup"><span data-stu-id="7152b-162">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="7152b-163">A következő lapokon csillaggal rendelkező mezőket kell megadni.</span><span class="sxs-lookup"><span data-stu-id="7152b-163">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="7152b-164">Ha nem tudja, mi a mező, válassza ki az információs ikont.</span><span class="sxs-lookup"><span data-stu-id="7152b-164">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="7152b-165">A **részletek** lapon végezze el a következő mezőket: **profilnév:** adjon meg egy egyedi nevet a fizetési profil azonosításához.</span><span class="sxs-lookup"><span data-stu-id="7152b-165">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="7152b-166">**Bankszámla helye:** Az ország, amelyben a vállalat bankja található.</span><span class="sxs-lookup"><span data-stu-id="7152b-166">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="7152b-167">**Fizetési mód:** A partner központ előnyben részesített fizetési módja az elektronikus banki átutalás.</span><span class="sxs-lookup"><span data-stu-id="7152b-167">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="7152b-168">Kattintson a **Tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="7152b-168">Select **Next**.</span></span>

3. <span data-ttu-id="7152b-169">A **Bankszámla** lapon adja meg az adatait.</span><span class="sxs-lookup"><span data-stu-id="7152b-169">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="7152b-170">Az ezen az oldalon látható mezők országonként eltérőek lesznek.</span><span class="sxs-lookup"><span data-stu-id="7152b-170">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="7152b-171">Kattintson a **Tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="7152b-171">Select **Next**.</span></span>

5. <span data-ttu-id="7152b-172">A **kedvezményezett** lapon adja meg a megfelelő adatokat.</span><span class="sxs-lookup"><span data-stu-id="7152b-172">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="7152b-173">A kedvezményezett az a személy, aki a vállalatnál kapcsolatba fog lépni, ha meg kell vitatnia a fiókját.</span><span class="sxs-lookup"><span data-stu-id="7152b-173">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="7152b-174">Ha a mezők befejeződik, válassza a **Befejezés** lehetőséget, majd válassza a **jóváhagyás** lehetőséget a banki profil létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="7152b-174">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="7152b-175">A rendszer átirányítja a **kifizetési és adózási profilok** lapra.</span><span class="sxs-lookup"><span data-stu-id="7152b-175">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="7152b-176">Az új profil állapota a **Microsoft-ellenőrzés függőben** állapotba kerül, amíg az ellenőrzés be nem fejeződik.</span><span class="sxs-lookup"><span data-stu-id="7152b-176">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="7152b-177">Ez a folyamat akár 48 órát is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="7152b-177">This process may take up to 48 hours.</span></span> <span data-ttu-id="7152b-178">Az érvényesítés befejezését követően a profil állapota vagy **jóváhagyása** vagy a **szükséges művelet** látható lesz.</span><span class="sxs-lookup"><span data-stu-id="7152b-178">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="7152b-179">Ha **beavatkozás szükséges**, ismételje meg a fenti lépéseket a szükséges információk megadásakor.</span><span class="sxs-lookup"><span data-stu-id="7152b-179">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="7152b-180">Az adózási profil létrehozása</span><span class="sxs-lookup"><span data-stu-id="7152b-180">Create your tax profile</span></span>

<span data-ttu-id="7152b-181">A következő eljárással biztosíthatja a Microsoft számára a szervezete számára szükséges adózási adatokat.</span><span class="sxs-lookup"><span data-stu-id="7152b-181">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="7152b-182">Az ebben a szakaszban szereplő lapok dinamikusak, és az adott országtól vagy régiótól függően változnak.</span><span class="sxs-lookup"><span data-stu-id="7152b-182">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="7152b-183">Ha segítségre van szüksége a helyes adózási információk azonosításához, lépjen kapcsolatba az országa megfelelő kormányzati forrásaival.</span><span class="sxs-lookup"><span data-stu-id="7152b-183">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="7152b-184">Abban az esetben, ha a W8 vagy a W9 űrlap kitöltéséhez szükséges információkra van szüksége a partner vállalatok számára, a következő címek az IRS webhelyre kerülnek:</span><span class="sxs-lookup"><span data-stu-id="7152b-184">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="7152b-185">Csak a vállalat adatait adja meg.</span><span class="sxs-lookup"><span data-stu-id="7152b-185">Enter only details for your company.</span></span> <span data-ttu-id="7152b-186">Soha ne adjon meg személyes adatokat.</span><span class="sxs-lookup"><span data-stu-id="7152b-186">Never enter personal details.</span></span>

1. <span data-ttu-id="7152b-187">Az **üzleti profil** lapon végezze el a szükséges mezőket, majd kattintson a **tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="7152b-187">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="7152b-188">A **telepítés** lapon válassza ki a vállalatára vonatkozó beállítást.</span><span class="sxs-lookup"><span data-stu-id="7152b-188">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="7152b-189">Válassza ki a bal oldali lehetőséget, ha a vállalata csak a Egyesült Államokban van beépítve, vagy ha ez a profil egyedi.</span><span class="sxs-lookup"><span data-stu-id="7152b-189">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="7152b-190">Ha a vállalat a Egyesült Államokon kívül van beépítve, válassza a jobb oldali lehetőséget, majd válassza ki az országot/régiót a listából.</span><span class="sxs-lookup"><span data-stu-id="7152b-190">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="7152b-191">Kattintson a **Tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="7152b-191">Select **Next**.</span></span> 

4. <span data-ttu-id="7152b-192">Az **adó állapota** lapon adja meg a szükséges adatokat, majd kattintson a **tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="7152b-192">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="7152b-193">Az ezen a lapon lévő mezők országonként eltérőek lesznek.</span><span class="sxs-lookup"><span data-stu-id="7152b-193">Fields on this page will vary by country.</span></span> <span data-ttu-id="7152b-194">a részleteket.</span><span class="sxs-lookup"><span data-stu-id="7152b-194">your details.</span></span> 

5. <span data-ttu-id="7152b-195">A **További dokumentáció** lapon a kötelező mezők és a **tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="7152b-195">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="7152b-196">Válassza a **Tallózás** lehetőséget az országa vagy régiója számára szükséges dokumentumok feltöltéséhez.</span><span class="sxs-lookup"><span data-stu-id="7152b-196">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="7152b-197">Ha megjelenik a dokumentum neve, válassza a **feltöltés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7152b-197">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="7152b-198">Ha el kell távolítania a dokumentumot, válassza az **Eltávolítás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7152b-198">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="7152b-199">A mentéshez és a folytatáshoz kattintson a **Befejezés** gombra.</span><span class="sxs-lookup"><span data-stu-id="7152b-199">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="7152b-200">Válassza az előugró üzenet **megerősítés** elemét.</span><span class="sxs-lookup"><span data-stu-id="7152b-200">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="7152b-201">Visszakerül a **kifizetés és az adó beállítása** lapra.</span><span class="sxs-lookup"><span data-stu-id="7152b-201">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7152b-202">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="7152b-202">Next steps</span></span>

- [<span data-ttu-id="7152b-203">A kifizetésekkel és az adókkal kapcsolatos gyakori kérdések</span><span class="sxs-lookup"><span data-stu-id="7152b-203">Common questions about payouts and taxes</span></span>](payout-faq.md)
