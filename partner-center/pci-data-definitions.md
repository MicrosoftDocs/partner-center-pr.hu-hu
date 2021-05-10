---
title: Az Insights adatdefiníciói
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A dokumentum felsorolja a különböző jelentéseket és azok adatdefinícióit, amelyeket az Elemzések letöltése jelentésoldalról tölthet le.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21be5b22c453174fcb66e9409d6e26dad8e25c6b
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686347"
---
# <a name="export--data-definitions"></a>Exportálás – Adatdefiníciók 

**Megfelelő szerepkörök** 

- Jelentésmegjelenítő
- Vezetői jelentésmegjelenítő

## <a name="introduction"></a>Bevezetés 

Az Insights irányítópult Jelentések letöltése központjának használatával exportálhatja a nyers adatkészleteket. 

A különböző jelentések, amelyeket letölthet az adatdefiníciójukkal együtt, az alábbi táblázatokban vannak felsorolva: 

### <a name="partner-profile-report"></a>**Partnerprofil-jelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| MPNId | A Microsoft Partner Network (MPN) azonosítója | 
| PartnerName | A partner neve | 
| PGA_MPNId | A partner globális fiókjának MPN-azonosítója | 
| PGA_PartnerName | Partner globális fiókneve | 
| City | A partner városának helye | 
| Ország | A partner országa | 
| Hierarchiaszint | Azt jelzi, hogy globális MPN-azonosítóról vagy hely MPN-azonosítóról van-e szó | 

### <a name="customer-details-report"></a>**Ügyféladatok jelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| CustomerName | Az ügyfél neve | 
| CustomerTenantId | Az ügyfélbérlő azonosítója | 
| CustomerTpid (Ügyféltpid) | Az ügyfél legfelső szülőazonosítója | 
| CustomerSegment (Ügyfélszegment) | Ügyfélszegmens | 
| CustomerMarket | Az ügyfél földrajzi piaca | 
| CustomerStatus (Ügyfélállapot) | Ügyfélállapot (aktív vagy inaktív) | 
| Termék | Az MPN által az ügyfélnek értékesített termék: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI vagy Microsoft Azure | 
| Termékváltozat | Termékváltozat | 
| Month (hónap) | A használat és a bevétel jelentésének hónapja | 
| MPNId | A Microsoft Partner Network | 
| PartnerName | A partner neve | 
| PartnerHely | A partner földrajzi helye | 
| PartnerAttributionType | A partner forrásmegjelölési típusa | 
| SalesChannel (Értékesítési csatorna) | Értékesítési csatorna | 
| AvailableSeats (Rendelkezésre álló adatok) | Elérhető helyek | 
| RevenueUSD (BevételiusD) | Bevétel amerikai dollárban | 

### <a name="reseller-performance-report"></a>**Viszonteladói teljesítményjelentés**

> [!Note]
> A bevételi és ACR-adatok csak a vezetői jelentés megtekintői számára érhetők el.

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| ResellerMPNid | Viszonteladói Microsoft Partner Network azonosítója | 
| ResellerName | Viszonteladó neve | 
| ResellerMarket | Viszonteladó országa | 
| IndirectProviderMPNId (KözvetettproviderMPNId) | A közvetett szolgáltatói azonosító Microsoft Partner Network | 
| IndirectProviderName | Közvetett szolgáltató neve | 
| Month (hónap) | A használat és a bevétel jelentésének hónapja | 
| Termék | Terméknév | 
| SubscriptionID (Előfizetés-azonosító) | Az előfizetés azonosítója | 
| AvailableSeats (Rendelkezésre álló adatok) | Elérhető helyek száma | 
| AssignedSeats (Hozzárendelések) | Hozzárendelt helyek száma | 
| BilledRevenueUSD | Számlázható bevétel amerikai dollárban | 
| CustomerName | Az ügyfél neve | 
| CustomerTPid (Ügyfél-pont) | Az ügyfél legfelső szülőazonosítója | 
| CustomerSegment (Ügyfélszegment) | Ügyfélszegmens | 
| CustomerMarket | Az ügyfél földrajzi piaca | 
| ResellerStatus | Viszonteladó állapota | 

### <a name="subscription-details-report"></a>**Előfizetés részletei jelentés**

>[!Note]
>A bevételi és ACR-adatok csak a vezetői jelentés megtekintői számára érhetők el.

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| SubscriptionId | Az előfizetés GUID-ja | 
| SubscriptionStartDate (Előfizetés kezdődátuma) | Az előfizetés kezdő dátuma | 
| SubscriptionEndDate (Előfizetési időszak) | Az előfizetés záró dátuma | 
| SubscriptionState (Előfizetési állam) | Az előfizetés állapota (aktív vagy lemorzsolódásos) | 
| Month (hónap) | A használat és a bevétel jelentésének hónapja | 
| IsAutoRenew | Azt jelzi, hogy az előfizetés automatikusan új -e (Igen vagy Nem) | 
| CustomerName | Az ügyfél neve | 
| CustomerTenantId | Az ügyfél GUID-ja | 
| CustomerTpid (Ügyféltpid) | Ügyfél legfelső szülőazonosítója | 
| Ügyfélszegmentálás | Az ügyfél piaci szegmense | 
| CustomerMarket (Ügyfél-piaci) | Az ügyfél földrajzi piaca | 
| Termék | A partner által az ügyfélnek eladott termék | 
| Termékváltozat | A termék termékváltozata | 
| MPNId | Microsoft Partner Network partner azonosítója | 
| PartnerName | A partner neve | 
| PartnerHely | A partner földrajzi helye | 
| PartnerAttributionType | Az előfizetés forrásmegjelölési típusa | 
| SalesChannel (Értékesítések csatorna) | Az értékesítés csatornája – Közvetlen, CSP (Felhőszolgáltató) és így tovább | 
| AvailableSeats (Rendelkezésre álló adatok) | Aktuálisan elérhető hely | 
| RevenueUSD | Bevétel amerikai dollárban | 
| Regisztrációs azonosító | Az előfizetés regisztrációs azonosítója | 

### <a name="azure-usage-report"></a>**Azure használati jelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| SubscriptionId | Az előfizetés GUID-ja | 
| SubscriptionStartDate (Előfizetés kezdődátuma) | Az előfizetés kezdési dátuma | 
| SubscriptionEndDate (Előfizetési időszak) | Az előfizetés végének dátuma | 
| SubscriptionState (Előfizetési állam) | Az előfizetés aktuális állapota (Nyitott, Lezárt, Aktív vagy Türelmi időszakban) | 
| Month (hónap) | Hónap szerint összesített dátum | 
| ServiceName | Az Azure-szolgáltatás neve | 
| MeterCategory | A fogyasztásmérő-kategória neve | 
| UsageUnits (Használati egység) | A számlázási ciklusban használt egységek száma | 
| CustomerName | Az ügyfél neve | 
| CustomerTenantId | Az ügyfél bérlőazonosítója | 
| CustomerTpid (Ügyféltpid) | Ügyfél felső szülőazonosítója | 
| Ügyfélszegmentálás | Az ügyfél szegmense | 
| CustomerMarket (Ügyfél-piaci) | Az ügyfél földrajzi piaca | 
| MPNId | Microsoft Partner Network ügyfél azonosítója | 
| PartnerName | A partner neve | 
| PartnerHely | A partner földrajzi helye | 
| PartnerAttributionType | A partner forrásmegjelölési típusa | 
| SalesChannel (Értékesítések csatorna) | Az értékesítés csatornája (Közvetlen/CSP, Közvetett/CSP, Közvetlen és így tovább) | 
| ACR_USD | Az Azure által felhasznált bevétel (ACR) amerikai dollárban | 
| Regisztrációs azonosító | Az Azure-előfizetés regisztrációs azonosítója | 

