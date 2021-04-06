---
title: A saját szolgáltatások megvásárlása a CSP-ben
description: Ismerje meg, hogy a CSP-program partnerei Hogyan vehetik igénybe az ügyfeleknek a saját szolgáltatásaikat, például az Azure-foglalásokat a partner Centerben megvásárolt előfizetésekhez.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4feaa8cba8ba17f553b5e936dcf892ffbf7ccc82
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441302"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>A partner Centerben a saját termékeinek vagy szolgáltatásainak megvásárlására jogosult ügyfelek számára

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Értékesítési ügynök

Ez a cikk azt mutatja be, hogy a felhőalapú megoldás-szolgáltatói (CSP) programban szereplő partnerek Hogyan vehetik igénybe az ügyfeleket a saját szolgáltatásaik vagy erőforrásaik megvásárlására.

A CSP program partnerei gyakran használják a partner centert és annak kereskedelmi piactérét, hogy megoldásokat és szolgáltatásokat vásároljanak ügyfeleiknek. A partnerek ezt követően lehetővé teszik egyes ügyfelek számára, hogy közvetlenül a Azure Portal tudják kiépíteni ezeket a szolgáltatásokat.

Íme egy példa. Tegyük fel, hogy vásárolnia kell egy Azure-előfizetést egy ügyfél számára a partner Centerben. Ezután dönthet úgy, hogy az ügyfél nevében további erőforrásokat vagy szolgáltatásokat ad hozzá az előfizetéshez. Ebben az esetben hozzáadhat Azure-foglalásokat az ügyfél előfizetéséhez (például fenntartott, virtuálisgép-példányok hozzáadásával). Ezt követően lehetővé teheti, hogy az ügyfél továbbra is kiépítse az Azure foglalási erőforrásait a Azure Portalban.

Most, hogy az **ügyfél engedélyei** funkcióval további önkiszolgáló lehetőségeket biztosíthat az Azure-erőforrásokkal. Az ügyfél engedélyeinek bekapcsolásával lehetővé teszi, hogy az ügyfelek megvásárolják saját erőforrásaikat (például saját Azure-foglalások vásárlásakor).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Az ügyfél engedélyeinek áttekintése a partner Centerben

Az ügyfél- **fiók** lapon be-és kikapcsolhatja az ügyfél engedélyeit. Ez a funkció jelenleg a következőket támogatja:

- **Azure-foglalások:** Ezen engedély bekapcsolása lehetővé teszi, hogy az ügyfél megvásárolja saját Azure-foglalásait egy adott Azure-előfizetéshez, amelyet már megvásárolt.

Az ügyfél engedélyeinek bekapcsolása előtt jegyezze fel ezeket a fontos pontokat:

- Alapértelmezés szerint az ügyfél engedélyei automatikusan le vannak tiltva (kikapcsolva) a partner Centerben.

- Ahhoz, hogy be lehessen kapcsolni (vagy ki kell kapcsolni) az engedélyeket az ügyfelek számára, hozzá kell rendelnie a felügyeleti ügynök szerepkört a partner Centerben.

  Az értékesítési ügynök vagy az ügyfélszolgálati ügynök szerepkörhöz rendelt partnerek csak olvasási hozzáféréssel rendelkeznek, és nem kapcsolhatják be vagy ki az ügyfél engedélyeit.

- A kiválasztott ügyfelekre vonatkozó engedélyeket bekapcsolhatja (engedélyezheti).

- A partneri központ irányítópultján vagy a [partner Center API](/partner-center/develop/manage-customers)-kon keresztül engedélyezheti (vagy kikapcsolhatja) az ügyfelek engedélyeit.

- Miután bekapcsolta az engedélyeket egy adott ügyfél számára, az ügyfél által végzett későbbi vásárlások kell fizetnie. Ha az ügyfelek szeretnék cserélni, megszakítani vagy megújítani az általuk készített vásárlást (vagy szeretnék módosítani a foglalás kezdeti hatókörét), azok nem lesznek képesek. Meg kell kérniük a partnert, hogy segítséget nyújtson a vásárlások cseréjéhez, megszakításához és megújításához, vagy később módosítsa a foglalás hatókörét.  

- Miután bekapcsolta az engedélyeket egy adott ügyfél számára, **nem** kap értesítést az ügyfél által végzett későbbi vásárlásokról.

- Az ügyfél által végzett későbbi vásárlások a partner Centerben jelennek meg, az Ön által végzett vásárlások mellett. Ezeket a vásárlásokat az ügyfél **Order History (megrendelési előzmények** ) lapján, a **foglalások** lapon vagy a [**tevékenység naplójában**](activity-logs.md)találja.

