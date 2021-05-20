---
title: Éves számlázás – gyakori forgatókönyvek
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Partnerközpont számlázás – új előfizetések hozzáadásakor, licencek hozzáadása a számlázási dátum előtt, licencmennyiség módosítása vagy előfizetések felfüggesztése/újraaktiválása.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6392094e000b899e0545655ecf9ed6117535f7f
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148703"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Gyakori éves számlázási forgatókönyvek a Partnerközpont

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Az | Értékesítési ügynök

Ezek a [gyakori számlázási forgatókönyvek akkor](common-billing-scenarios.md) alkalmazhatók, ha éves számlázást használ a Partnerközpont.

## <a name="new-annual-subscription"></a>Új éves előfizetés

A számlázási dátum minden hónap 15-e. Január 13-án vásárol egy új előfizetést egy licenccel 4 USD/hónapért, és kiválasztja az éves számlázást. A január 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Díjfizetés vásárláskor|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Licenc hozzáadása az előfizetés évfordulója után, de még a számlázási dátum előtt

Egy új előfizetést vásárol 2017. 02. 11-én, évi 211,20 dolláros licenccel. Az előfizetés évfordulója minden hónap 11. napjaként van beállítva. A Microsoft számlázási rendszere a következő számlázási sorokat hozza létre:

- 211,20 dollár díj a 2. 17. 02. 11. időszakban – 2/10/18. időszakban.

2017. 02. 12-én vásárol egy második licencet. A számlázási dátum: 2/14/17. Létrejön egy számla és egy egyeztetési fájl. Az egyeztetési fájl a következő számlázási sorokat tartalmazza:

|Díj kezdő dátuma  |Díj záró dátuma  |Díj típusa  |Egységár |Mennyiség | Összeg |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Vásárláskor fizetendő díjak |211.20 |1 | 211.20 |

Az előfizetés évfordulóján( 2017.03.11.) a Microsoft számlázási rendszere a következő számlázási sorokat hozza létre a licenc 2017. október 12-én való növeléséhez:

- 211,20 USD kredit a 2.11.17. időszakra – 2/10/18. időszakra.
- Licencenként 0,58 USD időzített díj licencenként, 2/11/17– 2/11/17 időszakra.
- Licencenként 15,62 USD időzített díj két licencre vonatkozóan 2017. 02. 12. 17. – 2017. 03. 10. időszakban.
- Licencenként 195,00 USD időzített díj két licencre vonatkozóan 2017. 03. 11. – 2018. 02. 10. időszakban.

2017. 02. 11-én vásárol egy előfizetést. 2017. október 12-én hozzáad egy licencet. A számlázási dátum 2/14/17. Az előfizetés megújítása 2018. 02. 11-én megújul.

A következő számlázási dátum 3/14/17, és létrejön egy számla és egy egyeztetési fájl. Az egyeztetési fájl a következő számlázási sorokat tartalmazza:

|Díj kezdő dátuma  |Díj záró dátuma  |Díj típusa  |Egységár |Mennyiség | Összeg |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Cycle Instance Prorate |-211.20 |1 |-211.20 |
|2/11/2017 |2/11/2017 |Cycle Instance Prorate |0.58 |1 |0.58 |
|2/12/2017 |3/10/2017 |Cycle Instance Prorate |15.62 |2 |31.25 |
|3/11/2017 |2/10/2018 |Cycle Instance Prorate |195.00 |2 |390.00 |

A 2/11/18-án az előfizetés egy újabb 12 hónapos időszakra újul meg.

## <a name="change-license-quantity"></a>Licenc mennyiségének módosítása

A számlázási dátum minden hónap 15-e. Január 13-án vásárol egy új előfizetést egy licenccel 4 USD/hónapért, és kiválasztja az éves számlázást. A január 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Díjfizetés vásárláskor|48.00|1|48.00

Február 1-jén 1-ről 2-re növeli a licencmennyiséget. A február 15-i licencalapú egyeztetési fájl a következő számlázási sorokat fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Cycle Instance Prorate|-48.00|1|-48.00
1/13/2018|1/31/2018|Cycle Instance Prorate|2.47|1|2.47
2/1/2018|1/12/2019|Cycle Instance Prorate|44.98|2|89.96

Az éves ár 48,00, amely a 0,13 (48,00/365) napi árnak megfelelő.

Egységár = szolgáltatási időszak napjai x napi ár x licencek száma.

A szolgáltatási időszak 19 napja 2018.01.13. – 2018.01.31.

Ezért az egységár = 2,47 (19x0,13x1)

A szolgáltatási időszak 2018. 02. 01. – 2019.01.12.

Ezért az egységár = 44,98 (346x0,13x2)

## <a name="suspend-before-30-days"></a>Felfüggesztés 30 nap előtt

A számlázási dátum minden hónap 15-e. Január 13-án vásárol egy új előfizetést egy licenccel 4 USD/hónapért, és kiválasztja az éves számlázást. A január 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Díjfizetés vásárláskor|48.00|1|48.00

Február 1-jén felfüggeszti az előfizetését. A február 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Lemondási díj|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Felfüggesztés 30 nap után

A számlázási dátum minden hónap 15- edike. Január 13-án vásárol egy új előfizetést egy licenccel 4 USD/hóért, és kiválasztja az éves számlázást. A január 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Díjfizetés vásárláskor|48.00|1|48.00

A február 15-i licencalapú egyeztetési fájl nem tartalmaz számlázási sorokat ehhez az előfizetéshez.
Március 1-jén felfüggeszti az előfizetését. A március 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Lemondási díj|-41.34|1|-41.34

Az éves ár 48,00, amely a 0,13 napi árat (48,00/365) jelenti.

Egységár = szolgáltatási időszak napjai x napi ár x licencek száma.

A szolgáltatási időszak 318 napja 2018. 03. 1. – 2019.01.12.

Ezért az egységár = 41,34 (318x0,13x1). Mivel ez egy kredit, az egységár -41,34.

## <a name="suspend-and-reactivate"></a>Felfüggesztés és újraaktiválás

A számlázási dátum minden hónap 15-e. Január 13-án vásárol egy új előfizetést egy licenccel 4 USD/hónapért, és kiválasztja az éves számlázást. A január 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Díjfizetés vásárláskor|48.00|1|48.00

Február 1-jén felfüggeszti az előfizetését. A február 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Lemondási díj|-48.00|1|-48.00

Március 1-jén újraaktiválhatja az előfizetését. A március 15-i licencalapú egyeztetési fájl a következő számlázási sort fogja tartalmazni:

|Díj kezdő dátuma |Díj záró dátuma |Díj típusa |Egységár |Mennyiség |Összeg |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Díjfizetés vásárláskor|41.34|1|41.34

Az éves ár 48,00, amely a 0,13 napi árat (48,00/365) jelenti.

Egységár = szolgáltatási időszak napjai x napi ár x licencek száma.

A szolgáltatási időszak 318 napja 2018. 03. 1. – 2019.01.12.

Ezért az egységár = 41,34 (318x0,13x1).
