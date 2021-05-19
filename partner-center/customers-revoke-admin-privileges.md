---
title: Ügyfél rendszergazdai jogosultságának beszerzése
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Szerezze be az ügyfél szolgáltatásának vagy előfizetésének a nevükben való kezeléséhez szükséges engedélyeket. Megtudhatja, hogyan adhatók meg, vonhatók vissza és kezelhetők az engedélyek.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: 779e76d6bb3e8df679a5ca6fa8ce441e42529161
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147292"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Engedélyek beszerzése egy ügyfél szolgáltatásának vagy előfizetésének kezeléséhez

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Értékesítési ügynök

Az ügyfél szolgáltatásának vagy előfizetésének a nevében történő kezeléséhez az ügyfélnek rendszergazdai engedélyeket kell ad önnek az adott szolgáltatáshoz. Ha rendszergazdai engedélyeket kér egy ügyféltől, küldjön neki egy viszonteladói kapcsolatkérést. Miután az ügyfél jóváhagyta a kérést, bejelentkezhet a szolgáltatás felügyeleti portálján, és kezelheti a szolgáltatást az ügyfél nevében. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Ügyfél meghívása viszonteladói kapcsolat létesítésre

1.  Válassza **az Ügyfelek,** majd **a Viszonteladói kapcsolat kérése lehetőséget.**

2.  A következő lapon tekintse át az e-mail-üzenet piszkozatát. Az üzenet piszkozatát az alapértelmezett e-mail-alkalmazásban nyithatja meg, vagy átmásolhatja az üzenetet a vágólapra, és beillesztheti egy e-mailbe. 

    >[!IMPORTANT]
    >Az e-mailben szereplő szöveget szerkesztheti, de mindenképpen mellékelje a hivatkozást, mivel az személyre szabott, és közvetlenül a fiókjához kapcsolja az ügyfelet. 
    
3.  Ha **végzett** ezzel a lépéssel, válassza a Kész lehetőséget.

4.  Küldje el az e-mailt az ügyfélnek.

5.  Miután az ügyfél elfogadta a meghívót,  megjelenik az Ügyfelek lapon, és onnan kiépíti és kezelheti a szolgáltatást.

6.  Az ügyfél fiókjának, szolgáltatásainak, felhasználóinak és licencének kezeléséhez bontsa ki az ügyfél rekordját a név melletti lefelé mutató nyílra kattintva, majd válassza ki a kezelni kívánt szolgáltatás felügyeleti portálját.

>[!IMPORTANT]  
>Az ügyfelek a szolgáltatás felügyeleti portálján újra hozzárendelheti vagy eltávolíthatja a rendszergazdai engedélyeket. Arról azonban tájékoztatnia kell az ügyfelet, hogy a rendszergazdai engedélyek eltávolítása azt jelenti, hogy a továbbiakban nem fog tudni szolgáltatási kérést nyitni a Microsoftnak a nevükben. Az ilyen típusú szolgáltatáskéréseket nem nyithatja meg az ügyfél nevében, amíg újra nem kötötte az ügyféllel kötött szerződést.

Az Ügyfelek az Office 365 felügyeleti portálon találhatják meg, hogy melyik partnerük rendelkezik rendszergazdai jogosultságokkal a bérlőjükhöz. Ehhez tegye a következőket:

1. Az ügyfélnek globális rendszergazdaként kell bejelentkeznie az Office 365 felügyeleti portálra.

2. Válassza **a Beállítások**  >  **Partnerkapcsolatok lehetőséget.**

3. A **Partnerkapcsolatok** lapon az ügyfél láthatja azon partnerek listáját, akikkel dolgozik, valamint azok, akik delegált rendszergazdai jogosultságot kaptak a bérlőjükhöz.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Az ügyfelek kezelhetik a partnerek delegált rendszergazdai jogosultságait 

Az ügyfél dönthet úgy, hogy eltávolítja a delegált rendszergazdai jogosultságokat a bérlőjéből, de az előfizetés és a licenc megújítása érdekében megtartja a kapcsolatot Önvel. Az ügyfelek az Office 365 Felügyeleti központ  Partnerkapcsolatok lapján kezelhetik office 365-fiókjaik jogosultságát és engedélyeiket. Ezen az oldalon az ügyfelek:

- Tekintse meg, hogy mely partnerekkel áll kapcsolatban, és mely partnerek delegált rendszergazdai jogosultságokkal

- Partner delegált rendszergazdai jogosultságának eltávolítása a bérlőből

Delegált rendszergazdai jogosultságok eltávolítása egy partnertől:

1. A **Partnerkapcsolatok lapon** válassza ki a kívánt partnert.
2. A részleteket tartalmazó panelen válassza a **Delegált rendszergazda eltávolítása lehetőséget.**
3. A megerősítési panelen válassza az Eltávolítás **lehetőséget.**

