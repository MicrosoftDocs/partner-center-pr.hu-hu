---
title: Váltás a Direct-Bill partner és a közvetett viszonteladó között
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy a CSP-program partnere hogyan használhatja a partner centert a Direct-Bill partnerről a közvetett viszonteladóra való áttéréshez.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e3cd791f5f9f781980d73c79f0ec18627585372a
ms.sourcegitcommit: b4771fd0781d95551e65baa481a572291c729d7d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/28/2020
ms.locfileid: "92795865"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="752f4-103">Váltás egy közvetlen felhőszolgáltatói (Cloud Solution Provider, CSP-) számlázási partnerről egy közvetett CSP-viszonteladóra</span><span class="sxs-lookup"><span data-stu-id="752f4-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="752f4-104">**A következőkre vonatkozik:**</span><span class="sxs-lookup"><span data-stu-id="752f4-104">**Applies to:**</span></span>
- <span data-ttu-id="752f4-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="752f4-105">Partner Center</span></span>

<span data-ttu-id="752f4-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="752f4-106">**Appropriate roles**</span></span>

- <span data-ttu-id="752f4-107">Minden CSP közvetlen számlázási partner</span><span class="sxs-lookup"><span data-stu-id="752f4-107">All CSP direct bill partners</span></span>

>[!Note]
><span data-ttu-id="752f4-108">Ez a cikk olyan közvetlen számlázási partnerek számára készült, akik úgy döntöttek, hogy áttérnek a közvetett viszonteladók felé.</span><span class="sxs-lookup"><span data-stu-id="752f4-108">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="752f4-109">Ha azonban még nem hozott létre explicit döntést a közvetett viszonteladóként való regisztráláshoz, akkor a Microsoft tájékoztatja a közvetlen számlázást a CSP közvetlen számlázási partneri programjára vonatkozó új [követelmények](direct-partner-new-requirements.md) teljesítéséről, ha a [közvetlen számlázási funkciói korlátozottak](restricted-direct-bill-capabilities.md)lesznek.</span><span class="sxs-lookup"><span data-stu-id="752f4-109">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="752f4-110">Január 2021-én új bevételi követelmény lesz hozzáadva.</span><span class="sxs-lookup"><span data-stu-id="752f4-110">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="752f4-111">A közvetlen számlás partnerként regisztrált partnereknek a felhőalapú megoldás-szolgáltatói program bevételeinek legalább USD $300K kell visszaadniuk az előző 12 hónap során a partner globális fiók szintjén.</span><span class="sxs-lookup"><span data-stu-id="752f4-111">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="752f4-112">A meglévő közvetlen számlázási bérlő használatával regisztrálhat a közvetett viszonteladói programba.</span><span class="sxs-lookup"><span data-stu-id="752f4-112">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="752f4-113">Bevezetés</span><span class="sxs-lookup"><span data-stu-id="752f4-113">Get started</span></span>

1. <span data-ttu-id="752f4-114">Győződjön meg arról, hogy a partneri profil és az MPN-azonosító aktuális.</span><span class="sxs-lookup"><span data-stu-id="752f4-114">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="752f4-115">Jelentkezzen be a partner Centerbe a közvetlen számlázási bérlő globális rendszergazdájaként, amely közvetett viszonteladóra vált.</span><span class="sxs-lookup"><span data-stu-id="752f4-115">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Áttekintés":::

3. <span data-ttu-id="752f4-117">Tekintse át a partner adatait a beléptetési űrlapon.</span><span class="sxs-lookup"><span data-stu-id="752f4-117">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Regisztráljon most":::

4. <span data-ttu-id="752f4-119">Válassza a regisztrálás most lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="752f4-119">Select Enroll now.</span></span> <span data-ttu-id="752f4-120">A közvetett viszonteladó vállalata ugyanazt a HRE-bérlőt fogja használni, amelyet a közvetlen üzleti tevékenységhez használ.</span><span class="sxs-lookup"><span data-stu-id="752f4-120">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="752f4-121">Ezt az új áttérési képességet kezdetben a szeptember és december között megjelenő partnerek számára is elérhetővé teszi.</span><span class="sxs-lookup"><span data-stu-id="752f4-121">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="752f4-122">Ha nem rendelkezik a szeptember és december közötti évfordulós dátummal, akkor a funkció jelenleg nem fog megjelenni.</span><span class="sxs-lookup"><span data-stu-id="752f4-122">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="752f4-123">A december 2018 utáni évfordulós dátummal rendelkező partnereket később értesítjük, amint a funkció engedélyezve van a partnereknek.</span><span class="sxs-lookup"><span data-stu-id="752f4-123">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="752f4-124">A regisztráció jóváhagyása után jelentkezzen be újra a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="752f4-124">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="752f4-125">Habár a jóváhagyás általában azonnali, akár öt munkanapot is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="752f4-125">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="752f4-126">A jóváhagyást követően értesítést kap arról az e-mail címre, amelyet az elsődleges partnernél megadott a beléptetési űrlapon.</span><span class="sxs-lookup"><span data-stu-id="752f4-126">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="752f4-127">A regisztrációs állapotát a **Beállítások**  >  **partner beállításai**  >  **partner profilja** > program adatai területen is megtekintheti.</span><span class="sxs-lookup"><span data-stu-id="752f4-127">You can also check your enrollment status under **Settings** > **Partner Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="752f4-128">Az **Áttekintés** oldalon a közvetett viszonteladói szerződés jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="752f4-128">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="752f4-129">Válassza **az elfogadás és folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="752f4-129">Select **Accept and continue** .</span></span> <span data-ttu-id="752f4-130">Ez a művelet engedélyezi a közvetett viszonteladói képességeket.</span><span class="sxs-lookup"><span data-stu-id="752f4-130">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="752f4-131">Ha elfogadta a közvetett viszonteladói szerződést, figyelje meg, hogy a partner profilja a közvetlen számlát és a közvetett viszonteladót **is** azonosítja.</span><span class="sxs-lookup"><span data-stu-id="752f4-131">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Közvetett viszonteladói szerződés":::

