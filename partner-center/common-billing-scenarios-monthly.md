---
title: Gyakori havi számlázási forgatókönyvek
ms.topic: article
ms.date: 05/13/2020
description: Gyakori forgatókönyvek a partner Centerben, ha havi számlázást használ – új előfizetések hozzáadását, a licencek mennyiségének módosítását és az előfizetések felfüggesztését foglalja magában.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 05c46faa3fd012677b615caa228cf4f7c6fe6c90
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354576"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Havi számlázási forgatókönyvek az új előfizetésekhez, a licencek összegének módosításához vagy a felfüggesztésekhez

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Számlázási adminisztrátor
- Segélyszolgálat ügynöke
- Értékesítési ügynök

Ezek a [gyakori számlázási forgatókönyvek](common-billing-scenarios.md) akkor érvényesek, ha havi számlázást használ a partner Centerben.

## <a name="new-monthly-subscription"></a>Új havi előfizetés

A számlázási dátum minden hónap 15. Január 13-án vásárolhat egy új előfizetést egy licenccel a $4/month számára, és kiválasztja a havi számlázást. A január 15-én a licenc-alapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Ciklus díja   |4,00       |1        |4,00 |

A február 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Ciklus díja   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Licenc mennyiségének módosítása

A számlázási dátum minden hónap 15. Január 13-án vásárolhat egy új előfizetést egy licenccel a $4/month számára, és kiválasztja a havi számlázást. A január 15-én a licenc-alapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Ciklus díja   |4,00       |1        |4,00    |

Február 1-jén növeljük a licencek mennyiségét egy-két értékre. A február 15-én a licenc-alapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Ciklus példányának gyakorisága   |– 4,00       |1        |– 4,00   |
|1/13/2018         |1/31/2018    | Ciklus példányának gyakorisága   |2.45       |1        |2.45    |
|2/1/2018         |2/12/2018    | Ciklus példányának gyakorisága   |1.55       |2        |3,10    |
|2/13/2018         |3/12/2018    | Ciklus példányának gyakorisága   |4,00       |2        |8,00    |

A havi díj 4,00, a 1/13/2018 – 2/12/2018 szolgáltatási időszakban pedig 31 nap van. Ez a 0,129-as napi díj (4/31) értéknek felel meg.

A 1/13/2018 – 1/31/2018 arányban 19 nap áll rendelkezésre.

Ration Unit Price = 2,451 = 19 x 0,129

12 nap van a 2/1/2018 – 2/12/2018 arányban.

Ration Unit Price = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Felfüggesztés 30 nap előtt

A számlázási dátum minden hónap 15. Január 13-án vásárolhat egy új előfizetést egy licenccel a $4/month számára, és kiválasztja a havi számlázást. A január 15-én a licenc-alapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Ciklus díja   |4,00       |1        |4,00    |

Február 1-jén felfüggesztheti az előfizetést. A február 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Megszakított díj|– 4,00|1|– 4,00

## <a name="suspend-after-30-days"></a>Felfüggesztés 30 nap után

A számlázási dátum minden hónap 15. Január 13-án vásárolhat egy új előfizetést egy licenccel a $4/month számára, és kiválasztja a havi számlázást. A január 15-én a licenc-alapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Ciklus díja|4,00|1|4,00

A február 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Ciklus díja|4,00|1|4,00

Március 1-én felfüggesztheti az előfizetést. A március 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Megszakított díj|– 1,72|1|– 1,72

A havi díj 4,00, a 2/13/2018 – 3/12/2018 szolgáltatási időszakban pedig 28 nap van. Ez a 0,143-as napi díj (4/28) értéknek felel meg.

Egység ára = nap a szolgáltatási időszakban x napi díj x licencek száma.

A 3/1/2018 – 3/12/2018 megszakítási időszakban 12 nap van.

Ezért az egység ára =-1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Következő lépések

- [Számlázási forgatókönyvek egyszeri használatra és az ismétlődő vásárlások kiválasztása](common-billing-scenarios-onetime-recurring.md)