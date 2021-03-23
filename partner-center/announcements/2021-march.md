---
title: Március 2021 közlemények
description: Március 2021 közlemények a Microsoft partner Centerben, beleértve az új képességeket, promóciókat, ajánlatokat, piacokat vagy a meglévő ajánlatok változásait.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 03/22/2021
ms.openlocfilehash: a3172b78d41a966b52a824703a7f15f163467d63
ms.sourcegitcommit: 715368e56fe669d29c7981906e08bc8d7d5d62a4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/23/2021
ms.locfileid: "104880735"
---
# <a name="march-2021-announcements"></a>Március 2021 közlemények

Ez az oldal a Microsoft partner Center 2021. márciusi hirdetményeit tartalmazza.

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Helyesbítések a 2021-es végleges szoftverek árlista

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-23
- Ajánlatok/piacok

### <a name="impacted-audience"></a>Érintett közönség

A közvetett szolgáltatók és a közvetlen számlázási partnerek örökös szoftvereket mutatnak a felhőalapú megoldás-szolgáltató programban 

### <a name="details"></a>Részletek

A 2021. március 1-én közzétett, Perpetual szoftverekhez tartozó árlista olyan piacokat foglal magában, amelyek nem voltak ott. A végleges szoftverhasználat-árlista 2021. március 17-én frissült a megfelelő értékekkel. Ezek a javítások csak a következőre voltak érvényesek:

- Termék azonosítója: DF77X4D43RKT 
- Terméknév: Windows 10 Home to Pro verziófrissítés Microsoft 365 Vállalati verzió
- Eltávolított vagy nem támogatott piacok: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, az LB, az LK, a MU, a NA, a NG , NI, NP, OM, PA, PE, PH, PK, PR, UY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG,, UZ, VE, VN, YE, ZM, ZW

Ezek a módosítások csak a fenti termékre vonatkoznak. Más termékek nem voltak kijavítani. 

### <a name="next-steps-and-resources"></a>Következő lépések és erőforrások

- Az örökös szoftvereket futtató partnereknek le kell tölteniük a legfrissebb végleges szoftverek árlista listáját.
- A [régióbeli országkód](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) alapján a két betűs rövidítések országokra való rövid hozzárendelését lehet megkeresni.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> SDK-kiadás a .NET standardban (v 1.17.0)

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-23

- Képességek
 
### <a name="impacted-audience"></a>Érintett közönség

A partner Center .NET SDK-t használó CSP programban részt vevő közvetlen számlázási partnerek és közvetett szolgáltatók.

### <a name="details"></a>Részletek

