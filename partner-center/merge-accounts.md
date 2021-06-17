---
title: A partnerfiók egyesítése másik partnerfiókkal
description: Megtudhatja, hogyan egyesítheti a partnerfiókját egy másik partnerfiókkal a Partnerközpont- a vállalatnál aktív Microsoft-partnerek Partnerközpont.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: bcef4c771d748b0e2fbeae8cf1daaf41d7f53b43
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276637"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a><span data-ttu-id="90ce5-103">A partnerfiók egyesítése másik partnerfiókkal</span><span class="sxs-lookup"><span data-stu-id="90ce5-103">Merge your partner account with another partner account</span></span>

<span data-ttu-id="90ce5-104">**Megfelelő szerepkörök:** Fiók-rendszergazda</span><span class="sxs-lookup"><span data-stu-id="90ce5-104">**Appropriate roles**: Account admin</span></span>

<span data-ttu-id="90ce5-105">Két vagy több vállalat, amelyek aktív Microsoft-partnerek, és fiókokkal Partnerközpont dönthetnek a fiókjaik egyesítése között.</span><span class="sxs-lookup"><span data-stu-id="90ce5-105">Two or more companies who are active Microsoft partners and have accounts in Partner Center can choose to merge their accounts.</span></span>

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a><span data-ttu-id="90ce5-106">Mi történik, ha két partner úgy dönt, hogy egyesíti a Partnerközpont fiókjait?</span><span class="sxs-lookup"><span data-stu-id="90ce5-106">What happens when two partners elect to merge their Partner Center accounts</span></span>

- <span data-ttu-id="90ce5-107">Az egyesítést kezdeményező partnerszervezet a globális partnerfiók (PGA) lesz.</span><span class="sxs-lookup"><span data-stu-id="90ce5-107">The partner organization who initiates the merge will be the Partner global account (PGA).</span></span>

- <span data-ttu-id="90ce5-108">A meghívott szervezet PGA-ja lesz a kezdeményező vállalat helye.</span><span class="sxs-lookup"><span data-stu-id="90ce5-108">The invited organization’s PGA becomes a location of the initiating company.</span></span>

- <span data-ttu-id="90ce5-109">Az egyesítési fiók minden helye a PGA-n található hely lesz.</span><span class="sxs-lookup"><span data-stu-id="90ce5-109">All the locations of the merging account become locations under the PGA.</span></span>

- <span data-ttu-id="90ce5-110">A fiók összeolvadása után láthatja a fiók adatait, például a helyeket és a PGA-profilban található felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="90ce5-110">Once the account merger is complete, you will see both account’s details such as locations and users within the PGA profile.</span></span> <span data-ttu-id="90ce5-111">Ez a folyamat nem fordítható meg.</span><span class="sxs-lookup"><span data-stu-id="90ce5-111">You can't reverse this process.</span></span>

- <span data-ttu-id="90ce5-112">A konszolidálás során a helyek összes MPN-i megmaradnak.</span><span class="sxs-lookup"><span data-stu-id="90ce5-112">All MPN IDs for locations are preserved during this consolidation.</span></span>

- <span data-ttu-id="90ce5-113">A felhasználó szerepkörei át vannak hozva.</span><span class="sxs-lookup"><span data-stu-id="90ce5-113">User's roles are brought over.</span></span> <span data-ttu-id="90ce5-114">Ha például egy felhasználó egy adott hely ösztönzőinek rendszergazdája lett volna, akkor az a egyesítés után is ilyen szerepkörben lenne, és láthatná az összeolvadás előtt látott ösztönzőket.</span><span class="sxs-lookup"><span data-stu-id="90ce5-114">For example, if a user had been the incentives admin for a specific location, they would still have that role after the merger and be able to see the incentives they saw prior to the merger.</span></span>

- <span data-ttu-id="90ce5-115">Az Azure AD-bérlők és a CSP-fiókok nincsenek egyesülve, és hatásük sincs.</span><span class="sxs-lookup"><span data-stu-id="90ce5-115">Azure AD tenants and CSP accounts are not merged and have no effect.</span></span>

- <span data-ttu-id="90ce5-116">A közzétett ajánlatok és a mindkét vállalathoz kapcsolódó közös értékesítési folyamatok adatai megmaradnak</span><span class="sxs-lookup"><span data-stu-id="90ce5-116">Published offers and Co-sell pipeline data associated to both companies are preserved</span></span>

