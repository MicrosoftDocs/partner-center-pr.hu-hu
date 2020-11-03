---
title: Elérhető Azure-szolgáltatások az Azure CSP-ben
description: Ez a szakasz a Azure Cloud Solution Provider (CSP) programban nem elérhető Azure-szolgáltatásokat ismerteti.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: 094aa585be3114c198a8581b3d23bd4b212393c9
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528498"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>Az Azure Cloud Solution Provider (CSP) programban elérhető Azure-szolgáltatások

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Számlázási adminisztrátor
- Globális rendszergazda
- Segélyszolgálat ügynöke
- Értékesítési ügynök
- Felhasználói felügyeleti rendszergazda

## <a name="available-azure-services-in-azure-csp"></a>Elérhető Azure-szolgáltatások az Azure CSP-ben

Ez a cikk azokat az Azure-szolgáltatásokat sorolja fel, amelyek nem érhetők el a Azure Cloud Solution Provider (CSP) programban. Emellett a szolgáltatás elérhetőségét is tárgyalja az országos felhőkben [Microsoft Azure Germany](https://azure.microsoft.com/overview/clouds/germany/) és [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/).

>[!Note]
> Az Azure [China](https://www.azure.cn/) nem érhető el az Azure CSP programban.

## <a name="global-cloud"></a>Globális felhő

Az Azure Resource Manager modellen alapuló szolgáltatások a CSP programban érhetők el.  A nem Azure Resource Manager szolgáltatások nem érhetők el a CSP programban.  

## <a name="csp-specific-service-configurations"></a>CSP-Specific szolgáltatás konfigurációi

A következő szolgáltatások speciális konfigurációkat igényelnek a CSP-ben:

- [StorSimple](/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory tartományi szolgáltatások](/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) A Time Series Insights-környezetben csak az ügyfél bérlője férhet hozzá az adatokhoz. A partnerek alapértelmezés szerint kezelhetik ügyfeleik Time Series Insights-környezetét, de ha hozzá kell férniük a hozzájuk tartozó információhoz, hozzá kell adni őket az ügyfél bérlője számára.

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Most megvásárolhatja az alább felsorolt elemeket a Visual Studio Marketplace-en, a harmadik féltől származó bővítmények kivételével.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Visual Studio-előfizetések](https://www.visualstudio.com/subscriptions/)

- [Xamarin University képzés](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Az első lépésekhez készítettünk videókat és dokumentációt arról, [hogyan kell beállítani, megvásárolni és felügyelni az Azure-DevOps](/vsts/billing/csp/set-up-csp-customer) a CSP-ben.

## <a name="azure-marketplace-items-in-azure-csp"></a>Azure Marketplace-elemek az Azure CSP-ben

Jelenleg nem minden Azure Marketplace-elem érhető el az Azure CSP-előfizetésekben.

- Microsoft-alapú Azure-szolgáltatások: ezek a szolgáltatások elérhetők. Tekintse át az előző táblázatot és megjegyzéseket.

- Saját licenc-(BYOL-) elemek használata: ezek az elemek elérhetők. Az BYOL-kompatibilis Azure Marketplace-elemek teljes listája az [Azure MARKETPLACE BYOL oldalon](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)érhető el.

- Külső gyártótól származó Azure Marketplace-elemek: ezek az elemek akkor érhetők el, ha a szolgáltató közzé lett téve a CSP-csatornán. További információ: [előfizetés eladása az Azure Marketplace-termékekhez](csp-commercial-marketplace-overview.md).

- Citrix XenApp Essentials: a partnerek a CSP-ben vásárolhatnak XenApp Essentialst. További információkért tekintse meg a következő Citrix blog- [disztribúciót XenApp Essentials mostantól elérhető Microsoft Cloud megoldás-szolgáltatói csatornán keresztül](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/).

## <a name="national-clouds"></a>Országos felhők

Az alábbi táblázat az első féltől származó Azure-termékek,-szolgáltatások és-funkciók listáját mutatja be az országos felhőkben.

| Azure-termék,-szolgáltatás vagy-szolgáltatás | Egyesült Államok – Államigazgatás | Németország |
| ------ | :-----------: | :-----------: |
|  **Számítás**  |    |    |
|  Virtual Machines  |  X  |  X  |
|  Cloud Services  |    |    |
|  Virtuálisgép-méretezési csoportok  |  X  |  X  |
|  Functions  |    |    |
|  Azure Container Service  |    |    |
|  **Hálózat**  |    |    |
|  Azure DNS  |    |    |
|  Content Delivery Network  |    |    |
|  Traffic Manager  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Virtual Network  |  X  |  X  |
|  Load Balancer  |  X  |  X  |
|  VPN Gateway  |  X  |  X  |
|  Application Gateway  |  X  |  X  |
|  Network Watcher  |  X  |  X  |
|  **Storage**  |    |    |
|  Tárolás  |  X  |  X  |
|  Backup  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Storage  |    |    |
|  Managed Disks  |  X  |  X  |
|  **Web + mobil**  |    |    |
|  App Service  |  X  |  X  |
|  App Service Linux rendszeren  |    |  X  |
|  API Management  |  X  |    |
|  Content Delivery Network  |    |    |
|  Media Services  |  X  |  X  |
|  Notification Hubs  |  X  |  X  |
|  Azure Search  |    |    |
|  Azure App Service Logic Apps szolgáltatása  |    |    |
|  **Containers**  |    |    |
|  App Service  |  X  |  X  |
|  App Service Linux rendszeren  |    |  X  |
|  Batch  |  X  |  X  |
|  Container Registry  |    |    |
|  Tárolópéldányok  |    |    |
|  Service Fabric  |  X  |  X  |
|  Container Service  |    |    |
|  **Adatbázisok**  |    |    |
|  SQL Database  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Data Warehouse  |  X  |  X  |
|  Redis Cache  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Azure Database for MySQL  |    |    |
|  Azure Database for PostgreSQL  |    |    |
|  **Adatok + analitika**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Data Catalog  |    |    |
|  Data Lake Storage  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **AI + Cognitive Services**  |    |    |
|  Machine Learning  |    |  X  |
|  Azure Bot Service  |    |    |
|  Cognitive Services  |    |    |
|  Azure Batch AI  |    |    |
|  **Eszközök internetes hálózata**  |    |    |
|  IoT Hub  |  X  |  X  |
|  IoT-központ  |    |    |
|  Machine Learning  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Event Hubs  |  X  |  X  |
|  Location-Based szolgáltatások  |    |    |
|  Notification Hubs  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **Vállalati integráció**  |    |    |
|  StorSimple  |  X  |    |
|  API Management  |    |    |
|  Event Grid  |    |    |
|  Data Factory  |    |    |
|  Service Bus  |  X  |  X  |
|  Data Catalog  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Azure App Service Logic Apps szolgáltatása  |    |    |
|  **Biztonság és identitáskezelés**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Többtényezős hitelesítés  |    |    |
|  Azure Active Directory tartományi szolgáltatások  |    |    |
|  Key Vault  |  X  |  X  |
|  Security Center  |  X  |  X  |
|  **Fejlesztői eszközök**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **Monitoring és felügyelet**  |    |    |
|  Advisor  |    |    |
|  Backup  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  Scheduler  |  X  |  X  |
|  Automation  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Alkalmazások Azure-Managed  |    |    |
|  Azure Migrate  |    |    |
|  Felügyeleti csoportok  |    |  

## <a name="next-steps"></a>Következő lépések

- [Ismerje meg](/azure/cloud-solution-provider/overview/partner-center-overview) az Azure elérhető képességeit a partner Centerben.

- [Hozza létre](/azure/cloud-solution-provider/customer-management/create-new-customer) első ügyfelét az Azure CSP-ben, és telepítse az Azure-szolgáltatásokat.
