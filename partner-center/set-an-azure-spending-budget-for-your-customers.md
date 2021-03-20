---
title: Azure-költségvetés beállítása az ügyfelek számára
ms.topic: how-to
ms.date: 03/17/2021
description: Megtudhatja, hogyan állíthatja be vagy távolíthatja el az ügyfelek havi Azure-költségkeretét, valamint megtekintheti az Azure-kiadások adatait, és megadhatja a költségvetéssel kapcsolatos értesítéseket is.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712749"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>A partner Center ügyfelei számára havi Azure-költségkeretek beállítása, bejelölése vagy eltávolítása

**Megfelelő szerepkörök**

- Felügyeleti ügynök

Megadhatja a partner Center [ügyfeleinek havi Azure-költségkeretét](#set-azure-spending-budget) . Ez segít az ügyfeleknek az Azure-kiadások kezelésében. Ez a beállítás lehetővé teszi, hogy az ügyfelek Azure-kiadásait a hónap folyamán összehasonlítsa a költségvetésbe. Emellett az ügyfelek számára is lehetővé teszi az Azure-kiadások költségvetését, így a havi számla nem nagyobb, mint amennyire várható.

> [!NOTE]  
> Ez a funkció nem érhető el a homokozóban vagy a tesztelés éles (TIP) fiókokban.

Miután [beállította az Azure-költségkeretet az ügyfél (ek) számára](#set-azure-spending-budget), a következő módokon tekintheti át az ügyfelek használatát. Ezek a lehetőségek segíthetnek a helytelenül konfigurált szolgáltatások vagy szokatlan, csalást okozó trendek felderítésében. Ezután a felhasználó (k) használatával azonosíthatja a kiváltó okot, és kezelheti a költségeket. Ha szükséges, [az ügyfél költségvetését is megváltoztathatja](#set-azure-spending-budget) magasabb értékre.

- [Aktuális Azure-kiadások keresése](#check-current-azure-spending)

- [E-mail-értesítések bekapcsolása, ha az ügyfél kiadásai közel vannak a költségvetési korláthoz](#notifications-for-budget-limits)

- [Részletezett költségek megtekintése szolgáltatás alapján a használaton alapuló előfizetésekhez](#itemized-costs-by-service)

Az Azure- [költségkeretet bármikor el is távolíthatja](#remove-azure-spending-budget) az ügyfelekhez.

## <a name="azure-spending-data"></a>Az Azure kiadásai

Az Azure-kiadási adatok *becsültek* , a *tényleges számlázási összegek pedig eltérőek lehetnek*. Az adatok értéke *nem tükrözi* az adókat, a krediteket, a beállításokat és az esetlegesen alkalmazandó egyéb díjakat.

A kiadási adat *naponta egyszer frissül*. Az ügyfelek továbbra is használhatják az Azure-szolgáltatások és-erőforrások használatát (és díjat számítanak fel), hacsak nem módosítja a fiók beállításait a Azure Portal.

## <a name="set-azure-spending-budget"></a>Az Azure-kiadások költségvetésének beállítása

A partner Centerben több ügyfél számára is *beállíthat havi Azure-költségkeretet* :

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).

2. A bal oldali menü **CSP** területén válassza az Azure- **kiadások** lehetőséget.

3. Az **Azure-kiadások** oldalon Microsoft Azure- **előfizetéssel rendelkező ügyfelek** területen válassza ki azokat az ügyfeleket, akik számára költségvetést kíván beállítani.

4. Adja meg a **havi költségkeret** értékét.

5. A módosítások mentéséhez kattintson az **alkalmaz** gombra.

Megadhat *egy költségvetést is egy egyéni ügyfél* számára az előfizetési beállításokban:

1. Jelentkezzen be a Partnerközpont irányítópultjába.

2. A bal oldali menüben a **CSP** területen válassza az **ügyfelek** lehetőséget.

3. Az **ügyfelek** lapon válassza ki az ügyfél **vállalatának nevét**.

4. Az ügyfél **előfizetések** lapján, a **használaton alapuló előfizetés** területen válassza a **költségvetés módosítása** lehetőséget.

5. Adja meg a költségvetés értékét.

6. A módosítások mentéséhez kattintson az **alkalmaz** gombra.

## <a name="remove-azure-spending-budget"></a>Az Azure-kiadások költségvetésének eltávolítása

A partner Centerben a következő *havi Azure-költségkeretet távolíthatja el* ügyfeleinek:

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).

2. A bal oldali menü **CSP** területén válassza az Azure- **kiadások** lehetőséget.

3. Az **Azure-kiadások** oldalon Microsoft Azure- **előfizetéssel rendelkező ügyfelek** területen válassza ki azokat az ügyfeleket, akiknek a költségvetését el szeretné távolítani.

4. Válassza a **költségvetés eltávolítása** lehetőséget.

## <a name="check-current-azure-spending"></a>Aktuális Azure-kiadások keresése

*Az ügyfelek aktuális Azure-kiadásait és havi költségkereteit bármikor nyomon követheti* :

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).

2. A bal oldali menü **CSP** területén válassza az Azure- **kiadások** lehetőséget.

3. Az **Azure-kiadások** oldalon Microsoft Azure- **előfizetéssel rendelkező ügyfeleknél** tekintse meg az ügyfelek havi költségkeretét, a jelenlegi kiadási becsléseket és a felhasznált költségvetés százalékos arányát.

## <a name="notifications-for-budget-limits"></a>A költségvetési korlátokkal kapcsolatos értesítések

*Bekapcsolhatja az e-mailes értesítéseket* , amikor az ügyfél havi kiadásai elérik a költségvetési korlátot. Ha bekapcsolja ezt a beállítást, a rendszer értesítést küld, ha az ügyfelek a havi költségkeretük 80%-át használják. Ez a beállítás segít megőrizni az Azure-számlázást. E-mail-értesítések konfigurálása:

1. Jelentkezzen be a Partnerközpontba.

2. Válassza a **Beállítások lehetőséget**.

3. Válassza **a saját beállítások** lehetőséget.

4. Ha még nem tette meg, konfiguráljon egy előnyben részesített e-mail címet.

5. Adja meg az értesítéshez használni kívánt nyelvet.

6. Válassza a **CSP** fület az **értesítési beállítások** szakaszban.

7. Keresse meg az Azure- **kiadások** értesítése e-mailben lehetőséget, és **mentse** a következőt:.


## <a name="itemized-costs-by-service"></a>Kitételi költségek szolgáltatás szerint

*A tételes költségeket (és a becsült használatot) a szolgáltatás alapján, a használaton alapuló előfizetések esetében tekintheti* meg:

1. Jelentkezzen be a Partnerközpontba.

2. A bal oldali menüben a **CSP** területen válassza az **ügyfelek** lehetőséget.

3. Az **ügyfelek** lapon válassza ki az ügyfél **vállalatának nevét**.

4. Az ügyfél **előfizetések** lapján, a **használat alapú előfizetések** területen válassza ki az **előfizetés** nevét.

5. Az előfizetés lapján áttekintheti a **részletezett költségeket** a szolgáltatás alapján, valamint az aktuális hónap **becsült felhasználását** .


## <a name="next-steps"></a>Következő lépések

- [Új kereskedelmi felület a CSP-ben – Azure-számlázás](azure-plan-billing.md)
