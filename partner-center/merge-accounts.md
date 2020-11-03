---
title: A partnerfiók egyesítése másik partnerfiókkal
description: Megtudhatja, hogyan egyesítheti a partneri fiókját egy másik partneri fiókkal a partner Centerben – olyan vállalatoknak, akik aktív Microsoft-partnerek a partner Centerben.
ms.topic: article
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: d38c11e564d6776a5755f8df40ba6ad2dca27d12
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530522"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a><span data-ttu-id="c1585-103">A partnerfiók egyesítése másik partnerfiókkal</span><span class="sxs-lookup"><span data-stu-id="c1585-103">Merge your partner account with another partner account</span></span>

<span data-ttu-id="c1585-104">**Alkalmazható szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="c1585-104">**Applicable roles**</span></span>

- <span data-ttu-id="c1585-105">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="c1585-105">Account admin</span></span>

<span data-ttu-id="c1585-106">Két vagy több olyan vállalat, akik aktív Microsoft-partnerek, és a partner központban található fiókokkal egyesítheti a fiókjaikat.</span><span class="sxs-lookup"><span data-stu-id="c1585-106">Two or more companies who are active Microsoft partners and have accounts in Partner Center can choose to merge their accounts.</span></span>

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a><span data-ttu-id="c1585-107">Mi történik, ha két partner választja a partneri központ fiókjainak egyesítését</span><span class="sxs-lookup"><span data-stu-id="c1585-107">What happens when two partners elect to merge their Partner Center accounts</span></span>

- <span data-ttu-id="c1585-108">Az egyesítést kezdeményező partnerszervezet a partner globális fiókja (PGA) lesz.</span><span class="sxs-lookup"><span data-stu-id="c1585-108">The partner organization who initiates the merge will be the Partner global account (PGA).</span></span>

- <span data-ttu-id="c1585-109">A meghívott szervezet PGA a kezdeményező cég helyévé válik.</span><span class="sxs-lookup"><span data-stu-id="c1585-109">The invited organization’s PGA becomes a location of the initiating company.</span></span>

- <span data-ttu-id="c1585-110">Az egyesítési fiók összes helye a PGA alatt lesz.</span><span class="sxs-lookup"><span data-stu-id="c1585-110">All the locations of the merging account become locations under the PGA.</span></span>

- <span data-ttu-id="c1585-111">A fiók egyesítésének befejezése után a rendszer a fiók adatait, például a helyeit és a felhasználóit is látni fogja a PGA-profilon belül.</span><span class="sxs-lookup"><span data-stu-id="c1585-111">Once the account merger is complete, you will see both account’s details such as locations and users within the PGA profile.</span></span> <span data-ttu-id="c1585-112">Ezt a folyamatot nem lehet megfordítani.</span><span class="sxs-lookup"><span data-stu-id="c1585-112">You can't reverse this process.</span></span>

- <span data-ttu-id="c1585-113">A rendszer a telephelyek összes MPN-azonosítóját megőrzi a konszolidáció során.</span><span class="sxs-lookup"><span data-stu-id="c1585-113">All MPN IDs for locations are preserved during this consolidation.</span></span>

- <span data-ttu-id="c1585-114">A felhasználó szerepkörei átkerülnek.</span><span class="sxs-lookup"><span data-stu-id="c1585-114">User's roles are brought over.</span></span> <span data-ttu-id="c1585-115">Ha például egy felhasználó egy adott helyhez tartozó ösztönző rendszergazda volt, akkor továbbra is ezt a szerepkört venné az egyesítés után, és láthatja az egyesítés előtt látott ösztönzőket.</span><span class="sxs-lookup"><span data-stu-id="c1585-115">For example, if a user had been the incentives admin for a specific location, they would still have that role after the merger and be able to see the incentives they saw prior to the merger.</span></span>

- <span data-ttu-id="c1585-116">Az Azure AD-bérlők és a CSP-fiókok nincsenek egyesítve, és nincsenek hatással a műveletekre.</span><span class="sxs-lookup"><span data-stu-id="c1585-116">Azure AD tenants and CSP accounts are not merged and have no impact.</span></span>

