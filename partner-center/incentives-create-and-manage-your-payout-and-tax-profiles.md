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
ms.openlocfilehash: 1e97e2e9db798e5ef90858cf96dc06602bbfe427
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492466"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="d675d-104">Ösztönzők létrehozása és kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="d675d-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="d675d-105">**A következőkre vonatkozik:**</span><span class="sxs-lookup"><span data-stu-id="d675d-105">**Applies to:**</span></span>

- <span data-ttu-id="d675d-106">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="d675d-106">Partner Center</span></span>

<span data-ttu-id="d675d-107">**Megfelelő szerepkörök:**</span><span class="sxs-lookup"><span data-stu-id="d675d-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="d675d-108">Ösztönzők rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="d675d-108">Incentives admin</span></span>
- <span data-ttu-id="d675d-109">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="d675d-109">Account admin</span></span>
- <span data-ttu-id="d675d-110">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="d675d-110">Global admin</span></span>

<span data-ttu-id="d675d-111">Ahhoz, hogy megkaphassa az egy adott MPN-helyhez tartozó ösztönzőprogramok kifizetését, be kell fejeznie a regisztrációt úgy, hogy a programhoz és az MPN-helyhez egy érvényes kifizetési és adóprofilt társít.</span><span class="sxs-lookup"><span data-stu-id="d675d-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="d675d-112">A Microsoft ezt a kifizetési és adóprofilt a kifizetésekhez fogja használni.</span><span class="sxs-lookup"><span data-stu-id="d675d-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="d675d-113">Az ösztönzőprogram szabályaitól függően lehetséges elektronikus banki átutalás vagy jóváírási értesítés használata is a kifizetéshez.</span><span class="sxs-lookup"><span data-stu-id="d675d-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="d675d-114">Szerepkörök, pénznemek és egyéb Microsoft-programok</span><span class="sxs-lookup"><span data-stu-id="d675d-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="d675d-115">Fontos megérteni az alábbi információkat, mielőtt megkezdi a befizetést és az adózási profilt.</span><span class="sxs-lookup"><span data-stu-id="d675d-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="d675d-116">Szerepkörök és engedélyek</span><span class="sxs-lookup"><span data-stu-id="d675d-116">Roles and permissions</span></span>

