---
title: Ügyféltársítás létrehozása
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Ügyfél-társítások létrehozása a igénylő regisztrált partner (CPOR) modellel. Segít a Dynamics 365-ügyfelek értékesítésének, használatának és Microsoft 365 & kezelésében.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 196009d9271324377be02d0b2d12ba8a4d7a993c
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489951"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="b7e4e-104">Ügyféltársítások az igényelt rekordpartner (CPOR) modellen keresztül a Microsoft 365 Dynamics 365-höz</span><span class="sxs-lookup"><span data-stu-id="b7e4e-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="b7e4e-105">**Megfelelő szerepkörök:** Ösztönzők rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="b7e4e-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="b7e4e-106">2019. október 1-től a Microsoft az igénylő regisztrált partner (CPOR) modellt kezdte használni az Microsoft 365- és Dynamics 365-ügyfelekkel való társítások kezelésére az Online Services Tanácsadás (OSA) Értékesítés, Online Services Usage (OSU)-Microsoft 365 és OSU-Business Application ösztönzők tekintetében.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="b7e4e-107">Az ügyfél-társítási (CPOR) igények csak az Online Services Advisor (OSA) értékesítésre, az Online Services Usage (OSU)-Microsoft 365 és az OSU-Business Application incentive programokra vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="b7e4e-108">Ha együttműködési igényt nyújt be egy másik program, például a Felhőszolgáltató (CSP), az Managed Reseller, az Hosting vagy a Surface számára, tekintse meg az itt ismertetett együttműködési igényfolyamatot.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider (CSP), Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="b7e4e-109">Az igénylés elküldésekor a Microsoft érvényesíti azt.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="b7e4e-110">Ezen a ponton további információkat kérhetünk Öntől.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="b7e4e-111">A társítási kérelemről is értesítjük az ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="b7e4e-112">Az ügyfeleknek öt munkanapjuk van a lemondásra. Ha nem fogják kikapcsolni a regisztrációt, az Adott bérlővel és számítási feladattal való társítása hivatalos lesz.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="b7e4e-113">Ezen a ponton hozzáférhet az ügyfél használati adataihoz.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="b7e4e-114">A jogcímek igénylésének befejezéséhez a következő információkra lesz szüksége:</span><span class="sxs-lookup"><span data-stu-id="b7e4e-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="b7e4e-115">A jogcímet igénylést Microsoft Partner Network entitás **MPN-azonosítója** (Microsoft Partner Network azonosítója)</span><span class="sxs-lookup"><span data-stu-id="b7e4e-115">The **MPN ID** (Microsoft Partner Network ID) for your entity that makes the claim</span></span>

