---
title: Partneri jóváírás felügyelt szolgáltatásokhoz
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan számítja ki és fizeti ki a microsoftos partneri jóváírást (PEC) a felügyelt szolgáltatásokhoz, és hogyan biztosíthatja a jogosultságot.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ba422a2feae2affb9c2b60ad345c4d6bb0d525c7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145864"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>A partneri jóváírás kiszámításának és kifizetésének részletei

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Rendszergazdai ügynök | Számlázási rendszergazdai | Értékesítési ügynök

A felügyelt szolgáltatások (PEC) partneri jóváírásai felismerik és megjutalmazzák az ügyfeleik részeinek vagy teljes Azure-környezetének 24 órás operatív vezérlését és felügyeletét. Alapértelmezés szerint a CSP-ben a partnerek a szükséges hozzáférési jogosultságokat kapják meg az ügyfél előfizetéséhez, így az előfizetés erőforrásainak 24 x 7-es működési felügyeletét és felügyeletét végezhetik el. A következő szakaszban ismertetjük, hogy az ügyfelek hogyan férhetnek hozzá a tranzakciós partnerekhez. A havi számla összege a partneri jóváírás nettó összege. A partnerek a havi felderítési fájljukban láthatják a PEC részleteit. Az ügyfelek számára a tranzakciós partner hozzáférésének további módjaiért olvassa el az Előfizetések és erőforrások kezelése az [Azure-csomag alatt cikkeket.](azure-plan-manage.md)

Olvassa el [a rendszergazdai jogosultságok visszaállítását Azure CSP előfizetések esetén című témakört is.](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Jogosultság

A partneri jóváírás (PEC) fogadására az alábbi követelmények vonatkoznak: 

- Aktív MPN-szerződéssel és érvényes szerepköralapú hozzáférés-vezérlési (RBAC) szerepkörsel kell rendelkezik ahhoz, hogy megkapja a felügyelet alatt álló Azure-eszközökért kapott jóváírást.

- Az ügyfél Azure-erőforrásainak 24 órás operatív vezérléssel és felügyeletével kell lennie a CSP-ben. Ez azt jelenti, hogy rendszergazdai jogosultságokkal kell rendelkezik az ügyfél Azure-előfizetésében, Azure-erőforráscsoportja vagy Azure-erőforrásában. Közvetett szolgáltatók és közvetett viszonteladóik esetében a közvetett szolgáltató jogosult lesz a PEC-re, ha vagy a közvetett szolgáltató, vagy a közvetett viszonteladó, vagy mindkettő felett ez a működési ellenőrzés áll. További információért lásd: Rendszergazdai jogosultságok újbóli [Azure CSP előfizetések esetén.](./revoke-reinstate-csp.md)

- A fenti követelmények mellett a PEC csak az Azure-csomag használatának díjszabásában felsorolt szolgáltatásokra vonatkozik, amelyeket az Azure-csomag díjszabási [oldalán exportálhat.](https://partner.microsoft.com/commerce/sales)

- A PEC **nem vonatkozik** a következő szolgáltatásokra:
    - Azure-csomag foglalása
    - Harmadik félként azonosított külső termékek az Azure-csomag fogyasztási árának Címkék oszlopában
    - A Marketplace árlistán található termékek
    - [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- A PEC az Azure-erőforrás szintjére van lekért érték. Ha érvényes hozzáféréssel rendelkezik az előfizetés vagy az erőforráscsoport szintjén, a magasabb entitást összeső összes erőforrás PEC-t kap.

- A PEC részletei az [Azure Cost Management oldalán is elérhetők.](/azure/cost-management-billing/costs/get-started-partners)

### <a name="calculation"></a>Számítás

A PEC számítása naponta történik, és megtekinthető a napi használati adatok fájljában és a havi számla recon fájljában. A partnernek (közvetett szolgáltatónak vagy közvetett viszonteladónak) a teljes napra (24 órás) hozzáféréssel kell lennie, hogy biztosítsa a PEC-t. A PEC kiszámítása naponta történik a felügyelt Azure-eszközök alapján. Az állandó emelt szintű hozzáférést a hónap (a hozzáférés hatóköre) és az összes jogosult erőforrás (hozzáférési hatókör) megtartásával fenntartó partnerek teljes PEC-t fognak kihozni. A hatókör és a hatókör csökkentése alacsonyabb PEC-arányt eredményez a hónapra. A napi minősítésű használati fájl naponta jelenik meg egy Azure-eszközben, akár alkalmazva van a PEC, akár nem. A partnerek az állandó emelt szintű hozzáférés változásainak figyelése érdekében is regisztrálhatnak a riasztásokbe.

## <a name="azure-cost-management"></a>Azure Cost Management

Azure Cost Management (ACM) használatával lehetővé teszi, hogy partnerként megtekintse a PEC által kapott költségeket.  

1. A [Azure Portal](https://portal.azure.com)jelentkezzen be a partnerbérlőbe, és válassza a **Cost Management + Billing.**

2. A **Cost Management kiválasztása**

3. Válassza a **Költségelemzés lehetőséget**

   A Költségelemzés nézet megjeleníti a számlázási fiók költségeit az összes megvásárolt és felhasznált szolgáltatáshoz a Microsoft által fizetett árakon.

4. A kimutatás legördülő listájában válassza a **PartnerEarnedCreditApplied** lehetőséget a PEC alkalmazásával kapcsolatos költségek listájának kiválasztásához. Ha **a PartnerEarnedCreditApplied** tulajdonság True (Igaz) érték, a kapcsolódó költséghez a partneri jóváírás jár. 

   Ha a PartnerEarnedCreditApplied tulajdonság hamis, a kapcsolódó költség nem érte el a jóváíráshoz szükséges jogosultságot, vagy a megvásárolt szolgáltatás nem jogosult a partneri jóváírásra.

   >[!NOTE] 
   >A szolgáltatások használata általában 8–24 órát  vesz igénybe az Cost Management-ben, a PEC-kreditek pedig a Azure Cost Management.

5. A **PartnerEarnedCreditApplied** tulajdonság alapján is csoportosíthat és szűrhet a **Group by** és az Add filter features (Szűrési funkciók hozzáadása) használatával a PEC-t és a PEC-t nem alkalmazott költségek részletezéséhez.

## <a name="next-steps"></a>Következő lépések

- [Partneri jóváírás – áttekintés](partner-earned-credit.md)

- A partneri jóváírások számításának részletes példái az árlistán találhatók, amely az irányítópulton Partnerközpont (bejelentkezés szükséges).

- [Áthelyezés Azure-csomagba – első lépések](azure-plan-get-started.md)

- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)

- [Rendszergazdai jogosultságok visszavonása vagy Azure CSP visszavonása](revoke-reinstate-csp.md)
