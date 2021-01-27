---
title: Az Insights adatdefiníciói
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A dokumentum felsorolja a különböző jelentéseket és azok adatdefinícióit, amelyeket az elemzések letöltéséről szóló jelentés oldaláról tölthet le.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 427ca3b60ec527a6a371a232538647448d03b084
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861393"
---
# <a name="export--data-definitions"></a>Exportálás – adatdefiníciók 

 **Megfelelő szerepkörök** 

- Jelentés megjelenítője 
- Executive Report Viewer 

## <a name="introduction"></a>Bevezetés 

Az adatforrások irányítópultján a jelentések letöltése központ használatával exportálhatja a nyers adatkészleteket. 

A különböző jelentések, amelyeket az adatdefiníciókkal együtt tölthet le, az alábbi táblázatokban láthatók: 

### <a name="partner-profile-report"></a>**Partneri profil jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| MPNId | Microsoft Partner Network (MPN) azonosítója | 
| PartnerName | A partner neve | 
| PGA_MPNId | A partner globális fiók MPN azonosítója | 
| PGA_PartnerName | Partner globális fiókjának neve | 
| City | A partner városának helye | 
| Country | A partner országának helye | 
| HierarchyLevel | Azt jelzi, hogy globális MPN-azonosító vagy Location MPN-azonosító | 

### <a name="customer-details-report"></a>**Ügyfél részletei jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| CustomerName | Az ügyfél neve | 
| CustomerTenantId | Az ügyfél bérlő azonosítója | 
| CustomerTpid | Az ügyfél elsődleges szülőjének azonosítója | 
| CustomerSegment | Felhasználói szegmens | 
| CustomerMarket | Az ügyfél földrajzi piaca | 
| CustomerStatus | Ügyfél állapota (aktív vagy inaktív) | 
| Termék | Az MPN által az ügyfélnek eladott termék: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI vagy Microsoft Azure | 
| Termékváltozat | Termék SKU | 
| Month (hónap) | A használat és a bevétel jelentésének hónapja | 
| MPNId | Microsoft Partner Network azonosítója | 
| PartnerName | A partner neve | 
| PartnerLocation | A partner földrajzi helye | 
| PartnerAttributionType | A partnerhez tartozó Attribution-típus | 
| SalesChannel | Értékesítési csatorna | 
| AvailableSeats | Rendelkezésre álló helyek | 
| RevenueUSD | Bevétel az USA dollárban | 

### <a name="reseller-performance-report"></a>**Viszonteladói teljesítmény jelentés**

> [!Note]
> A bevételi és ACR-adatforrások csak a vezetői jelentések megjelenítői számára érhetők el.

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| ResellerMPNid | Viszonteladói Microsoft Partner Network azonosítója | 
| ResellerName | Viszonteladó neve | 
| ResellerMarket | Viszonteladói ország piaca | 
| IndirectProviderMPNId | A közvetett szolgáltató azonosítója Microsoft Partner Network | 
| IndirectProviderName | Közvetett szolgáltató neve | 
| Month (hónap) | A használat és a bevétel jelentésének hónapja | 
| Termék | Terméknév | 
| SubscriptionID | Az előfizetés azonosítója | 
| AvailableSeats | Rendelkezésre álló helyek száma | 
| AssignedSeats | Hozzárendelt ülőhelyek száma | 
| BilledRevenueUSD | Számlázott bevétel az USA dollárban | 
| CustomerName | Az ügyfél neve | 
| CustomerTPid | Az ügyfél elsődleges szülőjének azonosítója | 
| CustomerSegment | Felhasználói szegmens | 
| CustomerMarket | Az ügyfél földrajzi piaca | 
| ResellerStatus | Viszonteladói állapot | 

### <a name="subscription-details-report"></a>**Előfizetés részletei jelentés**

>[!Note]
>A bevételi és ACR-adatforrások csak a vezetői jelentések megjelenítői számára érhetők el.

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| SubscriptionId | Az előfizetés GUID azonosítója | 
| SubscriptionStartDate | Az előfizetés kezdő dátuma | 
| SubscriptionEndDate | Az előfizetés befejező dátuma | 
| SubscriptionState | Az előfizetés állapota (aktív vagy átadott) | 
| Month (hónap) | A használat és a bevétel jelentésének hónapja | 
| IsAutoRenew | Azt jelzi, hogy az előfizetés megújítható-e (igen vagy nem) | 
| CustomerName | Az ügyfél neve | 
| CustomerTenantId | Az ügyfél GUID azonosítója | 
| CustomerTpid | Ügyfél elsődleges szülő-azonosítója | 
| CustomerSegment | Az ügyfél piaci szegmense | 
| CustomerMarket | Az ügyfél földrajzi piaca | 
| Termék | A partner által az ügyfélnek eladott termék | 
| Termékváltozat | A termék SKU-jának száma | 
| MPNId | A partner Microsoft Partner Network azonosítója | 
| PartnerName | A partner neve | 
| PartnerLocation | A partner földrajzi helye | 
| PartnerAttributionType | Az előfizetéshez tartozó Attribution-típus | 
| SalesChannel | A Sales-Direct, CSP (felhőalapú megoldás-szolgáltató) csatornája stb. | 
| AvailableSeats | Aktuálisan elérhető hely | 
| RevenueUSD | Bevétel az USA dollárban | 
| Regisztrációs azonosító | Az előfizetés regisztrációs azonosítója | 

### <a name="azure-usage-report"></a>**Azure-használati jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| SubscriptionId | Az előfizetés GUID azonosítója | 
| SubscriptionStartDate | Az előfizetés kezdetének dátuma | 
| SubscriptionEndDate | Az előfizetés végének dátuma | 
| SubscriptionState | Az előfizetés aktuális állapota (nyitott, lezárt, aktív vagy türelmi időszak) | 
| Month (hónap) | Dátum összesítése hónap alapján | 
| ServiceName | Az Azure-szolgáltatás neve | 
| MeterCategory | A fogyasztásmérő kategóriájának neve | 
| UsageUnits | A számlázási ciklusban használt egységek száma | 
| CustomerName | Az ügyfél neve | 
| CustomerTenantId | Az ügyfél bérlői azonosítója | 
| CustomerTpid | Ügyfél elsődleges szülő-azonosítója | 
| CustomerSegment | Az ügyfél szegmense | 
| CustomerMarket | Az ügyfél földrajzi piaca | 
| MPNId | Az ügyfél Microsoft Partner Network azonosítója | 
| PartnerName | A partner neve | 
| PartnerLocation | A partner földrajzi országának helye | 
| PartnerAttributionType | A partnerhez tartozó Attribution-típus | 
| SalesChannel | Értékesítési csatorna (Direct/CSP, indirekt/CSP, Direct stb.) | 
| ACR_USD | Az Azure által felhasznált bevétel (ACR) az USA dollárban | 
| Regisztrációs azonosító | Az Azure-előfizetés regisztrációs azonosítója | 