- <span data-ttu-id="b7e4e-116">Az ügyfél **tartományneve** (további információ: [Bérlőazonosító, tartománynév, felhasználói objektumazonosító)](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="b7e4e-116">Customer's **domain name** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="b7e4e-117">Az ügyfél **címtár-azonosítója** vagy **bérlőazonosítója** (további információért lásd: [Bérlőazonosító, tartománynév, felhasználói objektumazonosító)](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="b7e4e-117">Customer's **Directory ID** or **Tenant ID** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="b7e4e-118">A **Megoldás terület,** például Business Applications vagy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b7e4e-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="b7e4e-119">Az **elvégzett** tevékenység és a kívánt jogcím típusa( értékesítés előtti, használat vagy bevétel társítása)</span><span class="sxs-lookup"><span data-stu-id="b7e4e-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="b7e4e-120">Az ügyfél Kapcsolattartó **neve,** címe és e-mail-címe</span><span class="sxs-lookup"><span data-stu-id="b7e4e-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="b7e4e-121">A Dynamics 365 esetén az ügyfél műszaki  kapcsolattartója nevét, címét és e-mail-címét is meg kell adnia</span><span class="sxs-lookup"><span data-stu-id="b7e4e-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="b7e4e-122">Saját vállalata **kapcsolattartójának neve és** e-mail-címe</span><span class="sxs-lookup"><span data-stu-id="b7e4e-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="b7e4e-123">Létre fog hozni egy **Nevet** a jogcímhez</span><span class="sxs-lookup"><span data-stu-id="b7e4e-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="b7e4e-124">Az **igényelt termék(nek)** vagy számítási feladat(nak)</span><span class="sxs-lookup"><span data-stu-id="b7e4e-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="b7e4e-125">**A végrehajtás igazolása (PoE),** például az ügyfél által aláírt munkakivonat.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="b7e4e-126">A használathoz letöltheti a PoE-sablont is.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="b7e4e-127">Csak bevételi társítást igénylő partnerek esetén: **Dynamics-megoldás** értékesítői neve, Ügyfél **neve** és **ISV-termék/megoldás neve.**</span><span class="sxs-lookup"><span data-stu-id="b7e4e-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="b7e4e-128">A következő pontokkal is érdemes tisztában lennie:</span><span class="sxs-lookup"><span data-stu-id="b7e4e-128">You should also understand the following points:</span></span>

- <span data-ttu-id="b7e4e-129">Ha már vannak Microsoft 365 ügyfelek, újra kell társítva azokkal, akik továbbra is OSU-ösztönzőket szeretne keresni ezzel a folyamattal.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-129">If you have existing Microsoft 365 customers, you'll need to reassociate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="b7e4e-130">Ha már rendelkezik Dynamics 365- vagy Power BI-ügyfelekkel, ezek a társítások az előfizetésük lejáratáig érvényesek maradnak.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="b7e4e-131">Egy ügyfél több partnerrel is rendelkezik, de minden számítási feladat (OSU-Microsoft 365 esetében) vagy előfizetése (OSA-Sell és OSU-Business-alkalmazások esetén) csak egy partnerhez társítható.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="b7e4e-132">Ügyféltársítás létrehozása</span><span class="sxs-lookup"><span data-stu-id="b7e4e-132">Create a customer association</span></span>

1. <span data-ttu-id="b7e4e-133">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="b7e4e-133">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="b7e4e-134">Válassza az **Ösztönzők lapot,** válassza az **Áttekintés,** majd az Ügyfél-társítások **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b7e4e-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="b7e4e-135">Az Ügyfél-társítások lap tetején válassza a + Ügyfél **társítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b7e4e-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="b7e4e-136">Válassza ki az ügyfélhez társítani kívánt partnerhely **MPN-azonosítóját**, majd adja hozzá az ügyfél tartománynevét és címtár-azonosítóját.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="b7e4e-137">Keresse meg ezt</span><span class="sxs-lookup"><span data-stu-id="b7e4e-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="b7e4e-138">Válassza a **Folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-138">Select **Continue**.</span></span>

6. <span data-ttu-id="b7e4e-139">Válassza ki **a Megoldás területet és a** **Tevékenységet.**</span><span class="sxs-lookup"><span data-stu-id="b7e4e-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="b7e4e-140">Ha a Business Applications, válassza a **Használat és/vagy** az Értékesítés előtti , vagy a Bevétel **társítása** lehetőséget, majd válassza a Folytatás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b7e4e-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="b7e4e-141">Ha a bevétel társítását választja, a rendszer az alább felsorolttól némileg eltérő adatokat kér.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="b7e4e-142">Adja meg a megfelelő adatokat a **Associate customer (Ügyfél társítása)** lapon, majd válassza a Create claim (Jogcím **létrehozása) lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b7e4e-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="b7e4e-143">Válassza ki az ügyfél-társításhoz társított terméket/termék(eket), majd válassza a **Continue (Folytatás) lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b7e4e-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="b7e4e-144">Töltse ki az ügyfél és a vállalat kapcsolattartási adatait.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="b7e4e-145">Minden mezőt ki kell tölteni.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="b7e4e-146">Ha a termék a Dynamics 365, és a választott termék több előfizetéssel rendelkezik ehhez az ügyfélhez, meg kell adnia az előfizetés azonosítóját is.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="b7e4e-147">A PoE-t is meg kell adni.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-147">Supply your PoE.</span></span> <span data-ttu-id="b7e4e-148">Húzza a mezőbe, tallózással keresse meg a saját támogató dokumentációját, vagy válassza a **Sablon letöltése** lehetőséget, és használjon egy sablont.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="b7e4e-149">Tetszés szerint adja hozzá és mentse a megjegyzéseket, majd válassza az **Igénylés beküldése** elemet.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="b7e4e-150">Egy e-mailt küldünk az Ön ügyféltársítását elfogadását kérő ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="b7e4e-151">Miután beküldi az ügyfél-társítást, nem szerkesztheti.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="b7e4e-152">Az ügyféltársítás állapota az **Állapot** mezőben jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="b7e4e-153">Válassza az **Előzmények** lehetőséget az ügyféltársítás előzményeinek megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="b7e4e-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b7e4e-154">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="b7e4e-154">Next steps</span></span>

- [<span data-ttu-id="b7e4e-155">Ügyféltársítások kezelése</span><span class="sxs-lookup"><span data-stu-id="b7e4e-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)