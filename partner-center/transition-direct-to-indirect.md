---
title: Közvetlen számlázási partner váltása közvetett viszonteladóra
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan használhatnak a CSP-programpartnerek Partnerközpont a közvetlen számlázási partnerről a közvetett viszonteladóra való áttéréshez.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e57c4a5d0a02079e887b38fa9754d276062d20cc
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276416"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="40c28-103">Váltás egy közvetlen felhőszolgáltatói (Cloud Solution Provider, CSP-) számlázási partnerről egy közvetett CSP-viszonteladóra</span><span class="sxs-lookup"><span data-stu-id="40c28-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="40c28-104">**Megfelelő szerepkörök:** Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="40c28-104">**Appropriate roles**: Global admin</span></span>

>[!Note]
><span data-ttu-id="40c28-105">Ez a cikk olyan közvetlen számlázási partnerek számára lett szánva, akik úgy döntöttek, hogy áttűnnek közvetett viszonteladókra.</span><span class="sxs-lookup"><span data-stu-id="40c28-105">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="40c28-106">Azonban a Microsoft akkor is értesíti a Microsoftot, ha még nem hozott explicit döntést [](direct-partner-new-requirements.md) közvetett viszonteladóként való regisztrációról, a közvetlen számlázási partnerek, akik nem teljesítik a CSP közvetlen számlázási partnerprogramjának új követelményeit, a Microsoft értesítést kap, ha a közvetlen számlázási képességeik korlátozva [lesznek.](restricted-direct-bill-capabilities.md)</span><span class="sxs-lookup"><span data-stu-id="40c28-106">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="40c28-107">2021 januárjában új bevételi követelményt adunk hozzá.</span><span class="sxs-lookup"><span data-stu-id="40c28-107">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="40c28-108">A közvetlen számlázási partnerként regisztrált partnereknek legalább 300 000 USD összegű tranzakciót kell elenyük legalább 300 000 USD összegű, Felhőszolgáltató globális partnerfiókszinten az előző 12 hónapra vonatkozó program bevételében.</span><span class="sxs-lookup"><span data-stu-id="40c28-108">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="40c28-109">Regisztrálható lesz a közvetett viszonteladói programban a meglévő közvetlen számlázási bérlő használatával.</span><span class="sxs-lookup"><span data-stu-id="40c28-109">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="40c28-110">Bevezetés</span><span class="sxs-lookup"><span data-stu-id="40c28-110">Get started</span></span>

1. <span data-ttu-id="40c28-111">Győződjön meg arról, hogy a Partnerközpont és MPN-azonosítóban lévő partnerprofil aktuális.</span><span class="sxs-lookup"><span data-stu-id="40c28-111">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="40c28-112">Jelentkezzen be Partnerközpont a közvetett viszonteladóra áttűnés közvetlen számlázási bérlő globális rendszergazdájaként.</span><span class="sxs-lookup"><span data-stu-id="40c28-112">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Áttekintés.":::

3. <span data-ttu-id="40c28-114">Tekintse át a partner adatait a regisztrációs űrlapon.</span><span class="sxs-lookup"><span data-stu-id="40c28-114">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Regisztráljon most.":::

4. <span data-ttu-id="40c28-116">Válassza a Regisztráció most lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="40c28-116">Select Enroll now.</span></span> <span data-ttu-id="40c28-117">A közvetett viszonteladói üzlet ugyanazt az AAD-bérlőt fogja használni, mint a közvetlen üzletéhez.</span><span class="sxs-lookup"><span data-stu-id="40c28-117">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="40c28-118">Ez az új áttűnés funkció kezdetben a szeptembertől decemberig évfordulós dátumokkal rendelkező partnerek számára lesz elérhető.</span><span class="sxs-lookup"><span data-stu-id="40c28-118">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="40c28-119">Ha nincs évfordulója szeptember és december között, akkor a funkció jelenleg nem látható.</span><span class="sxs-lookup"><span data-stu-id="40c28-119">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="40c28-120">A 2018 decembere utáni évfordulós dátumokkal rendelkező partnerekről később értesítést kap, ha a funkció engedélyezve van a partnerek számára.</span><span class="sxs-lookup"><span data-stu-id="40c28-120">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="40c28-121">A regisztráció jóváhagyása után jelentkezzen be újra a Partnerközpont igényléshez.</span><span class="sxs-lookup"><span data-stu-id="40c28-121">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="40c28-122">Bár a jóváhagyás általában azonnali, akár öt munkanapot is el is vehet.</span><span class="sxs-lookup"><span data-stu-id="40c28-122">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="40c28-123">Jóváhagyás után értesítést kap a regisztrációs űrlap elsődleges kapcsolattartója alatt megadott e-mail-címre.</span><span class="sxs-lookup"><span data-stu-id="40c28-123">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="40c28-124">A regisztráció állapotát a Beállítások Fiókbeállítások Partnerprofil és a Program >  >    >   is ellenőrizheti.</span><span class="sxs-lookup"><span data-stu-id="40c28-124">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="40c28-125">Az Áttekintés **oldalon** látni fogja a közvetett viszonteladói szerződést.</span><span class="sxs-lookup"><span data-stu-id="40c28-125">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="40c28-126">Válassza **az Elfogadás lehetőséget, és folytassa a gombra.**</span><span class="sxs-lookup"><span data-stu-id="40c28-126">Select **Accept and continue**.</span></span> <span data-ttu-id="40c28-127">Ez a művelet lehetővé teszi a közvetett viszonteladói képességeket.</span><span class="sxs-lookup"><span data-stu-id="40c28-127">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="40c28-128">Ha elfogadta a közvetett viszonteladói szerződést, figyelje meg, hogy **a** Partnerprofil közvetlen számlaként és közvetett viszonteladóként is azonosítja.</span><span class="sxs-lookup"><span data-stu-id="40c28-128">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Közvetett viszonteladói szerződés.":::

