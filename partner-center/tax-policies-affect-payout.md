---
title: Hogyan befolyásolják az adózási szabályzatok a kifizetési Azure Marketplace
description: Megtudhatja, hogyan befolyásolják az adózási szabályzatok a kifizetési Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: a93e94912f840e4cb69c3cc834f03af1b34f19aa
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856015"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Hogyan befolyásolják az adózási szabályzatok a kifizetési Azure Marketplace

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Rendszergazdai ügynök

## <a name="introduction"></a>Bevezetés

A Microsoft kereskedelmi piactere globálisan elérhető. A tranzakciók a határokon keresztül történhetnek, és attól függően, hogy hol található az isv és az ügyfél, az adózási következmények eltérőek lehetnek. Microsoft AppSource és Azure Marketplace a Partnerközpont adóprofil-információk alapján határozzák meg az ISV országát. Az ügyfél országának meghatározásához használja az ügyfél számlázási adatait, vagy ha az ügyfél az EU-ban van, két különböző információt használunk.

A következő forgatókönyvek jobb érthetőségéhez [](tax-details-marketplace.md) tekintse meg az Adózási részletek táblázatot, amely azt mutatja be, hogy a Microsoft a közzétevő nevében gyűjti be és fizeti-e az adókat, vagy hogy a felelősség a közzétevőhöz tartozik-e.

> [!NOTE]
> Az ebben a témakörben szereplő összes értékesítési érték és adóarány csak szemléltető célokat szolgál, nem pedig pontos adatokat.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Közzétevői tranzakció a Microsoft által felügyelt adó országában

**A forgatókönyv** – A Microsoft által felügyelt adózási országban a közzétevő és az ügyfél [között tranzakciók.](tax-details-marketplace.md#microsoft-managed-countries) Ezekhez a tranzakciókhoz az értékesítéskor érvényes adó lesz hozzáadva, és a Microsoft elküldi ezt az adót az adott országnak. A kifizetési és kifizetési számítások nem tartalmazzák az adókat.

A [D forgatókönyvben](#foreign-publisher-transacts-with-us-customer) az USA-n kívüli közzétevő és egy EGYESÜLT ÁLLAMOK-ügyfél közötti tranzakciókat láthatja.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Megjeleníti az A kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Közzétevői tranzakció a Microsoft által felügyelt adózási országban, ahol a Marketplace-díj az adózható szolgáltatás

**B forgatókönyv** – Az USA-alapú közzétevő (az Partnerközpont adóprofil-információi által meghatározott) között egy, a Microsoft által felügyelt adózási országban található ügyfél számára, ahol az ország adót ír elő a Marketplace-díjra (ez egy adózható szolgáltatás). Ebben a forgatókönyvben az áruházi szolgáltatási díjra vonatkozó adó ki lesz vonva a közzétevő kifizetése alól.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="A B kifizetési folyamat forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Közzétevői tranzakció a közzétevő által kezelt adózási országban

**C forgatókönyv** – Olyan tranzakciók, amelyek egy közzétevő és egy közzétevő által kezelt adózási ország ügyfele között történik, és amelyek nem írnak elő forrásadót az ügyfelekre. Az ügyfelek nem fizetnek adót az értékesítéskor, és a közzétevőnek kell fizetnie az összes vonatkozó adóért.

További információ az országspecifikus díjszabásról (például a közelgő adózási költségek eltolása érdekében) a Csomagok és díjszabás [kereskedelmi piactéri ajánlatokhoz.](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="A C kifizetési folyamat forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Idegen közzétevői tranzakció az USA-ügyféllel

**D.** forgatókönyv – Minden olyan országban (amelyet az Partnerközpont adóprofil-adataik határoznak meg) olyan országokban, amelyekben az USA-ban nem volt probléma (lásd az [E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)forgatókönyvet), amely értékesítést készít egy USA-alapú ügyfélnek (az ügyfélfiókjuk címe határozza meg). Az Egyesült Államok kormánya megköveteli, hogy a Microsoft visszatartott adója a közzétevő nevében legyen. A kifizetésekből a közzétevőbe be nem számolt adó kiszámítása az ajánlat ára alapján történik.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="A D kifizetési folyamat forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Idegen közzétevő Egy Olyan tranzakcióval, amely az USA-ügyféllel van

**E forgatókönyv** – Minden olyan (az Partnerközpont Partnerközpont adóprofil-információ által meghatározott) idegen közzétevő, amely olyan országban van, ahol az USA-nak történő értékesítést az USA-alapú ügyfélnek (az ügyfélfiókjuk címe határozza meg). Az Egyesült Államok kormánya nem követeli meg, hogy a Microsoft visszatartsa a forrásadót a közzétevő nevében.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Megjeleníti az E kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>A külső közzétevő egy EU-ban regisztrált ügyfélnek értékesít a Microsoft által felügyelt országban (Írországon kívül)

**F forgatókönyv** – A külső közzétevők és az EU-ban (Írországon kívül) regisztrált ügyfelek közötti összes tranzakció egy Microsoft-Managed országban. Az ügyfél nem fizet adót az értékesítés után.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Megjeleníti az F kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>A idegen közzétevők a Microsoft által felügyelt országban (Írországban) értékesítik az EU-ban regisztrált áfabevallott ügyfeleket

**G.** forgatókönyv – Egy adott országban található, a idegen kiadók és az EU-ban regisztrált (Írországon belüli) ügyfelek közötti Microsoft-Managed tranzakciók. Az ügyfél az áfakulcsot fizeti, a Microsoft pedig ezt az adót a Kormány kormányának fizeti.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Megjeleníti a G kifizetési folyamat forgatókönyvének munkafolyamatát.":::

## <a name="next-steps"></a>Következő lépések

- [Közzétevő – gyakori kérdések](/azure/marketplace/marketplace-faq-publisher-guide)
- [Fizetési és adóprofilok létrehozására vonatkozó utasítások](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)