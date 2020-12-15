---
title: Elemzések adatdefiníciói
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A dokumentum megjeleníti a különböző jelentések listáját és az egyes jelentésekhez tartozó adatdefiníciókat, amelyek letölthetők az elemzések letöltése jelentés oldaláról.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2020
ms.locfileid: "97502128"
---
# <a name="export--data-definitions"></a>Exportálás – adatdefiníciók 

 **Megfelelő szerepkörök** 

- Jelentés megjelenítője 
- Executive Report Viewer 

## <a name="introduction"></a>Bevezetés 

Az elemzések irányítópultján a jelentések letöltése központ lehetővé teszi a nyers adatkészletek exportálását.  

A különböző jelentések, amelyek az adatdefinícióval együtt tölthetők le, az alábbi módon érhetők el: 

**Partner profil**: a profil jelentés különböző mezőinek adatdefiníciói a következők: 


| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|MPNId|Microsoft Partner Network azonosítója|
|PartnerName|A partner neve |
|PGA_MPNId|Partner globális fiók MPN-azonosítója|
|PGA_PartnerName|Partner globális fiókjának neve|
|City|Partner város helye |
|Ország|Partner országának helye |
|HierarchyLevel|Azt jelzi, hogy globális MPN-azonosító vagy Location MPN-azonosító|

**Vásárlói** adatok: az ügyfél részletei jelentés különböző mezőinek adatdefiníciói a következők:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|CustomerName|Az ügyfél neve |
|CustomerTenantId|Ügyfél bérlőjének azonosítója |
|CustomerTpid|Ügyfél elsődleges szülő-azonosítója |
|CustomerSegment|Felhasználói szegmens |
|CustomerMarket|Az ügyfél földrajzi piaca  |
|CustomerStatus|Ügyfél állapota (aktív/inactive) |
|Termék|Az MPN által az ügyfélnek eladott termék. Ez az egyik a O365, a D365, a nagyvállalati mobilitás, a Power BI Microsoft Azure.|
|Termékváltozat|   Termék SKU|
|Month (hónap)| A használat és a bevétel jelentésének hónapja|
|MPNId| Microsoft Partner Network azonosítója|
|PartnerName|   A partner neve|
|PartnerLocation|   Partner földrajzi helye|
|PartnerAttributionType|    Partneri típus|
|SalesChannel|  Értékesítési csatorna|
|AvailableSeats|    Rendelkezésre álló helyek| 
|RevenueUSD|    Bevétel USD-ben|

**Viszonteladói teljesítmény**: a viszonteladói teljesítmény jelentéseinek különböző mezőinek adatdefiníciói a következők:

> [!Note]
> A bevételek és az ACR-adatforrások csak az Executive-jelentések megjelenítői által biztosított felhasználók számára érhetők el.

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|ResellerMpnid|Viszonteladói Microsoft Partner Network azonosítója| 
|ResellerName|Viszonteladó neve|
|ResellerMarket|Viszonteladói ország piaca| 
|IndirectProviderMPNId|Közvetett szolgáltató Microsoft Partner Network azonosítója|
|IndirectProviderName|Közvetett szolgáltató neve|
|Month (hónap)|A használat és a bevétel jelentésének hónapja|
|Termék|Terméknév|
|SubscriptionID|Előfizetés azonosítója|
|AvailableSeats|Rendelkezésre álló helyek száma|
|AssignedSeats|Hozzárendelt ülőhelyek száma|
|BilledRevenueUSD|Számlázott bevétel ($)|
|CustomerName|Az ügyfél neve| 
|CustomerTPid|Ügyfél elsődleges szülő-azonosítója| 
|CustomerSegment|Felhasználói szegmens |
|CustomerMarket|Az ügyfél földrajzi piaca |
|ResellerStatus|Viszonteladói állapot| 

**Előfizetések részletei**: az előfizetés részletei jelentés különböző mezőinek adatdefiníciói a következők:

>[!Note]
>A bevételek és az ACR-adatforrások csak az Executive-jelentések megjelenítői által biztosított felhasználók számára érhetők el

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|SubscriptionId|    Az előfizetés GUID azonosítója|
|SubscriptionStartDate| Az előfizetés kezdő dátuma|
|SubscriptionEndDate|   Az előfizetés befejező dátuma|
|SubscriptionState| Az előfizetés állapota (aktív vagy átadott)|
|Month (hónap)| A használat és a bevétel jelentésének hónapja|
|IsAutoRenew|   Azt jelzi, hogy az előfizetés automatikus megújítása vagy sem (i/N)|
|CustomerName|  Ügyfél neve| 
|CustomerTenantId|  Ügyfél GUID azonosítója|
|CustomerTpid|  Ügyfél elsődleges szülő-azonosítója| 
|CustomerSegment|   Az ügyfél piaci szegmense| 
|CustomerMarket|    Az ügyfél földrajzi piaca|
|Termék|   A partner által az ügyfélnek eladott termék| 
|Termékváltozat|   A termék SKU-jának száma |
|MPNId| A partner Microsoft Partner Network azonosítója |
|PartnerName|   A partner neve |
|PartnerLocation|   A partner földrajzi helye |
|PartnerAttributionType|    Az előfizetéshez tartozó Attribution-típus|
|SalesChannel|  Értékesítési csatorna (Direct/CSP stb.) |
|AvailableSeats|    Aktuálisan elérhető hely|
|RevenueUSD|    Bevétel USD-ben|
|Regisztrációs azonosító| Az előfizetés regisztrációs azonosítója|