- <span data-ttu-id="c1585-117">A rendszer megőrzi a közzétett ajánlatokat és a két vállalathoz kapcsolódó, közös értékesítési folyamatokat</span><span class="sxs-lookup"><span data-stu-id="c1585-117">Published offers and co-sell pipeline data associated to both companies are preserved</span></span>

### <a name="view-of-merged-accounts"></a><span data-ttu-id="c1585-118">Egyesített fiókok megtekintése</span><span class="sxs-lookup"><span data-stu-id="c1585-118">View of merged accounts</span></span>

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Fiók egyesítése":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a><span data-ttu-id="c1585-120">Mire számíthat, ha meghívást kapott a partner Center-fiók összevonására egy másik partner Center-fiókkal</span><span class="sxs-lookup"><span data-stu-id="c1585-120">What to expect if you have been invited to merge your Partner Center account with another Partner Center account</span></span>

<span data-ttu-id="c1585-121">Ha úgy dönt, hogy elfogadja a meghívót a fiókok egyesítéséhez: · Az MPN-azonosító (k) és a helyszínek egyesítve lesznek a meghívott partner fiókba.</span><span class="sxs-lookup"><span data-stu-id="c1585-121">If you decide to accept the invitation to merge accounts: · Your MPN ID(s) and locations will be merged into the PGA of the partner account that invited you.</span></span>

- <span data-ttu-id="c1585-122">A felhasználók a szerepkörük érintetlen módon lesznek bevezetve az egyesített fiókba.</span><span class="sxs-lookup"><span data-stu-id="c1585-122">Your users will be brought into the merged account with their roles intact.</span></span>

- <span data-ttu-id="c1585-123">A meglévő előnyök és kompetenciák a megújítást követően mindkét vállalatnál megmaradnak.</span><span class="sxs-lookup"><span data-stu-id="c1585-123">Existing benefits and competencies will be preserved for both companies after the merger until renewal.</span></span> <span data-ttu-id="c1585-124">A megújítás során a rendszer a fiókokat egy vállalati és standard megújítási szabályként fogja kezelni.</span><span class="sxs-lookup"><span data-stu-id="c1585-124">At renewal, the accounts will be treated as one company and standard renewal rules will apply.</span></span>

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a><span data-ttu-id="c1585-125">Ismerje meg, hogy milyen hatással vannak a programokra és a kedvezményekre, amikor a partnerek egyesíteni tudják</span><span class="sxs-lookup"><span data-stu-id="c1585-125">Understand the impacts to programs and benefits when partners elect to merge accounts</span></span>

- <span data-ttu-id="c1585-126">Az összevonás során a meglévő kompetenciák (arany/ezüst), a vásárlások (például a Microsoft Action Pack) és a hozzájuk kapcsolódó előnyök is megmaradnak.</span><span class="sxs-lookup"><span data-stu-id="c1585-126">All existing competencies (Gold/Silver), purchases (such as Microsoft Action Pack), and associated benefits are preserved during consolidation.</span></span> <span data-ttu-id="c1585-127">Ha mindkét vállalat ugyanazzal a kompetenciával rendelkezik, de az egyik az arany, a másik ezüst, a legmagasabb szintű szakértelemmel rendelkező kompetenciát kapja meg, és a partnerek a következő megújításuk előtt egy sor ezüst előnnyel és egy arany előnnyel rendelkeznek.</span><span class="sxs-lookup"><span data-stu-id="c1585-127">If both companies have the same competency but one's is gold and the other silver, the competency with highest proficiency level will be awarded, and partners will have one set of silver benefits and one set of gold benefits for that competency until their next renewal.</span></span> 

- <span data-ttu-id="c1585-128">A Microsoft Action Pack számára a legmagasabb évfordulós időszakot az egyesítés után megőrzi a rendszer.</span><span class="sxs-lookup"><span data-stu-id="c1585-128">Highest anniversary date for Microsoft Action Pack will be retained after the merger.</span></span> <span data-ttu-id="c1585-129">Ha például az 2020 1. vállalat évfordulójának dátuma Action Pack a megújításhoz, és a 2. vállalat Action Pack megújításának évfordulós dátuma október 2020, a Microsoft az október 2020 dátumot fogja használni az egyesített vállalat új évfordulójának napján.</span><span class="sxs-lookup"><span data-stu-id="c1585-129">For example, if the anniversary date for company 1 is June 2020 for Action Pack renewal and the anniversary date for Action Pack renewal for company 2 is October 2020, Microsoft will use the October 2020 date as the new anniversary date for the merged company.</span></span>

