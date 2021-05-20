---
title: Egyszeri és ismétlődő & számlázása
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Partnerközpont egyszeri számlázási mintákat, majd az ismétlődő vásárlások kiválasztását – előfizetések vásárlásakor, további előfizetések hozzáadásakor, licencek hozzáadásakor vagy eltávolításakor.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a26b6e5299c5186959612e622808161ca0f7f7c2
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148618"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Partnerközpont egyszeri számlázási forgatókönyvek, és ismétlődő vásárlások kiválasztása

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Az | Értékesítési ügynök

Ezek gyakori [számlázási forgatókönyvek.](common-billing-scenarios.md) 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Előfizetés vásárlása és licenc hozzáadása ugyanazon a napon

Az 1. forgatókönyvben június 11-én vásárol egy 4 dolláros egységáron egy előfizetést. Ugyanezen a napon megvásárol egy másik előfizetést ugyanazon az áron.

A recon fájl a következőket tartalmazza:

- 4 USD számla a június 10-től július 9-ig időszakra.
- $4,00 USD időzített újrabetöltés a június 11–június 11. szolgáltatási időszakra. Ez az az időszak, amikor már volt licence. Számítás = (havi ár/szolgáltatási időszakban teljes nap) x nap az időzített szolgáltatási időszakban x licencek száma = (4/30) x 30 x 1 = 4,00.
- 8,00 USD időzített újrabetöltés a június 10– július 9. szolgáltatási időszakra. Ez az az időszak, amikor két licenccel rendelkezik. Számítás = (4/30) x 30 x 2 = 8,00.

|**Vásárlás dátuma**   |**Díj kezdete** |**Díj vége**  |**Egységár**  |**Mennyiség**  |**Összeg** |**Díj típusa** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |4 USD                |1                 |4 USD            |Új         |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        |1        | -$4       |addQuantity (hozzáadási szám)           |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        | 2      |8 USD         |addQuantity (hozzáadási szám)           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Előfizetés vásárlása és további előfizetések hozzáadása később

A 2. forgatókönyvben június 11-én vásárol egy előfizetést 4 dollár egységáron, június 12-én pedig vásárol egy másik előfizetést ugyanannak a terméknek ugyanazért az árért.

A recon fájl a következőket tartalmazza:

- 4 USD számla a június 10-től július 9-ig időszakra.
- $3,87 USD időzített újrabetöltés a június 11– június 12. szolgáltatási időszakra. Ez az az időszak, amikor egy licenccel rendelkezik. Számítás = (havi ár/szolgáltatási időszakban teljes nap) x nap az időzített szolgáltatási időszakban x licencek száma = (4/30) x 29 x 1 = 3,87.
- 7,74 USD időzített újrabetöltés a június 12– július 9. szolgáltatási időszakra. Ez az az időszak, amikor két licenccel rendelkezik. Számítás = (4/30) x 29 x 2 = 7,74.

|**Vásárlás dátuma**   |**Díj kezdete** |**Díj vége**  |**Egységár**  |**Mennyiség**  |**Összeg** |**Díj típusa** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019. 06. 11. (egy licenccel rendelkezik)     |6/10/2019   |7/09/2019         |4 USD         |1        |4 USD            |Új         |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 USD        |1        | -3,87 USD       |addQuantity (hozzáadási szám)           |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 USD        | 2      |7,74 DOLLÁR       |addQuantity (hozzáadási szám)           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Előfizetés vásárlása és licenc eltávolítása ugyanazon a napon

A 3. forgatókönyvben két előfizetést vásárol ugyanannak a terméknek a június 11-én, 4 dollár egységáron. Ugyanezen a napon eltávolítja az egyik licencet.  

A recon fájl a következőket tartalmazza:

- 8 dollár számla két licenchez a június 10-től július 9-ig érvényes szolgáltatási időszakra.
- 8,00 USD-s, időzített újrabetöltés a június 11. és június 11. szolgáltatási időszakra. Ez az az időszak, amikor két licenccel rendelkezik. Számítás = (havi ár/szolgáltatási időszakban teljes nap) x nap a szolgáltatási időszakban x licencek száma = (4/30) x 30 x 2 = 8,00.
- 4,00 USD időzített újrabetöltés a június 11–július 9. szolgáltatási időszakra. Ez az az időszak, amikor egy licenccel rendelkezik. Számítás = (4/30) x 30 x 1 = 4,00.

|**Vásárlás dátuma**   |**Díj kezdete** |**Díj vége**  |**Egységár**  |**Mennyiség**  |**Összeg** |**Díj típusa** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |4 USD                |2                 |8 DOLLÁR            |Új         |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        |2        | -8 USD       |removeQuantity (Quantity eltávolítása)           |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        | 1      |4 USD         |removeQuantity (Quantity eltávolítása)           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Előfizetés vásárlása és licencek eltávolítása később

A 4. forgatókönyvben két előfizetést vásárol június 11-én, 4 dollár egységáron, majd június 12-én eltávolítja az egyik licencet.

A recon fájl a következőket tartalmazza:

- 8 DOLLÁR számla a június 10. és július 9. szolgáltatási időszakra.
- 7,74 USD-s, időzített újratöltés a június 11–június 12. szolgáltatási időszakra. Ez az az időszak, amikor két licenccel rendelkezik. Számítás = (havi ár/szolgáltatási időszakban teljes nap) x nap a szolgáltatási időszakban x licencek száma = (4/30) x 29 x 2 = 7,74.
- 3,87 USD időzített újrabetöltés a június 12–július 9. szolgáltatási időszakra. Ez az az időszak, amikor egy licenccel rendelkezik. Számítás = (4/30) x 29 x 1 = 3,87.

|**Vásárlás dátuma**   |**Díj kezdete** |**Díj vége**  |**Egységár**  |**Mennyiség**  |**Összeg** |**Díj típusa** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019.06.11. (két licenccel rendelkezik)     |6/10/2019   |7/09/2019         |4 USD         |2        |8 USD       |Új       |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 USD        |2        | -7,74 USD       |removeQuantity (Quantity eltávolítása)           |
|2019.06.12. (egy licenccel rendelkezik)    | 6/10/2019    |7/09/2019   |4 USD    |1      |3,87 DOLLÁR    |removeQuantity (Quantity eltávolítása) |

## <a name="next-steps"></a>Következő lépések

- [Példák az új előfizetések havi számlázási forgatókönyveire, a licencmennyiség módosítására vagy felfüggesztésre](common-billing-scenarios-monthly.md)