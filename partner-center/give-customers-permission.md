---
title: Annak érdekében, hogy az ügyfelek saját szolgáltatásokat vásárolnak a CSP-ban
description: Megtudhatja, hogyan használhatja a CSP-programpartnereket arra, hogy az ügyfelek megvásárolják saját szolgáltatásaikat, például az Azure Reservationst egy, a Partnerközpont.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150760"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Adjon engedélyt az ügyfeleknek Partnerközpont saját termékeik vagy szolgáltatásaik vásárlására

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Értékesítési ügynök

Ez a cikk bemutatja, hogy a Felhőszolgáltató (CSP) program egyik partnere hogyan adhat engedélyt az ügyfélnek arra, hogy megvásároljon egyes szolgáltatásokat vagy erőforrásokat.

A CSP-programban részt vevő partnerek gyakran Partnerközpont piactéren vásárolnak megoldásokat és szolgáltatásokat az ügyfeleik számára. A partnerek ezt követően lehetővé teszik, hogy egyes ügyfelek közvetlenül a Azure Portal.

Íme egy példa. Tegyük fel, hogy vásárol egy Azure-csomagra való előfizetést egy Partnerközpont. Ezután úgy dönt, hogy az ügyfél nevében további erőforrásokat vagy szolgáltatásokat ad hozzá az előfizetéshez. Ebben az esetben Azure-foglalásokat adhat hozzá az ügyfél előfizetéséhez (például fenntartott virtuálisgép-példányok hozzáadásához). Ezután engedélyezheti az ügyfélnek, hogy további Azure-foglalási erőforrásokat létesítsen a Azure Portal.

Az **Ügyfélengedélyek** funkcióval mostantól több önkiszolgáló lehetőséget adhat az ügyfeleknek az Azure-erőforrásokhoz. Ha bekapcsolja az engedélyeket az ügyfél számára, lehetővé teszi, hogy az ügyfelek saját erőforrásokat vásárolnak (például saját Azure-foglalásokat vásárolnak).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Az ügyfélengedélyek áttekintése a Partnerközpont

Az Ügyfélfiók **oldalon** kapcsolhatja be (vagy kikapcsolhatja) az ügyfélengedélyeket. Ez a funkció jelenleg a következő funkciókat támogatja:

- **Azure Reservations:** Ha bekapcsolja ezt az engedélyt, az ügyfél megvásárolhatja a saját Azure-foglalását egy adott Azure-előfizetéshez, amit Ön vásárolt számukra.

Mielőtt bekapcsolja az ügyfélengedélyeket, vegye figyelembe a következő fontos pontokat:

- Alapértelmezés szerint az ügyfélengedélyek automatikusan le vannak tiltva (ki vannak kapcsolva) a Partnerközpont.

- Ahhoz, hogy be tudja kapcsolni (vagy kikapcsolja) az engedélyeket egy ügyfél számára, rendszergazdai ügynök szerepkört kell hozzárendelnie a Partnerközpont.

  Az értékesítési ügynök vagy az ügyfélszolgálati ügynök szerepkörrel rendelkező partnerek csak olvasási hozzáféréssel rendelkeziknak, és nem kapcsolják be vagy ki az ügyfélengedélyeket.

- Az engedélyeket bármely ön által választott ügyfélhez bekapcsolhatja (engedélyezheti).

