---
title: Tényleges egységár kiszámítása
ms.topic: how-to
ms.date: 04/02/2021
description: Megismeri a tényleges egységárat és számítását. Ez a cikk egy mintaszámítást is tartalmaz.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172217"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Az Azure-csomagfelhasználás tényleges egységárának kiszámítása

**Megfelelő szerepkörök**

- Számlázási adminisztrátor

## <a name="the-effective-unit-price"></a>A tényleges egységár

A tényleges egységár számítása a fogyasztásmérő szintjén történik (nem az erőforrás szintjén), és a mérőhasználat alapján naponta lesz módosítva.

A tényleges egységárat az alábbi három tényező alapján számítjuk ki:

- Felhasználás, amelyet naponta figyelnek a számlázási ciklus során
- A fogyasztásmérő számlázható költsége
- Rétegezés (ha van)

Mivel a használatot naponta monitorozni fogjuk a számlázási ciklusban, a tényleges egységár ingadozni fog. Az adott számlázási ciklus végső ára a használat kiszámításának leállítása és a számlázási időszak bezárása után lesz elérhető. A használat legtöbb változását a negyedik vagy ötödik tizedesjegy után fogja látni.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Annak kiderítése, hogy a fogyasztásmérő rétegzett díjszabást használ-e

Ha nem tudja, hogy a fogyasztásmérő rétegzett díjszabást használ-e, az alábbi eljárással derítse ki. 

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).
2. Válassza **az Értékesítés** lehetőséget, válassza a Díjszabás és **ajánlatok** lehetőséget, majd az **Azure-csomag díjszabása lehetőséget.**
3. Keresse meg a fogyasztásmérőt azonosító alapján, majd töltse le a díjszabási adatokat. 

## <a name="sample-calculation"></a>Mintaszámítás

Az alábbi táblázat egy példát mutat be arra, hogyan számítjuk ki a tényleges egységárat a nyitott időszakban.

A táblázatban a következő értékek érvényesek: 

- **UP** = az erőforrás óránkénti egységára = 0,868

- **BCU** = A fogyasztásmérő számlázható fogyasztási egysége

- **BC** = a fogyasztásmérő számlázható költsége = BCU * UP * 0,85. Ez a 15%-os PEC-kedvezmény kiigazítását tükrözi. Ezután a függvény alsó korlátját használva a tizedesvessző utáni két számjegyre korlátozjuk az értéket a minimális összeg felszámizálása érdekében. 

- **Tényleges egységár** = BCU/BC

>[!NOTE]

>Megjegyzés: Az ebben a példában található fogyasztásmérő nem rendelkezik tarifacsomagokkal vagy egyéb kedvezményekkel – a tényleges egységár a kedvezmény százalékos arányait és egyéb módosításokat is figyelembe veszi.


| Date | BCU (számlázható fogyasztási egység) | BC (számlázható költség) | Tényleges egységár |
| ------ | ----------- | ----------- | ----------- |  
| 3–Aug. | 29 | 21.39 | 0.737586206896552 |
| 10-Aug. | 210.950039 | 155.63 | 0.737757626107858 |
| 25-Aug. | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Következő lépések

- [Számlázás és adók](billing.md)