> [!IMPORTANT]
> <span data-ttu-id="752f4-133">Miután regisztrálta magát közvetett viszonteladóként az új képességgel, nincs lehetőség arra, hogy visszaállítson egy közvetlen, csak számlázási bérlőre.</span><span class="sxs-lookup"><span data-stu-id="752f4-133">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="752f4-134">A közvetett viszonteladóként való regisztrálás előtt győződjön meg arról, hogy az üzleti igények teljes körű kiértékelése megtörtént.</span><span class="sxs-lookup"><span data-stu-id="752f4-134">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="752f4-135">A közvetlenről a közvetett viszonteladóra való áttérés közben</span><span class="sxs-lookup"><span data-stu-id="752f4-135">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="752f4-136">Ebben a fázisban továbbra is kezelheti a közvetlen ügyfelek előfizetési igényeit, beleértve a számlázási folyamatot is.</span><span class="sxs-lookup"><span data-stu-id="752f4-136">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="752f4-137">Megkezdheti az ügyfelek fogadását a közvetett szolgáltatótól, és közvetett viszonteladóként is működik.</span><span class="sxs-lookup"><span data-stu-id="752f4-137">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Ön a közvetlen számla és a közvetett viszonteladó is":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="752f4-139">Közvetett szolgáltató keresése</span><span class="sxs-lookup"><span data-stu-id="752f4-139">Find an indirect provider</span></span>

<span data-ttu-id="752f4-140">A regisztráció után a rendszer a bal oldali NAV-ben megjelenik a közvetett szolgáltatókra mutató hivatkozás.</span><span class="sxs-lookup"><span data-stu-id="752f4-140">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="752f4-141">Közvetett viszonteladóként kapcsolatot létesít egy olyan közvetett szolgáltatóval, aki ezt követően kezelheti a számlázási adatait, megvásárolhatja az ügyfeleit, és támogatási infrastruktúrát is használhat.</span><span class="sxs-lookup"><span data-stu-id="752f4-141">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="752f4-142">A különböző közvetett szolgáltatók különböző támogatást és szolgáltatásokat kínálnak, ezért érdemes kiértékelnie, hogy mely szolgáltatók felelnek meg legjobban az igényeinek.</span><span class="sxs-lookup"><span data-stu-id="752f4-142">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="752f4-143">A legtöbb szolgáltató általában a következőket biztosítja:</span><span class="sxs-lookup"><span data-stu-id="752f4-143">Generally, most providers will:</span></span>

- <span data-ttu-id="752f4-144">Technikai képzést és segítséget nyújt</span><span class="sxs-lookup"><span data-stu-id="752f4-144">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="752f4-145">A termékek és szolgáltatások piacra jutásának elősegítése</span><span class="sxs-lookup"><span data-stu-id="752f4-145">Help you market your products and services</span></span>
- <span data-ttu-id="752f4-146">A finanszírozás és a kredit feltételeinek kezelése</span><span class="sxs-lookup"><span data-stu-id="752f4-146">Manage your financing and credit terms</span></span>

