---
title: Ügyfelek áthelyezése a jelenlegi Azure-ajánlatokból Azure-csomagba
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogy a CSP-partnerek hogyan Partnerközpont ügyfeleket a meglévő CSP Azure-ajánlatokból az Azure-szolgáltatásokba az Azure-csomag keretében.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 770df3cff40b8cc51eab16fb95d0bd43967a5a69
ms.sourcegitcommit: 3ac88f7925bfe1df90e267ee5c1ee4d752ac92d4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/29/2021
ms.locfileid: "113013267"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Ügyfelek váltása Azure-csomagra meglévő CSP Azure-ajánlatokból

**A következőkre vonatkozik:** Partnerközpont 

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Globális rendszergazdai | Az | Értékesítési ügynök | Felhasználókezelő rendszergazda

Ez a cikk azt ismerteti, hogy a CSP-partnerek hogyan Partnerközpont az ügyfeleket a meglévő CSP Azure-ajánlatokból az Azure-szolgáltatásokba az Azure-csomag keretében. A közvetett szolgáltatók és a közvetlen számlázási partnerek áttérnek az Azure-hoz elérhető Microsoft Cloud Service Provider Programban (CSP) elérhető új kereskedelmi élményre. (A közvetett viszonteladóknak a közvetett szolgáltatóikon keresztül kell dolgozniuk.) Az ügyfelek zökkenőmentesen vásárolhatnak felhőszolgáltatásokat, akár partnerektől, akár Microsoft-értékesítőktől vagy közvetlenül a weben vásárolnak.

Az áttérési képesség csak az azure-beli új kereskedelmi felhasználói élményre áttérő, és az előfizetést aláíró ügyfelek Microsoft Ügyfélszerződés. Ez nem más CSP-ajánlatokhoz, például az Office 365-hez vagy a Dynamics 365-hez való.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Meglévő CSP-ajánlatok váltása Azure-csomagra

A CSP-program új kereskedelmi élményében az ügyfél meglévő CSP Azure-ajánlataiból az Azure-szolgáltatásokra az Azure-csomag keretében, a felhőszolgáltatói programon belül Partnerközpont. Ehhez a partnernek és az ügyfélnek egy már létrehozott viszonteladói kapcsolattal kell Partnerközpont, és az ügyfélnek alá kell írnia a Microsoft Ügyfélszerződés.

### <a name="select-transition-to-azure-plan"></a>Váltás Azure-csomagra kiválasztása

1. Válassza az Azure-csomag lehetőséget az ügyfél számára.

2. Válassza **a Számlázás váltása Azure-csomagra lehetőséget.**

   :::image type="content" source="images/azure/transition1.png" alt-text="Képernyőkép a használatalapú előfizetések jelentési adatairól egy kiválasztható lehetőséggel: Az Azure-előfizetés számlázásának váltása Azure-csomagra.":::

3. Válassza a **Folytatás** elemet

   :::image type="content" source="images/azure/transition2.png" alt-text="Az Áttérés Az Azure-csomagra című párbeszédpanel, amely hatással van az átváltásra, valamint két választható lehetőség, a Folytatás vagy a Mégse elemre.":::

   Az ügyfél átvált az Azure-csomagra.

   **Az átváltási munkafolyamat automatizálja az előfeltételként szükséges lépéseket:**

   - Azure-csomag(ak) vásárlása
   - Ügyfélenként egy csomag a közvetlen CSP-forgatókönyvekben  
   - Viszonteladónként egy csomag  

   Egy partner például megvásárolt két Microsoft Azure, és két különálló POR-t tartalmazott a vásárlásban. Ebben az esetben az átváltási munkafolyamat két Azure-előfizetést vásárol (viszonteladónként egyet), és automatikusan leképezi a megfelelő Azure-előfizetéseket az Azure-csomagok alatt.  

   **Azure-előfizetés leképezése Azure-csomagra**

   Az Azure-csomagok megvásárlása után a rendszer leképezi a meglévő Azure-előfizetéseket az Azure-csomagokra. Az előrehaladás megtekinthető a Azure Portal a Partnerközpontban is.

