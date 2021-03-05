---
title: Bérlők hozzáadása a partner Center-fiókhoz
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan adhat hozzá, összevonhat vagy kezelhet több Azure AD-bérlőt a partner Center-fiókban, és megtudhatja, miért érdemes ezt megtenni.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124805"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Több bérlő hozzáadása és kezelése a partner Center-fiókban


**Megfelelő szerepkörök**

- Globális rendszergazda
- Fiókadminisztrátor

Ez a cikk azt ismerteti, hogyan lehet összevonni több Azure Active Directory (Azure AD) bérlőt a vállalat számára, majd a partner Center-fiókban felvenni és felügyelni azokat. Ennek számos oka van. Például:

- Tegyük fel, hogy vállalata, a contoso, megszerezte a fabrikam egy másik vállalatát. Azt szeretné, hogy a két vállalat külön maradjon, de azt szeretné, hogy az új alkalmazottak használni tudják a partner centert. Ebben az esetben az új vállalati Azure AD-bérlőt a partner globális fiókjával (PGA) társítja. Ez a társítás lehetővé teszi, hogy mindkét vállalat felhasználói működjenek a partner Centerben.

- Ha több Bérlővel is futtatja vállalkozását (például *contoso.com*, *contoso.uk* és *contoso.in*), a bérlős segítségével csoportosíthatja azokat ugyanazon a számítógép-fiókban.

- Ha az összeolvadások és a beszerzések irányelvei megkövetelik, hogy mindkét vállalat bérlői is működjenek, akkor a *constoso.com* és a *fabrikam.com* bérlőket is használni fogja.

- A bérlők felhasználói számára a következőket kell tudnia:
    * A Microsoft Certified Professional (MCP) társításának elérése a partner centerrel.
    * Társítsa a partner Center-szerepköröket, például a Microsoft Partner Network (MPN) rendszergazdai vagy ösztönző rendszergazdát.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Azure AD-bérlő hozzáadása a fiókjához

1. Jelentkezzen be globális rendszergazdaként a [Microsoft partner Centerbe](https://partner.microsoft.com/dashboard).

1. A jobb felső sarokban válassza a **Beállítások** lehetőséget, válassza a **Fiókbeállítások** lehetőséget, majd válassza a **bérlők** lehetőséget.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Képernyőkép az Azure AD-profil ablaktábla hozzárendelés gombjáról."::: 

1. Válassza a **hozzárendelés** lehetőséget, majd adja meg a hozzárendelni kívánt bérlőt.

1. A parancssorban jelentkezzen be globális rendszergazdaként a hozzárendelni kívánt bérlőre, majd válassza a **Confirm (megerősítés**) lehetőséget. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Képernyőkép az új Azure AD-társítás megerősítése panel megerősítés gombjáról."::: 

   Miután megerősítette a társítást, megjelenik az **összes beállított** üzenet. Az újonnan hozzáadott bérlő megtekintéséhez válassza a **Visszatérés a bérlői felügyeletbe** lehetőséget. 
 
>[!NOTE]
>Ha már társítva van egy másik partner Center-fiókkal, akkor nem lehet bérlőt társítani a fiókhoz.


## <a name="remove-a-tenant-from-your-account"></a>Bérlő eltávolítása a fiókból
 
1. Jelentkezzen be globális rendszergazdaként a [Microsoft partner Centerbe](https://partner.microsoft.com/dashboard).

1. A jobb felső sarokban válassza a **Beállítások** ikont, majd válassza a **Fiókbeállítások** lehetőséget.

1. A bal oldali ablaktáblán válassza a **bérlők** lehetőséget. Az **Azure ad-bérlők kezelése** területen válassza a **partner** lapot.
 
1. Válassza az **Eltávolítás** lehetőséget azon bérlő mellett, amelynek társítását el szeretné távolítani.

   :::image type="content" source="images/disassociate.png" alt-text="Képernyőkép az aktuális bérlői társításokról és azok eltávolítási kapcsolatairól.":::

   Ahogy az előző képernyőképen is látható, az **eltávolítási** hivatkozások minden társított bérlőhöz engedélyezve vannak, kivéve az elsődleges bérlőt és a bérlőt, amelyre jelenleg bejelentkezett. 

   > [!NOTE]   
   > Ha eltávolít egy bérlőt, az adott bérlő felhasználói már nem férnek hozzá a partner Center-fiókhoz, és az Eltávolítás hatással lehet a kompetenciára. 

## <a name="next-steps"></a>Következő lépések

- [Felhasználói fiókok létrehozása](create-user-accounts-and-set-permissions.md)






