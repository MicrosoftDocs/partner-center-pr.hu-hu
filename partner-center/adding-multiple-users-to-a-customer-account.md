---
title: Több felhasználó hozzáadása egy ügyfélfiókhoz
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ha több felhasználót szeretne hozzáadni egy ügyfél fiókjához, töltsön fel egy adatfájlt a Partnerközpont vesszővel elválasztott (.csv) fájlformátumban.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150471"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Felhasználók .csv-fájl feltöltése egy ügyfél fiókjába


**Megfelelő szerepkörök:** Globális rendszergazda

Egyszerre több felhasználót is hozzáadhat egy ügyfél fiókjához, ha feltölt egy vesszővel elválasztott értékfájlformátumban (.csv) egy adatfájlt a Partnerközpont. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Hozza létre az ügyfélfelhasználók fájlját, és töltse fel az ügyfélfiókba

1. Hozzon létre egy vesszővel elválasztott adatfájlt (.csv) a fent leírt adatokkal. Mentse a fájlt, hogy egy későbbi lépésben tallózni tudja. A [.csv-fájl mezőiben több felhasználót importálhat egy ügyfélfiókhoz.](file-customer-users.md) 

2. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)

3. A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.

4. Válassza az ügyfél Felhasználók és licencek **lapját,** majd válassza a **Felhasználók feltöltése lehetőséget.**

5. A **Felhasználói adatok feltöltése alatt válassza** a Tallózás **lehetőséget.**

6. A fájlválasztóban válassza ki az adatfájlt, majd válassza a **Megnyitás lehetőséget.**

7. Válassza az **Érvényesítés** lehetőséget.

    **Megjegyzés**  A fiók létrehozásával kapcsolatos legtöbb hibát adatfájlhibák okják, beleértve a hiányzó információkat, a helytelenül formázott vagy duplikált e-mail-címeket, vagy a fájl túl sok rekordját.

8. Miután a Partnerközpont érvényesíti a fájlt, válassza ki az új felhasználók **földrajzi** helyét.
9. Kattintson a **Mentés** gombra.
10. Töltse le a felhasználók ideiglenes jelszóinformációját.

    >[!IMPORTANT]
    > Ne aggódjon, most töltse le az ideiglenes jelszavakkal együtt a fájlt, mert később ezt nem fogja tudni megtenni. Az új felhasználóknak az új fiókjuk ideiglenes jelszavával kell bejelentkezniük az új fiókjukba.

11. Az új felhasználókhoz automatikusan hozzárendelt engedélyek: **Használhat licenceket és szolgáltatásokat.** 

## <a name="next-steps"></a>Következő lépések

- [Engedélyt adhat az ügyfeleknek a Partnerközpont saját termékeik vagy szolgáltatásaik vásárlására](give-customers-permission.md)
