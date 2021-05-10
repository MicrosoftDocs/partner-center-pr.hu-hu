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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Hogyan befolyásolják az adózási szabályzatok a kifizetési Azure Marketplace

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználókezelő rendszergazda
- Rendszergazdai ügynök

## <a name="introduction"></a>Bevezetés

A Microsoft kereskedelmi piactere globálisan elérhető. A tranzakciók a határokon keresztül történhetnek, és attól függően, hogy hol található az isv és az ügyfél, az adózási következmények eltérőek lehetnek. Microsoft AppSource és Azure Marketplace a Partnerközpont adóprofil-információk alapján határozzák meg az ISV országát. Az ügyfél országának meghatározásához használja az ügyfél számlázási adatait, vagy ha az ügyfél az EU-ban van, két különböző információt használunk.

A következő forgatókönyvek jobb érthetőségéhez [](tax-details-marketplace.md) tekintse meg az Adó részletei táblázatot, amely azt mutatja be, hogy a Microsoft a közzétevő nevében gyűjti be és fizeti-e az adókat, vagy hogy az adott felelősség a közzétevőhöz tartozik-e.

> [!NOTE]
> A témakörben szereplő összes értékesítési érték és adókulcs csak szemléltető célokat szolgál, nem pedig pontos adatokat.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Közzétevői tranzakció a Microsoft által felügyelt adó országában

**A forgatókönyv** – A Microsoft által felügyelt adózási országban a közzétevő és az ügyfél [között tranzakciók.](tax-details-marketplace.md#microsoft-managed-countries) Ezekhez a tranzakciókhoz az értékesítéskor érvényes adó lesz hozzáadva, és a Microsoft elküldi ezt az adót az adott országnak. A kifizetési és kifizetési számítások nem tartalmazzák az adókat.

A [D forgatókönyvben](#foreign-publisher-transacts-with-us-customer) az USA-n kívüli közzétevő és az USA-nak nem megfelelő ügyfelek közötti tranzakciókat láthatja.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Megjeleníti az A kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Közzétevői tranzakció a Microsoft által felügyelt adózási országban, ahol a Marketplace-díj az adózható szolgáltatás

**B forgatókönyv** – Az USA-alapú közzétevő (az Partnerközpont adóprofil-információi által meghatározott) között egy, a Microsoft által felügyelt adózási országban található ügyfél számára, ahol az ország adót ír elő a Marketplace-díjra (ez egy adózható szolgáltatás). Ebben a forgatókönyvben az áruházi szolgáltatási díjra vonatkozó adó ki lesz vonva a közzétevő kifizetésből.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Megjeleníti a B kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Közzétevői tranzakció a közzétevő által kezelt adó országában

**C forgatókönyv** – Olyan tranzakciók, amelyek egy közzétevő és egy közzétevő által kezelt adózási ország ügyfele között történik, és amelyek nem írnak elő forrásadót az ügyfelekre. Az ügyfelek nem fizetnek az értékesítéskor, és a közzétevőnek kell fizetnie az összes vonatkozó adóért.

További információ az országspecifikus díjszabásról (például a közelgő adózási költségek eltolása érdekében) a Kereskedelmi piactéri ajánlatok csomagja és [díjszabása oldalon található.](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="A C kifizetési folyamat forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Foreign Publisher Transacts with US Customer

**D** forgatókönyv – Minden olyan ( az Partnerközpont adóprofilra vonatkozó információ által meghatározott) idegen közzétevő, aki az USA-ban nem él (lásd az [E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)forgatókönyvet), amely értékesítést készít egy EGYESÜLT-alapú ügyfélnek (az ügyfélfiókjuk címe határozza meg). Az Egyesült Államok kormánya megköveteli, hogy a Microsoft visszatartott adója a közzétevő nevében legyen. A kifizetésekből a közzétevőbe történő kifizetésből származó adó kiszámítása az ajánlat ára alapján történik.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Megjeleníti a D kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Idegen közzétevő egy Us Customer-ügyféllel való Tranzakciós tranzakcióval

**E forgatókönyv** – Minden olyan (az Partnerközpont Partnerközpont adóprofillal kapcsolatos információ által meghatározott) idegen közzétevő, amely az USA-ban értékesítést készít egy EGYESÜLT-alapú ügyfélnek (az ügyfélfiók címe határozza meg). Az Egyesült Államok kormánya nem követeli meg, hogy a Microsoft visszatartsa az adót a közzétevő nevében.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Megjeleníti az E kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>A külső közzétevő egy EU-ban regisztrált, a Microsoft által felügyelt országban (Írországon kívül) értékesít

**F forgatókönyv** – Egy adott országban található külső közzétevők és az EU-ban regisztrált (Írországon kívüli) ügyfelek közötti Microsoft-Managed tranzakciók. Az ügyfél nem fizet adót az értékesítés után.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Megjeleníti az F kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>A idegen közzétevő egy EU-ban regisztrált ügyfélnek értékesít a Microsoft által felügyelt országban (Írországban)

**G.** forgatókönyv – Egy adott országban található, a külevők és az EU-ban (Írországon belül) regisztrált ügyfelek közötti Microsoft-Managed tranzakciók. Az ügyfél az áfakulcsot fizeti, a Microsoft pedig ezt az adót a kormánynak fizeti.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="A G kifizetési folyamat forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="next-steps"></a>Következő lépések

- [Közzétevő – gyakori kérdések](/azure/marketplace/marketplace-faq-publisher-guide)
- [Fizetési és adóprofilok létrehozására vonatkozó utasítások](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)