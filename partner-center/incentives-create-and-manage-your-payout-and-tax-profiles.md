---
title: Kifizetések és adóprofilok a Partnerközpontban
ms.topic: how-to
ms.date: 09/11/2020
description: Létrehozhatja és kezelheti a kifizetési és az adózási profilt, így Ön fizethet az ösztönzőkért. Ide tartozik a különböző profilok létrehozása, kezelése és használata.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ca2ffe992ff92b98546934f4a249779f39179acb
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530601"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="2ea92-104">Ösztönzők létrehozása és kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="2ea92-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="2ea92-105">**A következőkre vonatkozik:**</span><span class="sxs-lookup"><span data-stu-id="2ea92-105">**Applies to:**</span></span>

- <span data-ttu-id="2ea92-106">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="2ea92-106">Partner Center</span></span>

<span data-ttu-id="2ea92-107">**Megfelelő szerepkörök:**</span><span class="sxs-lookup"><span data-stu-id="2ea92-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="2ea92-108">Ösztönzők rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="2ea92-108">Incentives admin</span></span>
- <span data-ttu-id="2ea92-109">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="2ea92-109">Billing admin</span></span>
- <span data-ttu-id="2ea92-110">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="2ea92-110">Global admin</span></span>

<span data-ttu-id="2ea92-111">Ahhoz, hogy megkaphassa az egy adott MPN-helyhez tartozó ösztönzőprogramok kifizetését, be kell fejeznie a regisztrációt úgy, hogy a programhoz és az MPN-helyhez egy érvényes kifizetési és adóprofilt társít.</span><span class="sxs-lookup"><span data-stu-id="2ea92-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="2ea92-112">A Microsoft ezt a kifizetési és adóprofilt a kifizetésekhez fogja használni.</span><span class="sxs-lookup"><span data-stu-id="2ea92-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="2ea92-113">Az ösztönzőprogram szabályaitól függően lehetséges elektronikus banki átutalás vagy jóváírási értesítés használata is a kifizetéshez.</span><span class="sxs-lookup"><span data-stu-id="2ea92-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="2ea92-114">Szerepkörök, pénznemek és egyéb Microsoft-programok</span><span class="sxs-lookup"><span data-stu-id="2ea92-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="2ea92-115">Fontos megérteni az alábbi információkat, mielőtt megkezdi a befizetést és az adózási profilt.</span><span class="sxs-lookup"><span data-stu-id="2ea92-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="2ea92-116">Szerepkörök és engedélyek</span><span class="sxs-lookup"><span data-stu-id="2ea92-116">Roles and permissions</span></span>

