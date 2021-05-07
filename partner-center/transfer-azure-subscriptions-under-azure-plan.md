---
title: Azure-előfizetés átvitele Azure-csomag alá egy másik CSP-partnernek
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan módosíthatja Felhőszolgáltató ügyfél Azure-előfizetéséhez társított partnert egy Azure-csomag keretében.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: f0abfdfd2fbb242f7cdbe0ded04d387ea712cce5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702722"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Ügyfél Azure-csomag előfizetésének átadása egy másik partnernek

**Megfelelő szerepkörök**

- Fiókadminisztrátor
- Értékesítési ügynök
- Számlázási ügynök

Ez a cikk azt ismerteti, hogy az ügyfelek hogyan válthatnak Azure-előfizetéseik között egy Azure-Felhőszolgáltató (CSP) egy másikra.

Ha egy ügyfél Azure-előfizetéseit egy másik partnerről is átkapcsolja, kövesse az alábbi lépéseket. A partnernek és az ügyfélnek is vannak lépései.

>[!Note]  
>Csak a Microsofttal közvetlen számlázási kapcsolatban áll partnerek férhetnek hozzá az átváltási eszközökhez. A közvetett viszonteladóknak a közvetett szolgáltatóikkal együtt kell használniuk ezt az áttérési eszközt.

Az ügyfélnek mindkét partnerrel (aktuális és jövőbeli) kapcsolatban kell lennie az eszköz használata előtt. A félreértések és adatváltozások elkerülése érdekében offline beszélgetést kell folytatni. Emellett a partnereknek és az ügyfeleknek az átállás megkezdése előtt meg kell érteniük ezeket a szempontokat és előfeltételeket:

**Fő szempontok:**

- Az Azure Reservations nem lesz áthelyezve az előfizetéssel a jövőbeli partnerhez
- Az aktuális partnerhez az Azure-szolgáltatások CSP-díjszabása nem fog áttérni  
- Az ügyfél támogatási feladatai a jövőbeli partnerhez fognak átköltözni
- A számlázás és a számlázás az átadáskor át fog költözni a jövőbeli partnerhez
- Az azure Role-Based Access Control (RBAC) nincs hatással az átvitelre
- A következő partner alapértelmezés szerint nem kap rendszergazdai jogosultságot a nevében (AOBO).
- A harmadik féltől származó Marketplace-termékek akkor lesznek áthozva, ha a termékek megfelelnek a Marketplace-jogosultságellenőrzésen.
    - Nincsenek különleges kedvezmények vagy regionális korlátozások
    - A termékek nem előfizetésen alapulnak
    - A jövőbeli partnernek együtt kell működnie a közzétevővel, hogy biztosan fel legyen sorolva a termék üzembe helyezésének engedélyezése listában
    - Ha nem teljesül az összes feltétel a Marketplace-termékek átviteléhez, az Azure-előfizetések átadása, majd a Marketplace-termékek újravásárlása az új partnerrel

**Előfeltételek:**

- Az ügyfél kapcsolatba fog lépjen a jelenlegi CSP-partnerrel az átállás szándéka alapján
- A jövőbeli CSP-partner az ügyféllel együtt gondoskodik az ügyfelek igényeinek kielégítése érdekében
- A jövőbeli CSP-partner kapcsolatot létesít az ügyféllel, és megvásárol egy Azure-tervet az átállás megkezdése előtt  
- Az ügyfélnek Microsoft Ügyfélszerződés CSP-partnerrel kell bejelentkeznie
- A későbbi CSP-partnernek alá kell írnia a Microsoft Partnerszerződés az eszköz használatára

## <a name="customer-tasks-to-be-completed"></a>Teljesítenünk kell az ügyfélfeladatokat

Azure-előfizetés Azure-csomag keretében történő átviteléhez az ügyfélnek el kell kezdenie a folyamatot az aktuális partnerével való kapcsolatfelvétellel. Össze kell gyűjteniük jelenlegi partnerük vállalatnevét és tartományát, hogy a jövőbeli partnerük a nevükben ki tudja egészlatni az átadási kérelem űrlapját.

Az ügyfélnek azonosítania kell azokat az előfizetéseket is, amelyek átadása az aktuális partnertől lehetséges. Nem módosíthatja az Office 365-, Nagyvállalati mobilitási csomag- vagy Microsoft Dynamics CRM-előfizetések partnerét.

>[!Note]  
>A jövőbeli partner felelőssége, hogy töltse ki az átadási kérelem űrlapját, amely elindítja az átadási folyamatot. A Microsoft nem avatkozhat be az ügyfél vagy az aktuális partner nevében. Az ügyfélnek szorosan együtt kell működnie a jövőbeli és a jelenlegi partnerrel, hogy zökkenőmentesen működjön az átállás.

## <a name="future-partner-tasks-to-be-completed"></a>A jövőbeli befejezendő partnerfeladatok

Az előfizetés jövőbeli partnerének ki kell kitöltötte az átadási kérelem űrlapát a Partnerközpont az előfizetés átvitelének igényléséhez:

1.  A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, aki nevében el szeretné látni az átadási kérelem űrlapját.
2.  Az Ügyfél menüben válassza az **Előfizetések lehetőséget.**
3.  Válassza az **Átadási kérelem szakaszt.**
4.  Az **Átadási kérelem szakaszban válassza** az **Új kérelem hozzáadása lehetőséget.**

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Átvitelek szakasz":::

5.  Töltse ki **az Új átadási kérelem űrlapot.**

