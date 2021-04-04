---
title: Partner által létrehozott kredit a felügyelt szolgáltatásokhoz
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan számítják ki és fizetik ki a Microsoft partner által létrehozott kreditet (PEC) a felügyelt szolgáltatásokhoz, és hogy miként biztosítható a jogosultsága.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 022e7aabd0d850660f8236dce9a4fab9069af01b
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087127"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>A partneri jóváírás kiszámításának és kifizetésének részletei

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói felügyeleti rendszergazda
- Felügyeleti ügynök
- Számlázási adminisztrátor
- Értékesítési ügynök

A felügyelt szolgáltatások (PEC) partner által létrehozott kreditje felismeri és jutalmazza a partnereket, akik a saját nonstop, illetve az ügyfelek teljes, Azure-környezetének felügyeletét és felügyeletét végzik. A CSP-ben alapértelmezés szerint a partnerek megkapják a szükséges hozzáférési jogosultságokat az ügyfél előfizetéséhez, amely lehetővé teszi, hogy az előfizetéshez tartozó erőforrások 24 X 7 működési felügyeletét és felügyeletét végezzék el. A következő szakasz ismerteti, hogy az ügyfelek hogyan építhetnek ki hozzáférést a Transact partnerekhez. A havi számla összege a partner által felkeresett kreditek nettó mennyisége. A partnerek megtekinthetik a PEC részleteit a havi Recon-fájlon. Az [Azure-csomag előfizetések és erőforrások kezelése](azure-plan-manage.md)című cikkből megtudhatja, hogy az ügyfél hogyan építhet ki hozzáférést a transacting partnerhez.

Olvassa el [a rendszergazdai jogosultságok visszaállítása az Azure CSP-előfizetésekhez](revoke-reinstate-csp.md) lehetőséget is.

## <a name="eligibility"></a>Támogathatósági

A partner által létrehozott kredit (PEC) megszerzéséhez a következő követelmények érvényesek: 

- Rendelkeznie kell egy aktív MPN-szerződéssel és egy érvényes szerepköralapú hozzáférés-vezérlési (RBAC) szerepkörrel, amely az Ön által kezelt Azure-eszközök számára szerzett kreditet kap.

- Az ügyfél Azure-erőforrásainak nonstop operatív vezérléssel és felügyelettel kell rendelkeznie a CSP-ben. Ez azt jelenti, hogy rendszergazdai jogosultságokkal kell rendelkeznie az ügyfél Azure-előfizetéséhez, az Azure-erőforráscsoport, az Azure-erőforráshoz. Közvetett szolgáltatók és a közvetett viszonteladóik esetében a közvetett szolgáltató jogosult lesz a PEC-re, ha a közvetett szolgáltató vagy a közvetett viszonteladó vagy mindkettő rendelkezik ezzel az operatív ellenőrzéssel. További információ: [rendszergazdai jogosultságok visszaállítása az Azure CSP-előfizetésekhez](./revoke-reinstate-csp.md).

- A fenti követelményeken felül a PEC csak az Azure-csomag fogyasztási díjszabásában felsorolt szolgáltatásokra vonatkozik, amelyeket az [Azure-csomag díjszabási](https://partner.microsoft.com/commerce/sales) lapjáról exportálhat.

- A PEC **nem** alkalmazható a következő szolgáltatásokra:
    - Azure-csomag – foglalások
    - Harmadik féltől származó termékek, amelyek az Azure-csomag használati árát a címkék oszlopban vannak azonosítva
    - A piactér árlista termékei
    - [Azure spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- A PEC-t az Azure-erőforrás szintjén szerezték le. Ha az előfizetés vagy az erőforráscsoport szintjén érvényes hozzáférése van, akkor minden olyan erőforrás, amely a magasabb entitást összesíti, a PEC-t fogja keresni.

- A PEC részletei az [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) oldalán is elérhetők.

### <a name="calculation"></a>Számítás

A PEC napi rendszerességgel van kiszámítva, és a napi használati fájlban és a havi számlaengedmény-fájlban is megtekinthető. Egy partnernek (közvetett szolgáltató vagy közvetett viszonteladó) hozzáféréssel kell rendelkeznie a teljes naphoz (nonstop) annak biztosításához, hogy a PEC-t keresnek. A PEC kiszámítása napi rendszerességgel történik a felügyelt Azure-eszközökön. Az állandó jogosultsági szintű hozzáférés a hónapban (a hozzáférés hatóköre) és az összes jogosult erőforrás (a hozzáférés hatóköre) megőrzi a teljes PEC-t. A hatókör-és a sávszélesség-csökkentés az adott hónapban alacsonyabb PEC-arányt eredményez. A napi névleges használati fájl napi rendszerességgel jelenik meg egy Azure-eszközön, függetlenül attól, hogy a PEC van-e alkalmazva. A partnerek riasztásokat is regisztrálhatnak az állandó jogosultsági szintű hozzáférés változásainak figyelésére.

## <a name="azure-cost-management"></a>Azure Cost Management

A Cost Analysis Azure Cost Management (ACM) lehetővé teszi, hogy partnereként megtekintse a PEC előnyeit megillető költségeket.  

1. A [Azure Portal](https://portal.azure.com)jelentkezzen be a partner bérlőbe, és válassza a **Cost Management + számlázás** lehetőséget.

2. **Cost Management** kiválasztása

3. **Cost Analysis** kiválasztása

   A Cost Analysis View (költség elemzése) nézetben megjelennek a Számlázási fiók költségei, a Microsoft által megvásárolt és felhasznált összes szolgáltatás esetében.

4. Válassza a **PartnerEarnedCreditApplied** lehetőséget a kimutatás legördülő listájában a PEC által alkalmazott költségek megtekintéséhez. Ha a **PartnerEarnedCreditApplied** tulajdonság értéke TRUE (igaz), a kapcsolódó díj a partner által létrehozott kredit előnye. 

   Ha a PartnerEarnedCreditApplied tulajdonság értéke false (hamis), akkor a kapcsolódó költség nem teljesült a kredithez szükséges jogosultsággal, vagy a megvásárolt szolgáltatás nem jogosult a partner által szerzett kreditre.

   >[!NOTE] 
   >A szolgáltatások használata általában 8-24 órát vesz igénybe **Cost Managementban** , és a PEC-kreditek 48 órán belül megjelennek a Azure Cost Managementban való hozzáférés időpontjában.

5. A Group By, a Group By, a **PartnerEarnedCreditApplied** tulajdonság és a szűrési funkció alapján is szűrheti **a szűrési** funkciókat a PEC-t használó költségek és a PEC-t nem alkalmazó költségek részletezése céljából.

## <a name="next-steps"></a>Következő lépések

- [Partner által létrehozott kredit – áttekintés](partner-earned-credit.md)

- A partner által létrehozott kreditek számításának részletes példái a partner Center irányítópultján elérhető árlista alapján érhetők el (bejelentkezés szükséges).

- [Áttérés az Azure planre – első lépések](azure-plan-get-started.md)

- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)

- [Rendszergazdai jogosultságok visszavonása vagy visszaállítása az Azure CSP-előfizetésekhez](revoke-reinstate-csp.md)
