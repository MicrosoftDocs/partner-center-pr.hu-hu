---
title: A kereskedelmi piactéri termékek számlázása
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan működik a számlázás az ügyfelek számára a kereskedelmi piactéren vásárolt ISV SaaS-termékek vagy -előfizetések esetében a Partnerközpont.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c25d4ab3077c6a0f648c767472e8b7b60ef53a9c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148023"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>A kereskedelmi piactéren elérhető termékek és előfizetések számlázása a Partnerközpont


**Megfelelő szerepkörök:** Globális rendszergazdai | Számlázási rendszergazda

A CSP-programban partnerként a Partnerközpont licencalapú SaaS-termékeket vásárolhat az ISV-közzétevőktől a kereskedelmi piactéren. Ezt követően hozzáférhet az ilyen típusú vásárlások számláihoz. A számlázási időszak a naptári hónap első napján kezdődik, és a naptári hónap utolsó napján ér véget. A számlák a következő hónap 8. napján érhetők el.

A számlákat elérheti a Partnerközpont [irányítópultjáról](https://partner.microsoft.com/dashboard/) vagy a Partnerközpont [API-k használatával.](/partner-center/develop/)

A CSP-programban részt vevő partnereknek akkor kell fizetniük az ügyfelek számára megvásárolt, isV kereskedelmi piactéri megoldásokért, amikor megvásárolják ezeket a termékeket az Partnerközpont-tól vagy a Azure Portal-től (az ügyfél korábbi, CSP által megvásárolt Azure-bérlője használatával).

>[!NOTE]
>Ha az ügyfelek a saját Azure AD-bérlőjüket használják (nem a CSP-programban egy partnertől vásároltat), az ügyfelek dönthetnek úgy is, hogy közvetlenül a (Microsoft AppSource vagy a Azure Marketplace) webhelyről vásárolják meg a saját ISV[](https://appsource.microsoft.com/) SaaS-megoldásukat. [](https://azuremarketplace.microsoft.com/) Ha így történik, közvetlenül a Microsofttól kapják meg a saját számlájukat. Hasonlóképpen, ha a CSP-programban egy partner egy Azure-előfizetést vagy új [Azure-tervet](/azure/role-based-access-control/built-in-roles) értékesít az ügyfélnek, és szerepköralapú hozzáférést biztosít az ügyfélnek (vagy közvetett viszonteladónak) az adott bérlőhöz (az Olvasón kívül bármely szerepkört hozzárendel az ügyfélhez), az ügyfél (vagy közvetett viszonteladó) előzetes jóváhagyás vagy értesítés nélkül is vásárolhat kereskedelmi piactéri ajánlatokat. Ezekben az esetekben a Microsoft nem értesíti közvetlenül a CSP-programban részt vevő partnereket az ügyfeleik vásárlásairól. A Microsoft azonban nem kötelezően [Azure Monitor](/azure/azure-monitor/platform/alerts-activity-log) mechanizmust, amely segítségével riasztásokat vagy értesítéseket állíthat be egy Azure-előfizetésen végzett tevékenységgel kapcsolatban.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Hozzáférés a kereskedelmi piactéren elérhető termékek számlázási adataihoz

A vállalat globális rendszergazdája vagy számlázási rendszergazdája e-mailt kap, ha a számla készen áll a megtekintésre. A kereskedelmi piactéri termékvásárlások legfrissebb számla- és egyeztetési fájlja:

1. Jelentkezzen be a Partnerközpont [irányítópultjába](https://partner.microsoft.com/dashboard/).

2. A Partnerközpont válassza a Számlázás **lehetőséget.** 

    A Számlázás lap tetején két lap **látható:** Ismétlődő és **Ismétlődő és egyszeri vásárlások.** Minden lapon hozzáférhet a különböző Marketplace-termékekhez tartozó számlákhoz és egyeztetési (recon) fájlokhoz:

    - **Ismétlődő** lap: Az Office 365,Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro és Microsoft Azure.

    - Ismétlődő és egyszeri vásárlások lap: Az **Azure-csomag,** az Azure Reservations, a szoftverek és a kereskedelmi piactéri termékek számla- és egyeztetési fájljait jeleníti meg.
  
3. Válassza az **Ismétlődő és egyszeri vásárlások** lapot. Ha egy ügyfél számára más pénznemben vásárolt előfizetéseket, minden pénznemhez fog egy lapfület látni. Ezen az oldalon néhány dolgot is meg tud tenni:

    - A legfrissebb számla- és egyeztetési fájl megnyitásához válassza a **Számla vagy** az **Egyeztetési fájl lehetőséget.** (Ha úgy volna, a legújabb számlaadatokhoz is hozzáférhet, és a fájladatokat a következő [API Partnerközpont tudja használni:](/partner-center/develop/).

    - A korábbi számlák és a fájlok felderítéséhez bontsa ki az alábbi **Számlázási előzmények** sort.

    - Ha bármikor ellenőriznie kell a becsült számlaegyenlegét vagy számláját a legutóbbi fióktevékenység alapján, válasszon egy hivatkozást a **Becslések fejléc** alatt.  

    >[!NOTE]
    > Amikor a hónap 8. napján közzétenjük a számlát, az tartalmazza az adókat, valamint az egyéb vonatkozó díjakat és jóváírásokat. Ez azt jelenti, hogy a végleges esedékesség eltérhet a számlázási időszak során láthatótól.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>További információ a kereskedelmi piactéri termékek számláiról és recon-fájljairól

Ez a szakasz további információkat tartalmaz a kereskedelmi piactéri SaaS-előfizetések számlázási és egyeztetési fájljairól, amelyek külső ISV-közzétevőktől származó ügyfelek számára vásárolhatók meg.

Ha az  Ismétlődő és egyszeri vásárlások  lehetőséget választja a Partnerközpont menü Számlázási lehetőségében, hozzáférést szerez a Microsoft (külső) és a külső (isV) vásárlásokkal kapcsolatos díjakhoz tartozó számlákhoz és egyeztetési fájlokhoz. Ezek a vásárlások a következőhöz társíthatóak:

- SaaS-előfizetések (Microsoft- vagy ISV-közzétevőktől)

- Azure-csomag

- Azure Reserved Virtual Machine Instances

- Egyéb előfizetés-alapú szoftverek (Microsoft- vagy ISV-közzétevőktől)

Ilyen vásárlás például a SUSE Linux-szoftver (szoftver-előfizetés) vagy egy Azure ISV SaaS-termék-előfizetés.

>[!NOTE]
> A számlák és a felderítési fájlok olvasásának további információiért lásd még a számlázás [áttekintését.](billing.md)

### <a name="tips-on-reading-your-invoice"></a>Tippek a számla elolvasása során

Amikor licencalapú SaaS-terméket vásárol egy külső isv-közzétevőtől, csak a számlán szereplő licencdíjat fogja látni. Ez akkor is igaz, ha az ISV SaaS-terméke felhasználja (vagy felhasználja) a mögöttes Azure-infrastruktúra erőforrásait. Ennek az az oka, hogy az ügyfél Azure-infrastruktúrahasználati díjai egy isV SaaS-termékére közvetlenül az ISV-nek vannak kiszámlázva. (Az ISV-k a kapcsolódó Azure-használati díjakat a saját Azure-használatuk napi minősítésű számlaegyeztetési fájljában látják.)

A számla több oldalt fog tartalmazni:

- **A számla 1. oldala:** A CSP-programpartner számlázási részleteinek összefoglaló áttekintését tartalmazza. Ez magában foglalja a számlázási időszakra vonatkozó díjak összegzését, a számlaszámot, a fizetési feltételeket (60 nap) és a számlázási fizetési módokat átutalással vagy csekken történő fizetéshez.

- **A számla 2.** oldala (és az azt követő oldalak): Részletes információkat tartalmaz a külső Microsoft-vásárlások és a kereskedelmi piactérről (licencalapú) harmadik féltől származó ISV-vásárlások díjairól. Az ISV-licencalapú vásárlásokat az egyes terméknév alatti **Közzétevő** sor alapján azonosíthatja. A társított egyeztetési fájl további számlázási adatokat kínál az egyes számlázási díjakról.

- **A számla utolsó oldala:** Ha egy isV-től származó licencalapú Marketplace-termékekért kell fizetnie, ez az utolsó oldal további részleteket jelenít meg az ISV-közzétevő nevével és címével kapcsolatban.

### <a name="tips-on-reading-your-reconciliation-file"></a>Tippek az egyeztetési fájl olvasmányhoz

Az **Ismétlődő és egyszeri vásárlások egyeztetési** fájl több oszlopot tartalmaz, amelyek további részleteket tartalmaznak, amelyek a számlán szereplő díjakra vannak leképezve. A **PublisherName oszlopban** látható, hogy a vásárlás a Microsofttól vagy egy külső isV-közzétevőtől származik.

Előfordulhat, hogy az egyeztetési fájlban egyes díjak 0 usd költséggel jelennek meg. Ezt okozhatja egy isV "ingyenes próbaverziós" ajánlata (általában 30 vagy 60 nap), vagy egy saját licenccel rendelkező ajánlat.

Ingyenes isV-ajánlatok esetén:

- Az ingyenes próbaidőszak fedezi az ISV licencalapú SaaS-termékének költségeit az adott időszakban. Emellett nem számítunk fel díjat az adott SaaS-termék társított Azure-infrastruktúrájának használata után.  Ha azonban használatalapú isv-ajánlatot használ, az ingyenes próbaverzió nem tartalmazza a mögöttes Azure-infrastruktúra használatának költségeit. Ebben az esetben az Azure-infrastruktúra használati díjai egy külön Azure egyeztetési fájlban jelennek meg.

- Amikor megvásárolja és üzembe helyez egy ISV ingyenes próbaverzióra jogosult termékét az ügyfél számára, az isV közzétevője automatikusan regisztrálja az ügyfelet az ingyenes próbaverzióban. Az ingyenes próbaidőszak automatikusan véget ér az ISV-közzétevő által meghatározott időszak után. Az időszak vége után az ügyfélnek díjat kell fizetnie. Ez azt jelenti, hogy az egyeztetési fájl két sort is megjeleníthet a próbaverzióra jogosult termékhez: egyet, amely nyomon követi a próbaidőszakot, és egy másikat, amely nyomon követi a fizetős ajánlatot (amely a próbaidőszak végéig 0 DOLLÁR költségeket jelenít meg). A próbaidőszak végén a fizetős ajánlatot megjelenítő sor költségeket fog mutatni. 

Az egyes oszlopok jelentésére vonatkozó további információkért lásd: [Az egyeztetési fájlok használata.](use-the-reconciliation-files.md) Lásd [még: A](./billing-basics.md) számlázás típusai a Partnerközpont

## <a name="next-steps"></a>Következő lépések

- [Kereskedelmi piactéri termékek kezelése ügyfelek számára](csp-commercial-marketplace-manage.md)
- [További információ a kereskedelmi piactéri termékek támogatásról](csp-commercial-marketplace-support.md)