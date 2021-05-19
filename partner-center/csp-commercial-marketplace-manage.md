---
title: Marketplace-termékek kezelése & ajánlatokban
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A Partnerközpont megtudhatja, hogyan kezelhetik a felhőszolgáltatók a kereskedelmi piactérről az ügyfelek számára megvásárolt, külső isv-ajánlatokat.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e1bb2752dad5325478496c83fc368943780d8afb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147904"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Kereskedelmi piactéri termékek és ajánlatok kezelése az ügyfelek számára


**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök

A Felhőszolgáltató (CSP) program partnerei a Partnerközpont portal használatával számos ISV SaaS-ajánlatot vagy -előfizetést vásárolhatnak az ügyfeleik számára a kereskedelmi piactérről. Miután megvásárolt egy ajánlatot, többféleképpen is kezelheti azt.

## <a name="view-or-edit-a-subscription"></a>Előfizetés megtekintése vagy szerkesztése

Miután megvásárolt egy előfizetést egy külső ISV-közzétevőtől, a következőképpen áttekintheti vagy szerkesztheti azt:

1. Jelentkezzen be a Partnerközpont [irányítópultjára,](https://partner.microsoft.com/dashboard)majd válassza az **Ügyfelek lehetőséget** a bal oldali navigációs menüben.

2. Válasszon ki egy megfelelő ügyfelet, majd válassza az **Előfizetések lehetőséget.** Ez felsorolja az ügyfél számára megvásárolt licencalapú előfizetéseket.

3. Az Előfizetés **oszlopban** válassza ki a megtekinteni vagy szerkeszteni kívánt előfizetést. Ez további információt nyújt az ajánlat beállításról vagy építésről. (Ha további műveletre van szükség az ajánlaton, az Állapot oszlopban a "Beavatkozás szükséges" állapot is megjelenik. Ez az ISV-közzétevő webhelyére mutató hivatkozással is csatolható.)

4. Miután kiválasztotta a megtekinteni vagy szerkeszteni kívánt előfizetést, az előfizetés részletei oldalon szerkesztheti az előfizetést, és a következőt teszi lehetővé:

    - Az előfizetés becenevének módosítása

    - Licencek számának hozzáadása vagy csökkentése az előfizetésben

    - Az előfizetés lemondása

    - Az automatikus megújítás kikapcsolása

    - Közvetett viszonteladó MPN-azonosítójának hozzáadása, ha van

> [!NOTE]
> Előfordulhat, hogy el kell végeznie az ISV-közzétevő által meghatározott bizonyos lépéseket, mielőtt módosításokat végezhet egy előfizetésen, például megszakíthat egy előfizetést.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Licencek hozzárendelése és előfizetés aktiválása egy ügyfél nevében

Ha egy független szoftverszállító (ISV) kiadója által a kereskedelmi piactéren szolgáltatottszoftver-ajánlatot (SaaS) vásárol, a független szoftverszállító közzétevője segít kezelni a licencek hozzárendelésének és az előfizetés aktiválásának folyamatát az ügyfél nevében.

A közzétevőnek egy személyre szabott hivatkozást és egy engedélyezési kódot kell adnia, amely azonosítja az adott vásárlást.

1. Ezt a személyre szabott hivatkozást többféleképpen is megkeresheti az ISV-közzétevőtől:

   - A hivatkozást a megerősítő oldalon láthatja, amely az ISV SaaS-ajánlat megvásárlása után jelenik meg. A hivatkozásnak az oldalon való megkereshez keresse meg és válassza a **Go to publisher's site (Ugrás a közzétevő webhelyére) lehetőséget.**

   - A hivatkozást az adott ügyfél Előfizetések oldalán láthatja. Ez a közzétevői hivatkozás az ügyfél számára megvásárolt ISV-ajánlathoz vagy -előfizetéshez társított sorban jelenik meg.

   - A hivatkozást [a következő API Partnerközpont tudja lekérni.](/partner-center/develop/get-activation-link-by-order-line-item)

   > [!NOTE]
   > Ha ezt az ügyfél nevében szeretné megtenni, előfordulhat, hogy ki kell másolnia a személyre szabott hivatkozást, be kell illesztenie egy privát böngészőbe, és meg kell adnia az ügyfél hitelesítő adatait.

2. Miután az ISV-közzétevő webhelyén vagy rendszerében van, a közzétevő tudatja Az ügyfél beállítási folyamatának befejezéséhez, valamint a licencek kiosztásához vagy hozzárendeléséhez szükséges további lépésekről.

3. A CSP-program ügyfél nevében dolgozó partnerként Az Ön felelőssége a következő feladatok elvégzése:

    - Küldje el a szükséges információkat a közzétevőnek.

    - Küldje el a szükséges URL-címeket közvetlenül az ügyfélnek (vagy egyéb módon közvetlenül küldje el az előfizetés részleteit az ügyfélnek)

4. Miután a közzétevőnek megadhatja a szükséges információkat, a közzétevő kiépíti és hozzárendeli a megfelelő licenceket. Az előfizetés számlázása csak a következő események bekövetkezése után indul el:

    - Az ISV-közzétevő sikeresen hozzárendelte a megfelelő licenceket

    - Az ISV-közzétevő megerősítette a Microsoftnak (egy külön SaaS Fulfillment API-n keresztül), hogy a fiók beállítása sikeresen befejeződött

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Licencalapú SaaS-előfizetés lemondása ISV-közzétevőtől

Amikor a kereskedelmi piactéren egy ISV-közzétevő által kínált licencalapú SaaS-termékre iratk fel, lehetősége van megszüntetni az előfizetést a megadott lemondási időszakon belül. A lemondási időszak attól függően változik, hogy havi vagy éves előfizetéssel rendelkezik-e. Azt is eldöntheti, hogy automatikusan megújítja-e az előfizetést.

Az érvényes lemondási időtartamokkal, az előfizetések automatikus megújításának törlésével vagy megújításának mikéntével kapcsolatos további információkért lásd:

- [Előfizetés lemondása](create-a-new-subscription.md#cancel-a-subscription)

- [Kereskedelmi piactér-előfizetés automatikus megújítása](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>SaaS-előfizetés licencének hozzáadása vagy eltávolítása

SaaS kereskedelmi piactéri ajánlatok esetén felhasználói licenceket adhat hozzá vagy távolíthat el egy ügyfél-előfizetéshez.

1. Jelentkezzen be a Partnerközpont [irányítópultjára,](https://partner.microsoft.com/dashboard)majd válassza az **Ügyfelek lehetőséget** a bal oldali navigációs menüben.

2. Válasszon ki egy megfelelő ügyfelet, majd válassza az **Előfizetések lehetőséget.** Ez felsorolja az ügyfél számára megvásárolt licencalapú előfizetéseket.

3. Az Előfizetés **oszlopban** válassza ki a módosítani kívánt előfizetést.

4. Az előfizetés részletei oldalon keresse meg a **Mennyiség** mezőt. Itt növelheti vagy csökkentheti a licencek számát.

5. Módosítsa a mennyiséget, majd válassza a **Küldés lehetőséget.**

## <a name="manage-subscriptions-using-partner-center-apis"></a>Előfizetések kezelése Partnerközpont API-k használatával

Ezen kívül az Partnerközpont API-kat is használhatja az életciklus-felügyelethez és az előfizetések számláinak kezeléséhez. További információ: Előfizetés létrehozása [kereskedelmi piactéri termékekhez.](/partner-center/develop/create-subscription-azure-marketplace-products)

## <a name="next-steps"></a>Következő lépések

- [Kereskedelmi piactéri ajánlatok vásárlása](csp-commercial-marketplace-purchase.md)
- [Tudnivalók a számlázásról a kereskedelmi piactéren](csp-commercial-marketplace-billing.md)