<span data-ttu-id="d675d-117">Az ösztönző befizetések esetén a banki és adózási információk megadásához ösztönző rendszergazdának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="d675d-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="d675d-118">Ha Ön MPN/fiók rendszergazdája, rendeljen hozzá önmagát és/vagy kollégáját, hogy az ösztönözze a rendszergazdát.</span><span class="sxs-lookup"><span data-stu-id="d675d-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="d675d-119">Ha ösztönző rendszergazdai jogosultságokat kell kérnie, forduljon az MPN-rendszergazdához vagy a globális rendszergazdához. A [partner Center irányítópultra](https://partner.microsoft.com/dashboard/)való bejelentkezéssel megállapíthatja, hogy kik a vállalatnál vannak ezek a szerepkörök.</span><span class="sxs-lookup"><span data-stu-id="d675d-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="d675d-120">Kattintson a jobb felső sarokban található **Beállítások** ikonra, válassza a **felhasználói kezelés** , majd a globális rendszergazda szűrése lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d675d-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="d675d-121">Ösztönzők a felhasználók megtekinthetik az ösztönző bevételeket és a fizetési adatokat és jelentéseket, de nem szerkeszthetik a bank és az adó adatait.</span><span class="sxs-lookup"><span data-stu-id="d675d-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="d675d-122">Válassza ki a kifizetés pénznemét</span><span class="sxs-lookup"><span data-stu-id="d675d-122">Choose your disbursement currency</span></span>

<span data-ttu-id="d675d-123">Az ösztönző kifizetések a fizetési profil beállításakor kiválasztott pénznemben történnek.</span><span class="sxs-lookup"><span data-stu-id="d675d-123">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="d675d-124">A fizetések kiszámítása a Microsoft által havonta beállított árfolyamon történik.</span><span class="sxs-lookup"><span data-stu-id="d675d-124">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="d675d-125">A kiválasztott pénznem miatt az érték változásaiért felelős lesz.</span><span class="sxs-lookup"><span data-stu-id="d675d-125">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="d675d-126">Különböző profilok használata különböző Microsoft-programokhoz</span><span class="sxs-lookup"><span data-stu-id="d675d-126">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="d675d-127">Ha a vállalata több ösztönző programban is regisztrálva van, használhatja ugyanazt a fizetési fiókot, vagy választhat, hogy különböző fizetési fiókokat szeretne használni a különböző programokhoz.</span><span class="sxs-lookup"><span data-stu-id="d675d-127">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="d675d-128">Kifizetési és adózási profilok létrehozása és kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="d675d-128">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="d675d-129">Az alábbi szakasz végigvezeti a fizetési és adózási profilok a partner Centerben való létrehozásának és kezelésének folyamatán.</span><span class="sxs-lookup"><span data-stu-id="d675d-129">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="d675d-130">A fizetési profilok a partner Centerben való létrehozásához és kezeléséhez ösztönző rendszergazdának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="d675d-130">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="d675d-131">Az ösztönző szerepköröket minden egyes, az egyes ösztönző programok alá tartozó MPN-helyhez hozzá kell rendelni.</span><span class="sxs-lookup"><span data-stu-id="d675d-131">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="d675d-132">Az ösztönző rendszergazdák a partner Centerben való hozzáadásával kapcsolatos további információkért lásd: [felhasználói fiókok létrehozása](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="d675d-132">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="d675d-133">A partner Center kifizetési és adózási szakaszának elérése</span><span class="sxs-lookup"><span data-stu-id="d675d-133">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="d675d-134">Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard/) a Azure Active Directory-(Azure ad-) fiókkal (vállalati fiókkal) vagy a megfelelő e-mail-címmel, ha az egyik hozzá lett rendelve.</span><span class="sxs-lookup"><span data-stu-id="d675d-134">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="d675d-135">Egy Azure AD-fiókban több tartomány is regisztrálható.</span><span class="sxs-lookup"><span data-stu-id="d675d-135">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="d675d-136">Forduljon a globális rendszergazdához, és állapítsa meg, hogy mely tartományok vannak társítva.</span><span class="sxs-lookup"><span data-stu-id="d675d-136">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="d675d-137">Ha csak a tartományba tud bejelentkezni @onmicrosoft.com , lépjen kapcsolatba a fiók rendszergazdájával, és adjon hozzá további tartományokat az Azure ad-fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="d675d-137">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="d675d-138">Ha a rendszer kéri, hogy válassza a munkahelyi vagy **iskolai fiók** vagy a **személyes fiók** lehetőséget, válassza a **munkahelyi vagy iskolai fiók** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d675d-138">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="d675d-139">Kattintson a fogaskerék ikonra a **Beállítások** menü megnyitásához, majd válassza a **partner beállításai** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d675d-139">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="d675d-140">A **Fiókbeállítások** menüben válassza a **kifizetés és az adó** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d675d-140">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="d675d-141">Kifizetési és adózási profilok társítása az egyes programokhoz</span><span class="sxs-lookup"><span data-stu-id="d675d-141">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="d675d-142">Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard/), majd kattintson a fogaskerék ikonra a **Beállítások** menü megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="d675d-142">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="d675d-143">Válassza ki a **partner beállításait**, bontsa ki a **kifizetés és adó szakaszt**, majd válassza a **kifizetés és az adó profil hozzárendelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d675d-143">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="d675d-144">Ekkor megjelenik a programok listája.</span><span class="sxs-lookup"><span data-stu-id="d675d-144">A list of your programs will be displayed.</span></span> <span data-ttu-id="d675d-145">A profil részleteinek megtekintéséhez kattintson a program melletti nyílra.</span><span class="sxs-lookup"><span data-stu-id="d675d-145">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="d675d-146">Az **adó-profil** legördülő menüben válassza ki a kívánt adózási profilt, vagy válassza az új profil létrehozása lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d675d-146">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="d675d-147">Ha új profil létrehozását választja, akkor a megfelelő módon lesz átirányítva.</span><span class="sxs-lookup"><span data-stu-id="d675d-147">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="d675d-148">Válassza a Folytatás lehetőséget az előugró ablakban.</span><span class="sxs-lookup"><span data-stu-id="d675d-148">Select Continue in the pop-up window.</span></span> <span data-ttu-id="d675d-149">Az új adózási profil létrehozásának folyamata alább látható.</span><span class="sxs-lookup"><span data-stu-id="d675d-149">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="d675d-150">Válassza a **fizetési mód** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d675d-150">Select **Payment method**.</span></span>

   - <span data-ttu-id="d675d-151">Ha az **elektronikus banki átutalást** fizetési módként választotta, válassza ki a kívánt fizetési profilt, vagy válassza az új profil létrehozása lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d675d-151">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="d675d-152">Ha új profil létrehozását választja, akkor a megfelelő módon lesz átirányítva.</span><span class="sxs-lookup"><span data-stu-id="d675d-152">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="d675d-153">Válassza a Folytatás lehetőséget az előugró ablakban.</span><span class="sxs-lookup"><span data-stu-id="d675d-153">Select Continue in the pop-up window.</span></span> <span data-ttu-id="d675d-154">Az új fizetési profil létrehozásának folyamata alább látható.</span><span class="sxs-lookup"><span data-stu-id="d675d-154">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="d675d-155">Ha a fizetési mód mezőben a **jóváírási Megjegyzés** lehetőséget választotta, akkor végezze el az ellenőrzést.</span><span class="sxs-lookup"><span data-stu-id="d675d-155">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="d675d-156">Ezzel megerősíti, hogy a hivatkozott SAP-szám a szervezethez tartozik.</span><span class="sxs-lookup"><span data-stu-id="d675d-156">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="d675d-157">Ha több Microsoft üzleti entitás van felsorolva, ki kell választania egy fizetési profilt az egyes entitásokhoz.</span><span class="sxs-lookup"><span data-stu-id="d675d-157">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="d675d-158">A fizetési mód rendelkezésre állása az ösztönző program szabályaitól függ.</span><span class="sxs-lookup"><span data-stu-id="d675d-158">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="d675d-159">Válassza ki a **pénznemet**.</span><span class="sxs-lookup"><span data-stu-id="d675d-159">Select the **Currency**.</span></span>

6. <span data-ttu-id="d675d-160">Az összes fizetési mező kitöltése után válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d675d-160">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="d675d-161">A bank profiljának létrehozása</span><span class="sxs-lookup"><span data-stu-id="d675d-161">Create your bank profile</span></span>

<span data-ttu-id="d675d-162">A banki profilok szervezeti szinten jönnek létre.</span><span class="sxs-lookup"><span data-stu-id="d675d-162">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="d675d-163">Ez lehetővé teszi, hogy az egyik bank profilja több MPN-azonosító és egy szervezeten belüli ösztönző program között legyen hozzárendelve.</span><span class="sxs-lookup"><span data-stu-id="d675d-163">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="d675d-164">A banki profil különböző országokban való alkalmazása kivételeket okozhat, mivel a különböző banki és adózási szabályok érvényesek.</span><span class="sxs-lookup"><span data-stu-id="d675d-164">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="d675d-165">A következő lapokon csillaggal rendelkező mezőket kell megadni.</span><span class="sxs-lookup"><span data-stu-id="d675d-165">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="d675d-166">Ha nem tudja, mi a mező, válassza ki az információs ikont.</span><span class="sxs-lookup"><span data-stu-id="d675d-166">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="d675d-167">A **részletek** lapon végezze el a következő mezőket: **profilnév:** adjon meg egy egyedi nevet a fizetési profil azonosításához.</span><span class="sxs-lookup"><span data-stu-id="d675d-167">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="d675d-168">**Bankszámla helye:** Az ország, amelyben a vállalat bankja található.</span><span class="sxs-lookup"><span data-stu-id="d675d-168">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="d675d-169">**Fizetési mód:** A partner központ előnyben részesített fizetési módja az elektronikus banki átutalás.</span><span class="sxs-lookup"><span data-stu-id="d675d-169">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="d675d-170">Kattintson a **Tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="d675d-170">Select **Next**.</span></span>

3. <span data-ttu-id="d675d-171">A **Bankszámla** lapon adja meg az adatait.</span><span class="sxs-lookup"><span data-stu-id="d675d-171">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="d675d-172">Az ezen az oldalon látható mezők országonként eltérőek lesznek.</span><span class="sxs-lookup"><span data-stu-id="d675d-172">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="d675d-173">Kattintson a **Tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="d675d-173">Select **Next**.</span></span>

5. <span data-ttu-id="d675d-174">A **kedvezményezett** lapon adja meg a megfelelő adatokat.</span><span class="sxs-lookup"><span data-stu-id="d675d-174">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="d675d-175">A kedvezményezett az a személy, aki a vállalatnál kapcsolatba fog lépni, ha meg kell vitatnia a fiókját.</span><span class="sxs-lookup"><span data-stu-id="d675d-175">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="d675d-176">Ha a mezők befejeződik, válassza a **Befejezés** lehetőséget, majd válassza a **jóváhagyás** lehetőséget a banki profil létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="d675d-176">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="d675d-177">A rendszer átirányítja a **kifizetési és adózási profilok** lapra.</span><span class="sxs-lookup"><span data-stu-id="d675d-177">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="d675d-178">Az új profil állapota a **Microsoft-ellenőrzés függőben** állapotba kerül, amíg az ellenőrzés be nem fejeződik.</span><span class="sxs-lookup"><span data-stu-id="d675d-178">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="d675d-179">Ez a folyamat akár 48 órát is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="d675d-179">This process may take up to 48 hours.</span></span> <span data-ttu-id="d675d-180">Az érvényesítés befejezését követően a profil állapota vagy **jóváhagyása** vagy a **szükséges művelet** látható lesz.</span><span class="sxs-lookup"><span data-stu-id="d675d-180">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="d675d-181">Ha **beavatkozás szükséges**, ismételje meg a fenti lépéseket a szükséges információk megadásakor.</span><span class="sxs-lookup"><span data-stu-id="d675d-181">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="d675d-182">Az adózási profil létrehozása</span><span class="sxs-lookup"><span data-stu-id="d675d-182">Create your tax profile</span></span>

<span data-ttu-id="d675d-183">A következő eljárással biztosíthatja a Microsoft számára a szervezete számára szükséges adózási adatokat.</span><span class="sxs-lookup"><span data-stu-id="d675d-183">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="d675d-184">Az ebben a szakaszban szereplő lapok dinamikusak, és az adott országtól vagy régiótól függően változnak.</span><span class="sxs-lookup"><span data-stu-id="d675d-184">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="d675d-185">Ha segítségre van szüksége a helyes adózási információk azonosításához, lépjen kapcsolatba az országa megfelelő kormányzati forrásaival.</span><span class="sxs-lookup"><span data-stu-id="d675d-185">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="d675d-186">Abban az esetben, ha a W8 vagy a W9 űrlap kitöltéséhez szükséges információkra van szüksége a partner vállalatok számára, a következő címek az IRS webhelyre kerülnek:</span><span class="sxs-lookup"><span data-stu-id="d675d-186">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="d675d-187">Csak a vállalat adatait adja meg.</span><span class="sxs-lookup"><span data-stu-id="d675d-187">Enter only details for your company.</span></span> <span data-ttu-id="d675d-188">Soha ne adjon meg személyes adatokat.</span><span class="sxs-lookup"><span data-stu-id="d675d-188">Never enter personal details.</span></span>

1. <span data-ttu-id="d675d-189">Az **üzleti profil** lapon végezze el a szükséges mezőket, majd kattintson a **tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="d675d-189">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="d675d-190">A **telepítés** lapon válassza ki a vállalatára vonatkozó beállítást.</span><span class="sxs-lookup"><span data-stu-id="d675d-190">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="d675d-191">Válassza ki a bal oldali lehetőséget, ha a vállalata csak a Egyesült Államokban van beépítve, vagy ha ez a profil egyedi.</span><span class="sxs-lookup"><span data-stu-id="d675d-191">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="d675d-192">Ha a vállalat a Egyesült Államokon kívül van beépítve, válassza a jobb oldali lehetőséget, majd válassza ki az országot/régiót a listából.</span><span class="sxs-lookup"><span data-stu-id="d675d-192">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="d675d-193">Kattintson a **Tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="d675d-193">Select **Next**.</span></span> 

4. <span data-ttu-id="d675d-194">Az **adó állapota** lapon adja meg a szükséges adatokat, majd kattintson a **tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="d675d-194">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="d675d-195">Az ezen a lapon lévő mezők országonként eltérőek lesznek.</span><span class="sxs-lookup"><span data-stu-id="d675d-195">Fields on this page will vary by country.</span></span> <span data-ttu-id="d675d-196">a részleteket.</span><span class="sxs-lookup"><span data-stu-id="d675d-196">your details.</span></span> 

5. <span data-ttu-id="d675d-197">A **További dokumentáció** lapon a kötelező mezők és a **tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="d675d-197">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="d675d-198">Válassza a **Tallózás** lehetőséget az országa vagy régiója számára szükséges dokumentumok feltöltéséhez.</span><span class="sxs-lookup"><span data-stu-id="d675d-198">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="d675d-199">Ha megjelenik a dokumentum neve, válassza a **feltöltés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d675d-199">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="d675d-200">Ha el kell távolítania a dokumentumot, válassza az **Eltávolítás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d675d-200">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="d675d-201">A mentéshez és a folytatáshoz kattintson a **Befejezés** gombra.</span><span class="sxs-lookup"><span data-stu-id="d675d-201">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="d675d-202">Válassza az előugró üzenet **megerősítés** elemét.</span><span class="sxs-lookup"><span data-stu-id="d675d-202">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="d675d-203">Visszakerül a **kifizetés és az adó beállítása** lapra.</span><span class="sxs-lookup"><span data-stu-id="d675d-203">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d675d-204">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="d675d-204">Next steps</span></span>

- [<span data-ttu-id="d675d-205">A kifizetésekkel és az adókkal kapcsolatos gyakori kérdések</span><span class="sxs-lookup"><span data-stu-id="d675d-205">Common questions about payouts and taxes</span></span>](payout-faq.md)
