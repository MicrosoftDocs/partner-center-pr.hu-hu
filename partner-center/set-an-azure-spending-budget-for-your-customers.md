---
title: Azure-költségvetés beállítása az ügyfelek számára
ms.topic: how-to
ms.date: 03/17/2021
description: Megtudhatja, hogyan állíthat be vagy távolíthat el havi Azure-költségkereteket az ügyfelek számára, valamint megtekintheti az Azure-költségadatokat, és hogyan állíthat be költségvetéssel kapcsolatos értesítéseket.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855352"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Havi Azure-költségvetések beállítása, ellenőrzése vagy eltávolítása a Partnerközpont

**Megfelelő szerepkörök:** Rendszergazdai ügynök

Havi [Azure-költségkeretet állíthat](#set-azure-spending-budget) be az ügyfelek számára a Partnerközpont. Ez segít az ügyfeleknek az Azure-kiadások kezelésében. Ezzel a lehetőséggel összehasonlíthatja az ügyfelek Azure-kiadásait a költségvetéssel a hónap során. Emellett segít az ügyfeleknek az Azure-kiadások költségvetésében is, hogy a havi számla ne magasabb, mint amit várnak.

> [!NOTE]  
> Ez a funkció nem érhető el a tesztboxban vagy a Tesztelés éles környezetben (TIP) fiókokban.

Miután [beállította az Azure-költségvetést az ügyfél(ök)hez,](#set-azure-spending-budget)a következő módokon is áttekintheti az ügyfélhasználatot. Ezek a lehetőségek segíthetnek a helytelenül konfigurált szolgáltatások vagy szokatlan trendek felderítésében, amelyek csalásra utalhatnak. Ezután az ügyfél(ök) segítségével azonosíthatja a kiváltó okot és kezelheti a költségeket. Szükség esetén magasabb [összegre](#set-azure-spending-budget) is módosíthatja az ügyfél költségvetését.

- [Az aktuális Azure-kiadások ellenőrzése](#check-current-azure-spending)

- [E-mail-értesítéseket kapcsol be arra az értesítésre, amikor egy ügyfél költségkerete közeledik](#notifications-for-budget-limits)

- [Elemi költségek megtekintése szolgáltatás szerint a használatalapú előfizetések esetén](#itemized-costs-by-service)

Az [ügyfelekre vonatkozó Azure-költségkeretet](#remove-azure-spending-budget) bármikor eltávolíthatja.

## <a name="azure-spending-data"></a>Azure-beli kiadási adatok

Az Azure-költségadatok becsült *összegek,* és a *tényleges számlázási összegek eltérőek lehetnek.* Az adatok értéke *nem* tükrözi az adókat, jóváírásokat, helyesbítéseket és az esetlegesen fizetendő egyéb díjakat.

A költési adatok *naponta egyszer frissülnek.* Az ügyfelek továbbra is használhatnak (és díjat számolunk fel) az Azure-szolgáltatások és -erőforrások használata esetén, ha nem módosítja a fiókbeállításokat a Azure Portal.

## <a name="set-azure-spending-budget"></a>Az Azure-költségvetés beállítása

Havi *Azure-költségkeretet állíthat* be több ügyfélhez a Partnerközpont:

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).

2. A bal oldali menü **CSP** menüjében válassza az **Azure-kiadások lehetőséget.**

3. Az **Azure-kiadások oldal** Ügyfelek Microsoft Azure **előfizetéssel** alatt válassza ki azokat az ügyfeleket, akiknek költségvetést szeretne beállítani.

4. Adjon meg egy értéket a **Havi költségvetés mezőben.**

5. A **módosítások mentéshez** válassza az Alkalmaz lehetőséget.

Egyéni ügyfél *előfizetési beállításaiban is* beállíthatja a költségvetést:

1. Jelentkezzen be a Partnerközpont irányítópultjába.

2. A bal oldali menü **CSP** menüjében válassza az Ügyfelek **lehetőséget.**

3. Az Ügyfelek **lapon** válassza ki az ügyfél **cégnevét.**

4. Az ügyfél Előfizetések **lapján,** a **Használatalapú előfizetés** alatt válassza a **Költségvetés módosítása lehetőséget.**

5. Adja meg a költségvetés értékét.

6. A **módosítások mentéshez** válassza az Alkalmaz lehetőséget.

## <a name="remove-azure-spending-budget"></a>Azure-költségvetés eltávolítása

Az ügyfelek *havi Azure-költségkeretét* a következő Partnerközpont:

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).

2. A bal oldali menü **CSP** menüjében válassza az **Azure-kiadások lehetőséget.**

3. Az **Azure-kiadások oldal** Ügyfelek Microsoft Azure **előfizetéssel** területén válassza ki azokat az ügyfeleket, akiknek a költségvetését el szeretné távolítani.

4. Válassza a **Költségvetés eltávolítása lehetőséget.**

## <a name="check-current-azure-spending"></a>Az aktuális Azure-kiadások ellenőrzése

Az ügyfelek *aktuális Azure-kiadásait* és havi költségkeretét bármikor nyomon követheti:

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).

2. A bal oldali menü **CSP** menüjében válassza az **Azure-kiadások lehetőséget.**

3. Az **Azure-kiadások** oldalon a Customers **with Microsoft Azure subscriptions**(Ügyfelek Microsoft Azure-előfizetéssel) alatt áttekintheti az ügyfelek havi költségvetését, az aktuális költségbecsléseket és a felhasznált költségvetés százalékos arányát.

## <a name="notifications-for-budget-limits"></a>Költségvetési korlátokra vonatkozó értesítések

Bekapcsolhatja *az e-mail-értesítéseket,* ha az ügyfél havi költségkerete a költségkerethez közeledik. Ha bekapcsolja ezt a beállítást, értesítést kap, ha az ügyfelek a havi költségkeretük 80%-át vagy többet használják ki. Ezzel a lehetőséggel nyomon tudja tartani az Azure-számlát. E-mail-értesítések konfigurálása:

1. Jelentkezzen be a Partnerközpontba.

2. Ugrás a **Beállítások lapra.**

3. Válassza **a Saját beállítások lehetőséget.**

4. Ha még nem, konfigurálja az előnyben részesített e-mail-címet.

5. Konfigurálja az értesítés előnyben részesített nyelvét.

6. Az **Értesítési beállítások** szakaszban válassza a CSP **lapot.**

7. Jelölje be az Azure-beli **költési értesítés e-mailes beállítását,** majd a **Mentés lehetőséget.**


## <a name="itemized-costs-by-service"></a>Elemi költségek szolgáltatás szerint

A *használatalapú előfizetések* tételes költségeit (és becsült használatát) szolgáltatás szerint is megtekintheti:

1. Jelentkezzen be a Partnerközpontba.

2. A bal oldali menü **CSP** menüjében válassza az Ügyfelek **lehetőséget.**

3. Az Ügyfelek **lapon** válassza ki az ügyfél **Cégnevét.**

4. Az ügyfél Előfizetések **lapján,** a **Használatalapú** előfizetések alatt válassza ki az Előfizetés **nevét.**

5. Az előfizetés oldalán áttekintheti a  tételes költségeket szolgáltatás  szerint, valamint a Becsült használatot az aktuális hónapra.


## <a name="next-steps"></a>Következő lépések

- [Új kereskedelmi felület a CSP-ben – Azure-számlázás](azure-plan-billing.md)
