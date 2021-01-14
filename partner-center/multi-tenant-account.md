---
title: További bérlők hozzáadása a partner Center-fiókhoz
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan adhat hozzá, összevonhat vagy kezelhet több Azure AD-bérlőt a partner Center-fiókban. Ismerje meg az egyes okokat is, amelyeket érdemes megtennie.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182433"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Több bérlő hozzáadása és kezelése a partner Center-fiókban


**Megfelelő szerepkörök**

- Globális rendszergazda
- Fiókadminisztrátor

Ez a funkció lehetővé teszi több, a vállalathoz tartozó bérlő kezelését és konszolidálását a Partnerközpont-fiókban. Számos oka lehet annak, hogy több Azure AD-bérlőt kell kezelnie a partner Center-fiókjában. Például:

- A vállalat megvásárolhat egy másik vállalatot, és azt szeretné, hogy az új vállalat alkalmazottai használni tudják a partner centert. Azonban azt szeretné, hogy a két vállalat külön maradjon. Ebben az esetben az új vállalati Azure AD-bérlőt a partner globális fiókjával (PGA) társíthatja. Ez a társítás azt teszi lehetővé, hogy mindkét vállalat felhasználói működjenek a partner Centerben.

- Ha több Bérlővel is futtatja vállalkozását (pl.: contoso.com, contoso.uk, contoso.in), a több-bérlős használatával összekapcsolhatja őket ugyanazzal a PC-fiókkal.

- Az egyesülések és a beszerzések esetében több bérlőt kell használni (például ha a contoso a Fabrikamt szerezte be, akkor mindkét Constoso.com és a Fabrikam.com megfelelő bérlőt kell használnia).

- A bérlők bármelyikének a következőket kell tudnia:
    1.  Partneri központ elérése képzéshez, digitális letöltésekhez, MCP-társításhoz
    2.  Hozzá kell rendelni a partner Center-szerepköröket, például az MPN-rendszergazdát, az ösztönzők rendszergazdáját stb.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Másik Azure AD-bérlő hozzáadása a fiókhoz

1. Globális rendszergazdaként jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).
1. A **Beállítások** ikonban válassza a **Fiókbeállítások** , majd a **bérlők** lehetőséget.
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="bérlők hozzárendelése"::: 

3. Válassza a **másik ad-bérlő hozzárendelése** lehetőséget, és jelölje ki a hozzárendelni kívánt bérlőt.

1. Globális rendszergazdaként jelentkezzen be a társítani kívánt bérlőbe, és erősítse meg a társítást. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="bérlők hozzárendelésének megerősítése"::: 

5. A megerősítést követően megjelenik az **összes beállított** értesítés.  Válassza a **Visszatérés a bérlői felügyelethez** lehetőséget, majd megjelenik az újonnan hozzáadott bérlő. 
 

>[!NOTE]
>Nem lehet bérlőt társítani egy fiókhoz, ha már társítva van egy másik partner Center-fiókhoz.


## <a name="remove-a-tenant-from-your-account"></a>Bérlő eltávolítása a fiókból
 
1. Globális rendszergazdaként jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).

1. A **Beállítások** ikonban válassza a **Fiókbeállítások** – > bérlők lehetőséget, és kattintson a **partner** fülre.
 
3. Kattintson az **Eltávolítás** gombra a leválasztani kívánt bérlőhöz.

4. A bérlők leválasztása azt jelenti, hogy a bérlő felhasználóinak többé nem lesz hozzáférésük a partner Center-fiókhoz, és ez hatással lehet a kompetenciára. 

Az **Eltávolítás** gomb minden társított bérlő esetében engedélyezve van, kivéve az elsődleges bérlőt és azt a bérlőt, amelyhez jelenleg be van jelentkezve.

:::image type="content" source="images/disassociate.png" alt-text="az Eltávolítás gombbal rendelkező bérlők":::
 

## <a name="next-steps"></a>Következő lépések

- [Felhasználók hozzáadása](create-user-accounts-and-set-permissions.md)