- <span data-ttu-id="c1585-130">A fiók egyesítése és a következő megújítása előtt minden fiók megtartja Action Pack és/vagy kompetenciájuk előnyeit.</span><span class="sxs-lookup"><span data-stu-id="c1585-130">During the account merger and until your next renewal, each account will retain their Action Pack and/or competency benefits.</span></span> <span data-ttu-id="c1585-131">A Megújításkor a standard Action Pack és a kompetenciák megújítására vonatkozó szabályok érvényesek.</span><span class="sxs-lookup"><span data-stu-id="c1585-131">At renewal, standard Action Pack and competency renewal rules apply.</span></span>

- <span data-ttu-id="c1585-132">A megújítást követően a kompetenciák megvalósításához és a Action Packhoz tartozó előnyök a partner cég partner globális fiókjához tartoznak:</span><span class="sxs-lookup"><span data-stu-id="c1585-132">Upon renewal, benefits that are included with competency attainment and Action Pack are implemented for the partner company’s partner global account:</span></span>

  - <span data-ttu-id="c1585-133">Microsoft Action Pack: a partner cég egy Action Pack partner globális fiókban vásárolható meg.</span><span class="sxs-lookup"><span data-stu-id="c1585-133">Microsoft Action Pack: The partner company will be able to purchase one Action Pack per partner global account.</span></span>

  - <span data-ttu-id="c1585-134">Kompetencia: a partner cég egy, a legmagasabb szintű megvalósításhoz kapcsolódó alapellátási csomagot kap, valamint a kompetenciával kapcsolatos előnyökkel is rendelkezik, melyekhez a partner globális fiókja jogosult.</span><span class="sxs-lookup"><span data-stu-id="c1585-134">Competency: The partner company will receive one package of core benefits, associated to their highest attainment, plus competency-specific benefits the partner is eligible for per partner global account.</span></span>

