---
title: Fizetés a Partnerközpont
description: Ismerje meg a Microsoft-partnerként kapott bevételekkel kapcsolatos kifizetéseket, például a kereskedelmi piactéri ajánlatokon, az ösztönzőprogramokon és a Felhőszolgáltató keresztül. Tartalmazza a kifizetési szabályzatot, a kifizetési hold állapotát és a kifizetési kimutatásokat.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 3dc8b728ef20da77b9a6d2a925ebb0388ea53837
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146493"
---
# <a name="getting-paid-in-partner-center"></a>Fizetés a Partnerközpont

**Megfelelő szerepkörök:** Fiók-rendszergazdai | Globális rendszergazda

Ez a cikk fontos információkat tartalmaz az ajánlatok, bővítmények és a bevételek meghirdetése kifizetésének fogadására. Összegzi a kifizetési szabályzatot, a kifizetés előtt szükséges lépéseket és a kifizetési kimutatás áttekintését.

## <a name="payout-policies-and-agreements"></a>Kifizetési szabályzatok és szerződések

A fizetéshez meg kell felelnie a szerződéseknek és a kifizetési szabályzatnak.

- [Microsoft Azure Marketplace Közzétevői szerződés:](/legal/marketplace/msft-publisher-agreement)A fizetés előtt el kell fogadnia ezt a közzétevői szerződést. Ez a szerződés ismerteti az Ön és a Microsoft közötti kapcsolatot, mivel az a kereskedelmi piactéren elérhető értékesítői ajánlatokra vonatkozik, beleértve a Microsoft által az egyes eladásokért fizetendő áruházi díjat is.
- [A kifizetési szabályzat](payout-policy-details.md) megjeleníti a kifizetési szabályzatokat, beleértve a fizetési ütemezést és a fizetési módokat. A Policy az ügyfelek nem fizetésének folyamatát is ismerteti.
- [Az adó részletei](tax-details-marketplace.md) a Microsoft Közzétevői Szerződés alapján kiválasztott ár és adófizetés adózási [szempontját ismertetik.](/legal/marketplace/msft-publisher-agreement)
- **Az áruházi** díjakat a közzétevői szerződés hivatalosan határozza meg. Az áruházi díj a kereskedelmi piactér által gyűjtött összes ajánlatértékesítésre vonatkozik, beleértve a bővítményeket is.
- **A** kifizetések havonta történikek (feltéve, hogy a fizetési küszöbérték teljesült). Általában az adott hónap 15. napja szerint küldjük el az esedékes kifizetéseket. A kifizetések általában 3–10 további munkanapot venek fel a kifizetési fiók eléréséhez. Részletekért lásd: [Fizetési küszöbértékek, módszerek és időkeretek.](payment-thresholds-methods-timeframes.md)

## <a name="prerequisite-steps-before-getting-paid"></a>A fizetést megelőző előfeltételek

Az első fizetés előtt be kell állítania a kifizetési fiókját, és ki kell kitöltötte a szükséges banki és adózási űrlapokat. A banki és adó űrlapokon meg kell adnia az előnyben részesített fizetési módokat és a visszatartott adó adózási űrlapját. Bank- és adóbevallási űrlapokra van szükség a fizetéshez. Részletekért lásd a kifizetési számla és az adó űrlapok [beállítását.](set-up-your-payout-account.md)

### <a name="payout-hold-status"></a>Kifizetési hold állapota

Alapértelmezés szerint havonta küldünk kifizetéseket a fent leírtak szerint. Egy program kifizetései azonban fel is függedtetheti, és a Microsoft nem fogja kiadni a kifizetéseket az Ön fiókjához. Ha úgy dönt, hogy a kifizetéseket visszatartja, továbbra is rögzítjük a bevételeket a **Kifizetések lapon.** Addig azonban nem küldünk kifizetéseket a fiókjába, amíg el nem távolítja a visszatartott fizetést.

A kifizetéseket a jobb  felső sarokban lévő Beállítások fogaskerék ikonnal, majd a Fiókbeállítások menüben helyezze **el.** A **bal oldali menüben** válassza a  Kifizetés és adó elemet, majd a Kifizetési és adóprofil-hozzárendelés szakaszban keresse meg azt a programot, amelynek kifizetését el szeretné tartani. Jelölje be **a Fizetésem visszatartása** jelölőnégyzetet a program kifizetésének a kifizetésének a kifizetéseként. A kifizetési hold állapot bármikor megváltoztatható, de a döntés a következő havi kifizetésre is hatással lesz. Ha például áprilisi kifizetéseket szeretne megtartani, ügyeljen arra, hogy a kifizetési hold állapota Legyen **Be,** mielőtt március vége lenne.

Miután beállította a kifizetési hold állapot be van **kapcsolva,** a program összes kifizetése fel lesz függve, amíg nem törli a jelölőnégyzetet Ki **állapotra.** Ha így történik, a következő havi kifizetési ciklusban szerepelni fog (feltéve, hogy a fizetési küszöbérték teljesült). Ha a kifizetései fel vannak függve, de júniusban szeretne generálni egy kifizetést, akkor május vége előtt törölje a Kikapcsolva jelölőnégyzetet. 

>[!Note]
> A Kifizetési hold állapot minden programra külön vonatkozik (Microsoft Store, reklám, Azure Marketplace stb.). Ha az összes program kifizetését szeretné megtartani, minden program kifizetését külön-külön kell visszatartanunk.

## <a name="payout-statements"></a>Kifizetési utasítások

A kifizetési kimutatás az ajánlatokból és a tranzakcióelőzmények bővítményeiből származó bevételeket jeleníti meg. Megtekintheti a fizetési adatokat, és letöltheti a jelentéseket tsv vagy CSV formátumban. A [kifizetési kimutatások](payout-statement.md) elérésével, valamint a tranzakciós előzmények és a kifizetési jelentések részleteivel kapcsolatos további információkért lásd: Kifizetési kimutatások. Emellett a [Partner Payouts API-val](https://apidocs.microsoft.com/services/partnerpayouts) szisztematikus módon leküldheti a kifizetési jelentéseket.

## <a name="next-steps"></a>Következő lépések

- [Partner Payouts API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Kifizetések – GYIK](payout-faq.md)