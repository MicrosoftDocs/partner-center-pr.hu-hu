---
title: A .csv-fájl mezői több felhasználó importálása egy ügyfélfiókhoz
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ha több felhasználót szeretne hozzáadni egy ügyfélfiókhoz, hozzon létre egy vesszővel elválasztott értékfájlt (.csv) a megfelelő mezőkkel.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150981"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Több felhasználó hozzáadása egy ügyfélfiókhoz egy .csv-fájl létrehozásával

**Megfelelő szerepkörök:** Globális rendszergazda

Egyszerre több felhasználót is hozzáadhat egy ügyfél fiókjához úgy, hogy feltölt egy vesszővel elválasztott értékfájlformátumban (.csv) egy adatfájlt a Partnerközpont. Letölthet egy mintaadatfájlt a Partnerközpont majd saját használatra szerkesztheti, vagy létrehozhat egy új adatfájlt az alább definiált adatmodellel.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Adatfájlokkal kapcsolatos követelmények

Ha több felhasználót szeretne hozzáadni egy ügyfél fiókjához a tömeges feltöltési folyamattal, meg kell felelnie a következő követelményeknek:

- Globális rendszergazdai engedélyekkel kell rendelkeznie az ügyfélfiókhoz;
- Minden felhasználónak egyedi e-mail-címmel kell rendelkezik, amely az ügyfél e-mail-tartománya(i)hoz van hozzáfűzve;
- Egyszerre legfeljebb 100 rekordot tölthet fel. Ha több mint 100 felhasználót kell hozzáadnia, hozzon létre és töltsön fel további adatfájlokat.
- Minden felhasználónak azonos földrajzi helyen kell **lennie.**
- Csak az alább leírt adatokat adja meg. A felesleges adatok miatt a feltöltés sikertelen lesz.

Adja meg a következő adatokat az adatfájlban:

| **Oszlop neve** | **Leírás**  | **Korlátozás**  |
|:-------- |:------  |:----- |
| Utónév  | Felhasználó vezetékneve (nem kötelező mező)  | 50 karakteres korlát  |
| Vezetéknév  | Felhasználó vezetékneve (nem kötelező mező)  | 50 karakteres korlát  |
| Megjelenített név    | A név megjelenik a Partnerközpont (kötelező mező)                            | 50 karakteres korlát                         |
| E-mail   | A felhasználó vállalati e-mail-címe az ügyfél vállalatnál (kötelező mező)           | Minden felhasználónak egyedi e-mail-címmel kell |
| Állapotfrissítés   | Annak jelzésére használatos, hogy az új felhasználói rekord sikeresen létrejött-e | \*\*Hagyja üresen\*\*                        |

## <a name="next-steps"></a>Következő lépések

- [Több felhasználó hozzáadása egy ügyfélhez](adding-multiple-users-to-a-customer-account.md)