4. Térjen vissza az ügyfél Előfizetések Partnerközpont **oldalára,** és frissítse a költségkeretét a helyi pénznemük használatával.

   :::image type="content" source="images/azure/transition3.png" alt-text="Az Előfizetések Partnerközpont részleges nézete, amely a számlázási időszakra vonatkozó, helyi pénznemben beállított költségvetési korlátokkal rendelkezik.":::

   >[!NOTE]
   >Az ebben a Partnerközpont beállított költségvetés nem lesz áthozva a Azure Portal. A költségvetést és a riasztást a következő Azure Portal.

   Az Azure-csomagra való áttérve már nem vásárolhat Azure-előfizetéseket ehhez az ügyfélhez. Az előfizetéseket az Azure-csomag alatt hozhatja létre a Azure Portal.

   >[!NOTE]
   > Az RBAC-n keresztül az Azure-csomag keretében vásárolt összes Azure-előfizetés díjszabása és számlázása helyi pénznemben történik. Az FX-árfolyamok nem lesznek használva.

### <a name="track-your-transition-details"></a>Az átváltás részleteinek nyomon követése

Kövesse az áttérési előrehaladást a Azure Portal a következő Partnerközpont.

:::image type="content" source="images/azure/details1.png" alt-text="Képernyőkép az előfizetésenkénti áttűnés részleteinek listáját tartalmazó táblázatról – ide tartozik az előfizetésI D, az átváltás dátuma és az átváltás állapota.":::

### <a name="billing-impact-to-partners"></a>A partnerek számlázásra gyakorolt hatása

Ha egy ügyfelet egy meglévő CSP Azure-ajánlatból hoz át, az a következő számlázási hatásokkal jár:

- A meglévő CSP-számlán az összes használatért az eredeti CSP Azure-előfizetésből való kilépésig kell fizetni.

- Ha rendszergazdai hozzáférési jogosultságokkal rendelkezik a meglévő CSP-előfizetéshez, az előfizetés migrálkor továbbra is hozzáférhet.

Ha közvetlen Nagyvállalati Szerződéseket a CSP- és kiszolgáló- és felhőalapú regisztrációkról azure-szolgáltatásokra is át kell irányítania, olvassa el a következőt: [Azure-előfizetések](/azure/billing/mpa-request-ownership) számlázási tulajdonjogának Microsoft Partnerszerződés

### <a name="audit-log"></a>Az auditnaplóban

A számlázás egyeztetéséhez tekintse meg a "Microsoft Azure" (0145P) előfizetések előzményeit az **Előfizetések** lapon.

A "Microsoft Azure" (0145P) előfizetés két részből áll:

1. Kereskedelmi előfizetés
2. Azure-előfizetés (jogosultság)

Ha az átállás befejeződött, az Azure-előfizetés az új Azure-csomag alá kerül, és a kereskedelmi előfizetés fel lesz függesztve, hogy a rendszer ne jelentsen további használatot.  

>[!NOTE]
>Amikor Microsoft Azure (0145P) előfizetést vásárolnak a CSP-ben, a kereskedelmi előfizetés és az Azure-előfizetés (jogosultság) ugyanazokkal az értékkel rendelkezik. Ez csak abban az esetben változik, ha a számlázási tulajdonjog megváltozik vagy az átadások eltérnek az értékektől.

### <a name="transition-issues"></a>Áttűnésekkel kapcsolatos problémák

Az átváltások során nem számítunk problémákra. Ha van ilyen, magát az átváltási munkafolyamatot fogjuk frissíteni. Az Azure-használatot nem fogják zavarni.  

## <a name="next-steps"></a>Következő lépések

- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)

- [Partneri jóváírás – áttekintés](partner-earned-credit.md)
