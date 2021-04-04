---
title: A partnerfiók egyesítése másik partnerfiókkal
description: Megtudhatja, hogyan egyesítheti a partneri fiókját egy másik partneri fiókkal a partner Centerben – olyan vállalatoknak, akik aktív Microsoft-partnerek a partner Centerben.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: 90d1fe9728c43d2f34b6cfe2d9e4c9613d865aeb
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/01/2021
ms.locfileid: "106133063"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a><span data-ttu-id="545c6-103">A partnerfiók egyesítése másik partnerfiókkal</span><span class="sxs-lookup"><span data-stu-id="545c6-103">Merge your partner account with another partner account</span></span>

<span data-ttu-id="545c6-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="545c6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="545c6-105">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="545c6-105">Account admin</span></span>

<span data-ttu-id="545c6-106">Két vagy több olyan vállalat, akik aktív Microsoft-partnerek, és a partner központban található fiókokkal egyesítheti a fiókjaikat.</span><span class="sxs-lookup"><span data-stu-id="545c6-106">Two or more companies who are active Microsoft partners and have accounts in Partner Center can choose to merge their accounts.</span></span>

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a><span data-ttu-id="545c6-107">Mi történik, ha két partner választja a partneri központ fiókjainak egyesítését</span><span class="sxs-lookup"><span data-stu-id="545c6-107">What happens when two partners elect to merge their Partner Center accounts</span></span>

- <span data-ttu-id="545c6-108">Az egyesítést kezdeményező partnerszervezet a partner globális fiókja (PGA) lesz.</span><span class="sxs-lookup"><span data-stu-id="545c6-108">The partner organization who initiates the merge will be the Partner global account (PGA).</span></span>

- <span data-ttu-id="545c6-109">A meghívott szervezet PGA a kezdeményező cég helyévé válik.</span><span class="sxs-lookup"><span data-stu-id="545c6-109">The invited organization’s PGA becomes a location of the initiating company.</span></span>

- <span data-ttu-id="545c6-110">Az egyesítési fiók összes helye a PGA alatt lesz.</span><span class="sxs-lookup"><span data-stu-id="545c6-110">All the locations of the merging account become locations under the PGA.</span></span>

- <span data-ttu-id="545c6-111">A fiók egyesítésének befejezése után a rendszer a fiók adatait, például a helyeit és a felhasználóit is látni fogja a PGA-profilon belül.</span><span class="sxs-lookup"><span data-stu-id="545c6-111">Once the account merger is complete, you will see both account’s details such as locations and users within the PGA profile.</span></span> <span data-ttu-id="545c6-112">Ezt a folyamatot nem lehet megfordítani.</span><span class="sxs-lookup"><span data-stu-id="545c6-112">You can't reverse this process.</span></span>

- <span data-ttu-id="545c6-113">A rendszer a telephelyek összes MPN-azonosítóját megőrzi a konszolidáció során.</span><span class="sxs-lookup"><span data-stu-id="545c6-113">All MPN IDs for locations are preserved during this consolidation.</span></span>

- <span data-ttu-id="545c6-114">A felhasználó szerepkörei átkerülnek.</span><span class="sxs-lookup"><span data-stu-id="545c6-114">User's roles are brought over.</span></span> <span data-ttu-id="545c6-115">Ha például egy felhasználó egy adott helyhez tartozó ösztönző rendszergazda volt, akkor továbbra is ezt a szerepkört venné az egyesítés után, és láthatja az egyesítés előtt látott ösztönzőket.</span><span class="sxs-lookup"><span data-stu-id="545c6-115">For example, if a user had been the incentives admin for a specific location, they would still have that role after the merger and be able to see the incentives they saw prior to the merger.</span></span>

- <span data-ttu-id="545c6-116">Az Azure AD-bérlők és a CSP-fiókok nincsenek egyesítve, és nincs hatása.</span><span class="sxs-lookup"><span data-stu-id="545c6-116">Azure AD tenants and CSP accounts are not merged and have no effect.</span></span>

- <span data-ttu-id="545c6-117">A rendszer megőrzi a közzétett ajánlatokat és a két vállalathoz kapcsolódó, közös értékesítési folyamatokat</span><span class="sxs-lookup"><span data-stu-id="545c6-117">Published offers and Co-sell pipeline data associated to both companies are preserved</span></span>