### <a name="office-365-license-usage-report"></a>**Office 365-licencek használati jelentése**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| CustomerTenantId | Az ügyfél bérlői azonosítója | 
| CustomerTpid | Ügyfél elsődleges szülő-azonosítója | 
| WorkloadName | Skype vállalati verzió, csapat, Exchange Online | 
| Month (hónap) | Az a hónap, amelynek a felhasználását jelenteni kell | 
| PaidAvailableUnits | Fizetős rendelkezésre álló egységek száma | 
| MonthlyActiveUsers | Havi aktív felhasználók száma | 
| CustomerName | Az ügyfél neve | 
| CustomerMarket | Az ügyfél piacának földrajzi országbeli helye | 
| CustomerSegment | Felhasználói szegmens | 
| MPNId | Microsoft Partner Network azonosítója | 
| PartnerName | A partner neve | 
| PartnerLocation | A partner földrajzi helye | 
| PartnerAttributionType | A partnerhez tartozó Attribution-típus | 

### <a name="enterprise-mobility-license-usage-report"></a>**Nagyvállalati mobilitási licenc használati jelentése**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| CustomerTenantId | Az ügyfél bérlői azonosítója | 
| CustomerTpid | Ügyfél elsődleges szülő-azonosítója | 
| WorkloadName | A Enterprise Mobility + Security-(EMS-) munkaterhelés neve | 
| Month (hónap) | Az a hónap, amelynek a felhasználását jelenteni kell | 
| PaidAvailableUnits | Fizetős rendelkezésre álló egységek száma | 
| MonthlyActiveUsers | Havi aktív felhasználók száma | 
| CustomerName | Az ügyfél neve | 
| CustomerMarket | Az ügyfél piacának földrajzi országbeli helye | 
| CustomerSegment | Felhasználói szegmens | 
| MPNId | Microsoft Partner Network azonosítója | 
| PartnerName | A partner neve | 
| PartnerLocation | A partner földrajzi helye | 
| PartnerAttributionType | A partnerhez tartozó Attribution-típus | 

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365-licencek használati jelentése**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| SubscriptionId | Az előfizetés GUID azonosítója | 
| SubscriptionStartDate | Az előfizetés kezdő dátuma | 
| SubscriptionEndDate | Az előfizetés befejező dátuma | 
| SubscriptionStatus | Az előfizetés állapota | 
| Month (hónap) | Az a hónap, amelynek a felhasználását jelenteni kell | 
| RevSumDivisionName | A Rev Sum divízió neve | 
| RevSumCategoryName | A Rev Sum kategória neve | 
| Termékváltozat | A termék SKU-jának száma | 
| SKUId | A termék SKU-azonosítója | 
| FreeVsPaidSKU | Azt jelzi, hogy ingyenes vagy fizetős SKU-e | 
| SalesModel | Az előfizetés értékesítéséhez használt értékesítési csatorna | 
| DetailedSalesModel | Az előfizetés részletes értékesítési modellje | 
| CustomerName | Az ügyfél neve | 
| CustomerTenantId | Az ügyfél bérlője GUID azonosítója | 
| CustomerTpid | Ügyfél elsődleges szülő-azonosítója | 
| CustomerSegment | Az ügyfél piaci szegmense | 
| CustomerMarket | Az ügyfél földrajzi piaca | 
| MPNId | Microsoft Partner Network azonosítója | 
| PartnerName | A partner neve | 
| PartnerLocation | A partner földrajzi országának helye | 
| PartnerAttachType | Az előfizetéshez tartozó Attribution-típus | 
| AvailableSeats | Aktuálisan elérhető hely | 
| AssignedSeats | Aktuálisan hozzárendelt ülőhely | 
| ActiveSeats | Aktuális aktív helyek | 
| DeploymentOpportunity | Aktuális üzembe helyezési lehetőség | 
| ActiveUsagePercent | Aktuális aktív használati arány | 

### <a name="power-bi-license-usage-report"></a>**Licenc-használati jelentés Power BI**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| SubscriptionId | Az előfizetés GUID azonosítója | 
| SubscriptionStartDate | Az előfizetés kezdő dátuma | 
| SubscriptionEndDate | Az előfizetés befejező dátuma | 
| SubscriptionStatus | Az előfizetés állapota (aktív, inaktív vagy türelmi időszak) | 
| Month (hónap) | Dátum összesítése hónap alapján | 
| Termékváltozat | A termék SKU-jának száma | 
| SKUId | A termék SKU-azonosítója | 
| FreeVsPaidSKU | Ingyenes vagy fizetős SKU differenciáló | 
| SalesModel | Az előfizetés értékesítéséhez használt értékesítési modell | 
| DetailedSalesModel | Az előfizetés részletes értékesítési modellje | 
| CustomerName | Az ügyfél neve | 
| CustomerTenantId | Az ügyfél bérlője GUID azonosítója | 
| CustomerTpid | Az ügyfél elsődleges szülőjének azonosítója | 
| CustomerSegment | Az ügyfél piaci szegmense | 
| CustomerMarket | Az ügyfél földrajzi piaca | 
| MPNId | Microsoft Partner Network azonosítója | 
| PartnerName | A partner neve | 
| PartnerLocation | A partner földrajzi országának helye | 
| PartnerAttachType | Az előfizetéshez tartozó Attribution-típus | 
| AvailableSeats | Aktuálisan elérhető helyek | 
| AssignedSeats | Aktuálisan hozzárendelt helyek | 
| ActiveSeats | Aktuális aktív helyek | 
| DeploymentOpportunity | Aktuális üzembe helyezési lehetőség | 
| ActiveUsagePercent | Aktuális aktív használati arány | 

### <a name="teams-meetings-and-calls-report"></a>**Csapatok ülései és hívási jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| CustomerTenantId | Az ügyfél bérlői azonosítója | 
| CustomerTpid | Az ügyfél elsődleges szülőjének azonosítója | 
| Month (hónap) | Az a hónap, amelynek a felhasználását jelenteni kell | 
| Almunkaterhelés | Azon alterhelések, amelyekről jelentés készül (értekezletek, hívások vagy telefonos rendszerek) | 
| Értekezletek száma | Értekezletek száma | 
| Értekezlet időtartama | Értekezletek teljes időtartama (óra) | 

