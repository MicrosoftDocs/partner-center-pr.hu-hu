---
title: CSP regionális engedélyezési bérlők összevonása
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezekkel az utasításokkal konszolidálhatja a különböző országok/régiók bérlőit. Ez magában foglalja az ügyfélfiókok és ügyfél-előfizetések áttelepítésének lépéseit.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 84e5f7f2674e9b2f3c3c26ed2ea49f9bba0e96e0
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276875"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Útmutató a CSP regionális engedélyezési bérlőösszevonáshoz

**A következőkre vonatkozik:** Partnerközpont | Partnerközpont a Microsoft Cloud for US Government

**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök

\[Egyes információk az előre kiadott termékkel kapcsolatosak, amelyek a kereskedelmi forgalomban való nyilvánosságra kerül előtt jelentős mértékben módosíthatók. A Microsoft nem vállal kifejezett vagy törvényi garanciát az itt megjelenő információért.\]

Összevonhatja a vállalat bérlőit. Ezekkel az utasításokkal konszolidálhatja a különböző országok/régiók bérlőit.

>[!NOTE]  
>Tisztában kell lennie az összes kiépített előfizetéssel és licencszámmal abban a fiókban, amelyről átvált. A migrálási folyamat részeként újra kiépíti ugyanezeket az előfizetéseket ugyanazokkal a licencszámokkal az új központi CSP-fiókban. Az exportálási lista funkcióval létrehozhatja azon ügyfelek listáját, akik átlépnek a központosított bérlőre.  A konszolidálás befejezése után nem lehet visszaállni az előző bérlői állapotra. Szükség lehet az ügyfél beavatkozásra is.

## <a name="prepare-for-migration"></a>Előkészületek a migráláshoz

- Jelentkezzen be **Partnerközpont** fiókkal  (az új fiókra átváltáskor), és tekintse át az összes ügyfelet és az ezen ügyfelek számára kiépített szolgáltatásokat.

- Jelentkezzen ki ebből a fiókból.

## <a name="migrate-customer-accounts"></a>Ügyfélfiókok áttelepítése

1. Jelentkezzen be **a Partnerközpont**  az **Átmeneti** (új) fiókkal (arra, amelybe átveszi az ügyfeleket).

2. Válassza az **Ügyfelek** lehetőséget.

3. Válassza **a Viszonteladói kapcsolat kérése lehetőséget.** Megjelenik egy alapértelmezett e-mail-üzenet, amely elküldve lesz az ügyfeleknek. Ez az üzenet egy URL-címet tartalmaz, amely az új fiók egyedi szervezeti Partnerközpont tartalmazza.

4. **Ügyfél beavatkozása:** Győződjön meg arról, hogy az összes átemelni kívánt aktív ügyfél felkeresi ezt az URL-címet. Az URL-cím megnyitásakor a rendszer felkéri az ügyfelet, hogy jelentkezzen be az Office 365 portálra. Az ügyfél ugyanazokkal a szervezeti azonosítóval jelentkezik be, mint az Azure és az Office 365 felügyeleti portálok eléréséhez.

5. Bejelentkezés után a rendszer felkéri  az ügyfélfiók globális rendszergazdáját, hogy küldjön be egy olyan szerződést, amely delegált rendszergazdai jogosultságokat biztosít az új CSP-fióknak. Ha beleegyeznek, az ügyfél kiválasztja a jelölőnégyzetet, és engedélyezi a kapcsolatot.

Az ügyfelek a szerződés beküldtét követően jelennek meg a partner ügyféllistán, egyesével.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Office 365- és nem Azure-beli használatalapú előfizetések áttelepítése

1. Miután az ügyfél aláírta a szerződést, újra létrehozhatja az előfizetéseket a központi partnerbérlőben.

2. A **Partnerközpont** válassza a Customers (Ügyfelek) **lehetőséget.**

3. Nyissa meg annak az ügyfélnek a cégnevét, akiről migelni szeretne.

4. Válassza **az Előfizetés hozzáadása lehetőséget.**

5. Adja hozzá a megfelelő előfizetéseket és licencszámokat a katalógusból. Ellenőrizze a partnerfiókok váltása során **megadott** információkat.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="ügyféllista.":::

6. Válassza a **Küldés lehetőséget.**

   A szolgáltatásokat most már a Váltás partnerfiókból biztosítja **az** ügyfélnek.

7. Ismételje meg ezeket a lépéseket az összes további ügyfél előfizetésének áttelepítéséhez.

Mielőtt továbblépne a következő szakaszra, győződjön  meg arról, hogy a Váltás partnerfiókból területen meglévő összes ügyfél-előfizetés újra ki van építve a **Váltás** partnerfiókra területen.

> [!NOTE]
> A partnereknek az  előfizetések váltása partnerbérlői fiókból fiókra való váltásának napján fel  kell függesztenie Partnerközpont előfizetéseket ugyanazon a napon, amikor az előfizetések át vannak állítva és be vannak állítva az Partnerközpont-ban a Váltás partnerbérlőre fiókban annak érdekében, hogy a kettős számlázás ne fordul elő. A rendszer megtagadja a támogatási kéréseket a kreditekért, mert a számlázásban átfedés lép fel, és nem tiltja le megfelelően az előfizetésből **való váltást.**

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Az Office 365-előfizetések letiltása a Váltás a partnerfiókból alatt

