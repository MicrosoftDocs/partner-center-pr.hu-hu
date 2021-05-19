---
title: Ajánlatok felderítése – kereskedelmi piactér
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan használhatja a CSP Partnerközpont a független szoftverszállítóktól származó SaaS-ajánlatokat vagy díjszabást a piactéren.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147972"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Ajánlatok és díjszabás a kereskedelmi Partnerközpont piactéren

**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök

Amikor a független szoftverszállítók (ISV-k) úgy döntenek, hogy közzétesznek egy ajánlatot a kereskedelmi piactéren, azt is eldöntik, hogy szeretnék-e elérhetővé tenni az ajánlatot a CSP-programban. Ha úgy döntenek, hogy az ajánlatot a CSP-programon keresztül értékesítik, a CSP-partnereknek a Marketplace Partnerközpont kell látniuk.

Ha egy ISV-ajánlat nem a várt Partnerközpont jelenik meg, annak a következő lehet az oka:

- Az ISV úgy döntött, hogy nem adja el az ajánlatot a CSP-programon keresztül. Előfordulhat például, hogy egyes ISV-termékek elérhetők a kereskedelmi piactér más területein (például az [Microsoft AppSource-ban](https://appsource.microsoft.com/) és Azure Marketplace-ban), [](https://azuremarketplace.microsoft.com/)de nem biztos, hogy megjelennek a CSP-programban részt Partnerközpont partnerek számára.

- Az ISV úgy döntött, hogy az ajánlatot csak néhány CSP-partner számára teszi kizárólagosként. Az exkluzív ajánlatokkal kapcsolatos további információkért tekintse meg a jelen súgótémakör egy későbbi, későbbi, későbbiekben található témakörét.

- Előfordulhat, hogy az ajánlat típusa nem Partnerközpont vagy Azure Portal (például tárolókon vagy használatalapú ajánlatokon) keresztül.

- Előfordulhat, hogy a társított ügyfél(nek) számlázási országa nem támogatott ehhez az ISV-ajánlathoz.

## <a name="view-marketplace-offers-in-partner-center"></a>Marketplace-ajánlatok megtekintése a Partnerközpont

Az elérhető kereskedelmi piactéri ajánlatok megtekintése a CSP-programban:

1. Jelentkezzen be Partnerközpont [irányítópultra,](https://partner.microsoft.com/dashboard)majd válassza a **CSP lehetőséget** a bal oldali navigációs menüben.

2. Válassza **az Értékesítés,** majd a **Marketplace lehetőséget.** Alapértelmezés szerint minden típusú és kategóriás termék létezik.

3. Válasszon ki egy szűrőt típus vagy kategória alapján. A Search  használatával konkrét kulcsszavakat, ajánlatneveket vagy ISV-közzétevők nevét is megkeresheti.

4. Válasszon ki egy adott termékajánlatot a listából. Ezzel a termék Áttekintés lapját fogja látni, ahol további információt talál az ajánlatról. Az ezen a lapon található információk a következők lehetnek: 

    - A termék vagy ajánlat leírása

    - További információ az ISV-közzétevőről

    - Az ISV-közzétevő által feltöltött dokumentációkra vagy marketinganyagokra mutató hivatkozások

    - Egyéb lehetséges ISV-kapcsolattartók ügyfélszolgálathoz, mérnöki csapathoz vagy a CSP-program kapcsolattartóihoz

5. Az ajánlat elérhető csomagokkal, termékcsomagokkal vagy díjszabásokkal kapcsolatos további információkért válassza a Csomagok **+ díjszabás lapot.** Ezen a lapon a következőt fogja megmutatni:

    - A piacok, ahol ez az ajánlat elérhető az Ön számára

    - Az ajánlathoz elérhető SKUS-k vagy csomagok listája

    - Az elérhető termékváltozatok vagy csomagok díjszabása

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Marketplace-ajánlatok megtekintése Partnerközpont API-kon keresztül

A CSP-programpartnerek API-k használatával is visszaadják a jogosult ajánlatok listáját. A jogosult ajánlatok csak azok az SaaS ISV-ajánlatok lesznek, amelyek a partner számára a piactéren keresztül Partnerközpont lesznek. Azon partnerek számára, akik API-kat használnak az ajánlatok azonosítására a katalógusban, tekintse meg a piaci ajánlatok listáját lekért [útmutatót.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>A Marketplace-ajánlat legfrissebb díjszabását a Partnerközpont

Kövesse az alábbi lépéseket az ajánlathoz tartozó legújabb díjszabási részletekért:

1. Jelentkezzen be Partnerközpont [irányítópultra,](https://partner.microsoft.com/dashboard)majd a bal oldali navigációs menüben válassza a **CSP** lehetőséget.

2. Válassza **az Értékesítés,** majd a **Díjszabás és ajánlatok lehetőséget.**

3. Görgessen le a **Marketplace szakaszhoz,** válasszon egy helyet, és töltse le a **Marketplace díjszabását.** Ez létrehoz egy táblázatot az SaaS legújabb díjszabási adataival, a licencalapú ajánlatokkal és az ISV-közzétevők által elérhető forgalmi díjas ajánlatokkal. Az Azure-alkalmazások bizonyos díjszabása is megjelenhet itt. Ezek az információk naponta frissülnek, így a választott gyakoriséggel ellenőrizheti az aktuális árakat.

4. Ha egy ISV-termék ingyenes próbaidőszakot tartalmaz, a táblázatban két sor jelenik meg a termékhez:

    - Az egyik sorban a nulla ingyenes próbaverziós ár látható. Ez azt jelenti, hogy elérhető egy ingyenes próbaidőszak.

    - A másik sor az ingyenes próbaidőszak után érvényes árat és feltételeket jeleníti meg.

CSP-programpartnerként ön jogosult lehet az egyes kereskedelmi piactéri ajánlatokhoz kapcsolódó egyéb ösztönzőkre. További információt az egyéb ösztönzőkről a [CSP-ösztönző](https://aka.ms/partnerincentives) útmutatóban (CSP-bejelentkezés szükséges).

## <a name="learn-about-marketplace-exclusive-offers"></a>További információ a piactér kizárólagos ajánlatokkal kapcsolatban

Az isV-knek lehetősége van arra, hogy ajánlatukat csak a CSP-program meghatározott partnerei számára ttsdék elérhetővé. Ezt kizárólagos ajánlatnak nevezik. A CSP-programban minden partner továbbra is megtekintheti az összes isV-ajánlatot Partnerközpont kereskedelmi piactéren, beleértve az Exclusive (Kizárólagos) jelölésű ajánlatokat is.

Ha egy ajánlat **nem** kizárólagosként van megjelölve, minden partner megvásárolhatja az ajánlatot (feltéve, hogy a kiválasztott ügyfél számlázási országa megegyezik az ISV-ajánlat országának elérhetőségével).

Az Exclusive (Kizárólagos) jelölésű ajánlatok esetén azonban csak az ISV által kiválasztott partnerek vásárolhatják meg az ajánlatot.

> [!NOTE]
> Ha egy Exclusive (Kizárólagos) jelzésű ajánlatot lát, amit szeretne értékesíteni az ügyfeleinek, közvetlenül a isv-vel kapcsolatba kell kérnie a isv-t, és engedélyt kell kérnie az Exclusive ajánlat értékesítésére. Amikor megtekinti az Exclusive (Kizárólagos) ajánlat részleteit, előfordulhat, hogy használhatja a Contact ISV (Kapcsolatfelvétel **az ISV-vel)** hivatkozást.

A kereskedelmi piactéren elérhető ISV-vel kapcsolatos további információkért olvassa el a [felhőszolgáltatókkal kapcsolatos cikkeket.](/azure/marketplace/cloud-solution-providers)

A piactéren elérhető CSP-felhasználói élményről a kereskedelmi [piactér áttekintésében talál további információt.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Következő lépések

- [Kereskedelmi piactéri ajánlatok vásárlása](csp-commercial-marketplace-purchase.md)