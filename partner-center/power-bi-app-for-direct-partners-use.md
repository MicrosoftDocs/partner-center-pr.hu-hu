---
title: A Power BI a partner Center Analytics használata
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan tekintheti meg az üzleti adatait a Power BIhez készült partner Center Analytics alkalmazással (a CSP-ben található közvetlen partnereknél).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 244cb852728d47360cf8ecd1d1e9ccb641466b1d
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215747"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Üzleti adatai megtekinthetők a Microsoft Power BI partner Center Analytics alkalmazásával



**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói rendszergazda
- Értékesítési ügynök
- Felügyeleti ügynök

## <a name="view-your-business-data"></a>Üzleti adatai megtekintése

Tekintse meg az üzleti adatai vizuális megjelenítését a Power BIhez készült partner Center Analytics-alkalmazással, beleértve a következőket:

- Ügyfélkör, előfizetések és licencek növekedése

- Az Office 365, a Microsoft Dynamics és a Microsoft Azure termékek használata

- Napi fogyasztási egységek minden egyes mért erőforráshoz az elmúlt 60 napra vonatkozóan az egyes Azure-előfizetésekben

- Becsült költségek (a legújabb díjszabási kártya alapján)

- Lehetőség az adatkészletek exportálására és egyéni jelentések létrehozására, beleértve az ügyfeleket is.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Tudnivalók a partner Center Analytics alkalmazás előzetes kiadásáról

- Ez az alkalmazás csak a Cloud Solution Provider program közvetlen partnerei számára érhető el. A CSP-ben lévő többi partner (például a közvetett viszonteladók) nem tud majd bejelentkezni.

- A becsült költségek díjszabása adózási/számlázási, és nem jogilag kötelező. A becsült költségek csak az adatelemzések esetében használhatók.

- Az ügyfél adatai az előfizetéseken alapulnak. Azok a felhasználók, akikkel a közelmúltban létrehozott fiókokat, de még nincsenek előfizetések, nem számítanak bele a számba.

- A becsült költség a legújabb díjszabási kártyán alapul, amely a CSP díjszabásán alapul.

- A napok naptári napok.

### <a name="business-insights-report"></a>Üzleti célú adatjelentések

- **Ügyfél bérlői**: a megvásárolt előfizetéseket használó ügyfelek eltérő Azure ad-bérlőinak száma

- **Új (utolsó 30 nap)**: az új ügyfelek legalább egy előfizetést vásárolnak az elmúlt 30 napban

- Forgalom **(utolsó 30 nap)**: az ügyfelek "aktív", "türelmi" vagy "letiltott" előfizetések nélkül

- **Új (az elmúlt 24 órában)**: az új ügyfelek legalább egy előfizetést vásárolnak az elmúlt 24 órában

- A **becsült havi költség az elmúlt 12 hónapban**: a becsült ÁFA utáni becsült összeg havi száma az elmúlt 12 hónap során összesítve

- **Becsült költségek termékenként az elmúlt 12 hónapban**: eladott termékek – az elmúlt 12 hónap során összesítve becsült ÁFA után fizetendő összeg. Ez az állapot a legtöbb bevételt eredményező legfontosabb termékeket jelzi.

- Az **elmúlt 12 hónapban** megjelenő ügyfelek: az új ügyfelek és a forgalomban lévő ügyfelek havi hónapja az elmúlt 12 hónap során összesítve

- **Becsült költségek az ügyfél által az elmúlt 12 hónapban**: az ügyfelek az elmúlt 12 hónapra vonatkozó becsült ÁFA után fizetendő összeg alapján összesítve jelennek meg. Ez az állapot a legtöbb bevételt eredményező legfontosabb ügyfeleket jelzi.

- **Ügyfelek száma termék szerint**: az eladott termékek a társított ügyfelek szerint rendezve. Ez az állapot a legtöbb ügyfél számára eladott legfontosabb termékeket jelzi.

### <a name="subscription-insights-report"></a>Előfizetés-áttekintési jelentés

- **Előfizetés állapota**:

- Aktív: az "aktív" vagy "a" türelmi állapotba tartozó előfizetések

  - Felfüggesztve: a "Letiltva" állapothoz tartozó előfizetések

  - Kiépítve: "kiépített" vagy "lejárt" állapotba tartozó előfizetések

- **Lejárati állapot**:

  - Lejárt: már lejárt előfizetések (az előfizetés lejárati dátuma korábbi)

  - 30 nap után lejár: az előfizetések 30 nap után lejárnak (az előfizetés befejezési dátuma pedig a következő 30 nap után)

  - 30 nap alatt lejár: az előfizetések, amelyek a következő 30 napon belül lejárnak (az előfizetés befejezési dátuma ma és a következő 30 nap között van)

- **Összes előfizetés**: az "Active", "" in Grace "vagy" disabled "állapotú előfizetések

- **Új (utolsó 30 nap)**: az ügyfelek által az elmúlt 30 napban vásárolt új előfizetések

- **Új (az elmúlt 24 óra)**: az ügyfelek által az elmúlt 24 órában vásárolt új előfizetések

