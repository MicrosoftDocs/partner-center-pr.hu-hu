---
title: A Partnerközpont Analytics használata Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Útmutató üzleti adatainak megtekintéséhez a Partnerközpont adatelemzési alkalmazás a Power BI-hoz használatával (a Felhőszolgáltató (CSP) program közvetlen partnerei számára).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564981"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Üzleti adatok megtekintése a Microsoft Partnerközpont Analytics alkalmazással Power BI



**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Értékesítési ügynök | Rendszergazdai ügynök

## <a name="view-your-business-data"></a>Üzleti adatok megtekintése

Az üzleti adatok vizuális ábrázolása a Microsoft Partnerközpont Analytics alkalmazással, többek között a következő Power BI le:

- Az ügyfélkör, az előfizetések és a licencek növekedése

- Office 365-, Microsoft Dynamics- és Microsoft Azure termékek használata

- Az egyes Azure-előfizetések forgalmi díjas erőforrásának napi fogyasztási egységei az elmúlt 60 napra

- Becsült költség (a legújabb díjkártya alapján)

- Lehetőség az adatkészletek exportálására és egyéni jelentések létrehozására, beleértve az ügyfélenkénti jelentéseket is.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>A Partnerközpont Analytics alkalmazás előzetes kiadásának adatai

- Ez az alkalmazás csak a Felhőszolgáltató (CSP) program közvetlen partnerei számára való. A CSP más partnerei (például közvetett viszonteladók) nem tudnak bejelentkezni.

- A becsült költségek adók előtti számlázási/számlaadatok, és nem kötelezőek. A becsült költségek csak adatelemzéshez használhatók.

- Az ügyféladatok az előfizetésen alapulnak. Azok az ügyfelek, akikhez a közelmúltban létrehozott fiókokat, de még nem rendelkezik előfizetésekkel, nem szerepelnek a darabszámok között.

- A becsült költség a legújabb díjszabású kártyán alapul, amely a CSP díjszabásán alapul.

- A napok naptári napok.

### <a name="business-insights-report"></a>Business Insights-jelentés

- **Ügyfélbérlők:** Az előfizetéseket Azure Active Directory (Azure AD-) ügyfelek különböző bérlőinek száma

- **Új (az elmúlt 30 nap)**: Új ügyfelek, akik legalább egy előfizetést vásárolnak az elmúlt 30 napban

- **Adatváltozás (az elmúlt 30 nap)**: "aktív", "türelmi" vagy "letiltott" előfizetéssel nem

- **Új (az elmúlt 24 óra)**: Új ügyfelek, akik legalább egy előfizetést vásárolnak az elmúlt 24 órában

- Becsült havi költség az elmúlt 12 hónapra: Az adók előtti számlás dollárban becsült összeg havi összesítése az elmúlt **12** hónap időszakában

- **Termékonkénti becsült** költség az elmúlt 12 hónapra vonatkozóan: Az értékesített termékek az adók előtti számlás dollárban becsült összeg szerint rendezve, az elmúlt 12 hónapra vonatkozóan összesítve. Ez az állapot a legtöbb bevételt hozó leggyakoribb termékeket jelzi.

- **Az elmúlt 12** hónap ügyfelei: Az új ügyfelek és a lemorzsolódási ügyfelek havi trendje az elmúlt 12 hónapra vonatkozóan havonta

- Becsült költség ügyfél szerint az elmúlt **12** hónapra vonatkozóan: Ügyfelek az adók előtti, dollárban számlázott becsült összeg szerint rendezve az elmúlt 12 hónapra vonatkozóan. Ez az állapot a legtöbb bevételt hozó leggyakoribb ügyfeleket jelzi.

- **Ügyfelek száma termék szerint:** A társított ügyfelek szerint rendezve értékesített termékek. Ez az állapot a legtöbb ügyfél számára értékesített legnépszerűbb termékeket jelzi.

### <a name="subscription-insights-report"></a>Subscription Insights-jelentés

- **Előfizetés állapota:**

- Aktív: "aktív" vagy "türelmi" állapothoz tartozó előfizetések

  - Felfüggesztve: "Letiltott" állapothoz tartozó előfizetések

  - Kiépítve: A "kiépítve" vagy "lejárt" állapothoz tartozó előfizetések

- **Lejárati állapot:**

  - Lejárt: Lejárt előfizetések (ha az előfizetés záró dátuma lejárt)

  - Lejárat 30 nap után: 30 nap után lejáró előfizetések (ahol az előfizetés záró dátuma a következő 30 nap után lesz)

  - Lejárat 30 napon belül: A következő 30 napon belül lejáró előfizetések (ahol az előfizetés záró dátuma ma és a következő 30 nap között van)

- **Összes előfizetés:** Az "aktív", a "türelmi időszakban" vagy a "letiltva" állapotú előfizetések

- **Új (az elmúlt 30 nap)**: Az ügyfelek által az elmúlt 30 napban vásárolt új előfizetések

- **Új (az elmúlt 24 óra)**: Az ügyfelek által az elmúlt 24 órában vásárolt új előfizetések

- **Lejárat 30 napon belül:** A következő 30 napon belül lejáró előfizetések

