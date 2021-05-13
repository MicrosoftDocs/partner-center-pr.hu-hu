---
title: Credit limit enforcement
ms.topic: how-to
ms.date: 05/11/2021
description: Ismerje meg a kreditkorlátot és annak kiszámítását. Tartalmazza a gyakori kérdéseket.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819380"
---
# <a name="credit-limit-enforcement-cle"></a>Credit limit enforcement (CLE)

**Megfelelő szerepkörök**

- Számlázási adminisztrátor

## <a name="your-credit-limit-and-how-it-works"></a>A kreditkeret és annak működése

A kreditkorlát az a maximális összeg (amerikai dollárban), amit Partnerként elkölthet termékek vagy előfizetések vásárlására a Partnerközpont. Ha túllépi a kreditkeretét, addig nem vásárolhat új vásárlásokat, amíg nem fizet ki elegendő összeget. A meglévő előfizetések továbbra is megszakítás nélkül maradnak.

A kreditkorlátok az Azure-csomag, az Azure Reservations, a Szoftver, a Marketplace, az Azure 145 P, az Office és a Dynamics termékek ajánlataira vonatkoznak. A kreditkorlátok nem vonatkoznak a megújításra és a folyamatos használatra.

A kreditkorlátot a bérlői szinten rendeljük hozzá az előfizetési időszak alatt. Ezt az előre jelzett bevételre, a vásárlási lehetőségekre és a fizetési előzményekre alapozjuk. Ezután a következő képlettel számítjuk ki a rendelkezésre álló egyenleget:

**[Credit Limit – (Bejövő vásárlás + ki nem fizetett számlák + ki nem számlázott díjak – Túlfizetés)]**

## <a name="frequently-asked-questions"></a>Gyakori kérdések

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>A kreditkorlátom a bérlő vagy a globális szinten van beállítva?

A bérlői szint. Tegyük fel például, hogy az Egyesült Államokból, Kanadából és Japánból tevékenykedik. Ha a kanadai bérlő eléri a kreditkorlátját, akkor a bérlő értesítést kap, amikor megpróbál vásárolni a Partnerközpont. A többi bérlőre ez nem lesz hatással. 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a>Ha túllépem a kreditkorlátomat, folytatható a meglévő ügyfelek és előfizetések teljes körű kiszolgálása?

Igen. Az ügyfelek meglévő előfizetései megszakítás nélkül folytatódnak. Azonban nem vásárolhat új előfizetéseket az ügyfelei számára.

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a>Vonatkozik a CLE a közvetlen számlázási partnerekre és a közvetett szolgáltatókra is?

Igen, mindkettőre vonatkozik.

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a>Miután beküldtem a kifizetésemet a fiók visszaállításához, mikor vásárolhatok további előfizetéseket? 

A fizetést követő 24 órán belül folytathatja a vásárlást, feltéve, hogy a Microsoft megkapta a hitelkeret-ellenőrzés folyamatának folytatásához szükséges összes követelményt.

### <a name="how-can-i-check-my-credit-limit"></a>Hogyan tudom ellenőrizni a kreditkorlátomat?

Vegye [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) fel a kapcsolatot a kreditkorlátja és a legutóbbi vásárlások információinak lekért információkért.

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a>A vitatás alatt szereplő számlák beleszámnak a kreditkeretbe?

Igen. A probléma megoldásához azonban kapcsolatba léphet a Microsofttal [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) a következő elérhetőségen: .

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a>Milyen hamar hallok majd, ha a-be írjuk ucmwrcsp@microsoft.com a-t?

Kevesebb mint 24 órán belül választ kell adnunk. 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a>Milyen feltételeket használ a Microsoft egy partner hitelkeretének beállítására?

A kreditkorlátot az előre jelzett bevétel, a vásárlási idő és a kifizetési előzmények alapján határozzuk meg.

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a>A kreditkorlát jelenleg érvényben van az új kereskedelmi felhasználói élményben?

Igen. A kreditkorlátok az összes CSP-programra és termékre érvényesek a Partnerközpont.

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a>Ki kapja meg az értesítést, amikor a szervezetem a kreditkorlátja közeledik?

Az értesítést a szervezet pénzügyi kapcsolattartója kapja meg.

## <a name="next-steps"></a>Következő lépések

[A számlázás alapjai](./billing-basics.md)
