---
title: Felhasználói fiókok és felhasználói licencek kezelése az ügyfelek fiókjaihoz
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan kezelheti az ügyfelek felhasználói számára a partner Centerben, például felhasználói fiókok létrehozását, felhasználói licencek hozzáadását vagy eltávolítását, felhasználói jelszavak visszaállítását, valamint felhasználói fiókok törlését vagy visszaállítását.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fb7906b006540ef939e443a21855488e9d2c36f9
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474070"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Felhasználói fiókok és felhasználói licencek kezelése az ügyfelek fiókjaihoz

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói felügyeleti rendszergazda
- Felügyeleti ügynök


Az ügyfél fiókjában új felhasználókat hozhat létre és törölhet. A törléstől számított 30 napon belül egy vagy több olyan felhasználói fiókot is visszaállíthat, amelyet korábban törölt. A felhasználó korábbi előfizetési hozzárendelései is vissza lesznek állítva (feltéve, hogy az előző foglalások elérhetők).

Amikor új előfizetést vásárol az ügyfél számára, az ügyfélnek meg kell adnia az összes olyan felhasználó listáját, akiknek szükségük van a fiókra, a felhasználói engedélyeire és az egyes felhasználók által igényelt szolgáltatásokra.  

Egyszerre [több felhasználóhoz is hozzárendelhet előfizetéseket](bulk-license-provisioning-for-multiple-users.md) úgy, hogy a neveket egy [Excel-kompatibilis. csv számolótábla-fájllal](adding-multiple-users-to-a-customer-account.md)importálja.

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Felhasználói fiókok létrehozása az ügyfelek számára

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).

2. A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.

3. Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget.

4. Minden hozzáadott felhasználónál Válassza az **előfizetés hozzáadása** lehetőséget, majd adja meg az adatokat, beleértve az engedélyeket és a licenceket is. **Mentse** a módosításokat.

5. Ügyeljen arra, hogy a felhasználó számára küldendő felhasználónevet és ideiglenes jelszót jegyezze fel.

6. Ha egyszerre több felhasználót ad hozzá, akkor használjon **másik felhasználót**.

7. Egyszerre több felhasználót is hozzáadhat [egy Excel-kompatibilis. CSV formátumú számolótábla-fájl importálásával](adding-multiple-users-to-a-customer-account.md). Megvárhatja, amíg elkészült a teljes készlettel, mielőtt e-mailben vagy kinyomtatja a neveket és a jelszavakat a megerősítő képernyőn.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Felhasználói licencek hozzáadása vagy eltávolítása az ügyfélhez

A következő lépések a Microsoft-termékekhez tartozó felhasználói licencek hozzáadására vagy eltávolítására vonatkoznak. A licenc alapú SaaS-előfizetésekhez tartozó felhasználói licencek hozzáadásához vagy eltávolításához a kereskedelmi piactéren tekintse meg a [SaaS-előfizetés licencek hozzáadása vagy eltávolítása](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)című témakört.

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).

2. A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.

3. Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget.

4. Válasszon ki egy vagy több felhasználót a listából. Ha például az ügyfél csak új licenceket vásárolt, és azokat a felhasználók számára szeretné hozzárendelni, akik még nem rendelkeznek velük, akkor a megfelelő csoport megkereséséhez használhatja a **felhasználók szűrése...** lehetőséget.

5. Válassza a **licencek kezelése** lehetőséget. Végezze el a módosításokat, majd **mentse**.

> [!NOTE]
> Az [Azure Marketplace-termékek](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)esetében a licenc-hozzárendelést és az aktiválást a terméket közzétevő független SZOFTVERGYÁRTÓ (ISV) kezeli.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Felhasználó jelszavának alaphelyzetbe állítása az ügyfél számára

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).

2. A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.

3.  Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget. Válassza ki a felhasználót a listából.

4.  A képernyő alján válassza a **jelszó alaphelyzetbe állítása** lehetőséget. 

5.  Küldje el az új ideiglenes jelszót a felhasználónak.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Ügyfelek felhasználói fiókjainak törlése

1.  A **partner Center** menüben válassza az **ügyfelek** lehetőséget. Válassza ki az ügyfelet a listából.

2.  Az ügyfél menüben válassza a **felhasználók és licencek** lehetőséget. Válassza ki a felhasználót a listából.

3.  A képernyő alján válassza a **felhasználói fiók törlése** lehetőséget.

Ha vissza kell állítania ezt a fiókot, az ügyfél **felhasználói és licencek** listája **törölt felhasználók** lapján található. A törölt felhasználó visszaállításának 30 napja van.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Törölt felhasználói fiókok visszaállítása

1.  A **partner Center** menüben válassza az **ügyfelek** lehetőséget, majd válassza ki az ügyfelet a listából.

2.  Válassza **a felhasználók és licencek** lehetőséget.

3.  Válassza a **törölt felhasználók ()** lapot. Ha törölt felhasználók is visszaállíthatók, olvassa el **(1)** vagy annál nagyobb.

4.  Válasszon ki egy vagy több törölt felhasználó jelölőnégyzetet, majd válassza a **visszaállítás** lehetőséget.

    Az összes kiválasztott felhasználói fiók újra megjelenik a **felhasználók és licencek** lapon.

## <a name="related-topics"></a>Kapcsolódó témakörök


[Licencek hozzárendelése vagy visszavonása több felhasználó esetében](bulk-license-provisioning-for-multiple-users.md)

[Több felhasználó létrehozása egy ügyfél-fiókhoz](adding-multiple-users-to-a-customer-account.md)