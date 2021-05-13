---
title: Azure-előfizetés átvitele másik partnernek
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan módosíthatja Felhőszolgáltató ügyfél Azure-előfizetéséhez társított partnerprogram-partnert.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 94f79762e7fabb377b8d7b559ff9ba2623b135fe
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856066"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Megtudhatja, hogyan adhatja át egy ügyfél Azure-előfizetéseit egy másik partnernek

**A következőkre vonatkozik:** Partnerközpont | Partnerközpont a Microsoft Cloud for US Government

**Megfelelő szerepkörök:** Globális rendszergazda

Ez a cikk azt ismerteti, hogy az ügyfelek hogyan válthatnak Microsoft Azure szolgáltatásaik között az Felhőszolgáltató (CSP) között.

Ha egy ügyfél Azure-szolgáltatásait vagy -előfizetéseit egy másik partnerre cseréli, kövesse az alábbi manuális lépéseket. A lépéseket a partnernek és az ügyfélnek is el kell látnia.

>[!Note]  
>Jelenleg csak közvetlen vagy közvetett szolgáltatók továbbíthatók előfizetéseket.
>Az Azure-csomaghoz Felhőszolgáltató Office 365-höz, Nagyvállalati mobilitási csomaghoz vagy Microsoft Dynamics CRM-előfizetésekhez társított előfizetések partnerét nem módosíthatja.

## <a name="switch-partners-for-azure-subscriptions"></a>Partnerek váltása Azure-előfizetések esetén

1. Az Azure-előfizetés új partnernek való átadásához az ügyfélnek el kell kezdenie a folyamatot, és írásban kapcsolatba kell lépnie jelenlegi partnerével.

   >[!Note]
   > Az aktuális partner felelőssége, hogy létrehozza az átadási folyamatot elindítani szükséges szolgáltatásjegyet. A Microsoft nem avatkozhat be az ügyfél vagy az új partner nevében. Az ügyfélnek szorosan együtt kell működnie az aktuális partnerrel, hogy zökkenőmentesen működjön az átállás.

