---
title: Ügyfél rendszergazdai jogosultságának beszerzése
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Szerezze be az ügyfél szolgáltatásának vagy előfizetésének a nevében történő kezeléséhez szükséges engedélyeket. Ismerje meg, hogyan adhatók meg, vonhatók vissza és kezelhetők az engedélyek.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: 6f99c9ed9fb43136bccf0d3024377ba2208ed1a1
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534879"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Engedélyek beszerzése az ügyfél szolgáltatásának vagy előfizetésének kezeléséhez

**A következőre érvényes:**

- Partnerközpont

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Értékesítési ügynök

Ha az ügyfél szolgáltatását vagy előfizetését az Ön nevében szeretné kezelni, az ügyfélnek meg kell adnia a szolgáltatáshoz tartozó rendszergazdai engedélyeket. Ha rendszergazdai jogosultságokat szeretne kapni az ügyféltől, küldje el a viszonteladói kapcsolatra vonatkozó kérelmet. Miután az ügyfél jóváhagyta a kérelmét, bejelentkezhet a szolgáltatás felügyeleti portálján, és kezelheti a szolgáltatást az ügyfél nevében. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Ügyfél meghívása viszonteladói kapcsolat létesítéséhez

1.  Válassza az **ügyfelek** lehetőséget, majd válassza **a viszonteladói kapcsolat kérése** lehetőséget.

2.  A következő lapon tekintse át az e-mail-üzenet piszkozatát. Az üzenet piszkozatát az alapértelmezett e-mail-alkalmazásban nyithatja meg, vagy átmásolhatja az üzenetet a vágólapra, és beillesztheti egy e-mailbe. 

    >[!IMPORTANT]
    >Az e-mailben szereplő szöveget szerkesztheti, de mindenképpen mellékelje a hivatkozást, mivel az személyre szabott, és közvetlenül a fiókjához kapcsolja az ügyfelet. 
    
3.  Ha befejezte ezt a lépést, válassza a **kész** lehetőséget.

4.  Küldje el az e-mailt az ügyfélnek.

5.  Miután az ügyfél elfogadta a meghívót, megjelennek az **ügyfelek** oldalán, és az ügyfél számára is kiépítheti és kezelheti a szolgáltatást.

6.  Az ügyfél fiókjának, szolgáltatásainak, felhasználóinak és licencének kezeléséhez bontsa ki az ügyfél rekordját a neve melletti lefelé mutató nyílra kattintva, majd válassza ki a felügyelni kívánt szolgáltatás felügyeleti portálját.

>[!IMPORTANT]  
>Az ügyfelek a szolgáltatás felügyeleti portálján módosíthatják vagy eltávolíthatják a rendszergazdai engedélyeket. Azonban tájékoztatnia kell az ügyfelet, hogy távolítsa el a rendszergazdai engedélyeket, így többé nem fog tudni megnyitni egy szolgáltatási kérelmet a Microsoftnak a nevében. Az ügyfél nevében nem nyithatja meg az ilyen típusú szolgáltatási kérelmeket, amíg újra nem egyezteti a szerződést az ügyféllel.

Ügyfeleinek megtudhatják, hogy a partnerek közül melyiknek van rendszergazdai jogosultsága a bérlőnek az Office 365 felügyeleti portálján. Ehhez tegye a következőket:

1. Az ügyfélnek globális rendszergazdaként kell bejelentkeznie az Office 365 felügyeleti portálra.

2. Válassza a **Beállítások**  >  **partneri kapcsolatok** lehetőséget.

3. A **partneri kapcsolatok** lapon megjelenik az ügyfél azon partnereinek listája, akikkel működnek, és amelyek delegált rendszergazdai jogosultságot kaptak a bérlőik számára.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Az ügyfelek felügyelhetik a partner meghatalmazott rendszergazdai jogosultságait 

Az ügyfél dönthet úgy is, hogy eltávolítja a meghatalmazott rendszergazdai jogosultságokat a bérlőtől, de megtartja Önnel a kapcsolatot az előfizetés és a licenc megújítása céljából. A felhasználók az Office 365-fiókokhoz tartozó jogosultságokat és engedélyeket az Office 365 felügyeleti központ **partner kapcsolatok** lapján kezelhetik. Ezen az oldalon az ügyfelek a következőket tehetik:

- Megtudhatja, hogy mely partnerek rendelkeznek a kapcsolattal, és hogy mely partnerek delegált rendszergazdai jogosultságokkal rendelkeznek

- Partner delegált rendszergazdai jogosultságának eltávolítása a bérlőtől

Delegált rendszergazdai jogosultságok eltávolítása a partnertől:

1. A **partneri kapcsolatok** lapon válassza ki a partnert, aki érdeklődik.
2. A részleteket tartalmazó ablaktáblán válassza a **meghatalmazott rendszergazda eltávolítása** lehetőséget.
3. A megerősítő ablaktáblán válassza az **Eltávolítás** lehetőséget.

