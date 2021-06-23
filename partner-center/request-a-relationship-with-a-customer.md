---
title: Ügyféllel létesítendő viszonteladói kapcsolat kérelmezése
ms.topic: how-to
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Kapcsolat kérése egy ügyféllel többpartneres, többcsatornás forgatókönyvek esetén, vagy ha az ügyfél delegált rendszergazdai jogosultságait vissza kell állítani.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.openlocfilehash: 83f615e69a9285365e68305fa909104e0da52992
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551639"
---
# <a name="how-to-request-a-reseller-relationship-from-a-customer-in-partner-center"></a>Viszonteladói kapcsolat kérése egy ügyféltől a Partnerközpontban

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Globális rendszergazda

Ha egy ügyfél szolgáltatását vagy előfizetését szeretné kezelni a nevükben, az ügyfélnek rendszergazdai jogosultságokat kell önnek megszabadnie az adott szolgáltatáshoz vagy előfizetéshez, és alá kell írnia a Microsoft Ügyfélszerződés.

Ha viszonteladói kapcsolatot szeretne létesíteni egy ügyféllel, és csak az Ön által kiépíteni kívánt Azure-előfizetéseket szeretné kezelni, nem kell rendszergazdai engedélyeket beszereznie.

>[!NOTE] 
>Az engedélyek lekérésének mellőzését a microsoftos vagy a microsoftos felhőszolgáltatásban Microsoft Cloud for US Government partnerek nem kérhetik. További tudnivalókért lásd: [Ügyfelek delegálják a rendszergazdai jogosultságokat a partnereknek.](customers-revoke-admin-privileges.md)

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Ügyfél meghívása viszonteladói kapcsolat létesítésre

Viszonteladói kapcsolatot kérhet egy ügyféllel az országon vagy az Ön régióján belül.

1. Válassza **az Ügyfelek** lehetőséget **Partnerközpont** menüben, majd válassza **a Viszonteladói kapcsolat kérése lehetőséget.**

2. Ha rendszergazdai engedélyeket kell kérnie az ügyféltől, válassza a Delegált rendszergazdai jogosultságok is Azure Active Directory **Office 365-höz lehetőséget.** Ha rendszergazdai engedélyek kérése nélkül szeretné létrehozni a kapcsolatot, törölje ezt a beállítást.

3. A következő lapon tekintse át az e-mail-üzenet piszkozatát. Az üzenet piszkozatát az alapértelmezett e-mail-alkalmazásban nyithatja meg, vagy átmásolhatja az üzenetet a vágólapra, és beillesztheti egy e-mailbe.

   Az e-mailben szereplő szöveget szerkesztheti, de mindenképpen mellékelje a hivatkozást, mivel az személyre szabott, és közvetlenül a fiókjához kapcsolja az ügyfelet. Ha **végzett** ezzel a lépéssel, válassza a Kész lehetőséget.

4. Küldje el az e-mailt az ügyfélnek.

5. Miután az ügyfél elfogadta a meghívót,  megjelenik az Ügyfelek lapon, és onnan kiépítheti és kezelheti az ügyfél szolgáltatását.

   > [!NOTE]
   > Ha az ügyfél még nem fogadta el a Microsoft Ügyfélszerződés, akkor a meghívó elfogadásakor a rendszer felkéri erre. A meghívás elfogadásához az ügyfélnek globális rendszergazdának kell lennie.

6. Az ügyfél fiókjának, szolgáltatásainak, felhasználóinak és licencének kezeléséhez bontsa ki az ügyfél rekordját a név melletti lefelé mutató nyílra kattintva.

> [!IMPORTANT]  
> Az ügyfelek a szolgáltatás felügyeleti portálján újra hozzárendelheti vagy eltávolíthatja a rendszergazdai engedélyeket. Azonban, hacsak nem kötötte újra a szerződést az ügyféllel, továbbra is Az Ön felelőssége lesz az ügyféltámogatás biztosítása és a Microsoft Partnerszerződés használati útjára való betekintés, még akkor is, ha az ügyfél újra hozzárendeli vagy eltávolítja a rendszergazdai engedélyeket. Ebben az esetben, ha az ügyfélnek segítségre van szüksége, hívhatja a Microsoft ügyfélszolgálatát, hogy az ügyfél nevében nyisson meg egy szolgáltatáskérést.

## <a name="changes-to-the-customer-invitation-experience"></a>Az ügyfélmeghívási élmény változásai

A viszonteladói kapcsolatokra való meghívásnak egy Felhőszolgáltató (CSP) partnertől való elfogadásának felhasználói élményét különböző ügyfélkapcsolati portálok üzemeltetik. A portál helye attól függ, hogy az ügyfél a Microsoft nyilvános felhőben vagy az országos felhőben található:

|A felhőalapú ügyfelek típusai  | Hol fogadja el az ügyfél a viszonteladói kapcsolatokra való meghívást? |
|---------|---------
| Nyilvános felhőbeli ügyfelek | Microsoft 365 Felügyeleti központ |
| A Microsoft Cloud németországi Partnerközpont ügyfelei | Microsoft Office felügyeleti portál |
| A Partnerközpont ügyfelek Microsoft Cloud for US Government | Microsoft Office felügyeleti portál |
|

## <a name="next-steps"></a>Következő lépések

- [Támogatási kapcsolattartók hozzárendelése](assign-support-contacts.md)

- [Ügyféllel való kapcsolat eltávolítása](remove-a-relationship.md)
