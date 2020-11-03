---
title: Legyen a vállalat globális rendszergazdája
ms.topic: how-to
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A partner Centerben való működéshez először ellenőriznie kell a tartomány tulajdonjogát. Ebből a témakörből megtudhatja, hogyan teheti ezt meg, és hogyan válhat olyan globális rendszergazda, aki hozzáadhat felhasználókat.
author: vinayks
ms.author: vinayks
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: abec236f4856fdbfbcaa9654623c5f00b9a47584
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/02/2020
ms.locfileid: "92530192"
---
# <a name="verify-your-domain-ownership-to-become-global-admin"></a>A tartomány tulajdonjogának igazolása a globális rendszergazdává váláshoz 

**A következőkre vonatkozik:**

- Partnerközpont

**Megfelelő szerepkörök**

- Globális rendszergazda
- Fiókadminisztrátor

Ha a vállalat először hoz létre fiókot a partner Centerben, valószínűleg az alkalmazottak nem lesznek hozzárendelve a működés megkezdéséhez szükséges szerepkörökhöz.  Ahhoz, hogy működjön a partner Centerben, mindenkinek szüksége van egy szerepkörre, amely magában foglalja a hozzájuk rendelt engedélyeket.  

## <a name="find-the-companys-global-admin"></a>A vállalat globális rendszergazdájának megkeresése

1. A partner központ jobb felső sarkában található **Beállítások ikonra** kattintva válassza a **felhasználói kezelés** lehetőséget.

1. Szűrés a globális rendszergazda mezőben a keresőmezőbe. Ekkor megjelenik a vállalat globális rendszergazdáinak listája. Ha a vállalat még nem rendelkezik globális rendszergazdai jogosultsággal, kövesse az alábbi utasításokat.


## <a name="verify-your-domain-ownership-to-become-a-global-admin-in-partner-center"></a>Annak ellenőrzése, hogy a tartomány tulajdonjoga globális rendszergazda lesz-e a partner Centerben

Ahhoz, hogy globális rendszergazda legyen a vállalata számára, ellenőriznie kell a tartomány tulajdonjogát.

1. A partner központ irányítópultján, a **tagsági ajánlatok** lapon válassza a **globális rendszergazda lesz** lehetőséget. 

2. A **tartomány tulajdonjogának ellenőrzése** lapon másolja a txt-értékeket a táblából. Figyelje meg, hogy a tartomány már ki van választva.

3. Jelentkezzen be a tartományba. 

4. A tartomány által biztosított lépések végrehajtásával illessze be a TXT-értékeket a DNS-űrlapba.  Ez lehetővé teszi, hogy ellenőrizze, hogy a kívánt tartomány tulajdonosa-e.

5. Térjen vissza a partneri központba, és válassza **a rendben, Hozzáadtam a rekordot**

6. Az ellenőrzés befejezése után ki kell jelentkeznie. Az állapot frissítéséhez jelentkezzen be újra. 

A tartomány tulajdonjogának ellenőrzése globális rendszergazdai jogosultságokat is tesz lehetővé. A globális rendszergazdai szerepkörrel rendelkező egyes engedélyek a következők:

- Teljes körű jogosultságokkal fér hozzá minden Microsoft-fiók/szolgáltatáshoz 
- Támogatási jegyek létrehozása a partner központhoz
- Szerződések, árlisták és ajánlatok megtekintése
- Számlázás
- Partner-felhasználók megtekintése, létrehozása és kezelése
- Cloud Services vásárlása és kezelése

## <a name="next-steps"></a>Következő lépések

- A szerepkörökről és engedélyekről további információt a [felhasználói fiókok létrehozása](create-user-accounts-and-set-permissions.md)című témakörben talál. 