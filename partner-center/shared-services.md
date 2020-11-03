---
title: Azure partner megosztott szolgáltatások hozzáadása
description: Az Azure partner megosztott szolgáltatásaival saját használatra vásárolhat Azure-előfizetéseket, és egységes módszert használhat az Azure megvásárlásához, nyomon követéséhez és kezeléséhez.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 49b5bd1c9a7cd4c56f2fac28a45cc8a4b922b9b0
ms.sourcegitcommit: 2d11dbdcc2b1e64ad16d29182824984517470a63
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/24/2020
ms.locfileid: "92530103"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Azure partner megosztott szolgáltatások hozzáadása, hogy a partnerek saját használatra tudják megvásárolni az Azure-előfizetéseket

**A következőkre vonatkozik**

- Partnerközpont
 
**Megfelelő szerepkörök**

- Globális rendszergazda
- Felügyeleti ügynök
- Értékesítési ügynök

Az Azure partner Shared Services egy új ajánlat típusa a CSP programban lévő partnereknek, amely lehetővé teszi, hogy a partnerek saját használatra vásárolják meg az Azure-előfizetéseket.Lehetőséget teremt arra, hogy a partnerek egységes módszert használjanak az Azure megvásárlására, nyomon követésére és felügyeletére, valamint az Azure-licencek konszolidálása és a szerződések a Microsofttal való viszonteladásának lehetősége mellett. Az Azure partner megosztott szolgáltatásainak köszönhetően a partnerek mostantól ugyanolyan rugalmasan használhatják az Azure-előfizetéseket a CSP-ben, mint a Microsoft Nagyvállalati Szerződés és a webes Direct programokban, olyan forgatókönyveket nyitnak meg, mint például a fejlesztési és tesztelési környezetek létrehozása, a belső számítási feladatok üzembe helyezése és a megosztott szolgáltatások vagy több-bérlős alkalmazások  

## <a name="create-the-shared-services-tenant"></a>A megosztott szolgáltatások bérlő létrehozása

1. Lépjen a **Beállítások**  >  **fiók beállításai**  >  **megosztott szolgáltatások** menüpontra.

   :::image type="content" source="images/sharedservices2.png" alt-text="Fiókbeállítások > megosztott szolgáltatások":::

2. Ha még nem rendelkezik megosztott szolgáltatások Bérlővel, kattintson a **megosztott szolgáltatások létrehozása** lehetőségre.

   :::image type="content" source="images/sharedservices3.png" alt-text="Fiókbeállítások > megosztott szolgáltatások":::

3. Ez létrehoz egy megosztott szolgáltatások bérlőt, és megvásárolja az Azure CSP megosztott szolgáltatásainak előfizetését, amelyet a megosztott erőforrásokhoz és a belső számítási feladatokhoz használhat.

   :::image type="content" source="images/sharedservices5.png" alt-text="Fiókbeállítások > megosztott szolgáltatások":::

## <a name="about-the-azure--internalshared-services-offer"></a>Az Azure-Internal/Shared Services ajánlat

- A Azure-Internal/Shared Services-előfizetés egy olyan új Azure-ajánlat típusa, amely a partner centeren keresztül érhető el, és a partnerek az Azure-t használják.

- Azure-Internal/Shared Services ajánlat nem jogosult kedvezmények és ösztönzők használatára.

- Az Azure-Internal/Shared Services ajánlat csak a megosztott szolgáltatások bérlőre alkalmazható.

- Az Azure-Internal/Shared Services-előfizetés elsődleges használata, hogy az Azure-t saját fejlesztési célokra használhatja. Az ajánlat kiépítéséhez használt megosztott bérlő nem használható más szolgáltatásokhoz, például az Office 365-hez vagy a Dynamics-licencekhez.

- Megszakíthatja az előfizetést, mint bármely más előfizetést. Lépjen a **Beállítások**  >  **nézet minden beállítás**  >  **megosztott szolgáltatások** menüpontra. Válassza ki a Azure-Internal/Shared Services-előfizetést, és szakítsa meg.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Az Azure partner megosztott szolgáltatások használati adatainak elérése

Az Azure-beli felhasználást a CSP-számlán és a megbékélési fájlban találja. Ez a számla Microsoft Azure tételének részeként fog szerepelni. A részletes használati adatok az ajánlathoz létrehozott Bérlővel naplózott egyeztetési fájlban lesznek elérhetők.

## <a name="azure-partner-shared-services-pricing"></a>Az Azure partner megosztott szolgáltatásainak díjszabása

Ha szeretné megtekinteni az Azure partner megosztott szolgáltatásainak új díjszabási fájlját, válassza a **Sell**  >  **díjszabás és ajánlatok** eladása lehetőséget, és válassza ki az aktuális hónap árlista listáját. Az elkövetkező hetekben egy adott díj kártya API-t is kiadunk.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Piactéri ajánlatok és az Azure partner megosztott szolgáltatásai

2019. március 1-től az Azure partner Shared Services (APSS) már nem támogatja a Piactéri ajánlatokat.

|**Marketplace-támogatás**   |**A APSS a 2019. március 1. előtt támogatott**|**2019. március 1-től**|
|---------------------------|:----------------------------|:-------------------|
|Saját licenc használata (BYOL) és ingyenes szolgáltatások   | Igen   | Nem|
|Egyéb harmadik féltől származó Piactéri ajánlatok   | Nem   |Nem|

A APSS használatával üzembe helyezett BYOL-vagy ingyenes szolgáltatásokkal kapcsolatos partnereinket nem érinti a rendszer. 2019. március 1-től azonban nem vásárolhat új BYOL vagy ingyenes szolgáltatásokat.

A piactéren elérhető ajánlatok teljes katalógusának kihasználásához (nem csak BYOL és ingyenes szolgáltatásokhoz) javasoljuk, hogy a CSP-partnerek a web Direct Azure-előfizetések használatával közös szolgáltatásokat telepítsenek.  Azok a CSP-partnerek, akik korábban üzembe helyeztek harmadik féltől származó BYOL és ingyenes szolgáltatási erőforrásokat a piactéren, és továbbra is szeretnék használni őket, és több harmadik féltől származó ajánlatot is üzembe helyezhetnek, javasoljuk, hogy a APSS-előfizetés áttelepítését a [meglévő Azure-előfizetések áttelepítéséhez](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

Azok a partnerek, akik a APSS-előfizetés 2019. március 1. után való használatának folytatását tervezik, és új, harmadik féltől származó [BYOL-szolgáltatásokat](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) vagy ingyenes szolgáltatásokat kívánnak telepíteni, a független gyártóktól származó utasításokat követve telepíthetik ezeket a APSS-előfizetésekre.