- **Adatváltozás (az elmúlt 30 nap)**: Az elmúlt 30 napban fel lett függesztve vagy fel lett függesztve (letiltva) előfizetések

- **Elosztás előfizetés-típusok szerint:** Az összes előfizetés százalékos eloszlása licencalapú és használatalapú előfizetés-típus szerint

- **Aktív előfizetések száma termék szerint:** Eladott termékek az aktív előfizetések száma szerint rendezve

- **Előfizetések az elmúlt 12 hónapra:** Az új előfizetések és a lemorzsolódási előfizetések havi trendje az elmúlt 12 hónapra vonatkozóan

- **Ügyfél-előfizetés részletei:** Az ügyfelek, előfizetések és ajánlatok részletes nézete

### <a name="license-insights-report"></a>License Insights-jelentés:

- **Összes licenc:** Az összes licencalapú előfizetésben összesített licencek teljes száma

- **Új (az elmúlt 30 nap)**: Licenc összeadása az elmúlt 30 napon belül

- **Adatváltozás (az elmúlt 30 nap)**: Licenc csökkentése az elmúlt 30 napon belül

- **Új (az elmúlt 24 óra)**: Licenc összeadása az elmúlt 24 órában

- **Licencek az elmúlt 90 napban:** A licencek kiegészítésének és csökkentésének havi trendje az elmúlt 90 napban havonta

- **Aktív licencek száma termék szerint:** Eladott termékek aktív licencek száma szerint rendezve

- **Aktív licencek száma ügyfél szerint:** Az ügyfelek az aktív licencek száma szerint rendezve

- Ügyféllicenc-esemény adatai az elmúlt **90 napban:** Az ügyfelek, előfizetések és előfizetési események részletes nézete, beleértve az esemény dátumát, az esemény nevét, a mennyiséget és a mennyiség változását.

### <a name="licenses-usage-report"></a>Licenchasználati jelentés:

- **Termék szerint hozzárendelt licencek:** Eladott termékek licenc-hozzárendelések száma szerint rendezve

- **Termék szerint használt licencek:** Eladott termékek a licenchasználat száma szerint rendezve

- **Hozzárendelt licencek ügyfélelosztása:** Az összes ügyfél százalékos eloszlása 20%-os tartományra bontva licenc-hozzárendelés alapján %

- **Használatban található licencek ügyfélelosztása:** Az összes ügyfél százalékos eloszlása, 20%-os tartományba oszlása licenchasználat szerint %

- **Az ügyfél által hozzárendelt licencek:** Az ügyfelek és termékek által hozzárendelt eladott licencek és licencek részletes nézete

- **Az ügyfél által használt licencek:** Az ügyfelek és termékek által használt eladott licencek és licencek részletes nézete

### <a name="azure-insights-report"></a>Azure Insights-jelentés:

- Használatalapú ügyfelek az elmúlt **12** hónapra vonatkozóan: Az új használatalapú ügyfelek és a lemorzsolódáson alapuló ügyfelek havi összesítése az elmúlt 12 hónap időszakában

- Használatalapú előfizetések az elmúlt **12** hónapra: Az új használatalapú előfizetések és a lemorzsolódáson alapuló előfizetések havi összesítése az elmúlt 12 hónap időszakában

- Az ügyfél által az elmúlt **60** nap becsült használati költsége: Használatalapú ügyfelek az adók előtti számlás dollárban becsült összeg szerint rendezve az elmúlt 60 napban. Ez az állapot a legnagyobb bevételt hozó, használaton alapuló ügyfeleket jelzi

- Becsült használati költség kategória szerint az elmúlt **60** napra vonatkozóan: Használatalapú előfizetések fogyasztásmérő-kategóriái, az elmúlt 60 nap során összesített, adók előtti, dollárban becsült összeg szerint rendezve.

- Becsült használati költség előfizetés szerint az elmúlt **60** napban: Használatalapú előfizetések az adók előtti számlás dollárban becsült összeg szerint, az elmúlt 60 napban összesítve.

- **Az ügyfelek becsült használati költsége a** költségkeret alapján: Az ügyfelek a jelenlegi használati költségkeretük százalékos aránya szerint rendezve túllépik a küszöbértéket (100%).

### <a name="azure-resource-usage-report"></a>Azure-erőforráshasználati jelentés:

- **Az Azure-erőforrások napi** használata a kiválasztott időszakban: Az egyes használatalapú előfizetések egyes forgalmi díjas erőforrásainak napi használati egységei az elmúlt 60 napra vonatkozóan.

- **Az Azure-erőforrások becsült** használati költsége a kiválasztott időszakra vonatkozóan: Becsült költség az egyes használatalapú előfizetések használati díjának legutóbbi díjszabása alapján az elmúlt 60 napra vonatkozóan. 

## <a name="next-steps"></a>Következő lépések

- [Partnerközpont Analytics for Power BI alkalmazás áttekintése](power-bi-app-for-direct-partners.md)

- [A Partnerközpont adatelemzési alkalmazás a Microsoft Power BI-hoz telepítése és előzetes verziója](power-bi-app-for-direct-partners-install.md)