<span data-ttu-id="752f4-147">Keresse meg a hivatalos [Microsoft közvetett szolgáltatók](https://partnercenter.microsoft.com/partner/find-a-provider)listáját.</span><span class="sxs-lookup"><span data-stu-id="752f4-147">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="752f4-148">További információ,  [partnerek olvasása közvetett szolgáltatókkal](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="752f4-148">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="752f4-149">Partneri meghívás elfogadása a közvetett szolgáltatótól</span><span class="sxs-lookup"><span data-stu-id="752f4-149">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="752f4-150">Ha megtalál egy közvetett szolgáltatót a partnerrel, a partner Centerben hozzon létre egy kapcsolatot a közvetett szolgáltatóval.</span><span class="sxs-lookup"><span data-stu-id="752f4-150">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="752f4-151">A kiválasztott közvetett szolgáltató e-mailben elküld egy partneri Meghívási hivatkozást, amely elvégzi a meghívót a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="752f4-151">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="752f4-152">Győződjön meg arról, hogy a globális rendszergazda bejelentkezik a partner központba, és követi a Meghívási hivatkozást.</span><span class="sxs-lookup"><span data-stu-id="752f4-152">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="752f4-153">Ha elfogadja a meghívást, a szolgáltató neve megjelenik a közvetett szolgáltatók listájában.</span><span class="sxs-lookup"><span data-stu-id="752f4-153">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="752f4-154">Új ügyfelek megvásárlása közvetett viszonteladóként</span><span class="sxs-lookup"><span data-stu-id="752f4-154">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="752f4-155">Önnek és a közvetett szolgáltatónak is rendelkeznie kell viszonteladói kapcsolattal az ügyfelekkel.</span><span class="sxs-lookup"><span data-stu-id="752f4-155">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="752f4-156">Ezek a viszonteladói kapcsolatok lehetővé teszik az ügyfél előfizetéseit és szolgáltatásait az Ön nevében.</span><span class="sxs-lookup"><span data-stu-id="752f4-156">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="752f4-157">Ha meglévő Azure AD-Bérlővel rendelkező új ügyfelet szeretne beszerezni, meghívhatja az ügyfelet, hogy egyszerre hozzon létre egy viszonteladói kapcsolatot Önnel és a szolgáltatójával is.</span><span class="sxs-lookup"><span data-stu-id="752f4-157">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="752f4-158">Közvetett viszonteladói meghívás létrehozása:</span><span class="sxs-lookup"><span data-stu-id="752f4-158">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="752f4-159">Válassza ki a **közvetlen szolgáltatókat** a partner Center bal oldali NAV-ból.</span><span class="sxs-lookup"><span data-stu-id="752f4-159">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="752f4-160">Válassza az **új ügyfelek meghívása** lehetőséget, hogy meghívjon egy ügyfelet a viszonteladói kapcsolat létrehozására az Önnel és a közvetett szolgáltatóval egyszerre.</span><span class="sxs-lookup"><span data-stu-id="752f4-160">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="752f4-161">A szolgáltatónak viszonteladói kapcsolattal kell rendelkeznie az ügyféllel, így megrendeléseket küldhet az ügyfél nevében, amikor az ügyfél új előfizetéseket szeretne vásárolni, vagy új licenceket szeretne hozzáadni meglévő előfizetésekhez.</span><span class="sxs-lookup"><span data-stu-id="752f4-161">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="752f4-162">A következő lapon tekintse át az e-mail-üzenet piszkozatát.</span><span class="sxs-lookup"><span data-stu-id="752f4-162">On the next page, review the draft email message.</span></span> <span data-ttu-id="752f4-163">E-mailben megnyithatja az üzenet piszkozatát, vagy átmásolhatja az üzenetet a vágólapra, és beillesztheti egy e-mailbe.</span><span class="sxs-lookup"><span data-stu-id="752f4-163">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="752f4-164">Szerkessze az e-mailben szereplő szöveget, hogy megtudja, mire van szüksége, de ügyeljen arra, hogy a hivatkozást a saját fiókjához és a szolgáltató fiókjához való közvetlen csatlakozáshoz is használja.</span><span class="sxs-lookup"><span data-stu-id="752f4-164">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="752f4-165">Ezután válassza a **Done** (Kész) elemet.</span><span class="sxs-lookup"><span data-stu-id="752f4-165">Then select **Done** .</span></span>

5. <span data-ttu-id="752f4-166">Miután az ügyfél felhatalmazza Önt és a szolgáltatót a rekordok viszonteladói számára, rendszergazdai jogosultságokkal fog rendelkezni az előfizetések, a licencek és a felhasználók nevében történő kezeléséhez, és a közvetett szolgáltató elküldheti a megrendeléseket a nevükben.</span><span class="sxs-lookup"><span data-stu-id="752f4-166">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="752f4-167">Az ügyfél fiókjának, szolgáltatásainak, felhasználóinak és licencének kezeléséhez bontsa ki az ügyfél rekordját a neve melletti lefelé mutató nyílra kattintva.</span><span class="sxs-lookup"><span data-stu-id="752f4-167">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="752f4-168">A közvetlen számlázási partnerekkel ellentétben a közvetett viszonteladók nem hozhatnak létre Azure AD-bérlőket az új ügyfelek számára a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="752f4-168">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="752f4-169">A szolgáltató létrehozza a bérlőt, és az ügyfél számára közvetett viszonteladóként fogja megadni.</span><span class="sxs-lookup"><span data-stu-id="752f4-169">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="752f4-170">Ezzel biztosíthatja, hogy az ügyfél megjelenjen a partner Center ügyfél listájában.</span><span class="sxs-lookup"><span data-stu-id="752f4-170">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="752f4-171">Nem fogja tudni használni a közvetlen számlázási képességet arra, hogy vásárlásokat hozzon létre a közvetett viszonteladóként vásárolt ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="752f4-171">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="752f4-172">A közvetlen számlázási ügyfelek és a közvetett viszonteladói ügyfelek kezelése</span><span class="sxs-lookup"><span data-stu-id="752f4-172">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="752f4-173">A közvetlen számlázási ügyfelek és a közvetett viszonteladói ügyfelek különbözőképpen kezelhetők.</span><span class="sxs-lookup"><span data-stu-id="752f4-173">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="752f4-174">Közvetlen számlázási ügyfelek (olyan dolgok, amelyeket nem közvetett viszonteladóként végeznek)</span><span class="sxs-lookup"><span data-stu-id="752f4-174">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="752f4-175">Termékek rendelésének létrehozása</span><span class="sxs-lookup"><span data-stu-id="752f4-175">Create orders for products</span></span>
- <span data-ttu-id="752f4-176">Az Azure Reservations kezelése</span><span class="sxs-lookup"><span data-stu-id="752f4-176">Manage Azure reservations</span></span>
- <span data-ttu-id="752f4-177">A sorrend előzményeinek kezelése</span><span class="sxs-lookup"><span data-stu-id="752f4-177">Manage their order history</span></span>
- <span data-ttu-id="752f4-178">Szoftver vásárlása</span><span class="sxs-lookup"><span data-stu-id="752f4-178">Purchase software</span></span>
- <span data-ttu-id="752f4-179">Ügyfelek közvetlen számlázása</span><span class="sxs-lookup"><span data-stu-id="752f4-179">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="752f4-180">Közvetett viszonteladói ügyfelek</span><span class="sxs-lookup"><span data-stu-id="752f4-180">Indirect reseller customers</span></span>

- <span data-ttu-id="752f4-181">A közvetett szolgáltató a termékeket az ügyfelek számára rendeli</span><span class="sxs-lookup"><span data-stu-id="752f4-181">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="752f4-182">Ügyfelek licencek és felhasználók kezelése</span><span class="sxs-lookup"><span data-stu-id="752f4-182">Manage customers' licenses and users</span></span>
- <span data-ttu-id="752f4-183">Az előfizetés megújításának kezelése</span><span class="sxs-lookup"><span data-stu-id="752f4-183">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="752f4-184">A közvetlen számlázási partnernek beszerzett ügyfelek azonosítása</span><span class="sxs-lookup"><span data-stu-id="752f4-184">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="752f4-185">**Ügyfelek** kiválasztása</span><span class="sxs-lookup"><span data-stu-id="752f4-185">Select **Customers**</span></span>

2. <span data-ttu-id="752f4-186">Válasszon ki egy ügyfelet a részletek megtekintéséhez</span><span class="sxs-lookup"><span data-stu-id="752f4-186">Select a customer to view their details</span></span>

3. <span data-ttu-id="752f4-187">Ha ezt az ügyfelet közvetlen számlás partnerként szerezte be, akkor a termékek **hozzáadásával** vagy **megtekintésével** kapcsolatos lehetőségek jelennek meg, és látni fogja az előfizetéseit.</span><span class="sxs-lookup"><span data-stu-id="752f4-187">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="752f4-188">Ha az ügyfél közvetett viszonteladói kapcsolattal rendelkezik Önnel, ezek a beállítások nem lesznek elérhetők.</span><span class="sxs-lookup"><span data-stu-id="752f4-188">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="752f4-189">Közvetlen számlázási ügyfelek áthelyezése a közvetett szolgáltatóba</span><span class="sxs-lookup"><span data-stu-id="752f4-189">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="752f4-190">A közvetett szolgáltató nem tud megrendeléseket vagy meglévő előfizetéseket beküldeni a meglévő közvetlen számlázási ügyfeleinek, amíg nem rendelkeznek viszonteladói kapcsolattal.</span><span class="sxs-lookup"><span data-stu-id="752f4-190">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="752f4-191">A közvetett szolgáltató és a meglévő közvetlen számlázási ügyfél közötti viszonteladói kapcsolat létrehozásához az alábbi módszerek egyikét használhatja:</span><span class="sxs-lookup"><span data-stu-id="752f4-191">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="752f4-192">Viszonteladói kapcsolat kiterjesztése</span><span class="sxs-lookup"><span data-stu-id="752f4-192">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="752f4-193">Közvetett viszonteladói Meghívás küldése az ügyfélnek</span><span class="sxs-lookup"><span data-stu-id="752f4-193">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="752f4-194">Részletes áttekintést kaphat a [közvetlen és a közvetett áttérési dokumentum](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/) lépésenkénti folyamatáról</span><span class="sxs-lookup"><span data-stu-id="752f4-194">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="752f4-195">Viszonteladói kapcsolat kiterjesztése</span><span class="sxs-lookup"><span data-stu-id="752f4-195">Reseller relationship extension</span></span>

<span data-ttu-id="752f4-196">A viszonteladói kapcsolat kiterjesztése funkcióval viszonteladói kapcsolatot létesíthet a meglévő közvetlen számlázási ügyfelek és a közvetett szolgáltató között a partner Center irányítópult használatával.</span><span class="sxs-lookup"><span data-stu-id="752f4-196">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="752f4-197">A funkció használata előtt vegye figyelembe a következőket:</span><span class="sxs-lookup"><span data-stu-id="752f4-197">Before using the feature, note the following:</span></span>

- <span data-ttu-id="752f4-198">Ez a funkció csak olyan közvetlen számlázási partnerek számára érhető el, akik közvetett viszonteladóként váltanak át, és elvégezték a [közvetett viszonteladói regisztrációt](#get-started).</span><span class="sxs-lookup"><span data-stu-id="752f4-198">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="752f4-199">Ezt a funkciót csak a meglévő közvetlen számlázási ügyfelekre lehet alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="752f4-199">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="752f4-200">Nem alkalmazható a [közvetett viszonteladói ügyfeleknek](#acquire-new-customers-as-indirect-reseller).</span><span class="sxs-lookup"><span data-stu-id="752f4-200">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="752f4-201">Csak olyan közvetett szolgáltatót választhat ki, amelyhez [elfogadta a közvetett szolgáltatótól érkező partneri meghívást](#accept-a-partnership-invitation-from-your-indirect-provider).</span><span class="sxs-lookup"><span data-stu-id="752f4-201">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="752f4-202">Az ügyfélhez tartozó számlázási adatok másolata elérhetővé válik a közvetett szolgáltató számára.</span><span class="sxs-lookup"><span data-stu-id="752f4-202">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="752f4-203">A számlázási adatokat úgy érheti el, ha hozzáfér az ügyfélhez a partner Center irányítópultján.</span><span class="sxs-lookup"><span data-stu-id="752f4-203">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="752f4-204">A viszonteladói kapcsolat kiterjesztése funkcióval beleegyezik, hogy megosztja az ügyfélhez tartozó számlázási adatokat a közvetett szolgáltatóval.</span><span class="sxs-lookup"><span data-stu-id="752f4-204">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="752f4-205">A közvetett szolgáltató nem lesz biztosítva [delegált rendszergazdai jogosultságokkal](customers-revoke-admin-privileges.md) az ügyfél bérlője számára.</span><span class="sxs-lookup"><span data-stu-id="752f4-205">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="752f4-206">Ha a közvetett szolgáltató delegált rendszergazdai jogosultságokat igényel, akkor ehelyett egy közvetett viszonteladói meghívót kell küldenie az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="752f4-206">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="752f4-207">A viszonteladói kapcsolat létrejötte után a közvetett szolgáltató CSP-partnerként fog megjelenni az ügyfél számára a [M365 felügyeleti központ](https://admin.microsoft.com/AdminPortal/Home#/partners) partner kapcsolatok lapján, valamint [a vállalati Microsoft Store](/microsoft-store/work-with-partner-microsoft-store-business).</span><span class="sxs-lookup"><span data-stu-id="752f4-207">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="752f4-208">A félreértések és a félreértések elkerülése érdekében a partneri szerződése arra kötelezi Önt, hogy tájékoztassa és szerezzen be hozzájárulást a közvetlen számlázási ügyféltől, mielőtt a kapcsolati bővítményt használja a meglévő közvetlen számlázási ügyfél és a közvetett szolgáltató közötti viszonteladói kapcsolat létesítéséhez.</span><span class="sxs-lookup"><span data-stu-id="752f4-208">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="752f4-209">A szolgáltatás használata meglévő ügyfél-bérlőn:</span><span class="sxs-lookup"><span data-stu-id="752f4-209">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="752f4-210">Jelentkezzen be a partner Centerbe **rendszergazdai ügynökként** .</span><span class="sxs-lookup"><span data-stu-id="752f4-210">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="752f4-211">Az **ügyfelek lapon** válasszon ki egy meglévő ügyfelet, és kattintson a **gyors hivatkozások** ikonjára az ügyfél összefoglaló nézetének kibontásához.</span><span class="sxs-lookup"><span data-stu-id="752f4-211">In the **Customers page** , select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="752f4-212">A **közvetett szolgáltató (k)** alatt kattintson **az ügyfél átvitele közvetett szolgáltatóra** elemre.</span><span class="sxs-lookup"><span data-stu-id="752f4-212">Under **Indirect provider(s)** , click **Transfer customer on an indirect provider** .</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Ügyfél átvitele közvetett szolgáltatóba":::

4. <span data-ttu-id="752f4-214">Az előugró ablakban válassza ki azt a **közvetett szolgáltatót** , amelyhez viszonteladói kapcsolatot szeretne adni az ügyféllel.</span><span class="sxs-lookup"><span data-stu-id="752f4-214">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="752f4-215">Kattintson **a Mentés és folytatás** gombra.</span><span class="sxs-lookup"><span data-stu-id="752f4-215">Click **Save and continue** .</span></span>

6. <span data-ttu-id="752f4-216">Ellenőrizze, hogy a kiválasztott közvetett szolgáltató megjelenik **-e a közvetett szolgáltató (k)** alatt.</span><span class="sxs-lookup"><span data-stu-id="752f4-216">Verify the selected indirect provider shows up under **Indirect provider(s)** .</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Közvetett szolgáltató listázva":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="752f4-218">Közvetett viszonteladói Meghívás küldése az ügyfélnek</span><span class="sxs-lookup"><span data-stu-id="752f4-218">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="752f4-219">A közvetett szolgáltató nem tud megrendeléseket beküldeni meglévő közvetlen számlázási ügyfeleinek, amíg nem rendelkeznek viszonteladói kapcsolattal.</span><span class="sxs-lookup"><span data-stu-id="752f4-219">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="752f4-220">Ha a viszonteladói kapcsolatot a meglévő ügyfelek és a közvetett szolgáltató között szeretné létrehozni, hívja meg az ügyfelet egy közvetett viszonteladó meghívásával.</span><span class="sxs-lookup"><span data-stu-id="752f4-220">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="752f4-221">Válassza ki a **közvetlen szolgáltatókat** a partner Center bal oldali NAV-ból.</span><span class="sxs-lookup"><span data-stu-id="752f4-221">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="752f4-222">Válassza az **új ügyfelek meghívása** lehetőséget, hogy meghívjon egy ügyfelet a viszonteladói kapcsolat létrehozására az Önnel és a közvetett szolgáltatóval egyszerre.</span><span class="sxs-lookup"><span data-stu-id="752f4-222">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="752f4-223">A szolgáltatónak viszonteladói kapcsolattal kell rendelkeznie az ügyféllel, így megrendeléseket küldhet az ügyfél nevében, amikor az ügyfél új előfizetéseket szeretne vásárolni, vagy új licenceket szeretne hozzáadni meglévő előfizetésekhez.</span><span class="sxs-lookup"><span data-stu-id="752f4-223">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Új ügyfelek meghívása":::

3. <span data-ttu-id="752f4-225">A következő lapon tekintse át az e-mail-üzenet piszkozatát.</span><span class="sxs-lookup"><span data-stu-id="752f4-225">On the next page, review the draft email message.</span></span> <span data-ttu-id="752f4-226">E-mailben megnyithatja az üzenet piszkozatát, vagy átmásolhatja az üzenetet a vágólapra, és beillesztheti egy e-mailbe.</span><span class="sxs-lookup"><span data-stu-id="752f4-226">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="752f4-227">Szerkessze az e-mailben szereplő szöveget, hogy megtudja, mire van szüksége, de ügyeljen arra, hogy a hivatkozást a saját fiókjához és a szolgáltató fiókjához való közvetlen csatlakozáshoz is használja.</span><span class="sxs-lookup"><span data-stu-id="752f4-227">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="752f4-228">Ezután válassza a **Done** (Kész) elemet.</span><span class="sxs-lookup"><span data-stu-id="752f4-228">Then select **Done** .</span></span>

5. <span data-ttu-id="752f4-229">Miután az ügyfél felhatalmazza Önt és a szolgáltatót a rekordok viszonteladói számára, rendszergazdai jogosultságokkal fog rendelkezni az előfizetések, a licencek és a felhasználók nevében történő kezeléséhez, és a közvetett szolgáltató elküldheti a megrendeléseket a nevükben.</span><span class="sxs-lookup"><span data-stu-id="752f4-229">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="752f4-230">Az ügyfél fiókjának, szolgáltatásainak, felhasználóinak és licencének kezeléséhez bontsa ki az ügyfél rekordját a neve melletti lefelé mutató nyílra kattintva.</span><span class="sxs-lookup"><span data-stu-id="752f4-230">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="752f4-231">Microsoft Customer Agreement elfogadás</span><span class="sxs-lookup"><span data-stu-id="752f4-231">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="752f4-232">Microsoft Cloud szerződés 2020. január 31-ig érvényes.</span><span class="sxs-lookup"><span data-stu-id="752f4-232">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="752f4-233">Ezt követően az összes ügyfélnek, a meglévőknek és az új felhasználóknak alá kell írnia az új [Microsoft ügyfél-szerződést](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="752f4-233">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="752f4-234">Az ügyfelek átváltásához, ha:</span><span class="sxs-lookup"><span data-stu-id="752f4-234">For transitioning customers, if:</span></span>

- <span data-ttu-id="752f4-235">**Az ügyfél még nem fogadta el a Microsoft Customer szerződést**</span><span class="sxs-lookup"><span data-stu-id="752f4-235">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="752f4-236">Forduljon a közvetett szolgáltatóhoz, hogy [az ügyfelek elfogadják a Microsoft ügyfél-szerződést](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="752f4-236">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="752f4-237">**Az ügyfél elfogadta a Microsoft ügyfél-szerződést a Microsoft 365 felügyeleti központban**</span><span class="sxs-lookup"><span data-stu-id="752f4-237">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="752f4-238">A rendszer megőrzi az elfogadást, miután a viszonteladói kapcsolat létrejött a közvetett szolgáltatóval.</span><span class="sxs-lookup"><span data-stu-id="752f4-238">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="752f4-239">Semmit nem kell tennie.</span><span class="sxs-lookup"><span data-stu-id="752f4-239">There is nothing you need to do.</span></span>

- <span data-ttu-id="752f4-240">**Az ügyfél elfogadta a Microsoft ügyfél-szerződését a partneri igazoláson keresztül**</span><span class="sxs-lookup"><span data-stu-id="752f4-240">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="752f4-241">Az elfogadást nem őrzi meg a rendszer.</span><span class="sxs-lookup"><span data-stu-id="752f4-241">The acceptance will not be retained.</span></span> <span data-ttu-id="752f4-242">Forduljon a közvetett szolgáltatóhoz, és [frissítse az ügyfél elfogadását a partner Centerben](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span><span class="sxs-lookup"><span data-stu-id="752f4-242">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="752f4-243">Meglévő közvetlen számlázási előfizetések átvitele közvetett szolgáltatóba</span><span class="sxs-lookup"><span data-stu-id="752f4-243">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="752f4-244">A CSP közvetett modellben a közvetett viszonteladók nem rendelkeznek számlázási kapcsolattal a Microsofttal.</span><span class="sxs-lookup"><span data-stu-id="752f4-244">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="752f4-245">Ehelyett a közvetett viszonteladók előfizetéseket szereznek be ügyfeleiknek a közvetett szolgáltatókon keresztül.</span><span class="sxs-lookup"><span data-stu-id="752f4-245">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="752f4-246">A közvetlen számlázási partnertől a közvetett viszonteladóig történő áttérés során át kell adnia a meglévő előfizetéseket, amelyek közvetlen számlás partnere a közvetett szolgáltatónak.</span><span class="sxs-lookup"><span data-stu-id="752f4-246">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="752f4-247">A partner Center irányítópultján használhatja a saját kiszolgálású előfizetés-átvitel funkciót.</span><span class="sxs-lookup"><span data-stu-id="752f4-247">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="752f4-248">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="752f4-248">Pre-requisites</span></span>

- <span data-ttu-id="752f4-249">Ez a funkció csak olyan partnereink átváltására használható, akik a közvetett viszonteladói regisztrációt elvégezték meglévő közvetlen számlázási partner-bérlőik használatával</span><span class="sxs-lookup"><span data-stu-id="752f4-249">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants</span></span>

- <span data-ttu-id="752f4-250">Egy adott ügyfélhez társított előfizetések továbbítása előtt az áttérési partnernek át kell helyeznie az ügyfelet egy közvetett szolgáltatóra.</span><span class="sxs-lookup"><span data-stu-id="752f4-250">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="752f4-251">Az ügyfélnek [a közvetett szolgáltatón keresztül el kell fogadnia a Microsoft ügyfél-szerződését](#microsoft-customer-agreement-acceptance).</span><span class="sxs-lookup"><span data-stu-id="752f4-251">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="752f4-252">Áttérés a közvetett viszonteladói állapotra</span><span class="sxs-lookup"><span data-stu-id="752f4-252">How to transition to indirect reseller status</span></span>

<span data-ttu-id="752f4-253">A szolgáltatás egy 4 lépésből álló folyamat, ahol:</span><span class="sxs-lookup"><span data-stu-id="752f4-253">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="752f4-254">Az áttérési partner létrehoz egy előfizetés-átadási kérelmet.</span><span class="sxs-lookup"><span data-stu-id="752f4-254">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="752f4-255">A kérelem egy vagy több olyan meglévő előfizetést tartalmaz, amely ugyanahhoz az ügyfélhez van társítva, és egy közvetett szolgáltatóhoz van rendelve.</span><span class="sxs-lookup"><span data-stu-id="752f4-255">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="752f4-256">A közvetett szolgáltató áttekinti és elfogadja (vagy elutasítja) az átvitelre vonatkozó kérelmet.</span><span class="sxs-lookup"><span data-stu-id="752f4-256">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="752f4-257">A közvetett szolgáltató ellenőrzi, hogy befejeződött-e az átviteli kérelem.</span><span class="sxs-lookup"><span data-stu-id="752f4-257">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="752f4-258">Az áttérési partner ellenőrzi, hogy befejeződött-e az átviteli kérelem.</span><span class="sxs-lookup"><span data-stu-id="752f4-258">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="752f4-259">Átállási partner</span><span class="sxs-lookup"><span data-stu-id="752f4-259">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="752f4-260">A [partner Center API/SDK](/partner-center/develop/manage-customers) használatával is átviheti a meglévő előfizetéseket a közvetett szolgáltatóba.</span><span class="sxs-lookup"><span data-stu-id="752f4-260">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="752f4-261">Ügyfél-előfizetések áthelyezési jogosultságának beszerzése</span><span class="sxs-lookup"><span data-stu-id="752f4-261">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="752f4-262">Ügyfél átvitelének létrehozása</span><span class="sxs-lookup"><span data-stu-id="752f4-262">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="752f4-263">Ügyfél átvitelének visszavonása</span><span class="sxs-lookup"><span data-stu-id="752f4-263">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="752f4-264">Ügyfél átvitelének elfogadása</span><span class="sxs-lookup"><span data-stu-id="752f4-264">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="752f4-265">Ügyfél átvitelének elutasítása</span><span class="sxs-lookup"><span data-stu-id="752f4-265">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="752f4-266">Ügyfél-átutalások beszerzése</span><span class="sxs-lookup"><span data-stu-id="752f4-266">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="752f4-267">Adatátviteli adatok beolvasása azonosító alapján</span><span class="sxs-lookup"><span data-stu-id="752f4-267">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="752f4-268">Áttérés a partnernek – átviteli kérelem létrehozása</span><span class="sxs-lookup"><span data-stu-id="752f4-268">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="752f4-269">Átviteli kérelem létrehozása áttérési partnerként:</span><span class="sxs-lookup"><span data-stu-id="752f4-269">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="752f4-270">Jelentkezzen be a partner Centerbe **rendszergazdai ügynökként** .</span><span class="sxs-lookup"><span data-stu-id="752f4-270">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="752f4-271">Az **ügyfelek** lapon válassza ki a kívánt ügyfelet, majd kattintson a gyors hivatkozások ikonra az ügyfél összefoglaló nézetének kibontásához.</span><span class="sxs-lookup"><span data-stu-id="752f4-271">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="752f4-272">A **közvetett szolgáltató (k)** alatt ellenőrizze, hogy szerepel-e a kívánt közvetett szolgáltató.</span><span class="sxs-lookup"><span data-stu-id="752f4-272">Under **Indirect provider(s)** , confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="752f4-273">Kattintson az **előfizetések megtekintése** elemre.</span><span class="sxs-lookup"><span data-stu-id="752f4-273">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="752f4-274">Az **előfizetések** oldalon keresse meg az **előfizetés átvitelét** .</span><span class="sxs-lookup"><span data-stu-id="752f4-274">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

6. <span data-ttu-id="752f4-275">Az **előfizetés átvitele** területen kattintson az **előfizetés-átvitel kérése** elemre.</span><span class="sxs-lookup"><span data-stu-id="752f4-275">Under **Subscription Transfer** , click **Request subscription transfer** .</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Előfizetés-átvitel kérése":::

7. <span data-ttu-id="752f4-277">Az átadási kérelem párbeszédpanelen válasszon ki egy vagy több átvinni kívánt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="752f4-277">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Adatátviteli kérelem létrehozása":::

8. <span data-ttu-id="752f4-279">Kattintson a **Létrehozás** gombra.</span><span class="sxs-lookup"><span data-stu-id="752f4-279">Click **Create** .</span></span>

9. <span data-ttu-id="752f4-280">Az **előfizetés átvitele** alatt megjelenik egy aktív előfizetés-átvételi kérelem.</span><span class="sxs-lookup"><span data-stu-id="752f4-280">An active subscription transfer request will appear under **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Adatátviteli kérelmek listája":::

10. <span data-ttu-id="752f4-282">Tájékoztassa a közvetett szolgáltatót arról, hogy létrehozott egy előfizetés-áthelyezési kérelmet.</span><span class="sxs-lookup"><span data-stu-id="752f4-282">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="752f4-283">Közvetett szolgáltató – adatátviteli kérelem elfogadása</span><span class="sxs-lookup"><span data-stu-id="752f4-283">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="752f4-284">Adatátviteli kérelem felülvizsgálata és elfogadása közvetett szolgáltatóként:</span><span class="sxs-lookup"><span data-stu-id="752f4-284">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="752f4-285">Jelentkezzen be a partner központjába **rendszergazdai** ügynökként vagy **értékesítési ügynökként** .</span><span class="sxs-lookup"><span data-stu-id="752f4-285">Log in to Partner Center as an **Admin** Agent or **Sales Agent** .</span></span>

2. <span data-ttu-id="752f4-286">Az **ügyfelek** lapon válassza ki a kívánt ügyfelet, majd kattintson a gyors hivatkozások ikonjára az ügyfél összefoglaló nézetének kibontásához.</span><span class="sxs-lookup"><span data-stu-id="752f4-286">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="752f4-287">A **közvetett viszonteladó (k)** alatt ellenőrizze, hogy szerepel-e az áttérési partner.</span><span class="sxs-lookup"><span data-stu-id="752f4-287">Under **Indirect reseller(s)** , confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="752f4-288">Kattintson az **előfizetések megtekintése** elemre.</span><span class="sxs-lookup"><span data-stu-id="752f4-288">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="752f4-289">Az **előfizetések** oldalon keresse meg az **előfizetés átvitelét** .</span><span class="sxs-lookup"><span data-stu-id="752f4-289">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Adatátviteli kérelem megtekintése":::

6. <span data-ttu-id="752f4-291">Az **előfizetés átvitele** területen kattintson a felülvizsgálati kérelemre.</span><span class="sxs-lookup"><span data-stu-id="752f4-291">Under **Subscription Transfer** , click on the transfer request to review.</span></span>

7. <span data-ttu-id="752f4-292">Szükség szerint kattintson az **elfogadás** (vagy **elutasítás** ) lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="752f4-292">Click **Accept** (or **Reject** ) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Adatátviteli kérelem elfogadása":::

8. <span data-ttu-id="752f4-294">Várjon, amíg az átviteli kérelem befejeződik.</span><span class="sxs-lookup"><span data-stu-id="752f4-294">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="752f4-295">Közvetett szolgáltató – az adatátviteli kérelem ellenőrzése befejeződött</span><span class="sxs-lookup"><span data-stu-id="752f4-295">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="752f4-296">Az áttelepítési kérelem sikeres befejeződése után ellenőrizze, hogy látható-e az előfizetések az **előfizetések** területen.</span><span class="sxs-lookup"><span data-stu-id="752f4-296">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions** .</span></span>

2. <span data-ttu-id="752f4-297">Tájékoztassa az átállási partnert.</span><span class="sxs-lookup"><span data-stu-id="752f4-297">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="752f4-298">Átállási partner – az átadási kérelem ellenőrzése befejeződött</span><span class="sxs-lookup"><span data-stu-id="752f4-298">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="752f4-299">Az átállási partnernek a következőket kell tennie:</span><span class="sxs-lookup"><span data-stu-id="752f4-299">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="752f4-300">Jelentkezzen be a partner Centerbe **rendszergazdai ügynökként** vagy **értékesítési ügynökként** .</span><span class="sxs-lookup"><span data-stu-id="752f4-300">Sign into Partner Center as an **Admin Agent** or **Sales Agent** .</span></span>

2. <span data-ttu-id="752f4-301">Az **ügyfelek** lapon válassza ki a kívánt ügyfelet, majd kattintson a **gyors hivatkozások** ikonra az ügyfél összefoglaló nézetének kibontásához.</span><span class="sxs-lookup"><span data-stu-id="752f4-301">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="752f4-302">Kattintson az **előfizetések megtekintése** elemre.</span><span class="sxs-lookup"><span data-stu-id="752f4-302">Click **View Subscriptions** .</span></span>

4. <span data-ttu-id="752f4-303">Az **előfizetések** oldalon keresse meg az **előfizetés átvitelét** .</span><span class="sxs-lookup"><span data-stu-id="752f4-303">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

5. <span data-ttu-id="752f4-304">Ellenőrizze, hogy az átviteli kérelem **készként** van-e megjelölve.</span><span class="sxs-lookup"><span data-stu-id="752f4-304">Verify that the transfer request is marked as **Complete** .</span></span>

6. <span data-ttu-id="752f4-305">Ellenőrizze, hogy az előfizetés (ek) már nem jelennek-e meg aktívként az **előfizetések** oldalán:</span><span class="sxs-lookup"><span data-stu-id="752f4-305">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="752f4-306">Ha ez egy Azure-előfizetés (MS-AZR-0145P), akkor a továbbiakban nem jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="752f4-306">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="752f4-307">Ha ez egy licenc-alapú előfizetés (Office 365, Dynamics, Intune), akkor a rendszer **felfüggesztve** állapotba sorolja.</span><span class="sxs-lookup"><span data-stu-id="752f4-307">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended** .</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Előfizetés felfüggesztve":::

### <a name="considerations"></a><span data-ttu-id="752f4-309">Megfontolandó szempontok</span><span class="sxs-lookup"><span data-stu-id="752f4-309">Considerations</span></span>

- <span data-ttu-id="752f4-310">**Az előfizetés-azonosító eltérő lesz az átvitel után.**</span><span class="sxs-lookup"><span data-stu-id="752f4-310">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="752f4-311">Ha ez egy Azure-előfizetés (MS-AZR-0145P), akkor az Azure-előfizetés AZONOSÍTÓját fogja tartalmazni, amely az előző tulajdonostól megőrzött, és az Azure felügyeleti portálján fog megjelenni.</span><span class="sxs-lookup"><span data-stu-id="752f4-311">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="752f4-312">**Ugyanezt az előfizetést nem lehet több adatátviteli kérelemre hivatkozni.**</span><span class="sxs-lookup"><span data-stu-id="752f4-312">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="752f4-313">Miután létrehozta az adatátviteli kérelmet, amely tartalmaz egy meglévő előfizetést, nem hozhat létre további adatátviteli kéréseket, beleértve ugyanazt az előfizetést, amíg meg nem szakítja az első adatátviteli kérést.</span><span class="sxs-lookup"><span data-stu-id="752f4-313">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="752f4-314">**A licenc alapú előfizetésekhez tartozó bővítményeket az alap előfizetésével együtt kell továbbítani.**</span><span class="sxs-lookup"><span data-stu-id="752f4-314">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="752f4-315">Átadási kérelem létrehozásakor, ha egy vagy több bővítménnyel rendelkező meglévő előfizetést választ, a bővítmények automatikusan szerepelni fognak az átviteli kérelemben.</span><span class="sxs-lookup"><span data-stu-id="752f4-315">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="752f4-316">**Az előfizetéshez tartozó licencek számának változása nem jelenik meg a meglévő átadási kérelemben.**</span><span class="sxs-lookup"><span data-stu-id="752f4-316">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="752f4-317">A meglévő előfizetést tartalmazó átviteli kérelem létrehozása után ne frissítse az előfizetés (vagy a társított bővítmények) licencének mennyiségét.</span><span class="sxs-lookup"><span data-stu-id="752f4-317">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="752f4-318">Ha így tesz, az új mennyiség nem jelenik meg az átviteli kérelemben.</span><span class="sxs-lookup"><span data-stu-id="752f4-318">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="752f4-319">Miután a közvetett szolgáltató elfogadja az átmozgatási kérelmet, az eredő előfizetés a régi mennyiséget fogja tartalmazni.</span><span class="sxs-lookup"><span data-stu-id="752f4-319">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="752f4-320">Ha szeretné, hogy az új mennyiség átkerüljön a közvetett szolgáltatóba, meg kell szüntetnie a meglévő átadási kérelmet, és újra létre kell hoznia egy újat.</span><span class="sxs-lookup"><span data-stu-id="752f4-320">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="752f4-321">**Nem minden vásárlást lehet átvinni az önkiszolgáló előfizetés-átvitel használatával.**</span><span class="sxs-lookup"><span data-stu-id="752f4-321">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="752f4-322">Jelenleg csak a O365-előfizetések és az Azure TB-előfizetések (MS-AZR-0145P) helyezhetők át ezzel a szolgáltatással.</span><span class="sxs-lookup"><span data-stu-id="752f4-322">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="752f4-323">Egyéb vásárlások, például Azure-csomagok, Azure-beli fenntartott példányok, időszakos előfizetés és SaaS-előfizetések az Azure Marketplace-en nem támogatottak.</span><span class="sxs-lookup"><span data-stu-id="752f4-323">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="752f4-324">Itt láthatja, hogy miért nem lehet átvinni egy előfizetést az átadási kérelem elküldése oldalon.</span><span class="sxs-lookup"><span data-stu-id="752f4-324">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="752f4-325">Az előfizetések átviteléhez le kell [mondania a meglévő előfizetést](create-a-new-subscription.md#suspend-or-cancel-a-subscription) , és új ajánlatot kell vásárolnia az ügyfélnek a közvetett szolgáltatón keresztül.</span><span class="sxs-lookup"><span data-stu-id="752f4-325">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="752f4-326">**Nem tesztelhető a homokozó környezet használatával.**</span><span class="sxs-lookup"><span data-stu-id="752f4-326">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="752f4-327">Közvetett viszonteladói ösztönzők regisztrálása</span><span class="sxs-lookup"><span data-stu-id="752f4-327">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="752f4-328">Miután sikeresen regisztrálta magát közvetett viszonteladóként a meglévő közvetlen számlás partneri bérlőn, a rendszer 30 napon belül meghívót kap a közvetett viszonteladói ösztönzők regisztrálására.</span><span class="sxs-lookup"><span data-stu-id="752f4-328">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="752f4-329">A meghívás azon a partner MPN-fiókon alapul, amely jelenleg a CSP-partner bérlőhöz van társítva.</span><span class="sxs-lookup"><span data-stu-id="752f4-329">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="752f4-330">A rendszer elküldi a meghívót a partner MPN-fiókhoz társított e-mail-címre.</span><span class="sxs-lookup"><span data-stu-id="752f4-330">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="752f4-331">Jogosult arra is, hogy a közvetlen számlázási ösztönző programokat is regisztrálja ugyanazzal a partner Bérlővel.</span><span class="sxs-lookup"><span data-stu-id="752f4-331">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="752f4-332">A programokat külön kell kezelnie.</span><span class="sxs-lookup"><span data-stu-id="752f4-332">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="752f4-333">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="752f4-333">Next steps</span></span>

- [<span data-ttu-id="752f4-334">További információ a közvetett viszonteladók kiválásáról</span><span class="sxs-lookup"><span data-stu-id="752f4-334">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="752f4-335">CSP közvetlen partner új követelmények</span><span class="sxs-lookup"><span data-stu-id="752f4-335">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="752f4-336">Korlátozott közvetlen számlázási képességek</span><span class="sxs-lookup"><span data-stu-id="752f4-336">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)