### <a name="view-of-merged-accounts"></a><span data-ttu-id="90ce5-117">Egyesített fiókok nézete</span><span class="sxs-lookup"><span data-stu-id="90ce5-117">View of merged accounts</span></span>

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Számlaolvadás.":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a><span data-ttu-id="90ce5-119">Mi várható, ha meg lett hívva, hogy egyesítse a Partnerközpont-fiókot egy Partnerközpont fiókkal?</span><span class="sxs-lookup"><span data-stu-id="90ce5-119">What to expect if you have been invited to merge your Partner Center account with another Partner Center account</span></span>

<span data-ttu-id="90ce5-120">Ha úgy dönt, hogy elfogadja a fiókok egyesítésének meghívását: · Az MPN-azonosító(k) és -helyek egyesülnek az Önt meghívó partnerfiók PGA-jával.</span><span class="sxs-lookup"><span data-stu-id="90ce5-120">If you decide to accept the invitation to merge accounts: · Your MPN ID(s) and locations will be merged into the PGA of the partner account that invited you.</span></span>

- <span data-ttu-id="90ce5-121">A felhasználók az egyesített fiókba lesznek beolvasva, a szerepköreik érintetlenül maradnak.</span><span class="sxs-lookup"><span data-stu-id="90ce5-121">Your users will be brought into the merged account with their roles intact.</span></span>

- <span data-ttu-id="90ce5-122">Az összeolvadás után mindkét vállalat megőrzi a meglévő előnyöket és kompetenciákat a megújításig.</span><span class="sxs-lookup"><span data-stu-id="90ce5-122">Existing benefits and competencies will be preserved for both companies after the merger until renewal.</span></span> <span data-ttu-id="90ce5-123">A megújításkor a fiókok egyetlen vállalatként lesznek kezelve, és a szabványos megújítási szabályok érvényesek lesznek.</span><span class="sxs-lookup"><span data-stu-id="90ce5-123">At renewal, the accounts will be treated as one company and standard renewal rules will apply.</span></span>

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a><span data-ttu-id="90ce5-124">Annak a programokra és előnyökre gyakorolt hatása, amikor a partnerek a fiókok egyesítését választják</span><span class="sxs-lookup"><span data-stu-id="90ce5-124">Understand the impacts to programs and benefits when partners elect to merge accounts</span></span>

- <span data-ttu-id="90ce5-125">A meglévő kompetenciák (Gold/Silver), a vásárlások (például a Microsoft Action Pack) és a kapcsolódó előnyök megmaradnak a konszolidálás során.</span><span class="sxs-lookup"><span data-stu-id="90ce5-125">All existing competencies (Gold/Silver), purchases (such as Microsoft Action Pack), and associated benefits are preserved during consolidation.</span></span> <span data-ttu-id="90ce5-126">Ha mindkét vállalat ugyanazokkal a kompetenciával rendelkezik, de az egyik az arany, a másik ezüst, akkor a legmagasabb jártassági szintű kompetencia lesz díjazva, és a partnerek a következő megújításukig az ezüst és az arany előnyök egy készletével fognak rendelkezni.</span><span class="sxs-lookup"><span data-stu-id="90ce5-126">If both companies have the same competency but one's is gold and the other silver, the competency with highest proficiency level will be awarded, and partners will have one set of silver benefits and one set of gold benefits for that competency until their next renewal.</span></span> 

- <span data-ttu-id="90ce5-127">A Microsoft vállalat legmagasabb évfordulós Action Pack az összeolvadás után is megmarad.</span><span class="sxs-lookup"><span data-stu-id="90ce5-127">Highest anniversary date for Microsoft Action Pack will be retained after the merger.</span></span> <span data-ttu-id="90ce5-128">Ha például az 1. vállalat évfordulója 2020. június, az Action Pack Action Pack megújításának évfordulója pedig a 2020. október 2., a Microsoft a 2020. októberi dátumot használja az egyesített vállalat új évfordulójaként.</span><span class="sxs-lookup"><span data-stu-id="90ce5-128">For example, if the anniversary date for company 1 is June 2020 for Action Pack renewal and the anniversary date for Action Pack renewal for company 2 is October 2020, Microsoft will use the October 2020 date as the new anniversary date for the merged company.</span></span>

