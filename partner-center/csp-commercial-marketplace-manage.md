---
title: Marketplace-termékek & ajánlatok kezelése
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A partner Center használatával megtudhatja, hogyan kezelhetik a felhőalapú megoldások szolgáltatói a kereskedelmi piactéren vásárolt, harmadik féltől származó ISV-ajánlatokat.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5e6ca188aeb50cec6f847afb08be4a9d62b36984
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979676"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Kereskedelmi Piactéri termékek és ajánlatok kezelése az ügyfelek számára


**Megfelelő szerepkörök**

- Globális rendszergazda
- Felügyeleti ügynök

A Cloud Solution Provider (CSP) program partnerei a partner Center portál segítségével számos ISV SaaS-ajánlatot vagy-előfizetést vásárolhatnak a kereskedelmi piactéren. Az ajánlat megvásárlása után többféleképpen is kezelheti azt.

## <a name="view-or-edit-a-subscription"></a>Előfizetés megtekintése és szerkesztése

Miután megvásárolt egy előfizetést egy külső gyártótól származó ISV-közzétevőtől, a következőképpen tekintheti át vagy szerkesztheti:

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard), majd válassza a bal oldali navigációs menü **ügyfelek** elemét.

2. Válasszon ki egy megfelelő ügyfelet, majd válassza az **előfizetések** lehetőséget. Ez felsorolja az ügyfél számára megvásárolt licenc-alapú előfizetéseket.

3. Az **előfizetés** oszlopban válassza ki a megtekinteni vagy szerkeszteni kívánt előfizetést. Ez további információkat nyújt az ajánlat beállításához vagy kiépítéséhez. (Ha további műveletre van szükség az ajánlaton, akkor az Állapot oszlopban megjelenik egy "beavatkozás szükséges" állapot. Ezt az ISV-közzétevő webhelyére mutató hivatkozás is kísérheti.)

4. Miután kiválasztotta a megtekinteni vagy szerkeszteni kívánt előfizetést, az előfizetés részletei lapon szerkesztheti az előfizetést, és a következőkhöz hasonló műveleteket végezhet:

    - Előfizetés módosítása Felhasználónév

    - Az előfizetéshez tartozó licencek számának hozzáadása/csökkentése

    - Előfizetés megszakítása

    - Automatikus megújítás kikapcsolása

    - Közvetett viszonteladói MPN-azonosító hozzáadása, ha van ilyen

> [!NOTE]
> Előfordulhat, hogy végre kell hajtania bizonyos, az ISV-közzétevő által meghatározott lépéseket, mielőtt módosításokat hajt végre az előfizetésben, például egy előfizetés megszakításával.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Licencek kiosztása és előfizetés aktiválása az ügyfél nevében

Ha a kereskedelmi piactéren egy független szoftvergyártó (ISV) által biztosított szolgáltatott szoftver (SaaS) ajánlatot vásárol, az ISV-közzétevő segít a licencek hozzárendelésének és az előfizetés az ügyfél nevében történő aktiválásának kezelésében.

A közzétevőnek egy személyre szabott hivatkozást és egy engedélyezési kódot kell megadnia, amely azonosítja az adott vásárlást.

1. Ezt a személyre szabott hivatkozást az ISV-közzétevőből is megtalálhatja néhány módon:

   - Az ISV SaaS-ajánlat megvásárlása után megjelenő hivatkozást a megerősítő lapon tekintheti meg. Ha meg szeretné keresni ezt a hivatkozást az oldalon, keresse meg, majd válassza a **Ugrás a közzétevő webhelyére** lehetőséget.

   - A hivatkozást az adott ügyfél előfizetések oldalán tekintheti meg. Ez a közzétevő hivatkozás az ügyfélhez megvásárolt ISV-ajánlathoz vagy-előfizetéshez társított sorban jelenik meg.

   - [A hivatkozást a partner Center API](/partner-center/develop/get-activation-link-by-order-line-item)-k használatával kérheti le.

   > [!NOTE]
   > Ha ezt az ügyfél nevében szeretné elvégezni, előfordulhat, hogy át kell másolnia a személyre szabott hivatkozást, be kell illesztenie egy privát böngészőbe, és meg kell adnia az ügyfél hitelesítő adatait.

2. Ha az ISV-közzétevő webhelyét vagy rendszerét használja, a közzétevő megtudhatja, milyen további lépéseket kell végrehajtania az ügyfél-telepítési folyamat befejezéséhez, illetve a licencek kiosztásához és hozzárendeléséhez.

3. Ha az ügyfél nevében működő CSP-programban partnerként dolgozik, a következő feladatokat kell elvégeznie:

    - Küldje el a szükséges információkat a közzétevőnek.

    - Küldje el a szükséges URL-címet közvetlenül az ügyfelének (vagy más módon közvetlenül az előfizetésre vonatkozó adatokat az ügyfélnek)

4. Miután megadta a szükséges információkat a közzétevőnek, a közzétevő kiépíti és hozzárendeli a megfelelő licenceket. Az előfizetés számlázása csak a következő események bekövetkezése után indul el:

    - Az ISV-közzétevő sikeresen hozzárendelte a megfelelő licenceket

    - Az ISV-közzétevő megerősítette a Microsoft számára (egy különálló, SaaS-betöltési API-n keresztül), hogy a fiók telepítése sikeresen befejeződött.

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Licenc alapú SaaS-előfizetés megszakítása ISV-közzétevőből

Ha a kereskedelmi piactéren egy ISV-közzétevő által kínált licenccel rendelkező SaaS-termékre fizet elő, lehetősége van megszakítani az előfizetést a megadott megszakítási időszakon belül. Ez a lemondási időszak attól függően változik, hogy van-e havi vagy éves előfizetése. Azt is megadhatja, hogy automatikusan megújítsa-e az előfizetést.

További információ az előfizetéssel kapcsolatos lemondási időszakokról, a lemondás vagy az előfizetés automatikus megújításáról:

- [Előfizetés megszakítása](create-a-new-subscription.md#cancel-a-subscription)

- [Kereskedelmi piactér-előfizetés automatikus megújítása](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>SaaS-előfizetéshez tartozó licencek hozzáadása vagy eltávolítása

A SaaS kereskedelmi Piactéri ajánlatokhoz felhasználói licenceket adhat hozzá vagy távolíthat el az ügyfél-előfizetésekhez.

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard), majd válassza a bal oldali navigációs menü **ügyfelek** elemét.

2. Válasszon ki egy megfelelő ügyfelet, majd válassza az **előfizetések** lehetőséget. Ez felsorolja az ügyfél számára megvásárolt licenc-alapú előfizetéseket.

3. Az **előfizetés** oszlopban válassza ki a módosítani kívánt előfizetést.

4. Az előfizetés részletei lapon keresse meg a **mennyiség** mezőt. Itt növelheti vagy csökkentheti a licencek számát.

5. Módosítsa a mennyiséget, majd válassza a **Küldés** lehetőséget.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Előfizetések kezelése a partner Center API-kkal

A partner Center API-k segítségével is elvégezheti az életciklus-kezelést, és kezelheti az előfizetések számláit. További információ: [előfizetés létrehozása kereskedelmi piactér-termékekhez](/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>További lépések

- [Kereskedelmi Piactéri ajánlatok vásárlása](csp-commercial-marketplace-purchase.md)
- [Tudnivalók a kereskedelmi piactéren elérhető számlázásról](csp-commercial-marketplace-billing.md)