### <a name="office-365-license-usage-report"></a>**Office 365 licenchasználati jelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| CustomerTenantId | Az ügyfél bérlőazonosítója | 
| CustomerTpid (Ügyféltpid) | Ügyfél felső szülőazonosítója | 
| WorkloadName (Számítási feladat neve) | Skype Vállalati verzió, Teams, Exchange Online | 
| Month (hónap) | A hónap, amelyre a használatot jelenteni kell | 
| PaidAvailableUnits | Fizetős elérhető egységek száma | 
| MonthlyActiveUsers | Havi aktív felhasználók száma | 
| CustomerName | Az ügyfél neve | 
| CustomerMarket (Ügyfél-piaci) | Az ügyfél piacának földrajzi helye | 
| Ügyfélszegmentálás | Ügyfélszegmens | 
| MPNId | A Microsoft Partner Network | 
| PartnerName | A partner neve | 
| PartnerHely | A partner földrajzi helye | 
| PartnerAttributionType | A partner forrásmegjelölési típusa | 

### <a name="enterprise-mobility-license-usage-report"></a>**Nagyvállalati mobilitási licenc használati jelentése**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| CustomerTenantId | Az ügyfél bérlőazonosítója | 
| CustomerTpid (Ügyféltpid) | Ügyfél felső szülőazonosítója | 
| WorkloadName (Számítási feladat neve) | A Enterprise Mobility + Security (EMS) számítási feladat neve | 
| Month (hónap) | A hónap, amelyre a használatot jelenteni kell | 
| PaidAvailableUnits | Fizetős elérhető egységek száma | 
| MonthlyActiveUsers | Havi aktív felhasználók száma | 
| CustomerName | Az ügyfél neve | 
| CustomerMarket | Az ügyfél piacának földrajzi helye | 
| CustomerSegment (Ügyfélszegment) | Ügyfélszegmens | 
| MPNId | A Microsoft Partner Network | 
| PartnerName | A partner neve | 
| PartnerHely | A partner földrajzi helye | 
| PartnerAttributionType | A partner forrásmegjelölési típusa | 

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365-licenchasználati jelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| SubscriptionId | Az előfizetés GUID-ja | 
| SubscriptionStartDate (Előfizetés kezdődátuma) | Az előfizetés kezdő dátuma | 
| SubscriptionEndDate (Előfizetési időszak) | Az előfizetés záró dátuma | 
| SubscriptionStatus (Előfizetésiállapot) | Az előfizetés állapota | 
| Month (hónap) | A használati adatok jelentésének hónapja | 
| RevSumDivisionName | A fordított összeg osztásának neve | 
| RevSumCategoryName | A rev sum kategória neve | 
| Termékváltozat | A termék termékváltozata | 
| SKUId (Termékváltozat-id) | A termék termékváltozat-azonosítója | 
| FreeVsPaidSKU | Azt jelzi, hogy ingyenes vagy fizetős termékváltozatról van-e szó | 
| SalesModel (Értékesítési modell) | Az előfizetés értékesítéséhez használt értékesítési csatorna | 
| DetailedSalesModel | Az előfizetés részletes értékesítési modellje | 
| CustomerName | Az ügyfél neve | 
| CustomerTenantId | Az ügyfélbérlő GUID-ja | 
| CustomerTpid (Ügyféltpid) | Ügyfél felső szülőazonosítója | 
| CustomerSegment (Ügyfélszegment) | Az ügyfél piaci szegmense | 
| CustomerMarket | Az ügyfél földrajzi piaca | 
| MPNId | A Microsoft Partner Network | 
| PartnerName | A partner neve | 
| PartnerHely | A partner földrajzi helye | 
| PartnerAttachType | Az előfizetés forrásmegjelölési típusa | 
| AvailableSeats (Rendelkezésre álló adatok) | Aktuálisan elérhető hely | 
| AssignedSeats (Hozzárendelések) | Aktuálisan hozzárendelt hely | 
| ActiveSeats (Aktív leselek) | Aktuális aktív helyek | 
| DeploymentOpportunity (Üzembe helyezésiopportunitás) | Aktuális üzembe helyezési lehetőség | 
| ActiveUsagePercent | Aktuális aktív használat százalékos aránya | 

### <a name="power-bi-license-usage-report"></a>**Power BI jelentés készítése**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| SubscriptionId | Az előfizetés GUID-ja | 
| SubscriptionStartDate (Előfizetés kezdődátuma) | Az előfizetés kezdő dátuma | 
| SubscriptionEndDate (Előfizetési időszak) | Az előfizetés záró dátuma | 
| SubscriptionStatus (Előfizetésiállapot) | Az előfizetés állapota (Aktív, Inaktív vagy Türelmi időszakban) | 
| Month (hónap) | Hónap szerint összesített dátum | 
| Termékváltozat | A termék termékváltozata | 
| SKUId (Termékváltozat-id) | A termék termékváltozat-azonosítója | 
| FreeVsPaidSKU | Ingyenes vagy fizetős termékváltozat-különbözik | 
| SalesModel (Értékesítési modell) | Az előfizetés értékesítéséhez használt értékesítési modell | 
| DetailedSalesModel | Az előfizetés részletes értékesítési modellje | 
| CustomerName | Az ügyfél neve | 
| CustomerTenantId | Az ügyfélbérlő GUID-ja | 
| CustomerTpid (Ügyféltpid) | Az ügyfél legfelső szülőazonosítója | 
| CustomerSegment (Ügyfélszegment) | Az ügyfél piaci szegmense | 
| CustomerMarket | Az ügyfél földrajzi piaca | 
| MPNId | A Microsoft Partner Network | 
| PartnerName | A partner neve | 
| PartnerHely | A partner földrajzi helye | 
| PartnerAttachType | Az előfizetés forrásmegjelölési típusa | 
| AvailableSeats (Rendelkezésre álló adatok) | Aktuálisan elérhető helyek | 
| AssignedSeats (Hozzárendelések) | Aktuálisan hozzárendelt helyek | 
| ActiveSeats (Aktív leselek) | Aktuális aktív helyek | 
| DeploymentOpportunity (Üzembe helyezésiopportunitás) | Aktuális üzembe helyezési lehetőség | 
| ActiveUsagePercent | Aktuális aktív használat százalékos aránya | 