**Azure-használat**: az Azure-használati jelentés különböző mezőinek adatdefiníciói a következők:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|SubscriptionId|    Az előfizetés GUID azonosítója|
|SubscriptionStartDate| Az előfizetés kezdetének dátuma.|
|SubscriptionEndDate|   Az előfizetés befejezésének dátuma.|
|SubscriptionState| Az előfizetés aktuális állapota (nyitott/lezárt/aktív/intürelmi időszak)|
|Month (hónap)| Dátum összesítése hónap alapján |
|ServiceName|   Az Azure-szolgáltatás neve|
|MeterCategory| A fogyasztásmérő kategóriájának neve|
|UsageUnits|    A számlázási ciklusban használt egységek száma |
|CustomerName|  Az ügyfél neve |
|CustomerTenantId|  Ügyfél bérlői azonosítója |
|CustomerTpid|  Ügyfél elsődleges szülő-azonosítója |
|CustomerSegment|   Az ügyfél szegmense |
|CustomerMarket|    Az ügyfél földrajzi piaca |
|MPNId  |Az ügyfél Microsoft Partner Network azonosítója |
|PartnerName|   A partner neve |
|PartnerLocation    |A partner földrajzi országának helye |
|PartnerAttributionType |Partneri típus|
|SalesChannel|  Értékesítések csatornája (közvetlen/CSP közvetett/CSP közvetlen stb.) |
|ACR_USD|   Az Azure által felhasznált bevétel USD-ben|
|Regisztrációs azonosító| Az Azure-előfizetés regisztrációs azonosítója|

**Office 365 – licenc használata**: az Office 365-licencek használati jelentésének különböző mezőinek adatdefiníciói a következők:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|CustomerTenantId|  Ügyfél bérlői azonosítója| 
|CustomerTpid|  Ügyfél elsődleges szülő-azonosítója |
|WorkloadName|  SFB, csapatok, EXO |
|Month (hónap)| Az a hónap, amelynek a felhasználását jelenteni kell|
|PaidAvailableUnits|    Fizetős rendelkezésre álló egységek száma|
|MonthlyActiveUsers|    Havi aktív felhasználók száma|
|CustomerName|  Az ügyfél neve|
|CustomerMarket|    Az ügyfél piacának földrajzi országbeli helye |
|CustomerSegment|   Felhasználói szegmens |
|MPNId| Microsoft Partner Network azonosítója|
|PartnerName|   A partner neve|
|PartnerLocation|   Partner földrajzi helye|
|PartnerAttributionType|    Partneri típus|

**Nagyvállalati mobilitás – licencek használata**: az EMS – licenc-használati jelentés különböző mezőinek adatdefiníciója:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|CustomerTenantId|  Ügyfél bérlői azonosítója| 
|CustomerTpid|  Ügyfél elsődleges szülő-azonosítója |
|WorkloadName|  Az EMS munkaterhelésének neve |
|Month (hónap)| Az a hónap, amelynek a felhasználását jelenteni kell|
|PaidAvailableUnits|    Fizetős rendelkezésre álló egységek száma|
|MonthlyActiveUsers|    Havi aktív felhasználók száma|
|CustomerName|  Az ügyfél neve|
|CustomerMarket|Az ügyfél piacának földrajzi országbeli helye |
|CustomerSegment|   Felhasználói szegmens |
|MPNId| Microsoft Partner Network azonosítója|
|PartnerName|   A partner neve|
|PartnerLocation|   Partner földrajzi helye|
|PartnerAttributionType|    Partneri típus|

**Dynamics 365 – licenc-használat**: a Dynamics 365 – licenc-használati jelentés különböző mezőinek adatdefiníciója:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|SubscriptionId|Az előfizetés GUID azonosítója|
|SubscriptionStartDate| Az előfizetés kezdő dátuma|
|SubscriptionEndDate|   Az előfizetés befejező dátuma|
|SubscriptionStatus|    Az előfizetés állapota |
|Month (hónap)| Az a hónap, amelynek a felhasználását jelenteni kell|
|RevSumDivisionName|    A Rev Sum divízió neve|
|RevSumCategoryName|    A Rev Sum kategória neve|
|Termékváltozat|   A termék SKU-jának száma |
|SKUId| A termék SKU-azonosítója |
|FreeVsPaidSKU| Azt jelzi, hogy ingyenes vagy fizetős SKU-e |
|SalesModel|    Az előfizetés értékesítéséhez használt értékesítési csatorna|
|DetailedSalesModel|    Az előfizetés részletes értékesítési modellje|
|CustomerName|  Ügyfél neve |
|CustomerTenantId|  Ügyfél bérlője GUID |
|CustomerTpid|  Ügyfél elsődleges szülő-azonosítója |
|CustomerSegment|   Az ügyfél piaci szegmense |
|CustomerMarket|    Az ügyfél földrajzi piaca |
|MPNId| Microsoft Partner Network-azonosító |
|PartnerName|   A partner neve |
|PartnerLocation|   A partner földrajzi országának helye |
|PartnerAttachType| Az előfizetéshez tartozó Attribution-típus|
|AvailableSeats|    Aktuálisan elérhető hely|
|AssignedSeats| Aktuálisan hozzárendelt ülőhely |
|ActiveSeats|   Aktuális aktív helyek |
|DeploymentOpportunity| Aktuális üzembe helyezési lehetőség|
|ActiveUsagePercent|    Aktuális aktív használat százaléka|
 
**Power bi licenc használata**: a Power bi különböző mezőinek adatdefiníciója a licencek használati jelentése:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|SubscriptionId|    Az előfizetés GUID azonosítója|
|SubscriptionStartDate| Az előfizetés kezdő dátuma|
|SubscriptionEndDate|   Az előfizetés befejező dátuma|
|SubscriptionStatus|    Az előfizetés állapota (aktív vagy In-Active vagy türelmi időszak)|
|Month (hónap)| Dátum összesítése hónap alapján |
|Termékváltozat|   A termék SKU-jának száma |
|SKUId| A termék SKU-azonosítója |
|FreeVsPaidSKU| Ingyenes vagy fizetős SKU differenciáló |
|SalesModel|    Az előfizetés értékesítéséhez használt értékesítési modell|
|DetailedSalesModel|    Az előfizetés részletes értékesítési modellje|
|CustomerName|  Ügyfél neve |
|CustomerTenantId|  Ügyfél bérlője GUID |
|CustomerTpid|  Ügyfél elsődleges szülő-azonosítója| 
|CustomerSegment|   Az ügyfél piaci szegmense |
|CustomerMarket|    Az ügyfél földrajzi piaca |
|MPNId| Microsoft Partner Network azonosítója |
|PartnerName|   A partner neve |
|PartnerLocation|   A partner földrajzi országának helye |
|PartnerAttachType| Az előfizetéshez tartozó Attribution-típus|
|AvailableSeats|    Aktuálisan elérhető helyek|
|AssignedSeats| Aktuálisan hozzárendelt helyek|
|ActiveSeats|   Aktuális aktív helyek|
|DeploymentOpportunity| Aktuális üzembe helyezési lehetőség|
|ActiveUsagePercent|    Aktuális aktív használat százaléka|