<span data-ttu-id="2ea92-117">Az ösztönző befizetések esetén a banki és adózási információk megadásához ösztönző rendszergazdának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="2ea92-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="2ea92-118">Ha Ön MPN/fiók rendszergazdája, rendeljen hozzá önmagát és/vagy kollégáját, hogy az ösztönözze a rendszergazdát.</span><span class="sxs-lookup"><span data-stu-id="2ea92-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="2ea92-119">Ha ösztönző rendszergazdai jogosultságokat kell kérnie, forduljon az MPN-rendszergazdához vagy a globális rendszergazdához. A [partner Center irányítópultra](https://partner.microsoft.com/dashboard/)való bejelentkezéssel megállapíthatja, hogy kik a vállalatnál vannak ezek a szerepkörök.</span><span class="sxs-lookup"><span data-stu-id="2ea92-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="2ea92-120">Kattintson a jobb felső sarokban található **Beállítások** ikonra, válassza a **felhasználói kezelés** , majd a globális rendszergazda szűrése lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2ea92-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="2ea92-121">Ösztönzők a felhasználók megtekinthetik az ösztönző bevételeket és a fizetési adatokat és jelentéseket, de nem szerkeszthetik a bank és az adó adatait.</span><span class="sxs-lookup"><span data-stu-id="2ea92-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="2ea92-122">Válassza ki a kifizetés pénznemét</span><span class="sxs-lookup"><span data-stu-id="2ea92-122">Choose your disbursement currency</span></span>

<span data-ttu-id="2ea92-123">Alapértelmezés szerint az ösztönzők a megfelelő entitások helyi pénznemében történnek.</span><span class="sxs-lookup"><span data-stu-id="2ea92-123">By default, incentives payments are made in the local currency of each respective entity.</span></span> <span data-ttu-id="2ea92-124">A profil beállítása során más pénznemet is megadhat.</span><span class="sxs-lookup"><span data-stu-id="2ea92-124">You can specify a different currency during profile setup.</span></span> <span data-ttu-id="2ea92-125">A fizetések kiszámítása a Microsoft által havonta beállított árfolyamon történik.</span><span class="sxs-lookup"><span data-stu-id="2ea92-125">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="2ea92-126">A kiválasztott pénznem miatt az érték változásaiért felelős lesz.</span><span class="sxs-lookup"><span data-stu-id="2ea92-126">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="bank-and-tax-information-and-other-programs"></a><span data-ttu-id="2ea92-127">Banki és adózási információk és egyéb programok</span><span class="sxs-lookup"><span data-stu-id="2ea92-127">Bank and tax information and other programs</span></span>

<span data-ttu-id="2ea92-128">Adja meg az alább ismertetett információkat, még akkor is, ha a Microsoft már használja a banki adatokat a kifizetésekhez.</span><span class="sxs-lookup"><span data-stu-id="2ea92-128">Provide the information described below even if Microsoft already uses your bank data for payments.</span></span> <span data-ttu-id="2ea92-129">Így biztosíthatja a vállalati adatok védelmét és védelmét, mivel a profilt az új eszközre történő másolásával bizalmas adatokat tehet elérhetővé.</span><span class="sxs-lookup"><span data-stu-id="2ea92-129">This helps ensure the privacy and security of your company’s data, since copying your profile to the new tool could expose sensitive information.</span></span> <span data-ttu-id="2ea92-130">Ez a folyamat továbbra is jó lehetőség arra, hogy az adatfeldolgozás teljes és pontos legyen.</span><span class="sxs-lookup"><span data-stu-id="2ea92-130">Going through this process is also a good opportunity to ensure the data is complete and accurate.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="2ea92-131">Különböző profilok használata különböző Microsoft-programokhoz</span><span class="sxs-lookup"><span data-stu-id="2ea92-131">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="2ea92-132">A kiskereskedelmi forgalomban az öt kiskereskedelmi ösztönző programhoz tartozó kifizetések ugyanarra a bankszámlára léphetnek.</span><span class="sxs-lookup"><span data-stu-id="2ea92-132">Within retail, payments for each of the five retail incentive programs can go to the same bank account.</span></span> <span data-ttu-id="2ea92-133">Azt is megteheti, hogy a kiskereskedelmi Xbox-fizetések bekerülnek egy bankszámlára, míg a kiskereskedelmi iroda egy másik bankszámlájára van kifizetve.</span><span class="sxs-lookup"><span data-stu-id="2ea92-133">Alternatively, you can choose to have Retail Xbox payments go into one bank account while Retail Office is paid to a different bank account.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="2ea92-134">Kifizetési és adózási profilok létrehozása és kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="2ea92-134">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="2ea92-135">Az alábbi szakasz végigvezeti a fizetési és adózási profilok a partner Centerben való létrehozásának és kezelésének folyamatán.</span><span class="sxs-lookup"><span data-stu-id="2ea92-135">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="2ea92-136">A fizetési profilok a partner Centerben való létrehozásához és kezeléséhez ösztönző rendszergazdának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="2ea92-136">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="2ea92-137">Az ösztönző szerepköröket minden egyes, az egyes ösztönző programok alá tartozó MPN-helyhez hozzá kell rendelni.</span><span class="sxs-lookup"><span data-stu-id="2ea92-137">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="2ea92-138">Az ösztönző rendszergazdák a partner Centerben való hozzáadásával kapcsolatos további információkért lásd: [felhasználói fiókok létrehozása](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="2ea92-138">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="2ea92-139">A partner Center kifizetési és adózási szakaszának elérése</span><span class="sxs-lookup"><span data-stu-id="2ea92-139">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="2ea92-140">Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard/) a Azure Active Directory-(Azure ad-) fiókkal (vállalati fiókkal) vagy a megfelelő e-mail-címmel, ha az egyik hozzá lett rendelve.</span><span class="sxs-lookup"><span data-stu-id="2ea92-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="2ea92-141">Egy Azure AD-fiókban több tartomány is regisztrálható.</span><span class="sxs-lookup"><span data-stu-id="2ea92-141">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="2ea92-142">Forduljon a globális rendszergazdához, és állapítsa meg, hogy mely tartományok vannak társítva.</span><span class="sxs-lookup"><span data-stu-id="2ea92-142">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="2ea92-143">Ha csak a tartományba tud bejelentkezni @onmicrosoft.com , lépjen kapcsolatba a fiók rendszergazdájával, és adjon hozzá további tartományokat az Azure ad-fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="2ea92-143">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="2ea92-144">Ha a rendszer kéri, hogy válassza a munkahelyi vagy **iskolai fiók** vagy a **személyes fiók** lehetőséget, válassza a **munkahelyi vagy iskolai fiók** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2ea92-144">If you're prompted to select **Work or school account** or **Personal Account** , select **Work or school account** .</span></span>

2. <span data-ttu-id="2ea92-145">Kattintson a fogaskerék ikonra a **Beállítások** menü megnyitásához, majd válassza a **partner beállításai** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2ea92-145">Select the gear icon to open the **Settings** menu, and then select **Partner settings** .</span></span>

3. <span data-ttu-id="2ea92-146">A **Fiókbeállítások** menüben válassza a **kifizetés és az adó** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2ea92-146">In the **Account settings** menu, select **Payout and tax** .</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="2ea92-147">Kifizetési és adózási profilok társítása az egyes programokhoz</span><span class="sxs-lookup"><span data-stu-id="2ea92-147">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="2ea92-148">Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard/), majd kattintson a fogaskerék ikonra a **Beállítások** menü megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="2ea92-148">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="2ea92-149">Válassza ki a **partner beállításait** , bontsa ki a **kifizetés és adó szakaszt** , majd válassza a **kifizetés és az adó profil hozzárendelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2ea92-149">Select **Partner settings** , expand the **Payout and tax section** , and then select **Payout and tax profile assignment** .</span></span> 
   
   <span data-ttu-id="2ea92-150">Ekkor megjelenik a programok listája.</span><span class="sxs-lookup"><span data-stu-id="2ea92-150">A list of your programs will be displayed.</span></span> <span data-ttu-id="2ea92-151">A profil részleteinek megtekintéséhez kattintson a program melletti nyílra.</span><span class="sxs-lookup"><span data-stu-id="2ea92-151">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="2ea92-152">Az **adó-profil** legördülő menüben válassza ki a kívánt adózási profilt, vagy válassza az új profil létrehozása lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2ea92-152">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="2ea92-153">Ha új profil létrehozását választja, akkor a megfelelő módon lesz átirányítva.</span><span class="sxs-lookup"><span data-stu-id="2ea92-153">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="2ea92-154">Válassza a Folytatás lehetőséget az előugró ablakban.</span><span class="sxs-lookup"><span data-stu-id="2ea92-154">Select Continue in the pop-up window.</span></span> <span data-ttu-id="2ea92-155">Az új adózási profil létrehozásának folyamata alább látható.</span><span class="sxs-lookup"><span data-stu-id="2ea92-155">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="2ea92-156">Válassza a **fizetési mód** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2ea92-156">Select **Payment method** .</span></span>

   - <span data-ttu-id="2ea92-157">Ha az **elektronikus banki átutalást** fizetési módként választotta, válassza ki a kívánt fizetési profilt, vagy válassza az új profil létrehozása lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2ea92-157">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="2ea92-158">Ha új profil létrehozását választja, akkor a megfelelő módon lesz átirányítva.</span><span class="sxs-lookup"><span data-stu-id="2ea92-158">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="2ea92-159">Válassza a Folytatás lehetőséget az előugró ablakban.</span><span class="sxs-lookup"><span data-stu-id="2ea92-159">Select Continue in the pop-up window.</span></span> <span data-ttu-id="2ea92-160">Az új fizetési profil létrehozásának folyamata alább látható.</span><span class="sxs-lookup"><span data-stu-id="2ea92-160">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="2ea92-161">Ha a fizetési mód mezőben a **jóváírási Megjegyzés** lehetőséget választotta, akkor végezze el az ellenőrzést.</span><span class="sxs-lookup"><span data-stu-id="2ea92-161">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="2ea92-162">Ezzel megerősíti, hogy a hivatkozott SAP-szám a szervezethez tartozik.</span><span class="sxs-lookup"><span data-stu-id="2ea92-162">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="2ea92-163">Ha több Microsoft üzleti entitás van felsorolva, ki kell választania egy fizetési profilt az egyes entitásokhoz.</span><span class="sxs-lookup"><span data-stu-id="2ea92-163">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="2ea92-164">A fizetési mód rendelkezésre állása az ösztönző program szabályaitól függ.</span><span class="sxs-lookup"><span data-stu-id="2ea92-164">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="2ea92-165">Válassza ki a **pénznemet** .</span><span class="sxs-lookup"><span data-stu-id="2ea92-165">Select the **Currency** .</span></span>

6. <span data-ttu-id="2ea92-166">Az összes fizetési mező kitöltése után válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2ea92-166">When you’ve completed all of the payment fields, select **Submit** .</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="2ea92-167">A bank profiljának létrehozása</span><span class="sxs-lookup"><span data-stu-id="2ea92-167">Create your bank profile</span></span>

<span data-ttu-id="2ea92-168">A banki profilok szervezeti szinten jönnek létre.</span><span class="sxs-lookup"><span data-stu-id="2ea92-168">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="2ea92-169">Ez lehetővé teszi, hogy az egyik bank profilja több MPN-azonosító és egy szervezeten belüli ösztönző program között legyen hozzárendelve.</span><span class="sxs-lookup"><span data-stu-id="2ea92-169">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="2ea92-170">A banki profil különböző országokban való alkalmazása kivételeket okozhat, mivel a különböző banki és adózási szabályok érvényesek.</span><span class="sxs-lookup"><span data-stu-id="2ea92-170">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="2ea92-171">A következő lapokon csillaggal rendelkező mezőket kell megadni.</span><span class="sxs-lookup"><span data-stu-id="2ea92-171">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="2ea92-172">Ha nem tudja, mi a mező, válassza ki az információs ikont.</span><span class="sxs-lookup"><span data-stu-id="2ea92-172">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="2ea92-173">A **részletek** lapon végezze el a következő mezőket: **profilnév:** adjon meg egy egyedi nevet a fizetési profil azonosításához.</span><span class="sxs-lookup"><span data-stu-id="2ea92-173">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="2ea92-174">**Bankszámla helye:** Az ország, amelyben a vállalat bankja található.</span><span class="sxs-lookup"><span data-stu-id="2ea92-174">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="2ea92-175">**Fizetési mód:** A partner központ előnyben részesített fizetési módja az elektronikus banki átutalás.</span><span class="sxs-lookup"><span data-stu-id="2ea92-175">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="2ea92-176">Kattintson a **Tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="2ea92-176">Select **Next** .</span></span>

3. <span data-ttu-id="2ea92-177">A **Bankszámla** lapon adja meg az adatait.</span><span class="sxs-lookup"><span data-stu-id="2ea92-177">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="2ea92-178">Az ezen az oldalon látható mezők országonként eltérőek lesznek.</span><span class="sxs-lookup"><span data-stu-id="2ea92-178">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="2ea92-179">Kattintson a **Tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="2ea92-179">Select **Next** .</span></span>

5. <span data-ttu-id="2ea92-180">A **kedvezményezett** lapon adja meg a megfelelő adatokat.</span><span class="sxs-lookup"><span data-stu-id="2ea92-180">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="2ea92-181">A kedvezményezett az a személy, aki a vállalatnál kapcsolatba fog lépni, ha meg kell vitatnia a fiókját.</span><span class="sxs-lookup"><span data-stu-id="2ea92-181">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="2ea92-182">Ha a mezők befejeződik, válassza a **Befejezés** lehetőséget, majd válassza a **jóváhagyás** lehetőséget a banki profil létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="2ea92-182">When the fields are completed, select **Finish** , and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="2ea92-183">A rendszer átirányítja a **kifizetési és adózási profilok** lapra.</span><span class="sxs-lookup"><span data-stu-id="2ea92-183">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="2ea92-184">Az új profil állapota a **Microsoft-ellenőrzés függőben** állapotba kerül, amíg az ellenőrzés be nem fejeződik.</span><span class="sxs-lookup"><span data-stu-id="2ea92-184">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="2ea92-185">Ez a folyamat akár 48 órát is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="2ea92-185">This process may take up to 48 hours.</span></span> <span data-ttu-id="2ea92-186">Az érvényesítés befejezését követően a profil állapota vagy **jóváhagyása** vagy a **szükséges művelet** látható lesz.</span><span class="sxs-lookup"><span data-stu-id="2ea92-186">Once validation has been completed, your profile status will reflect either **Approved** or **Action required** .</span></span> <span data-ttu-id="2ea92-187">Ha **beavatkozás szükséges** , ismételje meg a fenti lépéseket a szükséges információk megadásakor.</span><span class="sxs-lookup"><span data-stu-id="2ea92-187">If **Action Required** , repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="2ea92-188">Az adózási profil létrehozása</span><span class="sxs-lookup"><span data-stu-id="2ea92-188">Create your tax profile</span></span>

<span data-ttu-id="2ea92-189">A következő eljárással biztosíthatja a Microsoft számára a szervezete számára szükséges adózási adatokat.</span><span class="sxs-lookup"><span data-stu-id="2ea92-189">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="2ea92-190">Az ebben a szakaszban szereplő lapok dinamikusak, és az adott országtól vagy régiótól függően változnak.</span><span class="sxs-lookup"><span data-stu-id="2ea92-190">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="2ea92-191">Ha segítségre van szüksége a helyes adózási információk azonosításához, lépjen kapcsolatba az országa megfelelő kormányzati forrásaival.</span><span class="sxs-lookup"><span data-stu-id="2ea92-191">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="2ea92-192">Abban az esetben, ha a W8 vagy a W9 űrlap kitöltéséhez szükséges információkra van szüksége a partner vállalatok számára, a következő címek az IRS webhelyre kerülnek:</span><span class="sxs-lookup"><span data-stu-id="2ea92-192">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="2ea92-193">Csak a vállalat adatait adja meg.</span><span class="sxs-lookup"><span data-stu-id="2ea92-193">Enter only details for your company.</span></span> <span data-ttu-id="2ea92-194">Soha ne adjon meg személyes adatokat.</span><span class="sxs-lookup"><span data-stu-id="2ea92-194">Never enter personal details.</span></span>

1. <span data-ttu-id="2ea92-195">Az **üzleti profil** lapon végezze el a szükséges mezőket, majd kattintson a **tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="2ea92-195">On the **Business Profile** page, complete the required fields and then select **Next** .</span></span> 

2. <span data-ttu-id="2ea92-196">A **telepítés** lapon válassza ki a vállalatára vonatkozó beállítást.</span><span class="sxs-lookup"><span data-stu-id="2ea92-196">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="2ea92-197">Válassza ki a bal oldali lehetőséget, ha a vállalata csak a Egyesült Államokban van beépítve, vagy ha ez a profil egyedi.</span><span class="sxs-lookup"><span data-stu-id="2ea92-197">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="2ea92-198">Ha a vállalat a Egyesült Államokon kívül van beépítve, válassza a jobb oldali lehetőséget, majd válassza ki az országot/régiót a listából.</span><span class="sxs-lookup"><span data-stu-id="2ea92-198">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="2ea92-199">Kattintson a **Tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="2ea92-199">Select **Next** .</span></span> 

4. <span data-ttu-id="2ea92-200">Az **adó állapota** lapon adja meg a szükséges adatokat, majd kattintson a **tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="2ea92-200">On the **Tax status** page, enter the required information, and then select **Next** .</span></span> <span data-ttu-id="2ea92-201">Az ezen a lapon lévő mezők országonként eltérőek lesznek.</span><span class="sxs-lookup"><span data-stu-id="2ea92-201">Fields on this page will vary by country.</span></span> <span data-ttu-id="2ea92-202">a részleteket.</span><span class="sxs-lookup"><span data-stu-id="2ea92-202">your details.</span></span> 

5. <span data-ttu-id="2ea92-203">A **További dokumentáció** lapon a kötelező mezők és a **tovább** gombra.</span><span class="sxs-lookup"><span data-stu-id="2ea92-203">On the **Additional documentation** page, the required fields and select **Next** .</span></span> 

6. <span data-ttu-id="2ea92-204">Válassza a **Tallózás** lehetőséget az országa vagy régiója számára szükséges dokumentumok feltöltéséhez.</span><span class="sxs-lookup"><span data-stu-id="2ea92-204">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="2ea92-205">Ha megjelenik a dokumentum neve, válassza a **feltöltés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2ea92-205">When the document name is shown, select **Upload** .</span></span> 

7. <span data-ttu-id="2ea92-206">Ha el kell távolítania a dokumentumot, válassza az **Eltávolítás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2ea92-206">If you need to remove the document, select **Remove** .</span></span>

8. <span data-ttu-id="2ea92-207">A mentéshez és a folytatáshoz kattintson a **Befejezés** gombra.</span><span class="sxs-lookup"><span data-stu-id="2ea92-207">To save and continue, select **Finish** .</span></span>

9. <span data-ttu-id="2ea92-208">Válassza az előugró üzenet **megerősítés** elemét.</span><span class="sxs-lookup"><span data-stu-id="2ea92-208">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="2ea92-209">Visszakerül a **kifizetés és az adó beállítása** lapra.</span><span class="sxs-lookup"><span data-stu-id="2ea92-209">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2ea92-210">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="2ea92-210">Next steps</span></span>

- [<span data-ttu-id="2ea92-211">Ösztönzők a kifizetési és az adózási profilokkal kapcsolatos gyakori kérdések</span><span class="sxs-lookup"><span data-stu-id="2ea92-211">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