>[!IMPORTANT]  
>A partnerhez tartozó Azure AD-szerepkör-hozzárendelések implicitek. Ha az Azure ad Portal/PowerShell/Graph használatával próbálja meg kilistázni az Azure AD-szerepkörök tagjait, a rendszer nem adja vissza a partnert. Annak megállapításához, hogy a partnerek Azure AD-szerepkörökhöz vannak-e rendelve, az Office 365 felügyeleti portálján partneri kapcsolatok lapjára kell hivatkoznia, ha meg szeretné tudni, hogy a partnernek van-e delegált rendszergazdai jogosultsága, vagy sem.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Delegált rendszergazdai jogosultságok az Azure AD-ben 

A partner Azure AD-bérlője két biztonsági csoportot, rendszergazdai ügynököt és segélyszolgálat-ügynököt használ a delegált felügyelethez. Ha egy ügyfél delegált rendszergazdai jogosultságot ad a partnernek:

- A rendszergazdai ügynök csoport a globális rendszergazdai szerepkörhöz van rendelve az ügyfél Azure AD-bérlőben.

- Az ügyfélszolgálati ügynök csoportot az ügyfél Azure AD-bérlője az ügyfélszolgálati rendszergazda szerepkörhöz rendeli.

A hozzárendelt címtárbeli szerepkörök alapján mindkét csoport tagjai bejelentkezhetnek az ügyfél Azure AD-bérlői és O365 szolgáltatásaiba a partneri hitelesítő adataik és a rendszergazda által az ügyfél nevében.

Ha az ügyfél eltávolítja a delegált rendszergazdai jogosultságokat, a rendszer eltávolítja az Azure AD szerepkör-hozzárendeléseket, és többé nem fogja tudni kezelni az ügyfél Azure AD-bérlőjét.

### <a name="azure-subscriptions-and-resource-management"></a>Azure-előfizetések és erőforrás-kezelés

Minden Azure-előfizetés saját erőforrás-kezelési szerepkörökkel rendelkezik. Mielőtt egy CSP-partner felügyelheti az ügyfél Azure-előfizetését, a partnert hozzá kell rendelni egy vagy több szerepkörhöz az Azure-előfizetésben. Ezek konkrétan a következők:

- Ha az ügyfél elfogad egy viszonteladói meghívást, és delegált rendszergazdai jogosultságot ad a partnernek, a partner nem kap automatikusan hozzáférést az ügyfél bérlője által biztosított meglévő Azure-előfizetésekhez.

- Ha a CSP-partner új Azure-előfizetést épít ki az ügyfél számára, akkor a CSP-partner bérlője alá tartozó rendszergazdai ügynökök csoport automatikusan hozzárendeli a tulajdonosi szerepkört az előfizetéshez. A szerepkör-hozzárendelés alapján a csoport tagjai hozzáférhetnek és kezelhetik az előfizetésben található erőforrásokat.

- Ha egy ügyfél az Office 365 portál használatával eltávolítja a delegált felügyeleti jogosultságokat egy partnertől, akkor a partner továbbra is kezelheti az ügyfél Azure-előfizetését, feltéve, hogy a partner még hozzá van rendelve egy vagy több szerepkörhöz az előfizetés alatt. Ha le szeretné állítani a partnert az Azure-előfizetés kezelésében, az ügyfélnek el kell távolítania a szerepkör-hozzárendelést.

## <a name="windows-autopilot"></a>Windows Autopilot

A partneri központból a CSP-partnerek a jelen körülmények között a delegált rendszergazdai jogosultságok nélkül kezelhetik ügyfeleik számára az Autopilot-profilokat: 

- Ha egy ügyfél eltávolítja a delegált felügyeleti jogosultságokat, de megtartja Önnel a viszonteladói kapcsolatot, továbbra is kezelheti az Autopilot-profilokat.

- Kezelheti az Ön vagy egy másik partner által hozzáadott ügyfeleket. 

- Nem kezelhet olyan eszközöket, amelyeket az ügyfél a Microsoft Store for Business, az Microsoft Store for Education vagy a Microsoft Intune Portal használatával hozzáadott.

Az Autopilot szolgáltatással kapcsolatos további információkért lásd: [az eszközök beállításának leegyszerűsítése a Windows Autopilot](autopilot.md)szolgáltatással.

>[!IMPORTANT]  
>Előfordulhat, hogy a partnervállalat jelenlegi robotpilóta-kezelési felülete továbbra is változhat. A cikk közzétételének időpontjában a következő változások tekintendők:

- A partnernek delegált rendszergazdai jogosultságot kell biztosítania az ügyfél számára, mielőtt a partner hozzáadhat/frissíthet/eltávolíthat profilokat, és a profil alkalmazásával vagy eltávolításával az ügyfél bérlője bármely eszközéről.

- A partnernek delegált rendszergazdai jogosultságot kell biztosítania ahhoz, hogy az ügyfél el tudja távolítani a többi partner vagy az ügyfél bérlője által felvett eszközöket. Ellenkező esetben a partner csak a korábban ugyanahhoz a partnerhez hozzáadott eszközöket távolíthatja el.
