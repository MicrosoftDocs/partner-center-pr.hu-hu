---
title: Regionális PSTN-szolgáltatási adók és díjak
description: Olyan Office 365-partnerként, aki Microsoft 365 hanganyagokat dolgoz fel, a PSTN-szolgáltatásokra vonatkozó regionális adók, díjak vagy szabályozási követelmények vonatkozhatnak rájuk.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 411932923e6bd35732e64521abe567f40f7499e9
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441489"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Regionális adók, nyilvános kapcsolású telefonos hálózati (PTSN) szolgáltatások szabályai

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói rendszergazda
- Felügyeleti ügynök

Bizonyos illetékességi területeken a nyilvános kapcsolású telefonos hálózati (PSTN) szolgáltatások olyan speciális adózási és szabályozási követelmények alá esnek, amelyek befolyásolhatják a partnerek sorrendjét és a számlázást. A Egyesült Államok, beleértve a Puerto Rico-t, a PSTN-szolgáltatásokat, például a hangkonferenciákat, a Meghívási terveket és a kommunikációs krediteket, a speciális adózási és szabályozási követelmények hatálya alá esnek. A Egyesült Államok és a Puerto Rico-ban a Microsoft a PSTN-szolgáltatásokat ÁFA-ként számítja fel.  Az egyedi PSTN-adók és-szabályozások hatással vannak az Office 365-partnerek által Microsoft 365 hangalapú termékekre.  Ha egy partner egy Microsoft PSTN-szolgáltatás árát jelzi, akkor a PSTN-adók és-díjak kiszámításához és az azokhoz való átutaláshoz felelősek lehetnek.

## <a name="partner-recommendations"></a>Partneri javaslatok

Az adó-és jogi tanácsadással tisztában lehet azzal, hogy a szervezet felelőssége a PSTN-szolgáltatások szabályozására, az adókra és a díjakra, valamint az egyéb lehetséges kötelezettségekre vonatkozik.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Számla bemutatási és partneri egyeztetési fájlja

A CSP-számlák és a CSP-egyeztetési fájlok a Egyesült Államokban, Puerto Ricoban és Kanadában, beleértve a Skype for Business PSTN-t és a Microsoft 365 hangszolgáltatásokat, külön vonalakat biztosítanak a PSTN-és a nem PSTN-összetevőkhöz.

A CSP-számlák emellett a következő lábjegyzetet is megjelenítik:

* A megjelenő díj a hangkonferencia díja, és a meghívott csomag szolgáltatásai.  A kapcsolódó tranzakciós adókat kizárólag a Egyesült Államokon belüli értékesítések után számítjuk fel.  Az USA-ban a megjelenő ár az adó, mivel a meghívót és a hangkonferencia-szolgáltatásokat is felszámítja, valamint a díjköteles adókat és díjakat.  A hangkonferencia és a Calling Plan Services szolgáltatást a Microsoft affiliate biztosítja.  A részleteket a [Microsoft mennyiségi licencelése](https://go.microsoft.com/fwlink/?LinkId=690247) című témakörben találja.

## <a name="reconciliation-file-example"></a>Példa egyeztetési fájlra

Az Office 365 Enterprise E5 az egyeztetési fájlban két, azonos nevű és azonos azonosítóval rendelkező sort jelenít meg, de minden egyes sorban egyedi egységár szerepel (például: $28,40 és $2,00). Ez elválasztja az Office 365-ajánlat Skype for Business PSTN-konferenciájának összetevőjét, így az adókat is megfelelően alkalmazhatja.

**Partneri egyeztetési példa #1 (oszlopok kiválasztása):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086 – a3a3b506fac2   |Office 365 Enterprise E5 csomag   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Ciklus díja   |28,40   |
|a044b16a-1861-4308-8086 – a3a3b506fac2   |Office 365 Enterprise E5 csomag   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Ciklus díja   |2.00   |

**Partneri egyeztetési példa #2**

A Kanadában elérhető Microsoft 365 Vállalati verzió-hang további PSTN-alapú adóköteles összetevőket tartalmaz, amelyek konszolidálva vannak a CSP-számlán (az Office 365 E5-hez hasonlóan, két sor elem jelenik meg, egyet a PSTN-összetevőkhöz, a másikat a nem PSTN-összetevőkhöz).  Microsoft 365 Vállalati verzió hanghoz tartozó CSP-egyeztetési fájl megjeleníti az összes PSTN-beli adóköteles összetevőt egyenként (az egyéni PSTN-összetevőket nem fogja összevonni a alkalmazásban. CSV vagy API-eszköz).  Az egyeztetési fájlban talált ügyfelekhez tartozó rendelési részletek és számlázott összegek összegzése megegyezik a CSP-számlával.

## <a name="additional-resources"></a>További források
További részletekért látogasson el a [Microsoft 365 for Partners](https://www.microsoft.com/microsoft-365/partners/) webhelyre.