### <a name="view-of-merged-accounts"></a><span data-ttu-id="545c6-118">Egyesített fiókok megtekintése</span><span class="sxs-lookup"><span data-stu-id="545c6-118">View of merged accounts</span></span>

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Fiók egyesítése":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a><span data-ttu-id="545c6-120">Mire számíthat, ha meghívást kapott a partner Center-fiók összevonására egy másik partner Center-fiókkal</span><span class="sxs-lookup"><span data-stu-id="545c6-120">What to expect if you have been invited to merge your Partner Center account with another Partner Center account</span></span>

<span data-ttu-id="545c6-121">Ha úgy dönt, hogy elfogadja a meghívót a fiókok egyesítéséhez: · Az MPN-azonosító (k) és a helyszínek egyesítve lesznek a meghívott partner fiókba.</span><span class="sxs-lookup"><span data-stu-id="545c6-121">If you decide to accept the invitation to merge accounts: · Your MPN ID(s) and locations will be merged into the PGA of the partner account that invited you.</span></span>

- <span data-ttu-id="545c6-122">A felhasználók a szerepkörük érintetlen módon lesznek bevezetve az egyesített fiókba.</span><span class="sxs-lookup"><span data-stu-id="545c6-122">Your users will be brought into the merged account with their roles intact.</span></span>

- <span data-ttu-id="545c6-123">A meglévő előnyök és kompetenciák a megújítást követően mindkét vállalatnál megmaradnak.</span><span class="sxs-lookup"><span data-stu-id="545c6-123">Existing benefits and competencies will be preserved for both companies after the merger until renewal.</span></span> <span data-ttu-id="545c6-124">A megújítás során a rendszer a fiókokat egy vállalati és standard megújítási szabályként fogja kezelni.</span><span class="sxs-lookup"><span data-stu-id="545c6-124">At renewal, the accounts will be treated as one company and standard renewal rules will apply.</span></span>

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a><span data-ttu-id="545c6-125">Ismerje meg, hogy milyen hatással vannak a programokra és a kedvezményekre, amikor a partnerek egyesíteni tudják</span><span class="sxs-lookup"><span data-stu-id="545c6-125">Understand the impacts to programs and benefits when partners elect to merge accounts</span></span>

- <span data-ttu-id="545c6-126">Az összevonás során a meglévő kompetenciák (arany/ezüst), a vásárlások (például a Microsoft Action Pack) és a hozzájuk kapcsolódó előnyök is megmaradnak.</span><span class="sxs-lookup"><span data-stu-id="545c6-126">All existing competencies (Gold/Silver), purchases (such as Microsoft Action Pack), and associated benefits are preserved during consolidation.</span></span> <span data-ttu-id="545c6-127">Ha mindkét vállalat ugyanazzal a kompetenciával rendelkezik, de az egyik az arany, a másik ezüst, a legmagasabb szintű szakértelemmel rendelkező kompetenciát kapja meg, és a partnerek a következő megújításuk előtt egy sor ezüst előnnyel és egy arany előnnyel rendelkeznek.</span><span class="sxs-lookup"><span data-stu-id="545c6-127">If both companies have the same competency but one's is gold and the other silver, the competency with highest proficiency level will be awarded, and partners will have one set of silver benefits and one set of gold benefits for that competency until their next renewal.</span></span> 

- <span data-ttu-id="545c6-128">A Microsoft Action Pack számára a legmagasabb évfordulós időszakot az egyesítés után megőrzi a rendszer.</span><span class="sxs-lookup"><span data-stu-id="545c6-128">Highest anniversary date for Microsoft Action Pack will be retained after the merger.</span></span> <span data-ttu-id="545c6-129">Ha például az 2020 1. vállalat évfordulójának dátuma Action Pack a megújításhoz, és a 2. vállalat Action Pack megújításának évfordulós dátuma október 2020, a Microsoft az október 2020 dátumot fogja használni az egyesített vállalat új évfordulójának napján.</span><span class="sxs-lookup"><span data-stu-id="545c6-129">For example, if the anniversary date for company 1 is June 2020 for Action Pack renewal and the anniversary date for Action Pack renewal for company 2 is October 2020, Microsoft will use the October 2020 date as the new anniversary date for the merged company.</span></span>

