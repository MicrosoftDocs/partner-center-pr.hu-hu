---
title: Tényleges egységár kiszámítása
ms.topic: how-to
ms.date: 04/02/2021
description: Ismerje meg a hatályos egység árát és a számítás módját. Ez a cikk egy minta számítást is tartalmaz.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a662e0b815c979b3454762c5b35eb510887c96ad
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374392"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Az Azure-csomag felhasználásának tényleges számítási egysége

## <a name="the-effective-unit-price"></a>A hatályos egység ára

A tényleges egység árát a mérési szint alapján számítjuk ki (az erőforrás szintjével szemben), és napi rendszerességgel korrigáljuk a mérési adatok alapján.

A következő három tényezővel számítjuk ki a hatályos egység árát:

- A teljes számlázási ciklusban naponta figyelt felhasználás
- A fogyasztásmérő számlázandó díja
- Rétegek (ha alkalmazható)

Mivel napi rendszerességgel figyeli a használatot a számlázási időszakban, a hatályos egység ára ingadozni fog. Az adott elszámolási időszakra vonatkozó végleges díj a felhasználás kiszámításának leállítása és a számlázási idő lezárása után lesz elérhető. A legtöbb változást a negyedik vagy az ötödik tizedesjegy után fogja látni.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Megtudhatja, hogy a mérőszám a lépcsőzetes díjszabást használja-e

Ha nem tudja, hogy a mérőszáma a lépcsőzetes díjszabást használja-e, az alábbi eljárással derítheti ki. 

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).
2. Válassza az **értékesítés** lehetőséget, válassza a **díjszabás és ajánlatok** lehetőséget, majd válassza az **Azure-csomag díjszabása** lehetőséget.
3. Keresse meg a mérőt azonosító alapján, majd töltse le a díjszabási adatait. 

## <a name="sample-calculation"></a>Minta kiszámítása

Az alábbi táblázat bemutatja, hogyan számítjuk ki a hatályos egység árát a nyitott időszak alatt.

A táblázatban a következő értékek érvényesek: 

- **Up** = az erőforrás egységenkénti ára/óra = 0,868

- **BCU** = a mérőhöz tartozó számlázható fogyasztási egység

- **BC** = a mérőhöz tartozó számlázandó díj = BCU * fel * 0,85. Ez megfelel a 15%-os PEC kedvezmény beállításának. Ezután a függvény alsó határát használjuk az értéknek a tizedesvessző utáni két számjegyre való korlátozásához a minimális mennyiség kiszámításához. 

- **Érvényes egységár** = BCU/BC

>[!NOTE]
>Az ebben a példában szereplő mérőszámhoz nem tartoznak díjszabási szintek. A hatályos egység díjszabása a kedvezmények százalékában és egyéb beállításokban.

| Date | BCU (számlázható fogyasztási egység) | BC (számlázható díj) | Érvényes Egységár |
| ------ | ----------- | ----------- | ----------- |  
| 3 – augusztus | 29 | 21,39 | 0.737586206896552 |
| 10 – augusztus | 210,950039 | 155,63 | 0.737757626107858 |
| 25 – augusztus | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>Következő lépések

- [Számlázás és adók](billing.md)
