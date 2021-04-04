---
title: A partner Center számlázási számláinak megismerése
ms.topic: article
ms.date: 05/18/2020
description: A számlázási fájl mezőinek megismerése a partner Center számlázása során. Ide tartoznak a mezők és a definíciók az összes számlázási mezőhöz és az egyszeri díj mezőhöz.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 44bda5256b14722f143a5bf937e73b2533b8c9f5
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "106178901"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>A partner Center számlázási számla mezőinek megismerése

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói felügyeleti rendszergazda
- Számlázási adminisztrátor
- Segélyszolgálat ügynöke

A következő táblázatok segítségével megismerheti a partner Center-számlázási fájlok mezőit.

## <a name="invoice-file-fields"></a>Számlázandó fájl mezői

A következő mezők jelennek meg a számlázási fájlokban.

| Mező | Meghatározás |
| ----- | ---------- |
| USA-BELI FEIN | A szövetségi munkaadó azonosító száma (FEIN). Ez a Egyesült Államok Szövetségi adóazonosító szám. |
| Ügyfél száma | Az ügyfél száma. |
| Bill to (Számlázási cím) | Az a címe, ahová elküldjük a számláját. A partner Center számlázási profiljában módosíthatja a vállalat nevét és címeit. |
| Licenc-alapú díjak | A vásárolt használaton alapuló licencek havi vagy éves díja, a szolgáltatás előzetes számlázása után. Ez a szám a licenc-alapú egyeztetési fájlban lévő **Részösszeg** oszlopban (a **T** oszlop) lévő összes költség összegét adja meg. |
| Használati alapú díjak | Az Azure-használat. Ez magában foglalja a számlázási időszakban engedélyezett és használt új szolgáltatásokat vagy alkalmazásokat. Ez a szám a **PretaxCharges** oszlop ( **Z**) oszlopban szereplő összes díj összege a használaton alapuló egyeztetési fájlban. |
| Discounts (Engedmények) | Az ügyfél által az előfizetés normál árán kapott kedvezmény. Ez a szám *átalányösszegként* jelenik meg, nem pedig egységenként vagy licenccel. |
| Kreditek | Az előfizetések módosításaira vonatkozó kreditek vagy módosítások (például a licencek növekedése vagy csökkentése). |
| Részösszeg | Adók és adómentes költségek és kreditek összege. |
| Adó | Az aktuális díjak teljes adója, amely a számla 2. oldalán kezdődő **részletek** szakaszban látható. Ez a szám a **TaxAmount** oszlopban szereplő összes díj ( **AA** oszlop) összege a használaton alapuló egyeztetési fájlban, valamint a licenc-alapú egyeztetési fájlban lévő **Tax** oszlop ( **U** oszlop). |
| Egyéb kreditek | Adó-kizárólagos kreditek. |
| Aktuális díjak összesen | A számlázási időszak számlázási pénznemében esedékes összeg. Ezeket a díjakat a fizetés határideje okozza. |
| Payment Instructions (Fizetési útmutató) | A számla fizetésének leírása a régió alapján. *A számla számát mindig adja meg a fizetéskor.* |
| Számla nem | A számla száma. |
| Számlázási időszak | A számlázási dátumig terjedő havi időszak. Ez az az időszak, amelynek során a rendszer felhasználja a használaton alapuló szolgáltatásokat, és a licenc-alapú szolgáltatások a kreditek változásaihoz vagy a licencek számának változásaihoz vannak egyeztetve. |
| Invoice Date (Számla dátuma) | Az a számlázási dátum vagy évfordulós dátum, amikor a számla generálása havonta történik. |
| Fizetési feltételek | A fizetési határidő. Egyszeri vásárlás esetén ez mindig 60 nap lesz. |
| Fizetési határidő | Az a dátum, ameddig a fizetést meg kell kapni. |
| Customer PO | A megrendelés megrendelése. |
| Ügyfélszolgálat | Annak a webhelynek a címe, amelyen keresztül elérheti az ügyfélszolgálatot. |
| Szolgáltatás címzettjének | Az a címe, ahol a szolgáltatást használják. (Ez a vállalat által bevett jogi cég címe.) |

## <a name="one-time-charges-fields"></a>Egyszeri felszámított díjak mezői

A következő mezők csak a partner Center **egyszeri díjaira** vonatkoznak:

| Mező | Meghatározás |
| ----- | ---------- |
| Dátum | A vásárlás dátuma. |
| Leírás | Termék neve. |
| Mennyiség | A megvásárolt termékek száma (például foglalások). |
| Egységár | Termék díja (például foglalás). |
| Discounts (Engedmények) | A vonatkozó kedvezmények. |
| Adózás előtti összeg | Az adók előtti beszerzések részösszege. |
| Forgalmi adó | Adó összege. |
| Összesen | A fizetendő teljes összeg. |
