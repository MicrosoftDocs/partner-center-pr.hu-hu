---
title: Kreditkorlát kényszerítve
ms.topic: how-to
ms.date: 05/11/2021
description: Ismerje meg a kreditkorlátot és annak kiszámítását. Tartalmazza a gyakori kérdéseket.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148108"
---
# <a name="credit-limit-enforcement-cle"></a>Kreditkorlát kényszerítési (CLE)

**Megfelelő szerepkörök:** Számlázási rendszergazda

## <a name="your-credit-limit-and-how-it-works"></a>A kreditkeret és annak működése

A kreditkorlát az a maximális összeg (amerikai dollárban), amit partnerként elkölthet termékek vagy előfizetések vásárlására a Partnerközpont. Ha túllépi a kreditkorlátot, addig nem vásárolhat új vásárlásokat, amíg nem fizet ki elegendő összeget. A meglévő előfizetések továbbra is zavartalanul maradnak.

A kreditkorlátok az Azure-csomagra, az Azure Reservationsre, a Szoftverre, a Marketplace-re, az Azure 145 P-re, az Office-re és a Dynamics-termékekre vonatkoznak. A jóváírási korlátok nem vonatkoznak a megújításra és a folyamatos használatra.

A kreditkorlátot a bérlői szinten rendeljük hozzá az előfizetési időszak alatt. Ezt az előre jelzett bevételre, a vásárlási lehetőségekre és a kifizetési előzményekre alapozjuk. Ezután a következő képlettel számítjuk ki a rendelkezésre álló egyenleget:

**[Kreditkorlát – (Bejövő vásárlás + Ki nem fizetett számlák + ki nem számlázott díjak – túlfizetés)]**

## <a name="frequently-asked-questions"></a>Gyakori kérdések

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>A kreditkorlátom a bérlő vagy a globális szinten van beállítva?

A bérlői szint. Tegyük fel például, hogy az Egyesült Államokból, Kanadából és Japánból üzemeltet. Ha a kanadai bérlő eléri a kreditkorlátot, akkor a bérlő értesítést kap, amikor megpróbál vásárolni a Partnerközpont. A többi bérlőre ez nem lesz hatással. 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a>Ha túllépem a kreditkorlátomat, folytatható a meglévő ügyfelek és előfizetések teljes körű kiszolgálása?

Igen. Az ügyfelek meglévő előfizetései megszakítás nélkül folytatódnak. Az ügyfelek számára azonban nem vásárolhat új előfizetéseket.

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a>Vonatkozik a CLE a közvetlen számlázási partnerekre és a közvetett szolgáltatókra is?

Igen, mindkettőre vonatkozik.

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a>Miután beküldtem a kifizetésemet a fiók visszaállításához, mikor vásárolhatok további előfizetéseket? 

A vásárlást a kifizetést követő 24 órán belül folytathatja, feltéve, hogy a Microsoft megkapta a hitelkeret-ellenőrzés folyamatának folytatásához szükséges összes követelményt.

### <a name="how-can-i-check-my-credit-limit"></a>Hogyan tudom ellenőrizni a kreditkorlátomat?

Vegye [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) fel a kapcsolatot a hitelkerete és a legutóbbi vásárlásokkal kapcsolatos információk lekért információkért.

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a>A vitatás alatt szereplő számlák beleszámnak a kreditkeretbe?

Igen. A probléma megoldásához azonban kapcsolatba léphet a Microsofttal [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) a következő elérhetőségen: .

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a>Milyen hamar hallok majd, ha a-be írjuk ucmwrcsp@microsoft.com a-t?

Kevesebb mint 24 órán belül választ kell adnunk. 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a>Milyen feltételeket használ a Microsoft egy partner hitelkeretének beállítására?

A kreditkorlátot az előre jelzett bevétel, a vásárlási lehetőségek és a fizetési előzmények alapján határozzuk meg.

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a>A kreditkorlát jelenleg érvényben van az új kereskedelmi felhasználói élményben?

Igen. A kreditkorlátok az összes CSP-programra és -termékre érvényesek a Partnerközpont.

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a>Ki kapja meg az értesítést, amikor a szervezetem közeledik a kreditkorláthoz?

A szervezet pénzügyi kapcsolattartója megkapja az értesítést.

## <a name="next-steps"></a>Következő lépések

[A számlázás alapjai](./billing-basics.md)