**Csapatok használata – értekezletek és hívások**: a különböző mezők adatdefiníciói a következők:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|CustomerTenantId|  Ügyfél bérlői azonosítója |
|CustomerTpid|  Ügyfél elsődleges szülő-azonosítója |
|Month (hónap)| Az a hónap, amelynek a felhasználását jelenteni kell|
|Almunkaterhelés|   Azon alszámítási feladatok, amelyekről jelentés készül (értekezletek, hívások, telefonos rendszerek)|
|Értekezletek száma| Értekezletek száma|
|Értekezlet időtartama|  Értekezletek teljes időtartama (óra)|

**Csapatok – havi használati adatok**: a különböző mezők adatdefiníciói a következők:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|CustomerTenantId|  Ügyfél bérlői azonosítója |
|CustomerTpid|  Ügyfél elsődleges szülő-azonosítója |
|Month (hónap)| Az a hónap, amelynek a felhasználását jelenteni kell|
|Almunkaterhelés|   Azon alszámítási feladatok, amelyekről jelentés készül (értekezletek, hívások, telefonos rendszerek)|
|Asztali felhasználók| Az asztali csapatokat használó felhasználók száma|
|Mobilfelhasználók|  A mobil csapatokat használó felhasználók száma|
|Webes felhasználók| A web Teams szolgáltatást használó felhasználók száma|
|AllUpParticipants| A csapat különálló felhasználói száma a hónapban|

**Teams-használat – 3p-alkalmazások**: a különböző mezők adatdefiníciói a következők:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|CustomerTenantId|  Ügyfél bérlői azonosítója| 
|CustomerTpid|  Ügyfél elsődleges szülő-azonosítója |
|Month (hónap)| Az a hónap, amelynek a felhasználását jelenteni kell|
|3P-alkalmazás neve|   A Teams alkalmazás neve|
|Felhasználók száma|    Az alkalmazáshoz tartozó felhasználók száma|


**Képzés részletei**: a betanítási részletek jelentés különböző mezőinek adatdefiníciói a következők:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|TrainingActivityId|    A képzés azonosítója |
|TrainingTitle| A képzés címe |
|TrainingType|  Képzés típusa (minősítés/vizsga)|
|IndividualFirstName|   Az ügyfél keresztneve| 
|IndividualLastName|    Az ügyfél vezetékneve| 
|E-mail| Az ügyfél személyes e-mail-azonosítója|
|CorpEmail| Ügyfél Office e-mail azonosítója|
|TrainingCompletionDate|    A képzés befejezési dátuma |
|Month (hónap)| Az adatgyűjtés hónapja|
|IcMCP| Azt jelzi, hogy a felhasználó Microsoft Certified Professional|
|MCPID| A felhasználó MCP-azonosítója|
|MPNId| Microsoft Partner Network azonosítója |
|PartnerName|   A partner neve |
|PartnerCityLocation|   A partner földrajzi városának helye |
|PartnerCountryLocation|    A partner földrajzi országának helye |

**Microsoft Learn**: a Microsoft Learn jelentés különböző mezőinek adatdefiníciói a következők:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|Felhasználónév|A felhasználó neve| 
|UserId (Felhasználóazonosító)|Felhasználói GUID |
|TrainingName|A képzés neve |
|TrainingType|Képzés típusa (modul/learning útvonala)|
|Termékek|Az a termék, amelyre a tanulási modul alkalmazható|
|Szerepkörök|A képzés megfelelő szerepkörei |
|CompletionDate|A képzés befejezésének dátuma |
|MPNId|Microsoft Partner Network azonosítója |
|PartnerName|A partner neve |
|Ország|A partner földrajzi országának helye |

**Kompetenciák összegzése és előzményei**: a kompetenciák összegzése és előzményei jelentés különböző mezőinek adatdefiníciója a következők:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|CompetencyName|A kompetencia neve |
|CompetencyLevel|Kompetencia szintje (Gold/Silver)|
|CompetencyStatus|Kompetencia aktuális állapota (aktív/inaktív/türelmi időszak)|
|CompetencyStartDate|Az adott kompetencia kezdési dátuma| 
|CompetencyEndDate|Az adott kompetencia befejezési dátuma |

**Kompetencia-teljesítmény**: a kompetencia-teljesítmény jelentés különböző mezőinek adatdefiníciói a következők:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|CompetencyName|    A kompetencia neve |
|CompetencyAttainmentOptionName|    A kompetencia-elérési lehetőség neve|
|Month (hónap)| A metrikák jelentésének hónapja|
|MetricName|    A kompetenciához kapcsolódó metrika neve|
|MetricMonthlyContribution| A metrika havi hozzájárulása|
|TTMAggregate|  A záró 12 hónapos időszak összesített mérőszáma|
|AnniversaryYearAggregate|  Az aktuális évfordulós év összesített mérőszáma|
|GoldThreshold| A Gold kompetenciát kielégítő teljesítményre vonatkozó követelmény|
|SilverThreshold|   Az Silver kompetencia teljesítésének követelménye|