- <span data-ttu-id="545c6-130">A fiók egyesítése és a következő megújítása előtt minden fiók megtartja Action Pack és/vagy kompetenciájuk előnyeit.</span><span class="sxs-lookup"><span data-stu-id="545c6-130">During the account merger and until your next renewal, each account will retain their Action Pack and/or competency benefits.</span></span> <span data-ttu-id="545c6-131">A Megújításkor a standard Action Pack és a kompetenciák megújítására vonatkozó szabályok érvényesek.</span><span class="sxs-lookup"><span data-stu-id="545c6-131">At renewal, standard Action Pack and competency renewal rules apply.</span></span>

- <span data-ttu-id="545c6-132">A megújítást követően a kompetenciák megvalósításához és a Action Packhoz tartozó előnyök a partner cég partner globális fiókjához tartoznak:</span><span class="sxs-lookup"><span data-stu-id="545c6-132">Upon renewal, benefits that are included with competency attainment and Action Pack are implemented for the partner company’s partner global account:</span></span>

  - <span data-ttu-id="545c6-133">Microsoft Action Pack: a partner cég egy Action Pack partner globális fiókban vásárolható meg.</span><span class="sxs-lookup"><span data-stu-id="545c6-133">Microsoft Action Pack: The partner company will be able to purchase one Action Pack per partner global account.</span></span>

  - <span data-ttu-id="545c6-134">Kompetencia: a partner cég egy, a legmagasabb szintű megvalósításhoz kapcsolódó alapellátási csomagot kap, valamint a kompetenciával kapcsolatos előnyökkel is rendelkezik, melyekhez a partner globális fiókja jogosult.</span><span class="sxs-lookup"><span data-stu-id="545c6-134">Competency: The partner company will receive one package of core benefits, associated to their highest attainment, plus competency-specific benefits the partner is eligible for per partner global account.</span></span>

