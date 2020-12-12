---
title: Egyszeri & ismétlődő vásárlások számlázása
ms.topic: article
ms.date: 05/05/2020
description: A partner Center számlázási mintái egyszeri és ismétlődő vásárlások esetén – Előfizetések vásárlása esetén további előfizetések hozzáadása, licencek hozzáadása vagy eltávolítása.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a301aa85310142b3327baabbf3c8545b31f489bd
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354389"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>A partner Center számlázási forgatókönyvei egyszeri használatra és az ismétlődő vásárlások kiválasztása

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Számlázási adminisztrátor
- Segélyszolgálat ügynöke
- Értékesítési ügynök

Ezek [általános számlázási forgatókönyvek](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Előfizetés vásárlása és licenc hozzáadása ugyanazon a napon

Az 1. forgatókönyvben a $4-es egységáron vásárolhat meg egy előfizetést. Később ugyanezen az előfizetésen belül ugyanazon az áron vásárolhatja meg a másikat.

A Recon-fájl a következőket tartalmazza:

- $4 számla a szolgáltatási időszakban, június 10 – július 9.
- $-4,00, arányosan elszámolt, a szolgáltatási időszak 11. június 11. Ez az az időszak, amikor 1 licenccel rendelkezett. Számítás = (havi díj/teljes nap a szolgáltatási időszakban) x nap az elszámolású szolgáltatási időszakban x licencek száma = (4/30) x 30 x 1 = 4,00.
- $8,00 arányosan elszámolt kiszámlázva a szolgáltatási időszakban, június 10 – július 9. Ez az az időszak, amikor 2 licenccel rendelkezett. Számítás = (4/30) x 30 x 2 = 8,00.

|**Vásárlás dátuma**   |**Díj kezdete** |**Díj vége**  |**Egység ára**  |**Mennyiség**  |**Mennyiség** |**Díj típusa** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |Új         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | – $4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Előfizetés vásárlása és további előfizetések hozzáadása később

A 2. forgatókönyvben egy, a $4-es egységáron vásárolt előfizetést, és június 12-én megvásárolt egy másik előfizetést ugyanarra a termékre, ugyanazon az áron.

A Recon-fájl a következőket tartalmazza:

- $4 számla a szolgáltatási időszakban, június 10 – július 9.
- $-3,87 arányosan elszámolt, a szolgáltatási időszakra vonatkozó, 11. június 12. Ez az az időszak, amikor 1 licenccel rendelkezett. Számítás = (havi díj/teljes nap a szolgáltatási időszakban) x nap az elszámolású szolgáltatási időszakban x licencek száma = (4/30) x 29 x 1 = 3,87.
- $7,74 a szolgáltatási időszakra vonatkozó, 12 – július 9. Ez az az időszak, amikor 2 licenccel rendelkezett. Számítás = (4/30) x 29 x 2 = 7,74.

|**Vásárlás dátuma**   |**Díj kezdete** |**Díj vége**  |**Egység ára**  |**Mennyiség**  |**Mennyiség** |**Díj típusa** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (egy licenccel rendelkezik)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Új         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | – $3,87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7,74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Előfizetés vásárlása és licencek eltávolítása ugyanazon a napon

A 3. forgatókönyvben két előfizetést vásárol ugyanarra a termékre, a $4-es egység ára szerint. Később ugyanezen a napon törölheti az egyik licencet.  

A Recon-fájl a következőket tartalmazza:

- $8 számla két, a szolgáltatási időszakra vonatkozó, 10 – július 9 licenchez.
- $-8,00, arányosan elszámolt, a szolgáltatási időszak 11. június 11. Ez az az időszak, amikor 2 licenccel rendelkezett. Számítás = (havi díj/teljes nap a szolgáltatási időszakban) x nap az elszámolású szolgáltatási időszakban x licencek száma = (4/30) x 30 x 2 = 8,00.
- $4,00 arányosan elszámolt, a szolgáltatási időszak 11 – július 9. Ez az az időszak, amikor 1 licenccel rendelkezett. Számítás = (4/30) x 30 x 1 = 4,00.

|**Vásárlás dátuma**   |**Díj kezdete** |**Díj vége**  |**Egység ára**  |**Mennyiség**  |**Mennyiség** |**Díj típusa** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |Új         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | – $8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Előfizetés vásárlása és licencek eltávolítása később

A 4. forgatókönyvben 2 előfizetést vásárol a $4-es egységáron, és június 12-én törli az egyik licencet.

A Recon-fájl a következőket tartalmazza:

- $8 számla a szolgáltatási időszakban, június 10 – július 9.
- $-7,74 arányosan elszámolt, a szolgáltatási időszakra vonatkozó, 11. június 12. Ez az az időszak, amikor 2 licenccel rendelkezett. Számítás = (havi díj/teljes nap a szolgáltatási időszakban) x nap az elszámolású szolgáltatási időszakban x licencek száma = (4/30) x 29 x 2 = 7,74.
- $3,87 a szolgáltatási időszakra vonatkozó, 12 – július 9. Ez az az időszak, amikor 1 licenccel rendelkezett. Számítás = (4/30) x 29 x 1 = 3,87.

|**Vásárlás dátuma**   |**Díj kezdete** |**Díj vége**  |**Egység ára**  |**Mennyiség**  |**Mennyiség** |**Díj típusa** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (2 licenccel rendelkezik)     |6/10/2019   |7/09/2019         |$4         |2        |$8       |Új       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | – $7,74       |removeQuantity           |
|6/12/2019 (1 licenccel rendelkezik)    | 6/10/2019    |7/09/2019   |$4    |1      |$3,87    |removeQuantity |

## <a name="next-steps"></a>Következő lépések

- [Havi számlázási forgatókönyvek az új előfizetésekhez, a licencek összegének módosításához vagy a felfüggesztésekhez](common-billing-scenarios-monthly.md)