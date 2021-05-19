---
title: Felhasználói fiókok létrehozása és szerepkörök hozzárendelése
description: Minden alkalmazotthoz hozzá kell rendelni egy szerepkört, mielőtt hozzáférhet Partnerközpont. Megtudhatja, hogyan hozhat létre felhasználói fiókokat, hogyan rendelhet hozzá szerepköröket és állíthatja be az engedélyeket.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148142"
---
# <a name="create-user-accounts"></a>Felhasználói fiókok létrehozása  

**Megfelelő szerepkörök:** Fiók-rendszergazdai | Globális rendszergazdai | Felhasználókezelő rendszergazda

Hozzon létre felhasználói fiókokat az olyan alkalmazottak számára, akiknek hozzáférésre van szükségük a Partnerközpont. Ezeket a feladatokat a felhasználókezelő rendszergazdának, a fiók rendszergazdának vagy a globális rendszergazdának kell elvégeznie. A feladatokat végző felhasználóhoz hozzá kell rendelni a felhasználói rendszergazda Azure Active Directory (AAD) szerepköreit is, globális rendszergazda. További információ az AAD-szerepkörökről: Rendszergazdai szerepkör engedélyei a [Azure Active Directory.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)

## <a name="add-a-new-user"></a>Új felhasználó hozzáadása

1. A jobb **felső sarokban** található Beállítások Partnerközpont válassza a Fiókbeállítások,  majd a **Felhasználókezelés lehetőséget.**

2. Válassza a **Felhasználó hozzáadása** elemet.

3. Adja meg a felhasználó teljes nevét és egyedi e-mail-címét.

4. Válassza ki az ügynök és/vagy a felhasználóhoz hozzárendelni kívánt rendszergazda típusát. Partnerközpont hozzáférés szerepköralapú, így engedélyeket rendelhet a felhasználói nézet testreszabásához, hogy csak a felhasználó által meghatározott feladatok elvégzéséhez szükséges funkciókat mutassa.  Ha a felhasználók szerepkör-hozzárendelést keresnek, a Felhasználókezelés és szűrés a globális rendszergazda számára oldalon találhatják meg a kapcsolatot a globális rendszergazdákkal. 

5. Kattintson a **Hozzáadás** gombra a felhasználói fiók létrehozásához. A következő oldalon erősítse meg a felhasználó adatait.

> [!IMPORTANT]  
> Jegyezze fel az új felhasználó ezen az oldalon megjelenő bejelentkezési adatait. Másolja ki és küldje el ezt az információt az új felhasználónak, mert később nem fogja tudni ismét elérni. 

A felhasználónak be kell jelentkeznie a Partnerközpont a felhasználónevét és ideiglenes jelszavát. Amikor a felhasználó először jelentkezik be a Partnerközpont, a rendszer kérni fogja, hogy változtassa meg a jelszavát.

## <a name="assign-user-roles"></a>Felhasználói szerepkörök hozzárendelése

Ahhoz, hogy a Partnerközpont dolgoznia kell, egy hozzárendelt szerepkört kell hozzárendelnie.  A szerepkörök jelenleg Azure Active Directory bérlői, Felhőszolgáltató (CSP) és a nem AAD-hez használt vállalati szerepköröket foglalnak magukban. Egy adott vállalatnak szüksége lehet az összes szerepkörre.

>[!Important]
>Az egyéni felhasználók csak akkor férhetnek hozzá a bérlőhöz, ha Partnerközpont. A szerepkör-hozzárendelések további hozzáférést biztosítanak.

## <a name="next-steps"></a>Következő lépések

- [Felhasználói szerepkörök és engedélyek hozzárendelése olyan alkalmazottakhoz, akik a munkahelyi Partnerközpont](permissions-overview.md)
