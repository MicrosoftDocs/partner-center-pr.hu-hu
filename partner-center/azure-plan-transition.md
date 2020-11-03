---
title: Ügyfelek áthelyezése az aktuális Azure-ajánlatokból az Azure-csomagba
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy a CSP-partnerek hogyan használhatják a partner központot a meglévő CSP Azure-ajánlatokból az Azure-csomag keretében az Azure-szolgáltatásokhoz.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 5390e950689e930b246aaaddcb1a9ef1b1ab6d46
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529922"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Ügyfelek átváltása Azure-csomagra meglévő CSP Azure-ajánlatokból

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Számlázási adminisztrátor
- Globális rendszergazda
- Segélyszolgálat ügynöke
- Értékesítési ügynök
- Felhasználói felügyeleti rendszergazda

A közvetett szolgáltatók és a közvetlen számlázási partnerek az Azure-beli Microsoft Cloud Service Provider program (CSP) szolgáltatásban elérhető új kereskedelmi élményre válthatnak. (A közvetett viszonteladóknak a közvetett szolgáltatókon keresztül kell dolgozniuk.) Az ügyfelek zökkenőmentesen vehetik igénybe a felhőalapú szolgáltatásokat, akár a partnerektől, akár a Microsoft értékesítőtől, akár közvetlenül a világhálón vásárolnak.

Az áttérési képesség csak olyan ügyfelek számára érhető el, akik az Azure új kereskedelmi tapasztalatára áttértek, és akik aláírták a Microsoft ügyfél-szerződést, nem pedig a CSP-ben, például az Office 365-ben vagy a Dynamics 365-ben.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Meglévő CSP-ajánlatok átváltása Azure-csomagra

A meglévő CSP Azure-ajánlatait áthelyezheti az Azure-szolgáltatásokba az Azure-csomag keretében az új kereskedelmi környezet keretében a CSP programban a partner Centerben. Ehhez a partnernek és az ügyfélnek rendelkeznie kell egy, a partner centeren keresztül létrehozott viszonteladói kapcsolattal, és az ügyfélnek alá kell írnia a Microsoft ügyfél-szerződést.

### <a name="select-transition-to-azure-plan"></a>Az Azure-csomagra való áttérés kiválasztása

1. Válassza ki az Azure-csomagot az ügyfél számára.

2. Válassza **az áttérési számlázás az Azure-csomagra** lehetőséget.

   :::image type="content" source="images/azure/transition1.png" alt-text="Képernyőfelvétel: a használaton alapuló előfizetések jelentési információi az Azure-előfizetésre váltás Azure-csomagra való áttéréskor használt választható lehetőséggel.":::

3. Válassza a **Folytatás** elemet

   :::image type="content" source="images/azure/transition2.png" alt-text="Képernyőfelvétel: a használaton alapuló előfizetések jelentési információi az Azure-előfizetésre váltás Azure-csomagra való áttéréskor használt választható lehetőséggel.":::

   Az ügyfelet az Azure-csomagra fogjuk áttérni.

   **Az áttérési munkafolyamat automatizálja az előfeltételként szükséges lépéseket** :

   - Azure-csomag (ok) vásárlása
   - Egy csomag ügyfélként a közvetlen CSP-forgatókönyvek esetében  
   - Egy csomag/viszonteladó  

   Egy partner például két Microsoft Azure ajánlatot vásárolt, és két különböző POR szerepel a vásárlásban. Ebben az esetben az áttérési munkafolyamat két Azure-csomagot (egy-egy viszonteladót) vásárol, és az Azure-csomagok megfelelő Azure-előfizetéseit automatikusan leképezi.  

   **Azure-előfizetés leképezése az Azure-csomagra**

   Az Azure-csomag (ok) megvásárlása után a rendszer leképezi a meglévő Azure-előfizetéseket az Azure-csomagokra. A folyamat Azure Portal és a partner Centerben is megtekinthető.

4. Térjen vissza az ügyfél partneri központ- **előfizetések** lapjára, hogy a helyi pénznem alapján frissítse a költségvetési korlátot.

   :::image type="content" source="images/azure/transition3.png" alt-text="Képernyőfelvétel: a használaton alapuló előfizetések jelentési információi az Azure-előfizetésre váltás Azure-csomagra való áttéréskor használt választható lehetőséggel.":::

   >[!NOTE]
   >A partner Centerben megadott költségkeret nem veszi át a Azure Portal. A költségvetést és a riasztást is be kell állítania Azure Portalban.

   Az Azure-csomagra való áttérés után már nem vásárolhat Azure-előfizetéseket ehhez az ügyfélhez. Az előfizetéseket az Azure Portal Azure-csomagjában hozza létre.

   >[!NOTE]
   > Az Azure-RBAC keresztül vásárolt Azure-előfizetések díjszabása és számlázása helyi pénznemben történik. Az FX díjszabása nem lesz használatban.

### <a name="track-your-transition-details"></a>Az áttérés részleteinek nyomon követése

Kövesse az áttérési folyamatot Azure Portal és a partner Centerben.

:::image type="content" source="images/azure/details1.png" alt-text="Képernyőfelvétel: a használaton alapuló előfizetések jelentési információi az Azure-előfizetésre váltás Azure-csomagra való áttéréskor használt választható lehetőséggel.":::

### <a name="billing-impact-to-partners"></a>A partnerek felé irányuló számlázási hatás

Ha egy meglévő CSP Azure-ajánlatból átvált egy ügyfelet, a következő számlázási hatások lesznek:

- A meglévő CSP-számlán minden használat után az eredeti CSP Azure-előfizetés kilépési pontjáig kell fizetnie.

- Ha rendszergazdai hozzáférési jogosultságokkal rendelkezik a meglévő CSP-előfizetéshez, akkor továbbra is hozzáférhet az előfizetés áttelepítésekor.

A közvetlen nagyvállalati szerződések a CSP-re, valamint a kiszolgáló-és Felhőbeli regisztrációra az Azure-szolgáltatásokra való áttéréshez olvassa el az [Azure-előfizetések számlázásának beszerzése](/azure/billing/mpa-request-ownership)

### <a name="audit-log"></a>Az auditnaplóban

A számlázás egyeztetéséhez tekintse meg a "Microsoft Azure" (0145P) előfizetések előzményeit az **előfizetések** lapon.

A "Microsoft Azure" (0145P) előfizetés két részből áll:

1. Kereskedelmi előfizetés
2. Azure-előfizetés (jogosultság)

Az áttérés befejezésekor az Azure-előfizetést új Azure-csomagba helyezi át, és a kereskedelmi előfizetés fel van függesztve, hogy ne jelentsen további használati adatokat.  

>[!NOTE]
>Ha Microsoft Azure (0145P) előfizetést vásárol a CSP-ben, akkor a kereskedelmi előfizetés és az Azure-előfizetés (jogosultság) is azonos értékű. Csak a számlázási tulajdonosi változások esetén, vagy az értékek eltérőek.

### <a name="transition-issues"></a>Átmeneti problémák

A váltás során nem számítunk fel problémákat. Ha ez történik, az áttérési munkafolyamatban is frissítjük Önt. Nem zavarja az Azure-használatot.  

## <a name="next-steps"></a>Következő lépések

- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)

- [Partner által létrehozott kredit – áttekintés](partner-earned-credit.md)