### <a name="teams-monthly-usage-report"></a>**Csapatok havi használati jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| CustomerTenantId | Az ügyfél bérlői azonosítója | 
| CustomerTpid | Az ügyfél elsődleges szülőjének azonosítója | 
| Month (hónap) | Az a hónap, amelynek a felhasználását jelenteni kell | 
| Almunkaterhelés | Azon alterhelések, amelyekről jelentés készül (értekezletek, hívások vagy telefonos rendszerek) | 
| Asztali felhasználók | Az asztali csapatokat használó felhasználók száma | 
| Mobilfelhasználók | A mobil csapatokat használó felhasználók száma | 
| Webes felhasználók | A webes csapatokat használó felhasználók száma | 
| AllUpParticipants | A csapat egyedi felhasználóinak száma a hónapban | 

### <a name="teams-usage-3p-apps-report"></a>**Csapatok használata 3P-alkalmazások jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| CustomerTenantId | Az ügyfél bérlői azonosítója | 
| CustomerTpid | Ügyfél elsődleges szülő-azonosítója | 
| Month (hónap) | Az a hónap, amelynek a felhasználását jelenteni kell | 
| 3P-alkalmazás neve | A Teams alkalmazás neve | 
| Felhasználók száma | Az alkalmazáshoz tartozó felhasználók száma | 


### <a name="training-details-report"></a>**Képzés részletei jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| TrainingActivityId | A képzés azonosítója | 
| TrainingTitle | A képzés címe | 
| TrainingType | Képzés típusa (minősítés vagy vizsga) | 
| IndividualFirstName | Az ügyfél keresztneve | 
| IndividualLastName | Az ügyfél vezetékneve | 
| E-mail | Az ügyfél személyes e-mail-azonosítója | 
| CorpEmail | Az ügyfél Office e-mail azonosítója | 
| TrainingCompletionDate | A képzés befejezési dátuma | 
| Month (hónap) | Az adatgyűjtés hónapja | 
| IcMCP | Azt jelzi, hogy a felhasználó Microsoft Certified Professional (MCP) | 
| MCPID | A felhasználó MCP-azonosítója | 
| MPNId | Microsoft Partner Network azonosítója | 
| PartnerName | A partner neve | 
| PartnerCityLocation | A partner földrajzi városának helye | 
| PartnerCountryLocation | A partner földrajzi országának helye | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| Felhasználónév | A felhasználó neve | 
| UserId (Felhasználóazonosító) | A felhasználó GUID azonosítója | 
| TrainingName | A képzés neve | 
| TrainingType | Képzés típusa (modul vagy képzési útvonal) | 
| Termékek | Az a termék, amelyre a tanulási modul alkalmazható | 
| Szerepkörök | A képzés megfelelő szerepkörei | 
| CompletionDate | A képzés befejezésének dátuma | 
| MPNId | Microsoft Partner Network azonosítója | 
| PartnerName | A partner neve | 
| Country | A partner földrajzi országának helye | 

### <a name="competency-summary-and-history-report"></a>**Kompetencia összegzése és előzményei – jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| CompetencyName | A kompetencia neve | 
| CompetencyLevel | A kompetencia szintje (arany vagy ezüst) | 
| CompetencyStatus | A kompetencia aktuális állapota (aktív, inaktív vagy türelmi időszak) | 
| CompetencyStartDate | A kompetencia kezdő dátuma | 
| CompetencyEndDate | A kompetencia befejező dátuma | 

