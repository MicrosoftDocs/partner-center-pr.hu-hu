---
title: Bérlők hozzáadása a Partnerközpont fiókjához
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan adhat hozzá, konszolidálhat vagy kezelhet több Azure AD-bérlőt Partnerközpont-fiókjában, és megtudhatja, miért érdemes ezt megtennie.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151202"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Több bérlő hozzáadása és kezelése a Partnerközpont fiókjában


**Megfelelő szerepkörök:** Globális rendszergazdai | Fiók adminisztrátora

Ez a cikk azt ismerteti, hogyan konszolidálhat több Azure Active Directory -bérlőt (Azure AD-bérlőt) a vállalat számára, majd hogyan adjuk hozzá és felügyelhetjük őket a Partnerközpont fiókjában. Ennek számos oka lehet. Például:

- Tegyük fel, hogy vállalata, a Contoso megvásárolt egy másik vállalatot, a Fabrikamot. Azt szeretné, hogy a két vállalat elkülönülő maradjon, de azt szeretné, hogy az új alkalmazottak használni tudják a Partnerközpont. Ebben az esetben az új vállalat Azure AD-bérlőjéhez társítja a globális partnerfiókját (PGA). Ez a társítás lehetővé teszi, hogy a felhasználók mindkét vállalatnál a Partnerközpont.

- Ha a vállalkozását több bérlővel (például *contoso.com,* *contoso.uk* és *contoso.in)* futtatja, több-bérlős rendszerekkel csoportosíthatja őket ugyanabban a számítógépfiókban.

- Ha az összeolvadással és felvásárlással kapcsolatos irányelvek megkövetelik, hogy  mindkét vállalat bérlőivel dolgozzon, akkor a constoso.com és fabrikam.com *bérlőket* is használnia kell.

- Bármely bérlő felhasználóinak képesnek kell lennie a következőre:
    * Hozzáférés Partnerközpont képzéshez, digitális letöltéshez vagy Microsoft Certified Professional (MCP) társításhoz.
    * Olyan szerepkörhöz Partnerközpont, mint Microsoft Partner Network (MPN) rendszergazda vagy ösztönzők rendszergazdája.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Azure AD-bérlő hozzáadása a fiókhoz

1. Jelentkezzen be globális rendszergazdaként a [Microsoft Partnerközpont.](https://partner.microsoft.com/dashboard)

1. A jobb felső sarokban válassza a **Beállítások,** a **Fiókbeállítások** lehetőséget, majd a **Bérlők lehetőséget.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Képernyőkép az Azure AD-profil panel Társítás gombjáról."::: 

1. Válassza **a Társítás** lehetőséget, majd jelölje ki a társítani kívánt bérlőt.

1. Amikor a rendszer kéri, jelentkezzen be globális rendszergazdaként a társítani kívánt bérlőbe, majd válassza a **Megerősítés lehetőséget.** 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Képernyőkép a Confirm (Megerősítés) gombról a Confirm new Azure AD association (Új Azure AD társítás megerősítése) panelen."::: 

   Miután megerősítette a társítást, megjelenik a **Minden beállítva** üzenet. Az újonnan hozzáadott bérlő megtekintéséhez válassza a Visszatérés a **bérlőkezeléshez lehetőséget.** 
 
>[!NOTE]
>Nem társíthat bérlőt egy fiókhoz, ha már társítva van egy másik Partnerközpont fiókkal.


## <a name="remove-a-tenant-from-your-account"></a>Bérlő eltávolítása a fiókból
 
1. Jelentkezzen be globális rendszergazdaként a [Microsoft Partnerközpont.](https://partner.microsoft.com/dashboard)

1. A jobb felső sarokban válassza a **Beállítások ikont,** majd a **Fiókbeállítások lehetőséget.**

1. A bal oldali panelen válassza a **Bérlők lehetőséget.** Az **Azure AD-bérlők kezelése alatt** válassza a **Partner** lapot.
 
1. Válassza **az Eltávolítás** lehetőséget azon bérlő mellett, amelynek társítását el szeretné távolítani.

   :::image type="content" source="images/disassociate.png" alt-text="Képernyőkép az aktuális bérlői társításról és azok Eltávolítás hivatkozásairól.":::

   Ahogy az előző képernyőképen  is látható, a Hivatkozások eltávolítása lehetőség engedélyezve van az összes társított bérlőn, kivéve az elsődleges bérlőt és azt a bérlőt, amelybe jelenleg be van jelentkezve. 

   > [!NOTE]   
   > Bérlő eltávolításakor a bérlő felhasználói már nem férhetnek hozzá a Partnerközpont-fiókhoz, és az eltávolítás hatással lehet a kompetenciákra. 

## <a name="next-steps"></a>Következő lépések

- [Felhasználói fiókok létrehozása](create-user-accounts-and-set-permissions.md)