- <span data-ttu-id="90ce5-129">A fiók összeolvadása során és a következő megújításáig minden fiók megőrzi a Action Pack/vagy kompetencia-előnyeit.</span><span class="sxs-lookup"><span data-stu-id="90ce5-129">During the account merger and until your next renewal, each account will retain their Action Pack and/or competency benefits.</span></span> <span data-ttu-id="90ce5-130">Megújításkor a standard Action Pack és a kompetencia megújítására vonatkozó szabályok érvényesek.</span><span class="sxs-lookup"><span data-stu-id="90ce5-130">At renewal, standard Action Pack and competency renewal rules apply.</span></span>

- <span data-ttu-id="90ce5-131">A megújítás után a kompetencia megszerzése és Action Pack előnyök a partnervállalat globális partnerfiókja számára vannak megvalósítva:</span><span class="sxs-lookup"><span data-stu-id="90ce5-131">Upon renewal, benefits that are included with competency attainment and Action Pack are implemented for the partner company’s partner global account:</span></span>

  - <span data-ttu-id="90ce5-132">Microsoft Action Pack: A partnervállalat partner globális fiókonként Action Pack vásárolhat egyet.</span><span class="sxs-lookup"><span data-stu-id="90ce5-132">Microsoft Action Pack: The partner company will be able to purchase one Action Pack per partner global account.</span></span>

  - <span data-ttu-id="90ce5-133">Kompetencia: A partnervállalat egy csomag alapvető előnyöket kap, amelyek a legmagasabb szintű végzettségüket, valamint a partner számára a partner számára elérhető kompetenciaspecifikus előnyöket kapják meg globális partnerfiókonként.</span><span class="sxs-lookup"><span data-stu-id="90ce5-133">Competency: The partner company will receive one package of core benefits, associated to their highest attainment, plus competency-specific benefits the partner is eligible for per partner global account.</span></span>

