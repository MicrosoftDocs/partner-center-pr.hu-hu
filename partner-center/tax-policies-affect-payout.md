---
title: Az adózási szabályzatok hatása az Azure Marketplace-re való kifizetésre
description: Ismerje meg, hogyan hatnak az adószabályok az Azure Marketplace-re való kifizetésre.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 19acb085b601212f1bf94316aab2b72c54aecc1a
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712953"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Az adózási szabályzatok hatása az Azure Marketplace-re való kifizetésre

**Megfelelő szerepkörök**
-    Globális rendszergazda
-    Felhasználói rendszergazda
-    Felügyeleti ügynök

## <a name="introduction"></a>Bevezetés

A Microsoft kereskedelmi piactér globális elérhetőséggel rendelkezik. A tranzakciók határokon keresztül történnek, és attól függően, hogy hol találhatók az ISV-és az ügyfél, az adó következményei változhatnak. A Microsoft AppSource és az Azure Marketplace a partner Center adózási profiljának adatait használja az ISV országának meghatározásához. Az ügyfél országának meghatározásához használja az ügyfél számlázási adatait, vagy ha az ügyfél az EU-ban található, két különböző információt használunk.

Az alábbi forgatókönyvek jobb megismeréséhez tekintse meg az [adó részletei](tax-details-marketplace.md) táblát, amely azt mutatja, hogy a Microsoft a közzétevő nevében gyűjt és fizet adót, vagy ha az adott felelősség a közzétevőhöz tartozik.

> [!NOTE]
> Ebben a témakörben az eladási értékek és az adókulcs-százalékarányok csak szemléltető célokat szolgálnak, nem pontos számadatokat tartalmaznak.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Közzétevői Transacts a Microsoft által felügyelt adózási országban

**A forgatókönyv** – a közzétevő és az ügyfél közötti, a [Microsoft által felügyelt adózási országokban](tax-details-marketplace.md#microsoft-managed-countries)lebonyolított tranzakciók. Ezek a tranzakciók érvényes adót kapnak az értékesítéskor, és a Microsoft ezt az adót a megfelelő országnak küldi el. A kifizetés és a kifizetési számítások alól nem számítunk fel adót.

A nem USA-beli közzétevő és az Egyesült államokbeli ügyfél közötti tranzakciókért lásd: [D. forgatókönyv](#foreign-publisher-transacts-with-us-customer) .

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="A kifizetési folyamat forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Kiadói Transacts a Microsoft által felügyelt adózási országban, ahol a piactér díja adóköteles szolgáltatás

" **B" forgatókönyv** – az USA-alapú közzétevő (a partneri központ adóügyi profilja alapján meghatározott) közötti tranzakciók egy Microsoft által felügyelt adózási országban lévő ügyfélre, ahol az ország a Piactéri díj (adóköteles szolgáltatás) esetében adót szab ki. Ebben a forgatókönyvben az áruházi szolgáltatási díj adóját kivonják a kiadó kifizetésével.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="A kifizetési folyamat &quot;B&quot; forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Közzétevői tranzakciók a közzétevő által kezelt adózási országban

**C. forgatókönyv** – a közzétevő által felügyelt adózási országban egy kiadó és egy ügyfél között zajló tranzakciók, amelyek nem írnak elő forrásadót az ügyfeleken. Az ügyfelek nem fizetnek adót az eladási helyen, és a kiadó köteles fizetni az összes vonatkozó adót.

Az országspecifikus díjszabással (például a közelgő adózás ellensúlyozására) kapcsolatos további információkért tekintse meg a [kereskedelmi Piactéri ajánlatok csomagjait és díjszabását](/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="A kifizetési folyamat C. forgatókönyvének munkafolyamatát mutatja be.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Külföldi kiadói tranzakciók az USA-beli ügyféllel

**D. forgatókönyv** – az Egyesült államokbeli szerződéssel nem rendelkező országokban (a partneri központ adózási profiljának adatai alapján) az összes külföldi közzétevő (lásd az [E FORGATÓKÖNYVET](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) az USA-beli ügyfélnek (az ügyfél-fiók címe alapján) való értékesítésének megtételéhez. Az Egyesült Államok kormánya megköveteli, hogy a Microsoft visszatartási adót tartson a közzétevő nevében. A kifizetésből a kiadóba visszatartott adót az ajánlati ár alapján számítjuk ki.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="A kifizetési folyamat &quot;D&quot; forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Külföldi kiadó szerződési tranzakciókkal az USA-beli ügyféllel

**E. forgatókönyv** – minden külső közzétevő (a partneri központ adózási profiljának adatai alapján) az USA-szerződéssel rendelkező országokban az Egyesült államokbeli ügyfél (az ügyfél-fiók címe alapján) értékesítést tesz elérhetővé. Az Egyesült Államok kormánya nem követeli meg a Microsofttól, hogy az adót a kiadó nevében visszatartsa.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="A kifizetési folyamat munkafolyamatát mutatja E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>A külföldi közzétevő a Microsoft által felügyelt országban (Írországon kívül) egy EU-beli ÁFA-regisztrált ügyfelet értékesít

**F. forgatókönyv** – a külföldi közzétevők és az EU áfa-regisztrált ügyfelei (Írországon kívül) Microsoft-Managed ország összes tranzakciója. Az ügyfél nem fizet adót az értékesítésért.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="A kifizetési folyamat F. forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>A külföldi kiadó egy Microsoft által felügyelt országban (Írországban) értékesíti az EU-beli ÁFA-regisztrált ügyfelet

**G. forgatókönyv** – a külföldi közzétevők és az EU-beli HÉA-regisztrált ügyfelek közötti összes tranzakció Microsoft-Managed országban (Írországon belül). Az ügyfél ír áfát fizet, a Microsoft pedig az ír kormánynak fizeti be ezt az adót.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="A kifizetési folyamat G. forgatókönyvének munkafolyamatát jeleníti meg.":::

## <a name="next-steps"></a>Következő lépések

- [Közzétevő – gyakori kérdések](/azure/marketplace/marketplace-faq-publisher-guide)
- [Fizetési és adózási profilok létrehozásához szükséges utasítások](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)