>[!NOTE]
> Az ügyfelek díjszabásával és a vásárlások kezelésével kapcsolatos információkért lásd: Segítség az ügyfelek számára a [megvásárolt foglalások kezelésében](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Engedélyt ad az ügyfeleknek a saját Azure-foglalások megvásárlására

Az Azure-szolgáltatások kedvezményes díjszabással vásárolhatják meg az Azure-szolgáltatásokat. Ha többet szeretne megtudni az Azure-foglalások előnyeiről, tekintse meg a [Mi a Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Most már dönthet úgy is, hogy az ügyfelek nevében megvásárolja az Azure-foglalásokat, ahogy azt már megtette. Vagy megadhatja az ügyfeleknek a saját Azure-foglalások megvásárlásához szükséges engedélyt.

>[!NOTE]
> Miután engedélyezte az ügyfeleknek, hogy megvásárolják saját Azure-foglalásait, segítenek a megvásárolt foglalások kezelésében. További információ: Segítség az [ügyfelek számára a megvásárolt foglalások kezeléséhez](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Annak engedélyezése, hogy az ügyfelek megvásárolják saját Azure-foglalásait

1. Győződjön meg arról, hogy az ügyfél rendelkezik egy meglévő Azure-csomaggal vagy az Ön nevében megvásárolt Azure globális előfizetéssel.

2. Ellenőrizze, hogy az ügyfél hozzá van-e rendelve a **tulajdonosi** szerepkörhöz ehhez az előfizetéshez.

3. A saját Azure-foglalások megvásárlásához engedélyezze az ügyfelek engedélyeit ( **a** funkció bekapcsolása).

Az egyes lépések alább láthatók.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Annak ellenőrzése, hogy az ügyfél rendelkezik-e meglévő Azure-előfizetéssel

Ahhoz, hogy az ügyfelek engedélyt adjanak saját Azure-foglalások megvásárlására, ellenőriznie kell, hogy az ügyfél rendelkezik-e meglévő Azure-csomaggal vagy Azure globális előfizetéssel. Ha az ügyfél nem jelenít meg aktuális Azure-előfizetést a partner Centerben, az ügyfél engedélyeinek bekapcsolása előtt meg kell vásárolnia az előfizetést.

- Ha szeretné megtekinteni, hogy egy ügyfél már rendelkezik Azure-előfizetéssel, jelentkezzen be a partner Center irányítópultra, majd válassza a **CSP** , majd az **ügyfelek** elemet. Válassza ki az adott ügyfelet a listából. Ezután válassza az **előfizetések** lehetőséget, és keresse meg az Azure-csomag vagy az Azure Global használati alapú előfizetéseit.

- Ha egy ügyfél nem rendelkezik meglévő Azure-előfizetéssel, vásárolhat előfizetést. Lásd: [Az Azure-csomag megvásárlása](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Ellenőrizze, hogy az ügyfél megfelelő szerepkört rendelt-e az Azure-ban

Miután meggyőződött arról, hogy az ügyfél rendelkezik egy meglévő Azure-előfizetéssel, ellenőriznie kell, hogy az ügyfélhez társított fő felhasználók hozzá lettek-e rendelve a megfelelő **tulajdonosi** szerepkörhöz az adott Azure-előfizetéshez. Ez a szerepköralapú hozzáférés (RBAC), amelyet az ügyfélnek meg kell vásárolnia az Azure-előfizetéshez, amelyet megvásárolt.

Előfordulhat, hogy néhány partner már hozzárendelte a **tulajdonosi** szerepkört azokhoz az ügyfelekhez, akik aktívan szeretnék kezelni és saját Azure-erőforrásaikat kiépíteni Ha már hozzárendelte a **tulajdonosi** állapotot egy ügyfélhez a számukra megvásárolt korábbi előfizetések kezeléséhez, kihagyhatja ezt a lépést.  

> [!IMPORTANT]
> Ha egy ügyfél még nincs hozzárendelve a **tulajdonosi** szerepkörhöz, hibaüzenetet kap a Azure Portal az Azure-foglalások megvásárlásának megakadályozása érdekében.

Annak ellenőrzéséhez, hogy az ügyfél hozzá van-e rendelve egy Azure-előfizetés **tulajdonosi** szerepköréhez:

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).

2. Válassza a **CSP**, majd az **ügyfelek** lehetőséget, és válassza ki az adott ügyfelet.

3. Válassza ki az ügyfél **előfizetéseit** , és keresse meg az adott Azure-előfizetést.

4. Kattintson az ügyfél előfizetése melletti **kezelés** gombra. Ekkor megnyílik a [Azure Portal](https://portal.azure.com/).

5. A **tulajdonosi** szerepkör egy adott felhasználóhoz való hozzárendeléséhez kövesse az alábbi lépéseket egy [felhasználó rendszergazdaként való hozzárendeléséhez](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Az ügyfél engedélyeinek bekapcsolása vagy kikapcsolása saját Azure-foglalások megvásárlásához

Miután meggyőződött arról, hogy az ügyfél rendelkezik egy meglévő Azure-előfizetéssel, és a felhasználók hozzá vannak rendelve a **tulajdonosi** szerepkörhöz az előfizetéshez, készen áll az ügyfél engedélyeinek bekapcsolására. Ezekkel a lépésekkel kikapcsolhatja (letilthatja) az ügyfél engedélyeit. A partneri központ irányítópultján vagy a [partner Center API](/partner-center/develop/manage-customers)-kon keresztül engedélyezheti vagy letilthatja az ügyfelek engedélyeit.

Felhasználói engedélyek bekapcsolása (vagy kikapcsolása) a partner Centerben:

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).

2. A bal oldali navigációs menüben válassza a **CSP**, majd az **ügyfelek** lehetőséget. Megjelenik egy ügyfél lista.

3. Válasszon ki egy adott ügyfél nevét.

4. Válassza a **fiók** lehetőséget az ügyfél menüben. Megjelenik az ügyfél- **fiók** lap.

5. Keresse meg az **ügyfél engedélyeinek** területét az oldal alján.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Ügyfél engedélyei a fiók lapon." border="true":::

6. Az **Azure-foglalások** területen keresse meg az **ügyfél megvásárlásának engedélyezése** lehetőséget.

7. Az ügyfél engedélyeinek bekapcsolásához helyezze át a kapcsolót **a beállítás melletti pozícióba** . Az ügyfél engedélyeinek kikapcsolásához helyezze át a kapcsolót a **kikapcsolt** pozícióra.

>[!NOTE]
> Ha meg szeretné tudni, hogy mi történik, amikor bekapcsolja az ügyfél saját Azure-foglalásának megvásárlására vonatkozó engedélyeit, tekintse meg a következő témakört: [az ügyfél engedélyeinek áttekintése a fiókpartner](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)
>
>Az ügyfél engedélyeinek bekapcsolásával (vagy kikapcsolásával) a tevékenység naplója rögzíti az egyes műveleteket. (Ez a napló akkor érhető el, ha a partner Center irányítópultjának tetején kiválasztja a fogaskerék ikont). Ha be-vagy kikapcsolja az ügyfelek engedélyeit, a művelet az **ügyfél-vásárlási engedélyek létrehozása** vagy az **ügyfél-vásárlási engedélyek törlése** lehetőséggel jelenik meg a tevékenység naplójában.

## <a name="help-customers-manage-reservations-they-purchase"></a>Segítsen az ügyfeleknek a megvásárolt foglalások kezelésében

Miután megadta az ügyfeleknek, hogy megvásárolják saját Azure-foglalásait, könnyebben kezelhetik a megvásárolt erőforrásokat. Az ügyfelek az Azure-foglalások számos aspektusát kezelhetik közvetlenül a [Azure Portal](https://portal.azure.com/). Segítségre van szükségük az Azure-foglalások a CSP-előfizetésen belüli megvásárlásának néhány további aspektusának kezeléséhez.  

Segítse az ügyfeleket az Azure-foglalások ezen szempontjainak kezelésében:

- Az ügyfeleknek az Azure-foglalások díjait kell fizetniük
- Az Azure-foglalások használatának optimalizálása az ügyfelek számára
- Mi történik, ha az ügyfelek közös hatókörű foglalásokat vásárolnak?
- Mi történik, ha az ügyfelek módosítani szeretnék, megszakítják és megújítják a foglalást, vagy megváltoztathatják a hatókörét?

**Az ügyfelek árai a foglalásuk után fizetendők.** Az ügyfél az Azure-foglalásokat egy korábban a CSP-partner számlázási fiókjában vásárolt előfizetés alapján vásárolja meg. Az ügyfél által az előfizetés alapján megvásárolt Azure-foglalások díjait is Ön határozza meg. Ez az ár különbözhet a Azure Portalban megjelenő webes közvetlen díjszabástól.

**Hogyan optimalizálhatja az ügyfelek a foglalások használatát.** Előfordulhat, hogy néhány ügyfél többet szeretne megtudni a foglalások használatának optimalizálásáról, illetve a foglalás kezdeti hatókörének a vásárlás során történő hozzárendeléséről. További információért kérje meg az ügyfeleket, hogy olvassák el az [Azure-erőforrások kezelésével kapcsolatos foglalásokat](/azure/cost-management-billing/reservations/manage-reserved-vm-instance).

**Mi történik, ha egy ügyfél megosztott hatókörű foglalást vásárol?** Ha az ügyfelek egy korábbi CSP-előfizetésen alapuló foglalást vásárolnak, és megosztott hatókört rendelnek hozzá a foglaláshoz, akkor az ügyfél által a CSP által megadott összes kedvezmény érvényes lesz a CSP-partner által az adott ügyfél számára megvásárolt összes előfizetés esetében.

**Mit kell tenniük az ügyfeleknek, ha szeretnének Exchange-et, megszakítani vagy megújítani az általuk készített vásárlást, vagy módosítani a foglalás kezdeti hatókörét?** Az ügyfeleknek fel kell kérniük a partnert arra, hogy megváltoztassák a foglalás kezdeti hatókörét. Emellett partneri segítségre van szükségük a foglalások cseréjéhez, megszakításához vagy megújításához. Ezek a feladatok önmagukban nem hajthatók végre foglalással a CSP-partner által vásárolt előfizetések alapján.

## <a name="next-steps"></a>Következő lépések

- [Azure-foglalások vásárlása az ügyfelek nevében](azure-reservations-buying.md)

- [Partneri központ – Microsoft-foglalások eladása](azure-reservations.md)

- [Azure-foglalások kezelése az ügyfelek nevében](azure-reservations-manage.md)