> [!IMPORTANT]
> <span data-ttu-id="40c28-130">Miután az új funkcióval regisztrált közvetett viszonteladóként, nincs lehetőség a közvetlen számlás bérlőre való visszaállításra.</span><span class="sxs-lookup"><span data-stu-id="40c28-130">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="40c28-131">Mielőtt közvetett viszonteladóként regisztrál, győződjön meg arról, hogy teljesen kiértékeli az üzleti igényeit.</span><span class="sxs-lookup"><span data-stu-id="40c28-131">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="40c28-132">A közvetlen viszonteladóról a közvetett viszonteladóra való váltás során</span><span class="sxs-lookup"><span data-stu-id="40c28-132">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="40c28-133">Ebben a fázisban továbbra is kezelni fogja a közvetlen ügyfelek előfizetési igényeit, beleértve a számlázási folyamatot is.</span><span class="sxs-lookup"><span data-stu-id="40c28-133">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="40c28-134">Emellett megkezdheti az ügyfelek elfogadását a közvetett szolgáltatótól, és közvetett viszonteladóként működik.</span><span class="sxs-lookup"><span data-stu-id="40c28-134">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Ön közvetlen számla és közvetett viszonteladó is.":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="40c28-136">Közvetett szolgáltató keresése</span><span class="sxs-lookup"><span data-stu-id="40c28-136">Find an indirect provider</span></span>

<span data-ttu-id="40c28-137">A regisztráció után a bal oldali navigációs sávon megjelenik a közvetett szolgáltatókra mutató hivatkozás.</span><span class="sxs-lookup"><span data-stu-id="40c28-137">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="40c28-138">Közvetett viszonteladóként kapcsolatot fog létesíteni egy közvetett szolgáltatóval, aki ezután képes kezelni a számlázást, termékeket vásárolni az ügyfelek számára, és támogatási infrastruktúrát.</span><span class="sxs-lookup"><span data-stu-id="40c28-138">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="40c28-139">A különböző közvetett szolgáltatók különböző támogatást és szolgáltatásokat kínálnak, ezért érdemes kiértékelni az Ön területén található szolgáltatókat, hogy eldöntse, melyik felel meg legjobban az igényeinek.</span><span class="sxs-lookup"><span data-stu-id="40c28-139">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="40c28-140">A legtöbb szolgáltató általában a következőt fogja:</span><span class="sxs-lookup"><span data-stu-id="40c28-140">Generally, most providers will:</span></span>

- <span data-ttu-id="40c28-141">Műszaki képzés és segítségnyújtás</span><span class="sxs-lookup"><span data-stu-id="40c28-141">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="40c28-142">Segítség a termékek és szolgáltatások piaci marketingjére</span><span class="sxs-lookup"><span data-stu-id="40c28-142">Help you market your products and services</span></span>
- <span data-ttu-id="40c28-143">Kezelheti a használati feltételeket és a jóváírási feltételeket</span><span class="sxs-lookup"><span data-stu-id="40c28-143">Manage your financing and credit terms</span></span>

