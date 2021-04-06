---
title: A. csv fájl mezői több felhasználó importálásához egy ügyfél-fiókhoz
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ha több felhasználót szeretne felvenni egy ügyfél-fiókba, hozzon létre egy vesszővel tagolt (. csv) fájlt a megfelelő mezőkkel.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441421"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Egy. csv-fájl létrehozásával több felhasználót is hozzáadhat egy felhasználói fiókhoz

**Megfelelő szerepkörök**

- Globális rendszergazda

Egyszerre több felhasználót is hozzáadhat egy ügyfél fiókjához, ha a vesszővel tagolt fájlformátumban (. csv) egy adatfájlt tölt fel a partner központba. Letölthet egy minta adatfájlt a partner központjából, és szerkesztheti a saját használatra, vagy létrehozhat egy új adatfájlt az alább meghatározott adatmodell használatával.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Az adatfájlra vonatkozó követelmények

Ha több felhasználót szeretne hozzáadni egy ügyfél fiókjához a tömeges feltöltési folyamat használatával, a következő követelményeknek kell megfelelnie:

- Globális rendszergazdai engedélyekkel kell rendelkeznie az ügyfél fiókhoz;
- Minden felhasználónak rendelkeznie kell egy egyedi e-mail-címmel, amely az ügyfél e-mail-tartományához van hozzáfűzve;
- Egyszerre akár 100 rekordot is feltölthet. Ha több mint 100 felhasználót kell felvennie, hozzon létre és töltsön fel további adatfájlokat.
- Minden felhasználónak ugyanabban a földrajzi **helyen** kell lennie.
- Csak az alábbiakban ismertetett adattípusokat adja meg. A külső adatok miatt a feltöltés sikertelen lesz.

Adja meg az adatfájl következő értékeit:

| **Oszlop neve** | **Leírás**  | **Korlátozás**  |
|:-------- |:------  |:----- |
| Utónév  | Felhasználó vezetékneve (nem kötelező mező)  | 50 – karakteres korlát  |
| Vezetéknév  | Felhasználó vezetékneve (nem kötelező mező)  | 50 – karakteres korlát  |
| Megjelenített név    | A partner Centerben megjelenő név (kötelező mező)                            | 50 – karakteres korlát                         |
| E-mail   | Felhasználó üzleti e-mail-címe az ügyfél cégnél (kötelező mező)           | Minden felhasználónak egyedi e-mail-címmel kell rendelkeznie |
| Állapot frissítése   | Annak jelzésére szolgál, hogy az új felhasználói rekord létrehozása sikerült-e | \*\*Hagyja üresen\*\*                        |

## <a name="next-steps"></a>Következő lépések

- [Több felhasználó hozzáadása egy ügyfélhez](adding-multiple-users-to-a-customer-account.md)