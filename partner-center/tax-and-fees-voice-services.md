---
title: Regionális PSTN szolgáltatási adók és díjak
description: Ha Office 365-partnerként Microsoft 365 Voice-termékeket, a PSTN-szolgáltatásokra vonatkozó regionális adó-, díj- vagy szabályozási követelmények vonatkozhatnak Rá.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80cb5503323f483c13c983375559baf70f9d0b6f
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854723"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Regionális adók, a nyilvános telefonhálózat (PTSN) szolgáltatásaira vonatkozó szabályozások

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználói rendszergazdai | Rendszergazdai ügynök

Egyes joghatóságok nyilvános telefonhálózati (PSTN) szolgáltatásaira speciális adózási és szabályozási követelmények vonatkozhatnak, amelyek befolyásolhatják a partnerrendelést és a számlázást. A Egyesült Államok, beleértve a AudioConferencinget, a hívási csomagokat és a kommunikációs krediteket is magában foglaló PsTN-szolgáltatásokat, speciális adózási és szabályozási követelmények vonatkoznak rá. A Egyesült Államok És a Microsoft a PSTN-szolgáltatásokat adóval integráltként áraz.  Az egyedi PSTN-adók és -szabályozások hatással lesznek az Office 365-partnerekre, akik hangalapú Microsoft 365 tranzakciót.  Ha egy partner egy Microsoft PSTN-szolgáltatás árát jelöli meg, akkor az ő felelőssége lehet a PSTN-adók és -díjak kiszámítása és átutalása.

## <a name="partner-recommendations"></a>Partneri javaslatok

Lépjen kapcsolatba adó- és jogi tanácsadói szolgálatával, hogy átlássa a szervezet a PSTN-szolgáltatások szabályozásával, adókkal és díjakkal kapcsolatos felelősségét, valamint az egyéb lehetséges problémákat.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Számla bemutatása és partner egyeztetési fájlja

A CsP-számlák és a CSP egyeztetési fájljai a Egyesült Államok, a Címtár Címtárban és Kanadában, amelyek tartalmazzák a Skype Vállalati verzió PSTN-ját és a Microsoft 365 Voice-szolgáltatásokat, külön sorelemeket biztosítanak a PSTN és a nem PSTN összetevők számára.

Emellett a CSP-számlák a következő lábjegyzetet jelenítik meg:

* A megjelenő ár a hangkonferencia és a hívó csomagszolgáltatások díjának számítható fel.  A vonatkozó tranzakciós adókat kizárólag a feltüntetett összeg alapján számoljuk fel, kivéve a Egyesült Államok.  Az Egyesült Államokban a megjelenített ár az adót is magában foglalja, mivel tartalmazza a hívó csomag és az audiokonferencia szolgáltatás díját, valamint a díjakat és díjakat.  Az audiokonferencia és a hívási csomag szolgáltatásainak kiszolgálását a Microsoft társvállalata biztosítja.  A részleteket a [Microsoft mennyiségi licencelése](https://go.microsoft.com/fwlink/?LinkId=690247) című témakörben találja.

## <a name="reconciliation-file-example"></a>Egyeztetési fájl – példa

Az Office 365 Nagyvállalati E5 verzió két sorelemként mutatja be az egyeztetési fájlt azonos névvel és azonos azonosítóval, de minden sorelem egyedi egységárral rendelkezik (például: 28,40 usd és 2,00 USD). Ez elkülöníti az Office 365-ajánlat Skype Vállalati verzió PSTN-konferencia összetevőjét, így megfelelően alkalmazhatja az adókat.

**Partneregyeztetési példa #1 (oszlopok kiválasztása):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5 csomag   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Ciklus díja   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5 csomag   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Ciklus díja   |2.00   |

**Partner egyeztetési példa #2**

Microsoft 365 Kanadában elérhető business Voice további, a PSTN-hez kapcsolódó, a CSP-számlán összevont összetevőket tartalmaz (az Office 365 E5-höz hasonlóan két sorelemet mutat be, egyet a PSTN-összetevőkhöz, egyet pedig a nem PSTN-összetevőkhöz).  A Microsoft 365 Business Voice CSP egyeztetési fájlja egyenként megjeleníti az összes PSTN-hez használható összetevőt (az egyes PSTN-összetevők nem lesznek egyesülve a-ban. CSV vagy API-eszköz).  Az egyeztetési fájlban található ügyfelek megrendelési részleteinek és számlázott összegének összege megegyezik a CSP-számlával.

## <a name="additional-resources"></a>További források
További részletekért látogasson el a [partnereknek Microsoft 365 webhelyére.](https://www.microsoft.com/microsoft-365/partners/)

