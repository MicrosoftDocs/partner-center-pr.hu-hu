---
title: Új Azure Partner Shared Services
description: A Azure Partner Shared Services saját használatra vásárolhat Azure-előfizetéseket, és egységes módszert használhat az Azure megvásárlására, nyomon követésére és kezelésére.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 40ba485cecce394dc81632d01f8774859690c522
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551605"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>További Azure Partner Shared Services, hogy a partnerek saját használatra vásárolják meg az Azure-előfizetéseket

**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök | Értékesítési ügynök

Azure Partner Shared Services (APSS) egy új ajánlattípus a Felhőszolgáltató -es (CSP) program partnerei számára, amely lehetővé teszi a partnerek számára, hogy saját használatra vásárolják meg az Azure-előfizetéseket.Lehetővé teszi a partnerek számára, hogy egységes módszert használjanak az Azure megvásárlására, nyomon követésére és felügyeletére, valamint összevonják az Azure-licencelési és újralicencelési szerződéseiket a Microsofttal. Az APSS-sel a partnerek ugyanolyan rugalmasan használhatnak Azure-előfizetéseket a CSP-kben, mint a Microsoft Nagyvállalati Szerződés és a Web Direct programokban, és olyan forgatókönyveket nyitnak meg, mint a fejlesztési és tesztelési környezetek kiépítése, a belső számítási feladatok üzembe helyezése, valamint a megosztott szolgáltatások vagy több-bérlős alkalmazások üzembe helyezése.  

## <a name="create-the-shared-services-tenant"></a>A megosztott szolgáltatások bérlője létrehozása

1. A Beállítások  >  **Fiókbeállítások Megosztott szolgáltatások**  >  **lapra.**

   :::image type="content" source="images/sharedservices2.png" alt-text="Fiókbeállítások > szolgáltatásokhoz":::

2. Ha még nem rendelkezik megosztott szolgáltatásbérlővel, válassza a **Megosztott szolgáltatások létrehozása lehetőséget.**

   :::image type="content" source="images/sharedservices3.png" alt-text="Megosztott szolgáltatások létrehozása.":::

3. Ez létrehoz egy megosztott szolgáltatásbérlőt, és megvásárolja Azure CSP Megosztott szolgáltatások előfizetést, amely a megosztott erőforrásokhoz és a belső számítási feladatokhoz lesz használva.

   :::image type="content" source="images/sharedservices5.png" alt-text="Hozza létre a bérlőt, és vásárolja meg az előfizetést.":::

## <a name="about-the-azure--internalshared-services-offer"></a>A Azure - Internal/Shared Services ajánlatról

- A Azure - Internal/Shared Services előfizetés egy új Azure-ajánlattípus CSP-beli, Partnerközpont a partnerek saját Azure-használatra kapják meg.

- Azure Partner Shared Services előfizetések jogosultak, és használhatók a RI-k megvásárlására.

- A Azure - Internal/Shared Services ajánlat csak a megosztott szolgáltatások bérlője számára alkalmazható.

- Az előfizetés elsődleges Azure - Internal/Shared Services, hogy az Azure-t saját fejlesztési célokra használjuk. Az ajánlat kiépítése érdekében használt megosztott bérlő nem használható más szolgáltatásokhoz, például Office 365- vagy Dynamics-licencekhez.

- Az előfizetést a többi előfizetéshez hasonló módon mondhatja le. A Megosztott szolgáltatások  >  **Az összes megtekintése**  >  **beállításokat.** Válassza ki Azure - Internal/Shared Services előfizetést, és mondja le.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>A Azure Partner Shared Services adatok elérése

Az Azure-használatot a CSP-számlán és az egyeztetési fájlban találja. Ez a számla egy Microsoft Azure részeként fog szerepelni. A részletes felhasználási adatok az ajánlathoz létrehozott bérlőhöz naplózott egyeztetési fájlban lesznek elérhetők.

## <a name="azure-partner-shared-services-pricing"></a>Azure Partner Shared Services díjszabás

Az APSS új díjszabási fájlját a **Díjszabás** és ajánlatok eladása alatt, az aktuális havi árlistában  >   láthatja. A következő hetekben egy adott rate card API is elérhető lesz.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Marketplace-ajánlatok és Azure Partner Shared Services

2019. március 1-től az APSS már nem támogatja a Marketplace-ajánlatokat.

|**Marketplace-támogatás**   |**Az APSS 2019. március 1. előtt támogatott**|**2019. március 1. után**|
|---------------------------|:----------------------------|:-------------------|
|Saját licenc (BYOL) és ingyenes szolgáltatások   | Igen   | Nem|
|Egyéb külső Marketplace-ajánlatok   | Nem   |Nem|

Az APSS használatával üzembe helyezett BYOL- vagy ingyenes szolgáltatásokkal kapcsolatos partnerekre ez nem lesz hatással; 2019. március 1. után azonban nem vásárolhatnak új BYOL-t vagy ingyenes szolgáltatásokat.

Az elérhető Marketplace-ajánlatok teljes katalógusának (nem csak a BYOL és az ingyenes szolgáltatások) előnyeinek kihasznál érdekében javasoljuk, hogy a CSP-partnerek megosztott szolgáltatásokat telepítsenek a web direct Azure-előfizetések használatával.  Azok a CSP-partnerek, akik korábban már telepítettek harmadik féltől származó BYOL- és ingyenes szolgáltatási erőforrásokat a Marketplace-ről, és továbbra is használni szeretnék őket, és további külső ajánlatok üzembe helyezését szeretnék, arra biztatjuk, hogy az APSS-előfizetést a webre telepítsék át közvetlenül a meglévő Azure-előfizetések [áttelepítésére.](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)

Azok a partnerek, akik 2019. március 1. után is szeretnék használni az APSS-előfizetést, és új, harmadik [féltől](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) származó BYOL-szolgáltatásokat vagy ingyenes szolgáltatásokat szeretnék üzembe helyezni, az ISV-k utasításait követve üzembe helyezhetik ezeket az APSS-előfizetéseikben.

## <a name="next-steps"></a>Következő lépések

- [Szoftver-előfizetések értékesítése felhőszolgáltatón keresztül](csp-software-subscriptions.md)