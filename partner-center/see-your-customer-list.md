---
title: Ügyféllista kezelése
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Az ügyfélrekordok az egyik legfontosabb információs eszköz. Megtudhatja, hogyan lehet megtekinteni, keresni, frissíteni, & exportálni az adatokat a Partnerközpont ügyféllistán.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1791d415d0004520e8c7dc950decf540c91cf003
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002841"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Ügyféllista kezelése – ügyfelek keresése, frissítése vagy exportálása a Partnerközpont

**A következőre érvényes:**

- A Microsoft Cloud for US Government Partnerközpontja

**Megfelelő szerepkörök**

- Rendszergazdai ügynök
- Globális rendszergazda

Az ügyfélrekordok az egyik legfontosabb információs eszköz a Partnerközpont. Kereshet az ügyfélfiókok adatbázisában, exportálhatja a teljes ügyféladatbázist, vagy exportálhat egy részkészletet egy Excel-kompatibilis, vesszővel elválasztott értékfájlformátumba (.csv). Az ügyfelek előfizetési adatait .csv-fájlba is exportálhatja.

A tevékenységnaplók exportálható adatokat is biztosítanak az ügyfelek tranzakcióiról és felügyeleti műveleteiről. További információ: [Ügyféltevékenység-naplók megtekintése.](activity-logs.md)

## <a name="search-for-a-customer"></a>Ügyfél keresése

1. A **Partnerközpont** válassza az Ügyfelek **lehetőséget.**
2. Az ügyfél kereséséhez írja be az ügyfél nevét vagy tartománynevét a keresőmezőbe.
3. Az **ügyfélsor végén** található lefelé mutató nyílra kattintva láthatja a Microsoft-azonosítóját, valamint a társított előfizetések és szolgáltatások gyorshivatkozását.

## <a name="update-a-customers-company-name"></a>Ügyfél cégnevének frissítése

A **Partnerközpont** válassza az Ügyfelek **lehetőséget.**
2. Az ügyfél kereséséhez írja be az ügyfél nevét vagy tartománynevét a keresőmezőbe.
3. Az **ügyfélsor végén** található lefelé mutató nyílra kattintva láthatja a Microsoft-azonosítóját, valamint a kapcsolódó előfizetések és szolgáltatások gyorshivatkozását.
4. Az ügyfél számlázási **adatai** alatt frissítse a vállalat nevét. Az új érték mentésekor az megjelenik az ügyféllistában. Ez csak a számlázási vállalat nevét és az ügyféllista értékét módosítja. Máshol nem fog tükröződni.

## <a name="export-your-customer-list"></a>Ügyféllista exportálása

1. A **Partnerközpont** válassza az Ügyfelek **lehetőséget.**
2. Válassza az **Ügyfelek exportálása lehetőséget.**

   Partnerközpont a teljes ügyféllistát egy .csv-fájlba konvertálja, és feltölti azt a számítógép alapértelmezett letöltési mappájába. Az ügyféladatok rész részkészletét is exportálhatja. Az adatoszlopok a következők:

   - **Microsoft-azonosító;**
   - **Vállalat neve;**
   - **Elsődleges tartománynév;**
   - **Kapcsolat**– a partner és az egyes felsorolt ügyfelek közötti üzleti kapcsolat.

    Alapértelmezés szerint a Partnerközpont exportálja a teljes ügyféllistát, a hossztól függetlenül. Az ügyféllistában a vállalat neve vagy tartománya alapján is kereshet, és exportálhatja az adatok egy részkészletét.

3. Ha Ön közvetett szolgáltató, szűrheti az ügyféllistát közvetett viszonteladó szerint. Válassza **a Szűrés közvetett viszonteladó alapján lehetőséget** a listából, majd válasszon ki egy viszonteladót.


## <a name="export-customer-subscription-information"></a>Ügyfél-előfizetési adatok exportálása

1. A **Partnerközpont** válassza az Ügyfelek **lehetőséget.**

2. Válassza ki **bármelyik ügyfél** cégnevét. Megnyílik az ügyfél **Előfizetések oldala,** amely megjeleníti a termék-előfizetések teljes listáját.

3. Válassza **az Előfizetések exportálása lehetőséget.** Partnerközpont az ügyfél előfizetési adatait egy .csv-fájlba konvertálja, és feltölti őket a számítógép alapértelmezett letöltési mappájába. Az adatoszlopok a következőket tartalmazzák:
   - **Előfizetés azonosítója**;
   - **Előfizetés**– az előfizetés termékneve;
   - **Mennyiség**– a megvásárolt licencek száma;
   - **Állapot**;
   - **Reseller**– annak a viszonteladónak az azonosítója, aki az előfizetést tulajdonában van és kezeli.

> [!NOTE]  
> További információ az előfizetések kezelésével kapcsolatban: [Ügyfél-előfizetések.](customer-subscriptions.md)