- <span data-ttu-id="545c6-135">Minden előnyre a [Microsoft Partner Network előnyök használati útmutatója](https://aka.ms/partner-benefits-use-guide)vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="545c6-135">All benefits are subject to the [Microsoft Partner Network benefits usage guide](https://aka.ms/partner-benefits-use-guide).</span></span> <span data-ttu-id="545c6-136">Például: az aktivált O365 E3-token az aktiválást követő 12 hónapig működik.</span><span class="sxs-lookup"><span data-stu-id="545c6-136">For example: an activated O365 E3 token is functional for 12 months after activation.</span></span> <span data-ttu-id="545c6-137">Miután aktiválta a jogkivonatot a bérlői licencekhez, előfordulhat, hogy ezek a licencek nem helyezhetők át másik bérlőre.</span><span class="sxs-lookup"><span data-stu-id="545c6-137">Once a token has been activated for licenses on a tenant, those licenses may not be moved to another tenant.</span></span>

- <span data-ttu-id="545c6-138">Mindkét vállalathoz tartozó MCP-azonosító társítások megmaradnak és a PGA MPN-AZONOSÍTÓhoz lesznek társítva.</span><span class="sxs-lookup"><span data-stu-id="545c6-138">The MCP ID associations for both companies will be retained and associated with the PGA MPN ID.</span></span>

- <span data-ttu-id="545c6-139">A piaci megjelenés és a technikai előnyök a kompetenciák alapszintű juttatásként is elérhetők.</span><span class="sxs-lookup"><span data-stu-id="545c6-139">Go-to-market and technical benefits are offered as competency core benefit.</span></span> <span data-ttu-id="545c6-140">Az egyesítés után javasoljuk, hogy ellenőrizze a banki és adózási adatokat, hogy biztosítsa a pontosságot.</span><span class="sxs-lookup"><span data-stu-id="545c6-140">Post-merge, it’s recommended that you check your bank and tax information to ensure accuracy.</span></span>

- <span data-ttu-id="545c6-141">Ha a vállalata az Azure szakértői MSP-programban van, akkor a rendszer a megújítás után is megőrzi az előnyöket.</span><span class="sxs-lookup"><span data-stu-id="545c6-141">If your company is in the Azure Expert MSP program, benefits are retained until renewal.</span></span>

- <span data-ttu-id="545c6-142">Ha a vállalata fejlett specializációkat szerzett, ezeket a rendszer megőrzi mindkét fiókban.</span><span class="sxs-lookup"><span data-stu-id="545c6-142">If your company has earned advanced specializations, they are retained across both accounts are retained.</span></span>

- <span data-ttu-id="545c6-143">Minden frissítési garanciát igazoló bizonylatot mindkét fiókban meg kell őrizni.</span><span class="sxs-lookup"><span data-stu-id="545c6-143">Any software assurance vouchers are retained across both accounts.</span></span> 

- <span data-ttu-id="545c6-144">A DPOR és a PAL társításnak nincs hatása.</span><span class="sxs-lookup"><span data-stu-id="545c6-144">There is no effect to DPOR or PAL association.</span></span> <span data-ttu-id="545c6-145">A kapcsolódó bevételi hozzájárulások megkezdik az új partner globális fiókba való beáramlást</span><span class="sxs-lookup"><span data-stu-id="545c6-145">Any associated revenue contributions will begin to flow into the new Partner Global Account</span></span>

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a><span data-ttu-id="545c6-146">Kérje meg a vállalatot, hogy egyesítse a partner Center-fiókját a partner Center-fiókkal</span><span class="sxs-lookup"><span data-stu-id="545c6-146">Invite a company to merge their Partner Center account with your Partner Center account</span></span>

>[!Note]
><span data-ttu-id="545c6-147">A fiók egyesítésének végrehajtásához a vállalata **fiókjának rendszergazdájának** kell lennie.</span><span class="sxs-lookup"><span data-stu-id="545c6-147">To perform the account merger, you must be the **Account admin** for your company.</span></span>

1. <span data-ttu-id="545c6-148">Válassza ki a kívánt **beállításokat** a partner Center irányítópultján.</span><span class="sxs-lookup"><span data-stu-id="545c6-148">Select **Settings** from your Partner Center dashboard.</span></span> 

2. <span data-ttu-id="545c6-149">Válassza a **fiók egyesítése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="545c6-149">Select **Account merge**.</span></span>

3. <span data-ttu-id="545c6-150">Adja hozzá annak a fióknak a **partner-profiljában** található MPN-azonosítót, amelyet meg szeretne hívni az egyesítéshez.</span><span class="sxs-lookup"><span data-stu-id="545c6-150">Add the MPN ID located in the **Partner profile** of the account that you want to invite to merge with you.</span></span> <span data-ttu-id="545c6-151">A partner globális MPN-AZONOSÍTÓját kell használnia.</span><span class="sxs-lookup"><span data-stu-id="545c6-151">You must use their Partner global MPN ID.</span></span> <span data-ttu-id="545c6-152">A Location MPN-azonosító nem használható.</span><span class="sxs-lookup"><span data-stu-id="545c6-152">You can't use a location MPN ID.</span></span>

4. <span data-ttu-id="545c6-153">Ha az **Egyesítés** lehetőséget választja, a rendszer meghívót küld a partner cégnek.</span><span class="sxs-lookup"><span data-stu-id="545c6-153">When you select **Merge**, an invitation is sent to the partner company.</span></span> <span data-ttu-id="545c6-154">Ha elfogadja a kérést, elindíthatja a fiók egyesítését a partner centeren belül.</span><span class="sxs-lookup"><span data-stu-id="545c6-154">When they accept your request, you can initiate the account merge within Partner Center.</span></span> <span data-ttu-id="545c6-155">Ha a vállalat elutasítja a fiókok egyesítésére vonatkozó kérelmét, megtudhatja, miért utasította el a kérést.</span><span class="sxs-lookup"><span data-stu-id="545c6-155">If the company rejects your request to merge accounts, they can explain why they rejected the request.</span></span> <span data-ttu-id="545c6-156">Az **egyesítési előzmények** listájában az összes fiók egyesítése elérhető.</span><span class="sxs-lookup"><span data-stu-id="545c6-156">A list of all your account merges is available to you under **Merge history**.</span></span>
 
### <a name="example-of-two-companies-merging-accounts"></a><span data-ttu-id="545c6-157">Példa két vállalat fiókjainak egyesítésére</span><span class="sxs-lookup"><span data-stu-id="545c6-157">Example of two companies merging accounts</span></span>

1. <span data-ttu-id="545c6-158">Contoso, Ltd.</span><span class="sxs-lookup"><span data-stu-id="545c6-158">Contoso, Ltd. has</span></span> 

    <span data-ttu-id="545c6-159">a.</span><span class="sxs-lookup"><span data-stu-id="545c6-159">a.</span></span> <span data-ttu-id="545c6-160">az [1111111-es globális MPN-azonosító](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) és a 2222222-es ALÁRENDELT [hely MPN](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)-azonosítója.</span><span class="sxs-lookup"><span data-stu-id="545c6-160">a [global MPN ID of 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) and one subordinate [location MPN IDs of 2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).</span></span>
  
    <span data-ttu-id="545c6-161">b.</span><span class="sxs-lookup"><span data-stu-id="545c6-161">b.</span></span> <span data-ttu-id="545c6-162">egy Azure AD-bérlő = @contoso.com</span><span class="sxs-lookup"><span data-stu-id="545c6-162">an Azure AD tenant = @contoso.com</span></span>
 
    <span data-ttu-id="545c6-163">c.</span><span class="sxs-lookup"><span data-stu-id="545c6-163">c.</span></span> <span data-ttu-id="545c6-164">Gold kompetencia, amely 2020. október 1-től lejár</span><span class="sxs-lookup"><span data-stu-id="545c6-164">a gold competency that expires October 1, 2020</span></span>
2. <span data-ttu-id="545c6-165">Fabrikam, Inc.</span><span class="sxs-lookup"><span data-stu-id="545c6-165">Fabrikam, Inc. has</span></span>
 
    <span data-ttu-id="545c6-166">a.</span><span class="sxs-lookup"><span data-stu-id="545c6-166">a.</span></span>  <span data-ttu-id="545c6-167">az 3333333-es globális MPN-azonosító és a 4444444-es és 5555555-as két alárendelt hely MPN-azonosítói</span><span class="sxs-lookup"><span data-stu-id="545c6-167">a global MPN ID of 3333333 and two subordinate location MPN IDs of 4444444 and 5555555</span></span>

    <span data-ttu-id="545c6-168">b.</span><span class="sxs-lookup"><span data-stu-id="545c6-168">b.</span></span>  <span data-ttu-id="545c6-169">egy Azure AD-bérlő = @fabrikam.com</span><span class="sxs-lookup"><span data-stu-id="545c6-169">an Azure AD tenant = @fabrikam.com</span></span>

    <span data-ttu-id="545c6-170">c.</span><span class="sxs-lookup"><span data-stu-id="545c6-170">c.</span></span>  <span data-ttu-id="545c6-171">két arany-kompetencia, amely 2020 december 1-től lejár</span><span class="sxs-lookup"><span data-stu-id="545c6-171">two gold competencies that expire December 1, 2020</span></span>
3.  <span data-ttu-id="545c6-172">A contoso megvásárolja a Fabrikamt, és elindít egy [merge-kérelmet](https://partner.microsoft.com/dashboard/account/merger) .</span><span class="sxs-lookup"><span data-stu-id="545c6-172">Contoso buys Fabrikam and goes [here](https://partner.microsoft.com/dashboard/account/merger) to initiate a merge request.</span></span>
4.  <span data-ttu-id="545c6-173">A fabrikam bejelentkezik a fiókpartner-központba, és a contoso kérésének jóváhagyásához a contoso által #3 lépésben megjelenő lapra kerül.</span><span class="sxs-lookup"><span data-stu-id="545c6-173">Fabrikam signs into Partner Center and goes to the same page as Contoso did in step #3, to approve Contoso’s request.</span></span>
5.  <span data-ttu-id="545c6-174">A contoso megtekinti az ugyanazon az oldalon lévő egyesítés részleteit, és megerősítést nyújt a fiók egyesítésének folytatásához.</span><span class="sxs-lookup"><span data-stu-id="545c6-174">Contoso reviews the details of the merge on that same page and provides confirmation to proceed with the account merger.</span></span>
6.  <span data-ttu-id="545c6-175">Az egyesítés után a vállalati fiók a következőképpen jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="545c6-175">After the merger, the company account will display as:</span></span>

    <span data-ttu-id="545c6-176">a.</span><span class="sxs-lookup"><span data-stu-id="545c6-176">a.</span></span>  <span data-ttu-id="545c6-177">Egy contoso nevű vállalat, amelynek globális MPN-azonosítója 1111111 és 4 alárendelt Location MPN-azonosító, 2222222, 3333333, 4444444 és 5555555</span><span class="sxs-lookup"><span data-stu-id="545c6-177">A company named Contoso with a global MPN ID of 1111111 and 4 subordinate location MPN IDs of 2222222, 3333333, 4444444, and 5555555</span></span>
    
    <span data-ttu-id="545c6-178">b.</span><span class="sxs-lookup"><span data-stu-id="545c6-178">b.</span></span>  <span data-ttu-id="545c6-179">Két Azure AD-bérlő ( @contoso.com + @fabrikam.com ) fér hozzá ugyanahhoz a partner Center-fiókhoz</span><span class="sxs-lookup"><span data-stu-id="545c6-179">It will have two Azure AD tenants (@contoso.com + @fabrikam.com) that have access to the same Partner Center account</span></span>
    
    <span data-ttu-id="545c6-180">c.</span><span class="sxs-lookup"><span data-stu-id="545c6-180">c.</span></span>  <span data-ttu-id="545c6-181">Két kompetenciával rendelkezik, amelyek közül az egyik a 2020. október 1-től lejár, a másik pedig a 2020. december 1-től lejár.</span><span class="sxs-lookup"><span data-stu-id="545c6-181">It will have two competency benefits packages, one that expires October 1, 2020 and another that expires December 1, 2020.</span></span> <span data-ttu-id="545c6-182">A rendszer a 2020-es december 1-jén megújíthatja a kompetencia előnyeit.</span><span class="sxs-lookup"><span data-stu-id="545c6-182">They'll be able to renew as a single competency benefits package on December 1, 2020.</span></span> <span data-ttu-id="545c6-183">Amikor megújítják, a contoso mindhárom kompetenciát megőrzi, annak ellenére, hogy csak egyetlen kedvezményt biztosító csomagot tudnak fenntartani.</span><span class="sxs-lookup"><span data-stu-id="545c6-183">When they renew, Contoso will retain all three competencies even though they can only maintain a single benefits package.</span></span>
    
7.  <span data-ttu-id="545c6-184">A contoso rendszergazdái továbbra is felügyelik a partneri központ szerepköreit a @contoso.com felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="545c6-184">Contoso’s admins will continue to manage Partner Center roles for @contoso.com’s users.</span></span> <span data-ttu-id="545c6-185">A fabrikam rendszergazdái továbbra is felügyelik a partneri központ szerepköreit a @fabrikam.com felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="545c6-185">Fabrikam’s admins will continue to manage Partner Center roles for @fabrikam.com’s users.</span></span> <span data-ttu-id="545c6-186">A contoso rendszergazdái csak akkor felügyelhetik a fabrikam felhasználóit, ha vendégként meghívja őket a fabrikam bérlője számára.</span><span class="sxs-lookup"><span data-stu-id="545c6-186">Contoso’s admins can only administer Fabrikam’s users if they are invited as a guest into Fabrikam’s tenant.</span></span>
8.  <span data-ttu-id="545c6-187">A contoso dönthet úgy, hogy figyelmen kívül hagyja a @fabrikam.com bérlőt, és új szerepkörökkel és engedélyekkel adja ki újra a fabrikam alkalmazottainak új @contoso.com hitelesítő adatait.</span><span class="sxs-lookup"><span data-stu-id="545c6-187">Contoso could decide to ignore the @fabrikam.com tenant, and reissue the Fabrikam employees new @contoso.com credentials with new roles and permissions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="545c6-188">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="545c6-188">Next steps</span></span>

- [<span data-ttu-id="545c6-189">Felhasználói szerepkörök és engedélyek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="545c6-189">Assign users roles and permissions</span></span>](permissions-overview.md)

- [<span data-ttu-id="545c6-190">Partneri profil adatainak ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="545c6-190">Verify your partner profile information</span></span>](update-your-partner-profile.md)

- [<span data-ttu-id="545c6-191">Azure partner megosztott szolgáltatások hozzáadása, hogy a partnerek saját használatra tudják megvásárolni az Azure-előfizetéseket</span><span class="sxs-lookup"><span data-stu-id="545c6-191">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>](shared-services.md)
