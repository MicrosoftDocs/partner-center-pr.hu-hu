---
title: CSP regionális engedélyezési bérlői konszolidáció
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ezekkel az utasításokkal összevonhatja a bérlőket a különböző országokban/régiókban. Ez magában foglalja a felhasználói fiókok és az ügyfél-előfizetések áttelepíthető lépéseit.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2171e2b10101e99bdd8d415a936ba98af65c2a1b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502570"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Útmutató a CSP regionális engedélyezési bérlőösszevonáshoz

**A következőre érvényes:**

- A Microsoft Cloud for US Government Partnerközpontja

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felügyeleti ügynök

\[Néhány információ az előzetesen kiadott termékhez kapcsolódik, amely jelentősen módosítható a kereskedelmi forgalomba bocsátás előtt. A Microsoft nem vállal kifejezett vagy törvényi garanciát az itt megjelenő információért.\]

A bérlőket összevonhatja a vállalata számára. Ezekkel az utasításokkal összevonhatja a bérlőket a különböző országokban/régiókban.

>[!NOTE]  
>Tisztában kell lennie az összes olyan kiosztott előfizetéssel és licenccel, amely az Ön által használt fiókban található ügyfelekre vonatkozik. Az áttelepítési folyamat részeként ugyanezeket a pontos előfizetéseket fogja újból kiépíteni az új központi CSP-fiókban. Az exportálási lista funkció segítségével létrehozhat egy listát azokról az ügyfelekről, amelyek áthelyezhetők a központi bérlőbe.  A konszolidáció befejezése után nem lehet visszaállítani az előző bérlői állapotot. Az ügyfél beavatkozására is szükség lehet.

## <a name="prepare-for-migration"></a>Előkészületek a migráláshoz

- Jelentkezzen be a **partner Centerbe**  az **átváltási** fiók használatával (amely az új fiókra fog áttérni), és tekintse át az ügyfelek számára kiosztott összes ügyfelet és szolgáltatást.

- Jelentkezzen ki ebből a fiókból.

## <a name="migrate-customer-accounts"></a>Felhasználói fiókok áttelepíthetők

1. Jelentkezzen be a **partner Centerbe**  az **áttérési** (új) fiókkal (amely az ügyfeleket áthelyezi).

2. Válassza az **Ügyfelek** lehetőséget.

3. Válassza **a viszonteladói kapcsolat kérése** lehetőséget. Az ügyfeleknek küldött alapértelmezett e-mail-üzenet jelenik meg. Ez az üzenet egy olyan URL-címet tartalmaz, amely az új partner Center-fiókban egyedi szervezeti AZONOSÍTÓval rendelkezik.

4. **Ügyfél-művelet:** Győződjön meg arról, hogy az áttelepíteni kívánt összes aktív ügyfél meglátogatja ezt az URL-címet. Az URL megnyitásakor a rendszer felszólítja az ügyfelet, hogy jelentkezzen be az Office 365 portálra. Az ügyfél ugyanazzal a szervezeti AZONOSÍTÓval jelentkezik be, amelyet az Azure-és Office 365 felügyeleti portálok elérésére használ.

5. Bejelentkezés után az **ügyfél fiókjának** globális rendszergazdája megkéri, hogy küldjön be egy szerződést, amely delegált rendszergazdai jogosultságokat biztosít az új CSP-fiókhoz. Ha elfogadják, az ügyfél kiválasztja a jelölőnégyzetet, és elfogadja a kapcsolat engedélyezését.

Az ügyfelek a partner ügyfeleinek listájában jelennek meg, miután elküldték a szerződést, egyenként.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Office 365-és nem Azure-alapú használati előfizetés áttelepítése

1. Miután az ügyfél aláírta a szerződést, újra létrehozhatja előfizetéseit a központi partner bérlője alatt.

2. A **partner Centerben** válassza az **ügyfelek** lehetőséget.

3. Nyissa meg az áttelepíteni kívánt ügyfél vállalatának nevét.

4. Válassza az **előfizetés hozzáadása** lehetőséget.

5. Adja hozzá a megfelelő előfizetéseket és a licencek számát a katalógusból. Győződjön meg arról, hogy az **áttérés** partneri fiókokból című témakörben szereplő információk szerepelnek.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="ügyfelek listája":::

6. Válassza a **Küldés lehetőséget.**

   A szolgáltatásokat mostantól a partner fiókba való **áttéréssel** biztosítjuk az ügyfélnek.

7. Ismételje meg ezeket a lépéseket az előfizetések áttelepíteni az összes további ügyfélre.

Mielőtt továbblép a következő szakaszra, gondoskodjon arról, hogy a partneri fiókokba **való áttérés** alatt meglévő összes ügyfél-előfizetés újra kiépítve legyen a partner fiókba való **áttérés** alatt.

> [!NOTE]
> A partnereknek meg kell függeszteniük **az előfizetéseket a fiókpartner** partner bérlői fiókjából a partner Centerben, hogy az előfizetések átkerülnek **a partner központ partner** bérlői fiókjába, hogy a kettős számlázás ne történjen meg. A támogatási kérelmeket a rendszer megtagadja a jóváírások miatt, mert a számlázás olyan átfedésben van, amely nem megfelelően tiltja le az előfizetések közötti **váltást** .

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Az Office 365-előfizetések letiltása a partneri fiókból való áttérés alatt