Ha letiltja a CSP-előfizetést a **Partnerfiókok** váltása alatt, azzal leállítja a jövőbeli számlázást. Nem kell manuálisan letiltania az Azure-előfizetéseket, mert az Azure-előfizetések automatikusan le vannak tiltva a migrálási folyamat során.

1. Jelentkezzen be a **Partnerközpont** csp-fiókból való áttéréssel, és lépjen az ügyféllistára. 

2. Nyissa meg az előfizetéseket a letiltásához, majd válassza ki az első letiltani kívánt ajánlatot.

3. Állítsa az előfizetést **felfüggesztettre,** majd válassza a **Küldés lehetőséget.**

   >[!Note]
   >Az előfizetés felfüggesztése biztosítja, hogy a dupla számlázás nem történik meg.

   Az előfizetés fel **van függesztve** az előfizetések listájában.

4. Ismételje meg ezeket a lépéseket az ügyfél összes előfizetése esetén. Ellenőrizze, hogy az összes fel **van-e függesztve.**

5. Válassza ki a listából a következő ügyfelet, és ismételje meg az összes előfizetés letiltásának folyamatát.

## <a name="migrating-azure-usage-based-subscriptions"></a>Használatalapú Azure-előfizetések áttelepítése

Az Office 365 CSP-előfizetésekkel ellentétben az Azure-beli használatalapú CSP-előfizetéseket nem kell manuálisan migrálni. Microsoft Azure-támogatás át fogja telepíteni az Azure-előfizetéseket és az összes  üzembe helyezett szolgáltatást vagy erőforrást a CSP-viszonteladói fiókokról a **VÁLTÁS** CSP-re viszonteladói fiókra. Az átállás során nem fog megszakadni az ügyfél kiszolgálása.

1. Győződjön meg arról, hogy a migrált Azure-előfizetésekkel rendelkező ügyfélfiókok elfogadták az új CSP-fiókra való áttérésre vonatkozó szerződést. 

2. Értesítenie kell a Microsoftot arról, hogy mely ügyfélfiókok állnak készen az áttelepítésre, és meg kell adnia az ügyfél vállalatnevét.

3. A Microsoft migrálta az Azure használatalapú előfizetéseket, és értesíti, ha a migrálás befejeződött.

4. Meg kell erősítenie, hogy a CSP-viszonteladói fiókról váltás  alatt található Azure-előfizetés most fel van jelölve a Partnerközpont előfizetések szakaszban. 

5. Győződjön meg arról, hogy a **Váltás** CSP-viszonteladói fiókra  területen lévő Azure-előfizetésnél az aktív állapot Partnerközpont az ügyfél-előfizetések szakaszban.

   >[!Note]
   > Az előfizetések ügyfél alatti letiltása nem módosítja az ügyfél megjelenését az Ügyfelek listában. Jelenleg nincs lehetőség ügyfelek eltávolítására a listából. A partnereknek el kell kerülniük,  hogy a jövőben előfizetéseket adjanak vissza ezekhez az ügyfelekhez a fiókjukból való áttérésből.

6. Ismételje meg ezeket a lépéseket az összes ügyfélhez elérhető  összes előfizetés esetében, hogy a jövőbeli díjakat leállítsa a váltás fiók(ak)on. A partner egy utolsó számlát kap, amely a lemondás napja és a számlázási időszak utolsó napja közötti fel nem használt napok számára vonatkozó jóváírást is megkapja. A végső számlázási időszak után nem fog számlát generálni.

### <a name="additional-information"></a>További információ

- Ha letiltja az  előfizetést a CSP-fiókról való váltásról, az nem befolyásolja az ügyfél szolgáltatását, ha a szolgáltatást az előfizetés letiltása előtt kiépítik a Váltás  CSP-fiókra fiókból.

- Az előfizetések nem használhatók az ügyfél által, és nem generálnak díjakat, ha fel vannak függesztve vagy törölve.

- Jelenleg nincs mód arra, hogy teljesen eltávolítson egy ügyfelet az Ügyfelek **listából.**
- 
    >[!Note]
    > A partnereknek ugyanazon  a napon fel kell függesztenie az előfizetéseket Partnerközpont partnerbérlői fiókról való váltásra, amikor az előfizetések át vannak állítva és be vannak állítva a Váltás fiókra, hogy a kettős számlázás ne fordul elő.  A Microsoft nem támogatja a kreditek kérését a számlázás bármilyen  átfedése miatt, amely abból ad vissza, hogy nem megfelelően beállította az előfizetésből való váltást felfüggesztettre.

### <a name="simplify-migration-using-export"></a>A migrálás egyszerűsítése az Exportálás használatával

Az **Export függvény használatával** rögzítheti az új konszolidált struktúrában használnia szükséges előfizetéseket:

1. Az **ügyfelek listájának** Partnerközpont válassza az Ügyfelek lehetőséget. 

2. Nyissa meg a kívánt ügyfélnevet.

3. Az **Előfizetések lapon** válassza az **Előfizetések exportálása** lehetőséget az előfizetések részleteinek Excel-fájlba való exportálásához.

4. Ezzel a listával újra létrehozhatja az előfizetéseket az új összevont bérlőben.

### <a name="api-registration"></a>API-regisztráció

További információ az API-regisztrációról: [API-hozzáférés beállítása a Partnerközpont.](/partner-center/develop/set-up-api-access-in-partner-center)

## <a name="next-steps"></a>Következő lépések

- [Felhőszolgáltató piacok és pénznemek, ahol CSP-ajánlatokat értékesíthet](regional-authorization-overview.md)
