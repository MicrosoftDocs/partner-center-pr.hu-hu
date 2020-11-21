---
title: Azure Marketplace-partnerintegrációk
description: Ismerje meg az Azure-környezettel integrálható Azure Marketplace-megoldásokat, valamint a Microsoft-partnerek telepítési útmutatóinak hivatkozását.
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: b31486000e59f3d85ee30019ecea000252b297a8
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006905"
---
# <a name="azure-marketplace-partner-integrations"></a>Azure Marketplace-partnerintegrációk

Ismerje meg, hogyan integrálhatja a partneri megoldásokat az Azure-környezetbe. Ez a cikk áttekintést nyújt az egyes megoldásokról, valamint a részletes üzembe helyezési útmutatókra mutató hivatkozásokat tartalmaz. A megoldások betűrendben vannak felsorolva. 

## <a name="apache-kafka-on-confluent-cloud"></a>Apache Kafka az Fluent felhőben

![Felhőalapú felhő](./media/partners/confluent-cloud.png)

Az Azure lehetővé teszi, hogy a felhőalapú alkalmazásain kívül integrálja az Fluent-felhőt. A Fluent ügyfelek gyakran navigálnak a Azure Portal és a felhő között. Ha például egy felhasználó egy Fluent Felhőbeli ajánlatot vásárol az Azure Marketplace-en, akkor várhatóan egy olyan fiókot kell létrehoznia, amely az Fluent-felhővel rendelkezik. Ez a folyamat bonyolultságot és időt vesz igénybe, és megköveteli, hogy a felhasználók a két portál között kezeljék a konfigurációt és az erőforrásokat. A többplatformos felügyelet terhének csökkentése érdekében a Microsoft, együttműködve a közös felhővel, integrált kiépítési réteget épített ki az Azure-ból a felhőre. A megoldás az Azure Marketplace-en érhető el, és zökkenőmentes élményt nyújt az Azure-beli, felhőalapú ajánlat használatával

A megoldás az Azure-ban engedélyezett erőforrás-szolgáltatót használ a Felhőbeli felhőalapú erőforrások kiépítéséhez. Ez lehetővé teszi a felhasználók számára, hogy a Azure Portal, az Azure CLI és az Azure SDK-k segítségével férhessenek hozzá a valós idejű események folyamatos átviteléhez. A felhő tulajdonosa és futtatja az SaaS-alkalmazást, beleértve a környezeteket, a fürtöket, a témákat, az API-kulcsokat és a felügyelt összekötőket.

Az Fluent felhővel való mélyreható integráció a következő képességeket biztosítja:

- Hozzon létre egy új, a teljes körűen felügyelt infrastruktúrával rendelkező felhőalapú szervezeti erőforrást a Azure Portal.
- Egyszerűsítse az Azure-ba való egyszeri bejelentkezést, hogy Azure Active Directory; nincs szükség külön hitelesítésre az Fluent felhő-portálon.
- Az Azure-előfizetések számlázása révén egységes számlázást kaphat a Felhőbeli fogyasztási díjakról.
- Felügyelheti a Azure Portal a felhőalapú erőforrásokat, és nyomon követheti azokat a **minden erőforrás** lapon, az Azure-erőforrások mellett.

[A felhőalapú üzembe helyezési útmutatók](https://docs.confluent.io/current/cloud/marketplace/index.html)

Az Azure-hoz kapcsolódó problémákkal kapcsolatban nyissa meg a következőt: [https://support.confluent.io](https://support.confluent.io) . Ha első alkalommal felhasználó, állítsa alaphelyzetbe a jelszót, mielőtt bejelentkezne az Fluent támogatási portálra. Ha nem rendelkezik Fluent-fiókkal, küldjön e-mailt a címre [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![Datadoggal embléma](./media/partners/datadog.png)

A datadoggal megfigyelhető és biztonsági eszközöket biztosít az Azure-felhasználók számára, hogy megértsék az alkalmazásaikat a hibrid és a többfelhős környezetekben. A szükséges integrációk konfigurálásához azonban gyakran szükség van a Azure Portal és a Datadoggal közötti navigálásra. A különböző portálokon a konfiguráció-és erőforrás-kezelés egyszerűsítése érdekében a Microsoft a Datadoggal-mel együttműködve integrált Datadoggal-megoldást hoz létre az Azure-ban. Ez a megoldás az Azure Marketplace-en keresztül érhető el, és zökkenőmentesen használhatja az Azure-ügyfeleket a Datadoggal felhőalapú figyelési megoldásának használatára.

A megoldással kapcsolatos további információkért tekintse meg a [Azure monitor dokumentációt](/azure/azure-monitor/platform/partners#datadog) , és regisztráljon a nyilvános előzetes verzióra.

## <a name="next-steps"></a>Következő lépések

- [Azure Marketplace online áruház](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: Azure-fiók létrehozása](/learn/modules/create-an-azure-account/)