**Cloud megmászás – M365-hajlam**: a Cloud megmászás – M365-alapú adatkezelési jelentés különféle mezőinek adatdefiníciói:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|MPN-azonosító|    Microsoft Partner Network azonosítója|
|Partner neve|  A partner neve|
|Ügyfél-azonosító|   Ügyfél-azonosító száma |
|DUNS-szám|   A Dun & Bradstreettől száma, amelyet a rendszer a kiértékeléshez|
|Fiók neve|  A fiók neve |
|Tartomány|    A fiók tartománya|
|Szervezeti méret|  Szervezet mérete|
|Iparág|  Iparág  |
|Függőleges|  A Microsoft és az egyéb iparági szabványok alapján (D&B) azonosított ügyfél vertikális értéke|
|Terület|  A hely földrajzi területe|
|Leányvállalat|    Az ügyfél leányvállalata, amelynek a kiértékelése megtörténik|
|Sales Territory|   Az ügyfél értékesítési területe, amely a kiértékeléshez van kiértékelve|
|City|  Földrajzi város helye |
|Állam| Földrajzi állapot helye|
|Irányítószám|   Irányítószám|
|Ország|   Földrajzi ország helye |
|Segment|   Piaci szegmens |
|Alszegmens|   Piaci alszegmens |
|SMC-típus összegzése|  SMC-típus |
|Leggyakoribb nem felügyelt számítási alap|  Leggyakoribb nem felügyelt ügyfelek – számítás|
|Leggyakoribb nem felügyelt – felhasználói bázis| Leggyakoribb nem felügyelt ügyfelek – felhasználó|
|IsNonProfit|   Akár nonprofit, akár haszon (igen/nem)|
|Távoli munka engedélyezése – az Exchange Online megcélzása|   Azok az ügyfelek, akik aktív Exchange Online-előfizetéssel rendelkeznek, upsell to M365|
|A helyszíni helyszíni beszerzések (jelenlegi verzió) engedélyezése a klasszikus és a 10 licenccel|Az a felhasználó, aki aktuális helyszíni Office-vagy Win-ügyféllel rendelkezik (azaz az EOS-termékek után). Az ügyfél 10 vagy több licenccel rendelkezik. Az a felhasználó, aki a feldolgozói pontszámmal rendelkezik. A partnereknek a M365 való átalakításra kell célozniuk.|
|A helyszíni helyszíni beszerzések (aktuális verzió) használatának engedélyezése a klasszikus <10 licenccel|Az a felhasználó, aki aktuális helyszíni Office-vagy Win-ügyféllel rendelkezik (azaz az EOS-termékek után). Az ügyfél kevesebb mint 10 licenccel rendelkezik. Az a felhasználó, aki a feldolgozói pontszámmal rendelkezik. A partnereknek a M365 való átalakításra kell célozniuk.|
|Helyszíni helyszíni beszerzések (aktuális verzió) használatának engedélyezése a klasszikus teljesítmény nélkül – + 10 licenc| Az a felhasználó, aki aktuális helyszíni Office-vagy Win-ügyféllel rendelkezik (azaz az EOS-termékek után). Az ügyfél 10 vagy több licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek a M365 való átalakításra kell célozniuk.|
|Helyszíni helyszíni beszerzések (aktuális verzió) engedélyezése a klasszikus környezetek nélkül – <10 licenc| Az a felhasználó, aki aktuális helyszíni Office-vagy Win-ügyféllel rendelkezik (azaz az EOS-termékek után). Az ügyfél kevesebb mint 10 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek a M365 való átalakításra kell célozniuk.|
|A távoli munkahelyi helyszíni vásárlás engedélyezése (EOS) a klasszikus feldolgozóval – + 10 licenc|Az a felhasználó, aki az EOS helyszíni Office-vagy a Win-ügyfelet tartalmazza (azaz az EOS-termékek megkezdése előtt és után). Az ügyfél 10 vagy több licenccel rendelkezik. Az ügyfélnek van egy megállási pontszáma. A partnereknek a M365 való átalakításra kell célozniuk.|
|A távoli munkahelyi helyszíni vásárlás engedélyezése (EOS) a klasszikus <10 licenccel|Az a felhasználó, aki az EOS helyszíni Office-vagy a Win-ügyfelet tartalmazza (azaz az EOS-termékek megkezdése előtt és után). Az ügyfél kevesebb mint 10 licenccel rendelkezik. Az ügyfélnek van egy megállási pontszáma. A partnereknek a M365 való átalakításra kell célozniuk.|
|A helyszíni helyszíni beszerzések (EOS) használatának engedélyezése a klasszikus teljesítmény nélkül – + 10 licenc| Az a felhasználó, aki a jelenlegi helyszíni Office-vagy Win-ügyféllel rendelkezik (azaz az EOS-termékek megkezdése előtt és után is). Az ügyfél 10 vagy több licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek a M365 való átalakításra kell célozniuk.|
|Távoli munkahelyi helyszíni vásárlás engedélyezése (EOS) a klasszikus környezetek nélkül – <10 licenc| Az a felhasználó, aki a jelenlegi helyszíni Office-vagy Win-ügyféllel rendelkezik (azaz az EOS-termékek megkezdése előtt és után is). Az ügyfél kevesebb mint 10 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek a M365 való átalakításra kell célozniuk.|
|Távoli munka engedélyezése – magas szintű M365 (cselekedjen most/kiértékelés)| A M365 nagy hajlandóságot biztosít az ügyfelek számára.|
|Távoli működés engedélyezése (nagyítás) a M365| Nagyítással és M365 rendelkező ügyfelek, csoportokba való átalakítás céljával|
|Távoli működés engedélyezése (nagyítás) M365 nélkül|  A csapatoknak való átalakításra tervezett nagyítással rendelkező ügyfelek|
|Csökkentse a költségeket és a felügyeletet – az M365 E3 a M365 E5 célját célozza meg| Meglévő ügyfél, M365 E3, cél: M365 E5|
|Csökkentse a költségeket és a felügyeletet – a M365 BB és a BS ügyfeleinek szánt M365 BP|    Meglévő M365 BB és BS ügyfelek, a cél a M365 BP|
|A szervezeti termelékenység átalakítása – felszíni hajlam|    Az ügyfél felszínre való hajlamot mutat.|
|M365Cluster|Azonosítja az ügyfél M365 megvásárlására való hajlamot.  A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|M365Fit|   A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás a legjobb SMB modell használatával hasonlítja össze az ügyfeleket, és megtudhatja, hogy lehetséges-e a Microsoft Cloud termékekhez való illeszkedés. Az illesztési pontozás negyedévente frissül.|
|M365Intent|    A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül.|
|SurfaceCluster|    Ez azonosítja az ügyfél megvásárlásának feltételeit úgy, hogy összevonta a megfelelő és szándékú javaslatokat egy fürtbe.  A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|SurfaceFit|    A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás a legjobb SMB modell használatával hasonlítja össze az ügyfeleket, és megtudhatja, hogy lehetséges-e a Microsoft Cloud termékekhez való illeszkedés. Az illesztési pontozás negyedévente frissül.|
|SurfaceIntent| A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül.|
|O365Cluster|   Ez azonosítja az ügyfélnek a O365 megvásárlására való hajlamát.  A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|O365Fit|   A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás a legjobb SMB modell használatával hasonlítja össze az ügyfeleket, és megtudhatja, hogy lehetséges-e a Microsoft Cloud termékekhez való illeszkedés. Az illesztési pontozás negyedévente frissül.|
|O365Intent|    A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül.|
|M365UpsellCustomer|    Ez azonosítja, hogy az ügyfél a M365 upsell-hajlamot jelenít meg|
|A Google|    Ez a jelző azonosítja, hogy az ügyfél versenyképes jeleket mutat-e a Google-termékek tulajdonosának|
|AWS|   Ez a jelző azonosítja, hogy az ügyfél versenyképes jeleket mutat-e az AWS-termékek tulajdonosának|
|EA|    Ez azonosítja, hogy a megújítás nagyvállalati szerződés (EA) vagy EA-előfizetés|
|Nyitva van|  Ez határozza meg, hogy a megújítás nyitott vagy nyitott értékű szerződés-e|