- **30 nap alatt lejár**: az előfizetések, amelyek a következő 30 napon belül lejárnak

- Forgalom **(utolsó 30 nap)**: az elmúlt 30 napban kiosztott vagy felfüggesztett (letiltott) előfizetések

- **Elosztás előfizetési típusok** szerint: az összes előfizetés%-os elosztása licenc-alapú és használati alapú előfizetési típus szerint

- **Aktív előfizetés darabszáma termékenként**: aktív előfizetések száma szerint értékesített termékek száma

- **Előfizetések az elmúlt 12 hónapban**: az új előfizetések és a változási előfizetések hónapja az elmúlt 12 hónap során összesített havi gyakorisággal

- **Ügyfél-előfizetés részletei**: az ügyfelek, előfizetések és ajánlatok részletes áttekintése

### <a name="license-insights-report"></a>Licencelési jelentés:

- Összes **licenc**: teljes licenc-alapú előfizetések összesített száma

- **Új (utolsó 30 nap)**: licenc hozzáadása az elmúlt 30 napban

- Adatforgalom **(utolsó 30 nap)**: a licencek csökkentése az elmúlt 30 napban

- **Új (utolsó 24 óra)**: licenc hozzáadása az elmúlt 24 órában

- Az **elmúlt 90 napra vonatkozó licencek**: a licencek hozzáadásának hónapja, valamint az elmúlt 90 nap során összesített havi összesítések.

- **Aktív licencek száma termék szerint**: az eladott termékek aktív licencek száma szerint rendezve

- **Aktív licencek száma ügyfél szerint**: az ügyfelek az aktív licencek száma szerint rendezve

- **Ügyfél-licencelési esemény részletei az elmúlt 90 napban**: az ügyfelek, előfizetések és előfizetési események részletes nézete, beleértve az esemény dátumát, az esemény nevét, a mennyiséget és a mennyiség változását.

### <a name="licenses-usage-report"></a>Licencek használati jelentése:

- **A termék által hozzárendelt licencek**: az eladott termékek licenc-hozzárendelések száma szerint rendezve

- **Termék által használt licencek**: a licencek használati száma szerint rendezve értékesített termékek

- **A hozzárendelt licencek ügyfél-eloszlása**: a teljes ügyfelek%-os elosztása a licenc-hozzárendeléssel számított 20%-ban

- A **használatban lévő licencek ügyfél-eloszlása**:%-ban a teljes ügyfél%-os elosztása a licencek kihasználtsága alapján%-kal megszakadt.

- **Ügyfél által hozzárendelt licencek**: az eladott licencek és az ügyfelek és termékek által hozzárendelt licencek részletes nézete

- **Ügyfél által használt licencek**: az eladott licencek és az ügyfelek és termékek által használt licencek részletes nézete

### <a name="azure-insights-report"></a>Azure-beli bepillantást ismertető jelentés:

- A **használaton alapuló ügyfelek az elmúlt 12 hónapban**: az új, használati alapú ügyfelek és a felhasználható használaton alapuló ügyfelek havi hónapjának trendje az elmúlt 12 hónap során összesítve

- **Használaton alapuló előfizetések az elmúlt 12 hónapban**: az új használati-alapú előfizetések és a felhasználható használaton alapuló előfizetések havi hónapja az elmúlt 12 hónap során összesítve

- Az **ügyfél által az elmúlt 60 napban becsült használati költségek**: a használaton alapuló ügyfelek az utolsó 60 nap során összesítve becsült ÁFA nélküli számla összegét használják. Ez az állapot a legtöbb bevételt eredményező, legszélesebb körű használatú ügyfeleket jelzi

- A **becsült használati költségek kategóriánként az elmúlt 60 napban**: a használati alapú előfizetések kategóriái az utolsó 60 nap során összesített, a számlán becsült, ÁFA nélküli számla összegével.

- Az **előfizetés becsült használati díja az elmúlt 60 napban**: a használaton alapuló előfizetések száma az utolsó 60 nap során összesített, ÁFA nélkül számlázott összeg alapján.

- Az **ügyfél becsült használati díja költségvetés szerint**: az ügyfelek a jelenlegi használati költségkeretük százalékában meghaladják a küszöbértéket (100%).

### <a name="azure-resource-usage-report"></a>Azure-Erőforrás-használati jelentés:

- Az **Azure-erőforrások napi használata a kiválasztott időszakra** vonatkozóan: az elmúlt 60 napon belül minden használaton alapuló előfizetéshez tartozó napi fogyasztási egység

- A **kiválasztott időszakra vonatkozó Azure-erőforrások becsült használati díja**: az elmúlt 60 napban megadott időszakra vonatkozó, a legújabb díjszabási kártyán alapuló becsült költségek az egyes használati alapú előfizetésekben 

## <a name="next-steps"></a>Következő lépések

- [A Power BI alkalmazáshoz készült partner Center Analytics áttekintése](power-bi-app-for-direct-partners.md)

- [A Partnerközpont adatelemzési alkalmazás a Microsoft Power BI-hoz telepítése és előzetes verziója](power-bi-app-for-direct-partners-install.md)
