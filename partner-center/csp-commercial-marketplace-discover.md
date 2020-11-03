---
title: Ajánlatok felderítése – kereskedelmi piactér
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy a CSP-partnerek hogyan használhatják a partner centert a piactéren az SaaS-ajánlatok vagy a független szoftvergyártók (ISV-EK) díjszabásának megtekintéséhez vagy kereséséhez.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cb7b4ffdb4edf75e3e121e4ddea6b9de191ddbbf
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529964"
---
# <a name="discover-offers-and-pricing-in-the-partner-center-commercial-marketplace"></a>Ajánlatok és díjszabások felderítése a partner Center kereskedelmi piactéren

**A következőkre vonatkozik**

- Partnerközpont
- Partnerek a CSP programban

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felügyeleti ügynök

Ha a független szoftvergyártók (ISV-ket) úgy döntenek, hogy közzétesznek egy ajánlatot a kereskedelmi piactéren, dönthetnek arról is, hogy az ajánlatot elérhetővé kívánják-e tenni a CSP programban. Ha úgy dönt, hogy eladja az ajánlatot a CSP programon keresztül, a CSP-partnereknek az ajánlatot a partner Center Marketplace területen kell látniuk.

Ha egy ISV-ajánlat nem jelenik meg a partneri központban várt módon, az a következők miatt fordulhat elő:

- Az ISV úgy döntött, hogy nem értékesíti az ajánlatot a CSP programon keresztül. Előfordulhat például, hogy egyes ISV-termékek elérhetővé válnak a kereskedelmi piactér más területein (például [Microsoft AppSource](https://appsource.microsoft.com/) és az [Azure Marketplace](https://azuremarketplace.microsoft.com/)-en), de nem jelennek meg a partnervállalat számára a partner Center piactéren.

- Az ISV úgy döntött, hogy az ajánlatot kizárólag kiválasztott számú CSP-partnernek teszi ki. Az exkluzív ajánlatokról további információt a jelen témakör későbbi, című szakaszában talál.

- Előfordulhat, hogy az ajánlat típusa nem hívható meg a partnervállalat vagy a Azure Portal (például tárolók vagy valamilyen használaton alapuló ajánlatok) segítségével.

- Előfordulhat, hogy a társított ügyfél (ek) számlázási országa nem támogatott ezen az ISV-ajánlaton.

## <a name="view-marketplace-offers-in-partner-center"></a>Piactéri ajánlatok megtekintése a partner Centerben

Az elérhető kereskedelmi Piactéri ajánlatok megtekintése a CSP programban: 

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard), majd a bal oldali navigációs menüben válassza a **CSP** elemet.

2. Válassza az **értékesítés** , majd a **piactér** elemet. Alapértelmezés szerint minden típusú és kategóriájú terméket látni fog.

3. Válasszon egy szűrőt típus vagy kategória alapján. A **kereséssel** konkrét kulcsszavakat, ajánlat-NEVEKET vagy ISV-közzétevők nevét is megkeresheti.

4. Válasszon ki egy adott terméket a listából. Ekkor megjelenik a Product Overview (termék áttekintése) lap, ahol többet is megtudhat az ajánlatról. Az ezen a lapon található információk a következők lehetnek: 

    - A termék vagy ajánlat leírása

    - További információ az ISV-közzétevőről

    - Az ISV-közzétevő által feltöltött dokumentációra vagy marketinganyagokra mutató hivatkozások

    - Egyéb lehetséges ISV-kapcsolatok az ügyfélszolgálathoz, a mérnöki tevékenységhez vagy a CSP-programhoz való kapcsolattartáshoz

5. Ha többet szeretne megtudni az ajánlat rendelkezésre álló csomagjairól, SKU-ról vagy díjszabásáról, válassza a **csomagok + díjszabás** lapot. Ezen a lapon a következő jelenik meg:

    - Azok a piacok, amelyeken elérhető az ajánlat

    - Az ajánlathoz elérhető SKU-i vagy csomagok listája

    - Az egyes SKU-vagy díjcsomag díjszabása

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Piactéri ajánlatok megtekintése a partner Center API-kon keresztül

A CSP program partnerei API-kat is használhatnak a jogosult ajánlatok listájának visszaküldéséhez. A jogosult ajánlatok csak azokra a SaaS ISV-ajánlatokra lesznek elérhetők, amelyek a partner Center Piactéren keresztül értékesíthetők. A katalógusban található ajánlatok azonosítására szolgáló API-kat használó partnereink számára tekintse meg az útmutatót, amely a [piacon elérhető ajánlatok listáját tartalmazza](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Tekintse meg a piactér legújabb ajánlatának díjszabását a partner Centerben

Az ajánlatokkal kapcsolatos legújabb díjszabási részletekért kövesse az alábbi lépéseket:

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard), majd a bal oldali navigációs menüben válassza a **CSP** elemet.

2. Válassza az **értékesítés** lehetőséget, majd a **díjszabást és az ajánlatokat** .

3. Görgessen le a **piactér** szakaszhoz, válasszon egy helyet, és töltse le a **piactér díjszabását** . Ez létrehoz egy táblázatot a SaaS-közzétevők által biztosított, a legújabb díjszabási adatokkal. Néhány Azure-alkalmazás díjszabása is itt jelenhet meg. A rendszer naponta frissíti ezeket az információkat, így a választott gyakorisággal a jelenlegi árakon is megtekintheti.

4. Ha egy ISV-termék ingyenes próbaidőszakot tartalmaz, a táblázat két sort fog megjeleníteni a termékhez:

    - Az egyik sor a nulla ingyenes próba árát mutatja. Ez azt jelenti, hogy az ingyenes próbaidőszak elérhető.

    - A másik sor az ingyenes próbaidőszak lejárta után alkalmazandó árat és feltételeket mutatja.

A CSP program partnereként jogosult lehet az egyes kereskedelmi Piactéri ajánlatokhoz kapcsolódó egyéb ösztönzőkre. További információ az egyéb ösztönzőkről: CSP- [ösztönző útmutató](https://aka.ms/partnerincentives) (CSP-bejelentkezést igényel).

## <a name="learn-about-marketplace-exclusive-offers"></a>Ismerje meg a Marketplace exkluzív ajánlatait

Az ISV-ket lehetőségük van arra, hogy az ajánlatait csak bizonyos partnereknek lehessen elérhetővé tenni a CSP programban. Ezt exkluzív ajánlatnak nevezzük. A CSP program összes partnere továbbra is megtekintheti a partner Center kereskedelmi piactéren található összes ISV-ajánlatot, beleértve az exkluzív jelölésű ajánlatokat is.

Ha egy ajánlat **nem** kizárólagos jelölésű, az összes partner megvásárolhatja az ajánlatot (feltéve, hogy a kiválasztott ügyfél számlázási országa megfelel az ISV-k ajánlatának országa számára elérhetőnek).

Az exkluzív jelölésű ajánlatok esetében azonban csak az ISV által kiválasztott partnerek vásárolhatják meg az ajánlatot.

> [!NOTE]
> Ha olyan exkluzív ajánlat jelenik meg, amelyet szeretne értékesíteni az ügyfeleknek, forduljon közvetlenül az ISV-hoz, és kérjen engedélyt az exkluzív ajánlat eladására. Ha megtekinti egy exkluzív ajánlat részleteit, megjelenhet egy **partneri ISV** -hivatkozás, amelyet kiválaszthat.

Ha többet szeretne megtudni a kereskedelmi piactéren található ISV-ról, olvassa el a [Cloud Solution Providers szolgáltatást](/azure/marketplace/cloud-solution-providers).

A piactéren elérhető CSP-vel kapcsolatos további információkért olvassa el a [kereskedelmi piactér – áttekintés](csp-commercial-marketplace-overview.md)című témakört.

## <a name="next-steps"></a>Következő lépések

- [Kereskedelmi Piactéri ajánlatok vásárlása](csp-commercial-marketplace-purchase.md)