**Cloud megmászás – D365-hajlam**: a Cloud megmászás – D365-alapú adatkezelési jelentés különféle mezőinek adatdefiníciói:

| **Oszlop neve** | **Az adatleírás** |
|---------|:---------|
|MPN-azonosító|    Microsoft Partner Network azonosítója|
|Partner neve|  A partner neve|
|Ügyfél-azonosító|   Ügyfél-azonosító száma |
|DUNS-szám|   A Dun & Bradstreettől száma, amelyet a rendszer a kiértékeléshez|
|Fiók neve|  A fiók neve |
|Tartomány|    A fiók tartománya|
|Szervezeti méret|  Szervezet mérete|
|Iparág|  Iparág  |
|Függőleges|  A Microsoft és az egyéb iparági szabványok alapján (D&B) azonosított ügyfél vertikális értéke
|Terület|  A hely földrajzi területe|
|Leányvállalat|    Az ügyfél leányvállalata, amelynek a kiértékelése megtörténik|
|Sales Territory|   Sales Territory|
|City|  Földrajzi város helye |
|Állam| Földrajzi állapot helye|
|Irányítószám|   Irányítószám|
|Ország|   Földrajzi ország helye |
|Segment|   Piaci szegmens |
|Alszegmens|   Piaci alszegmens |
|SMC-típus összegzése|  Az ügyfél kategorizálása: az első nem felügyelt felhasználói bázisok a 300-nál több alkalmazottat foglalkoztató ügyfelek, a legfelső szintű nem felügyelt számítási alapértékek az Azure 3 éves verziójában a $10k-mel rendelkező ügyfelek|
|Leggyakoribb nem felügyelt számítási alap   |Leggyakoribb nem felügyelt ügyfelek – számítás|
|Leggyakoribb nem felügyelt – felhasználói bázis| Leggyakoribb nem felügyelt ügyfelek – felhasználók|
|IsNonProfit|   Akár nonprofit, akár haszon (igen/nem)|
|Digitális értékesítés-M365-ülőke méretének aktiválása >= 25 ülőhely (SalesPro-alapú modell)|   Az ügyfél D365 nélkül. Ülőhely mérete: 25 +. A partnereknek meg kell célozniuk a D365-Salespro értékesítését|
|A digitális értékesítés – D365 SalesPro-hajlam aktiválása (cselekedjen most/kiértékelés) |Nagy teljesítményű ügyfelek D365 nélkül.  A partnereknek meg kell célozniuk a D365 SalesPro.|
|Pénzügyi kockázat & csalás – Dynamics helyszíni telepítési alap – Navision (a BC-modell)|Meglévő ügyfél a helyszíni Navision programban.  A partnernek a BC D365 kell megcéloznia|
|Pénzügyi kockázat & csalás – Dynamics helyszíni telepítési alap – AX (F&O-alapú előfizetési modell)    |Meglévő ügyfél a helyszíni AX-vel.  A partnernek az F&O D365 kell megcéloznia|
|Pénzügyi kockázatok & csalás – Dynamics helyszíni telepítési alap – nagyszerű síkságok (BC-alapú modell)|  A meglévő ügyfél helyszíni nagyszerű Síkságokkal rendelkezik.  A partnernek a BC D365 kell megcéloznia|
|Pénzügyi kockázat & csalás – Dynamics helyszíni telepítési alap – Salamon (a BC-modell)|Meglévő ügyfél a helyszíni Salamon-val.  A partnernek a BC D365 kell megcéloznia|
|Pénzügyi kockázatok & csalás – a Dynamics helyszíni telepítési alapja – egyebek (a BC-modell) |Meglévő ügyfél más, a fentiekben nem felsorolt helyszíni-megoldásokkal.  A partnernek a BC D365 kell megcéloznia|
|Agilis üzleti folyamatok létrehozása – a Dynamics helyszíni telepítési alap-AX/GP/SL/NAV/other (D365-alapú adatfeldolgozási modell)|   Agilis üzleti folyamatok létrehozása – a Dynamics helyszíni telepítési alap-AX/GP/SL/NAV/other (D365-alapú adatfeldolgozási modell)|
|Agilis üzleti folyamatok létrehozása – Dynamics verseny alapja – Mendix/Salesforce/(D365-alapú modell)| Agilis üzleti folyamatok létrehozása – Dynamics verseny alapja – Mendix/Salesforce/(D365-alapú modell)|
|Agilis üzleti folyamatok létrehozása – D365 F&O telepítési alap |Meglévő D365 F&O-ügyfelek.  Partner a Power apps megcélzásához.|
|Agilis üzleti folyamatok készítése – D365 BC telepítési alapja| Meglévő D365 BC-ügyfelek. Partner a Power apps megcélzásához.|
|Agilis üzleti folyamatok létrehozása – D365 CE telepítési alap| Meglévő D365 CE-ügyfelek. Partner a Power apps megcélzásához.|
|Hozzon létre egy rugalmas ellátási láncot – nyerjen és aktiválja az első D365 számítási feladatot D365-ellátási láncként a nem Oracle/SAP ERP-ügyfelekkel|  A D365-ellátási lánc ügyfeleinek megcélzása.|
|Rugalmas ellátási lánc létrehozása – D365-ellátási lánc és/vagy kereskedelmi forgalom és kereskedelem a meglévő D365 CE-ügyfelek számára |Meglévő D365 CE-ügyfelek, amelyek a D365-ellátási láncot adják át|
|Hozzon létre egy rugalmas ellátási láncot, amely több értékesítésre D365 sup-t biztosít. Lánc és/vagy kiskereskedelmi/kereskedelmi D365 CE és (Oracle vagy SAP)| Meglévő D365 CE-ügyfelek Oracle vagy SAP használatával a D365-ellátási lánc megcélzásához|
|D365BCCluster| Ez azonosítja az ügyfélnek a D365 Business Central vásárlására való hajlamát.  Azok az ügyfelek, akik a BC-vel való hajlamot mutatják, közepes és kis kategóriába kerülnek.  A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|D365BCFit| A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás a legjobb SMB modell használatával hasonlítja össze az ügyfeleket, és megtudhatja, hogy lehetséges-e a Microsoft Cloud termékekhez való illeszkedés. Az illesztési pontozás negyedévente frissül.|
|D365BCIntent|  A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül.|
|D365FOCluster| Ez azonosítja az ügyfél által a D365 pénzügyi és üzemeltetési műveletek megvásárlására való hajlamot.  Az F&O-re való hajlamot mutató ügyfelek a legfelső szintű nem felügyelt kategóriákba kerülnek. A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|D365FOFit| A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás a legjobb SMB modell használatával hasonlítja össze az ügyfeleket, és megtudhatja, hogy lehetséges-e a Microsoft Cloud termékekhez való illeszkedés. Az illesztési pontozás negyedévente frissül.|
|D365FOIntent|  A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül.|
|D365CECluster| Ez azonosítja az ügyfélnek a D365 vásárlói részvétel megvásárlására való hajlamát.  A CE-vel való elállást bemutató ügyfelek közepes és kis kategóriába kerülnek.  A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|D365CEFit| D365 CE-hez igazítás|
|D365CEIntent|  A D365 CE szándéka|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Ez azonosítja, hogy az ügyfél rendelkezik-e nyílt megújítással a Dynamics on-Prem AX vagy a CRM esetében.|
|M365UpsellCustomer|    Ez azonosítja, hogy az ügyfél a M365 upsell-hajlamot jelenít meg|
|A Google|    Ez a jelző azonosítja, hogy az ügyfél versenyképes jeleket mutat-e a Google-termékek tulajdonosának|
|AWS|   Ez a jelző azonosítja, hogy az ügyfél versenyképes jeleket mutat-e az AWS-termékek tulajdonosának|
|EA |Ez azonosítja, hogy a megújítás nagyvállalati szerződés (EA) vagy EA-előfizetés|
|Nyitva van|  Ez határozza meg, hogy a megújítás nyitott vagy nyitott értékű szerződés-e|

