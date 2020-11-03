---
title: Partner által létrehozott kredit a felügyelt szolgáltatásokhoz
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan számítják ki és fizetik ki a Microsoft partner által létrehozott kreditet (PEC) a felügyelt szolgáltatásokhoz, és hogy miként biztosítható a jogosultsága.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 89fce612d5756da3f9674d4170ac8c0c3a48abfe
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530588"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>A partner által szerzett kredit kiszámítása és kifizetése

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói rendszergazda
- Felügyeleti ügynök
- Számlázási adminisztrátor
- Értékesítési ügynök

A felügyelt szolgáltatások (PEC) partner által létrehozott kreditje felismeri és jutalmazza a partnereket, akik a saját nonstop, illetve az ügyfelek teljes, Azure-környezetének felügyeletét és felügyeletét végzik. A CSP-ben alapértelmezés szerint a partnerek megkapják a szükséges hozzáférési jogosultságokat az ügyfél előfizetéséhez, amely lehetővé teszi, hogy az előfizetéshez tartozó erőforrások 24 X 7 működési felügyeletét és felügyeletét végezzék el. A következő szakasz ismerteti az ügyfelek által a transacting partnerhez való hozzáférés kiépítésének további módjait. A havi számla összege a partneri jóváírás levonása utána érték. A partnerek megtekinthetik a PEC részleteit a havi Recon-fájlon. Az [Azure-csomag előfizetések és erőforrások kezelése](azure-plan-manage.md)című cikkből megtudhatja, hogy az ügyfél hogyan építhet ki hozzáférést a transacting partnerhez.

Olvassa el [a rendszergazdai jogosultságok visszaállítása az Azure CSP-előfizetésekhez](revoke-reinstate-csp.md) lehetőséget is.

## <a name="important-eligibility-and-calculation-information"></a>Fontos jogosultsági és számítási információk

- A partnernek aktív MPN-szerződéssel és érvényes RBAC-szerepkörrel kell rendelkeznie ahhoz, hogy megkapja a kezelt Azure-eszközökhöz kapcsolódó kreditet. 

- Közvetett szolgáltatók és közvetett viszonteladóik esetén a közvetett szolgáltató jogosult lesz a PEC-re, ha a közvetett szolgáltató vagy a közvetett viszonteladó vagy mindkettő nonstop az ügyfél Azure-erőforrásainak működési vezérlését és felügyeletét a CSP-ben.

- A PEC a partner által felügyelt, az ügyfél Azure-hagyatékának számlázott (díjköteles) felhasználására van társítva. A PEC csak a Microsoft által számlázott (közvetett szolgáltatói és közvetlen számlázási partneri) partnerek számára érhető el. 

- Jogosult szolgáltatások: a partner által létrehozott kredit az Azure-csomag használati **díjszabásában** felsorolt szolgáltatásokra vonatkozik, amelyeket a partnerek az [Azure-csomag díjszabási](https://partner.microsoft.com/commerce/sales) oldaláról exportálhatunk. A partner által létrehozott kreditek nem alkalmazhatók harmadik féltől származó termékekre az **Azure-csomag** fogyasztási árlista, az Azure Plan Reservations, a Piactéri árlista és az [Azure spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/) **címkék oszlopában** .

- A PEC napi rendszerességgel van kiszámítva, és a napi használati fájlban és a havi számlaengedmény-fájlban is megtekinthető. Egy partnernek (közvetett szolgáltató vagy közvetett viszonteladó) hozzáféréssel kell rendelkeznie a teljes naphoz (nonstop) annak biztosításához, hogy a PEC-t keresnek. A PEC kiszámítása napi rendszerességgel történik a felügyelt Azure-eszközökön. Egy adott számlázási időszak (hónap) maximális PEC-értéke 15%. Az állandó jogosultsági szintű hozzáférést a hónapban (a hozzáférés hatóköre) és az összes jogosult erőforráshoz (a hozzáférés hatóköre) megőrzött partnereknek a teljes PEC-t 15%-kal kell megszerezniük. A hatókör-és a sávszélesség-csökkentés az adott hónapban alacsonyabb PEC-arányt eredményez. A napi névleges használati fájl napi rendszerességgel jelenik meg egy Azure-eszközön, függetlenül attól, hogy a PEC van-e alkalmazva. A partnerek riasztásokat is regisztrálhatnak annak észlelésére, hogy vannak-e állandó jogosultságokkal rendelkező hozzáférések.

- A PEC-t az Azure-erőforrás szintjén szerezték le. Ha a partner érvényes hozzáféréssel rendelkezik az előfizetéshez vagy az erőforráscsoport szintjéhez, akkor minden olyan erőforrás, amely a magasabb entitásnak felel meg, a PEC-t fogja keresni.  

- A PEC részletei az [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) szolgáltatásban is elérhetők lesznek

## <a name="azure-cost-management"></a>Azure Cost Management

A Cost Analysis Azure Cost Management (ACM) lehetővé teszi, hogy partnereként megtekintse a PEC előnyeit megillető költségeket.  

1. A [Azure Portal](https://portal.azure.com)jelentkezzen be a partner bérlőbe, és válassza a **Cost Management + számlázás** lehetőséget.

2. **Cost Management** kiválasztása

3. **Cost Analysis** kiválasztása

   A Cost Analysis View (költség elemzése) nézetben megjelennek a Számlázási fiók költségei, a Microsoft által megvásárolt és felhasznált összes szolgáltatás esetében.

4. Válassza a **PartnerEarnedCreditApplied** lehetőséget a kimutatás legördülő listájában a PEC-t alkalmazó költségek megtekintéséhez. Ha a **PartnerEarnedCreditApplied** tulajdonság értéke TRUE (igaz), a kapcsolódó díj a partner által létrehozott kredit előnye. 

Ha a PartnerEarnedCreditApplied tulajdonság értéke false (hamis), akkor a kapcsolódó költség nem teljesült a kredithez szükséges jogosultsággal, vagy a megvásárolt szolgáltatás nem jogosult a partner által szerzett kreditre.

>[!NOTE] 
>A szolgáltatások használata általában 8-24 órát vesz igénybe **Cost Managementban** , és a PEC-kreditek 48 órán belül megjelennek a Azure Cost Managementban való hozzáférés időpontjában.

5. A Group By, a Group By, a **PartnerEarnedCreditApplied** tulajdonság és a szűrési funkció alapján is szűrheti **a szűrési** funkciókat a PEC-t használó költségek és a PEC-t nem alkalmazó költségek részletezése céljából.

## <a name="next-steps"></a>Következő lépések

- [Partner által létrehozott kredit – áttekintés](partner-earned-credit.md)

- A partneri kreditek kiszámítására vonatkozó részletes példákat az árlista tartalmazza, amely a partner Center irányítópultján érhető el (bejelentkezés szükséges).

- [Áttérés az Azure planre – első lépések](azure-plan-get-started.md)

- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)

- [Rendszergazdai jogosultságok visszavonása vagy újraindítása az Azure CSP-előfizetésekhez](revoke-reinstate-csp.md)