<span data-ttu-id="40c28-144">Keresse meg a [hivatalos Közvetett Microsoft-szolgáltatók listáját.](https://partnercenter.microsoft.com/partner/find-a-provider)</span><span class="sxs-lookup"><span data-stu-id="40c28-144">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="40c28-145">További információ:  [Partner közvetett szolgáltatókkal](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="40c28-145">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="40c28-146">Partneri meghívó elfogadása a közvetett szolgáltatótól</span><span class="sxs-lookup"><span data-stu-id="40c28-146">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="40c28-147">Ha közvetett szolgáltatót talál a partnerhez, partnerkapcsolatot létesítsen a közvetett szolgáltatóval a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="40c28-147">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="40c28-148">A kiválasztott közvetett szolgáltató e-mailben elküldi Önnek a partneri meghívó hivatkozását, amely a partneri meghívóra Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="40c28-148">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="40c28-149">Győződjön meg arról, hogy a globális rendszergazda bejelentkezik a Partnerközpont, és követi a meghívó hivatkozást.</span><span class="sxs-lookup"><span data-stu-id="40c28-149">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="40c28-150">Amikor elfogadja a meghívót, a szolgáltató neve megjelenik a közvetett szolgáltató listájában.</span><span class="sxs-lookup"><span data-stu-id="40c28-150">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="40c28-151">Új ügyfelek beszerzése közvetett viszonteladóként</span><span class="sxs-lookup"><span data-stu-id="40c28-151">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="40c28-152">Önnek és a közvetett szolgáltatónak is viszonteladói kapcsolatra van szüksége az ügyfelekkel.</span><span class="sxs-lookup"><span data-stu-id="40c28-152">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="40c28-153">Ezekkel a viszonteladói kapcsolatokkal kezelheti az ügyfelek előfizetését és szolgáltatásait a nevükben.</span><span class="sxs-lookup"><span data-stu-id="40c28-153">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="40c28-154">Ha egy meglévő Azure AD-bérlővel rendelkezik új ügyfelet, meghívhatja az ügyfelet, hogy egyszerre hozzon létre viszonteladói kapcsolatot Ön és a szolgáltató között.</span><span class="sxs-lookup"><span data-stu-id="40c28-154">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="40c28-155">Közvetett viszonteladói meghívó létrehozása:</span><span class="sxs-lookup"><span data-stu-id="40c28-155">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="40c28-156">A **bal oldali navigációs sávon** válassza Partnerközpont Közvetett szolgáltatók lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="40c28-156">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="40c28-157">Válassza **az Új ügyfelek meghívása,** hogy egyszerre hívjanak meg egy ügyfelet, hogy viszonteladói kapcsolatot létesítsen Önvel és a közvetett szolgáltatóval.</span><span class="sxs-lookup"><span data-stu-id="40c28-157">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="40c28-158">A szolgáltatónak viszonteladói kapcsolatban kell lennie az ügyféllel, hogy be tudja nyújtani a rendeléseket az ügyfél nevében, amikor az ügyfél új előfizetéseket szeretne vásárolni, vagy új licenceket szeretne hozzáadni a meglévő előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="40c28-158">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="40c28-159">A következő lapon tekintse át az e-mail-üzenet piszkozatát.</span><span class="sxs-lookup"><span data-stu-id="40c28-159">On the next page, review the draft email message.</span></span> <span data-ttu-id="40c28-160">A piszkozatüzenetet megnyithatja e-mailben, vagy a vágólapra másolhatja, és beillesztheti egy e-mailbe.</span><span class="sxs-lookup"><span data-stu-id="40c28-160">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="40c28-161">Szerkessze az e-mailben található szöveget úgy, hogy az tartalmazza, amire szüksége van, de mindenképpen foglalja bele a hivatkozást, mivel az személyre szabott, hogy az ügyfelet közvetlenül az Ön fiókjához és a szolgáltató fiókjához is csatlakoztassa.</span><span class="sxs-lookup"><span data-stu-id="40c28-161">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="40c28-162">Ezután válassza a **Done** (Kész) elemet.</span><span class="sxs-lookup"><span data-stu-id="40c28-162">Then select **Done**.</span></span>

5. <span data-ttu-id="40c28-163">Miután az ügyfél engedélyezte Önnek és a szolgáltatónak, hogy a rekord viszonteladója legyen, rendszergazdai jogosultsággal fog rendelkezni az előfizetések, licencek és felhasználók kezeléséhez a nevükben, és a közvetett szolgáltató be tudja majd nyújtani a rendeléseket a nevükben.</span><span class="sxs-lookup"><span data-stu-id="40c28-163">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="40c28-164">Az ügyfél fiókjának, szolgáltatásainak, felhasználóinak és licencének kezeléséhez bontsa ki az ügyfél rekordját a név melletti lefelé mutató nyílra kattintva.</span><span class="sxs-lookup"><span data-stu-id="40c28-164">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="40c28-165">A közvetlen számlázási partnerektől eltérően a közvetett viszonteladók nem hozhatnak létre Azure AD-bérlőket az új ügyfeleik számára a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="40c28-165">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="40c28-166">A szolgáltató létrehozza a bérlőt, és Ön lesz az ügyfél közvetett viszonteladója.</span><span class="sxs-lookup"><span data-stu-id="40c28-166">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="40c28-167">Ez biztosítja, hogy az ügyfél megjelenik az Ön ügyféllistán a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="40c28-167">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="40c28-168">A közvetlen számlázási funkcióját nem használhatja arra, hogy vásárlásokat hozzon létre a közvetett viszonteladóként beszerzett ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="40c28-168">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="40c28-169">A közvetlen számlázási ügyfelek és a közvetett viszonteladói ügyfelek kezelése</span><span class="sxs-lookup"><span data-stu-id="40c28-169">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="40c28-170">Ön másképp kezeli a közvetlen számlázási ügyfeleket és a közvetett viszonteladói ügyfeleket.</span><span class="sxs-lookup"><span data-stu-id="40c28-170">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="40c28-171">Közvetlen számlázási ügyfelek (olyan dolgok, amelyekre nem közvetett viszonteladóként lesz képes)</span><span class="sxs-lookup"><span data-stu-id="40c28-171">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="40c28-172">Termékek rendelésének létrehozása</span><span class="sxs-lookup"><span data-stu-id="40c28-172">Create orders for products</span></span>
- <span data-ttu-id="40c28-173">Az Azure Reservations kezelése</span><span class="sxs-lookup"><span data-stu-id="40c28-173">Manage Azure reservations</span></span>
- <span data-ttu-id="40c28-174">Rendelési előzményeik kezelése</span><span class="sxs-lookup"><span data-stu-id="40c28-174">Manage their order history</span></span>
- <span data-ttu-id="40c28-175">Szoftver vásárlása</span><span class="sxs-lookup"><span data-stu-id="40c28-175">Purchase software</span></span>
- <span data-ttu-id="40c28-176">Ügyfelek közvetlen számlázása</span><span class="sxs-lookup"><span data-stu-id="40c28-176">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="40c28-177">Közvetett viszonteladói ügyfelek</span><span class="sxs-lookup"><span data-stu-id="40c28-177">Indirect reseller customers</span></span>

- <span data-ttu-id="40c28-178">A közvetett szolgáltató termékeket rendel az ügyfeleinek</span><span class="sxs-lookup"><span data-stu-id="40c28-178">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="40c28-179">Ügyféllicencek és -felhasználók kezelése</span><span class="sxs-lookup"><span data-stu-id="40c28-179">Manage customers' licenses and users</span></span>
- <span data-ttu-id="40c28-180">Előfizetés megújításának kezeléséhez</span><span class="sxs-lookup"><span data-stu-id="40c28-180">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="40c28-181">A közvetlen számlázási partnerként beszerzett ügyfelek azonosítása</span><span class="sxs-lookup"><span data-stu-id="40c28-181">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="40c28-182">Válassza az **Ügyfelek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="40c28-182">Select **Customers**.</span></span>

2. <span data-ttu-id="40c28-183">Válasszon ki egy ügyfelet a részleteik megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="40c28-183">Select a customer to view their details.</span></span>

3. <span data-ttu-id="40c28-184">Ha ezt az ügyfelet közvetlen számlázási partnerként szerezte be,  látni fogja a termékek hozzáadásának vagy megtekintésének lehetőségeit, valamint az előfizetéseiket. </span><span class="sxs-lookup"><span data-stu-id="40c28-184">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="40c28-185">Ha az ügyfél közvetett viszonteladói kapcsolatban áll Önvel, ezek a lehetőségek nem lesznek elérhetők.</span><span class="sxs-lookup"><span data-stu-id="40c28-185">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="40c28-186">A közvetlen számlázási ügyfelek áthelyezése a közvetett szolgáltatóba</span><span class="sxs-lookup"><span data-stu-id="40c28-186">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="40c28-187">A közvetett szolgáltató nem küldhet rendeléseket vagy meglévő előfizetés-átadásokat a meglévő közvetlen számlázási ügyfelek számára, amíg nem áll velük viszonteladói kapcsolat.</span><span class="sxs-lookup"><span data-stu-id="40c28-187">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="40c28-188">Ha viszonteladói kapcsolatot létesít a közvetett szolgáltató és a meglévő közvetlen számlázási ügyfél között, az alábbi módszerek egyikét használhatja:</span><span class="sxs-lookup"><span data-stu-id="40c28-188">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="40c28-189">Viszonteladói kapcsolat bővítménye</span><span class="sxs-lookup"><span data-stu-id="40c28-189">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="40c28-190">Közvetett viszonteladói meghívó küldése az ügyfélnek</span><span class="sxs-lookup"><span data-stu-id="40c28-190">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="40c28-191">Részletes áttekintést kaphat a részletes folyamatról a [](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/) Közvetlenről közvetettre történő átállásról</span><span class="sxs-lookup"><span data-stu-id="40c28-191">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="40c28-192">Viszonteladói kapcsolat bővítménye</span><span class="sxs-lookup"><span data-stu-id="40c28-192">Reseller relationship extension</span></span>

<span data-ttu-id="40c28-193">A viszonteladói kapcsolatbővítmény funkcióval viszonteladói kapcsolatot hozhat létre a meglévő közvetlen számlázási ügyfelek és a közvetett szolgáltató között az Partnerközpont irányítópulton.</span><span class="sxs-lookup"><span data-stu-id="40c28-193">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="40c28-194">A funkció használata előtt vegye figyelembe a következőket:</span><span class="sxs-lookup"><span data-stu-id="40c28-194">Before using the feature, note the following:</span></span>

- <span data-ttu-id="40c28-195">Ez a funkció csak olyan közvetlen számlázási partnerek számára érhető el, akik közvetett viszonteladóvá válnak, befejezték a közvetett [viszonteladói regisztrációt.](#get-started)</span><span class="sxs-lookup"><span data-stu-id="40c28-195">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="40c28-196">Ezt a funkciót csak a meglévő közvetlen számlázási ügyfelekre alkalmazhatja.</span><span class="sxs-lookup"><span data-stu-id="40c28-196">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="40c28-197">Ez nem vonatkozik a [közvetett viszonteladói ügyfelekre.](#acquire-new-customers-as-indirect-reseller)</span><span class="sxs-lookup"><span data-stu-id="40c28-197">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="40c28-198">Csak olyan közvetett szolgáltatót választhat ki, amelyhez elfogadta a közvetett szolgáltatótól származó [partnermeghívást.](#accept-a-partnership-invitation-from-your-indirect-provider)</span><span class="sxs-lookup"><span data-stu-id="40c28-198">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="40c28-199">Az ügyfélhez rendelkezésre álló számlázási adatok másolata elérhető lesz a közvetett szolgáltató számára.</span><span class="sxs-lookup"><span data-stu-id="40c28-199">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="40c28-200">A számlázási adatokhoz úgy férhet hozzá, ha az ügyfél Fiók lapjára Partnerközpont irányítópulton.</span><span class="sxs-lookup"><span data-stu-id="40c28-200">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="40c28-201">A viszonteladói kapcsolatbővítmény funkció használatával beleegyezik, hogy az ügyfélre vonatkozó számlázási adatokat megossa a közvetett szolgáltatóval.</span><span class="sxs-lookup"><span data-stu-id="40c28-201">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="40c28-202">A közvetett szolgáltató nem fog delegált [rendszergazdai jogosultságokat](customers-revoke-admin-privileges.md) biztosítani az ügyfélbérlőnek.</span><span class="sxs-lookup"><span data-stu-id="40c28-202">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="40c28-203">Ha a közvetett szolgáltató delegált rendszergazdai jogosultságokat igényel, akkor inkább közvetett viszonteladói meghívót kell küldenie az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="40c28-203">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="40c28-204">A viszonteladói kapcsolat létrejötte után a közvetett szolgáltató CSP-partnerként jelenik meg az ügyfél számára a Felügyeleti központ Partnerkapcsolatok [lapján, Microsoft 365 felügyeleti](https://admin.microsoft.com/AdminPortal/Home#/partners) [Microsoft Store Vállalatoknak.](/microsoft-store/work-with-partner-microsoft-store-business)</span><span class="sxs-lookup"><span data-stu-id="40c28-204">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="40c28-205">A félreértések és félreértések elkerülése érdekében a partnerszerződése arra kötelezi Önt, hogy tájékoztassa és szerezze be a közvetlen számlázási ügyfél beleegyezését, mielőtt a kapcsolatbővítmény-funkcióval viszonteladói kapcsolatot hoz létre egy meglévő közvetlen számlázási ügyfél és egy közvetett szolgáltató között.</span><span class="sxs-lookup"><span data-stu-id="40c28-205">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="40c28-206">A funkció használata meglévő ügyfélbérlőn:</span><span class="sxs-lookup"><span data-stu-id="40c28-206">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="40c28-207">Jelentkezzen be a Partnerközpont **rendszergazdai ügynökként.**</span><span class="sxs-lookup"><span data-stu-id="40c28-207">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="40c28-208">Az Ügyfelek **lapon válasszon ki** egy meglévő  ügyfelet, és kattintson a Gyorshivatkozások ikonra az ügyfél összefoglaló nézetének kibontásához.</span><span class="sxs-lookup"><span data-stu-id="40c28-208">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="40c28-209">A **Közvetett szolgáltató(k) alatt kattintson** az Ügyfél **átadása közvetett szolgáltatón lehetőségre.**</span><span class="sxs-lookup"><span data-stu-id="40c28-209">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Ügyfél átadása közvetett szolgáltatónak.":::

4. <span data-ttu-id="40c28-211">Az előugró párbeszédpanelen  válassza ki azt a közvetett szolgáltatót, amely viszonteladói kapcsolatot szeretne az ügyféllel.</span><span class="sxs-lookup"><span data-stu-id="40c28-211">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="40c28-212">Kattintson a **Mentés gombra, és folytassa a gombra.**</span><span class="sxs-lookup"><span data-stu-id="40c28-212">Click **Save and continue**.</span></span>

6. <span data-ttu-id="40c28-213">Ellenőrizze, hogy a kiválasztott közvetett szolgáltató megjelenik-e a **Közvetett szolgáltató(k) alatt.**</span><span class="sxs-lookup"><span data-stu-id="40c28-213">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Közvetett szolgáltató listázva.":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="40c28-215">Közvetett viszonteladói meghívó küldése az ügyfélnek</span><span class="sxs-lookup"><span data-stu-id="40c28-215">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="40c28-216">A közvetett szolgáltató nem küldhet rendeléseket a meglévő közvetlen számlázási ügyfeleinek, amíg nem áll velük viszonteladói kapcsolat.</span><span class="sxs-lookup"><span data-stu-id="40c28-216">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="40c28-217">A meglévő ügyfelek és a közvetett szolgáltató közötti viszonteladói kapcsolat létesítenie érdekében meghívja az ügyfelet egy közvetett viszonteladói meghívóval.</span><span class="sxs-lookup"><span data-stu-id="40c28-217">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="40c28-218">A **bal oldali navigációs sávon** válassza Partnerközpont Közvetett szolgáltatók lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="40c28-218">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="40c28-219">Válassza **az Új ügyfelek meghívása,** hogy egyszerre hívjanak meg egy ügyfelet, hogy viszonteladói kapcsolatot létesítsen Önvel és a közvetett szolgáltatóval.</span><span class="sxs-lookup"><span data-stu-id="40c28-219">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="40c28-220">A szolgáltatónak viszonteladói kapcsolatban kell lennie az ügyféllel, hogy be tudja nyújtani a rendeléseket az ügyfél nevében, amikor az ügyfél új előfizetéseket szeretne vásárolni, vagy új licenceket szeretne hozzáadni a meglévő előfizetésekhez.</span><span class="sxs-lookup"><span data-stu-id="40c28-220">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Új ügyfelek meghívása.":::

3. <span data-ttu-id="40c28-222">A következő lapon tekintse át az e-mail-üzenet piszkozatát.</span><span class="sxs-lookup"><span data-stu-id="40c28-222">On the next page, review the draft email message.</span></span> <span data-ttu-id="40c28-223">Megnyithatja e-mailben a vázlatos üzenetet, vagy a vágólapra másolhatja, és beillesztheti egy e-mailbe.</span><span class="sxs-lookup"><span data-stu-id="40c28-223">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="40c28-224">Szerkessze az e-mail szövegét úgy, hogy az tartalmazza, amire szüksége van, de mindenképpen csatolja a hivatkozást, mivel az személyre szabott, hogy az ügyfelet közvetlenül az Ön fiókjához és a szolgáltató fiókjához is csatlakoztassa.</span><span class="sxs-lookup"><span data-stu-id="40c28-224">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="40c28-225">Ezután válassza a **Done** (Kész) elemet.</span><span class="sxs-lookup"><span data-stu-id="40c28-225">Then select **Done**.</span></span>

5. <span data-ttu-id="40c28-226">Miután az ügyfél engedélyezte Önnek és a szolgáltatónak, hogy a rekord viszonteladója legyen, rendszergazdai engedélyekkel fog rendelkezni az előfizetések, licencek és felhasználók kezeléséhez a nevükben, és a közvetett szolgáltató be tudja majd nyújtani a rendeléseket a nevükben.</span><span class="sxs-lookup"><span data-stu-id="40c28-226">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="40c28-227">Az ügyfél fiókjának, szolgáltatásainak, felhasználóinak és licencének kezeléséhez bontsa ki az ügyfél rekordját a név melletti lefelé mutató nyílra kattintva.</span><span class="sxs-lookup"><span data-stu-id="40c28-227">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="40c28-228">Microsoft Ügyfélszerződés elfogadása</span><span class="sxs-lookup"><span data-stu-id="40c28-228">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="40c28-229">Microsoft Cloud szerződés 2020. január 31-ig érvényes.</span><span class="sxs-lookup"><span data-stu-id="40c28-229">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="40c28-230">Ezt követően minden meglévő és új ügyfélnek alá kell írnia az új [Microsoft Ügyfélszerződés.](confirm-customer-agreement.md)</span><span class="sxs-lookup"><span data-stu-id="40c28-230">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="40c28-231">Az áttűnő ügyfelek esetén, ha:</span><span class="sxs-lookup"><span data-stu-id="40c28-231">For transitioning customers, if:</span></span>

- <span data-ttu-id="40c28-232">**Az ügyfél még nem fogadta el Microsoft Ügyfélszerződés-**</span><span class="sxs-lookup"><span data-stu-id="40c28-232">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="40c28-233">Működjön együtt a Közvetett szolgáltatóval, hogy az [ügyfél elfogadja a Microsoft Ügyfélszerződés.](confirm-customer-agreement.md)</span><span class="sxs-lookup"><span data-stu-id="40c28-233">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="40c28-234">**Az ügyfél elfogadta a Microsoft Ügyfélszerződés a felügyeleti központon Microsoft 365 keresztül**</span><span class="sxs-lookup"><span data-stu-id="40c28-234">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="40c28-235">Az elfogadás a közvetett szolgáltatóval való viszonteladói kapcsolat létrejötte után is megmarad.</span><span class="sxs-lookup"><span data-stu-id="40c28-235">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="40c28-236">Semmit nem kell megtennie.</span><span class="sxs-lookup"><span data-stu-id="40c28-236">There is nothing you need to do.</span></span>

- <span data-ttu-id="40c28-237">**Az ügyfél elfogadta Microsoft Ügyfélszerződés partneri igazoláson keresztül**</span><span class="sxs-lookup"><span data-stu-id="40c28-237">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="40c28-238">Az elfogadás nem lesz megőrizve.</span><span class="sxs-lookup"><span data-stu-id="40c28-238">The acceptance will not be retained.</span></span> <span data-ttu-id="40c28-239">Forduljon a Közvetett szolgáltatóhoz az ügyfél elfogadásának frissítéséhez a [Partnerközpont.](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)</span><span class="sxs-lookup"><span data-stu-id="40c28-239">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="40c28-240">Meglévő közvetlen számlázási előfizetések átvitele közvetett szolgáltatónak</span><span class="sxs-lookup"><span data-stu-id="40c28-240">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="40c28-241">A közvetett CSP-modell alatt a közvetett viszonteladók nem számlázási kapcsolatban vannak a Microsofttal.</span><span class="sxs-lookup"><span data-stu-id="40c28-241">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="40c28-242">Ehelyett a közvetett viszonteladók közvetett szolgáltatókon keresztül szereznek be előfizetéseket az ügyfeleik számára.</span><span class="sxs-lookup"><span data-stu-id="40c28-242">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="40c28-243">A közvetlen számlázási partnerről a közvetett viszonteladóra való áttérés során át kell ruházni a közvetlen számlázási partnerként meglévő előfizetéseket a közvetett szolgáltatóra.</span><span class="sxs-lookup"><span data-stu-id="40c28-243">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="40c28-244">Erre használhatja a saját maga által kiszolgált előfizetés-Partnerközpont irányítópulton.</span><span class="sxs-lookup"><span data-stu-id="40c28-244">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="40c28-245">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="40c28-245">Prerequisites</span></span>

- <span data-ttu-id="40c28-246">Ez a funkció csak olyan áttevő partnerek számára érhető el, akik már meglévő közvetlen számlázási partnerbérlőik használatával befejezték a közvetett viszonteladói regisztrációt.</span><span class="sxs-lookup"><span data-stu-id="40c28-246">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="40c28-247">Az adott ügyfélhez társított előfizetések átadása előtt az áttűnéspartnernek közvetett szolgáltatóra kell áthelyeznie az ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="40c28-247">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="40c28-248">Az ügyfélnek el kell [fogadnia Microsoft Ügyfélszerződés közvetett szolgáltatón keresztül.](#microsoft-customer-agreement-acceptance)</span><span class="sxs-lookup"><span data-stu-id="40c28-248">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="40c28-249">Váltás közvetett viszonteladói állapotra</span><span class="sxs-lookup"><span data-stu-id="40c28-249">How to transition to indirect reseller status</span></span>

<span data-ttu-id="40c28-250">A funkció egy négylépéses folyamat, amelyben:</span><span class="sxs-lookup"><span data-stu-id="40c28-250">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="40c28-251">Az áttűnéspartner létrehoz egy előfizetés-átadási kérelmet.</span><span class="sxs-lookup"><span data-stu-id="40c28-251">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="40c28-252">A kérelem egy vagy több meglévő előfizetést tartalmaz, amelyek ugyanannak az ügyfélnek vannak társítva, és egy közvetett szolgáltatóhoz vannak meg címzve.</span><span class="sxs-lookup"><span data-stu-id="40c28-252">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="40c28-253">A közvetett szolgáltató felülvizsgálja és elfogadja (vagy elutasítja) az átadási kérelmet.</span><span class="sxs-lookup"><span data-stu-id="40c28-253">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="40c28-254">A közvetett szolgáltató ellenőrzi, hogy az átadási kérelem befejeződött-e.</span><span class="sxs-lookup"><span data-stu-id="40c28-254">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="40c28-255">Az áttűnéspartner ellenőrzi, hogy az átadási kérelem befejeződött-e.</span><span class="sxs-lookup"><span data-stu-id="40c28-255">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="40c28-256">Átváltási partner</span><span class="sxs-lookup"><span data-stu-id="40c28-256">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="40c28-257">A meglévő [előfizetéseket a Partnerközpont API-val/SDK-val](/partner-center/develop/manage-customers) is áthelyezheti a közvetett szolgáltatónak.</span><span class="sxs-lookup"><span data-stu-id="40c28-257">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="40c28-258">Egy ügyfél előfizetési áthelyezési jogosultságainak lekérése</span><span class="sxs-lookup"><span data-stu-id="40c28-258">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="40c28-259">Egy ügyfél áthelyezésének létrehozása</span><span class="sxs-lookup"><span data-stu-id="40c28-259">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="40c28-260">Egy ügyfél áthelyezésének visszavonása</span><span class="sxs-lookup"><span data-stu-id="40c28-260">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="40c28-261">Egy ügyfél áthelyezésének elfogadása</span><span class="sxs-lookup"><span data-stu-id="40c28-261">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="40c28-262">Ügyfél átadásának elutasítása</span><span class="sxs-lookup"><span data-stu-id="40c28-262">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="40c28-263">Egy ügyfél áthelyezéseinek lekérése</span><span class="sxs-lookup"><span data-stu-id="40c28-263">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="40c28-264">Átviteli adatok lekérte azonosító alapján</span><span class="sxs-lookup"><span data-stu-id="40c28-264">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="40c28-265">Váltási partner – átadási kérelem létrehozása</span><span class="sxs-lookup"><span data-stu-id="40c28-265">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="40c28-266">Átadási kérelem létrehozása áttűnéspartnerként:</span><span class="sxs-lookup"><span data-stu-id="40c28-266">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="40c28-267">Jelentkezzen be a Partnerközpont **rendszergazdai ügynökként.**</span><span class="sxs-lookup"><span data-stu-id="40c28-267">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="40c28-268">Az Ügyfelek **lapon** válassza ki a kívánt ügyfelet, és kattintson a Gyorshivatkozások ikonra az ügyfél összefoglaló nézetének kibontásához.</span><span class="sxs-lookup"><span data-stu-id="40c28-268">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="40c28-269">A **Közvetett szolgáltató(k) alatt** ellenőrizze, hogy a kívánt közvetett szolgáltató szerepel-e a listán.</span><span class="sxs-lookup"><span data-stu-id="40c28-269">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="40c28-270">Kattintson **az Előfizetések megtekintése elemre.**</span><span class="sxs-lookup"><span data-stu-id="40c28-270">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="40c28-271">Az **Előfizetések lapon** keresse meg az **Előfizetések átvitele lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="40c28-271">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="40c28-272">Az **Előfizetés átvitele alatt** kattintson a Request subscription transfer **(Előfizetés átvitelének igénylése) elemre.**</span><span class="sxs-lookup"><span data-stu-id="40c28-272">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Előfizetés átvitelének igénylése.":::

7. <span data-ttu-id="40c28-274">Az átadási kérelem párbeszédpanelen válasszon ki egy vagy több átvitt előfizetést.</span><span class="sxs-lookup"><span data-stu-id="40c28-274">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Átadási kérelem létrehozása.":::

8. <span data-ttu-id="40c28-276">Kattintson a **Létrehozás** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="40c28-276">Click **Create**.</span></span>

9. <span data-ttu-id="40c28-277">Az aktív előfizetés-átadási kérelem az Előfizetés **átvitele alatt jelenik meg.**</span><span class="sxs-lookup"><span data-stu-id="40c28-277">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Átadási kérelmek listája.":::

10. <span data-ttu-id="40c28-279">Tájékoztassa a közvetett szolgáltatót arról, hogy előfizetés-átadási kérelmet hozott létre számukra.</span><span class="sxs-lookup"><span data-stu-id="40c28-279">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="40c28-280">Közvetett szolgáltató – átadási kérelem elfogadása</span><span class="sxs-lookup"><span data-stu-id="40c28-280">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="40c28-281">Átadási kérelem áttekintése és elfogadása közvetett szolgáltatóként:</span><span class="sxs-lookup"><span data-stu-id="40c28-281">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="40c28-282">Jelentkezzen be a Partnerközpont **rendszergazdai ügynökként** vagy **értékesítési ügynökként.**</span><span class="sxs-lookup"><span data-stu-id="40c28-282">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="40c28-283">Az Ügyfelek **lapon** válassza ki a kívánt ügyfelet, és kattintson a Gyorshivatkozások ikonra az ügyfél összefoglaló nézetének kibontásához.</span><span class="sxs-lookup"><span data-stu-id="40c28-283">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="40c28-284">A **Közvetett viszonteladó(k) alatt ellenőrizze,** hogy az áttűnéspartner szerepel-e a listán.</span><span class="sxs-lookup"><span data-stu-id="40c28-284">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="40c28-285">Kattintson **az Előfizetések megtekintése elemre.**</span><span class="sxs-lookup"><span data-stu-id="40c28-285">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="40c28-286">Az **Előfizetések lapon** keresse meg az **Előfizetések átvitele lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="40c28-286">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Átadási kérelem megtekintése.":::

6. <span data-ttu-id="40c28-288">Az **Előfizetés átvitele alatt** kattintson az átadási kérelemre az áttekintéshez.</span><span class="sxs-lookup"><span data-stu-id="40c28-288">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="40c28-289">Szükség **esetén kattintson az Elfogadás** (vagy **Elutasítás)** gombra.</span><span class="sxs-lookup"><span data-stu-id="40c28-289">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Átadási kérelem elfogadása.":::

8. <span data-ttu-id="40c28-291">Várjon, amíg az átadási kérelem befejeződik.</span><span class="sxs-lookup"><span data-stu-id="40c28-291">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="40c28-292">Közvetett szolgáltató – az átadási kérelem befejezésének ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="40c28-292">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="40c28-293">Az átadási kérelem sikeres befejezése után ellenőrizze, hogy látja-e az előfizetéseket az **Előfizetések alatt.**</span><span class="sxs-lookup"><span data-stu-id="40c28-293">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="40c28-294">Tájékoztassa az áttűnéspartnert.</span><span class="sxs-lookup"><span data-stu-id="40c28-294">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="40c28-295">Váltási partner – az átadási kérelem befejezésének ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="40c28-295">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="40c28-296">Az áttűnéspartnernek a következőket kell megtennie:</span><span class="sxs-lookup"><span data-stu-id="40c28-296">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="40c28-297">Jelentkezzen be Partnerközpont **rendszergazdai ügynökként vagy** **értékesítési ügynökként.**</span><span class="sxs-lookup"><span data-stu-id="40c28-297">Sign into Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="40c28-298">Az Ügyfelek **lapon** válassza ki a kívánt ügyfelet, és kattintson a **Gyorshivatkozások** ikonra az ügyfél összefoglaló nézetének kibontásához.</span><span class="sxs-lookup"><span data-stu-id="40c28-298">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="40c28-299">Kattintson **az Előfizetések megtekintése elemre.**</span><span class="sxs-lookup"><span data-stu-id="40c28-299">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="40c28-300">Az **Előfizetések lapon** keresse meg az **Előfizetések átvitele lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="40c28-300">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="40c28-301">Ellenőrizze, hogy az átadási kérelem Befejezettként **van-e megjelölve.**</span><span class="sxs-lookup"><span data-stu-id="40c28-301">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="40c28-302">Ellenőrizze, hogy az előfizetés(ök) már nem aktívként jelennek-e meg az **Előfizetések** lapon:</span><span class="sxs-lookup"><span data-stu-id="40c28-302">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="40c28-303">Ha ez egy Azure-előfizetés (MS-AZR-0145P), akkor a továbbiakban nem fog szerepelni a listán.</span><span class="sxs-lookup"><span data-stu-id="40c28-303">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="40c28-304">Ha ez egy licencalapú előfizetés (Office 365, Dynamics, Intune), felfüggesztett állapotban jelenik **meg.**</span><span class="sxs-lookup"><span data-stu-id="40c28-304">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Az előfizetés fel van függesztve.":::

### <a name="considerations"></a><span data-ttu-id="40c28-306">Megfontolandó szempontok</span><span class="sxs-lookup"><span data-stu-id="40c28-306">Considerations</span></span>

- <span data-ttu-id="40c28-307">**Az előfizetés azonosítója az átvitel után eltérő lesz.**</span><span class="sxs-lookup"><span data-stu-id="40c28-307">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="40c28-308">Ha ez egy Azure-előfizetés (MS-AZR-0145P), akkor egy Azure-előfizetés-azonosítóval is rendelkezik, amelyet az előző tulajdonos őriz meg, és megjelenik az Azure felügyeleti portálon.</span><span class="sxs-lookup"><span data-stu-id="40c28-308">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="40c28-309">**Ugyanazon előfizetésre nem hivatkozhat több átadási kérelem.**</span><span class="sxs-lookup"><span data-stu-id="40c28-309">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="40c28-310">Miután létrehozott egy átadási kérelmet, amely egy meglévő előfizetést is tartalmaz, nem hozhat létre további átadási kéréseket, beleértve ugyanazt az előfizetést is, amíg az első átadási kérelmet meg nem szakítják.</span><span class="sxs-lookup"><span data-stu-id="40c28-310">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="40c28-311">**A licencalapú előfizetések bővítményei az alap előfizetéssel együtt továbbíthatók.**</span><span class="sxs-lookup"><span data-stu-id="40c28-311">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="40c28-312">Átadási kérelem létrehozásakor, ha egy meglévő előfizetést választ egy vagy több bővítménysel, a bővítmények automatikusan bekerülnek az átadási kérelembe.</span><span class="sxs-lookup"><span data-stu-id="40c28-312">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="40c28-313">**Az előfizetés licencszámának változásai nem jelennek meg a meglévő átadási kérelemben.**</span><span class="sxs-lookup"><span data-stu-id="40c28-313">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="40c28-314">Miután létrehozott egy átadási kérelmet, amely egy meglévő előfizetést is tartalmaz, kerülje az előfizetés (vagy a társított bővítmények) licencmennyiségének frissítését.</span><span class="sxs-lookup"><span data-stu-id="40c28-314">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="40c28-315">Ha így történik, az új mennyiség nem fog tükröződni az átadási kérelemben.</span><span class="sxs-lookup"><span data-stu-id="40c28-315">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="40c28-316">Miután a közvetett szolgáltató elfogadta az átadási kérelmet, az eredményül kapott előfizetés a régi mennyiséggel fog rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="40c28-316">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="40c28-317">Ha azt szeretné, hogy az új mennyiség átkerül a közvetett szolgáltatóhoz, meg kell szakítania a meglévő átadási kérelmet, és újra létre kell hoznia egy újat.</span><span class="sxs-lookup"><span data-stu-id="40c28-317">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="40c28-318">**Nem minden vásárlás továbbítható önkiszolgáló előfizetés-átadással.**</span><span class="sxs-lookup"><span data-stu-id="40c28-318">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="40c28-319">Jelenleg csak O365- és Azure PAYG-előfizetéseket (MS-AZR-0145P) továbbíthat ezzel a funkcióval.</span><span class="sxs-lookup"><span data-stu-id="40c28-319">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="40c28-320">Az egyéb vásárlások, például az Azure-csomagok, az Azure Reserved Instances, az időszakalapú előfizetések és a Azure Marketplace SaaS-előfizetések nem támogatottak.</span><span class="sxs-lookup"><span data-stu-id="40c28-320">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="40c28-321">Az átadási kérelem beküldését lehetővé tő oldalon láthatja, hogy miért nem lehet előfizetést átvini.</span><span class="sxs-lookup"><span data-stu-id="40c28-321">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="40c28-322">Az előfizetések átviteléhez le [](create-a-new-subscription.md#suspend-or-cancel-a-subscription) kell mondania a meglévő előfizetést, és új ajánlatot kell vásárolnia az ügyfél számára közvetett szolgáltatón keresztül.</span><span class="sxs-lookup"><span data-stu-id="40c28-322">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="40c28-323">**Tesztkörnyezetben nem tesztelhető.**</span><span class="sxs-lookup"><span data-stu-id="40c28-323">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="40c28-324">Regisztráció közvetett viszonteladói ösztönzőkre</span><span class="sxs-lookup"><span data-stu-id="40c28-324">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="40c28-325">Miután sikeresen regisztrált közvetett viszonteladóként a meglévő közvetlen számlázási partnerbérlőben, 30 napon belül meghívót kap arra, hogy regisztráljon közvetett viszonteladói ösztönzőre.</span><span class="sxs-lookup"><span data-stu-id="40c28-325">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="40c28-326">A meghívó azon a partner MPN-fiókon alapul, amely jelenleg a CSP-partnerbérlőhöz van társítva.</span><span class="sxs-lookup"><span data-stu-id="40c28-326">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="40c28-327">A meghívó a partner MPN-fiókhoz társított e-mail-címre lesz elküldve.</span><span class="sxs-lookup"><span data-stu-id="40c28-327">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="40c28-328">Emellett regisztrálható közvetlen számlázási ösztönzőprogramokra ugyanazokkal a partnerbérlővel.</span><span class="sxs-lookup"><span data-stu-id="40c28-328">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="40c28-329">A programokat külön kell kezelnie.</span><span class="sxs-lookup"><span data-stu-id="40c28-329">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="40c28-330">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="40c28-330">Next steps</span></span>

- [<span data-ttu-id="40c28-331">További információ a közvetett viszonteladóvá válásról</span><span class="sxs-lookup"><span data-stu-id="40c28-331">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="40c28-332">A közvetlen CSP-partnerre vonatkozó új követelmények</span><span class="sxs-lookup"><span data-stu-id="40c28-332">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="40c28-333">Korlátozott közvetlen számlázási képességek</span><span class="sxs-lookup"><span data-stu-id="40c28-333">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