Március 23 2020-én a partnerek megkezdhetik a [MicrosoftPartnerCenter. NETSDK (NuGet Gallery) verziójának letöltését. Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), valamint a frissített Public partner Center SDK [GitHub-mintákat](https://github.com/Microsoft/Partner-Center-DotNet-Samples). Ez a verzió a következő módszerek frissítéseit tartalmazza:

#### <a name="audit-updated-new-operation-types"></a>Naplózás frissítve: új műveleti típusok

Új [műveleti típusok](https://docs.microsoft.com/partner-center/develop/auditing-resources) lettek hozzáadva, amelyekből megtudhatja, mikor hagyta jóvá és szakítja meg a DAP szolgáltatást.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Napló frissítve: új erőforrás-és műveleti típusok

Új [erőforrás-és műveleti típusok](https://docs.microsoft.com/partner-center/develop/auditing-resources) lettek hozzáadva az ügyfél-címtár szerepkör-forgatókönyv támogatásához.

- Új erőforrástípus: "CustomerDirectoryRole"

- A "AddUserMember" és a "RemoveUserMember" típusú műveletek

#### <a name="sdk-updates-to-customer-accounts"></a>Ügyfél-fiókok SDK-frissítései

- Támogatás a/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus beolvasásához

- /Customers/{Customer-Tenant-ID}/Qualifications beolvasása

- POST/Customers/{customer_id}/Qualifications? Code = {validationCode}

#### <a name="additional-changes"></a>További módosítások

A következő változások az új kereskedelmi szolgáltatás részeként jelennek meg, és a meghívással jelenleg csak olyan partnereink számára érhetők el, akik a M365/D365 új kereskedelmi élményhez tartoznak. Azok a partnerek, akik nem részei az új kereskedelmi technikai előzetes verziónak, nem észlelik a hatásokat, és visszamenőlegesen kompatibilisnek kell lenniük.

- Katalógus változásai:

  - /Products/{Product-ID}/SKUs/{SKU-ID} beolvasása

- Vásárlás és kezelés:
  - /Customers/{customerId}/subscriptions beolvasása
  - /Customers/{customerId}/subscriptions/{subscriptionId} beolvasása
  - /Customers/{customerId}/subscriptions/{subscriptionId} javítása
  - /Customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities beolvasása
  - /Customers/{customerId}/subscriptions/{subscriptionId}/transitions beolvasása
  - /Customers/{customerId}/subscriptions/{subscriptionId}/transitions közzététele

### <a name="next-steps"></a>Következő lépések

- Töltse le a legújabb verziót: [MicrosoftPartnerCenter. NETSDK (NuGet Gallery | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- A [GitHub-minták](https://github.com/Microsoft/Partner-Center-DotNet-Samples) letöltése és áttekintése

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>CSP kereskedelmi Marketplace ajánlat és FY21 CSP-ösztönzők a jogosult ajánlatok számára

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-18
- Képességek

### <a name="impacted-audience"></a>Érintett közönség

Közvetett szolgáltatók és közvetlen számlázási partnerek a Cloud Solution Provider programban 

### <a name="details"></a>Részletek

A közvetett szolgáltatók és a közvetlen számlázási partnerek a felhőalapú megoldás-szolgáltatói programban harmadik féltől származó ajánlatokat is értékesíthetik, és kedvezményeket szerezhetnek a partner Centerben vagy a Azure Portalban lebonyolított, jogosult harmadik féltől származó ajánlatokra vonatkozóan. Az ösztönzés a jogosult ajánlatok esetében a számlázott értékesítések esetében engedmény formájában történik, és **2021. június 30-ig érhető el**.  

Folytassa a jelen CSP kereskedelmi Marketplace ajánlatának megismerését, és lépjen kapcsolatba az ügyfelekkel a megfelelő ajánlatok azonosításához, hogy azok továbbra is sikeresek és digitális átalakítást nyújtsanak.

Független szoftvergyártók (ISV-ket) partnereink, hogy a legújabb IaaS és SaaS-megoldásokat a Microsoft ügyfelei számára is piacra hozzák. Az ISV-közzétevők lehetővé teszik, hogy a Microsoft partneri csatornán keresztül engedélyezzék az ajánlatok értékesítését. Az ösztönzőre jogosult ajánlatok két kategóriába sorolhatók:

- Válassza ki a SaaS-és IaaS külső ajánlatokat az Azure IP-címek közös értékesítésének incentivized állapotával. 

- Csapatokkal vagy legalább két Microsoft 365 hatékonyságnövelő alkalmazásokkal integrált SaaS-alkalmazások, mint például a PowerPoint, a Word, az Excel, az Outlook vagy a SharePoint.

### <a name="next-steps-and-resources"></a>Következő lépések és erőforrások

- Ismerje meg, hogyan szerezhet [partneri ösztönzőket](https://partner.microsoft.com/membership/partner-incentives) a jogosult Marketplace-alkalmazások értékesítésére az ösztönző jogosult alkalmazások számára. Az új ajánlatok havonta lesznek hozzáadva.  
- [Felhőalapú megoldás-szolgáltató közvetlen számlázási partneri ösztönző erőforrásai](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Felhőalapú megoldás szolgáltatójának közvetett szolgáltatói ösztönző erőforrásai](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Tekintse át ezt a [bemutatót](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) , ha többet szeretne megtudni a kereskedelmi piactéren elérhető alkalmazások értékesítéséről. További forrásokat [itt találhat](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/). 
- Fedezze fel a kereskedelmi piactér katalógusát a [partner Centerben](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) vagy [Azure Portal](https://ms.portal.azure.com/#home)
- [API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) -k használata az alkalmazások vállalati piactéren való integrálásához
- Tegye elérhetővé az olyan ISV-ket, akik érdeklődnek a
- A közvetett szolgáltatóknak integrálnia kell az API-k és az útmutató viszonteladók használatával

### <a name="questions"></a>Kérdése van?  

Tekintse át [ezt a cikket](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) a partner Center kereskedelmi piactérének áttekintéséhez.

Ha további segítségre van szüksége, létrehozhat egy támogatási kérést a partner Centerben. További információ: [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium ajánlat elnevezési és előfeltétel-frissítése

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-18
- Képességek

### <a name="summary"></a>Összefoglalás

Az 2021-as április 1-től a végső árlista frissül, hogy egyértelművé tegye a felhasználók által kínált Power BI Premium elnevezési és/vagy előfeltétel-információit.

### <a name="impacted-audience"></a>Érintett közönség

Cloud Solution Provider (CSP) közvetlen és közvetett partnerek

### <a name="details"></a>Részletek

Az 2021-as április 1-től a végső árlista frissül, hogy egyértelművé tegye a felhasználók által kínált Power BI Premium elnevezési és/vagy előfeltétel-információit.

A végleges árlista frissítése előtt használja az ebben a szakaszban található információkat a megfelelő termék megrendelésének biztosításához.

Az alábbi részletek az érintett SKU-t és az előfeltételek részleteit mutatják be.

| Ajánlat megjelenítendő neve március 1-től árlista |  Frissített ajánlat megjelenítendő neve április 1-től végleges árlista| Ajánlat azonosítója |
| ------ | ----------- | ----------- |
| Felhasználónkénti Add-On Power BI Premium (nonprofit alkalmazottak díjszabása)  |  Power BI Premium felhasználónkénti Add-On **(Office)** (nonprofit alkalmazottak díjszabása)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Az ajánlat megvásárlásához az ügyfélnek az alábbi előfeltételek valamelyikét kell megadnia:

| Ajánlat megjelenítendő neve | Ajánlat azonosítója |
| ------ | ----------- |
| Microsoft 365 E5 (nonprofit alkalmazottak díjszabása)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 hangkonferencia nélkül (nonprofit munkatársak díjszabása)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (nonprofit alkalmazottak díjszabása)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Office 365 E5 (nonprofit alkalmazottak díjszabása) próbaverzió|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 hangkonferencia nélkül (nonprofit munkatársak díjszabása)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

Az alábbi Power BI Premium ajánlat előfeltétele a vásárláshoz szükséges:

| Ajánlat megjelenítendő neve | Ajánlat azonosítója |
| ------ | ----------- |
|   Felhasználónkénti Add-On Power BI Premium (nonprofit alkalmazottak díjszabása)|  ef0b895b-681B-4026-a5b1-dda182a57d40 |

Az ajánlat megvásárlásához az ügyfeleknek meg kell követelniük az alábbi előfeltételeket:

| Ajánlat megjelenítendő neve | Ajánlat azonosítója |
| ------ |----------|
| Power BI Pro (nonprofit alkalmazottak díjszabása)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Következő lépések

Tekintse át a témakör erőforrásait, és ossza meg ezeket az információkat a szervezete megfelelő szereplőivel.  

### <a name="questions"></a>Kérdése van?

Az ajánlatokkal kapcsolatos bármilyen kérdés esetén keresse meg a megfelelő Yammer-közösségeket. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> A Microsoft 365 F3 díjszabási frissítései

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-16
- Ajánlatok/piacok

### <a name="summary"></a>Összefoglalás

Helytelen a március 2021 díjszabása kijavítva a Microsoft 365 F3 angol font (GBP) és az euro (EUR) esetében.

### <a name="impacted-audience"></a>Érintett közönség

A partnerek a Cloud Solution Provider (CSP) program keretében a 2021. március 1. és március 17. között megvásárolt Microsoft 365 F3-at.

### <a name="details"></a>Részletek

A Microsoft a Microsoft 365 F3 helytelen díjszabását oldotta meg. A helytelen árak a GBP és az EUR, és csak a 2021. március 1. és március 17. között megvásárolt ajánlatokra érvényesek. Az érintett ajánlatok és pénznemek az alábbiakban láthatók. 

| Ajánlat neve | Pénznem | Ajánlat azonosítója | Anyag azonosítója |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (jótékonysági) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | HRE-11626 |
| Microsoft 365 F3 (kereskedelmi) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
A márciusi és áprilisi előzetes verzióra vonatkozó alapszintű árlista a csendes-óceáni téli idő szerint 15. március 16-án frissült.

### <a name="next-steps"></a>Következő lépések

- Ha szükséges, a partnereknek újra le kell tölteniük az aktuális licenccel-alapú árlistát, valamint a márciusi és az áprilisi előzetes verziót is.  
- A Microsoft e-mailben kapcsolatba lép a kapcsolódó partnerekkel az elkövetkező hetekben, hogy tájékoztassa őket az érintett tranzakciók kijavítására vonatkozó következő lépésekről.

### <a name="questions"></a>Kérdése van?

További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeit.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Jogi cég nevének frissítése a partner centeren keresztül

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-16
- A meghajtó hatékonyságának & skálázása

### <a name="summary"></a>Összefoglalás

Március 2021, Microsoft Partner Network (MPN) partnerek és a felhőalapú megoldás-szolgáltató (CSP) közvetett viszonteladók a partner centeren keresztül frissíthetik a vállalatuk nevét.

### <a name="impacted-audience"></a>Érintett közönség

MPN-partnerek és CSP közvetett viszonteladók (nem alkalmazható a CSP Direct Bill-partnereknek)

### <a name="details"></a>Részletek

A március 2021-től kezdődően az MPN-partnerek és a CSP közvetett viszonteladók megfelelő, önkiszolgáló módon frissíthetik a vállalatuk nevét a partner centeren keresztül. Ezzel az új funkcióval a partnereknek többé nem kell beküldeniük a partner Center támogatási jegyét a vállalat nevének frissítéséhez. Így jelentős mennyiségű időt takaríthat meg a partnerek számára ezen tevékenységek végrehajtásakor. 

További információ: [a jogi üzleti profil frissítése](../update-your-partner-profile.md#update-your-legal-business-profile).

>[!NOTE]
>Győződjön meg arról, hogy a vállalat neve a jogi üzleti profilban nem tartalmaz helyesírási hibákat és rövidítéseket, és pontosan megfelel a vállalati üzleti regisztrációs rekordoknak. A szervezeti profil frissítésével kapcsolatos további információkért tekintse meg a [szervezet profiljának ellenőrzése](../update-your-partner-profile.md#update-your-legal-business-profile)című témakört.

### <a name="next-steps"></a>Következő lépések

Ossza meg ezt az információt a szervezeten belül, hogy a megfelelő csapat áttekintse és frissítse a folyamatait.

### <a name="questions"></a>Kérdése van?

További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeit.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Frissítés a Cloud Solution Provider (CSP) program fejleményeire és a licencelési program megnyitására

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-15
- Képességek

### <a name="summary"></a>Összefoglalás

Az új kereskedelmi és közszektorbeli örökös szoftverek a Cloud Solution Provider (CSP) programba kerülnek, valamint az Open licencelési program módosításait.

### <a name="impacted-audience"></a>Érintett közönség

A nyílt licencelési programon keresztül árusító kereskedelmi terjesztők és felügyelt viszonteladók, valamint az örökös szoftvereket lebonyolító CSP-partnerek

### <a name="details"></a>Részletek

A Microsoft szeptember 2020-án [bejelentette](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a digitális átalakulás lépéseinek egy sorozatát, amely kibővíti a partnereinkkel kapcsolatos lehetőségeket a CSP programban, beleértve a helyszíni szoftverek rendelkezésre állását a partnerek számára. Ezek a változások lehetővé teszik, hogy a partnerek a CSP-ben a szoftver licenceit kihasználva növeljék üzleti tevékenységüket Emellett képessé teszik az ügyfeleket a felhőre való áttérésre, és lehetővé teszik a partnerek számára a hibrid felhőalapú környezetekhez szükséges rugalmasságot.

A digitális átalakítás folytatásakor a következő módosításokat tesszük közzé:

- 2021. július 1-jén: a program nem ad hozzá új SKU-t, terméket vagy előléptetést az Open szoftverlicenc-árlista listájához.

- Július 7., 2021: két kereskedelmi ajánlat, valódi Windows-és Visual Studio Professional-és nyilvános szektor-ajánlatok (kormányzati, oktatási és nonprofit – lásd a [bejelentést](./2020-december.md#9)) a CSP Perpetual Software Prices listához lesznek hozzáadva.  Az árlista a partner Center [értékesítési > díjszabása & ajánlatok](https://partnercenter.microsoft.com/pcv/sales) oldalának szoftver szakaszában található, és ezen a napon újra közzé lesz téve.

A CSP-program evolúciójának és a licencelési program változásának részletes ismertetését az alábbi, **következő lépésekben** találhatja meg.

### <a name="next-steps"></a>További lépések:

- CSP-program evolúciója: Tekintse át az [örökös szoftvereket a Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) készenléti anyagaiban. Ezzel a [készültségi térképsel](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) gyorsan megtalálhatja a szerepkörének megfelelő információkat.

- A licencelési program módosításainak megnyitása: Tekintse át a [CSP-program evolúcióját, és nyissa meg a licencelési program változásait](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) . Ezzel a [készültségi térképsel](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) gyorsan megtalálhatja a szerepkörének megfelelő információkat.

### <a name="questions"></a>Kérdések

További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeit.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Frissítés korábbi bejelentésre: prémium szintű felmérések, a megfelelőségi vezető bővítménye

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-15
- Vállalkozás fejlesztése

### <a name="summary"></a>Összefoglalás

A próbaverziós ajánlatokat nem lehet listázni az árlista alapján, és el lesznek távolítva.

### <a name="impacted-audience"></a>Érintett közönség

Felhőalapú megoldás-szolgáltatón keresztül lebonyolított partnerek

### <a name="details"></a>Részletek

A próbaverziós ajánlatokat nem tartalmazza az árlista. Ezeket a rendszer eltávolítja a 2021-es árlista-listából.

Az eredeti hirdetmény [itt](./2021-february.md#4)található.

### <a name="additional-resources"></a>További források

- [Az E5 biztonsági és megfelelőségi Microsoft 365](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Értékelések készítése és kezelése a Microsoft megfelelőségi kezelőjében – Microsoft 365 megfelelőség](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Következő lépések

Tekintse át a témakör erőforrásait, és ossza meg ezeket az információkat a szervezete megfelelő szereplőivel.

### <a name="questions"></a>Kérdése van?

Az ajánlatokkal kapcsolatos kérdésekben keresse meg a megfelelő Yammer-közösségeket.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Megoldásait áttelepítheti egy kereskedelmi partnertől (OCP) a Microsoft kereskedelmi Marketplace-re (GTM)

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-12
- Képességek

### <a name="summary"></a>Összefoglalás

2021. március 29-én elkezdjük korlátozni a kereskedelmi partneri (OCP) piacra lépéseit (GTM). Javasoljuk, hogy telepítse át megoldásait a kereskedelmi piactérre a partner Centerben.

### <a name="impacted-audience"></a>Érintett közönség

OCP GTM-megoldásokkal közösen értékesítő szervezetek

### <a name="details"></a>Részletek

2020 decemberében kezdtük el utunkat a Microsoft OCP GTM eszközről a Microsoft kereskedelmi piactérről a partner Centerben. Ez az áttérés kibővíti a kereskedelmi piactér képességeit, ahol több millió ügyfél számára is kiterjesztheti megoldásait, és kétirányú módon megoszthatja a lehetőségeket más Microsoft-és partner-értékesítővel, és közösen értékesítheti az innovatív megoldásokat.

Az áttérés következő mérföldköve a 2021. március 29-én kerül megadásra. Ez az, amikor elkezdi megtapasztalni a korlátozott OCP GTM képességeket, és egyes mezők csak olvashatók lesznek. Ha jelenleg a OCP GTM-megoldásokkal együtt értékesíti a megoldásokat, javasoljuk, hogy a megoldásait a kereskedelmi piactérre telepítse át, hogy kiaknázza a képességeit, és egyszerűsítse a közzétételi élményt. 

A kereskedelmi piactérre való áttéréssel a partneri központ az elsődleges cél a közös értékesítésű közzétételi élmény. Így tovább bővítheti üzleti tevékenységét úgy, hogy a Microsoft-termékekhez hasonló csatornákkal és a termékkel kapcsolatos felhasználói élményekkel összeköti megoldásait közös ügyfeleinkkel. [További információ a kereskedelmi piactérről](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Következő lépések

- Ha még nem helyezte át a megoldásait, kövesse az [áttérési útmutatóban](/azure/marketplace/co-sell-solution-migration) részletezett utasításokat, vagy tekintse meg az összes áttelepítési tevékenység befejezéséhez szükséges [útmutatót, és](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) kezdje el közzétenni a megoldás (oka) t a kereskedelmi piactéren.

- A OCP-GTM korlátozott képességekkel kapcsolatos kérdéseivel kapcsolatban tekintse meg a [Microsoft kereskedelmi piactéren feltett gyakori kérdések című szakaszban közzétett közös értékesítésre vonatkozó követelményeket](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf). (Lásd a "OCP GTM korlátozott képességek" című szakaszt, amely 2021. március 29-én kezdődik. ")

### <a name="questions"></a>Kérdése van?

Ha bármilyen kérdése van, vagy további információra van szüksége, forduljon az [ügyfélszolgálathoz](https://partner.microsoft.com/support/?stage=1) .

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Az új kereskedelmi élmény kibővítése az Azure-beli Cloud Solution Provider (CSP) program keretében

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-10
- Képességek

### <a name="impacted-audience"></a>Érintett közönség

Az Oroszországban lévő összes partner a Cloud Solution Provider (CSP) programon keresztül lebonyolítja a tranzakciót.

### <a name="details"></a>Részletek

A 10 2021. március 1-től örömmel jelentjük be, hogy elérhetővé tettük az **új kereskedelmi élményt az Azure-beli CSP-ben Oroszországban**. Ez a tapasztalat egyszerűsíti és javítja az Azure-szolgáltatások vásárlásának és felhasználásának módját. Emellett a CSP program partnereinek is egységes áttekintést nyújt az Azure díjszabásáról az értékesítési mozgások során, a globális konzisztencia, a számlázási dátum-igazítás és a Azure Cost Management elérésének USD-díja.

### <a name="next-steps"></a>Következő lépések

Számos erőforrás érhető el az új Azure-beli kereskedelmi élmény bevezetéséhez és további információk biztosításához. A legújabb gyakori kérdések, a paklik, a videók és egyebek a [CSP program frissítésének erőforrás-gyűjteményében](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)találhatók.

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>A partner Center szoftverlicenc-kulcsa és a letöltés teljesítése

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-04
- Képességek

### <a name="summary"></a>Összefoglalás

A partner Center szoftver letöltése és a licencek kulcsának teljesítésére szolgáló képesség vissza lett állítani.

### <a name="impacted-audience"></a>Érintett közönség

Minden olyan felhőalapú megoldás-szolgáltatói (CSP) partner, amely az örökös és a kiszolgálói előfizetési szoftverek rendeléseit a partner centeren keresztül

### <a name="details"></a>Részletek

A partneri visszajelzések megválaszolásával a visszaállítja teljesítjük a szoftver-és licenckulcs beszerzését az örökös és a kiszolgálói előfizetési szoftverek rendeléseihez. A rendszer a korábbi állapotába állítja vissza, mielőtt a 2021. január 19-én megszűnik. (Lásd a [közleményt](2020-september.md#17).)

Vegye figyelembe, hogy a szoftverlicenc-kulcsok és a letöltési hivatkozások értékesek és rendkívül keresettek a szellemi tulajdonban lévő eszközök után. Ha kiszivárgott, gyorsan kimerítheti az aktiválási korlátokat, és negatív ügyfél-és partneri élményt eredményezhet.

### <a name="next-steps"></a>Következő lépések

Tekintse át a következő forrásokat a használati utasításokhoz, valamint a szoftveres kulcs terjesztésével kapcsolatos fontos útmutatást:

- [Helyszíni szoftverek értékesítése a CSP programon keresztül](../csp-on-premise-software.md)
- A [partner Center új kereskedelmi üzemeltetési útmutatója](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (lásd: **útmutató a szoftveres kulcs terjesztéséhez** .)

### <a name="questions"></a>Kérdése van?

Ha további kérdése van a nyilatkozattal kapcsolatban, tekintse meg a megfelelő Yammer-közösségeket.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>A partner értékesítési összekötő (PSC) és a partner Center közötti ajánlatok áttelepíthetők

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-04
- Képességek

### <a name="summary"></a>Összefoglalás

A partner Sales-kapcsolódás (PSC) a 2021-as naptól kezdődő írásvédett hozzáférésre vált, ezért javasoljuk, hogy kezdje el áttelepíteni az ajánlatokat a PSC-ből a partneri központba.

### <a name="impacted-audience"></a>Érintett közönség

Partnerek a PSC-ben található ügyletekkel

### <a name="details"></a>Részletek

A növekedés iránti közös elkötelezettségünk részeként a **Microsofttal közösen értékesítjük** a **felderített, szakértelmét, és kiterjesztjük** az ügyfél-lábnyomot a pozitív ügyfelek eredményeire. Ha átlagosan **3,5-szor gyorsabb** , mint a normál, a partner Center közös értékesítésű felhasználói élményének kezelése lehetővé teszi a közvetlen ügyfél-, partner-és Microsoft-értékesítői csatornák értékesítését, és egy helyen kezelheti a teljes átirányítási folyamatot.

A **PSC** a **2021**-as naptól kezdve **csak olvasási hozzáférésre** kerül át, ezért javasoljuk, hogy indítsa el a partneri központba való áttérést 

- A Microsoft és a megfelelő eladó közötti megosztások **pontosabb irányítása** a szükséges segítségnyújtási típus alapján.
- **Előzetes támogatási jogosultságok érvényesítése** az ösztönzőre jogosult megoldások esetében, valamint az ISV kapcsolódási program feltételeinek teljesítése, a jóváhagyási folyamat és a végrehajtás végleges igazolása (PoE) igazolása.
- **Zökkenőmentes felhasználói élmény** , amellyel egyetlen helyen kezelheti az összes közös értékesítéssel kapcsolatos lehetőséget és értékesítési minősítéssel rendelkező érdeklődőket.

Nemrégiben új funkciókat is hozzáadott a partner Centerben, hogy segítséget nyújtson az áthelyezéshez:

- [Tömeges műveletek közös értékesítési lehetőségekhez](../bulk-operations.md)
- Az [ügylet áttelepítési funkciója](../psc-to-pc.md) (lásd: a **PSC-ajánlatok áttelepítése** szakasz)

Az értékesítési csapatoknak több idő áll rendelkezésére a partner Center közös értékesítéssel kapcsolatos tapasztalataira, így az érdeklődők és a lehetőségek kiépítésére, az ajánlatok bezárására és a tartós ügyfélkapcsolatok létrehozására összpontosítanak.

### <a name="next-steps"></a>Következő lépések

A partneri központ [áttérési útmutatója](../psc-to-pc.md) végigvezeti Önt az ajánlatok PSC-ből a partneri központba való átirányításának lépésein.

### <a name="questions"></a>Kérdése van?

További kérdésekért forduljon az [ügyfélszolgálathoz](https://partner.microsoft.com/support/?stage=1).

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Új Microsoft Dynamics 365-termékek és-ajánlatok, amelyek az 2021. április 1-jén érhetők el

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-04
- Képességek

### <a name="summary"></a>Összefoglalás

2021. április 1-jén a Microsoft számos új terméket és ajánlatot indít el a Cloud Solution Provider (CSP) programhoz.

### <a name="impacted-audience"></a>Érintett közönség

Minden partner a Cloud Solution Provider (CSP) programon keresztül lebonyolít

### <a name="details"></a>Részletek

2021. április 1-jén a Microsoft a következő új termékeket és ajánlatokat fogja elindítani:

- Felhasználónként Power BI Premium
- Az ügyfelek hang-és marketing-felhasználói előfizetési licenc földrajzi és szegmensek bővítése

**Felhasználónként Power BI Premium**

A Microsoft az első felhasználónkénti Power BI Premium ajánlatokat fogja bevezetni. A Power BI Premium jelenleg csak egy kapacitás-konstrukcióban értékesíti. A felhasználónként Power BI Premium hozzáférést biztosít a vállalati üzleti intelligencia (BI) és az elemzési funkciókhoz. A rugalmas egyéni munkaállomás-licencelés kis-és közepes méretű vállalkozások számára is elérhető.

Tekintse át a [Power bi kiadásának részleteit](/power-platform-release-plan/2020wave2/power-bi/planned-features) , és tudjon meg többet az ajánlatról.


**Ajánlat részletei**

Vegye figyelembe, hogy az ajánlat neve kis mértékben eltér a árlista előzetes verziójától.

| Ajánlat neve | Ajánlat azonosítója |
| ------ |----------- |
| Felhasználónként Power BI Premium | 9c810018-9356-4903-95ab-eeb956289290 | 
| Felhasználónként Power BI Premium oktatóknak | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Felhasználónként Power BI Premium tanulók számára | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Felhasználónkénti Power BI Premium (nonprofit alkalmazottak díjszabása) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Felhasználónként Power BI Premium Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium felhasználói Add-On oktatóknak | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium felhasználónként Add-On diákoknak | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Felhasználónkénti Add-On Power BI Premium (nonprofit alkalmazottak díjszabása) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Az ügyfelek hang-és marketing-felhasználói előfizetési licenc földrajzi és szegmensek bővítése**

A decemberi 2020-es indítás után a Dynamics 365-ügyfelek hang-és marketing-felhasználói előfizetési licenc ajánlatai új országok és több nonprofit és oktatási SKU hozzáadására lettek kialakítva.

| Ajánlat neve | Ajánlat azonosítója |
| ------ |----------- |
| Dynamics 365-ügyfél hangalapú felhasználói előfizetési licenc (nonprofit személyzet díjszabása) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dynamics 365-ügyfelek hang-felhasználói előfizetési licenc az oktatók számára | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

A következő lapokon további információkat talál az ajánlatokról:

- [Dynamics 365 ügyfél-szolgáltatás hangpostájának kezdőlapja](https://dynamics.microsoft.com/customer-voice/overview/)
- [Dynamics 365 marketing Kezdőlap](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Következő lépések

Tekintse át a témakör erőforrásait, és ossza meg ezeket az információkat a szervezete megfelelő szereplőivel.  

### <a name="questions"></a>Kérdése van?

Az ajánlatokkal kapcsolatos bármilyen kérdés esetén keresse meg a megfelelő Yammer-közösségeket. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> A Microsoft Universal Print már elérhető néhány lakosztályban

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-33
- Képességek

### <a name="summary"></a>Összefoglalás

A Microsoft Universal Print elérhető lesz a Select Microsoft 365 Suite-ban, valamint önálló bővítményként, 2021. március 1-től.

### <a name="impacted-audience"></a>Érintett közönség

Minden partner a Cloud Solution Provider (CSP) programon keresztül lebonyolít

### <a name="details"></a>Részletek

Az [univerzális nyomtatás](https://aka.ms/universalprint) egy Microsoft 365 nyomtatási szolgáltatás, amely eltávolítja a helyszíni nyomtatókiszolgálók szükségességét, és lehetővé teszi a Windows-eszközök számára az Azure-ban regisztrált nyomtatókhoz való nyomtatást. A tranzakció 2021. március 1-től lesz elérhető.

A feldolgozók kihasználhatják az illesztőprogram nélküli nyomtatást, a egyszerűsített helymeghatározást, valamint az intuitív nyomtatási élményt tanulási görbe nélkül. A Azure Active Directoryhoz (Azure AD) csatlakoztatott eszközök a meglévő Azure AD-beli hitelesítő adatokat használják a biztonságos nyomtatáshoz. A rendszergazdák a Azure Portal használatával kezelhetik a nyomtatást, és könnyen csatlakoztathatók a nyomtatók az univerzális nyomtatás natív támogatásával. Az univerzális nyomtatás a nem kompatibilis nyomtatókra is telepíthető univerzális nyomtatási összekötő szoftver használatával.

Az univerzális nyomtatás a Windows E3, a3, E5 és a5 nyelven, valamint Microsoft 365 a BP, az F3, az E3, az a3, az E5 és az A5 nyelven is visszatöltötte.  

**Ajánlat részletei**

Vegye figyelembe, hogy az ajánlat neve kis mértékben eltér a árlista előzetes verziójától.

| Ajánlat neve | Ajánlat azonosítója | Anyag azonosítója |
| ------ |----------- |----------- |  
| Univerzális nyomtatási kötet bővítmény (500 feladat) – Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Univerzális nyomtatási hangerő bővítmény (500-es feladat) az oktatók számára – Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Univerzális nyomtatási kötet bővítmény (500 feladat) – Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Univerzális nyomtatási hangerő bővítmény (500 feladat) a kari-Windows rendszerhez   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Következő lépések

Ismerkedjen meg az árlista és az [univerzális nyomtatás áttekintése](/universal-print/fundamentals/universal-print-whatis)szolgáltatással. Ossza meg ezeket az információkat a szervezet összes megfelelő ügyfelével.

### <a name="questions"></a>Kérdése van?

Az ajánlatokkal kapcsolatos bármilyen kérdés esetén keresse meg a megfelelő Yammer-közösségeket.