6.  Válassza az **Átadási kérelem küldése**  >  **Küldés lehetőséget.**

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Átadási kérelem kitöltése űrlap":::

7.  Átadási kérelem megerősítésének áttekintése

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Függőben lévő átvitel áttekintése":::

    >[!Note]
    >A jövőbeli partner csak akkor  szakíthatja meg az átadási kérelmet, ha a jobb felső sarokban a Kérelem visszavonása gombra választ, ha az átadási kérelem állapota "Függőben". Ha az átadási kérelem állapota "folyamatban" vagy "kész", a megszakítások nem lesznek lehetségesek.

## <a name="current-partner-tasks-to-be-completed"></a>Jelenleg teljesítenünk kell a partneri feladatokat

Az ügyfél aktuális partnerének rendszergazdai ügynöke e-mailt fog kapni arról, hogy az ügyfél az előfizetések átvitelét kéri:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Áttekintés":::

Tekintse át és fogadja el az átadási kérelem űrlapját Partnerközpont előfizetés átvitelének befejezéséhez.

>[!Note]  
>Ha az aktuális partner 30 napon belül nem hoz létre semmilyen műveletet, a kérelem lejár, és a jövőbeli partnernek lesz egy új átadási kérése.

1.  Válassza **az Átadási kérelem áttekintése lehetőséget** az e-mailből VAGY
1.  A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válassza ki azt az ügyfelet, aki nevében elküldött egy átadási kérelmet.
2.  Az Ügyfél menüben válassza az **Előfizetések lehetőséget.**
3.  Válassza az **Átadási kérelem szakaszt.**
4.  Bontsa ki az átadási adatokat a kiválasztott **átadási kérelem azonosítójának kiválasztásával a** **Fogadott kérések alatt**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Forrás-felülvizsgálatok átadási kérése":::

5.  Tekintse át az átadási kérelmet. Válassza ki az átvitelhez kért Azure-előfizetéseket.

>[!Note]  
> Mielőtt továbblépne, vegye figyelembe, hogy a továbbiakban nem fog hozzáférni a kiválasztott előfizetéshez.
> A további használatért nem lesz számlázva.
> Az Azure-foglalások nem átvitele az előfizetésekkel együtt.

6.  Ezután válassza **az Elfogadás és átvitel lehetőséget** az átviteli folyamat befejezéséhez.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Válassza ki az Azure-csomagokban átvihető előfizetéseket":::

7.  Az átadás elfogadásának megerősítésének megtekintése.

   Ezen a ponton a jövőbeli partner, az ügyfél és az aktuális partner e-mailben értesítést kap az elfogadott átadási kérelemről.

   Az átváltás elfogadott állapota akár 15 percig is függőben maradhat a rendszer frissítése közben. Ha ez hosszabb időt vesz igénybe, a rendszer három napig próbálkozik. Ha az átvitel állapota továbbra is Függőben marad, a partnernek be kell nyújtania egy szolgáltatáskérést.

   Az átvitel befejezése után a kérésben szereplő előfizetések megjelennek a jövőbeli partner Azure-csomagja alatt, és a továbbiakban nem lesznek felsorolva.

>[!Note]  
>Közvetett szolgáltatók esetén: Tájékoztassa a közvetett viszonteladót arról, hogy az átadási kérelem el lett fogadva.

### <a name="managing-your-transferred-customer-subscriptions"></a>Az átvitt ügyfél-előfizetések kezelése

- A meglévő felhasználók, csoportok vagy szolgáltatásnevek hozzáféréseire, amelyek az Azure szerepköralapú hozzáférés-vezérlés (RBAC) segítségével lettek hozzárendelve, a váltás nincs hatással. Az Azure szerepköralapú hozzáférés-vezérlés [(Azure RBAC)](/azure/role-based-access-control/overview) segítségével az ügyfelek kezelhetik, hogy ki férhet hozzá az Azure-erőforrásokhoz, mire használhatja őket, és milyen területekhez férhetnek hozzá. Új partnerként nem kap RBAC-hozzáférést az ügyfél erőforrásaihoz az előfizetés átvitele után. Az ügyfél korábbi partnere megtartja RBAC-hozzáférését. Az ügyféllel együtt értse meg, hogy ki kaphat betekintést az előfizetéseibe, és hogyan lehet bármilyen módosítást tenni.

- Ezért fontos, hogy az ügyfél eltávolítsa az Azure RBAC-hozzáférést a korábbi partnertől, és hozzáférést adjon hozzá az új partnerhez. Az új hozzáférést adó ügyféllel kapcsolatos további információkért lásd: [Mi az az Azure szerepköralapú hozzáférés-vezérlés (Azure RBAC)?](/azure/role-based-access-control/overview) Az előző partner RBAC-hozzáférésének eltávolításával kapcsolatos további információkért [lásd: Szerepkör-hozzárendelés eltávolítása.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)

- Emellett nem kap automatikusan rendszergazdai hozzáférést az előfizetései [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) nevében. Az AOBO szükséges ahhoz, hogy a partnerek a nevükben kezelték az ügyfél Azure-előfizetését. Az Azure-jogosultságokkal kapcsolatos további információkért lásd: Ügyfél szolgáltatásának vagy előfizetésének kezeléséhez szükséges [engedélyek beszerzése.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Következő lépések:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Engedélyek beszerzése egy ügyfél szolgáltatásának vagy előfizetésének kezeléséhez.](./customers-revoke-admin-privileges.md)