>[!IMPORTANT]  
>Az Azure AD-beli szerepkör-hozzárendelések implicitek a partnerhez. Ha megpróbálja listába sorolni az Azure AD-szerepkörök tagjait az Azure AD Portal/PowerShell/Graph használatával, a rendszer nem ad vissza partnert. Ha meg kell tudni, hogy a partnerek Azure AD-szerepkörökhöz vannak-e rendelve, az Office 365 felügyeleti portál Partnerkapcsolatok oldalán kell tájékozódni, hogy kapott-e delegált rendszergazdai jogosultságot a partnernek.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Delegált rendszergazdai jogosultságok az Azure AD-ban 

A partner Azure AD-bérlője két biztonsági csoportot (rendszergazdai ügynököket és támogatási ügynököket) használ a delegált felügyelethez. Ha egy ügyfél delegált felügyeleti jogosultságot biztosít egy partnernek:

- A rendszergazdai ügynök csoport az ügyfél Azure AD-bérlője globális rendszergazdai szerepköréhez van rendelve.

- A Támogatási ügynök csoport az ügyfélszolgálati rendszergazda szerepkörhöz van rendelve az ügyfél Azure AD-bérlője számára.

A hozzárendelt címtárbeli szerepkörök alapján mindkét csoport tagjai bejelentkeznek az ügyfél Azure AD-bérlőjébe és O365-szolgáltatásaiba a partneri hitelesítő adataik és a rendszergazda segítségével az ügyfél nevében.

Ha az ügyfél eltávolítja a delegált rendszergazdai jogosultságokat, az Azure AD szerepkör-hozzárendelései törlődnek, és Ön többé nem fogja tudni kezelni az ügyfél Azure AD-bérlőit.

### <a name="azure-subscriptions-and-resource-management"></a>Azure-előfizetések és erőforrás-kezelés

Minden Azure-előfizetés saját erőforrás-kezelési szerepkörökkel rendelkezik. Mielőtt egy CSP-partner kezelné egy ügyfél Azure-előfizetését, a partnert hozzá kell rendelni egy vagy több szerepkörhöz az Azure-előfizetésben. Ezek konkrétan a következők:

- Ha egy ügyfél elfogadja a viszonteladói meghívót, és delegált rendszergazdai jogosultságot biztosít egy partnernek, a partner nem kap automatikusan hozzáférést az ügyfélbérlőn belül meglévő Azure-előfizetéshez.

- Amikor a CSP-partner új Azure-előfizetést hoz létre az ügyfél számára, a CSP-partnerbérlőben a Rendszergazdai ügynökök csoport automatikusan tulajdonosi szerepkört kap az előfizetéshez. Ezen szerepkör-hozzárendelés alapján a csoport tagjai hozzáférhetnek az előfizetés erőforrásaihoz, és kezelhetik azt.

- Ha egy ügyfél az Office 365 portál használatával eltávolítja a delegált rendszergazdai jogosultságokat egy partnertől, a partner továbbra is kezelheti az ügyfél Azure-előfizetését, ha a partner továbbra is hozzá van rendelve az előfizetés egy vagy több szerepköréhez. Ha meg szeretné akadályozni, hogy a partner kezeli az Azure-előfizetést, az ügyfélnek el kell távolítania a szerepkör-hozzárendelést.

## <a name="windows-autopilot"></a>Windows Autopilot

A Partnerközpont csp-partnerek a következő esetekben kezelhetik az ügyfeleik AutoPilot-profiljait delegált rendszergazdai jogosultságok nélkül: 

- Ha egy ügyfél eltávolítja a delegált rendszergazdai jogosultságokat, de viszonteladói kapcsolatot tart meg Önvel, továbbra is kezelheti az Autopilot-profilokat.

- Kezelheti az Ön vagy egy másik partner által hozzáadott ügyféleszközöket. 

- Nem kezelheti az ügyfél által a portálon Microsoft Store Vállalatoknak, Microsoft Store Oktatási Intézményeknek vagy Microsoft Intune hozzáadott eszközöket.

További információ az Autopilotról: Az eszköz [beállításának egyszerűsítése a Windows Autopilot.](autopilot.md)

>[!IMPORTANT]  
>A jelenlegi Autopilot-Partnerközpont továbbra is változhatnak. A cikk közzétételekor a következő változásokat kell figyelembe venni:

- A partnernek delegált rendszergazdai jogosultságot kell adni az ügyfélnek, mielőtt a partner profilokat adhat hozzá, frissíthet/távolíthat el, illetve profilokat alkalmazhat/távolíthat el az ügyfélbérlőben elérhető összes eszközről.

- A partnernek delegált rendszergazdai jogosultságot kell adni az ügyfélnek, mielőtt a partner eltávolíthatja a más partnerek vagy az ügyfél bérlője által hozzáadott eszközöket. Ellenkező esetben a partner csak az ugyanazon partner által korábban hozzáadott eszközöket távolíthatja el.
