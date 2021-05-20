---
title: Gyakori havi számlázási forgatókönyvek
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A havi Partnerközpont használatának gyakori forgatókönyvei – ide tartozik az új előfizetések hozzáadása, a licencmennyiség módosítása és az előfizetések felfüggesztése.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66c9ec09f707d87248fdef31e4cf66f4ca927ce1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148652"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Példák az új előfizetések havi számlázási forgatókönyveire, a licencösszegek módosítására vagy felfüggesztésre

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Az | Értékesítési ügynök

Ezek a [gyakori számlázási forgatókönyvek akkor](common-billing-scenarios.md) alkalmazhatók, ha havi számlázást használ a Partnerközpont.

## <a name="new-monthly-subscription"></a>Új havi előfizetés

A számlázási dátum minden hónap 15-e. Január 13-án vásárol egy új előfizetést egy licenccel 4 USD/hónapért, és kiválasztja a havi számlázást. A január 15-i licencalapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Ciklus díja   |4,00       |1        |4,00 |

A február 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Ciklus díja   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Licenc mennyiségének módosítása

A számlázási dátum minden hónap 15- edike. Január 13-án vásárol egy új előfizetést egy licenccel 4 USD/hóért, és kiválasztja a havi számlázást. A január 15-i licencalapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Ciklus díja   |4,00       |1        |4,00    |

Február 1-jén 1-ről 2-re növeli a licencmennyiséget. A február 15-i licencalapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Cycle Instance Prorate   |-4.00       |1        |-4.00   |
|1/13/2018         |1/31/2018    | Cycle Instance Prorate   |2.45       |1        |2.45    |
|2/1/2018         |2/12/2018    | Cycle Instance Prorate   |1.55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Cycle Instance Prorate   |4,00       |2        |8.00    |

A havi ár 4,00, és a szolgáltatási időszak 31 napja 2018.01.13. – 2018.02.12. Ez 0,129 (4/31) napi árat jelent.

A prorációs időszakban 19 nap 2018.01.13. – 2018.01.31.

Proration unit price = 2.451 = 19 x 0.129

A prorációs időszakban 12 nap van 2018. 02. 01. – 2018. 02. 12.

Proration unit price = 1.54 = 12 x 0.129

## <a name="suspend-before-30-days"></a>Felfüggesztés 30 nap előtt

A számlázási dátum minden hónap 15-e. Január 13-án vásárol egy új előfizetést egy licenccel 4 USD/hónapért, és kiválasztja a havi számlázást. A január 15-i licencalapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Ciklus díja   |4,00       |1        |4,00    |

Február 1-jén felfüggeszti az előfizetést. A február 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Lemondási díj|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Felfüggesztés 30 nap után

A számlázási dátum minden hónap 15-e. Január 13-án vásárol egy új előfizetést egy licenccel 4 USD/hónapért, és kiválasztja a havi számlázást. A január 15-i licencalapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Ciklus díja|4,00|1|4,00

A február 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Ciklus díja|4,00|1|4,00

Március 1-jén felfüggeszti az előfizetést. A március 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Lemondási díj|-1.72|1|-1.72

A havi ár 4,00, és a szolgáltatási időszak 28 napja 2018.02.13. – 2018.03.12. Ez 0,143 (4/28) napi árat jelent.

Egységár = szolgáltatási időszak napjai x napi ár x licencek száma.

A lemondási időszakban 12 nap van 2018. 03. 01. – 2018. 03. 12.

Ezért az egységár = -1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Következő lépések

- [Számlázási forgatókönyvek egyszeri vásárláshoz és ismétlődő vásárlások kiválasztása](common-billing-scenarios-onetime-recurring.md)