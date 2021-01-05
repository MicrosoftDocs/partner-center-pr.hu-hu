---
title: Azure-előfizetés átvitele egy Azure-csomagból egy másik CSP-partnerbe
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan változtathatja meg egy Azure-csomag keretében az ügyfél Azure-előfizetéséhez társított felhőalapú megoldás-szolgáltatói partnert.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e792e4af2999924ba8be77ec0517ce56c1db7a27
ms.sourcegitcommit: ed5c873d19f0464cc986fe6e852383cd4280daf6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/05/2021
ms.locfileid: "97893206"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Ügyfél Azure-csomag-előfizetésének átvitele egy másik partnerre

**Megfelelő szerepkörök**

- Partnerek a Cloud Solution Provider (CSP) programban

Ez a cikk azt ismerteti, hogy az ügyfél hogyan válthat az Azure-előfizetések között egy felhőalapú megoldás-szolgáltató (CSP) között egy másikra.

Az ügyfél Azure-előfizetésének egy másik partnertől való átváltásához kövesse az alábbi lépéseket. A partner és az ügyfél is elvégezheti a szükséges lépéseket.

>[!Note]  
>Csak a Microsofttal közvetlen számlázási kapcsolattal rendelkező partnerek férhetnek hozzá az áttérési eszközökhöz. A közvetett viszonteladóknak működniük kell a közvetett szolgáltatókkal az áttérési eszköz kihasználása érdekében.

Az ügyfélnek az eszköz kihasználása előtt mindkét partnerrel (aktuális és jövőbeli) kell kommunikálnia. Az offline beszélgetéseknek el kell kerülniük a félreértések és a forgalom elkerülését. Emellett a partnereknek és az ügyfeleknek meg kell érteniük ezeket a szempontokat és előfeltételeket az áttérés megkezdése előtt:

**Legfontosabb szempontok:**

- A Azure Reservations nem kerül át az előfizetésbe a jövőbeli partnernek
- A jelenlegi partnernél az Azure-szolgáltatások CSP-díjszabása nem fog áttérni  
- Az ügyfél támogatási feladatai a jövőbeli partnernek lesznek áthelyezve
- A számlázás és a számlázás a jövőbeli partnernek az átvitel időpontjában kerül át
- Az átvitel nem érinti az Azure Role-Based Access Controlt (RBAC)
- Alapértelmezés szerint a (z) (AOBO) rendszergazdai nevében nem adható meg a jövőbeli partner
- A harmadik féltől származó Piactéri termékek addig lesznek továbbítva, amíg a termékek átadják a piactér jogosultsági ellenőrzését.
    - Nincsenek különleges kedvezmények vagy regionális korlátozások
    - A termékek nem előfizetésen alapulnak
    - A jövőbeli partnernek együtt kell működnie a közzétevővel annak ellenőrzéséhez, hogy az engedélyezési listán vannak-e a termék telepítéséhez
    - Ha a piactér-termékek átadásához nem teljesülnek az összes feltétel, akkor az Azure-előfizetések át lesznek adva, majd a piactér-termékek újravásárlása az új partnerrel

**Előfeltételek:**

- Az ügyfél az aktuális CSP-partnert az áttérés céljára irányítja
- A jövőbeli CSP-partner az ügyféllel együttműködve biztosítja az ügyfelek igényeinek teljesítését
- A jövőbeli CSP-partner kapcsolatot létesít az ügyféllel, és megvásárol egy Azure-csomagot az áttérés megkezdése előtt  
- Az ügyfélnek regisztrálnia kell a Microsoft ügyfél-szerződést a jövőbeli CSP-partnerrel
- A jövőbeli CSP-partnernek alá kell írnia a Microsoft partneri szerződést az eszköz használatához

## <a name="customer-tasks-to-be-completed"></a>Elvégzendő felhasználói feladatok

Ha Azure-csomag keretében szeretne Azure-előfizetést továbbítani, az ügyfélnek a jelenlegi partnerével kell megindítania a folyamatot. Össze kell gyűjteniük az aktuális partnere vállalatának nevét és tartományát, hogy a jövőbeli partnerük az adatátviteli kérelem űrlapját a nevében tudja befejezni.

Az ügyfélnek továbbá azonosítania kell az aktuális partnertől átvinni kívánt előfizetéseket. Az Office 365, a nagyvállalati mobilitási csomag vagy a Microsoft Dynamics CRM-előfizetések partnerei nem változtathatók meg.

>[!Note]  
>A jövőbeli partner feladata az adatátviteli kérelem űrlapjának elvégzése, amely elindítja az átvitel folyamatát. A Microsoft nem tud beavatkozni az ügyfél vagy az aktuális partner nevében. Az ügyfélnek meg kell terveznie, hogy a jövőben zökkenőmentesen működjön együtt a jövőbeli és a jelenlegi partnerével.

## <a name="future-partner-tasks-to-be-completed"></a>A jövőbeli partneri feladatok elvégzése

Az előfizetés jövőbeli partnerének el kell végeznie egy átadási kérelem űrlapját a partner Centertől az előfizetés átadásának igényléséhez:

1.  A partner Center menüjében válassza az **ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, aki az átadási kérelem űrlapját a nevében szeretné végrehajtani.
2.  Az ügyfél menüben válassza az **előfizetések** lehetőséget.
3.  Válassza az **átviteli kérelem** szakaszt.
4.  Az **átadási kérelem szakaszban** válassza az **új kérelem hozzáadása** elemet.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Átvitelek szakasz":::

