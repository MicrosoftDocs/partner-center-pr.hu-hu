---
title: Érvényes egységár kiszámítása
ms.topic: how-to
ms.date: 11/10/2020
description: Ismerje meg a hatályos árat és a számítás módját. Egy minta számítást tartalmaz.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/11/2020
ms.locfileid: "94499137"
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
>Megjegyzés: az ebben a példában szereplő mérőszám nem rendelkezik a díjszabási csomaggal.

| Date | BCU (számlázható fogyasztási egység) | BC (számlázható díj) | Érvényes Egységár |
| ------ | ----------- | ----------- | ----------- |  
| 3 – augusztus | 29 | 21,39 | 0.737586206896552 |
| 10 – augusztus | 210,950039 | 155,63 | 0.737757626107858 |
| 25 – augusztus | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>További lépések

- [Számlázás és adók](billing.md)
