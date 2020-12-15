---
title: Felhasználói fiókok létrehozása és szerepkörök társítása
description: Minden alkalmazottnak hozzá kell rendelnie egy szerepkört, mielőtt hozzá tudnak férni a partner központhoz. Megtudhatja, hogyan hozhat létre felhasználói fiókokat, rendelhet hozzá szerepköröket és állíthat be engedélyeket.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: c8fad4432f9aabba69877d80038ec9e2665c639d
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492534"
---
# <a name="create-user-accounts"></a>Felhasználói fiókok létrehozása  

**Megfelelő szerepkörök**

- Fiókadminisztrátor
- Globális rendszergazda
- Felhasználói felügyeleti rendszergazda

Hozzon létre felhasználói fiókokat azon alkalmazottak számára, akiknek hozzáférésre van szükségük a partner központhoz. Ezeket a feladatokat a felhasználói felügyeleti rendszergazdának, a fiókok rendszergazdájának vagy a globális rendszergazdának kell elvégeznie. A feladatokat végrehajtó felhasználónak hozzá kell rendelnie a felhasználói rendszergazda vagy a globális rendszergazda Azure Active Directory (HRE) szerepkörét is. További információ a HRE szerepköreiről: [rendszergazdai szerepkör engedélyei Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="add-a-new-user"></a>Új felhasználó hozzáadása

1. A partner központ jobb felső részén található **Beállítások** ikonban válassza a **Fiókbeállítások** , majd a **felhasználói kezelés** lehetőséget.

2. Válassza a **Felhasználó hozzáadása** elemet.

3. Adja meg a felhasználó teljes nevét és egyedi e-mail-címét.

4. Válassza ki az ügynök típusát és/vagy a felhasználóhoz hozzárendelni kívánt rendszergazda típusát. A fiókpartner-hozzáférés szerepköralapú, így engedélyeket rendelhet a felhasználó nézetének testreszabásához, hogy csak azok a funkciók jelenjenek meg, amelyekre a felhasználónak szüksége van az adott feladatok elvégzéséhez.  Ha a felhasználók szerepkör-hozzárendelést kívánnak, a globális adminisztrátorok **és a** globális rendszergazda szűrése lehetőségre kattintva megtalálhatják a kapcsolattartáshoz szükséges globális rendszergazdákat.

5. Kattintson a **Hozzáadás** gombra a felhasználói fiók létrehozásához. Erősítse meg a felhasználó adatait a következő oldalon.

> [!IMPORTANT]  
> Jegyezze fel az új felhasználó bejelentkezési információit ezen az oldalon. Ügyeljen arra, hogy ezeket az adatokat az új felhasználónak másolja és küldje el, mivel később nem fogja tudni elérni. 

A felhasználónak felhasználónevével és ideiglenes jelszavával be kell jelentkeznie a partner központba. Amikor a felhasználó első alkalommal jelentkezik be a partner központba, a rendszer felszólítja a jelszó módosítására.

## <a name="assign-user-roles"></a>Felhasználói szerepkörök kiosztása

A partner Centerben való működéshez hozzárendelt szerepkörrel kell rendelkeznie.  A szerepkörök jelenleg Azure Active Directory bérlői szerepköröket, a Cloud Solution Provider (CSP) szerepköröket, valamint a nem HRE vállalati szerepköröket tartalmazzák. Az egyes vállalatok igénybe vehetik az összes ilyen szerepkört.

>[!Important]
>A partneri központ eléréséhez a bérlőnek szerepelnie kell az egyéni felhasználók listáján. A szerepkör-hozzárendelések további hozzáférést biztosítanak.

## <a name="next-steps"></a>Következő lépések

- [Felhasználói szerepkörök és engedélyek kiosztása a partner Centerben való működéshez szükséges alkalmazottak számára](permissions-overview.md)