5.  Fejezze be az **új adatátviteli kérés** űrlapot.

6.  Válassza az **átvitel küldése kérelem**  >  **Küldés** lehetőséget.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Adatátviteli kérelem űrlapjának befejezése":::

7.  Átmozgatási kérelem megerősítése

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Ellenőrzés függőben":::

    >[!Note]
    >A jövőbeli partner megszakíthatja az adatátviteli kérést a jobb felső sarokban lévő **kérelem megszakítása** lehetőség kiválasztásával, ha az átadási kérelem állapota "függőben van". Ha az átviteli kérelem állapota "folyamatban" vagy "kész", a lemondások nem lesznek lehetségesek.

## <a name="current-partner-tasks-to-be-completed"></a>Az aktuálisan elvégzendő partneri feladatok

Az ügyfél a jelenlegi partner rendszergazdai ügynöke egy e-mailt kap arról, hogy az ügyfél az előfizetésük átvitelét kéri:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Áttekintés":::

Tekintse át és fogadja el az adatátviteli kérés űrlapot a partner Centertől az előfizetés átvitelének befejezéséhez.

>[!Note]  
>Ha a jelenlegi partner semmilyen műveletet nem végez a kérés érvényességét követő 30 napon belül, és a jövőbeli partner egy új adatátviteli kérést fog létrehozni.

1.  Válassza az **átadási kérelem megtekintése** az e-mailben vagy a
1.  A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, akinek a nevében elküldte az átadási kérelmet.
2.  Az ügyfél menüben válassza az **előfizetések** lehetőséget.
3.  Válassza az **átviteli kérelem** szakaszt.
4.  Az átadási adatok kibontása a kiválasztott **átadási kérelem azonosítójának** kiválasztásával a **fogadott kérelmek** között

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Forrás-felülvizsgálati kérelem átvitele":::

5.  Átmozgatási kérelem áttekintése. Válassza ki az átvinni kívánt Azure-előfizetéseket.

>[!Note]  
> A továbblépés előtt vegye figyelembe, hogy a továbbiakban nem fog tudni hozzáférni a kijelölt előfizetésekhez.
> A további használatra nem lesz számlázva.
> Az Azure-foglalások nem vihetők át az előfizetésekre.

6.  Ezután válassza az **elfogadás és az átvitel** lehetőséget az adatátviteli folyamat befejezéséhez.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Válassza ki az Azure-csomagok alá továbbítandó előfizetéseket":::

7.  Az átvitel elfogadási megerősítésének megtekintése.

   Ezen a ponton a jövőbeli partner, az ügyfél és a jelenlegi partner értesítést kap az elfogadott átküldési kérelemről e-mailben.

   Az áttérés elfogadását követően az átvitel állapota akár 15 percet is igénybe vehet, amíg a rendszer frissül. Ha a rendszer továbbra is tart, a rendszer három napig próbálkozik. Ha az átvitel állapota továbbra is függőben van, a partnernek be kell küldenie egy szolgáltatási kérelmet.

   Az átvitel befejezése után a kérelemben foglalt előfizetések megjelennek a jövőbeli partner Azure-tervében, és már nem jelennek meg Önnel.

>[!Note]  
>Közvetett szolgáltatók esetén: Kérjük, tájékoztassa a közvetett viszonteladót arról, hogy az átadási kérelem el lett fogadva.

### <a name="managing-your-transferred-customer-subscriptions"></a>Az átvitt ügyfél-előfizetések kezelése
- A meglévő felhasználók, csoportok vagy szolgáltatásnevek hozzáféréseire, amelyek az Azure szerepköralapú hozzáférés-vezérlés (RBAC) segítségével lettek hozzárendelve, a váltás nincs hatással. Az Azure szerepköralapú hozzáférés-vezérlés [(Azure RBAC)](/azure/role-based-access-control/overview) segítségével az ügyfelek felügyelhetik, hogy ki férhet hozzá az Azure-erőforrásokhoz, mit tehetnek ezekkel az erőforrásokkal, és milyen területekhez férnek hozzá. Az új partnerként nem kap RBAC hozzáférést az ügyfél erőforrásaihoz az előfizetés átvitele után. Az ügyfél korábbi partnere megtartja a RBAC-hozzáférését. Az ügyféllel együttműködve megismerheti, hogy kik betekintést nyújtanak az előfizetésbe, és hogyan teheti meg a kívánt módosításokat.

- Ezért fontos, hogy az ügyfél eltávolítsa az Azure RBAC-hozzáférést az előző partnerhez, és hozzá lehessen férni az új partnerhez. További információ az ügyfél új hozzáféréséről: [Mi az az Azure szerepköralapú hozzáférés-vezérlés (Azure RBAC)?](/azure/role-based-access-control/overview) További információ az előző partner RBAC-hozzáférésének eltávolításáról: [szerepkör-hozzárendelés eltávolítása](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- Emellett nem kap automatikusan rendszergazdai jogosultságot az előfizetések nevében [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) . Ahhoz, hogy a partner felügyelje ügyfele Azure-előfizetéseit az Ön nevében, az AOBO szükséges. További információ az Azure-jogosultságokról: az [ügyfél szolgáltatásának vagy előfizetésének kezeléséhez szükséges engedélyek beszerzése.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Következő lépések:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Az ügyfél szolgáltatásának vagy előfizetésének kezeléséhez szükséges engedélyek beszerzése.](./customers-revoke-admin-privileges.md)