- <span data-ttu-id="90ce5-134">Minden előnyre az Microsoft Partner Network [használati útmutatója vonatkozik.](https://aka.ms/partner-benefits-use-guide)</span><span class="sxs-lookup"><span data-stu-id="90ce5-134">All benefits are subject to the [Microsoft Partner Network benefits usage guide](https://aka.ms/partner-benefits-use-guide).</span></span> <span data-ttu-id="90ce5-135">Például: az aktivált O365 E3 token az aktiválást követően 12 hónapig működik.</span><span class="sxs-lookup"><span data-stu-id="90ce5-135">For example: an activated O365 E3 token is functional for 12 months after activation.</span></span> <span data-ttu-id="90ce5-136">Miután aktiválta a bérlői licencek jogkivonatát, előfordulhat, hogy ezeket a licenceket nem lehet áthelyezni egy másik bérlőbe.</span><span class="sxs-lookup"><span data-stu-id="90ce5-136">Once a token has been activated for licenses on a tenant, those licenses may not be moved to another tenant.</span></span>

- <span data-ttu-id="90ce5-137">Mindkét vállalat MCP-azonosító társításai megmaradnak, és társítva lesznek a PGA MPN-azonosítóval.</span><span class="sxs-lookup"><span data-stu-id="90ce5-137">The MCP ID associations for both companies will be retained and associated with the PGA MPN ID.</span></span>

- <span data-ttu-id="90ce5-138">A piaci piacra juttatás és a műszaki előnyök a kompetencia alapvető előnyeiként állnak rendelkezésre.</span><span class="sxs-lookup"><span data-stu-id="90ce5-138">Go-to-market and technical benefits are offered as competency core benefit.</span></span> <span data-ttu-id="90ce5-139">Az egyesítés után ajánlott ellenőrizni a bank- és adóinformációt a pontosság biztosítása érdekében.</span><span class="sxs-lookup"><span data-stu-id="90ce5-139">Post-merge, it’s recommended that you check your bank and tax information to ensure accuracy.</span></span>

- <span data-ttu-id="90ce5-140">Ha a vállalata a Azure Expert MSP programban van, az előnyök a megújításig megmaradnak.</span><span class="sxs-lookup"><span data-stu-id="90ce5-140">If your company is in the Azure Expert MSP program, benefits are retained until renewal.</span></span>

- <span data-ttu-id="90ce5-141">Ha a vállalata speciális specializációkat szerzett, akkor mindkét fiók megtartja őket.</span><span class="sxs-lookup"><span data-stu-id="90ce5-141">If your company has earned advanced specializations, they are retained across both accounts are retained.</span></span>

- <span data-ttu-id="90ce5-142">A frissítési garanciához szükséges összegeket mindkét fiók megőrzi.</span><span class="sxs-lookup"><span data-stu-id="90ce5-142">Any software assurance vouchers are retained across both accounts.</span></span> 

- <span data-ttu-id="90ce5-143">A DPOR- vagy PAL-társítás nincs hatással.</span><span class="sxs-lookup"><span data-stu-id="90ce5-143">There is no effect to DPOR or PAL association.</span></span> <span data-ttu-id="90ce5-144">A kapcsolódó bevételi hozzájárulások elkezdenek beáramlni az új globális partnerfiókba</span><span class="sxs-lookup"><span data-stu-id="90ce5-144">Any associated revenue contributions will begin to flow into the new Partner Global Account</span></span>

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a><span data-ttu-id="90ce5-145">Vállalat meghívása a saját Partnerközpont a saját Partnerközpont fiókkal</span><span class="sxs-lookup"><span data-stu-id="90ce5-145">Invite a company to merge their Partner Center account with your Partner Center account</span></span>

>[!Note]
><span data-ttu-id="90ce5-146">A fiókegyesítés végrehajtásához Önnek kell **a** vállalat fiókadminisztrátának lennie.</span><span class="sxs-lookup"><span data-stu-id="90ce5-146">To perform the account merger, you must be the **Account admin** for your company.</span></span>

1. <span data-ttu-id="90ce5-147">Az **irányítópulton** válassza a Beállítások Partnerközpont lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="90ce5-147">Select **Settings** from your Partner Center dashboard.</span></span> 

2. <span data-ttu-id="90ce5-148">Válassza a **Fiók egyesítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="90ce5-148">Select **Account merge**.</span></span>

3. <span data-ttu-id="90ce5-149">Adja hozzá a meghívni kívánt fiók **Partnerprofilban** található MPN-azonosítót az egyesítéshez.</span><span class="sxs-lookup"><span data-stu-id="90ce5-149">Add the MPN ID located in the **Partner profile** of the account that you want to invite to merge with you.</span></span> <span data-ttu-id="90ce5-150">A partner globális MPN-azonosítóját kell használnia.</span><span class="sxs-lookup"><span data-stu-id="90ce5-150">You must use their Partner global MPN ID.</span></span> <span data-ttu-id="90ce5-151">Nem használhat hely MPN-azonosítót.</span><span class="sxs-lookup"><span data-stu-id="90ce5-151">You can't use a location MPN ID.</span></span>

4. <span data-ttu-id="90ce5-152">Az **Egyesítés lehetőség kiválasztásakor** a partnervállalat meghívót kap.</span><span class="sxs-lookup"><span data-stu-id="90ce5-152">When you select **Merge**, an invitation is sent to the partner company.</span></span> <span data-ttu-id="90ce5-153">Amikor elfogadják a kérést, kezdeményezheti a fiók egyesítését a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="90ce5-153">When they accept your request, you can initiate the account merge within Partner Center.</span></span> <span data-ttu-id="90ce5-154">Ha a vállalat elutasítja a fiókok egyesítésének kérését, elmagyarázhatja, hogy miért utasítja el a kérelmet.</span><span class="sxs-lookup"><span data-stu-id="90ce5-154">If the company rejects your request to merge accounts, they can explain why they rejected the request.</span></span> <span data-ttu-id="90ce5-155">A fiókegyesítések listája az Egyesítési előzmények **alatt érhető el.**</span><span class="sxs-lookup"><span data-stu-id="90ce5-155">A list of all your account merges is available to you under **Merge history**.</span></span>
 
### <a name="example-of-two-companies-merging-accounts"></a><span data-ttu-id="90ce5-156">Példa két vállalatra, amelyek fiókokat egyesülnek</span><span class="sxs-lookup"><span data-stu-id="90ce5-156">Example of two companies merging accounts</span></span>

1. <span data-ttu-id="90ce5-157">A Contoso, Ltd.</span><span class="sxs-lookup"><span data-stu-id="90ce5-157">Contoso, Ltd. has</span></span> 

    <span data-ttu-id="90ce5-158">a.</span><span class="sxs-lookup"><span data-stu-id="90ce5-158">a.</span></span> <span data-ttu-id="90ce5-159">egy [1111111-es](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) globális MPN-azonosító és egy alárendelt hely [2222222 MPN-azonosítója.](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)</span><span class="sxs-lookup"><span data-stu-id="90ce5-159">a [global MPN ID of 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) and one subordinate [location MPN IDs of 2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).</span></span>
  
    <span data-ttu-id="90ce5-160">b.</span><span class="sxs-lookup"><span data-stu-id="90ce5-160">b.</span></span> <span data-ttu-id="90ce5-161">egy Azure AD-bérlő = @contoso.com</span><span class="sxs-lookup"><span data-stu-id="90ce5-161">an Azure AD tenant = @contoso.com</span></span>
 
    <span data-ttu-id="90ce5-162">c.</span><span class="sxs-lookup"><span data-stu-id="90ce5-162">c.</span></span> <span data-ttu-id="90ce5-163">arany kompetencia, amely 2020. október 1-jére lejár</span><span class="sxs-lookup"><span data-stu-id="90ce5-163">a gold competency that expires October 1, 2020</span></span>
2. <span data-ttu-id="90ce5-164">A Fabrikam, Inc.</span><span class="sxs-lookup"><span data-stu-id="90ce5-164">Fabrikam, Inc. has</span></span>
 
    <span data-ttu-id="90ce5-165">a.</span><span class="sxs-lookup"><span data-stu-id="90ce5-165">a.</span></span>  <span data-ttu-id="90ce5-166">a globális MPN-azonosító 333333, két alárendelt hely MPN-azonosítója pedig 44444444 és 5555555</span><span class="sxs-lookup"><span data-stu-id="90ce5-166">a global MPN ID of 3333333 and two subordinate location MPN IDs of 4444444 and 5555555</span></span>

    <span data-ttu-id="90ce5-167">b.</span><span class="sxs-lookup"><span data-stu-id="90ce5-167">b.</span></span>  <span data-ttu-id="90ce5-168">egy Azure AD-bérlő = @fabrikam.com</span><span class="sxs-lookup"><span data-stu-id="90ce5-168">an Azure AD tenant = @fabrikam.com</span></span>

    <span data-ttu-id="90ce5-169">c.</span><span class="sxs-lookup"><span data-stu-id="90ce5-169">c.</span></span>  <span data-ttu-id="90ce5-170">két arany kompetencia, amelyek 2020. december 1-én lejárnak</span><span class="sxs-lookup"><span data-stu-id="90ce5-170">two gold competencies that expire December 1, 2020</span></span>
3.  <span data-ttu-id="90ce5-171">A Contoso megvásárolja a Fabrikamot, és [itt kezdeményezi](https://partner.microsoft.com/dashboard/account/merger) az egyesítési kérelmet.</span><span class="sxs-lookup"><span data-stu-id="90ce5-171">Contoso buys Fabrikam and goes [here](https://partner.microsoft.com/dashboard/account/merger) to initiate a merge request.</span></span>
4.  <span data-ttu-id="90ce5-172">A Fabrikam bejelentkezik a Partnerközpont, és a Contoso kérésének jóváhagyásához #3 Contoso oldalára lép, mint a #3.</span><span class="sxs-lookup"><span data-stu-id="90ce5-172">Fabrikam signs into Partner Center and goes to the same page as Contoso did in step #3, to approve Contoso’s request.</span></span>
5.  <span data-ttu-id="90ce5-173">A Contoso ugyanezen az oldalon áttekinti az egyesítés részleteit, és megerősíti a fiókegyesítést.</span><span class="sxs-lookup"><span data-stu-id="90ce5-173">Contoso reviews the details of the merge on that same page and provides confirmation to proceed with the account merger.</span></span>
6.  <span data-ttu-id="90ce5-174">A egyesítés után a vállalati fiók a következőként jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="90ce5-174">After the merger, the company account will display as:</span></span>

    <span data-ttu-id="90ce5-175">a.</span><span class="sxs-lookup"><span data-stu-id="90ce5-175">a.</span></span>  <span data-ttu-id="90ce5-176">Egy Contoso nevű vállalat, amely globális MPN-azonosítóval (1111111 és 4 alárendelt hely) 2222222, 3333333, 4444444 és 555555 MPN-azonosítóval</span><span class="sxs-lookup"><span data-stu-id="90ce5-176">A company named Contoso with a global MPN ID of 1111111 and 4 subordinate location MPN IDs of 2222222, 3333333, 4444444, and 5555555</span></span>
    
    <span data-ttu-id="90ce5-177">b.</span><span class="sxs-lookup"><span data-stu-id="90ce5-177">b.</span></span>  <span data-ttu-id="90ce5-178">Két Olyan Azure AD-bérlővel ( + ) rendelkezik, amelyek ugyanathoz a fiókhoz @contoso.com @fabrikam.com Partnerközpont hozzáféréssel</span><span class="sxs-lookup"><span data-stu-id="90ce5-178">It will have two Azure AD tenants (@contoso.com + @fabrikam.com) that have access to the same Partner Center account</span></span>
    
    <span data-ttu-id="90ce5-179">c.</span><span class="sxs-lookup"><span data-stu-id="90ce5-179">c.</span></span>  <span data-ttu-id="90ce5-180">Két kompetencia-kedvezménycsomaggal fog rendelkezni, amelyek közül az egyik 2020. október 1-jére, a másik pedig 2020. december 1-ére lejár.</span><span class="sxs-lookup"><span data-stu-id="90ce5-180">It will have two competency benefits packages, one that expires October 1, 2020 and another that expires December 1, 2020.</span></span> <span data-ttu-id="90ce5-181">2020. december 1-én megújulnak egyetlen kompetencia-juttatási csomagként.</span><span class="sxs-lookup"><span data-stu-id="90ce5-181">They'll be able to renew as a single competency benefits package on December 1, 2020.</span></span> <span data-ttu-id="90ce5-182">A megújításkor a Contoso mindhárom kompetenciát megtartja annak ellenére, hogy csak egyetlen juttatási csomagot tud fenntartani.</span><span class="sxs-lookup"><span data-stu-id="90ce5-182">When they renew, Contoso will retain all three competencies even though they can only maintain a single benefits package.</span></span>
    
7.  <span data-ttu-id="90ce5-183">A Contoso rendszergazdái továbbra is Partnerközpont a @contoso.com felhasználók szerepköreit.</span><span class="sxs-lookup"><span data-stu-id="90ce5-183">Contoso’s admins will continue to manage Partner Center roles for @contoso.com’s users.</span></span> <span data-ttu-id="90ce5-184">A Fabrikam rendszergazdái továbbra is Partnerközpont a @fabrikam.com felhasználók szerepköreit.</span><span class="sxs-lookup"><span data-stu-id="90ce5-184">Fabrikam’s admins will continue to manage Partner Center roles for @fabrikam.com’s users.</span></span> <span data-ttu-id="90ce5-185">A Contoso rendszergazdái csak akkor felügyelik a Fabrikam felhasználóit, ha vendégként vannak meghívva a Fabrikam bérlőjébe.</span><span class="sxs-lookup"><span data-stu-id="90ce5-185">Contoso’s admins can only administer Fabrikam’s users if they are invited as a guest into Fabrikam’s tenant.</span></span>
8.  <span data-ttu-id="90ce5-186">A Contoso dönthet úgy, hogy figyelmen kívül hagyja a bérlőt, és új szerepkörökkel és engedélyekkel új hitelesítő adatokat ad ki a @fabrikam.com Fabrikam-alkalmazottaknak. @contoso.com</span><span class="sxs-lookup"><span data-stu-id="90ce5-186">Contoso could decide to ignore the @fabrikam.com tenant, and reissue the Fabrikam employees new @contoso.com credentials with new roles and permissions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="90ce5-187">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="90ce5-187">Next steps</span></span>

- [<span data-ttu-id="90ce5-188">Felhasználói szerepkörök és engedélyek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="90ce5-188">Assign users roles and permissions</span></span>](permissions-overview.md)

- [<span data-ttu-id="90ce5-189">A partnerprofil információinak ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="90ce5-189">Verify your partner profile information</span></span>](update-your-partner-profile.md)

- [<span data-ttu-id="90ce5-190">További Azure Partner Shared Services, hogy a partnerek saját használatra vásárolhatnak Azure-előfizetéseket</span><span class="sxs-lookup"><span data-stu-id="90ce5-190">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>](shared-services.md)
