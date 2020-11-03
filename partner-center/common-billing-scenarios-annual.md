---
title: Éves számlázás – gyakori forgatókönyvek
ms.topic: article
ms.date: 05/05/2020
description: Partneri Központ – éves számlázás – új előfizetések hozzáadásakor, licencek hozzáadása a számlázási dátum előtt, a licencek mennyiségének módosítása, illetve az előfizetések felfüggesztése/újraaktiválása.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 086a7d359e1b903684af4ecddac37eda584e55f8
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/17/2020
ms.locfileid: "92527998"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Közös éves számlázási forgatókönyvek a partner Centerben

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Számlázási adminisztrátor
- Segélyszolgálat ügynöke
- Értékesítési ügynök

A példában szereplő [általános számlázási forgatókönyvek](common-billing-scenarios.md) akkor érvényesek, ha az éves számlázást használja a partner Centerben.

## <a name="new-annual-subscription"></a>Új éves előfizetés

A számlázási dátum minden hónap 15. Január 13-án vásárolhat egy új előfizetést egy licenccel a $4/hónapra, és válassza az éves számlázás lehetőséget. A január 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Díjszabási díjak a vásárláskor|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Licenc hozzáadása az előfizetés évfordulójának dátuma és a számlázási dátum előtt

Egy új előfizetést vásárol a 2/11/17-es verzióban egy $211.20/év licenccel. Az előfizetés évfordulója minden hónap 11. napján van beállítva. A Microsoft számlázási rendszere a következő számlázási sorokat hozza létre:

- $211,20 a 2/11/17 – 2/10/18 időszakra vonatkozó díj.

2/12/17-on vásárol egy második licencet. A számlázási dátum 2/14/17. Létrejön egy számla-és egyeztetési fájl. Az egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma  |Díj befejezési dátuma  |Díj típusa  |Egységár |Mennyiség | Mennyiség |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Díjszabási díjak a vásárláskor |211,20 |1 | 211,20 |

Az előfizetése 3/11/17-es évfordulóján a Microsoft számlázási rendszere a következő számlázási sorokat hozza létre a 2/12/17-es licencek növeléséhez:

- $211,20 kredit a 2/11/17 – 2/10/18 időszakra.
- $0,58 a 2/11/17 – 2/11/17 időszakra vonatkozó licencelési díj 1 licenccel számolva.
- $15,62 a 2/12/17 – 3/10/2017 időszakra vonatkozó, 2 licenccel elszámolt díj.
- $195,00 a 3/11/2017 – 2/10/2018 időszakra vonatkozó, 2 licenccel elszámolt díj.

Az 2/11/17-es előfizetés megvásárlásakor. 2/12/17-on hozzáadunk egy licencet. A számlázási dátum 2/14/17. Az előfizetéshez tartozó 2/11/18-es verzióban.

A következő számlázási dátum 3/14/17, és létrejön egy számla & egyeztetési fájl. Az egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma  |Díj befejezési dátuma  |Díj típusa  |Egységár |Mennyiség | Mennyiség |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Ciklus példányának gyakorisága |– 211,20 |1 |– 211,20 |
|2/11/2017 |2/11/2017 |Ciklus példányának gyakorisága |0,58 |1 |0,58 |
|2/12/2017 |3/10/2017 |Ciklus példányának gyakorisága |15,62 |2 |31,25 |
|3/11/2017 |2/10/2018 |Ciklus példányának gyakorisága |195,00 |2 |390,00 |

Az előfizetés 2/11/18 egy másik 12 hónapos időszakra újítja meg az előfizetést.

## <a name="change-license-quantity"></a>Licenc mennyiségének módosítása

A számlázási dátum minden hónap 15. Január 13-án vásárolhat egy új előfizetést egy licenccel a $4/hónapra, és válassza az éves számlázás lehetőséget. A január 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Díjszabási díjak a vásárláskor|48,00|1|48,00

Február 1-jén növeljük a licencek mennyiségét egy-két értékre. A február 15-én a licenc-alapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ciklus példányának gyakorisága|– 48,00|1|– 48,00
1/13/2018|1/31/2018|Ciklus példányának gyakorisága|2,47|1|2,47
2/1/2018|1/12/2019|Ciklus példányának gyakorisága|44,98|2|89,96

Az éves díj 48,00, amely a 0,13 (48.00/365) napi árával egyenlő.

Egység ára = nap a szolgáltatási időszakban x napi díj x licencek száma.

A szolgáltatási időszakban 19 nap van: 1/13/2018 – 1/31/2018.

Ezért az egység ára = 2,47 (19x 0.13 X1)

346 nap van a szolgáltatási időszakban 2/1/2018 – 1/12/2019.

Ezért az egység ára = 44,98 (346x 0.13 x2)

## <a name="suspend-before-30-days"></a>Felfüggesztés 30 nap előtt

A számlázási dátum minden hónap 15. Január 13-án vásárolhat egy új előfizetést egy licenccel a $4/hónapra, és válassza az éves számlázás lehetőséget. A január 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Díjszabási díjak a vásárláskor|48,00|1|48,00

Február 1-jén felfüggesztheti az előfizetését. A február 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Megszakított díj|– 48,00|1|– 48,00

## <a name="suspend-after-30-days"></a>Felfüggesztés 30 nap után

A számlázási dátum minden hónap 15. Január 13-án vásárolhat egy új előfizetést egy licenccel a $4/hónapra, és válassza az éves számlázás lehetőséget. A január 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Díjszabási díjak a vásárláskor|48,00|1|48,00

A február 15-től a licenc-alapú egyeztető fájl nem tartalmaz számlázási sort ehhez az előfizetéshez.
Március 1-től felfüggesztheti az előfizetést. A március 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Megszakított díj|– 41,34|1|– 41,34

Az éves díj 48,00, amely a 0,13 (48.00/365) napi árával egyenlő.

Egység ára = nap a szolgáltatási időszakban x napi díj x licencek száma.

318 nap van a szolgáltatási időszakban 3/1/2018 – 1/12/2019.

Ezért az egység ára = 41,34 (318x 0.13 X1). Mivel ez egy kredit, az egység ára:-41,34.

## <a name="suspend-and-reactivate"></a>Felfüggesztés és újraaktiválás

A számlázási dátum minden hónap 15. Január 13-án vásárolhat egy új előfizetést egy licenccel a $4/hónapra, és válassza az éves számlázás lehetőséget. A január 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Díjszabási díjak a vásárláskor|48,00|1|48,00

Február 1-jén felfüggesztheti az előfizetését. A február 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Megszakított díj|– 48,00|1|– 48,00

Március 1-én aktiválja újra az előfizetését. A március 15-én a licenc-alapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj befejezési dátuma |Díj típusa |Egységár |Mennyiség |Mennyiség |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Díjszabási díjak a vásárláskor|41,34|1|41,34

Az éves díj 48,00, amely a 0,13 (48.00/365) napi árával egyenlő.

Egység ára = nap a szolgáltatási időszakban x napi díj x licencek száma.

318 nap van a szolgáltatási időszakban 3/1/2018 – 1/12/2019.

Ezért az egység ára = 41,34 (318x 0.13 X1).
