---
title: Ügyféltársítás létrehozása
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Hozzon létre ügyfél-hozzárendeléseket a Recording (CPOR) modell igénylési partnerével. Segíti az értékesítések, a használat és a Microsoft 365 & Dynamics 365-ügyfelek által nyújtott ösztönzők kezelését.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7a7e3ed40dcc6b1248f008201bff667a9eb9a0f8
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028315"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="2e147-104">Ügyfél-hozzárendelések a Microsoft 365 és a Dynamics 365-es rekord (CPOR) modellje révén</span><span class="sxs-lookup"><span data-stu-id="2e147-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="2e147-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="2e147-105">**Appropriate roles**</span></span>

- <span data-ttu-id="2e147-106">Ösztönzők rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="2e147-106">Incentives admin</span></span>

<span data-ttu-id="2e147-107">2019. október 1-jén a Microsoft megkezdte a CPOR-modell igénylési partnerének használatát a Microsoft 365 és a Dynamics 365-ügyfelekkel kapcsolatos társítások kezeléséhez az online szolgáltatások tanácsadó (OSA) értékesítés, online szolgáltatások használata (OSU) – Microsoft 365 és OSU-Business alkalmazási ösztönzők tekintetében.</span><span class="sxs-lookup"><span data-stu-id="2e147-107">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="2e147-108">Az ügyfél-hozzárendelési (CPOR) jogcímek csak az online szolgáltatások tanácsadó (OSA) értékesítésére, az online szolgáltatások használatára (OSU) vonatkoznak, és a OSU-Business alkalmazás Microsoft 365-ösztönző programokra.</span><span class="sxs-lookup"><span data-stu-id="2e147-108">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="2e147-109">Ha egy másik programhoz (például a felhőalapú megoldás-szolgáltatóhoz, a felügyelt viszonteladóhoz, az üzemeltetéshez vagy a felszínhez) tartozó együttes op-jogcímet küld, tekintse meg az itt ismertetett együttes op-jogcímek folyamatát.</span><span class="sxs-lookup"><span data-stu-id="2e147-109">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="2e147-110">A jogcímek beküldésekor a Microsoft érvényesíti azt.</span><span class="sxs-lookup"><span data-stu-id="2e147-110">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="2e147-111">Ezen a ponton további információkat kérhetünk.</span><span class="sxs-lookup"><span data-stu-id="2e147-111">We may ask you for more information at this point.</span></span> <span data-ttu-id="2e147-112">A társulási kérelem ügyfelét is értesíteni fogjuk.</span><span class="sxs-lookup"><span data-stu-id="2e147-112">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="2e147-113">Az ügyfeleknek öt munkanapon belül kell kijelentkezniük. Ha nem, akkor az adott Bérlővel és munkaterheléssel való társítása hivatalos lesz.</span><span class="sxs-lookup"><span data-stu-id="2e147-113">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="2e147-114">Ezen a ponton elérheti az ügyfél használati adatait.</span><span class="sxs-lookup"><span data-stu-id="2e147-114">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="2e147-115">A jogcímek elvégzéséhez a következő információkra lesz szüksége:</span><span class="sxs-lookup"><span data-stu-id="2e147-115">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="2e147-116">Az entitáshoz tartozó **MPN-azonosító** , amely a jogcímet végrehajtja</span><span class="sxs-lookup"><span data-stu-id="2e147-116">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="2e147-117">Az ügyfél **tartománynevének** [megkeresése](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="2e147-117">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="2e147-118">Az ügyfél **címtár-azonosítójának** vagy **bérlői azonosítójának** [megkeresése](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="2e147-118">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="2e147-119">A **megoldási területen**, például Business Applications vagy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2e147-119">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="2e147-120">A végrehajtott **tevékenység** és a kívánt jogcím típusa, például értékesítés előtti, használati vagy bevételi társítás</span><span class="sxs-lookup"><span data-stu-id="2e147-120">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="2e147-121">Az ügyfél **kapcsolattartási neve**, címe és e-mail-címe</span><span class="sxs-lookup"><span data-stu-id="2e147-121">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="2e147-122">A Dynamics 365 esetében meg kell adnia az ügyfél **technikai kapcsolattartójának** nevét, címét és e-mail-címét is.</span><span class="sxs-lookup"><span data-stu-id="2e147-122">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="2e147-123">Saját vállalata **kapcsolattartójának neve** és e-mail-címe</span><span class="sxs-lookup"><span data-stu-id="2e147-123">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="2e147-124">Létre kell hoznia egy **nevet** a jogcím számára</span><span class="sxs-lookup"><span data-stu-id="2e147-124">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="2e147-125">Az Ön által igényelt **termék (ek)** vagy számítási feladat (ok)</span><span class="sxs-lookup"><span data-stu-id="2e147-125">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="2e147-126">A **végrehajtás igazolása (PoE)**, például az ügyfél által aláírt munkavégzési utasítás.</span><span class="sxs-lookup"><span data-stu-id="2e147-126">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="2e147-127">Le is töltheti a használni kívánt PoE-sablont.</span><span class="sxs-lookup"><span data-stu-id="2e147-127">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="2e147-128">Csak a bevételi társulást igénylő partnerek esetén: a **Dynamics-megoldás eladójának neve**, az **ügyfél neve** és **az ISV termék/megoldás neve**.</span><span class="sxs-lookup"><span data-stu-id="2e147-128">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="2e147-129">A következő szempontokat is ismernie kell:</span><span class="sxs-lookup"><span data-stu-id="2e147-129">You should also understand the following points:</span></span>

- <span data-ttu-id="2e147-130">Ha már rendelkezik Microsoft 365 ügyfelekkel, újra hozzá kell rendelnie azokat, akikkel továbbra is OSU-ösztönzőket szeretne keresni a folyamat használatával.</span><span class="sxs-lookup"><span data-stu-id="2e147-130">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="2e147-131">Ha meglévő, Dynamics 365-as vagy Power BI ügyfelekkel rendelkező társításokkal rendelkezik, ezek a társítások érvényesek maradnak az előfizetésük lejárta után.</span><span class="sxs-lookup"><span data-stu-id="2e147-131">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="2e147-132">Egy ügyfél több partnerrel is rendelkezhet, de a munkaterhelések (OSU-Microsoft 365) vagy az előfizetés (OSA-Sell és OSU-Business alkalmazások esetében) csak egyetlen partnerhez társíthatók.</span><span class="sxs-lookup"><span data-stu-id="2e147-132">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="2e147-133">Ügyféltársítás létrehozása</span><span class="sxs-lookup"><span data-stu-id="2e147-133">Create a customer association</span></span>

1. <span data-ttu-id="2e147-134">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="2e147-134">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="2e147-135">Válassza az **ösztönzők** lapot, válassza az **Áttekintés** lehetőséget, majd válassza az **ügyfelek társítások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2e147-135">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="2e147-136">Az ügyfél-hozzárendelések lap tetején válassza a **+ Ügyfél-hozzárendelés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2e147-136">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="2e147-137">Válassza ki az ügyfélhez társítani kívánt partnerhely **MPN-azonosítóját**, majd adja hozzá az ügyfél tartománynevét és címtár-azonosítóját.</span><span class="sxs-lookup"><span data-stu-id="2e147-137">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="2e147-138">Keresés</span><span class="sxs-lookup"><span data-stu-id="2e147-138">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="2e147-139">Válassza a **Folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2e147-139">Select **Continue**.</span></span>

6. <span data-ttu-id="2e147-140">Válassza ki a **megoldási területeket** és **tevékenységeket**.</span><span class="sxs-lookup"><span data-stu-id="2e147-140">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="2e147-141">Ha a Business Applications lehetőséget választja, válassza a **használat és/vagy az értékesítés előtti** vagy a **bevételi társítás** lehetőséget, majd válassza a **Folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2e147-141">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="2e147-142">Ha a bevétel társítását választja, a rendszer az alább felsorolttól némileg eltérő adatokat kér.</span><span class="sxs-lookup"><span data-stu-id="2e147-142">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="2e147-143">Adja meg a megfelelő adatokat az **Ügyfél hozzárendelése** lapon, majd válassza a **jogcím létrehozása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2e147-143">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="2e147-144">Válassza ki az ügyfél-hozzárendeléshez társított terméket (ka) t, majd válassza a **Folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2e147-144">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="2e147-145">Töltse ki az ügyfél és a vállalat kapcsolattartási adatait.</span><span class="sxs-lookup"><span data-stu-id="2e147-145">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="2e147-146">Minden mezőt ki kell tölteni.</span><span class="sxs-lookup"><span data-stu-id="2e147-146">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="2e147-147">Ha a termék a Dynamics 365, és a kiválasztott termék több előfizetéssel rendelkezik ehhez az adott ügyfélhez, meg kell adnia az előfizetés-azonosítót is.</span><span class="sxs-lookup"><span data-stu-id="2e147-147">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="2e147-148">Adja meg a végrehajtás igazolását (PoE).</span><span class="sxs-lookup"><span data-stu-id="2e147-148">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="2e147-149">Húzza a mezőbe, tallózással keresse meg a saját támogató dokumentációját, vagy válassza a **Sablon letöltése** lehetőséget, és használjon egy sablont.</span><span class="sxs-lookup"><span data-stu-id="2e147-149">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="2e147-150">Tetszés szerint adja hozzá és mentse a megjegyzéseket, majd válassza az **Igénylés beküldése** elemet.</span><span class="sxs-lookup"><span data-stu-id="2e147-150">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="2e147-151">Egy e-mailt küldünk az Ön ügyféltársítását elfogadását kérő ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="2e147-151">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="2e147-152">Miután elküldte az ügyfél-hozzárendelést, nem szerkesztheti.</span><span class="sxs-lookup"><span data-stu-id="2e147-152">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="2e147-153">Az ügyféltársítás állapota az **Állapot** mezőben jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="2e147-153">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="2e147-154">Válassza az **Előzmények** lehetőséget az ügyféltársítás előzményeinek megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="2e147-154">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2e147-155">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="2e147-155">Next steps</span></span>

- [<span data-ttu-id="2e147-156">Ügyféltársítások kezelése</span><span class="sxs-lookup"><span data-stu-id="2e147-156">Manage customer associations</span></span>](incentives-manage-customer-associations.md)