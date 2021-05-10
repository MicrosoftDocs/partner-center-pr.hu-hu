---
title: Hogyan befolyásolják az adózási szabályzatok a kifizetési Azure Marketplace
description: Megtudhatja, hogyan befolyásolják az adózási szabályzatok a kifizetési Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686313"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="745f6-103">Hogyan befolyásolják az adózási szabályzatok a kifizetési Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="745f6-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="745f6-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="745f6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="745f6-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="745f6-105">Global admin</span></span>
- <span data-ttu-id="745f6-106">Felhasználókezelő rendszergazda</span><span class="sxs-lookup"><span data-stu-id="745f6-106">User management admin</span></span>
- <span data-ttu-id="745f6-107">Rendszergazdai ügynök</span><span class="sxs-lookup"><span data-stu-id="745f6-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="745f6-108">Bevezetés</span><span class="sxs-lookup"><span data-stu-id="745f6-108">Introduction</span></span>

<span data-ttu-id="745f6-109">A Microsoft kereskedelmi piactere globálisan elérhető.</span><span class="sxs-lookup"><span data-stu-id="745f6-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="745f6-110">A tranzakciók a határokon keresztül történhetnek, és attól függően, hogy hol található az isv és az ügyfél, az adózási következmények eltérőek lehetnek.</span><span class="sxs-lookup"><span data-stu-id="745f6-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="745f6-111">Microsoft AppSource és Azure Marketplace a Partnerközpont adóprofil-információk alapján határozzák meg az ISV országát.</span><span class="sxs-lookup"><span data-stu-id="745f6-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="745f6-112">Az ügyfél országának meghatározásához használja az ügyfél számlázási adatait, vagy ha az ügyfél az EU-ban van, két különböző információt használunk.</span><span class="sxs-lookup"><span data-stu-id="745f6-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="745f6-113">A következő forgatókönyvek jobb érthetőségéhez [](tax-details-marketplace.md) tekintse meg az Adó részletei táblázatot, amely azt mutatja be, hogy a Microsoft a közzétevő nevében gyűjti be és fizeti-e az adókat, vagy hogy az adott felelősség a közzétevőhöz tartozik-e.</span><span class="sxs-lookup"><span data-stu-id="745f6-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="745f6-114">A témakörben szereplő összes értékesítési érték és adókulcs csak szemléltető célokat szolgál, nem pedig pontos adatokat.</span><span class="sxs-lookup"><span data-stu-id="745f6-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="745f6-115">Közzétevői tranzakció a Microsoft által felügyelt adó országában</span><span class="sxs-lookup"><span data-stu-id="745f6-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="745f6-116">**A forgatókönyv** – A Microsoft által felügyelt adózási országban a közzétevő és az ügyfél [között tranzakciók.](tax-details-marketplace.md#microsoft-managed-countries)</span><span class="sxs-lookup"><span data-stu-id="745f6-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="745f6-117">Ezekhez a tranzakciókhoz az értékesítéskor érvényes adó lesz hozzáadva, és a Microsoft elküldi ezt az adót az adott országnak.</span><span class="sxs-lookup"><span data-stu-id="745f6-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="745f6-118">A kifizetési és kifizetési számítások nem tartalmazzák az adókat.</span><span class="sxs-lookup"><span data-stu-id="745f6-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="745f6-119">A [D forgatókönyvben](#foreign-publisher-transacts-with-us-customer) az USA-n kívüli közzétevő és az USA-nak nem megfelelő ügyfelek közötti tranzakciókat láthatja.</span><span class="sxs-lookup"><span data-stu-id="745f6-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Megjeleníti az A kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="745f6-121">Közzétevői tranzakció a Microsoft által felügyelt adózási országban, ahol a Marketplace-díj az adózható szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="745f6-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="745f6-122">**B forgatókönyv** – Az USA-alapú közzétevő (az Partnerközpont adóprofil-információi által meghatározott) között egy, a Microsoft által felügyelt adózási országban található ügyfél számára, ahol az ország adót ír elő a Marketplace-díjra (ez egy adózható szolgáltatás).</span><span class="sxs-lookup"><span data-stu-id="745f6-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="745f6-123">Ebben a forgatókönyvben az áruházi szolgáltatási díjra vonatkozó adó ki lesz vonva a közzétevő kifizetésből.</span><span class="sxs-lookup"><span data-stu-id="745f6-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Megjeleníti a B kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="745f6-125">Közzétevői tranzakció a közzétevő által kezelt adó országában</span><span class="sxs-lookup"><span data-stu-id="745f6-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="745f6-126">**C forgatókönyv** – Olyan tranzakciók, amelyek egy közzétevő és egy közzétevő által kezelt adózási ország ügyfele között történik, és amelyek nem írnak elő forrásadót az ügyfelekre.</span><span class="sxs-lookup"><span data-stu-id="745f6-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="745f6-127">Az ügyfelek nem fizetnek az értékesítéskor, és a közzétevőnek kell fizetnie az összes vonatkozó adóért.</span><span class="sxs-lookup"><span data-stu-id="745f6-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="745f6-128">További információ az országspecifikus díjszabásról (például a közelgő adózási költségek eltolása érdekében) a Kereskedelmi piactéri ajánlatok csomagja és [díjszabása oldalon található.](/azure/marketplace/plans-pricing#custom-prices)</span><span class="sxs-lookup"><span data-stu-id="745f6-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="A C kifizetési folyamat forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="745f6-130">Foreign Publisher Transacts with US Customer</span><span class="sxs-lookup"><span data-stu-id="745f6-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="745f6-131">**D** forgatókönyv – Minden olyan ( az Partnerközpont adóprofilra vonatkozó információ által meghatározott) idegen közzétevő, aki az USA-ban nem él (lásd az [E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)forgatókönyvet), amely értékesítést készít egy EGYESÜLT-alapú ügyfélnek (az ügyfélfiókjuk címe határozza meg).</span><span class="sxs-lookup"><span data-stu-id="745f6-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="745f6-132">Az Egyesült Államok kormánya megköveteli, hogy a Microsoft visszatartott adója a közzétevő nevében legyen.</span><span class="sxs-lookup"><span data-stu-id="745f6-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="745f6-133">A kifizetésekből a közzétevőbe történő kifizetésből származó adó kiszámítása az ajánlat ára alapján történik.</span><span class="sxs-lookup"><span data-stu-id="745f6-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Megjeleníti a D kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="745f6-135">Idegen közzétevő egy Us Customer-ügyféllel való Tranzakciós tranzakcióval</span><span class="sxs-lookup"><span data-stu-id="745f6-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="745f6-136">**E forgatókönyv** – Minden olyan (az Partnerközpont Partnerközpont adóprofillal kapcsolatos információ által meghatározott) idegen közzétevő, amely az USA-ban értékesítést készít egy EGYESÜLT-alapú ügyfélnek (az ügyfélfiók címe határozza meg).</span><span class="sxs-lookup"><span data-stu-id="745f6-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="745f6-137">Az Egyesült Államok kormánya nem követeli meg, hogy a Microsoft visszatartsa az adót a közzétevő nevében.</span><span class="sxs-lookup"><span data-stu-id="745f6-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Megjeleníti az E kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="745f6-139">A külső közzétevő egy EU-ban regisztrált, a Microsoft által felügyelt országban (Írországon kívül) értékesít</span><span class="sxs-lookup"><span data-stu-id="745f6-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="745f6-140">**F forgatókönyv** – Egy adott országban található külső közzétevők és az EU-ban regisztrált (Írországon kívüli) ügyfelek közötti Microsoft-Managed tranzakciók.</span><span class="sxs-lookup"><span data-stu-id="745f6-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="745f6-141">Az ügyfél nem fizet adót az értékesítés után.</span><span class="sxs-lookup"><span data-stu-id="745f6-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Megjeleníti az F kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="745f6-143">A idegen közzétevő egy EU-ban regisztrált ügyfélnek értékesít a Microsoft által felügyelt országban (Írországban)</span><span class="sxs-lookup"><span data-stu-id="745f6-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="745f6-144">**G.** forgatókönyv – Egy adott országban található, a külevők és az EU-ban (Írországon belül) regisztrált ügyfelek közötti Microsoft-Managed tranzakciók.</span><span class="sxs-lookup"><span data-stu-id="745f6-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="745f6-145">Az ügyfél az áfakulcsot fizeti, a Microsoft pedig ezt az adót a kormánynak fizeti.</span><span class="sxs-lookup"><span data-stu-id="745f6-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="A G kifizetési folyamat forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="next-steps"></a><span data-ttu-id="745f6-147">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="745f6-147">Next steps</span></span>

- [<span data-ttu-id="745f6-148">Közzétevő – gyakori kérdések</span><span class="sxs-lookup"><span data-stu-id="745f6-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="745f6-149">Fizetési és adóprofilok létrehozására vonatkozó utasítások</span><span class="sxs-lookup"><span data-stu-id="745f6-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)