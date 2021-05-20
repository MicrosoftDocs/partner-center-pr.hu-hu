---
title: Elérhető Azure-szolgáltatások az Azure CSP-ben
description: Ez a cikk az Azure-felhőszolgáltató (CSP) programjában elérhető és nem elérhető Azure-szolgáltatásokat ismerteti.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: da97dded531b6792a4468d9be9b63367f818b352
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149740"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>A Azure-felhőszolgáltató (CSP) programban elérhető Azure-szolgáltatások

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Globális rendszergazdai | Az | Értékesítési ügynök | Felhasználókezelő rendszergazda

## <a name="available-azure-services-in-azure-csp"></a>Elérhető Azure-szolgáltatások az Azure CSP-ben

Ez a cikk azokat az Azure-szolgáltatásokat sorolja fel, amelyek a Azure-felhőszolgáltató (CSP) programban nem érhetők el. Emellett az országos felhőkben és felhőkben elérhető [Microsoft Azure Germany](https://azure.microsoft.com/overview/clouds/germany/) [és](https://azure.microsoft.com/overview/clouds/government/)Microsoft Azure Government.

>[!Note]
> [Az Azure China](https://www.azure.cn/) nem érhető el a Azure CSP programjában.

## <a name="global-cloud"></a>Globális felhő

A csp-Azure Resource Manager minden szolgáltatás elérhető.  A nem Azure Resource Manager szolgáltatások nem érhetők el a CSP-programban.  

## <a name="csp-specific-service-configurations"></a>CSP-Specific szolgáltatáskonfigurációk

Az alábbi szolgáltatások speciális konfigurációkat igényelnek a CSP-hez:

- [StorSimple](/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory tartományi szolgáltatások](/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) Csak az ügyfélbérlő felhasználói férhetnek hozzá a saját Time Series Insights adataihoz. A partnerek alapértelmezés szerint kezelhetik az ügyfél Time Series Insights környezetét, de ha hozzá kell férni az abban megadott adatokhoz, akkor hozzá kell adni őket az ügyfélbérlőhöz.

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Most már megvásárolhatja az alább felsorolt elemeket a Visual Studio Marketplace-en, a külső bővítmények kivételével.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Visual Studio előfizetések](https://www.visualstudio.com/subscriptions/)

- [Xamarin University betanítás](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Az első lépésekhez videókat és dokumentációt hoztunk létre az [Azure DevOps](/vsts/billing/csp/set-up-csp-customer) CSP-beli beállítására, megvásárlására és kezelésére.

## <a name="azure-marketplace-items-in-azure-csp"></a>Azure Marketplace-elemek az Azure CSP-ben

Jelenleg nem minden Azure Marketplace érhető el a Azure CSP előfizetésben.

- Microsoft-alapú Azure-szolgáltatások: Ezek a szolgáltatások elérhetők. Tekintse át az előző táblázatot és megjegyzéseket.

- Saját licenc (BYOL) elemek: Ezek az elemek elérhetők. A BYOL-kompatibilis Azure Marketplace teljes lista a [BYOL Azure Marketplace érhető el.](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)

- Harmadik féltől származó, harmadik féltől származó Azure Marketplace: Ezek az elemek akkor érhetők el, ha a szolgáltató közzétette a CSP-csatornát. További információ: [Előfizetések eladása Azure Marketplace termékekhez.](csp-commercial-marketplace-overview.md)

- Citrix XenApp Essentials: A partnerek vásárolhatnak XenApp Essentials csp-ügyfelek számára. További információkért tekintse meg a következő Citrix blogot: A XenApp Essentials terjesztése a Microsoft felhőszolgáltató [csatornán keresztül.](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/)

## <a name="national-clouds"></a>Országos felhők

Az alábbi táblázat az országos felhők felhőiben a CSP-hez elérhető, külső Azure-termékek, -szolgáltatások és -funkciók rendszeresen frissített listáját jeleníti meg.

| Azure-termék, -szolgáltatás vagy -funkció | Egyesült Államok – Államigazgatás | Németország |
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
|  **Web és mobil**  |    |    |
|  App Service  |  X  |  X  |
|  App Service Linux rendszeren  |    |  X  |
|  API Management  |  X  |    |
|  Content Delivery Network  |    |    |
|  Media Services  |  X  |  X  |
|  Notification Hubs  |  X  |  X  |
|  Azure Search  |    |    |
|  Logic Apps szolgáltatás Azure App Service  |    |    |
|  **Containers**  |    |    |
|  App Service  |  X  |  X  |
|  App Service Linux rendszeren  |    |  X  |
|  Batch  |  X  |  X  |
|  Container Registry  |    |    |
|  Container Instances  |    |    |
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
|  IoT Central  |    |    |
|  Machine Learning  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Event Hubs  |  X  |  X  |
|  Location-Based Services  |    |    |
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
|  Logic Apps szolgáltatás Azure App Service  |    |    |
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
|  Azure-Managed Alkalmazások  |    |    |
|  Azure Migrate  |    |    |
|  Felügyeleti csoportok  |    |  

## <a name="next-steps"></a>Következő lépések

- [Ismerje](/azure/cloud-solution-provider/overview/partner-center-overview) meg az Azure-ban elérhető képességeket a Partnerközpont.

- [Hozza](/azure/cloud-solution-provider/customer-management/create-new-customer) létre első ügyfélét a Azure CSP, és telepítse az Azure-szolgáltatásokat.