**Cloud Ascent-Azure-hajlam**: a Cloud Ascent-Azure-alapú adatkezelési jelentés különböző mezőinek adatdefiníciói a következők:

|**Oszlop neve** |**Az adatleírás** |
|---------|:---------|
|MPN-azonosító|    Microsoft Partner Network azonosítója|
|Partner neve|  A partner neve|
|Ügyfél-azonosító|   Ügyfél-azonosító száma |
|DUNS-szám|   A Dun & Bradstreettől száma, amelyet a rendszer a kiértékeléshez|
|Fiók neve|  A fiók neve |
|Tartomány|    A fiók tartománya|
|Szervezeti méret|  Szervezet mérete|
|Iparág|  Iparág  |
|Függőleges|  A Microsoft és az egyéb iparági szabványok alapján (D&B) azonosított ügyfél vertikális értéke|
|Terület|  A hely földrajzi területe|
|Leányvállalat|    Az ügyfél leányvállalata, amelynek a kiértékelése megtörténik|
|Sales Territory|   Sales Territory|
|City|  Földrajzi város helye |
|Állam| Földrajzi állapot helye|
|Irányítószám|   Irányítószám|
|Ország|   Földrajzi ország helye |
|Segment|   Piaci szegmens |
|Alszegmens|   Piaci alszegmens |
|SMC-típus összegzése|  SMC-típus |
|Leggyakoribb nem felügyelt számítási alap|  Leggyakoribb nem felügyelt ügyfelek – számítás|
|Leggyakoribb nem felügyelt – felhasználói bázis| Leggyakoribb nem felügyelt ügyfelek – felhasználók|
|IsNonProfit|   Akár nonprofit, akár haszon (igen/nem)|
|Migrálás-EOS Win Server-EOS Windows Server IB a klasszikus feladataival – 5 + licenc|   Az a felhasználó, aki a (z) EOS on-Prem Win-kiszolgálóval rendelkezik (ez az a verzió, amely az EOS-termékeket is tartalmazza). Az ügyfél 5 vagy több licenccel rendelkezik. Az a felhasználó, aki a feldolgozói pontszámmal rendelkezik.  A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás-EOS Win Server-EOS Windows Server IB a klasszikus <5 licenccel|   Az a felhasználó, aki a (z) EOS (a szolgáltatás végén) helyszíni Win-kiszolgálót (azaz a (z) és az EOS-termékeket is beleértve) tartalmazza. Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az a felhasználó, aki a feldolgozói pontszámmal rendelkezik.  A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás-EOS Win Server-EOS Windows Server IB a klasszikus teljesítmény nélkül – 5 + licenc |Az a felhasználó, aki a (z) EOS on-Prem Win-kiszolgálóval rendelkezik (ez az a verzió, amely az EOS-termékeket is tartalmazza). Az ügyfél több mint 5 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás-EOS Win Server-EOS Windows Server IB a klasszikus hajlam nélkül – <5 licenc|    Az a felhasználó, aki a (z) EOS on-Prem Win-kiszolgálóval rendelkezik (ez az a verzió, amely az EOS-termékeket is tartalmazza). Kevesebb mint 5 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás-EOS SQL-EOS SQL Server IB-vel, klasszikus szintű, 5 + licenccel|  Az a felhasználó, aki rendelkezik az EOS on-SQL Server (azaz az EOS-termékekkel megelőzően telepített verziókkal). Az ügyfél 5 licenctel rendelkezik. Az ügyfélnek van egy megállási pontszáma.  A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás-EOS SQL-EOS SQL Server IB-vel, klasszikus szintű, <5 licenccel|  Az a felhasználó, aki rendelkezik az EOS on-SQL Server (azaz az EOS-termékekkel megelőzően telepített verziókkal). Kevesebb mint 5 licenccel rendelkezik. Az a felhasználó, aki a feldolgozói pontszámmal rendelkezik. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás-EOS SQL-EOS SQL Server IB-t a klasszikus teljesítmény nélkül – 5 + licenc|   Az a felhasználó, aki rendelkezik az EOS on-SQL Server (azaz az EOS-termékekkel megelőzően telepített verziókkal). Az ügyfél 5 vagy több licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás-EOS SQL-EOS SQL Server IB-t a klasszikus hajlam nélkül – <5 licenc|   Az a felhasználó, aki rendelkezik az EOS on-SQL Server (azaz az EOS-termékekkel megelőzően telepített verziókkal). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – helyszíni Win-kiszolgáló áttelepíteni – jelenlegi Windows Server IB|   Az a felhasználó, aki aktuális helyszíni Win-kiszolgálóval rendelkezik (azaz az EOS-termékek után). Az ügyfél 5 licenctel rendelkezik. Az ügyfélnek van egy megállási pontszáma. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – helyszíni Win-kiszolgáló áttelepíteni – jelenlegi Windows Server <IB|   Az a felhasználó, aki aktuális helyszíni Win-kiszolgálóval rendelkezik (azaz az EOS-termékek után). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfélnek van egy, az Azure-hoz való kiértékelési pontszáma. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – helyszíni Win-kiszolgáló áttelepíteni – a Windows Server IB jelenlegi verziójának hiánya a klasszikus teljesítmény – 5 + licenc nélkül|    Az a felhasználó, aki aktuális helyszíni Win-kiszolgálóval rendelkezik (azaz az EOS-termékek után). Az ügyfél 5 licenctel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – helyszíni Win-kiszolgáló áttelepíteni – a Windows Server IB jelenlegi verziójának hiánya a klasszikus hajlam nélkül – <5 licenc |Az a felhasználó, aki aktuális helyszíni Win-kiszolgálóval rendelkezik (azaz az EOS-termékek után). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – áttelepítés Azure SQL-vagy SQL-alapú virtuális gépekre – jelenlegi SQL Server IB-vel – 5 + licenc|  Az a felhasználó, aki aktuális helyszíni SQL Server (azaz az EOS-termékek utáni verziókat). Az ügyfél 5 licenctel rendelkezik. Az ügyfélnek van egy megállási pontszáma. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – áttelepítés Azure SQL <SQL Server-vagy SQL-alapú virtuális gépekre|  Az a felhasználó, aki aktuális helyszíni SQL Server (azaz az EOS-termékek utáni verziókat). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfélnek van egy megállási pontszáma. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – Migrálás Azure SQL-vagy SQL-alapú virtuális gépekre – jelenlegi SQL Server i/b|   Az a felhasználó, aki aktuális helyszíni SQL Server (azaz az EOS-termékek utáni verziókat). Az ügyfél 5 licenctel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – Migrálás Azure SQL-vagy SQL-alapú virtuális gépekre – jelenlegi SQL Server i/<b.|   Az a felhasználó, aki aktuális helyszíni SQL Server (azaz az EOS-termékek utáni verziókat). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – OSS – áttelepítés OSS-ADATBÁZISba| Meglévő ügyfél a következő versengő termékek valamelyikével: PostgreSQL, MySQL, MariaDB. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás-OSS-Linux az Azure-on |Meglévő ügyfél a termékkel: Linux. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás-SAP-SAP az Azure-on|  Meglévő ügyfél a termékkel: SAP. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás-WVD-RDS IB |Az aktív Windows Távoli asztali szolgáltatások ügyfeleket azonosítja. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – WVD – modern munka átadása az Azure-ba/WVD|   Azonosítja az ügyfeleket a M365, és nem rendelkezik az Azure-val. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – VMware IB|   Meglévő ügyfél a termékkel: VMware. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Migrálás – Citrix IB|   Meglévő ügyfél a termékkel: Citrix Systems. A partnereknek ezeket az ügyfeleket az Azure-ba való Migrálás céljára kell célozni|
|Innováció – elemzés – Power BI IB-n/magas Azure-beli hajlam|   A és az aktív Power BI-előfizetéssel rendelkező ügyfelek, beleértve a következőket: Power BI-önálló Pro, Power BI-Azure Suite, Power BI-Office Suite, Power BI Suite-M365|
|Enable-DevOps a GitHub-VisualStudio/MSDN IB-vel|    Aktív Visual Studióval rendelkező ügyfelek azonosítva|
|A Win Server standard verziója|   Ez az ügyfél a Windows Server standard vásárlások verzióját jeleníti meg|
|A Win Server standard licence|   Ez az ügyfél a Windows Server standard vásárlások licencének típusát jeleníti meg|
|A Server adatközpont-verziójának megnyerése|    Ez a Windows adatközpont-vásárlások által az ügyfél által vásárolt verziót mutatja.|
|Win Server adatközpont-licenc| Az ügyfél által vásárolt Windows adatközpont-vásárlások licencelési típusát mutatja.|
|AzureFit|  A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás a legjobb SMB modell használatával hasonlítja össze az ügyfeleket, és megtudhatja, hogy lehetséges-e a Microsoft Cloud termékekhez való illeszkedés. Az illesztési pontozás negyedévente frissül.|
|AzureIntent|   A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül.|
|AzureCluster|  Ez azonosítja az ügyfél által az Azure megvásárlására való hajlamot úgy, hogy összevonta a megfelelő és szándékú javaslatokat egy fürtbe.  A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|WindowsServerDataCenter_HasOpenRenewal|    Ez azonosítja, hogy egy ügyfél nyitott megújítással rendelkezik-e a Windows Server adatközponthoz|
|WindowsServerStandard_HasOpenRenewal|  Ez azonosítja, hogy egy ügyfél nyitott megújítással rendelkezik-e a Windows Server Standard rendszerhez|
|AzureUpsellCustomer|   Ez azonosítja, ha az ügyfél az Azure-beli upsell-hajlamot jeleníti meg|
|A Google|    Ez a jelző azonosítja, hogy az ügyfél versenyképes jeleket mutat-e a Google-termékek tulajdonosának|
|AWS|   Ez a jelző azonosítja, hogy az ügyfél versenyképes jeleket mutat-e az AWS-termékek tulajdonosának|
|EA |Ez azonosítja, hogy a megújítás nagyvállalati szerződés (EA) vagy EA-előfizetés|
|Nyitva van|  Ez határozza meg, hogy a megújítás nyitott vagy nyitott értékű szerződés-e|

