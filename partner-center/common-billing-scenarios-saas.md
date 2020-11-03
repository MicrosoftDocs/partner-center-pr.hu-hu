---
title: Számlázási licenc alapú SaaS-tranzakciók
ms.topic: article
ms.date: 05/05/2020
description: Ismerje meg az általános számlázási forgatókönyveket a partnervállalat licencelési, szoftveres (SaaS) tranzakciói esetében.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d63e8345bf127cb91f1812193b1f0311cd569b3
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/14/2020
ms.locfileid: "92530301"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Általános számlázási forgatókönyvek a fiókpartner licenc alapú SaaS-tranzakciói esetén

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Számlázási adminisztrátor
- Segélyszolgálat ügynöke
- Értékesítési ügynök


Ezek a [gyakori számlázási forgatókönyvek](common-billing-scenarios.md) a fiókpartner szolgáltatásként (SaaS) való előfizetésekre érvényesek.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Ingyenes próbaverziós SaaS-előfizetés átalakítása fizetős előfizetésre

Ez a forgatókönyv a licenc-alapú ingyenes próbaverziós SaaS-előfizetés megújítására vonatkozó számlázást ismerteti. A megújítás az ingyenes próbaidőszak végén átalakítja az ingyenes próbaverziót egy fizetős előfizetésre.

Ebben a példában a licenc-alapú SaaS (szoftveres szolgáltatás) előfizetésének ingyenes próbaverzióját vásárolta, június 10-én. Ez az ingyenes próbaverzió automatikusan megújítva fizetett előfizetésként az ingyenes próbaidőszak lejárta után.

A Recon-fájlok a következő díjakat tartalmazzák:

| Vásárlás dátuma | Díj kezdő dátuma | Díj befejezési dátuma | Egységár | Egység mennyisége | Teljes összeg | Díj típusa | Előfizetés leírása |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 1 | 0 USD | Új | Ingyenes próbaidőszak |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | $2 | 1 | $2 | Frissítés | Fizetős előfizetés |

## <a name="cancel-a-free-trial-saas-subscription"></a>Ingyenes próbaverziós SaaS-előfizetés megszakítása

> [!TIP]
> A licenc-alapú ingyenes próbaverziós SaaS-előfizetés bármikor lemondható, még az ingyenes próbaidőszak során is.

Ebben a forgatókönyvben egy licenccel rendelkező ingyenes próbaverziós SaaS-előfizetést vásárolt július 1-jén, majd azonnal megszakították a partner Centerben.

A Recon-fájl a következő díjakat fogja tartalmazni:

| Vásárlás dátuma | Díj kezdő dátuma | Díj befejezési dátuma | Egységár | Egység mennyisége | Teljes összeg | Díj típusa | Előfizetés leírása |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Új | Ingyenes próbaidőszak |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Mégse | Ingyenes próbaidőszak |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Egyéni fogyasztásmérő SaaS-előfizetés átalakítása másik SKU-ra

Ez a forgatókönyv azt ismerteti, hogyan alakíthat át egy egyéni fogyasztásmérő SaaS-előfizetést egy adott készletet tartalmazó egységből egy másik SKU-ra ugyanarra a termékre vonatkozóan ugyanazon a napon.

Ebben a forgatókönyvben egy termék keretében vásárolt egy SKU-t (Silver), és átalakította egy másik elérhető SKU-ra (Bronzra) a termék keretében ugyanezen a napon belül.

A Recon-fájl a következő díjakat fogja tartalmazni:

| Vásárlás dátuma | Termékváltozat | Díj kezdő dátuma | Díj befejezési dátuma | Egységár | Egység mennyisége | Teljes összeg | Díj típusa | Előfizetés leírása |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Ezüst | 06/10/2019 | 06/10/2019 | 20 USD | 1 | 20 USD | Új | Egyéni fogyasztásmérő SaaS-előfizetés |
| 06/10/2019 | Ezüst | 06/10/2019 | 06/10/2019 | 20 USD | 1 | – $20 | Konvertálás | Arányos számlázás az egyéni fogyasztásmérő SaaS-előfizetéséhez |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Konvertálás | Egyéni fogyasztásmérő SaaS-előfizetés |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Ügyfél-fogyasztásmérő SaaS-előfizetés megvásárlása és megszakítása ugyanazon a napon

Ez a forgatókönyv a megvásárolt és a Azure Portalon megszakított ügyfél-fogyasztásmérő SaaS-előfizetés számlázását ismerteti ugyanazon a napon.

Ebben a forgatókönyvben egyéni fogyasztásmérő SaaS-előfizetést vásárolt a Azure Portal. Ezután megszakította az előfizetést ugyanarra a dátumra.

| Vásárlás dátuma | Termékváltozat | Díj kezdő dátuma | Díj befejezési dátuma | Egységár | Egység mennyisége | Teljes összeg | Díj típusa | Előfizetés leírása |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Új | Egyéni fogyasztásmérő SaaS-előfizetés |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10 USD | 1 | – $10 | CancelImmediate | Egyéni fogyasztásmérő SaaS-előfizetés |