2. Az előfizetés partnerének a következő feladatokat kell elvégeznie:

   Hozzon létre egy Azure-szolgáltatásjegyet Partnerközpont előfizetés átvitelének igényléséhez:

   1. A Partnerközpont válassza az **Ügyfelek** lehetőséget, válassza ki az ügyfelet a listából, majd válassza a **Szolgáltatáskezelés lehetőséget.**

   2. A Támogatási **jegyek szakaszban** válassza az Új **jegy** legördülő menüt, majd a **Microsoft Azure.**
   
   3. A [Azure Portal](https://portal.azure.com)válassza az **Új támogatási kérelem lehetőséget.**
   
   4. Az 1.  lépésben válassza az Előfizetés-kezelés problématípust, adja meg az átvitni kívánt előfizetés-azonosítót, és válassza Felhőszolgáltató **előfizetést** támogatási csomagként.
   
   5. A 2. lépésben válassza a **C–Minimális hatás lehetőséget,** és válassza az **Egyéb általános kérdések** lehetőséget a probléma típusaként.
   
   6. Töltse le a [CSP-előfizetés átvitele űrlapot.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)

3. Az előfizetés partnere: Töltse ki a [CSP-előfizetés](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)átviteli űrlapját, írja alá, majd küldje el az ügyfélnek. 

   Az űrlap kitöltéshez a következő információkra lesz szüksége:

   - Az aktuális partner kapcsolattartási adatai és Microsoft-azonosítója. A Partnerközpont válassza a Fiókbeállítások  Szervezeti profil lehetőséget, és használja az itt felsorolt &gt;  **Microsoft-azonosítót,** Szervezetnevet és **Címet.** 

   - Az ügyfél Microsoft-azonosítója. A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd bontsa ki az ügyfél termékoldalát a **Microsoft-azonosítójukhoz.**

   - Az átvitelhez szükséges előfizetés-azonosító. A bővített ügyféllistában válassza az Előfizetések megtekintése lehetőséget, majd **bontsa** ki a kiválasztott előfizetést az előfizetés **azonosítójának megtekintéséhez.**

   >[!Note]
   >Az előfizetés átvitele két előfizetés-azonosítót ad vissza, amelyek az átvitt előfizetés Előfizetés szerkesztése lapján fognak látni: **1**– Az Partnerközpont-előfizetés azonosítóját számlázási célokra használjuk.  **2**– A rendszer megőrzi az eredeti Azure-előfizetés azonosítóját, és Partnerközpont az Azure felügyeleti portálján is. Ez az azonosító megjelenik a recon fájlban.  **Támogatási jegyek naplózásakor mindkét bérletet használnia kell.**

4. Az előfizetéshez az ügyfél és az új partner:

   Tekintse át az űrlapot, adja meg az új partner adatait, és írja alá. Ellenőrizze, hogy az új ügyfél rendelkezik-e szerződéssel. Küldje vissza az űrlapot az aktuális rekordpartnernek.

   *Fontos:* Ha az új CSP-partner nem rendelkezik viszonteladói kapcsolattal az ügyféllel, az előfizetés átadása előtt létre kell hoznia egyet. [Ennek mikéntjről itt talál információt:](request-a-relationship-with-a-customer.md).

   >[!Note]
   >Az új CSP-partnernek és az ügyfélbérlőnek ugyanabban az országban kell lennie. 

5. Aktuális partner:

   Győződjön meg arról, hogy az űrlap mindkét partner-rendszergazda kapcsolattartási adatait tartalmazza. Microsoft ügyfélszolgálata mindkét rendszergazdával kapcsolatba lép az átvitel ellenőrzéséhez. Győződjön meg arról, hogy mindhárom aláírással van. Ezután a **Fájlfeltöltés lehetőséggel** csatolja a kitöltött űrlapot a meglévő szolgáltatáskéréshez. A Microsoft támogatási szakembere nyolc órán belül visszatér Önhez, hogy ellenőrizze a nyugtát és a befejezést.

6. Új partner:

   Frissítse az Azure-előfizetés beállításait, hogy eltávolítsa a régi partnert a fiókból. Két PowerShell-parancsmag futtatásával láthatja, hogy mely szerepkör-hozzárendelések vannak kiépítve.

   - Adja hozzá az új partnert viszonteladóként a fiókhoz:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > Az ügyfél **bérlőazonosítója** megjelenik a Partnerközpont az ügyfél **Microsoft-azonosítójaként.** Egy adott ügyfél Microsoft-azonosítójának (bérlőazonosítójának) megkereséhez jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard) Ezután válassza **az Ügyfelek** lehetőséget a menüből. Keresse meg az ügyfelet a listában. A lefelé mutató nyílra kattintva bontsa ki az ügyfél termékoldalát. Az ügyfél tartománynevére és  Microsoft-azonosítójára vonatkozó adatokat **fog látni.** Használja a 16 jegyű **Microsoft-azonosítót** a PowerShell-parancsmagban.

   - Megtekintheti a fiók szerepköreit, beleértve a korábbi CSP-partnereket is:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Távolítsa el az elavult hozzáférési engedélyeket:

   - A Partnerközpont válassza az Ügyfelek **lehetőséget.**
   - Keresse meg az ügyfelet a listában. Válassza ki (kattintson duplán) a vállalata nevére. Ez a művelet megnyitja az ügyfél **Előfizetések oldalát.**
   - Az ügyféladatok menüben válassza a **Szolgáltatáskezelés lehetőséget.**
   - A **Microsoft Azure** alatt kattintson a hivatkozásra, hogy a következőre **a Microsoft Azure felügyeleti portálja.**

## <a name="next-steps"></a>Következő lépések

- Töltse le a [CSP-előfizetés átvitele űrlapot.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA)

- További információ [a többpartneres támogatásról.](multipartner.md)

- [többpartneres támogatás.](multipartner.md)
- [többcsatornás támogatás.](multichannel.md)
- [Azure-előfizetések átvitele](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)