**Cloud Ascent-Agreement megújítási hajlandóság**: a felhőalapú átfedések – szerződés megújítási jelentés különböző mezőinek adatdefiníciói a következők:

|**Oszlop neve** |**Az adatleírás** |
|---------|:---------|
|MPN-azonosító|    Microsoft Partner Network azonosítója|
|Partner neve|  A partner neve|
|Ügyfél-azonosító|   Ügyfél-azonosító száma |
|DUNS-szám|   A Dun & Bradstreettől száma, amelyet a rendszer a kiértékeléshez|
|Fiók neve|  A fiók neve |
|Tartomány|    A fiók tartománya|
|Szervezeti méret|  Szervezet mérete|
|Iparág|  Iparág  |
|Függőleges|  A Microsoft és az egyéb iparági szabványok alapján (D&B) azonosított ügyfél vertikális értéke|
|Terület|  A hely földrajzi területe|
|Leányvállalat|    Az ügyfél leányvállalata, amelynek a kiértékelése megtörténik|
|Sales Territory|   Sales Territory|
|City|  Földrajzi város helye |
|Állam| Földrajzi állapot helye|
|Irányítószám|   Irányítószám|
|Ország|   Földrajzi ország helye |
|Segment|   Piaci szegmens |
|Alszegmens|   Piaci alszegmens |
|SMC-típus összegzése|  SMC-típus |
|Leggyakoribb nem felügyelt számítási alap|  Leggyakoribb nem felügyelt ügyfelek – számítás|
|Leggyakoribb nem felügyelt – felhasználói bázis| Leggyakoribb nem felügyelt ügyfelek – felhasználók|
|IsNonProfit|Akár nonprofit, akár haszon (igen/nem)|
|A Google|Ez a jelző azonosítja, hogy az ügyfél versenyképes jeleket mutat-e az AWS-termékek tulajdonosának|
|AWS|Ez a jelző azonosítja, hogy az ügyfél versenyképes jeleket mutat-e az AWS-termékek tulajdonosának|
|Azure-fürt|Ez azonosítja az ügyfél által az Azure megvásárlására való hajlamot.  A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|D365 F&O-fürt|  Ez azonosítja az ügyfél által a D365 pénzügyi és üzemeltetési műveletek megvásárlására való hajlamot.  Az F&O-re való hajlamot mutató ügyfelek a legfelső szintű nem felügyelt kategóriákba kerülnek.  A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|D365 CE-fürt|   Ez azonosítja az ügyfélnek a D365 vásárlói részvétel megvásárlására való hajlamát.  A CE-vel való elállást bemutató ügyfelek közepes és kis kategóriába kerülnek.  A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|D365 BC-fürt|   Ez azonosítja az ügyfélnek a D365 Business Central vásárlására való hajlamát.  Azok az ügyfelek, akik a BC-vel való hajlamot mutatják, közepes és kis kategóriába kerülnek.  A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|M365-fürt|  Ez azonosítja az ügyfélnek a M365 megvásárlására való hajlamát.  A fürtöket most kell megcélozni, és ki kell értékelni, hogy magasabb hozamot hozzanak létre.  Az ügyfelek bevonása és nevelése csak akkor célzott, ha a megcélzott jogi intézkedés után továbbra is fennáll a kapacitás, és értékeli az ügyfeleket.|
|Licencprogram|   Ez azonosítja a megújításhoz tartozó Licencprogram típusát|
|Szerződés azonosítója|  Szerződés azonosítója|
|Szerződés befejezési dátuma|    Szerződés befejezési dátuma |
|Lejárat típusa|   Lejárat típusa|
|Lejáró bevétel|  Lejáró előfizetésekhez kapcsolódó bevétel|
|EA|    Ez azonosítja, hogy a megújítás nagyvállalati szerződés (EA) vagy EA-előfizetés|
|Nyitva van|  Ez határozza meg, hogy a megújítás nyitott vagy nyitott értékű szerződés-e|
|Azure upsell-ügyfél| Ez azonosítja, ha az ügyfél az Azure-beli upsell-hajlamot jeleníti meg|
|M365 upsell-ügyfél|  Ez azonosítja, hogy az ügyfél a M365 upsell-hajlamot jelenít meg|
|RevSumDivisionName|    Ez azonosítja a megújításra felkészülő terméket.|

## <a name="next-steps"></a>Következő lépések

A jelentések a jelentések [letöltése](pci-download-reports.md)című részben olvashatók.