Ha letiltja a CSP-előfizetést a partneri fiókokból **való áttérés alatt,** a jövőben nem számítunk fel díjat Nem kell manuálisan letiltania az Azure-előfizetéseket, mert az Azure-előfizetések automatikusan le vannak tiltva az áttelepítési folyamat során.

1. Jelentkezzen be a **partner Centerbe** az **áttérés CSP-** fiókjából, és navigáljon az ügyfél listához.

2. Nyissa meg a letiltani kívánt előfizetésekkel rendelkező ügyfelet, majd válassza ki az első letiltani ajánlatot.

3. Állítsa az előfizetést **felfüggesztve** értékre, majd válassza a **Küldés** lehetőséget.

   >[!Note]
   >Az előfizetés felfüggesztése biztosítja a kettős számlázást.

   Az előfizetés fel van **függesztve** az előfizetések listáján.

4. Ismételje meg ezeket a lépéseket az ügyfélhez tartozó összes előfizetéshez. Ellenőrizze az összes **felfüggesztett** megjelenítést.

5. Válassza ki a következő ügyfelet a listán, és ismételje meg az összes előfizetés letiltásának folyamatát.

## <a name="migrating-azure-usage-based-subscriptions"></a>Azure-alapú használati előfizetés áttelepítése

Az Office 365 CSP-előfizetésekkel ellentétben az Azure-ban nem kell manuálisan áttelepíteni a használati alapú CSP-előfizetéseket. Microsoft Azure támogatás áttelepíti az Azure-előfizetéseket **és az összes** telepített szolgáltatást vagy erőforrást a CSP-viszonteladói fiókoktól a CSP viszonteladói fiókra **való áttéréstől** . Az áttelepítés során az ügyfél nem zavarja a szolgáltatást.

1. Győződjön meg arról, hogy az Azure-előfizetésekkel rendelkező felhasználói fiókok elfogadták az új, CSP-re **való áttéréssel** kapcsolatos szerződést.

2. Értesíteni fogja a Microsoftot arról, hogy mely ügyfél-fiókok állnak készen az áttelepítésre, és adja meg az ügyfél vállalatának nevét.

3. A Microsoft áttelepíti az Azure-beli használaton alapuló előfizetéseket, és értesíti az áttelepítés befejezésekor.

4. Győződjön meg arról, hogy az Azure-előfizetés a CSP-viszonteladói fiókra történő **áttérés** alatt most már fel van **függesztve** a partner Centerben az ügyfél-előfizetések szakaszban.

5. Győződjön meg arról, hogy az Azure **-** előfizetés a CSP-viszonteladói fiókra történő áttérés alatt most az ügyfél-előfizetések szakaszban az **aktív** a partneri központban állapotot jeleníti meg.

   >[!Note]
   > Az ügyfél-előfizetések letiltása nem módosítja az ügyfél megjelenését az ügyfelek listájában. Jelenleg nincs lehetőség az ügyfelek eltávolítására a listából. A partnereknek kerülniük kell az előfizetések hozzáadását az ügyfeleknek **a fiókból a jövőben** .

6. Ismételje meg ezeket a lépéseket az összes ügyfél összes előfizetése számára, hogy leállítsa a jövőbeli díjakat a fiók (ok) **ról való áttéréskor** . A partner a lemondás napja és a számlázási időszak utolsó napján a használaton kívüli napok száma után egy végső számlát kap. A végső számlázási időszak után nem fog létrejönni jövőbeli számla.

### <a name="additional-information"></a>További információ

- Ha letiltotta az előfizetést a CSP-fiókból **való áttérésből** , az előfizetés letiltását megelőzően nem **befolyásolja a végfelhasználó** szolgáltatását.

- Az ügyfelek nem használhatják az előfizetéseket, és nem hozhatnak fel díjat a felfüggesztés vagy a visszavonás után.

- Jelenleg nem lehet teljesen eltávolítani az ügyfelet az **ügyfelek** listájáról.
- 
    >[!Note]
    > A partnereknek meg kell függeszteniük az előfizetéseket a fiókpartner partner bérlői fiókjából való **áttéréskor** , az előfizetések pedig a fiókhoz való áttérés alatt **, a kettős** számlázás biztosításához pedig az áttelepítés alatt állnak. A Microsoft nem támogatja a kreditek iránti kérelmeket, mert a számlázás olyan átfedésben van, amely nem megfelelően van beállítva az előfizetések felfüggesztésére való **áttéréskor** .

### <a name="simplify-migration-using-export"></a>Az áttelepítés egyszerűbbé tétele az exportálással

Az **Exportálás funkcióval** rögzítheti az új összevont struktúrában használni kívánt előfizetéseket:

1. Válassza ki az **ügyfeleket** a partner központban az ügyfelek listájának megtekintéséhez. 

2. Nyissa meg a kívánt ügyfél nevét.

3. Az **előfizetések** lapon válassza az előfizetések **exportálása** lehetőséget, hogy egy Excel-fájlba exportálja az előfizetések részleteit.

4. Ezzel a listával újból létrehozhatja az előfizetéseket az új konszolidált bérlőben.

### <a name="api-registration"></a>API-regisztráció

Az API-regisztrációval kapcsolatos további információkért lásd: [API-hozzáférés beállítása a partner Centerben](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Következő lépések

- [A Cloud Solution Provider program regionális piacai és pénznemei, amelyekben a CSP-ajánlatok értékesíthetők](regional-authorization-overview.md)
