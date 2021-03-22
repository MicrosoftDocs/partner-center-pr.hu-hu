---
title: Az adózási szabályzatok hatása az Azure Marketplace-re való kifizetésre
description: Ismerje meg, hogyan hatnak az adószabályok az Azure Marketplace-re való kifizetésre.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 817cdb895efab553b6f0131cdcdcf9b24bc6db3e
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768822"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="8675b-103">Az adózási szabályzatok hatása az Azure Marketplace-re való kifizetésre</span><span class="sxs-lookup"><span data-stu-id="8675b-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="8675b-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="8675b-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="8675b-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="8675b-105">Global admin</span></span>
-    <span data-ttu-id="8675b-106">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="8675b-106">User management admin</span></span>
-    <span data-ttu-id="8675b-107">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="8675b-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="8675b-108">Bevezetés</span><span class="sxs-lookup"><span data-stu-id="8675b-108">Introduction</span></span>

<span data-ttu-id="8675b-109">A Microsoft kereskedelmi piactér globális elérhetőséggel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="8675b-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="8675b-110">A tranzakciók határokon keresztül történnek, és attól függően, hogy hol találhatók az ISV-és az ügyfél, az adó következményei változhatnak.</span><span class="sxs-lookup"><span data-stu-id="8675b-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="8675b-111">A Microsoft AppSource és az Azure Marketplace a partner Center adózási profiljának adatait használja az ISV országának meghatározásához.</span><span class="sxs-lookup"><span data-stu-id="8675b-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="8675b-112">Az ügyfél országának meghatározásához használja az ügyfél számlázási adatait, vagy ha az ügyfél az EU-ban található, két különböző információt használunk.</span><span class="sxs-lookup"><span data-stu-id="8675b-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="8675b-113">Az alábbi forgatókönyvek jobb megismeréséhez tekintse meg az [adó részletei](tax-details-marketplace.md) táblát, amely azt mutatja, hogy a Microsoft a közzétevő nevében gyűjt és fizet adót, vagy ha az adott felelősség a közzétevőhöz tartozik.</span><span class="sxs-lookup"><span data-stu-id="8675b-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="8675b-114">Ebben a témakörben az eladási értékek és az adókulcs-százalékarányok csak szemléltető célokat szolgálnak, nem pontos számadatokat tartalmaznak.</span><span class="sxs-lookup"><span data-stu-id="8675b-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="8675b-115">Közzétevői Transacts a Microsoft által felügyelt adózási országban</span><span class="sxs-lookup"><span data-stu-id="8675b-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="8675b-116">**A forgatókönyv** – a közzétevő és az ügyfél közötti, a [Microsoft által felügyelt adózási országokban](tax-details-marketplace.md#microsoft-managed-countries)lebonyolított tranzakciók.</span><span class="sxs-lookup"><span data-stu-id="8675b-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="8675b-117">Ezek a tranzakciók érvényes adót kapnak az értékesítéskor, és a Microsoft ezt az adót a megfelelő országnak küldi el.</span><span class="sxs-lookup"><span data-stu-id="8675b-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="8675b-118">A kifizetés és a kifizetési számítások alól nem számítunk fel adót.</span><span class="sxs-lookup"><span data-stu-id="8675b-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="8675b-119">A nem USA-beli közzétevő és az Egyesült államokbeli ügyfél közötti tranzakciókért lásd: [D. forgatókönyv](#foreign-publisher-transacts-with-us-customer) .</span><span class="sxs-lookup"><span data-stu-id="8675b-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="A kifizetési folyamat forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="8675b-121">Kiadói Transacts a Microsoft által felügyelt adózási országban, ahol a piactér díja adóköteles szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="8675b-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="8675b-122">" **B" forgatókönyv** – az USA-alapú közzétevő (a partneri központ adóügyi profilja alapján meghatározott) közötti tranzakciók egy Microsoft által felügyelt adózási országban lévő ügyfélre, ahol az ország a Piactéri díj (adóköteles szolgáltatás) esetében adót szab ki.</span><span class="sxs-lookup"><span data-stu-id="8675b-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="8675b-123">Ebben a forgatókönyvben az áruházi szolgáltatási díj adóját kivonják a kiadó kifizetésével.</span><span class="sxs-lookup"><span data-stu-id="8675b-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="A kifizetési folyamat &quot;B&quot; forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="8675b-125">Közzétevői tranzakciók a közzétevő által kezelt adózási országban</span><span class="sxs-lookup"><span data-stu-id="8675b-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="8675b-126">**C. forgatókönyv** – a közzétevő által felügyelt adózási országban egy kiadó és egy ügyfél között zajló tranzakciók, amelyek nem írnak elő forrásadót az ügyfeleken.</span><span class="sxs-lookup"><span data-stu-id="8675b-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="8675b-127">Az ügyfelek nem fizetnek adót az eladási helyen, és a kiadó köteles fizetni az összes vonatkozó adót.</span><span class="sxs-lookup"><span data-stu-id="8675b-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="8675b-128">Az országspecifikus díjszabással (például a közelgő adózás ellensúlyozására) kapcsolatos további információkért tekintse meg a [kereskedelmi Piactéri ajánlatok csomagjait és díjszabását](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="8675b-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="A kifizetési folyamat C. forgatókönyvének munkafolyamatát mutatja be.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="8675b-130">Külföldi kiadói tranzakciók az USA-beli ügyféllel</span><span class="sxs-lookup"><span data-stu-id="8675b-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="8675b-131">**D. forgatókönyv** – az Egyesült államokbeli szerződéssel nem rendelkező országokban (a partneri központ adózási profiljának adatai alapján) az összes külföldi közzétevő (lásd az [E FORGATÓKÖNYVET](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) az USA-beli ügyfélnek (az ügyfél-fiók címe alapján) való értékesítésének megtételéhez.</span><span class="sxs-lookup"><span data-stu-id="8675b-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="8675b-132">Az Egyesült Államok kormánya megköveteli, hogy a Microsoft visszatartási adót tartson a közzétevő nevében.</span><span class="sxs-lookup"><span data-stu-id="8675b-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="8675b-133">A kifizetésből a kiadóba visszatartott adót az ajánlati ár alapján számítjuk ki.</span><span class="sxs-lookup"><span data-stu-id="8675b-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="A kifizetési folyamat &quot;D&quot; forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="8675b-135">Külföldi kiadó szerződési tranzakciókkal az USA-beli ügyféllel</span><span class="sxs-lookup"><span data-stu-id="8675b-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="8675b-136">**E. forgatókönyv** – minden külső közzétevő (a partneri központ adózási profiljának adatai alapján) az USA-szerződéssel rendelkező országokban az Egyesült államokbeli ügyfél (az ügyfél-fiók címe alapján) értékesítést tesz elérhetővé.</span><span class="sxs-lookup"><span data-stu-id="8675b-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="8675b-137">Az Egyesült Államok kormánya nem követeli meg a Microsofttól, hogy az adót a kiadó nevében visszatartsa.</span><span class="sxs-lookup"><span data-stu-id="8675b-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="A kifizetési folyamat munkafolyamatát mutatja E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="8675b-139">A külföldi közzétevő a Microsoft által felügyelt országban (Írországon kívül) egy EU-beli ÁFA-regisztrált ügyfelet értékesít</span><span class="sxs-lookup"><span data-stu-id="8675b-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="8675b-140">**F. forgatókönyv** – a külföldi közzétevők és az EU áfa-regisztrált ügyfelei (Írországon kívül) Microsoft-Managed ország összes tranzakciója.</span><span class="sxs-lookup"><span data-stu-id="8675b-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="8675b-141">Az ügyfél nem fizet adót az értékesítésért.</span><span class="sxs-lookup"><span data-stu-id="8675b-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="A kifizetési folyamat F. forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="8675b-143">A külföldi kiadó egy Microsoft által felügyelt országban (Írországban) értékesíti az EU-beli ÁFA-regisztrált ügyfelet</span><span class="sxs-lookup"><span data-stu-id="8675b-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="8675b-144">**G. forgatókönyv** – a külföldi közzétevők és az EU-beli HÉA-regisztrált ügyfelek közötti összes tranzakció Microsoft-Managed országban (Írországon belül).</span><span class="sxs-lookup"><span data-stu-id="8675b-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="8675b-145">Az ügyfél ír áfát fizet, a Microsoft pedig az ír kormánynak fizeti be ezt az adót.</span><span class="sxs-lookup"><span data-stu-id="8675b-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="A kifizetési folyamat G. forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="next-steps"></a><span data-ttu-id="8675b-147">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="8675b-147">Next steps</span></span>

- [<span data-ttu-id="8675b-148">Közzétevő – gyakori kérdések</span><span class="sxs-lookup"><span data-stu-id="8675b-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="8675b-149">Fizetési és adózási profilok létrehozásához szükséges utasítások</span><span class="sxs-lookup"><span data-stu-id="8675b-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)