- Az ügyfélengedélyeket a következő API-Partnerközpont kapcsolhatja be [(vagy Partnerközpont ki:](/partner-center/develop/manage-customers).

- Miután bekapcsolta (engedélyezi) az engedélyeket egy adott ügyfél számára, az Ön felelőssége lesz az ügyfél által történt minden további vásárlásért fizetnie. Ha az ügyfelek cserére, lemondásra vagy megújításra szeretnék használni a megvásárolt vásárlást (vagy módosítani szeretnék a foglalás kezdeti hatókörét), akkor ezt nem fogják tudni megtenni. A partner megkéri, hogy segítsen Önnek a vásárlások cseréjében, lemondásában és megújításában, vagy a foglalás hatókörének későbbi módosításaiban.  

- Miután bekapcsolta egy adott ügyfél engedélyét, nem kap értesítést az ügyfél által történt későbbi vásárlásról. 

- Az ügyfél által történt későbbi vásárlások a Partnerközpont az Ön által történt vásárlásokkal együtt jelennek meg. Ezeket a vásárlásokat az ügyfél  Rendelési előzmények oldalán, a **Foglalások** oldalon vagy a Tevékenységnaplóban [**találja.**](activity-logs.md)

>[!NOTE]
> Az ügyfél által fizetett árakról és arról, hogyan segíthet az ügyfeleknek a vásárlások kezelésében, lásd: Segítség az ügyfeleknek a megvásárolt [foglalások kezeléséhez.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Engedélyt adhat az ügyfeleknek a saját Azure-foglalásaik vásárlásra

Az Azure Reservations nagyszerű módja az Azure-szolgáltatások kedvezményes áron való vásárlásának. Az Azure Reservations előnyeivel kapcsolatos további információkért lásd: [Mi az az Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Most már úgy vásárolhat Azure-foglalásokat az ügyfelek nevében, ahogyan eddig is. Vagy engedélyt adhat az ügyfeleknek arra, hogy megvásárolják saját Azure-foglalásukat.

>[!NOTE]
> Miután engedélyt adott az ügyfeleknek a saját Azure-foglalásaik megvásárlására, segíthet nekik a megvásárolt foglalások kezelésében. További információ: Segítség az ügyfeleknek [a megvásárolt foglalások kezeléséhez.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Annak érdekében, hogy az ügyfelek megvásárolják saját Azure-foglalásukat

1. Ellenőrizze, hogy az ügyfél rendelkezik-e a nevükben megvásárolt Meglévő Azure-csomag vagy Azure Globális előfizetéssel.

2. Ellenőrizze, hogy az ügyfélhez hozzá lett-e rendelve **az előfizetés tulajdonosi** szerepköre.

3. Engedélyezze az ügyfélengedélyeket (kapcsolja be ezt **a** funkciót) a saját Azure-foglalások megvásárlásához.

Minden lépés alább látható.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Annak ellenőrzése, hogy az ügyfél rendelkezik-e meglévő Azure-előfizetéssel

Mielőtt engedélyt adna az ügyfeleknek a saját Azure-foglalásaik vásárlására, ellenőriznie kell, hogy az ügyfél rendelkezik-e meglévő Azure-csomaggal vagy Globális Azure-előfizetéssel. Ha az ügyfél nem jeleníti meg az aktuális Azure-előfizetést a Partnerközpont, akkor az ügyfélengedélyek bekapcsolás előtt meg kell vásárolnia számukra egy előfizetést.

- Ha látnia kell, hogy egy ügyfél már rendelkezik-e Azure-előfizetéssel, jelentkezzen be a Partnerközpont irányítópultra, majd válassza a **CSP,** majd az **Ügyfelek lehetőséget.** Válassza ki az adott ügyfelet a listából. Ezután válassza **az Előfizetések** lehetőséget, és keresse meg az Azure-csomagra vagy az Azure Globalra vonatkozó használatalapú előfizetéseket.

- Ha egy ügyfél nem rendelkezik meglévő Azure-előfizetéssel, akkor vásárolhat egyet. Lásd: [Az Azure-csomag megvásárlása.](purchase-azure-plan.md)

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Annak ellenőrzése, hogy az ügyfél a megfelelő szerepkört rendelte-e hozzá az Azure-ban

Miután ellenőrizte, hogy az ügyfél rendelkezik-e meglévő Azure-előfizetéssel, azt is ellenőriznie kell, hogy az ügyfélhez társított kulcsfelhasználók a megfelelő Tulajdonos szerepkört kapták-e az adott Azure-előfizetéshez.  Ez az a szerepköralapú hozzáférés (RBAC), amelyre az ügyfélnek Azure-foglalásokat kell vásárolnia egy Ön által megvásárolt Azure-előfizetéshez.

Előfordulhat, hogy egyes  partnerek már hozzárendelték a Tulajdonos szerepkört azon ügyfelekhez, akik aktívan szeretnék felügyelni és kiépíteni a saját Azure-erőforrásaikat. Ha már hozzárendelt **tulajdonosi** állapotot egy ügyfélhez a számukra megvásárolt korábbi előfizetések kezeléséhez, kihagyhatja ezt a lépést.  

> [!IMPORTANT]
> Ha egy ügyfélhez nincs  tulajdonosi szerepkör rendelve, hibaüzenetet kap a Azure Portal megakadályozza, hogy Azure-foglalásokat vásároljon.

Annak ellenőrzése, hogy az ügyfélhez hozzá lett-e rendelve **az** Azure-előfizetés Tulajdonos szerepköre:

1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)

2. Válassza **a CSP,** majd **az Ügyfelek lehetőséget,** és válassza ki az adott ügyfelet.

3. Válassza **az adott ügyfél előfizetései** lehetőséget, és keresse meg az adott Azure-előfizetést.

4. Válassza **az ügyfél** előfizetése melletti Kezelés gombot. Ha így tesz, megnyílik [a Azure Portal.](https://portal.azure.com/)

5. Ha **tulajdonosi szerepkört szeretne** hozzárendelni egy adott felhasználóhoz, kövesse az alábbi lépéseket A felhasználó [rendszergazdaként való hozzárendelése lépéseit.](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Saját Azure-foglalások vásárlására vonatkozó ügyfélengedélyek be- vagy kikapcsolása

Miután ellenőrizte, hogy az ügyfél rendelkezik-e  meglévő Azure-előfizetéssel, és a felhasználókhoz hozzá van-e rendelve az előfizetés tulajdonosi szerepköre, készen áll az ügyfélengedélyek bekapcsolára (engedélyezésére). Ezekkel a lépésekkel kikapcsolhatja (letilthatja) az ügyfelek engedélyeit. Az ügyfélengedélyeket a következő API Partnerközpont vagy Partnerközpont [engedélyezheti vagy tilthatja le:](/partner-center/develop/manage-customers).

Az ügyfélengedélyek bekapcsolás (vagy kikapcsolása) a Partnerközpont:

1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)

2. A bal oldali navigációs menüben válassza a **CSP,** majd az **Ügyfelek lehetőséget.** Megjelenik egy ügyféllista.

3. Válasszon ki egy adott ügyfélnevet.

4. Az **ügyfélmenüben** válassza a Fiók lehetőséget. Megjelenik **az ügyfélfiók** oldala.

5. Keresse meg **az Ügyfélengedélyek** területet a lap alján.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Ügyfélengedélyek a Fiók lapon." border="true":::

6. Az **Azure Reservations alatt** keresse meg az Ügyfél **vásárlásának engedélyezése** lehetőséget.

7. Az ügyfélengedélyek bekapcsoláshoz helyezze át a kapcsolót a beállítás mellett a **Be állásba.** Az ügyfélengedélyek kikapcsolhoz helyezze át a kapcsolót a **Ki állásba.**

>[!NOTE]
> Ha többet szeretne megtudni arról, hogy mi történik még, ha bekapcsolja az ügyfél saját Azure-foglalások megvásárlására vonatkozó engedélyét, tekintse meg a következő témakört: Az ügyfélengedélyek áttekintése a [Partnerközpont.](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)
>
>Ha bekapcsolja (vagy kikapcsolja) az ügyfélengedélyeket, a Tevékenységnapló rögzíti az egyes tevékenységeket. (Ez a napló akkor érhető el, ha a fogaskerék ikonra kattint a Partnerközpont irányítópult tetején). Ha be- vagy kikapcsolja az ügyfélengedélyeket,  a művelet ügyfélvásárlási engedélyek létrehozása vagy Ügyfélvásárlási engedélyek törlése műveletként jelenik meg a tevékenységnaplóban. 

## <a name="help-customers-manage-reservations-they-purchase"></a>Segítség az ügyfeleknek a megvásárolt foglalások kezeléséhez

Miután engedélyt adott az ügyfeleknek a saját Azure-foglalásaik megvásárlására, ön segíthet számukra a megvásárolt erőforrások jobb kezelésében. Az ügyfelek az Azure-foglalások számos aspektusát közvetlenül a [Azure Portal.](https://portal.azure.com/) Segítségre van szükségük a CSP-előfizetésen belül megvásárolt Azure-foglalások néhány egyéb aspektusának kezeléséhez.  

Segítsen az ügyfeleknek jobban megérteni az Azure Reservations ezen aspektusainak felügyeletét:

- Az azure-beli foglalásokért az ügyfelek által fizetett árak
- Hogyan optimalizálják az ügyfelek az Azure Reservations használatát?
- Mi történik, ha az ügyfelek megosztott hatókörrel vásárolnak foglalásokat?
- Mi történik, ha az ügyfelek módosítani, törölni vagy megújítani szeretnék a foglalást, vagy módosítani szeretnék annak hatókörét?

**Az ügyfelek által a foglalásokért fizetett árak.** Az ügyfél a CSP-partner számlázási fiókjában korábban megvásárolt előfizetés alapján vásárolja meg az Azure Reservationst. Az ügyfélnek az előfizetés alapján vásárolt Azure-foglalások árát Is Ön állíthatja be. Ez az ár eltérhet az ügyfél által a webcímen látható Web Direct-Azure Portal.

**Hogyan optimalizálják az ügyfelek a foglalások használatát?** Egyes ügyfelek számára hasznos lehet, ha többet tud meg arról, hogyan optimalizálhatja a foglalás használatát, vagy hogyan rendelheti hozzá a foglalás kezdeti hatókörét a vásárlás során. További információért kérje meg az ügyfeleket, hogy olvassa el [a Foglalások kezelése Az Azure-erőforrások esetében cikkeket.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**Mi történik, ha egy ügyfél vásárol egy foglalást egy megosztott hatókörrel?** Ha az ügyfelek egy korábbi CSP-előfizetés alapján vásárolnak foglalást, és megosztott hatókört rendelnek hozzá a foglaláshoz, az ügyfél által a CSP által adott kedvezmények a CSP-partner által az adott ügyfél számára megvásárolt összes előfizetés megfelelő használatára vonatkoznak.

**Mit tegyenek az ügyfelek, ha cserére, lemondásra vagy megújításra van szükség egy megvásárolt vásárlásra, vagy módosítani szeretnék a foglalás kezdeti hatókörét?** Az ügyfeleknek meg kell kérniük a partnerüket, hogy segítsenek módosítani a foglalás kezdeti hatókörét. Emellett egy partner segítségére is szükségük van a foglalás cseréjéhez, lemondáshoz vagy megújításhoz. Ezeket a feladatokat nem hajthatja végre maguk a foglalásokkal a CSP-partner által megvásárolt előfizetések alapján.

## <a name="next-steps"></a>Következő lépések

- [Azure Reservations vásárlása az ügyfelek nevében](azure-reservations-buying.md)

- [Partnerközpont – Microsoft Reservations értékesítés](azure-reservations.md)

- [Azure-foglalások kezelése az ügyfelek nevében](azure-reservations-manage.md)