---
title: Azure-előfizetés átvitele másik partnernek
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan módosíthatja az ügyfél Azure-előfizetéséhez társított felhőalapú megoldás-szolgáltatói partnert.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 20e00034e9c20a5d41500892df059b34a9347a63
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028298"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Megtudhatja, hogyan adhatja át egy ügyfél Azure-előfizetéseit egy másik partnernek

**A következőre érvényes:**

- Partneri központ a Microsoft Government cloudhoz
- A Microsoft globális felhőhöz tartozó partneri központ

Ez a cikk azt ismerteti, hogy az ügyfelek hogyan válthatják át a Microsoft Azure szolgáltatásaikat egy felhőalapú megoldás-szolgáltatóról (CSP) egy másikra.

Ha az ügyfél Azure-szolgáltatásait vagy előfizetéseit egy másik partnerre szeretné váltani, kövesse az alábbi utasításokat. A partnernek és az ügyfélnek is végre kell hajtania a lépéseket.

>[!Note]  
>Jelenleg csak a közvetlen vagy a közvetett szolgáltatók vihetnek át előfizetéseket.
>Az Azure-csomaggal, az Office 365-mel, a nagyvállalati mobilitási csomaggal vagy a Microsoft Dynamics CRM-előfizetésekkel társított felhőalapú megoldás-szolgáltatói előfizetések partnerei

## <a name="switch-partners-for-azure-subscriptions"></a>Partnerek váltása az Azure-előfizetésekhez

1. Ha egy Azure-előfizetést új partnernek szeretne továbbítani, az ügyfélnek el kell indítania a folyamatot, és írásban kell megadnia a rekord aktuális partnerét.

   >[!Note]
   > Az aktuális partner felelőssége, hogy létrehozza az adatátviteli folyamatot kezdeményező szolgáltatási jegyet. A Microsoft nem tud beavatkozni az ügyfél vagy az új partner nevében. Az ügyfélnek meg kell terveznie, hogy szorosan működjön együtt az aktuális partnerrel, hogy az átmenet zökkenőmentes legyen.