### <a name="teams-meetings-and-calls-report"></a>**Teams-értekezletek és -hívások jelentése**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| CustomerTenantId | Az ügyfél bérlőazonosítója | 
| CustomerTpid (Ügyféltpid) | Az ügyfél legfelső szintű szülőazonosítója | 
| Month (hónap) | A használati adatok jelentésének hónapja | 
| Alhálózati terhelés | Alhálózati adatok, amelyekről a rendszer jelentést ad a használatról (értekezletek, hívások vagy telefonos rendszerek) | 
| Értekezletek száma | Értekezletek száma | 
| Értekezlet időtartama | Értekezletek teljes időtartama órákban | 

### <a name="teams-monthly-usage-report"></a>**Teams havi használati jelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| CustomerTenantId | Az ügyfél bérlőazonosítója | 
| CustomerTpid (Ügyféltpid) | Az ügyfél legfelső szülőazonosítója | 
| Month (hónap) | A hónap, amelyre a használatot jelenteni kell | 
| Alhálózat | Az almunkaterhelés, amelynek a használata jelentésre szolgál (értekezletek, hívások vagy telefonos rendszerek) | 
| Asztali felhasználók | A Teamset asztali környezetben használó felhasználók száma | 
| Mobilfelhasználók | A Teamset mobileszközökön használó felhasználók száma | 
| Webes felhasználók | A Weben Teamset használó felhasználók száma | 
| AllUpParticipants (AllUpParticipants) | A Teams egyedi felhasználóinak száma az adott hónapban | 

### <a name="teams-usage-3p-apps-report"></a>**Teams-használati 3P-alkalmazások jelentése**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| CustomerTenantId | Az ügyfél bérlőazonosítója | 
| CustomerTpid (Ügyféltpid) | Ügyfél felső szülőazonosítója | 
| Month (hónap) | A használati adatok jelentésének hónapja | 
| 3P-alkalmazás neve | A Teams-alkalmazás neve | 
| Felhasználók száma | Az alkalmazás felhasználóinak száma | 


### <a name="training-details-report"></a>**Betanítás részletei jelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| TrainingActivityId | A betanítás azonosítója | 
| TrainingTitle (Betanítás) | A képzés címe | 
| TrainingType (Betanítás típusa) | A képzés típusa (minősítés vagy vizsga) | 
| IndividualFirstName (Egyéni oszlopnév) | Az ügyfél vezetékneve | 
| IndividualLastName (EgyénilastName) | Az ügyfél vezetékneve | 
| E-mail | Az ügyfél személyes e-mail-azonosítója | 
| CorpEmail (Vállalati e-mail) | Az ügyfél Office-e-mail-azonosítója | 
| TrainingCompletionDate (Betanítás kiegészítésidátum) | A betanítás befejezési dátuma | 
| Month (hónap) | Az a hónap, amelyre az adatokat jelenteni kell | 
| IcMCP | Jelzi, hogy a felhasználó Microsoft Certified Professional (MCP) | 
| MCPID | A felhasználó MCP-azonosítója | 
| MPNId | A Microsoft Partner Network | 
| PartnerName | A partner neve | 
| PartnerCityLocation | A partner földrajzi helye | 
| PartnerCountryLocation | A partner földrajzi helye | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn jelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| Felhasználónév | A felhasználó neve | 
| UserId (Felhasználóazonosító) | A felhasználó GUID-ja | 
| TrainingName (Betanítás neve) | A betanítás neve | 
| TrainingType (Betanítás típusa) | A betanítás típusa (modul vagy képzési út) | 
| Termékek | Az a termék, amelyre a tanulási modul alkalmazható | 
| Szerepkörök | A képzés vonatkozó szerepkörei | 
| CompletionDate (Befejezésidátum) | A betanítás befejezésének dátuma | 
| MPNId | A Microsoft Partner Network | 
| PartnerName | A partner neve | 
| Ország | A partner földrajzi helye | 

### <a name="competency-summary-and-history-report"></a>**Kompetencia összegzése és előzményjelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| KompetenciaNév | A kompetencia neve | 
| Kompetenciaszint | A kompetencia szintje (arany vagy ezüst) | 
| KompetenciaÁllapot | A kompetencia aktuális állapota (Aktív, Inaktív vagy Türelmi időszakban) | 
| KompetenciaStartDate | A kompetencia kezdő dátuma | 
| KompetenciaEndDate | A kompetencia záró dátuma | 