- <span data-ttu-id="c1585-135">Minden előnyre a [Microsoft Partner Network előnyök használati útmutatója](https://aka.ms/partner-benefits-use-guide)vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="c1585-135">All benefits are subject to the [Microsoft Partner Network benefits usage guide](https://aka.ms/partner-benefits-use-guide).</span></span> <span data-ttu-id="c1585-136">Például: egy aktivált O365 E3 token az aktiválás után tizenkét (12) hónapig működik.</span><span class="sxs-lookup"><span data-stu-id="c1585-136">For example: an activated O365 E3 token is functional for twelve (12) months after activation.</span></span> <span data-ttu-id="c1585-137">Miután aktiválta a jogkivonatot a bérlői licencekhez, előfordulhat, hogy ezek a licencek nem helyezhetők át másik bérlőre.</span><span class="sxs-lookup"><span data-stu-id="c1585-137">Once a token has been activated for licenses on a tenant, those licenses may not be moved to another tenant.</span></span>

- <span data-ttu-id="c1585-138">Mindkét vállalathoz tartozó MCP-azonosító társítások megmaradnak és a PGA MPN-AZONOSÍTÓhoz lesznek társítva.</span><span class="sxs-lookup"><span data-stu-id="c1585-138">The MCP ID associations for both companies will be retained and associated with the PGA MPN ID.</span></span>

- <span data-ttu-id="c1585-139">A piaci megjelenés és a technikai előnyök a kompetenciák alapszintű juttatásként is elérhetők.</span><span class="sxs-lookup"><span data-stu-id="c1585-139">Go-to-market and technical benefits are offered as competency core benefit.</span></span> <span data-ttu-id="c1585-140">Az egyesítés után javasoljuk, hogy ellenőrizze a banki és adózási adatokat, hogy biztosítsa a pontosságot.</span><span class="sxs-lookup"><span data-stu-id="c1585-140">Post-merge, it’s recommended that you check your bank and tax information to ensure accuracy.</span></span>

- <span data-ttu-id="c1585-141">Ha a vállalata az Azure szakértői MSP-programban van, akkor a rendszer a megújítás után is megőrzi az előnyöket.</span><span class="sxs-lookup"><span data-stu-id="c1585-141">If your company is in the Azure Expert MSP program, benefits are retained until renewal.</span></span>

- <span data-ttu-id="c1585-142">Ha a vállalata fejlett specializációkat szerzett, ezeket a rendszer megőrzi mindkét fiókban.</span><span class="sxs-lookup"><span data-stu-id="c1585-142">If your company has earned advanced specializations, they are retained across both accounts are retained.</span></span>

- <span data-ttu-id="c1585-143">Minden frissítési garanciát igazoló bizonylatot mindkét fiókban meg kell őrizni.</span><span class="sxs-lookup"><span data-stu-id="c1585-143">Any software assurance vouchers are retained across both accounts.</span></span> 

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a><span data-ttu-id="c1585-144">Kérje meg a vállalatot, hogy egyesítse a partner Center-fiókját a partner Center-fiókkal</span><span class="sxs-lookup"><span data-stu-id="c1585-144">Invite a company to merge their Partner Center account with your Partner Center account</span></span>

>[!Note]
><span data-ttu-id="c1585-145">A fiók egyesítésének végrehajtásához a vállalata **fiókjának rendszergazdájának** kell lennie.</span><span class="sxs-lookup"><span data-stu-id="c1585-145">To perform the account merger, you must be the **Account admin** for your company.</span></span>

1. <span data-ttu-id="c1585-146">Válassza ki a kívánt **beállításokat** a partner Center irányítópultján.</span><span class="sxs-lookup"><span data-stu-id="c1585-146">Select **Settings** from your Partner Center dashboard.</span></span> 

2. <span data-ttu-id="c1585-147">Válassza a **fiók egyesítése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c1585-147">Select **Account merge** .</span></span>

3. <span data-ttu-id="c1585-148">Adja hozzá az MPN-azonosítót annak a fióknak a **partner profiljában** , amelyet meg szeretne hívni az egyesítéshez.</span><span class="sxs-lookup"><span data-stu-id="c1585-148">Add the MPN ID located in the **Partner profile** of the account you want to invite to merge with you.</span></span> <span data-ttu-id="c1585-149">A partner globális MPN-AZONOSÍTÓját kell használnia.</span><span class="sxs-lookup"><span data-stu-id="c1585-149">You must use their Partner global MPN ID.</span></span> <span data-ttu-id="c1585-150">A Location MPN-azonosító nem használható.</span><span class="sxs-lookup"><span data-stu-id="c1585-150">You can't use a location MPN ID.</span></span>

4. <span data-ttu-id="c1585-151">Ha az **Egyesítés** lehetőséget választja, a rendszer meghívót küld a partner cégnek.</span><span class="sxs-lookup"><span data-stu-id="c1585-151">When you select **Merge** , an invitation is sent to the partner company.</span></span> <span data-ttu-id="c1585-152">Ha elfogadja a kérést, elindíthatja a fiók egyesítését a partner centeren belül.</span><span class="sxs-lookup"><span data-stu-id="c1585-152">When they accept your request, you can initiate the account merge within Partner Center.</span></span> <span data-ttu-id="c1585-153">Ha a vállalat elutasítja a fiókok egyesítésére vonatkozó kérelmét, megtudhatja, miért utasította el a kérést.</span><span class="sxs-lookup"><span data-stu-id="c1585-153">If the company rejects your request to merge accounts, they can explain why they rejected the request.</span></span> <span data-ttu-id="c1585-154">Az **egyesítési előzmények** listájában az összes fiók egyesítése elérhető.</span><span class="sxs-lookup"><span data-stu-id="c1585-154">A list of all your account merges is available to you under **Merge history** .</span></span>

## <a name="next-steps"></a><span data-ttu-id="c1585-155">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c1585-155">Next steps</span></span>

- [<span data-ttu-id="c1585-156">Felhasználói szerepkörök és engedélyek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="c1585-156">Assign users roles and permissions</span></span>](permissions-overview.md)

- [<span data-ttu-id="c1585-157">Partneri profil adatainak ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="c1585-157">Verify your partner profile information</span></span>](update-your-partner-profile.md)

- [<span data-ttu-id="c1585-158">Azure partner megosztott szolgáltatások hozzáadása, hogy a partnerek saját használatra tudják megvásárolni az Azure-előfizetéseket</span><span class="sxs-lookup"><span data-stu-id="c1585-158">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>](shared-services.md)
