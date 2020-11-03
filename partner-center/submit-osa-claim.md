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
ms.openlocfilehash: fec01e6c4554421593de4135ccd1af5c5e7ce13b
ms.sourcegitcommit: 1840767efa4c5de41889bc9245567cf286a084c8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/29/2020
ms.locfileid: "92917254"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="ded43-104">Ügyfél-hozzárendelések a Microsoft 365 és a Dynamics 365-es rekord (CPOR) modellje révén</span><span class="sxs-lookup"><span data-stu-id="ded43-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>

<span data-ttu-id="ded43-105">**A következőre érvényes:**</span><span class="sxs-lookup"><span data-stu-id="ded43-105">**Applies to**</span></span>

- <span data-ttu-id="ded43-106">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ded43-106">Partner Center</span></span>

<span data-ttu-id="ded43-107">**Megfelelő szerepkörök:**</span><span class="sxs-lookup"><span data-stu-id="ded43-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="ded43-108">Ösztönzők rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="ded43-108">Incentives admin</span></span>

<span data-ttu-id="ded43-109">2019. október 1-jén a Microsoft megkezdte a CPOR-modell igénylési partnerének használatát a Microsoft 365 és a Dynamics 365-ügyfelekkel folytatott társítások kezeléséhez az online szolgáltatások tanácsadó (OSA) értékesítés, online szolgáltatások használata (OSU) Microsoft 365 és OSU-Business alkalmazási ösztönzők tekintetében.</span><span class="sxs-lookup"><span data-stu-id="ded43-109">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="ded43-110">Az ügyfél-hozzárendelési (CPOR) jogcímek csak az online szolgáltatások tanácsadó (OSA) értékesítésére, az online szolgáltatások használatára (OSU) vonatkoznak, és a OSU-Business alkalmazás Microsoft 365-ösztönző programokra.</span><span class="sxs-lookup"><span data-stu-id="ded43-110">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="ded43-111">Ha egy másik programhoz (például a felhőalapú megoldás-szolgáltatóhoz, a felügyelt viszonteladóhoz, az üzemeltetéshez vagy a felszínhez) tartozó együttes op-jogcímet küld, tekintse meg az itt ismertetett együttes op-jogcímek folyamatát.</span><span class="sxs-lookup"><span data-stu-id="ded43-111">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="ded43-112">A jogcímek beküldésekor a Microsoft érvényesíti azt.</span><span class="sxs-lookup"><span data-stu-id="ded43-112">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="ded43-113">Ezen a ponton további információkat kérhetünk.</span><span class="sxs-lookup"><span data-stu-id="ded43-113">We may ask you for more information at this point.</span></span> <span data-ttu-id="ded43-114">A társulási kérelem ügyfelét is értesíteni fogjuk.</span><span class="sxs-lookup"><span data-stu-id="ded43-114">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="ded43-115">Az ügyfeleknek öt munkanapon belül kell kijelentkezniük. Ha nem, akkor az adott Bérlővel és munkaterheléssel való társítása hivatalos lesz.</span><span class="sxs-lookup"><span data-stu-id="ded43-115">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="ded43-116">Ezen a ponton elérheti az ügyfél használati adatait.</span><span class="sxs-lookup"><span data-stu-id="ded43-116">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="ded43-117">A jogcímek elvégzéséhez a következő információkra lesz szüksége:</span><span class="sxs-lookup"><span data-stu-id="ded43-117">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="ded43-118">Az entitáshoz tartozó **MPN-azonosító** , amely a jogcímet végrehajtja</span><span class="sxs-lookup"><span data-stu-id="ded43-118">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="ded43-119">Az ügyfél **tartománynevének** [megkeresése](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="ded43-119">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="ded43-120">Az ügyfél **címtár-azonosítójának** vagy **bérlői azonosítójának** [megkeresése](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="ded43-120">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="ded43-121">A **megoldási területen** , például Business Applications vagy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ded43-121">The **Solution area** , such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="ded43-122">A végrehajtott **tevékenység** és a kívánt jogcím típusa, például értékesítés előtti, használati vagy bevételi társítás</span><span class="sxs-lookup"><span data-stu-id="ded43-122">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="ded43-123">Az ügyfél **kapcsolattartási neve** , címe és e-mail-címe</span><span class="sxs-lookup"><span data-stu-id="ded43-123">Your customer's **Contact name** , title, and email address</span></span>

- <span data-ttu-id="ded43-124">A Dynamics 365 esetében meg kell adnia az ügyfél **technikai kapcsolattartójának** nevét, címét és e-mail-címét is.</span><span class="sxs-lookup"><span data-stu-id="ded43-124">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="ded43-125">Saját vállalata **kapcsolattartójának neve** és e-mail-címe</span><span class="sxs-lookup"><span data-stu-id="ded43-125">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="ded43-126">Létre kell hoznia egy **nevet** a jogcím számára</span><span class="sxs-lookup"><span data-stu-id="ded43-126">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="ded43-127">Az Ön által igényelt **termék (ek)** vagy számítási feladat (ok)</span><span class="sxs-lookup"><span data-stu-id="ded43-127">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="ded43-128">A **végrehajtás igazolása (PoE)** , például az ügyfél által aláírt munkavégzési utasítás.</span><span class="sxs-lookup"><span data-stu-id="ded43-128">**Proof of execution (PoE)** , such as a statement of work signed by the customer.</span></span> <span data-ttu-id="ded43-129">Le is töltheti a használni kívánt PoE-sablont.</span><span class="sxs-lookup"><span data-stu-id="ded43-129">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="ded43-130">Csak a bevételi társulást igénylő partnerek esetén: a **Dynamics-megoldás eladójának neve** , az **ügyfél neve** és **az ISV termék/megoldás neve** .</span><span class="sxs-lookup"><span data-stu-id="ded43-130">For partners claiming revenue association only: **Dynamics solution seller name** , **Customer name** , and **Name of ISV product/solution** .</span></span> 

<span data-ttu-id="ded43-131">A következő szempontokat is ismernie kell:</span><span class="sxs-lookup"><span data-stu-id="ded43-131">You should also understand the following points:</span></span>

- <span data-ttu-id="ded43-132">Ha már rendelkezik Microsoft 365 ügyfelekkel, újra hozzá kell rendelnie azokat, akikkel továbbra is OSU-ösztönzőket szeretne keresni a folyamat használatával.</span><span class="sxs-lookup"><span data-stu-id="ded43-132">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="ded43-133">Ha meglévő, Dynamics 365-as vagy Power BI ügyfelekkel rendelkező társításokkal rendelkezik, ezek a társítások érvényesek maradnak az előfizetésük lejárta után.</span><span class="sxs-lookup"><span data-stu-id="ded43-133">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="ded43-134">Egy ügyfél több partnerrel is rendelkezhet, de a munkaterhelések (OSU-Microsoft 365) vagy az előfizetés (OSA-Sell és OSU-Business alkalmazások esetében) csak egyetlen partnerhez társíthatók.</span><span class="sxs-lookup"><span data-stu-id="ded43-134">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="ded43-135">Ügyféltársítás létrehozása</span><span class="sxs-lookup"><span data-stu-id="ded43-135">Create a customer association</span></span>

1. <span data-ttu-id="ded43-136">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ded43-136">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ded43-137">Válassza az **ösztönzők** lapot, válassza az **Áttekintés** lehetőséget, majd válassza az **ügyfelek társítások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ded43-137">Select the **Incentives** tab, select **Overview** , and then select **Customer associations** .</span></span>

3. <span data-ttu-id="ded43-138">Az ügyfél-hozzárendelések lap tetején válassza a **+ Ügyfél-hozzárendelés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ded43-138">At the top of the Customer associations page, select **+ Customer association** .</span></span>

4. <span data-ttu-id="ded43-139">Válassza ki az ügyfélhez társítani kívánt partnerhely **MPN-azonosítóját** , majd adja hozzá az ügyfél tartománynevét és címtár-azonosítóját.</span><span class="sxs-lookup"><span data-stu-id="ded43-139">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="ded43-140">Keresés</span><span class="sxs-lookup"><span data-stu-id="ded43-140">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="ded43-141">Válassza a **Folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ded43-141">Select **Continue** .</span></span>

6. <span data-ttu-id="ded43-142">Válassza ki a **megoldási területeket** és **tevékenységeket** .</span><span class="sxs-lookup"><span data-stu-id="ded43-142">Select the **Solution area** and **Activity** .</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="ded43-143">Ha a Business Applications lehetőséget választja, válassza a **használat és/vagy az értékesítés előtti** vagy a **bevételi társítás** lehetőséget, majd válassza a **Folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ded43-143">If you select Business Applications, select either **Usage and/or Pre-sales** , or **Revenue association** , and then select **Continue** .</span></span> 
   <br><br><span data-ttu-id="ded43-144">Ha a bevétel társítását választja, a rendszer az alább felsorolttól némileg eltérő adatokat kér.</span><span class="sxs-lookup"><span data-stu-id="ded43-144">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="ded43-145">Adja meg a megfelelő adatokat az **Ügyfél hozzárendelése** lapon, majd válassza a **jogcím létrehozása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ded43-145">Enter the appropriate information on the **Associate customer** page, and then select **Create claim** .</span></span>

8. <span data-ttu-id="ded43-146">Válassza ki az ügyfél-hozzárendeléshez társított terméket (ka) t, majd válassza a **Folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ded43-146">Select the product(s) associated with this customer association, and then select **Continue** .</span></span>

9. <span data-ttu-id="ded43-147">Töltse ki az ügyfél és a vállalat kapcsolattartási adatait.</span><span class="sxs-lookup"><span data-stu-id="ded43-147">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="ded43-148">Minden mezőt ki kell tölteni.</span><span class="sxs-lookup"><span data-stu-id="ded43-148">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="ded43-149">Ha a termék a Dynamics 365, és a kiválasztott termék több előfizetéssel rendelkezik ehhez az adott ügyfélhez, meg kell adnia az előfizetés-azonosítót is.</span><span class="sxs-lookup"><span data-stu-id="ded43-149">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="ded43-150">Adja meg a végrehajtás igazolását (PoE).</span><span class="sxs-lookup"><span data-stu-id="ded43-150">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="ded43-151">Húzza a mezőbe, tallózással keresse meg a saját támogató dokumentációját, vagy válassza a **Sablon letöltése** lehetőséget, és használjon egy sablont.</span><span class="sxs-lookup"><span data-stu-id="ded43-151">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template** .</span></span> 

11. <span data-ttu-id="ded43-152">Tetszés szerint adja hozzá és mentse a megjegyzéseket, majd válassza az **Igénylés beküldése** elemet.</span><span class="sxs-lookup"><span data-stu-id="ded43-152">Add and save comments if you like, and then select **Submit claim** .</span></span> <span data-ttu-id="ded43-153">Egy e-mailt küldünk az Ön ügyféltársítását elfogadását kérő ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="ded43-153">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="ded43-154">Miután elküldte az ügyfél-hozzárendelést, nem szerkesztheti.</span><span class="sxs-lookup"><span data-stu-id="ded43-154">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="ded43-155">Az ügyféltársítás állapota az **Állapot** mezőben jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="ded43-155">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="ded43-156">Válassza az **Előzmények** lehetőséget az ügyféltársítás előzményeinek megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="ded43-156">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ded43-157">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ded43-157">Next steps</span></span>

- [<span data-ttu-id="ded43-158">Ügyféltársítások kezelése</span><span class="sxs-lookup"><span data-stu-id="ded43-158">Manage customer associations</span></span>](incentives-manage-customer-associations.md)