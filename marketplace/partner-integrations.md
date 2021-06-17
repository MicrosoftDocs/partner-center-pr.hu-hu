---
title: Azure Marketplace-partnerintegrációk
description: Ismerje meg Azure Marketplace Azure-környezettel integrálható megoldásokat, és hivatkozásokat talál a Microsoft-partnerektől származó üzembe helyezési útmutatókra.
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: 56e72af367cdcb264cc444446c5fcbedcd880451
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276484"
---
# <a name="azure-marketplace-partner-integrations"></a>Azure Marketplace-partnerintegrációk

Megtudhatja, hogyan integrálhatja a partnermegoldásokat az Azure-környezetbe. Ez a cikk áttekintést nyújt az egyes megoldásokról, és részletes üzembe helyezési útmutatókra mutató hivatkozásokat tartalmaz. A megoldások betűrendben vannak felsorolva. 

## <a name="apache-kafka-on-confluent-cloud"></a>Apache Kafka a Confluent Cloudon

![Confluent Cloud.](./media/partners/confluent-cloud.png)

Az Azure lehetővé teszi a Confluent Cloud integrálását a felhőalkalmazások mellett. A confluent ügyfelek gyakran navigálnak a Azure Portal és a Confluent Cloud között. Ha például egy felhasználó megvásárol egy Confluent Cloud-ajánlatot az Azure Marketplace-ban, be kell állítania egy fiókot a Confluent Cloudhoz. Ez a folyamat növeli az összetettséget és az időt, és megköveteli a felhasználóktól a konfiguráció és az erőforrások kezelését a két portál között. A Több platformon való felügyelet terhének csökkentése érdekében a Microsoft a Confluent Cloudgal együttműködésben egy integrált kiépítési réteget épített ki az Azure-ból a Confluent Cloudba. A megoldás elérhető a Azure Marketplace, és zökkenőmentes felhasználói élményt nyújt a Confluent Cloud ajánlat azure-beli használatában

A megoldás egy, az Azure-ban engedélyezett erőforrás-szolgáltatót használ a Confluent Cloud-erőforrások kiépítése érdekében. Ez lehetővé teszi a felhasználók számára a valós idejű eseménystreamelést a Azure Portal, az Azure CLI-n és az Azure SDK-n keresztül. A Confluent Cloud tulajdonában van és futtatja az SaaS-alkalmazást, amely környezeteket, fürteket, témaköröket, API-kulcsokat és felügyelt összekötőket tartalmaz.

A Confluent Cloud mély integrációja a következő képességeket teszi lehetővé:

- Új Confluent Cloud szervezeti erőforrás üzembe Azure Portal teljes mértékben felügyelt infrastruktúrával.
- Az Azure-ból a Confluent Cloudba való egyszeri bejelentkezés zökkenőmentessé Azure Active Directory; nincs szükség külön hitelesítésre a Confluent Cloud portálról.
- A Confluent Cloud fogyasztási díjának egységes számlázása az Azure-előfizetés számlázásán keresztül.
- A Confluent Cloud-erőforrásokat a Azure Portal kezelheti,  és az Azure-erőforrások mellett az Összes erőforrás lapon is nyomon követheti őket.

[Confluent Cloud üzembe helyezési útmutatók](https://docs.confluent.io/current/cloud/marketplace/index.html)

A Confluent on Azure-ral kapcsolatos problémákat itt talál: [https://support.confluent.io](https://support.confluent.io) . Ha Ön első felhasználó, állítsa alaphelyzetbe a jelszavát, mielőtt bejelentkezik a Confluent támogatási portálra. Ha nincs Confluent-fiókja, küldjön egy e-mailt a [cloud-support@confluent.io](mailto:cloud-support@confluent.io) címre.

## <a name="datadog"></a>Datadog

![DataDog embléma.](./media/partners/datadog.png)

A Datadog megfigyelhetőséget és biztonsági eszközöket biztosít az Azure-felhasználók számára, hogy megértsék az alkalmazások állapotát és teljesítményét a hibrid és többfelhős környezetekben. A szükséges integrációk konfigurálásához azonban gyakran a Azure Portal a Datadog között kell navigálni. A portálok közötti konfiguráció és erőforrás-kezelés egyszerűsítése érdekében a Microsoft a Datadoggal együtt létrehozott egy integrált Datadog-megoldást az Azure-ban. A portálon Azure Marketplace megoldás zökkenőmentes felhasználói élményt nyújt az Azure-ügyfelek számára a Datadog felhőalapú monitorozási megoldásának használatára.

A [megoldással Azure Monitor és](/azure/azure-monitor/platform/partners#datadog) a nyilvános előzetes verzióra való regisztrációval kapcsolatos további információkért tekintse meg az Azure Monitor dokumentációját.

## <a name="next-steps"></a>Következő lépések

- [Azure Marketplace online áruház](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: Azure-fiók létrehozása](/learn/modules/create-an-azure-account/)
