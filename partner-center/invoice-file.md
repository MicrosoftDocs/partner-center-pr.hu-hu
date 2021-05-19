---
title: A Partnerközpont számlákkal kapcsolatos információk
ms.topic: article
ms.date: 05/18/2020
description: A számlázási fájl mezőinek megtekintése a Partnerközpont alapján. Ide tartoznak az összes számlamező és az egyszeres díjmezők mezői és definíciói.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5cb60c775bd8de38b8d7ca69c4dd97cf11b919fd
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146612"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>A Partnerközpont számlázási mezők

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Számlázási rendszergazdai | Helpdesk Agent

Az alábbi táblázatok segítségével megértheti a számlafájlokban Partnerközpont mezőket.

## <a name="invoice-file-fields"></a>Számlafájl mezői

A számlafájlokban a következő mezők jelennek meg.

| Mező | Meghatározás |
| ----- | ---------- |
| US FEIN | Az Ön szövetségi munkáltatói azonosító száma (FEIN). Ez az Ön Egyesült Államok adóazonosító száma. |
| Ügyfélszám | Az Ön ügyfélszáma. |
| Bill to (Számlázási cím) | Az a cím, ahová a számlát küldjük. A vállalat nevét és címét a számlázási profiljában Partnerközpont módosíthatja. |
| Licencalapú díjak | A megvásárolt használatalapú licencek havi vagy éves, a szolgáltatás előtt számlázható díjai. Ez a szám a licencalapú  egyeztetési fájl Részösszeg oszlopában **(T** oszlop) található díjak összege. |
| Használatalapú díjak | Az Ön Azure-használata. Ide tartoznak a számlázási időszakban engedélyezett és használt új szolgáltatások vagy alkalmazások. Ez a szám a használatalapú egyeztetési fájl **PretaxCharges** oszlopában **(Z** oszlop) található összes díj összege. |
| Discounts (Engedmények) | Az ügyfél által az előfizetés normál árára kapott kedvezmény. Ez a szám *egyösszegű összegként jelenik meg,* nem egységárként vagy licencenként. |
| Kreditek | Kreditek vagy helyesbítések az előfizetések módosításaihoz (például a licenc növelése vagy csökkenése). |
| Részösszeg | Az adók és az adómentes díjak és jóváírások teljes összege. |
| Adó | Az aktuális díjak teljes adója a  számla 2. oldalán kezdődő Részletek szakaszban összegzve. Ez a szám a használatalapú egyeztetési fájl **TaxAmount** oszlopában **(AA** oszlop)  és a licencalapú egyeztetési fájl Adózási oszlopában **(U** oszlop) lévő összes díj összege. |
| Egyéb kreditek | Adómentes jóváírások. |
| Összes aktuális díj | A számlázási időszak számlázási pénznemében esedékes összeg. Ezek a díjak a fizetési határidőig esedékesek. |
| Payment Instructions (Fizetési útmutató) | A számla kifizetésének leírása a régiója alapján. *A fizetéskor mindig foglalja bele a számlaszámot.* |
| Számlaszám | A számla száma. |
| Számlázási időszak | A számla dátumát elvezető havi időszak. Ez az az időszak, amely alatt a használatalapú szolgáltatásokat felhasználják, és a licencalapú szolgáltatásokat egyeztetik a kreditek módosításaival vagy a licencszám változásaival. |
| Invoice Date (Számla dátuma) | A számlázási dátum vagy évforduló dátuma, amelyen a számla minden hónapban létrejön. |
| Fizetési feltételek | A fizetési időszak. Az egyszer vásárolt vásárlások esetén ez mindig 60 nap. |
| Fizetési határidő | Az a dátum, amely szerint a kifizetést meg kell érkezik. |
| Ügyfél rendelése | A rendelésszáma. |
| Ügyfélszolgálat | A webhely címe, ahol elérheti az ügyfélszolgálatot. |
| Szolgáltatás címzettje | Az a cím, ahol a szolgáltatás használva van. (Ez a céges átvizsgáláshoz kapcsolódó jogi cég címe.) |

## <a name="one-time-charges-fields"></a>Az Egyszeres díjak mezői

A következő mezők  csak az adott időszakban érvényes Partnerközpont:

| Mező | Meghatározás |
| ----- | ---------- |
| Dátum | A vásárlás dátuma. |
| Description | Terméknév. |
| Mennyiség | A megvásárolt termékek (például foglalások) száma. |
| Egységár | Termékenkénti ár (például foglalás). |
| Discounts (Engedmények) | Minden alkalmazható kedvezmény. |
| Adóz előtti összeg | Az adók előtti vásárlások részösszege. |
| Értékesítési adó | Adó összege. |
| Összesen | Teljes fizetendő összeg. |