2. Az előfizetéshez tartozó partnernek a következő feladatokat kell elvégeznie:

   Hozzon létre egy Azure-szolgáltatási jegyet a partner Centertől az előfizetés-átvitel igényléséhez:

   1. A partner Center menüben válassza az **ügyfelek** lehetőséget, válassza ki az ügyfelet a listából, majd válassza a **Service Management** lehetőséget.

   2. A **támogatási jegyek** szakaszban válassza ki az **új jegy** legördülő menüt, és válassza a **Microsoft Azure** lehetőséget.
   
   3. A [Azure Portal](https://portal.azure.com)válassza az **új támogatási kérelem** lehetőséget.
   
   4. Az 1. lépésben válassza az **előfizetés-kezelés** lehetőséget a probléma típusa mezőben, adja meg az átvinni kívánt előfizetés-azonosítót, és válassza a **Cloud Solution Provider** lehetőséget támogatási csomagként.
   
   5. A 2. lépésben válassza a **C-minimal Impact** lehetőséget, majd a probléma típusaként válassza ki a **többi általános kérdést** .
   
   6. Töltse le a [CSP-előfizetés átvitele űrlapot](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC).

3. Az előfizetés partnere: töltse ki a [CSP-előfizetés továbbítása űrlapot](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC), írja alá, majd küldje el az ügyfélnek. 

   Az űrlap kitöltéséhez a következő információkra lesz szüksége:

   - Az aktuális partner kapcsolattartási adatai és a Microsoft azonosítója. A partner Center menüben válassza a **Fiókbeállítások** &gt; **szervezeti profil** lehetőséget, és használja az ott **felsorolt Microsoft-azonosító**, **szervezet neve** és **címe** elemet.

   - Az ügyfél Microsoft-azonosítója. A partner Center menüben válassza az **ügyfelek** lehetőséget, majd bontsa ki az ügyfél listáját, hogy megtekintse a **Microsoft-azonosítót**.

   - Az átvinni kívánt előfizetés-azonosító. A kibontott ügyfelek listájában válassza az **előfizetések megtekintése** lehetőséget, majd a kiválasztott előfizetés kibontásával tekintse meg az **előfizetés azonosítóját**.

   >[!Note]
   >Az előfizetések továbbítása két előfizetés-azonosítóval történik, amelyet az átvitt előfizetés **előfizetés szerkesztése** lapján láthat: **1**– a partner Center előfizetés-azonosítója a számlázási célokra szolgál. **2**– az eredeti Azure-ELŐfizetési azonosítót megőrzi a rendszer, és megjelenik a partner Centerben és az Azure felügyeleti portálján is. Ez az azonosító megjelenik a Recon-fájlban.  **A támogatási jegyek naplózásakor mindkét azonosítót kell használnia.**

4. Az előfizetéshez tartozó ügyfél és új partner:

   Tekintse át az űrlapot, adja meg az új partner adatait, és jelentkezzen be. Győződjön meg arról, hogy az új ügyfél szerződést kötött. Küldje vissza az űrlapot a rekord aktuális partnerének.

   *Fontos*: Ha az új CSP-partner nem rendelkezik viszonteladói kapcsolattal az ügyféllel, az előfizetés átadása előtt létre kell hoznia egyet. [Itt megtudhatja, hogyan teheti ezt meg](request-a-relationship-with-a-customer.md).

   >[!Note]
   >Az új CSP-partnernek és az ügyfél bérlőnek ugyanabban az országban kell lennie. 

5. Aktuális partner:

   Győződjön meg arról, hogy az űrlap tartalmazza a partner-rendszergazdák kapcsolattartási adatait is. Microsoft ügyfélszolgálata felveszi Önnel a kapcsolatot a rendszergazdákkal az átvitel ellenőrzéséhez. Győződjön meg arról, hogy mindhárom aláírása megtörtént. Ezután a **fájlfeltöltés** lehetőséggel csatolja a kész űrlapot a meglévő szolgáltatási kérelemhez. A Microsoft támogatási szakembere nyolc munkanapon belül vissza fog térni a kézhezvétel és a Befejezés ellenőrzéséhez.

6. Új partner:

   Frissítse az Azure-előfizetési beállításokat, hogy eltávolítsa a régi partnert a fiókból. Ha szeretné megtekinteni, hogy mely szerepkör-hozzárendelések vannak kiépítve, futtasson két PowerShell-parancsmagok.

   - Adja hozzá az új partnert viszonteladóként a fiókhoz:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > Az ügyfél **bérlői azonosítója** a partner Centerben jelenik meg az ügyfél **Microsoft-azonosítójaként**. Egy adott ügyfél Microsoft-AZONOSÍTÓjának (bérlői AZONOSÍTÓjának) megkereséséhez jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard). Ezután válassza az **ügyfelek** lehetőséget a menüből. Keresse meg az ügyfelet a listán. Válassza ki a lefelé mutató nyilat az ügyfél listájának kibontásához. Az ügyfél *tartománynevét* és az ügyfél **Microsoft-azonosítóját** fogja látni. Használja a 16 számjegyű **Microsoft-azonosítót** a PowerShell-parancsmagot.

   - A fiók szerepköreinek megtekintése, beleértve a korábbi CSP-partnereket:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Elavult hozzáférési engedélyek eltávolítása:

   - A partner Center menüben válassza az **ügyfelek** lehetőséget.
   - Keresse meg az ügyfelet a listán. Válassza ki (kattintson duplán) a vállalata nevére. Ez a művelet megnyitja az ügyfél- **előfizetések** lapot.
   - Az ügyfél részletei menüben válassza a **Service Management** lehetőséget.
   - A **Microsoft Azure** alatt válassza ki a hivatkozást, és nyissa meg a **a Microsoft Azure felügyeleti portálja**.

## <a name="next-steps"></a>Következő lépések

- Töltse le a [CSP-előfizetés átvitele űrlapot](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

- További információ a [többpartneres támogatásról](multipartner.md).

- [több partner támogatása](multipartner.md).
- [többcsatornás támogatás](multichannel.md).
- [Azure-előfizetések átvitele](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)