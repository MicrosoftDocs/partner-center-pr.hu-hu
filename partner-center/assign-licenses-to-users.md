---
title: Ügyfélfiókok felhasználóinak kezelése
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Az ügyfelek felhasználóinak kezelése a Partnerközpont – felhasználói fiókokat hozhat létre, felhasználói licenceket adhat hozzá vagy távolíthat el, új jelszavakat állíthat vissza, valamint törölheti vagy visszaállíthatja a felhasználói fiókokat.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149893"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Az ügyfélfiókok felhasználói és felhasználói licenceinek kezelése 

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Rendszergazdai ügynök


Új felhasználókat hozhat létre és törölhet az ügyfél fiókjában. Egy vagy több olyan felhasználói fiókot is visszaállíthat, amelyet a törlést követő 30 napon belül törölt. A felhasználó korábbi előfizetés-hozzárendelései szintén visszaállnak (feltéve, hogy a korábbi foglalások elérhetők).

Amikor új előfizetéseket vásárol egy ügyfélnek, az ügyfélnek meg kell adni egy listát az összes felhasználóról, akiknek fiókra van szüksége, a felhasználói engedélyeiket, valamint az egyes felhasználóknak szükséges szolgáltatásokat.  

>[!NOTE]
>Az **Ügyfél lap** Felhasználók  és licencek szakasza az adott ügyfél bérlője által létrehozott összes felhasználót megjeleníti, beleértve azokat a felhasználókat is, akik más CSP-partnertől vagy más vásárlási csatornáról vásárolt licenccel rendelkezik.

Az [előfizetéseket egyszerre](bulk-license-provisioning-for-multiple-users.md) több felhasználóhoz is hozzárendelheti, ha a neveket [egy Excel-kompatibilis .csv-táblázatfájllal importálja.](adding-multiple-users-to-a-customer-account.md)

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Felhasználói fiókok létrehozása egy ügyfélnél

1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)

2. A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.

3. Az ügyfélmenüben válassza a **Felhasználók és licencek lehetőséget.**

4. Minden egyes felhasználónál válassza az **Előfizetés** hozzáadása lehetőséget, majd töltse ki az adatokat, beleértve az engedélyeket és a licenceket. **Mentse a** módosításokat.

5. Mindenképpen jegyezd fel a felhasználónak küldend el küldened a felhasználónevet és az ideiglenes jelszót.

6. Ha egyszerre több felhasználót ad hozzá, használja a **Másik felhasználó hozzáadása gombra.**

7. Egy Excel-kompatibilis .csv-számolótáblafájl importálása lehetővé teszi, hogy egyszerre több felhasználót [is hozzáadjon.](adding-multiple-users-to-a-customer-account.md) Megvárhatja, amíg a teljes készlettel végzett, mielőtt e-mailt küld, vagy kinyomtatja a neveket és jelszavakat a megerősítési képernyőn.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Felhasználói licenc hozzáadása vagy eltávolítása egy ügyfélnél

Az alábbi lépések a Microsoft-termékek felhasználói licenceinek hozzáadására vagy eltávolítására vonatkoznak. A licencalapú SaaS-előfizetések felhasználói licenceinek kereskedelmi piactéren való hozzáadásához vagy eltávolításához lásd: Licencek hozzáadása vagy [eltávolítása SaaS-előfizetéshez.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)

1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)

2. A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.

3. Az ügyfélmenüben válassza a **Felhasználók és licencek lehetőséget.**

4. Válasszon ki a listából egy vagy több felhasználót. Ha például az ügyfél most vásárolt új licenceket, és olyan személyekhez kívánt hozzárendelni őket, akik még nem rendelkezik velük, a Felhasználók **szűrése...** lehetőséggel megkeresheti a megfelelő csoportot.

5. Válassza ki a **Licencek kezelése** lehetőséget. Módosításokat kell tenni, majd a **Mentés gombra.**

> [!NOTE]
> A [Azure Marketplace termékek](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)esetében a licenc-hozzárendelést és az aktiválást a terméket közzétevő független szoftverszállító (ISV) kezeli.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Felhasználó jelszavának visszaállítása egy ügyfélhez

1. Jelentkezzen be a Partnerközpont [irányítópultjába](https://partner.microsoft.com/dashboard).

2. A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.

3. Az ügyfélmenüben válassza a **Felhasználók és licencek lehetőséget.** Válassza ki a felhasználót a listából.

4. A képernyő alján válassza a Jelszó **alaphelyzetbe állítása lehetőséget.** 

5. Küldje el az új ideiglenes jelszót a felhasználónak.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Ügyfél felhasználói fiókjainak törlése

1. A **Partnerközpont** válassza az Ügyfelek **lehetőséget.** Válassza ki az ügyfelet a listából.

2. Az ügyfélmenüben válassza a **Felhasználók és licencek lehetőséget.** Válassza ki a felhasználót a listából.

3. A képernyő alján válassza a **Felhasználói fiók törlése lehetőséget.**

Ha vissza kell állítania ezt a fiókot, az Ügyfél felhasználók és licencek listájának Törölt felhasználók lapján **találhatja** meg.  30 napja van a törölt felhasználók visszaállítására.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Törölt felhasználói fiókok visszaállítása

1. A **Partnerközpont** válassza az **Ügyfelek** lehetőséget, majd válassza ki az ügyfelet a listából.

2. Válassza **a Felhasználók és licencek lehetőséget.**

3. Válassza a **Törölt felhasználók ( )** lapot. Ha vannak visszaállítható törölt felhasználók, akkor a következőt kell olvasnia: **(1)** vagy nagyobb.

4. Jelölje be a törölt felhasználók egy vagy több jelölőnégyzetét, majd válassza a Visszaállítás **lehetőséget.**

    Az összes kiválasztott felhasználói fiók megjelenik a Felhasználók és **licencek lapon.**

## <a name="next-steps"></a>Következő lépések

- [Licencek hozzárendelése vagy visszavonása több felhasználó esetében](bulk-license-provisioning-for-multiple-users.md)

- [Több felhasználó létrehozása egy ügyfélfiókhoz](adding-multiple-users-to-a-customer-account.md)