---
title: Kereskedelmi Piactéri termékek számlázása
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan működik a számlázás a partner centeren belül a kereskedelmi piactéren vásárolt ISV SaaS-termékek vagy-előfizetések esetében.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c03ab358b8fb6ab0f23ea5f42b9d35c6f6c2b80c
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92529965"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Kereskedelmi piactér-termékek és-előfizetések számlázása a partner Centerben

**A következőkre vonatkozik**

- Partnerközpont
- Partnerek a CSP programban

**Megfelelő szerepkörök**

- Globális rendszergazda
- Számlázási adminisztrátor

A CSP program partnereként a partner Center használatával vásárolhat licenc alapú SaaS-termékeket a kereskedelmi piactéren található ISV-közzétevők közül. Ezt követően elvégezheti az ilyen típusú vásárlásokhoz tartozó számla elérését. A számlázási időszak a naptári hónap első napján kezdődik, és a naptári hónap utolsó napján ér véget. A számlák a következő hónap 8. napján lesznek elérhetők.

A partner Center- [irányítópultról](https://partner.microsoft.com/dashboard/) vagy a [partner Center API](/partner-center/develop/)-k használatával is elérheti a számlákat.

A CSP programban részt vevő partnerek számlázása akkor történik meg, ha az ügyfél a partner központból vagy a Azure Portalból vásárolja meg ezeket a termékeket (az ügyfél korábbi, CSP-megvásárolt Azure-bérlőjét használva).

>[!NOTE]
>Ha az ügyfelek saját Azure AD-bérlőt használnak (a CSP program egyik partnere sem vásárolja meg), az ügyfelek a saját ISV SaaS-megoldást közvetlenül a ([Microsoft AppSource](https://appsource.microsoft.com/) vagy az [Azure Marketplace](https://azuremarketplace.microsoft.com/)-ről) is megvásárolhatják. Ha így tesznek, akkor közvetlenül a Microsofttól kapják meg a számláját. Hasonlóképpen, ha a CSP program egyik partnere eladja az Azure-előfizetést vagy az új Azure-csomagot az ügyfél számára, és az ügyfél (vagy közvetett viszonteladó) [szerepkör-alapú hozzáférést](/azure/role-based-access-control/built-in-roles) biztosít az adott bérlőhöz (az **olvasón** kívül bármely szerepkört rendel az ügyfélhez), az ügyfél (vagy közvetett viszonteladó) is vásárolhat kereskedelmi PIACTÉRi ajánlatokat a CSP-partnernek előzetes jóváhagyás vagy értesítés nélkül Ezekben az esetekben a Microsoft nem értesíti közvetlenül a partnereket a CSP programban az ügyfelek által végzett vásárlásokról. A Microsoft azonban opcionális [Azure monitor](/azure/azure-monitor/platform/alerts-activity-log) mechanizmust is kínál, amellyel riasztásokat vagy értesítéseket állíthat be az Azure-előfizetések tevékenységeivel kapcsolatban.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Hozzáférés a kereskedelmi Piactéri termékek számlázási adataihoz

A vállalat globális rendszergazdája vagy számlázási rendszergazdája e-mailt fog kapni, ha a számla készen áll a megtekintésre. A kereskedelmi piactéren vásárolt termékek legutóbbi számlázási és egyeztetési fájljának elérése:

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/).

2. A partner Center menüben válassza a **számlázás** lehetőséget. 

    A számlázási oldal tetején két lap jelenik meg: **ismétlődő** és **ismétlődő, egyszeri vásárlás** . Mindegyik lapon elérhetővé válik a különböző Piactéri termékekhez tartozó számla-és egyeztetési (Recon) fájlok:

    - **Ismétlődő** lap: az Office 365, a Microsoft 365, a Dynamics 365, a Azure Active Directory, a Power bi Pro és a Microsoft Azure szolgáltatáshoz kapcsolódó előfizetések számlázási és egyeztetési fájljait jeleníti meg.

    - **Ismétlődő és egyszeri vásárlás** lap: az Azure-csomag, az Azure-foglalások, a szoftverek és a kereskedelmi piactér-termékek számlázási és egyeztetési fájljait jeleníti meg.
  
3. Válassza az **ismétlődő és egyszeri vásárlás** lapot. Ha más pénznemben vásárolt egy ügyfél előfizetéseit, megjelenik az egyes pénznemek lapja. Ezt az oldalt elvégezheti:

    - A legutóbbi számla-és egyeztetési fájl megtekintéséhez válassza a **számla** vagy a **megbékélési fájl** elemet. (Ha szeretné, a [partner Center API](/partner-center/develop/)-kkal is elérheti a legújabb számlázási és felderítési fájlokat.

    - A korábbi számlák és a felderítési fájlok megjelenítéséhez bontsa ki az alábbi **Számlázási előzmények** sort.

    - A becsült fiók egyenlegének vagy számlájának a legutóbbi fiók tevékenység alapján bármikori ellenőrzéséhez válasszon egy hivatkozást a **becslések** fejléc alatt.  

    >[!NOTE]
    > Ha a hónap 8. napján közzétesszük a számlát, az adót és az egyéb alkalmazandó díjakat és jóváírásokat is tartalmazza. Ez azt jelenti, hogy a végső esedékes összeg eltérhet a számlázási időszak során láthatótól.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>További információ a kereskedelmi Piactéri termékekkel kapcsolatos számlákból és felderítési fájlokról

Ez a szakasz további információkat tartalmaz a harmadik féltől származó ISV-közzétevők ügyfelei számára vásárolt kereskedelmi Piactéri SaaS-előfizetések számlázási és egyeztetési fájljairól.

Ha a partner Center menüjében a **számlázás** lehetőségnél az **ismétlődő és egyszeri vásárlás** lehetőséget választja, akkor a Microsoft (első féltől származó) és az ISV (harmadik féltől származó) vásárlásokhoz kapcsolódó díjakhoz is hozzáférhet a számlákon és a megbékélési fájlokhoz. Ezek a vásárlások az alábbiakhoz társíthatók:

- SaaS-előfizetések (Microsoft vagy ISV-közzétevőtől)

- Azure-csomag

- Azure Reserved Virtual Machine Instances

- Egyéb előfizetés-alapú szoftverek (Microsoft vagy ISV közzétevőtől)

Ilyen vásárlás például a SUSE Linux szoftver (szoftveres előfizetés) vagy egy Azure ISV SaaS-termék előfizetése lehet.

>[!NOTE]
> A számlázási és a felderítési fájlok olvasásával kapcsolatos további információkért lásd még: a [számlázás áttekintése](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Tippek a számla olvasásához

Ha egy harmadik féltől származó ISV-közzétevőtől vásárol licenc-alapú SaaS-terméket, csak a számlán szereplő licencfeltételek díját fogja látni. Ez akkor is igaz, ha az ISV SaaS-terméke a mögöttes Azure-infrastruktúra erőforrásait használja. Ennek az az oka, hogy az ügyfél Azure-infrastruktúrájának használati díját az ISV SaaS-termékért közvetlenül az ISV-k számlázzák. (Az ISV-ket a saját Azure-használati díjakra vonatkozó, napi rendszerességgel felszámított számlázási egyeztetési fájlban láthatja.)

A számla több oldalt is tartalmaz:

- **A számla 1. lapja:** A CSP-Partnerprogram számlázási adatainak összegzését tartalmazza. Ez magában foglalja a számlázási időszak díjait, a számla számát, a fizetési feltételeket (nettó 60 nap) és a Számlázási fizetési módokat a vezetékes vagy ellenőrzés útján történő fizetéshez.

- **A számla 2. lapja (és a többi oldal):** A Microsoft és a harmadik féltől származó független szoftvergyártók (licenc-alapú) vásárlásának díjai a kereskedelmi piactéren. Az ISV-licenceken alapuló vásárlásokat a **közzétevői** sor alapján azonosíthatja az egyes termékek neve alatt. A társított egyeztetési fájl több számlázási részletet is kínál az adott számlázási díjakhoz.

- **A számla utolsó lapja:** Ha a licenccel rendelkező Marketplace-termékekért díjat számítunk fel egy ISV-ból, akkor ez a végső oldal további részleteket jelenít meg az ISV-közzétevő nevével és címtől kapcsolatban.

### <a name="tips-on-reading-your-reconciliation-file"></a>Tippek a megbékélési fájl olvasásához

Az **ismétlődő és egyszeri beszerzések** egyeztetésére szolgáló fájl több oszlopot tartalmaz, amelyek további részleteket tartalmaznak a számlán lévő díjakra leképezve. A **közzétevő neve** oszlopban látható, hogy a vásárlás a Microsofttól vagy egy külső gyártótól származó ISV-közzétevőtől származik-e.

A megbékélési fájlban lévő egyes díjak $0-as költségekkel jelenhetnek meg. Ennek oka az lehet, hogy egy ISV "ingyenes próbaverzió" (általában 30 vagy 60 nap) vagy egy saját licencelési ajánlat.

Ingyenes próbaverziós ISV-ajánlatok esetén:

- Az ingyenes próbaidőszak az ISV-k licenc-alapú SaaS-termékének költségét fedezi az adott időszakban. Az adott SaaS-termékhez tartozó Azure infrastruktúra-használatért nem számítunk fel díjat.  Ha azonban használaton alapuló ISV-ajánlatot használ, az ingyenes próbaverzió nem tartalmazza a mögöttes Azure-infrastruktúra használatának költségeit. Ebben az esetben az Azure-infrastruktúra használati díjait külön Azure-egyeztetési fájlban fogjuk megjelenni.

- Ha az ügyfél számára ingyenes próbaverzióra jogosult terméket vásárol és helyez üzembe, az ügyfelet a rendszer automatikusan regisztrálja az ingyenes próbaverzióban az ISV közzétevővel. Az ingyenes próbaidőszak az ISV-közzétevő által meghatározott időszak után automatikusan véget ér. Az időszak lejárta után az ügyfél díjat számítunk fel. Ez azt jelenti, hogy az egyeztetési fájl két sort mutat a próbaverzióra jogosult termékre vonatkozóan: az egyik, amely nyomon követi a próbaidőszakot, és az egyiket, amely nyomon követi a fizetős ajánlatot (amely a próbaidőszak lejárta után $0-as díjat fog megjelenni). A próbaidőszak lejárta után a fizetős ajánlatot tartalmazó sor megkezdi a díjak megjelenítését. 

További információ az egyes oszlopokról: [a megbékélési fájlok használata](use-the-reconciliation-files.md). Lásd még: [Számlázási típusok a partner Centerben](billing-different-types.md)

## <a name="next-steps"></a>Következő lépések

- [Kereskedelmi Marketplace-termékek kezelése ügyfelek számára](csp-commercial-marketplace-manage.md)
- [További információ a kereskedelmi Piactéri termékek támogatásáról](csp-commercial-marketplace-support.md)