### <a name="competency-performance-report"></a>**Kompetencia-teljesítmény jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| CompetencyName | A kompetencia neve | 
| CompetencyAttainmentOptionName | A kompetencia-elérési lehetőség neve | 
| Month (hónap) | A metrikák jelentésének hónapja | 
| MetricName | A kompetenciához kapcsolódó metrika neve | 
| MetricMonthlyContribution | A metrika havi hozzájárulása | 
| TTMAggregate | A záró 12 hónapos időszak összesített mérőszáma | 
| AnniversaryYearAggregate | Az aktuális évfordulós év összesített mérőszáma | 
| GoldThreshold | A Gold kompetenciát kielégítő teljesítményre vonatkozó követelmény | 
| SilverThreshold | Az Silver kompetencia teljesítésének követelménye | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud bejutás – Microsoft 365-alapú adatszolgáltatási jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| MPN-azonosító | Microsoft Partner Network azonosítója | 
| Partner neve | A partner neve | 
| Ügyfél-azonosító | Az ügyfél azonosító száma | 
| DUNS-szám | A Dun & Bradstreettől (D&B) száma az ügyfél számára | 
| Fiók neve | A fiók neve | 
| Tartomány | A fiók tartománya | 
| Szervezeti méret | A szervezet mérete | 
| Iparág | Az iparág, amelyhez a szervezet tartozik | 
| Függőleges | A Microsoft, a D&B és más iparági szabványok alapján a szolgáltatáshoz kapcsolódóan felmerülő, a felmerülő ügyfél vertikális értéke | 
| Terület | A hely földrajzi területe | 
| Leányvállalat | Annak az ügyfélnek a leányvállalata, aki a kisegítő hajlandóságot szerzi be | 
| Sales Territory | Az ügyfél értékesítési területe, aki a kiértékeléshez | 
| City | A szervezet földrajzi városának helye | 
| Állam | A szervezet földrajzi állapotának helye | 
| Irányítószám | A szervezet postai irányítószáma | 
| Country | A szervezet földrajzi országának helye | 
| Segment | Piaci szegmens | 
| Alszegmens | Piaci alszegmens | 
| SMC-típus összegzése | SMC-típus | 
| Leggyakoribb nem felügyelt számítási alap | Leggyakoribb nem felügyelt ügyfelek – számítás | 
| Leggyakoribb nem felügyelt – felhasználói bázis | Leggyakoribb nem felügyelt ügyfelek – felhasználó | 
| IsNonProfit | Azt jelzi, hogy a szervezet nem profitorientált (igen vagy nem) | 
| Távoli munka engedélyezése – az Exchange Online megcélzása | Azok az ügyfelek, akik aktív Exchange Online-előfizetéssel rendelkeznek, upsell to Microsoft 365 | 
| Távoli helyszíni beszerzések engedélyezése (aktuális verzió) a Cloud bejutási hajlammal – + 10 licenc | Az a felhasználó, aki aktuális helyszíni irodával vagy Windows-ügyféllel rendelkezik. Ez az ügyfél verziója későbbi, mint az elhasználódott (EOL) verzió. Az ügyfél 10 vagy több licenccel rendelkezik. Az a felhasználó, aki a feldolgozói pontszámmal rendelkezik. A partnernek a Microsoft 365ra való átalakítás céljára kell irányulnia. | 
| Távoli helyszíni beszerzések engedélyezése (aktuális verzió) a Cloud bejutási hajlammal – <10 licenc | Az a felhasználó, aki az aktuális helyszíni Office-vagy Windows-ügyféllel rendelkezik (azaz a EOL-nál újabb verzió). Az ügyfél kevesebb mint 10 licenccel rendelkezik. Az a felhasználó, aki a feldolgozói pontszámmal rendelkezik. A partnernek a Microsoft 365ra való átalakítás céljára kell irányulnia. | 
| Távoli helyszíni beszerzések (aktuális verzió) engedélyezése felhőalapú átfedések nélkül – + 10 licenc | Az a felhasználó, aki az aktuális helyszíni Office-vagy Windows-ügyféllel rendelkezik (azaz a EOL-nál újabb verzió). Az ügyfél 10 vagy több licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek a Microsoft 365ra való átalakítás céljára kell irányulnia. | 
| Távoli helyszíni beszerzések (aktuális verzió) engedélyezése felhőalapú átfedések nélkül – <10 licenc | Az a felhasználó, aki az aktuális helyszíni Office-vagy Windows-ügyféllel rendelkezik (azaz a EOL-nál újabb verzió). Az ügyfél kevesebb mint 10 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek a Microsoft 365ra való átalakítás céljára kell irányulnia. | 
| Távoli helyszíni beszerzések (EOL-verzió) engedélyezése a Cloud megmászási szolgáltatással – + 10 licenc | A EOL helyszíni Office-vagy Windows-ügyféllel rendelkező ügyfél (azaz egy EOL vagy egy korábbi verzió). Az ügyfél 10 vagy több licenccel rendelkezik. Az ügyfélnek van egy megállási pontszáma. A partnernek a Microsoft 365ra való átalakítás céljára kell irányulnia. | 
| Távoli helyszíni beszerzések (EOL-verzió) engedélyezése a Cloud kapaszkodás szolgáltatással – <10 licenc | A EOL helyszíni Office-vagy Windows-ügyféllel rendelkező ügyfél (azaz egy EOL vagy egy korábbi verzió). Az ügyfél kevesebb mint 10 licenccel rendelkezik. Az ügyfélnek van egy megállási pontszáma. A partnernek a Microsoft 365ra való átalakítás céljára kell irányulnia. | 
| Távoli helyszíni beszerzések (EOL-verzió) engedélyezése felhőalapú átfedések nélkül – + 10 licenc | Az a felhasználó, aki aktuális helyszíni Office-vagy Windows-ügyféllel rendelkezik (azaz egy EOL vagy egy korábbi verzió). Az ügyfél 10 vagy több licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek a Microsoft 365ra való átalakítás céljára kell irányulnia. | 
| Távoli helyszíni beszerzések (EOL-verzió) engedélyezése felhőalapú átfedések nélkül – <10 licenc | Az a felhasználó, aki aktuális helyszíni Office-vagy Windows-ügyféllel rendelkezik (azaz egy EOL vagy egy korábbi verzió). Az ügyfél kevesebb mint 10 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek a Microsoft 365ra való átalakítás céljára kell irányulnia. | 
| Távoli munkavégzés – nagy kapacitású megoldás engedélyezése Microsoft 365 (NowithEvaluate) | A Microsoft 365 magas szintű kitartása a potenciális ügyfelek számára | 
| Távoli működés engedélyezése (nagyítás) Microsoft 365 | Az ügyfél zoom-és Microsoft 365okkal, a csapatokba való átalakítás céljával | 
| Távoli működés engedélyezése (nagyítás) Microsoft 365 nélkül | Ügyfél nagyítással, cél a csapatokba való átalakításhoz | 
| Csökkentse a költségeket és a felügyeletet – a Microsoft 365 E5-re irányuló Microsoft 365 E3 | Meglévő ügyfél Microsoft 365 E3-nál, Microsoft 365 E5 cél | 
| Csökkentse a költségeket és a felügyeletet – Microsoft 365 Vállalati verzió az alapszintű és az üzleti szabványoknak megfelelő, Microsoft 365 Vállalati verzió Premium szintű ügyfeleket | Meglévő Microsoft 365 Vállalati verzió alapszintű és üzleti standard szintű ügyfelek, a Microsoft 365 Vállalati verzió Premium célja | 
| A szervezeti termelékenység átalakítása – felszíni hajlam | Az ügyfél felszínre mutató hajlamot mutat | 
| M365Cluster | Azonosít egy ügyfelet a Microsoft 365 megvásárlásához. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot hoznak létre. Célozza meg, hogy az ügyfelek csak akkor legyenek ápolva és oktatva, ha továbbra is fennáll a kapacitás, és az ügyfelek kiértékelése megcélzott | 
| M365Fit | A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás egy kinézeti modellt használ a legjobb kis-és közepes méretű vállalkozásoknál (SMB) az ügyfelek összehasonlításához, és megtekintheti, hogy lehetséges-e a Microsoft Cloud Products. Az illesztési pontozás negyedévente frissül. | 
| M365Intent | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül. | 
| SurfaceCluster | Azonosít egy ügyfelet, hogy megvásárolja a felületet úgy, hogy összevonta a Fit és a szándékot a fürtbe. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot hoznak létre. Célozza meg, hogy az ügyfelek csak akkor legyenek ápolva és oktatva, ha továbbra is fennáll a kapacitás, és az ügyfelek kiértékelése megcélzott | 
| SurfaceFit | A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás egy kinézeti modellt használ a legjobb SMB-hez az ügyfelek összehasonlításához, és megtudhatja, hogy lehetséges-e a Microsoft Cloud Products. Az illesztési pontozás negyedévente frissül. | 
| SurfaceIntent | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül. | 
| O365Cluster | Azonosítja az ügyfélnek az Office 365 megvásárlására való hajlamát. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot hoznak létre. Célozza meg, hogy az ügyfelek csak akkor legyenek ápolva és oktatva, ha továbbra is fennáll a kapacitás, és az ügyfelek kiértékelése megcélzott | 
| O365Fit | A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás egy kinézeti modellt használ a legjobb SMB-hez az ügyfelek összehasonlításához, és megtudhatja, hogy lehetséges-e a Microsoft Cloud Products. Az illesztési pontozás negyedévente frissül. | 
| O365Intent | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül. | 
| M365UpsellCustomer | Meghatározza, hogy az ügyfél a Microsoft 365 upsell-hajlamot jeleníti-e meg | 
| A Google | Azt határozza meg, hogy az ügyfél versenyképes jeleket mutat-e a Google-termékek tulajdonosának | 
| AWS | Meghatározza, hogy az ügyfél versenyképes jeleket mutat-e a tulajdonosi Amazon Web Services (AWS) termékekhez | 
| EA | Azt határozza meg, hogy a megújítás nagyvállalati szerződés (EA) vagy EA-előfizetés | 
| Nyitva van | Meghatározza, hogy a megújítások nyitott vagy nyitott értékű szerződések-e | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud megmászás – Dynamics 365-alapú adatszolgáltatási jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| MPN-azonosító | Microsoft Partner Network azonosítója | 
| Partner neve | A partner neve | 
| Ügyfél-azonosító | Ügyfél-azonosító száma | 
| DUNS-szám | Az a Dun & Bradstreettől-szám, amelynek a kiértékelése megtörténik | 
| Fiók neve | A fiók neve | 
| Tartomány | A fiók tartománya | 
| Szervezeti méret | A szervezet mérete | 
| Iparág | Az iparág, amelyhez a szervezet tartozik | 
| Függőleges | A Microsoft, a D&B és más iparági szabványok alapján a szolgáltatáshoz kapcsolódóan felmerülő, a felmerülő ügyfél vertikális értéke
| Terület | A hely földrajzi területe | 
| Leányvállalat | Annak az ügyfélnek a leányvállalata, aki a kisegítő hajlandóságot szerzi be | 
| Sales Territory | Az ügyfél értékesítési területe, aki a kiértékeléshez | 
| City | Földrajzi város helye | 
| Állam | Földrajzi állapot helye | 
| Irányítószám | A szervezet postai irányítószáma | 
| Country | Földrajzi ország helye | 
| Segment | Piaci szegmens | 
| Alszegmens | Piaci alszegmens | 
| SMC-típus összegzése | Az ügyfél kategorizálása: az első nem felügyelt felhasználói bázisok a 300-nál több alkalmazottat foglalkoztató ügyfelek, a legfelső szintű nem felügyelt számítási alapértékek az Azure-ban hároméves USD10 rendelkező ügyfelek, a közepes méretű vállalkozások pedig 25 alkalmazottal vagy annál nagyobb számú ügyfelet használnak, és a kisvállalkozások kevesebb mint 25 alkalmazottat foglalkoztatnak. | 
| Leggyakoribb nem felügyelt számítási alap | Leggyakoribb nem felügyelt ügyfelek – számítás | 
| Leggyakoribb nem felügyelt – felhasználói bázis | Leggyakoribb nem felügyelt ügyfelek – felhasználók | 
| IsNonProfit | Azt jelzi, hogy a szervezet nem profitorientált (igen vagy nem) | 
| A digitális értékesítés – Microsoft 365 ülőhelyek méretének aktiválása >= 25 ülőhely (SalesPro-alapú modell) | A Dynamics 365 nélküli ügyfél. Ülőhely mérete: 25 +. A partnernek meg kell céloznia a Dynamics 365 SalesPro értékesítését. | 
| A digitális értékesítés aktiválása – Dynamics 365 SalesPro-hajlam (a jogszabály most vagy a kiértékelése) | Nagy mennyiségű, Dynamics 365 nélküli ügyfelek. A partnernek a Dynamics 365 SalesPro kell megcéloznia. | 
| A pénzügyi kockázat & a csalások kezelése – Dynamics helyszíni telepítési alap – Navision (Business Central-alapú adatkezelési modell) | Meglévő ügyfél helyszíni Navisionval. A partnernek a Dynamics 365 Business Central számára kell megcéloznia. | 
| A pénzügyi kockázat & a csalások kezelése – Dynamics helyszíni telepítési alap – Dynamics AX (Dynamics 365 Finance + Operations-felépítési modell) | Meglévő ügyfél helyszíni AX-vel. A partnernek meg kell céloznia a Dynamics 365 Finance + műveleteit. | 
| A pénzügyi kockázatok & a csalások kezelése – Dynamics helyszíni telepítési alap – nagyszerű síkságok (Business Central-alapú modellezési modell) | A meglévő ügyfél a helyszíni nagyszerű Síkságokkal rendelkezik. A partnernek a Dynamics 365 Business Central számára kell megcéloznia. | 
| A pénzügyi kockázat & csalás – a Dynamics helyszíni telepítési alap – Salamon (Business Central-alapú adatkezelési modell) | Meglévő ügyfél helyszíni Salamon-val. A partnernek a Dynamics 365 Business Central számára kell megcéloznia. | 
| A pénzügyi kockázatok & a csalások kezelése – Dynamics helyszíni telepítési alap – egyebek (Business Central-alapú adatkezelési modell) | A meglévő ügyfél más helyszíni megoldásokkal már nem szerepel. A partnernek a Dynamics 365 Business Central számára kell megcéloznia. | 
| Agilis üzleti folyamatok létrehozása – a Dynamics helyszíni telepítési alap-AX/GP/SL/NAV/other (Dynamics 365-alapú modell) | Agilis üzleti folyamatok létrehozása – a Dynamics helyszíni telepítési alap-AX/GP/SL/NAV/other (Dynamics 365-alapú modell) | 
| Agilis üzleti folyamatok létrehozása – Dynamics verseny alapja – Mendix/Salesforce/(Dynamics 365-alapú modell) | Agilis üzleti folyamatok létrehozása – Dynamics verseny alapja – Mendix/Salesforce/(Dynamics 365-alapú modell) | 
| Agilis üzleti folyamatok létrehozása – Dynamics 365 Finance + Operations Install Base | Meglévő Dynamics 365 Finance + Operations-ügyfelek. Partner a Power apps megcélzásához. | 
| Agilis üzleti folyamatok létrehozása – Dynamics 365 Business Central telepítési alap | Meglévő Dynamics 365 Business Central-ügyfelek. Partner a Power apps megcélzásához. | 
| Agilis üzleti folyamatok létrehozása – Dynamics 365 Customer engagement telepítési alapja | Meglévő Dynamics 365 Customer engagement-ügyfelek. Partner a Power apps megcélzásához. | 
| Rugalmas ellátási lánc létrehozása – Windows és az első Dynamics 365-alapú számítási feladat aktiválása Dynamics 365 ellátási láncként a nem Oracle vagy SAP ERP (vállalati erőforrás-tervezési) ügyfelekkel | Célzott ügyfelek a Dynamics 365 ellátási lánc kezeléséhez | 
| Rugalmas ellátási lánc létrehozása – a Dynamics 365 ellátási lánc kezelése és/vagy kiskereskedelmi vagy kereskedelmi forgalom a meglévő Dynamics 365 Customer engagement-ügyfelek számára | A meglévő Dynamics 365-ügyfelek a Dynamics 365-ellátási láncok értékesítését célozzák meg. | 
| Rugalmas ellátási lánc létrehozása – a Dynamics 365 ellátási lánc kezelése és/vagy kiskereskedelmi vagy kereskedelmi forgalom a Dynamics 365 Customer engagement és az Oracle vagy az SAP használatával | Meglévő Dynamics 365 Customer engagement-ügyfelek Oracle vagy SAP használatával a Dynamics 365 ellátási lánc felügyeletének megcélzásához | 
| D365BCCluster | Az ügyfél által a Dynamics 365 Business Central megvásárlására való hajlamot azonosítja. Azok az ügyfelek, akik a Business Central-t mutatják, közepes és kis kategóriába lesznek bevezetve. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot eredményez. Célozza meg, hogy az ügyfelek csak akkor ápolják és nevelik az ügyfelet, ha még mindig van kapacitásuk, és az ügyfelek kiértékelése után. | 
| D365BCFit | A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás egy kinézeti modellt használ a legjobb SMB-hez, hogy összehasonlítsa az ügyfeleket, és ellenőrizze, hogy lehetséges-e a Microsoft Cloud Products. Az illesztési pontozás negyedévente frissül. | 
| D365BCIntent | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül. | 
| D365FOCluster | Az ügyfél által a Dynamics 365-pénzügyi és-műveletek megvásárlására való hajlamot azonosítja. Azok az ügyfelek, akik a Finance + műveletekre való hajlamot mutatnak, a legfelső szintű nem felügyelt kategóriákban lesznek elérhetők. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot eredményez. Célozza meg, hogy az ügyfelek csak akkor ápolják és nevelik az ügyfelet, ha még mindig van kapacitásuk, és az ügyfelek kiértékelése után. | 
| D365FOFit | A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás egy kinézeti modellt használ a legjobb SMB-hez, hogy összehasonlítsa az ügyfeleket, és ellenőrizze, hogy lehetséges-e a Microsoft Cloud Products. Az illesztési pontozás negyedévente frissül. | 
| D365FOIntent | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül. | 
| D365CECluster | Azonosítja a Dynamics 365-ügyfelek bevonásának megvásárlására való hajlamot. Azok az ügyfelek, akik az ügyfelek részvételét mutatják, közepes és kis kategóriába lesznek bevezetve. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot eredményez. Célozza meg, hogy az ügyfelek csak akkor ápolják és nevelik az ügyfelet, ha még mindig van kapacitásuk, és az ügyfelek kiértékelése után. | 
| D365CEFit | A Dynamics 365-ügyfelek részvételéhez való illeszkedést jelzi | 
| D365CEIntent | A Dynamics 365-ügyfél részvételének szándékát jelzi | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Azt határozza meg, hogy az ügyfél rendelkezik-e nyílt megújítással a Dynamics helyszíni AX vagy a CRM számára | 
| M365UpsellCustomer | Meghatározza, hogy az ügyfél a Microsoft 365 upsell-hajlamot jeleníti-e meg | 
| A Google | Azt határozza meg, hogy az ügyfél versenyképes jeleket mutat-e a Google-termékek tulajdonosának | 
| AWS | Meghatározza, hogy az ügyfél versenyképes jeleket mutat-e az AWS-termékek tulajdonosának | 
| EA | Meghatározza, hogy a megújítási szolgáltatás EA vagy nagyvállalati előfizetés-e | 
| Nyitva van | Meghatározza, hogy a megújítások nyitott vagy nyitott értékű szerződések-e | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud bejutás – Azure-beli adatszolgáltatási jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| MPN-azonosító | Microsoft Partner Network azonosítója | 
| Partner neve | A partner neve | 
| Ügyfél-azonosító | Ügyfél-azonosító száma | 
| DUNS-szám | Az a Dun & Bradstreettől-szám, amelynek a kiértékelése megtörténik | 
| Fiók neve | A fiók neve | 
| Tartomány | A fiók tartománya | 
| Szervezeti méret | A szervezet mérete | 
| Iparág | Iparág | 
| Függőleges | A Microsoft, a D&B és más iparági szabványok alapján a szolgáltatáshoz kapcsolódóan felmerülő, a felmerülő ügyfél vertikális értéke | 
| Terület | A hely földrajzi területe | 
| Leányvállalat | Annak az ügyfélnek a leányvállalata, aki a kisegítő hajlandóságot szerzi be | 
| Sales Territory | Az ügyfél értékesítési területe, aki a kiértékeléshez | 
| City | Földrajzi város helye | 
| Állam | Földrajzi állapot helye | 
| Irányítószám | A szervezet postai irányítószáma | 
| Country | Földrajzi ország helye | 
| Segment | Piaci szegmens | 
| Alszegmens | Piaci alszegmens | 
| SMC-típus összegzése | SMC-típus | 
| Leggyakoribb nem felügyelt számítási alap | Leggyakoribb nem felügyelt ügyfelek – számítás | 
| Leggyakoribb nem felügyelt – felhasználói bázis | Leggyakoribb nem felügyelt ügyfelek – felhasználók | 
| IsNonProfit | Azt jelzi, hogy a szervezet nem profitorientált (igen vagy nem) | 
| Migrálás-EOL Windows Server-EOL Windows Server IB – felhőalapú átfedések – 5 + licenc | A helyszíni Windows Server EOL rendelkező ügyfél (azaz egy EOL vagy korábbi verzió). Az ügyfél 5 vagy több licenccel rendelkezik. Az a felhasználó, aki a feldolgozói pontszámmal rendelkezik. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás-EOL Windows Server-EOL Windows Server IB – felhőalapú átfedések – <5 licenc | A helyszíni Windows Server EOL rendelkező ügyfél (azaz egy EOL vagy korábbi verzió). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az a felhasználó, aki a feldolgozói pontszámmal rendelkezik. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás-EOL Windows Server-EOL Windows Server IB – felhőalapú átfedések nélkül – 5 + licenc | A helyszíni Windows Server EOL rendelkező ügyfél (azaz egy EOL vagy korábbi verzió). Az ügyfél több mint 5 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás-EOL Windows Server-EOL Windows Server IB – felhőalapú átfedések nélkül – <5 licenc | A helyszíni Windows Server EOL rendelkező ügyfél (azaz egy EOL vagy korábbi verzió). Kevesebb mint 5 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás-EOL SQL-EOL SQL Server IB a Cloud megmászással – 5 + licenc | Az a felhasználó, aki helyszíni EOL rendelkezik SQL Server (azaz egy EOL vagy egy korábbi verzió). Az ügyfél 5 licenctel rendelkezik. Az ügyfélnek van egy megállási pontszáma. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás-EOL SQL-EOL SQL Server IB a Cloud megmászással – <5 licenc | Az a felhasználó, aki helyszíni EOL rendelkezik SQL Server (azaz egy EOL vagy egy korábbi verzió). Kevesebb mint 5 licenccel rendelkezik. Az a felhasználó, aki a feldolgozói pontszámmal rendelkezik. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás-EOL SQL-EOL SQL Server IB Cloud felemelkedés nélkül – 5 + licenc | Az a felhasználó, aki helyszíni EOL rendelkezik SQL Server (azaz egy EOL vagy egy korábbi verzió). Az ügyfél 5 vagy több licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás-EOL SQL-EOL SQL Server IB felhőalapú átfedések nélkül – <5 licenc | Az a felhasználó, aki helyszíni EOL rendelkezik SQL Server (azaz egy EOL vagy egy korábbi verzió). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| A helyszíni Windows Server migrálása – a Windows Server IB jelenlegi és a felhőalapú átfedések – 5 + licenc | Az a felhasználó, aki az aktuális helyszíni Windows Server-kiszolgálóval rendelkezik (azaz a EOL-nál újabb verzió). Az ügyfél 5 licenctel rendelkezik. Az ügyfélnek van egy megállási pontszáma. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – helyszíni Windows Server-kiszolgáló migrálása – a Windows Server IB jelenlegi és felhőalapú átfedések – <5 licenc | Az a felhasználó, aki az aktuális helyszíni Windows Server-kiszolgálóval rendelkezik (azaz a EOL-nál újabb verzió). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfélnek van egy, az Azure-hoz való kiértékelési pontszáma. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – helyszíni Windows Server migrálása – a Windows Server IB jelenlegi verziójának Felhőbeli átfedések nélkül – 5 + licenc | Az a felhasználó, aki az aktuális helyszíni Windows Server-kiszolgálóval rendelkezik (azaz a EOL-nál újabb verzió). Az ügyfél 5 licenctel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – helyszíni Windows Server migrálása – a Windows Server IB jelenlegi verziójának Felhőbeli átfedések nélkül – <5 licenc | Az a felhasználó, aki az aktuális helyszíni Windows Server-kiszolgálóval rendelkezik (azaz a EOL-nál újabb verzió). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – áttelepítés Azure SQL-vagy SQL-alapú virtuális gépekre (VM-EK) – aktuális SQL Server IB a Cloud megmászási felemelkedéssel – 5 + licenc | Az a felhasználó, aki az aktuális helyszíni SQL Server (azaz a EOL-nál újabb verzió). Az ügyfél 5 licenctel rendelkezik. Az ügyfélnek van egy megállási pontszáma. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – áttelepítés Azure SQL-vagy SQL-alapú virtuális gépekre – jelenlegi SQL Server IB a Cloud megmászási felemelkedéssel – <5 licenc | Az a felhasználó, aki az aktuális helyszíni SQL Server (azaz a EOL-nál újabb verzió). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfélnek van egy megállási pontszáma. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – áttelepítés Azure SQL SQL Server-vagy SQL-alapú virtuális gépekre | Az a felhasználó, aki az aktuális helyszíni SQL Server (azaz a EOL-nál újabb verzió). Az ügyfél 5 licenctel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – áttelepítés Azure SQL-vagy SQL-alapú virtuális gépekre – jelenlegi SQL Server IB-re a Cloud felemelkedési hajlam nélkül – <5 licenc | Az a felhasználó, aki az aktuális helyszíni SQL Server (azaz a EOL-nál újabb verzió). Az ügyfél kevesebb mint 5 licenccel rendelkezik. Az ügyfél nem rendelkezik a rendelkezésre állási pontszámmal. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – OSS – áttelepítés nyílt forráskódú Shakespeare (OSS) ADATBÁZISba | Meglévő ügyfél a következő versengő termékek valamelyikével: PostgreSQL, MySQL, MariaDB. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás-OSS-Linux az Azure-on | Meglévő ügyfél Linuxon. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás-SAP-SAP az Azure-on | Meglévő ügyfél SAP-vel. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – Windows rendszerű virtuális asztali Távoli asztali szolgáltatások IB | Az aktív Windows Távoli asztali szolgáltatások ügyfeleket azonosítja. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – Windows rendszerű virtuális asztal – modern munka átadása az Azure-ba/WVD | Azonosíthatja az ügyfeleket Microsoft 365 és nem rendelkezik Azure-val. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – VMware IB | Meglévő ügyfél a termékkel: VMware. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Migrálás – Citrix IB | Meglévő ügyfél a termékkel: Citrix Systems. A partnernek meg kell céloznia ezt az ügyfelet az Azure-ba való áttelepítés során | 
| Innováció – elemzés – Power BI IB magas Azure-beli szolgáltatással | A és az aktív Power BI-előfizetéssel rendelkező ügyfelek, beleértve a következőket: Power BI-önálló Pro, Power BI-Azure Suite, Power BI-Office Suite, Power BI Suite-Microsoft 365 | 
| Enable-DevOps a GitHubon – Visual Studio/MSDN IB | Az aktív Visual Studio-verziókkal rendelkező ügyfelek azonosítása | 
| A Windows Server standard verziója | Megjeleníti az ügyfél által a Windows Server standard vásárlások verzióját. | 
| Windows Server Standard licenc | Megjeleníti az ügyfél által használt Windows Server standard szintű vásárlások licencének típusát | 
| Windows Server adatközpont verziója | Megjeleníti a Windows adatközpont-vásárlások ügyfelének verzióját. | 
| Windows Server adatközpont-licenc | Megjeleníti az ügyfél által a Windows adatközpont-vásárlások licencének típusát | 
| AzureFit | A firmographics definiáló belső és külső adatpontok. Az illeszkedő pontozás egy kinézeti modellt használ a legjobb SMB-hez, hogy összehasonlítsa az ügyfeleket, és ellenőrizze, hogy lehetséges-e a Microsoft Cloud Products. Az illesztési pontozás negyedévente frissül. | 
| AzureIntent | A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot. A leképezési pontozás a fürtök definiálására alkalmas. A szándékok pontozása havonta frissül. | 
| AzureCluster | Azonosítja az ügyfelet az Azure megvásárlásához, ha összevonta az illeszkedő és szándékozott javaslatokat egy fürtbe. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot eredményez. Célozza meg, hogy az ügyfelek csak akkor ápolják és nevelik az ügyfelet, ha még mindig van kapacitásuk, és az ügyfelek kiértékelése után. | 
| WindowsServerDataCenter_HasOpenRenewal | Azt határozza meg, hogy az ügyfél rendelkezik-e nyitott megújítással a Windows Server Datacenter rendszerhez | 
| WindowsServerStandard_HasOpenRenewal | Azt határozza meg, hogy az ügyfél rendelkezik-e nyitott megújítással a Windows Server Standard rendszerhez | 
| AzureUpsellCustomer | Meghatározza, hogy az ügyfél az Azure-beli upsell-hajlamot jeleníti-e meg | 
| A Google | Azt határozza meg, hogy az ügyfél versenyképes jeleket mutat-e a Google-termékek tulajdonosának | 
| AWS | Meghatározza, hogy az ügyfél versenyképes jeleket mutat-e az AWS-termékek tulajdonosának | 
| EA | Meghatározza, hogy a megújítási szolgáltatás EA vagy nagyvállalati előfizetés-e | 
| Nyitva van | Meghatározza, hogy a megújítások nyitott vagy nyitott értékű szerződések-e | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Felhőalapú átfedés – szerződés megújítása – jelentés**