### <a name="competency-performance-report"></a>**Kompetenciateljesítmény-jelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| KompetenciaNév | A kompetencia neve | 
| KompetenciaAttainmentOptionName | A kompetencia megszerzése lehetőség neve | 
| Month (hónap) | A metrikák jelentésének hónapja | 
| MetricName | A kompetencia szempontjából releváns metrika neve | 
| MetricMonthlyContribution (MetrikamonthlyContribution) | A metrika havi hozzájárulása | 
| TTMAggregate (TTMAggregate) | Összesített metrika a záró 12 hónapra | 
| ÉvfordulóÉvAggregate | Az aktuális évforduló évének összesített metrika | 
| GoldThreshold | Teljesítményre vonatkozó követelmények a Gold kompetencia követelményeinek való megfeleléshez | 
| SilverThreshold (SilverThreshold) | A Silver kompetencia teljesítménnyel kapcsolatos követelményei | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Felhőbeli Microsoft 365 jelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| MPN-azonosító | Microsoft Partner Network azonosítója | 
| Partner neve | A partner neve | 
| Ügyfél-azonosító | Az ügyfél azonosítószáma | 
| AMITS-szám | A & pontozás alatt&ügyfél Bradstreet (D&B) száma | 
| Fiók neve | A fiók neve | 
| Tartomány | A fiók tartománya | 
| Szervezet mérete | A szervezet mérete | 
| Iparág | Iparág, amelyhez a szervezet tartozik | 
| Függőleges | Annak az ügyfélnek a függőleges vonala, akit a Microsoft, a D&B és más iparági szabványok azonosítnak a nem megfelelőségért | 
| Terület | A hely földrajzi területe | 
| Leányvállalat | Annak az ügyfélnek a leányvállalata, akit a meg nem felelőség miatt pontozásra szereznek be | 
| Sales Territory | Annak az ügyfélnek az értékesítési területe, akit a nem megfelelőségért pontolnak | 
| City | A szervezet földrajzi helye | 
| Állapot | A szervezet földrajzi állapota | 
| Irányítószám | A szervezet irányítószáma | 
| Ország | A szervezet földrajzi helye | 
| Segment | Piaci szegmens | 
| Alszegmens | Piaci részszegmentálás | 
| SMC-típus összegzése | SMC típusa | 
| Top Unmanaged – Compute Base | Vezető nemmanaged ügyfelek – számítás | 
| Top Unmanaged - User Base | Vezető nemmanaged ügyfelek – felhasználó | 
| IsNonProfit | Jelzi, hogy a szervezet nonprofit-e (Igen vagy Nem) | 
| Távoli munka engedélyezése – Exchange Online-cél | Aktív Exchange Online-előfizetéssel és előfizetéssel Microsoft 365 | 
| Távoli munka engedélyezése – helyszíni beszerzés (aktuális verzió) a Cloud Ascent propensity funkcióval – +10 licenc | Olyan ügyfél, aki aktuális helyszíni Office- vagy Windows-ügyféllel rendelkezik. Ez azt jelenti, hogy az ügyfél verziója későbbi, mint az életciklus végén (EOL). Az ügyfél 10 vagy több licenccel rendelkezik. A támogatói pontszámmal rendelkezik. A partnernek a következőt kell célozni: átalakítás Microsoft 365. | 
| Távoli munka engedélyezése – helyszíni beszerzés (aktuális verzió) a Cloud Ascent propensity funkcióval – <10 licenc | Az aktuális helyszíni Office- vagy Windows-ügyféllel (vagyis az EOL-lal későbbi verzióval) rendelkezik. Az ügyfél kevesebb mint 10 licenccel rendelkezik. A propensitási pontszámmal rendelkezik. A partnernek a következőt kell célozni: átalakítás Microsoft 365. | 
| Távoli munka engedélyezése – helyszíni beszerzés (aktuális verzió) felhőalapú propensitás nélkül – +10 licenc | Az aktuális helyszíni Office- vagy Windows-ügyféllel (vagyis az EOL-lal későbbi verzióval) rendelkezik. Az ügyfél 10 vagy több licenccel rendelkezik. Az ügyfélnek nincs támogatói pontszáma. A partnernek a következőt kell célozni: átalakítás Microsoft 365. | 
| Távoli munka engedélyezése – helyszíni beszerzés (aktuális verzió) felhőalapú propensitás nélkül – <10 licenc | Az aktuális helyszíni Office- vagy Windows-ügyféllel (vagyis az EOL-lal későbbi verzióval) rendelkezik. Az ügyfél kevesebb mint 10 licenccel rendelkezik. Az ügyfélnek nincs támogatói pontszáma. A partnernek a következőt kell célozni: átalakítás Microsoft 365. | 
| Távoli munka engedélyezése – helyszíni beszerzés (EOL-verzió) felhőalapú propensitással – +10 licenc | Helyszíni EOL-ügyféllel vagy Windows-ügyféllel (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Az ügyfél 10 vagy több licenccel rendelkezik. Az ügyfélnek van egy propensitási pontszáma. A partnernek meg kell célozni a Microsoft 365. | 
| Távoli munka engedélyezése – helyszíni beszerzés (EOL-verzió) felhőalapú rugalmassággal – 10 licenc <engedélyezése | Helyszíni Office- vagy Windows-EOL-ügyféllel (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Az ügyfél kevesebb mint 10 licenccel rendelkezik. Az ügyfélnek van egy támogatói pontszáma. A partnernek meg kell célozni a Microsoft 365. | 
| Távoli munka engedélyezése – helyszíni beszerzés (EOL-verzió) felhőalapú ascent propensitás nélkül – +10 licenc | Aktuális helyszíni Office- vagy Windows-ügyféllel (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Az ügyfél 10 vagy több licenccel rendelkezik. Az ügyfélnek nincs propensitási pontszáma. A partnernek meg kell célozni a Microsoft 365. | 
| Távoli munka engedélyezése – helyszíni beszerzés (EOL-verzió) felhőbeli ascent propensitás nélkül – <10 licenc | Aktuális helyszíni Office- vagy Windows-ügyféllel (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Az ügyfél kevesebb mint 10 licenccel rendelkezik. Az ügyfélnek nincs propensitási pontszáma. A partnernek meg kell célozni a Microsoft 365. | 
| Távoli munka engedélyezése – magas propensitású potenciális Microsoft 365 (Act NowithEvaluate) | Potenciális ügyfél, aki nagy propenzitást támaszt a Microsoft 365 | 
| Távoli munka engedélyezése – versenyzés (nagyítás) Microsoft 365 | Zoom és Microsoft 365 ügyfelek, a Teamsre való átalakítás célja | 
| Távoli munka engedélyezése – versenyzés (nagyítás) Microsoft 365 | Ügyfél Nagyítással, cél a Teamsre konvertáláshoz | 
| Költségcsökkentés és kezelés – Microsoft 365 E3 E3 E5 Microsoft 365 megcélzva | E3-as Microsoft 365 meglévő ügyfél, az E5 Microsoft 365 cél | 
| Költségek csökkentése és kezelés – Microsoft 365 Business Basic és Standard szintű ügyfelek, Microsoft 365 Business Premiumot | Meglévő Microsoft 365 Business Basic- és Standard-ügyfelek, Microsoft 365 Business Premiumot céloznak meg | 
| Szervezeti hatékonyság átalakítása – Felületi propensitás | Az ügyfél a Surface-hez való támogatóságot mutat | 
| M365Cluster | Meghatározza, hogy az ügyfél nem hajlandó-e megvásárolni Microsoft 365. Target Act Now (Cél most) és Evaluate clusters (Fürtök kiértékelése, mert magasabb hozamot fognak eredményezni). A Célőrség és a Képzés ügyfeleket csak akkor kell megcélozni, ha az Act Now és az Evaluate customers (Ügyfelek értékelése) után még van kapacitás. | 
| M365Fit | Belső és külső adatpontok, amelyek a céges adatokat határozzák meg. A illeszkedés pontozása a legjobb kis- és középvállalatainkhoz hasonlító modellt használ az ügyfelek összehasonlítására, és annak összehasonlítása érdekében, hogy azok megfelelőek-e a Microsoft felhőalapú termékeihez. A illeszkedés pontozása negyedévente frissül. | 
| M365Intent | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A szándékpontozás átfedi a Fit (Igazítás) halmazt a fürtök meghatározásához. A szándékpontozás havonta frissül. | 
| SurfaceCluster | Azonosítja az ügyfél a Surface megvásárlásának szándékát az illeszkedési és szándékra vonatkozó javaslatok fürtbe való összevonásával. Target Act Now (Cél megcélzott törvény most) és Evaluate clusters (Fürtök kiértékelése, mert magasabb hozamot fognak eredményezni). A Célőrség és az Oktatás ügyfeleket csak akkor kell megcélozni, ha az Act Now és az Evaluate customers (Ügyfelek kiértékelése) után még van kapacitás. | 
| SurfaceFit | Belső és külső adatpontok, amelyek a céges adatokat határozzák meg. A illeszkedés pontozása a legjobb SBS-hez egy olyan modellt használ, amely összehasonlítja az ügyfeleket, és eldönti, hogy megfelelőek-e a Microsoft felhőalapú termékeihez. A illeszkedés pontozása negyedévente frissül. | 
| SurfaceIntent (SurfaceIntent) | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A szándékpontozás átfedi a Illeszkedés halmazt a fürtök meghatározásához. A szándékpontozás havonta frissül. | 
| O365Cluster | Az ügyfél Office 365-vásárlásra való hajlandóságát azonosítja. Target Act Now és Evaluate clusters because they'll produce higher yield. A Célőrség és az Oktatás ügyfeleket csak akkor kell megcélozni, ha az Act Now és az Evaluate customers (Ügyfelek kiértékelése) után még van kapacitás. | 
| O365Fit | Belső és külső adatpontok, amelyek a céges adatokat határozzák meg. A illeszkedés pontozása a legjobb SBS-hez egy olyan modellt használ, amely összehasonlítja az ügyfeleket, és eldönti, hogy megfelelőek-e a Microsoft felhőalapú termékeihez. A illeszkedés pontozása negyedévente frissül. | 
| O365Intent | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A szándékpontozás átfedi a Fit (Igazítás) halmazt a fürtök meghatározásához. A szándékpontozás havonta frissül. | 
| M365UpsellCustomer | Megállapítja, hogy az ügyfél megfelelőnek látszik-e a Microsoft 365 | 
| Rendelkezik a Google-lal | Megállapítja, hogy az ügyfél mutat-e versenyjelzéseket a Google-termékek tulajdonában | 
| Rendelkezik AWS-hez | Megállapítja, hogy az ügyfél versenyképes jeleket mutat-e a Amazon Web Services (AWS) termékeinek tulajdonában | 
| Nagyvállalati Szerződéssel rendelkezik | Megállapítja, hogy a megújítás nagyvállalati szerződés (EA) vagy EA-előfizetés | 
| Nyitott | Megállapítja, hogy a megújítás nyílt vagy nyílt értékű szerződés-e | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent – Dynamics 365 propensity report**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| MPN-azonosító | Microsoft Partner Network azonosítója | 
| Partner neve | A partner neve | 
| Ügyfél-azonosító | Ügyfélazonosító száma | 
| MÁS-MÁS SZÁM | A & Bradstreet azon ügyfél száma, akit a nem megfelelőségért pontolnak | 
| Fiók neve | A fiók neve | 
| Tartomány | A fiók tartománya | 
| Szervezet mérete | A szervezet mérete | 
| Iparág | Iparág, amelyhez a szervezet tartozik | 
| Függőleges | Annak az ügyfélnek a függőlegessége, akit a Microsoft, a D&B és más iparági szabványok azonosítnak
| Terület | A hely földrajzi területe | 
| Leányvállalat | Annak az ügyfélnek a leányvállalata, akit a propensitás miatt pontozással érnek el | 
| Sales Territory | Annak az ügyfélnek az értékesítési területe, akit a propensitási pontszámmal érnek el | 
| City | Földrajzi hely | 
| Állapot | Földrajzi állapot helye | 
| Irányítószám | A szervezet irányítószáma | 
| Ország | Földrajzi ország helye | 
| Segment | Piaci szegmens | 
| Alszegmens | Piaci részszegmentálás | 
| SMC-típus összegzése | Az ügyfelek kategorizálása: A legtöbb nemmanedizált felhasználói bázis a 300-nál is több alkalmazottal rendelkező ügyfelek, a legnagyobb nemmanedizált számítási bázisok azok az ügyfelek, akik 10 000 USD-t használhatnak az Azure-ban, a közepes üzletek 25 alkalmazottal vagy annál nagyobb ügyfelek, a kisvállalkozások pedig kevesebb mint 25 alkalmazottal rendelkező ügyfelek. | 
| Top Unmanaged – Compute Base | Felső szintű nem által nemott ügyfelek – számítás | 
| Top Unmanaged – User Base | Felső szintű nem regisztrált ügyfelek – felhasználók | 
| IsNonProfit | Jelzi, hogy a szervezet nonprofit-e (Igen vagy Nem) | 
| Digitális értékesítés aktiválása – Microsoft 365 – helyméret >= 25 hely (SalesPro propensity model) | Dynamics 365 nélküli ügyfél. Helyméret: 25+. A partnernek a Dynamics 365 SalesPro keresztértékesítését kell célozni. | 
| Digitális értékesítés aktiválása – Dynamics 365 SalesPro-propensitás (Act Now or Evaluate) | A Dynamics 365-öt nem támogató ügyfelek. A partnernek a Dynamics 365 SalesPro-t kell célozni. | 
| Pénzügyi kockázati & csalások kezelése – Dynamics helyszíni telepítési bázis – Navision (Business Central-beli támogató modell) | Meglévő ügyfél helyszíni Navisionvel. A partnernek a Dynamics 365 Business Centralt kell célozni. | 
| Pénzügyi kockázati & csalások kezelése – Dynamics helyszíni telepítési alap – Dynamics AX (Dynamics 365 Finance + Operations propensity model) | Meglévő ügyfél helyszíni AX-el. A partnernek a Dynamics 365 Finance + Operationst kell célozni. | 
| Pénzügyi kockázatkezelés & csalások esetén – Dynamics helyszíni telepítési bázis – Great Plains (Business Central-nak megfelelő modell) | Meglévő ügyfél helyszíni Great Plains-sel. A partnernek a Dynamics 365 Business Centralt kell célozni. | 
| Pénzügyi kockázati & csalások kezelése – Dynamics helyszíni telepítési bázis – Microsoft (Business Central propensity model) | Meglévő ügyfél helyszíniVel. A partnernek a Dynamics 365 Business Centralt kell célozni. | 
| Pénzügyi kockázat & csalások kezelése – Dynamics helyszíni telepítési bázis – Egyéb (Business Central-támogató modell) | Meglévő ügyfél más, korábban fel nem sorolt helyszíni megoldásokkal. A partnernek a Dynamics 365 Business Centralt kell célozni. | 
| Agilis üzleti folyamatok kiépítése – Dynamics helyszíni telepítési alap – AX/GP/SL/NAV/Other (Dynamics 365-támogató modell) | Agilis üzleti folyamatok kiépítése – Dynamics helyszíni telepítési alap – AX/GP/SL/NAV/Other (Dynamics 365-támogató modell) | 
| Agilis üzleti folyamatok összeállítása – Dynamics-versenybázis – Mendix/OutSystems/Salesforce (Dynamics 365 propensity model) | Agilis üzleti folyamatok kiépítése – Dynamics-versenybázis – Mendix/OutSystems/Salesforce (Dynamics 365 propensity model) | 
| Agilis üzleti folyamatok kiépítése – Dynamics 365 Finance + Operations telepítési alap | Meglévő Dynamics 365 Finance + Operations-ügyfelek. Partner a célcsoport Power Apps. | 
| Agilis üzleti folyamatok kiépítése – Dynamics 365 Business Central telepítési alap | Meglévő Dynamics 365 Business Central-ügyfelek. Partner a célcsoport Power Apps. | 
| Agilis üzleti folyamatok kiépítése – Dynamics 365 Customer Engagement telepítési alap | Meglévő Dynamics 365 Customer Engagement-ügyfelek. Partner a célcsoport Power Apps. | 
| Rugalmas ellátási lánc kiépítése – A Windows és az első Dynamics 365-beli számítási feladat aktiválása Dynamics 365 supply Chain Managementként nem Oracle- vagy SAP ERP-ügyfelekkel (nagyvállalati erőforrás-tervezés) | Megcélzott ügyfelek a Dynamics 365 ellátási láncának kezeléséhez | 
| Rugalmas ellátási lánc kiépítése – Dynamics 365 ellátásilánc-kezelés és/vagy kiskereskedelem és/vagy kereskedelem a meglévő Dynamics 365 Customer Engagement-ügyfelek számára | Meglévő Dynamics 365 Customer Engagement-ügyfelek, akik keresztértékesítési Dynamics 365 supply Chain Managementet céloznak meg. | 
| Rugalmas ellátási lánc kiépítése – a Dynamics 365 ellátásilánc-kezelési és/vagy kiskereskedelmi és/vagy kereskedelmi értékesítésének keresztajátszása a Dynamics 365 Customer Engagement és az Oracle vagy az SAP számára | Meglévő Dynamics 365 Customer Engagement-ügyfelek Oracle-hez vagy SAP-hez a Dynamics 365 ellátásilánc-kezeléshez | 
| D365BCCluster | Meghatározza, hogy az ügyfél nem hajlandó megvásárolni a Dynamics 365 Business Centralt. A Business Centralra támogató ügyfelek a Közepes és a Kis kategóriákba tartoznak. Target Act Now és Evaluate clusters, mert nagyobb hozamot fognak eredményezni. A Célőrség és a Képzés az ügyfelek számára csak akkor, ha az Act Now (Most megcélzott) és az Evaluate customers (Ügyfelek kiértékelése) cél megcélzott kapacitás még mindig rendelkezésre áll. | 
| D365BCFit | Belső és külső adatpontok, amelyek a céges adatokat határozzák meg. A illeszkedés pontozása a legjobb SMB-hez hasonlító modellt használ az ügyfelek összehasonlítására, és annak összehasonlítása érdekében, hogy azok megfelelőek-e a Microsoft felhőalapú termékeihez. A illeszkedés pontozása negyedévente frissül. | 
| D365BCIntent | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A szándékpontozás átfedi a Fit (Igazítás) halmazt a fürtök meghatározásához. A szándékpontozás havonta frissül. | 
| D365FOCluster | Azonosítja az ügyfél dynamics 365 Finance and Operations megvásárlására való hajlandóságát. Azok az ügyfelek, akik a Finance + Operationsre való támogatóságot mutatnak, a felső nem használt kategóriákba fognak sorolni. Target Act Now (Cél törvény most) és Evaluate clusters (Fürtök kiértékelése) – ezek nagyobb hozamot fognak eredményezni. A Célőrség és a Képzés az ügyfelek számára csak akkor, ha van még kapacitás az Act Now (Most megcélzott) és a Evaluate customers (Ügyfelek kiértékelése) megcélzott cél után. | 
| D365FOFit | Belső és külső adatpontok, amelyek a céges adatokat határozzák meg. A illeszkedés pontozása a legjobb SMB-modellünkhöz hasonlítva hasonlítja össze az ügyfeleket, és eldönti, hogy azok megfelelőek-e a Microsoft felhőalapú termékeihez. A illeszkedés pontozása negyedévente frissül. | 
| D365FOIntent | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A szándékpontozás átfedi a Illeszkedés halmazt a fürtök meghatározásához. A szándékpontozás havonta frissül. | 
| D365CECluster | Azonosítja az ügyfél Dynamics 365 Customer Engagement megvásárlására való hajlandóságát. A Customer Engagementre támogató ügyfelek a Közepes és a Kis kategóriákba tartoznak. Target Act Now (Cél törvény most) és Evaluate clusters (Fürtök kiértékelése) – ezek nagyobb hozamot fognak eredményezni. A Célőrség és a Képzés az ügyfelek számára csak akkor, ha van még kapacitás az Act Now (Most megcélzott) és a Evaluate customers (Ügyfelek kiértékelése) megcélzott cél után. | 
| D365CEFit | A Dynamics 365 Customer Engagementhez való illeszkedést jelzi | 
| D365CEIntent | A Dynamics 365 Customer Engagement szándékát jelzi | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Megállapítja, hogy az ügyfél rendelkezik-e nyílt megújítással a Dynamics helyszíni AX-hez vagy CRM-hez | 
| M365UpsellCustomer | Megállapítja, hogy az ügyfél megfelelőnek látszik-e a Microsoft 365 | 
| Rendelkezik a Google-lal | Megállapítja, hogy az ügyfél mutat-e versenyjelzéseket a Google-termékek tulajdonában | 
| Rendelkezik AWS-hez | Megállapítja, hogy az ügyfél mutat-e versenyjelzéseket az AWS-termékek tulajdonában | 
| Nagyvállalati Szerződéssel rendelkezik | Megállapítja, hogy a megújítás EA- vagy EA-előfizetés-e | 
| Nyitott | Megállapítja, hogy a megújítás nyílt vagy nyílt értékű szerződés-e | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent – Az Azure támogatási jelentése**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| MPN-azonosító | Microsoft Partner Network azonosítója | 
| Partner neve | A partner neve | 
| Ügyfél-azonosító | Ügyfélazonosító száma | 
| AMITS-szám | A & Bradstreet azon ügyfél száma, akit a nem megfelelőségért pontolnak | 
| Fiók neve | A fiók neve | 
| Tartomány | A fiók tartománya | 
| Szervezet mérete | A szervezet mérete | 
| Iparág | Iparág | 
| Függőleges | Annak az ügyfélnek a függőlegessége, akit a Microsoft, a D&B és más iparági szabványok azonosítnak | 
| Terület | A hely földrajzi területe | 
| Leányvállalat | Annak az ügyfélnek a leányvállalata, akit a propensitás miatt pontozással érnek el | 
| Sales Territory | Annak az ügyfélnek az értékesítési területe, akit a propensitási pontszámmal érnek el | 
| City | Földrajzi hely | 
| Állapot | Földrajzi állapot helye | 
| Irányítószám | A szervezet irányítószáma | 
| Ország | Földrajzi ország helye | 
| Segment | Piaci szegmens | 
| Alszegmens | Piaci részszegmentálás | 
| SMC-típus összegzése | SMC típusa | 
| Top Unmanaged – Compute Base | Vezető nemmanaged ügyfelek – számítás | 
| Top Unmanaged - User Base | Felső szintű nem regisztrált ügyfelek – felhasználók | 
| IsNonProfit | Jelzi, hogy a szervezet nonprofit-e (Igen vagy Nem) | 
| Áttelepítés – EOL Windows Server – EOL Windows Server IB felhőalapú rugalmassággal – 5+ licenc | Helyszíni Windows Server EOL-lal (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Az ügyfél 5 vagy több licenccel rendelkezik. A propensitási pontszámmal rendelkezik. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – EOL Windows Server – EOL Windows Server IB felhőalapú rugalmassággal – <5 licenc | Helyszíni Windows Server EOL-lal (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Az ügyfél kevesebb mint 5 licenccel rendelkezik. A propensitási pontszámmal rendelkezik. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – EOL Windows Server – EOL Windows Server IB felhőalapú rugalmasság nélkül – 5+ licenc | Helyszíni Windows Server EOL-lal (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Az ügyfél több mint 5 licenccel rendelkezik. Az ügyfélnek nincs támogatói pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – EOL Windows Server – EOL Windows Server IB felhőalapú rugalmasság nélkül – <5 licenc | Helyszíni Windows Server EOL-lal (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Kevesebb mint 5 licenccel rendelkezik. Az ügyfélnek nincs propensitási pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Migrate – EOL SQL – EOL SQL Server IB felhőalapú rugalmassággal – 5+ licenc | Helyszíni EOL-SQL Server (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Az ügyfél több mint 5 licenccel rendelkezik. Az ügyfélnek van egy támogatói pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Migrate – EOL SQL – EOL SQL Server IB felhőalapú rugalmassággal – 5 licenc <licenc | Helyszíni EOL-SQL Server (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Kevesebb mint 5 licenccel rendelkezik. A támogatói pontszámmal rendelkezik. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – EOL SQL – Az EOL SQL Server IB felhőbeli ascent propensitása nélkül – 5+ licenc | Helyszíni EOL-SQL Server (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Az ügyfél 5 vagy több licenccel rendelkezik. Az ügyfélnek nincs propensitási pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Miigrate – EOL SQL – EOL SQL Server IB felhőalapú ascent propensitása nélkül – <5 licenc | Helyszíni EOL-SQL Server (azaz EOL-verzióval vagy korábbi verzióval) rendelkezik. Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfélnek nincs támogatói pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – Helyszíni Windows Server áttelepítése – jelenlegi Windows Server IB felhőalapú rugalmassággal – 5+ licenc | Az aktuális helyszíni Windows Serverrel (azaz az EOL-lal későbbi verzióval) rendelkezik. Az ügyfél több mint 5 licenccel rendelkezik. Az ügyfélnek van egy propensitási pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – Helyszíni Windows Server áttelepítése – jelenlegi Windows Server IB felhőalapú rugalmassággal – <5 licenc | Az aktuális helyszíni Windows Serverrel (azaz az EOL-lal későbbi verzióval) rendelkezik. Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfélnek van egy Azure-támogatási pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – Helyszíni Windows Server áttelepítése – jelenlegi Windows Server IB felhőalapú propensitás nélkül – 5+ licenc | Az aktuális helyszíni Windows Serverrel (azaz az EOL-lal későbbi verzióval) rendelkezik. Az ügyfél több mint 5 licenccel rendelkezik. Az ügyfélnek nincs támogatói pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – Helyszíni Windows Server áttelepítése – jelenlegi Windows Server IB felhőalapú rugalmasság nélkül – <5 licenc | Az aktuális helyszíni Windows Serverrel (azaz az EOL-lal későbbi verzióval) rendelkezik. Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfélnek nincs propensitási pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – Áttelepítés Azure SQL vagy SQL virtuális gépekre (VM) – aktuális SQL Server IB felhőbeli ascent propensitással – 5+ licenc | Olyan ügyfél, aki aktuális helyszíni SQL Server (vagyis az EOL-on kívül újabb verzióval rendelkezik). Az ügyfél több mint 5 licenccel rendelkezik. Az ügyfélnek van egy támogatói pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Miigrate – Miigrate to Azure SQL or SQL VMs - current SQL Server IB with Cloud Ascent propensity – <5 licenses ( aktuális SQL Server IB with Cloud Ascent propensity – <5 licenc | Olyan ügyfél, aki aktuális helyszíni SQL Server (vagyis az EOL-on kívül újabb verzióval rendelkezik). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfélnek van egy támogatói pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – Áttelepítés Azure SQL vagy SQL virtuális gépekre – aktuális SQL Server IB felhőalapú propensitás nélkül – 5+ licenc | Olyan ügyfél, aki aktuális helyszíni SQL Server (vagyis az EOL-on kívül újabb verzióval rendelkezik). Az ügyfél több mint 5 licenccel rendelkezik. Az ügyfélnek nincs propensitási pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – Áttelepítés Azure SQL vagy SQL virtuális gépekre – jelenlegi SQL Server IB felhőalapú propensitás nélkül – <5 licenc | Olyan ügyfél, aki aktuális helyszíni SQL Server (vagyis az EOL-on kívül újabb verzióval rendelkezik). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfélnek nincs támogatói pontszáma. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – OSS – Áttelepítés nyílt forráskódú Verzióra (OSS) | Meglévő ügyfél a következő termékek bármelyikével: PostgreSQL, MySQL, MariaDB. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – OSS – Linux az Azure-ban | Meglévő ügyfél Linuxszal. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – SAP – Azure-beli SAP | Meglévő ügyfél az SAP-val. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – Windows Virtual Desktop – Távoli asztali szolgáltatások IB | Azonosítja az aktív Windows-Távoli asztali szolgáltatások. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Miigrate - Windows Virtual Desktop - Cross Sell Modern Work to Azure/WVD | Azonosítja a Microsoft 365, és nem az Azure-ral. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – VMware IB | Meglévő ügyfél a termékkel: VMware. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Áttelepítés – Citrix IB | Meglévő ügyfél a termékkel: Citrix Systems. A partnernek ezt az ügyfelet kell megcélzottnak lennie az Azure-ba való migráláshoz. | 
| Innováció – Elemzés – Power BI Azure-propensitású IB-hez | Az ügyfelek és az Active Power BI-előfizetéssel, beleértve a következőket: Power BI - Standalone Pro, Power BI - Azure Suites, Power BI - Office Suites, Power BI Suites - Microsoft 365 | 
| Engedélyezés – DevOps a GitHubbal – Visual Studio/MSDN IB | Az aktív ügyfélverzióval Visual Studio ügyfeleket azonosítja | 
| Windows Server Standard verzió | Megjeleníti az ügyfél által megvásárolt Windows Server Standard-vásárlások verzióját | 
| Windows Server Standard-licenc | Megjeleníti az ügyfél által megvásárolt Windows Server Standard-vásárlások licenctípusát | 
| Windows Server Data Center verziója | Megjeleníti az ügyfél által megvásárolt Windows Data Center-verziókat | 
| Windows Server Data Center-licenc | Megjeleníti az ügyfél által megvásárolt Windows Data Center-vásárlások licenctípusát | 
| AzureFit | Belső és külső adatpontok, amelyek a céges adatokat határozzák meg. A illeszkedés pontozása a legjobb SMB-modellünkhöz hasonlítva hasonlítja össze az ügyfeleket, és eldönti, hogy azok megfelelőek-e a Microsoft felhőalapú termékeihez. A illeszkedés pontozása negyedévente frissül. | 
| AzureIntent | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A szándékpontozás átfedi a Fit (Igazítás) halmazt a fürtök meghatározásához. A szándékpontozás havonta frissül. | 
| AzureCluster | Azonosítja az ügyfélnek az Azure megvásárlására való szándékát a illeszkedési és szándékra vonatkozó javaslatok egy fürtbe való összevonásával. Target Act Now és Evaluate clusters, mert nagyobb hozamot fognak eredményezni. A Célőrség és a Képzés az ügyfelek számára csak akkor, ha az Act Now (Most megcélzott) és az Evaluate customers (Ügyfelek kiértékelése) cél megcélzott kapacitás még mindig rendelkezésre áll. | 
| WindowsServerDataCenter_HasOpenRenewal | Megállapítja, hogy az ügyfél rendelkezik-e nyílt megújítással a Windows Server Datacenterhez | 
| WindowsServerStandard_HasOpenRenewal | Megállapítja, hogy az ügyfél rendelkezik-e nyílt megújítással a Windows Server Standardhez | 
| AzureUpsellCustomer | Megállapítja, hogy az ügyfél megfelelőnek látszik-e az Azure-ban | 
| Rendelkezik a Google-lal | Megállapítja, hogy az ügyfél mutat-e versenyjelzéseket a Google-termékek tulajdonában | 
| Rendelkezik AWS-hez | Megállapítja, hogy az ügyfél mutat-e versenyjelzéseket az AWS-termékek tulajdonában | 
| Nagyvállalati Szerződéssel rendelkezik | Megállapítja, hogy a megújítás EA- vagy EA-előfizetés-e | 
| Nyitott | Megállapítja, hogy a megújítás nyílt vagy nyílt értékű szerződés-e | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud Ascent – szerződés megújítására vonatkozó propensitási jelentés**

| Oszlop neve | Adatok leírása | 
| :--------- | :--------- | 
| MPN-azonosító | Microsoft Partner Network azonosítója | 
| Partner neve | A partner neve | 
| Ügyfél-azonosító | Ügyfélazonosító száma | 
| MÁS-MÁS SZÁM | A & Bradstreet azon ügyfél száma, akit a nem megfelelőségért pontolnak | 
| Fiók neve | A fiók neve | 
| Tartomány | A fiók tartománya | 
| Szervezet mérete | A szervezet mérete | 
| Iparág | Iparág | 
| Függőleges | Annak az ügyfélnek a függőlegessége, akit a Microsoft, a D&B és más iparági szabványok azonosítnak | 
| Terület | A hely földrajzi területe | 
| Leányvállalat | Annak az ügyfélnek a leányvállalata, akit a propensitás miatt pontozással érnek el | 
| Sales Territory | Annak az ügyfélnek az értékesítési területe, akit a propensitási pontszámmal érnek el | 
| City | Földrajzi város helye | 
| Állapot | Földrajzi állapot helye | 
| Irányítószám | A szervezet irányítószáma | 
| Ország | Földrajzi ország helye | 
| Segment | Piaci szegmens | 
| Alszegmens | Piaci részszegmentálás | 
| SMC-típus összegzése | SMC típusa | 
| Top Unmanaged – Compute Base | Felső szintű nem által nemott ügyfelek – számítás | 
| Top Unmanaged – User Base | Felső szintű nem regisztrált ügyfelek – felhasználók | 
| IsNonProfit | Jelzi, hogy a szervezet nonprofit-e (Igen vagy Nem) | 
| Rendelkezik a Google-lal | Megállapítja, hogy az ügyfél mutat-e versenyjelzéseket az AWS-termékek tulajdonában | 
| Rendelkezik AWS-hez | Megállapítja, hogy az ügyfél mutat-e versenyjelzéseket az AWS-termékek tulajdonában | 
| Azure-fürt | Meghatározza, hogy az ügyfél nem hajlandó megvásárolni az Azure-t. Target Act Now és Evaluate clusters, mert nagyobb hozamot fognak eredményezni. A Célőrség és a Képzés az ügyfelek számára csak akkor, ha az Act Now (Most megcélzott) és az Evaluate customers (Ügyfelek kiértékelése) cél megcélzott kapacitás még mindig rendelkezésre áll. | 
| D365 Finance + Operations Cluster | Azonosítja az ügyfél dynamics 365 Finance and Operations megvásárlására való hajlandóságát. Azok az ügyfelek, akik a Finance + Operationsre való támogatóságot mutatnak, a felső nem használt kategóriákba fognak sorolni. Target Act Now (Cél törvény most) és Evaluate clusters (Fürtök kiértékelése) – ezek nagyobb hozamot fognak eredményezni. A Célőrség és a Képzés az ügyfelek számára csak akkor, ha van még kapacitás az Act Now (Most megcélzott) és a Evaluate customers (Ügyfelek kiértékelése) megcélzott cél után. | 
| D365 CE-fürt | Azonosítja az ügyfél Dynamics 365 Customer Engagement megvásárlására való hajlandóságát. A Customer Engagementre támogató ügyfelek a Közepes és a Kis kategóriákba tartoznak. Target Act Now (Cél törvény most) és Evaluate clusters (Fürtök kiértékelése) – ezek nagyobb hozamot fognak eredményezni. A Célőrség és a Képzés az ügyfelek számára csak akkor, ha van még kapacitás az Act Now (Most megcélzott) és a Evaluate customers (Ügyfelek kiértékelése) megcélzott cél után. | 
| D365 BC-fürt | Azonosítja az ügyfél dynamics 365 Business Central megvásárlására való hajlandóságát. A Business Centralra támogató ügyfelek a Közepes és a Kis kategóriákba tartoznak. Target Act Now (Cél törvény most) és Evaluate clusters (Fürtök kiértékelése) – ezek nagyobb hozamot fognak eredményezni. A Célőrség és a Képzés az ügyfelek számára csak akkor, ha van még kapacitás az Act Now (Most megcélzott) és a Evaluate customers (Ügyfelek kiértékelése) megcélzott cél után. | 
| Microsoft 365 fürt | Azonosítja, hogy az ügyfél nem hajlandó megvásárolni a Microsoft 365. Target Act Now (Cél törvény most) és Evaluate clusters (Fürtök kiértékelése) – ezek nagyobb hozamot fognak eredményezni. A Célőrség és a Képzés az ügyfelek számára csak akkor, ha van még kapacitás az Act Now (Most megcélzott) és a Evaluate customers (Ügyfelek kiértékelése) megcélzott cél után. | 
| Licencprogram | A megújítás licencprogram-típusának azonosítására | 
| Szerződésazonosító | A szerződés azonosítója | 
| Szerződés záró dátuma | A szerződés záró dátuma | 
| Lejárat típusa | Lejárat típusa | 
| Lejáró bevétel | A lejáró előfizetésekkel kapcsolatos bevétel | 
| Nagyvállalati Szerződéssel rendelkezik | Megállapítja, hogy a megújítás EA- vagy EA-előfizetés-e | 
| Nyitott | Megállapítja, hogy a megújítás nyílt vagy nyílt értékű szerződés-e | 
| Azure Upsell-ügyfél | Megállapítja, hogy az ügyfél megfelelőnek látszik-e az Azure-ban | 
| Microsoft 365 Upsell-ügyfél | Megállapítja, hogy az ügyfél megfelelőnek látszik-e a Microsoft 365 | 
| RevSumDivisionName | A megújításra alkalmas terméket azonosítja | 

## <a name="next-steps"></a>Következő lépések

További információ: Jelentések [letöltése.](pci-download-reports.md)
