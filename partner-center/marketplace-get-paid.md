---
title: Fizetés fogadása a kereskedelmi piactéren
description: Ismerje meg, hogyan fogadhat fizetéseket a kereskedelmi piactéren az Azure Marketplace-en. Tartalmazza a kifizetési szabályzatot, a kifizetéssel kapcsolatos állapotot és a kifizetési utasításokat.
ms.service: marketplace
ms.topic: conceptual
ms.date: 09/28/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 61730eec204674d7ad095d1fffcd997f65d135ea
ms.sourcegitcommit: 7f595faf952bf2d6cdc229da38bd67ee701b2083
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/02/2020
ms.locfileid: "93189730"
---
# <a name="getting-paid-in-the-commercial-marketplace"></a>Fizetés fogadása a kereskedelmi piactéren

Ez a cikk fontos információkat nyújt az ajánlatok, a bővítmények és a hirdetési bevételek fizetésének fogadásáról. Összefoglalja a kifizetési szabályzatot, a befizetéshez szükséges lépéseket, valamint a kifizetési utasítások áttekintését.

## <a name="commercial-marketplace-payout-policies-and-agreements"></a>Kereskedelmi Marketplace kifizetési szabályzatok és szerződések

A fizetés megkezdéséhez meg kell felelnie a szerződéseknek és a kifizetési szabályzatnak.

- [Microsoft Azure Marketplace kiadói szerződés](https://go.microsoft.com/fwlink/p/?LinkID=699560): a befizetésük előtt el kell fogadnia ezt a közzétevői szerződést. Ez a szerződés az Ön és a Microsoft közötti, a kereskedelmi piactéren található értékesítői ajánlatokra vonatkozó kapcsolatot ismerteti.
- A kifizetési szabályzat a kifizetési határidőket, például a fizetési ütemtervet és a fizetési [módszereket mutatja.](payout-policy-details.md) A szabályzat emellett ismerteti az ügyfelek nem teljesített fizetési folyamatát is.
- Az [adózás részletei](tax-details-marketplace.md) a Microsoft [kiadói szerződés](https://go.microsoft.com/fwlink/p/?LinkID=699560)keretében a díjak kiválasztására és az adózásra vonatkozó adózási szempontokat ismertetik.
- A **tárolási díjakat** a kiadói szerződésben hivatalosan definiáljuk. Az áruházi díjat a kereskedelmi piactér által gyűjtött összes ajánlati értékesítésre, beleértve a bővítményeket is.
- A **fizetések** havi rendszerességgel történnek (amennyiben a fizetési küszöbérték teljesült). Általában a hónap 15. napján egy adott hónapban esedékes fizetést küldünk. A kifizetések általában 3 – 10 további munkanapot vesznek igénybe a kifizetési fiók eléréséhez. Részletekért lásd: [fizetési küszöbértékek, metódusok és időbeli keretek](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Előfeltételként szükséges lépések a beszerzés előtt

Az első befizetést megelőzően be kell állítania a kifizetési fiókját, és el kell végeznie a szükséges banki és adózási űrlapok beszerzését. A bank és az adó űrlapokon az előnyben részesített fizetési módokat és a forrásadót adó űrlapokat kell megadnia. A bank és az adó űrlapokra azért van szükség, hogy fizessen Önnek. Részletekért lásd: [a kifizetési fiók és az adózási űrlapok beállítása](set-up-your-payout-account.md).

### <a name="payout-hold-status"></a>Kifizetés holdjának állapota

Alapértelmezés szerint a fentiekben leírtak szerint havi rendszerességgel küldjük el a kifizetéseket. Lehetősége van azonban arra is, hogy a kifizetéseit egy megtartott programba helyezi el, és a Microsoft nem szabadítja fel a számláján befizetett összegeket. Ha úgy dönt, hogy megtartja a befizetését, a **nyeremények** oldalon továbbra is rögzítjük a bevételt. Azonban addig nem küldünk fizetést a fiókjába, amíg el nem távolítja a tárolót.

A befizetések tárolásához kattintson a jobb felső sarokban található **Beállítások** fogaskerék ikonra, majd a **fejlesztői beállítások** elemre. Válassza ki a **kifizetés és az adó** lehetőséget a bal oldali menüben, és a **kifizetési és adózási profil hozzárendelése** szakaszban keresse meg azt a programot, amelyhez a kifizetéseket tárolni szeretné. Jelölje be a **fizetés megtartása** jelölőnégyzetet a programhoz tartozó fizetések tárolásához. Bármikor módosíthatja a kifizetési állapotot, de a döntés a következő havi kifizetésre is hatással lesz. Ha például a április végét szeretné megtartani, mindenképpen **a március vége előtt állítsa** be a kifizetési Holding állapotát.

Miután beállította a kifizetés állapotát **a be** értékre, a program összes kifizetése megmarad **, amíg** be nem törli a jelölőnégyzetet. Ha így tesz, a következő havi kifizetési ciklusban fog szerepelni (ha a fizetési küszöbérték teljesült). Ha már megtartotta a befizetését, de a júniusi kifizetést is **ki** szeretné állítani, akkor törölje a jelet a jelölőnégyzetből a május vége előtt.

>[!Note]
> A kifizetési Holding-állapot minden egyes programra külön vonatkozik (Microsoft Store, reklám, Azure Marketplace stb.). Ha meg szeretné tartani az összes programhoz való kifizetést, akkor a fizetést külön kell megfizetnie.

## <a name="payout-statements"></a>Kifizetési utasítások

A kifizetési utasítás a tranzakciók előzményeiben az ajánlatok és a bővítmények értékesítéséből származó bevételt jeleníti meg. A fizetési adatokat és a jelentések letöltését TSV vagy CSV formátumban is megtekintheti. A kifizetési [utasításokkal](payout-statement.md) kapcsolatos további információkért tekintse meg a kifizetés utasításait, valamint a tranzakciós előzmények és fizetési jelentések részleteit. Emellett a [partner kifizetések API](https://apidocs.microsoft.com/services/partnerpayouts) -val is használhatja a kifizetési jelentések szisztematikus lekérését.

## <a name="next-steps"></a>Következő lépések

- [Partneri kifizetések API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Marketplace-kifizetések – gyakori kérdések](payout-faq.md)