| Oszlop neve | Az adatleírás | 
| :--------- | :--------- | 
| MPN-azonosító | Microsoft Partner Network azonosítója | 
| Partner neve | A partner neve | 
| Ügyfél-azonosító | Ügyfél-azonosító száma | 
| DUNS-szám | Az a Dun & Bradstreettől-szám, amelynek a kiértékelése megtörténik | 
| Fiók neve | A fiók neve | 
| Tartomány | A fiók tartománya | 
| Szervezeti méret | A szervezet mérete | 
| Iparág | Iparág | 
| Függőleges | A Microsoft, a D&B és más iparági szabványok alapján a szolgáltatáshoz kapcsolódóan felmerülő, a felmerülő ügyfél vertikális értéke | 
| Terület | A hely földrajzi területe | 
| Leányvállalat | Annak az ügyfélnek a leányvállalata, aki a kisegítő hajlandóságot szerzi be | 
| Sales Territory | Az ügyfél értékesítési területe, aki a kiértékeléshez | 
| City | Földrajzi város helye | 
| Állam | Földrajzi állapot helye | 
| Irányítószám | A szervezet postai irányítószáma | 
| Country | Földrajzi ország helye | 
| Segment | Piaci szegmens | 
| Alszegmens | Piaci alszegmens | 
| SMC-típus összegzése | SMC-típus | 
| Leggyakoribb nem felügyelt számítási alap | Leggyakoribb nem felügyelt ügyfelek – számítás | 
| Leggyakoribb nem felügyelt – felhasználói bázis | Leggyakoribb nem felügyelt ügyfelek – felhasználók | 
| IsNonProfit | Azt jelzi, hogy a szervezet nem profitorientált (igen vagy nem) | 
| A Google | Meghatározza, hogy az ügyfél versenyképes jeleket mutat-e az AWS-termékek tulajdonosának | 
| AWS | Meghatározza, hogy az ügyfél versenyképes jeleket mutat-e az AWS-termékek tulajdonosának | 
| Azure-fürt | Azonosítja az ügyfél által az Azure megvásárlására való hajlamot. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot eredményez. Célozza meg, hogy az ügyfelek csak akkor ápolják és nevelik az ügyfelet, ha még mindig van kapacitásuk, és az ügyfelek kiértékelése után. | 
| D365 Finance + Operations-fürt | Az ügyfél által a Dynamics 365-pénzügyi és-műveletek megvásárlására való hajlamot azonosítja. Azok az ügyfelek, akik a Finance + műveletekre való hajlamot mutatnak, a legfelső szintű nem felügyelt kategóriákban lesznek elérhetők. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot eredményez. Célozza meg, hogy az ügyfelek csak akkor ápolják és nevelik az ügyfelet, ha még mindig van kapacitásuk, és az ügyfelek kiértékelése után. | 
| D365 CE-fürt | Azonosítja a Dynamics 365-ügyfelek bevonásának megvásárlására való hajlamot. Azok az ügyfelek, akik az ügyfelek részvételét mutatják, közepes és kis kategóriába lesznek bevezetve. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot eredményez. Célozza meg, hogy az ügyfelek csak akkor ápolják és nevelik az ügyfelet, ha még mindig van kapacitásuk, és az ügyfelek kiértékelése után. | 
| D365 BC-fürt | Az ügyfél által a Dynamics 365 Business Central megvásárlására való hajlamot azonosítja. Azok az ügyfelek, akik a Business Central-t mutatják, közepes és kis kategóriába lesznek bevezetve. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot eredményez. Célozza meg, hogy az ügyfelek csak akkor ápolják és nevelik az ügyfelet, ha még mindig van kapacitásuk, és az ügyfelek kiértékelése után. | 
| Microsoft 365 fürt | Azonosítja Microsoft 365 vásárlásához szükséges ügyfelet. A TARGET most és kiértékeli a fürtöket, mert magasabb hozamot eredményez. Célozza meg, hogy az ügyfelek csak akkor ápolják és nevelik az ügyfelet, ha még mindig van kapacitásuk, és az ügyfelek kiértékelése után. | 
| Licencprogram | A megújításhoz tartozó Licencprogram típusát azonosítja. | 
| Szerződés azonosítója | A szerződés azonosítója | 
| Szerződés befejezési dátuma | A szerződés befejező dátuma | 
| Lejárat típusa | Lejárat típusa | 
| Lejáró bevétel | Lejáró előfizetésekhez kapcsolódó bevétel | 
| EA | Meghatározza, hogy a megújítási szolgáltatás EA vagy nagyvállalati előfizetés-e | 
| Nyitva van | Meghatározza, hogy a megújítások nyitott vagy nyitott értékű szerződések-e | 
| Azure upsell-ügyfél | Meghatározza, hogy az ügyfél az Azure-beli upsell-hajlamot jeleníti-e meg | 
| Microsoft 365 upsell-ügyfél | Meghatározza, hogy az ügyfél a Microsoft 365 upsell-hajlamot jeleníti-e meg | 
| RevSumDivisionName | Azonosítja a megújításra felkészülő terméket | 

## <a name="next-steps"></a>További lépések

További információ: [jelentések letöltése](pci-download-reports.md).
