---
title: 2021. márciusi bejelentések
description: A Microsoft 2021. márciusi közleményei Partnerközpont új képességeket, promóciókat, ajánlatokat, piacokat vagy a meglévő ajánlatok változásait is beleértve.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 17b8082b8a42050892ff434010952d5f91a39431
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328066"
---
# <a name="march-2021-announcements"></a>2021. márciusi bejelentések

Ez az oldal a Microsoft 2021. márciusi Partnerközpont bejelentését mutatja be.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a>Készenlét: A Felhőszolgáltató (CSP) ügyfélcím-ellenőrzési API-jának változásai júniusban érvénybe fognak tolni; tesztelési képesség már elérhető

### <a name="categories"></a>Kategóriák

- Dátum: 2021-04-30
- Készenlét

### <a name="summary"></a>Összefoglalás

Annak érdekében, hogy a partnerek és az ügyfelek bizalom alapján futtassanak üzletüket, meghívjuk a partnereket, hogy teszteljék a Validate Address API módosításait az összes országban világszerte.

### <a name="impacted-audience"></a>Érintett célközönség

A CSP közvetlen számlázási partnerek és közvetett szolgáltatók, akik új ügyfeleket hoznak létre vagy frissítik a címadatokat.

### <a name="details"></a>Részletek

A Microsoft megbízhatósági kapcsolaton fut. Elkötelezettek vagyunk amellett, hogy megfelelő, biztonságos és biztonságos módszert biztosítsunk az ügyfélcímek érvényesítéséhez az ügyfél-előfizetések tranzakciója során a CSP-programban. 2021. március 31-én bevezettük a Validate Address API módosításait, amelyek tesztelésére hívtuk meg a partnereket, mielőtt a 2021. júniusi változásokat bevezettük volna.

A módosítások csak a Validate Address API-t érintik. A Create Customer and Update Billing Profile API-kat ez nem befolyásolja.

A válasz a következő állapotüzenetek egyikét adja vissza:

| Állapot     | Leírás |    A visszaadott javasolt címek száma |
|-------|---------------|-------------------|
|Ellenőrzött szállításra használható | A cím ellenőrizve van, és szállítható a címre. | Egyirányú |
|Ellenőrzött | A cím ellenőrizve van. | Egyirányú |
|Beavatkozás szükséges | A javasolt cím jelentős mértékben módosult, és a felhasználó megerősítését kell kér. | Egyirányú |
|Utca részleges | A címben megadott utca részleges, és további információra van szüksége. | Többszörös – legfeljebb három |
|Részleges helyszín | Az adott helyszín (épületszám, csomagszám stb.) részleges, és további információra van szüksége. | Többszörös – legfeljebb három |
|Többszörös | Több mező is részleges a címben (beleértve az utca részleges és a helyszíni részleges mezőket is). | Többszörös – legfeljebb három |
|Nincsenek | A cím helytelen. | Nincsenek |
|Nincs ellenőrizve. | A cím nem lett elküldve az érvényesítési folyamaton keresztül. | Nincsenek |

Az USA-nak az irányítószámai további 4 számjegyet és kötőjelet ( például 12345-6789) fognak visszaadni.

Miután a Validate Address API-val elküldött egy címet ellenőrzésre, a rendszer a következő válaszsémát fogja visszaadni:

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

Nézze meg ezt a mintaválaszt. Vegye figyelembe, hogy az Egyesült Államok esetén a válasz egy további négyjegyű utótagot ad vissza az irányítószámhoz, ha csak öt számjegyet ad meg az irányítószámhoz.

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>Következő lépések

- Ossza meg a tesztgép bérlőazonosítóját a témaszakértővel (Ali Sandki), aki szerepelni fog a tesztúton, hogy megkezdje a frissítés előkészítését.

- Ha vezérlőpult-szállító (CPV) megoldást használ, tekintse meg a CPV-t.

### <a name="questions"></a>Kérdése van?

Ha támogatásra van szüksége a Microsofttal kapcsolatos műveleteihez, a partnertámogatási Yammer-csoporthoz kell segítséget nyújtanunk.

### <a name="change-log"></a>Változásnapló:

- 2020. március 31. : Eredeti közzététel

- 2021. április 30.: A mintaválasz és az irányítószám részleteinek frissítései

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>Új Exchange felügyeleti központ (EAC) felhasználói élmény

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-29
- Képességek

### <a name="summary"></a>Összefoglalás

2021. április 27-től az Exchange felügyeleti központ (EAC) új felhasználói élményt nyújt, amely javítja a felhasználók napi hatékonyságát.

### <a name="impacted-audience"></a>Érintett célközönség

Az Exchange-et a Partnerközpont

### <a name="details"></a>Részletek

2021. április 27-től az Exchange-hez Partnerközpont az új EAC-hoz lesznek átirányítva.

Ez az új felület jelenleg előzetes verzióként érhető el, és a rendszergazdák a klasszikus EAC jobb felső sarkában található váltógombot választva aktiválják ezt a felhasználói élményt. Az összes oldalon megjelenő "Kipróbálom most" szalagcímre kattintva is navigálhat az új EAC-hoz.

Az új EAC előnyei többek között a következők:

- Elemzések, jelentések és riasztási mechanizmusok hozzáadva a levélforgalomhoz kapcsolódó problémákhoz. 

- Személyre szabott irányítópultok a hatékonyság növelése érdekében.

Az új felhasználói élményben való eligazodás érdekében a videók az új EAC-& képzési útmutató szakaszában érhetők el.  Ezek áttekintést nyújtanak arról, hogyan használhatja a legjobban az új portált.

>[!NOTE]
>Ezzel a módosítással a klasszikus EAC-élmény nem lesz elavult. A változások megvalósítása előtt értesítést kap.

### <a name="next-steps"></a>Következő lépések

- Tekintse meg az [ezzel a témakörvel](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)kapcsolatos forrásokat, ahol képernyőképeket készíthet az új felhasználói élményről.

- Ossza meg ezt az információt a szervezet megfelelő érdekelt felével. 

### <a name="questions"></a>Kérdése van?

A változásokkal kapcsolatos kérdésekért tekintse meg az érintett Yammer-közösségeket.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Microsoft Operations: A termékindítási naptár bevezetése

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-25
- Ajánlatok | Modern munkahely

### <a name="summary"></a>Összefoglalás

A microsoftos visszajelzésekre reagálva a Microsoft Operations leegyszerűsíti a termékbeindítások kommunikációját.

### <a name="impacted-audience"></a>Érintett célközönség

Felhőszolgáltató (CSP) partnerek

### <a name="details"></a>Részletek

A Microsoft elkötelezett amellett, hogy folyamatosan javítsa a partneri élményeket. Visszajelzést kaptunk Öntől, hogy túl sok információt kapott a Microsofttól, beleértve a termékbeindítások duplikált bejelentéseit is.

Visszajelzésére válaszul a Microsoft leegyszerűsíti a termékindítások készenlétét az új és meglévő ajánlatokhoz.

Mostantól a termékindítások egyetlen havi nézetét biztosítjuk, amely az Operations readiness erőforrás-katalógusban van közzétéve. Ez a [havi termékindítási naptárnézet](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) felváltja az egyes termékindítási kommunikációt az Üzemeltetési készenlét erőforrás-katalógusban és a Partnerközpont közlemények között.

A termékindítási [](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) naptárt közösségi gyűjtemények, [](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)naptárnézetek [és](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated) [CSP-hírlevelek segítségével is elérheti.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/) Az egyes hónap termékindítási naptárának közzétételekor értesítést adjuk át az Operations readiness erőforrás-katalógusban található bejelentéssel.

Az új és meglévő ajánlatokkal kapcsolatos információkat az árlista előnézetében és az árlista változásnaplóiban, valamint a termék blogjaiban, licencelési útmutatóiban és termék marketingoldalán találja.

A módosítás a következő termékek indítására vonatkozik:

- Helyszíni Dynamics
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Kiszolgáló  
- Eszközök
- Teams és Telco

Továbbra is küldünk olyan termékindításokkal kapcsolatos konkrét közleményeket, amelyekhez műveleti készenlétre vonatkozó részletekre van szükség.

### <a name="next-steps"></a>Következő lépések

Tekintse át a témakörre vonatkozó forrásokat, és ossza meg ezt az információt a szervezet megfelelő érdekelt felével.

### <a name="questions"></a>Kérdése van?

Az ajánlatokkal kapcsolatos további kérdésekért tekintse meg az érintett Yammer-közösségeket.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>A CSP-ügyfelekre vonatkozó, az ügyfelekre vonatkozó követelmények változásai

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-25
- Képességek

### <a name="summary"></a>Összefoglalás

Elkötelezettségünk részeként, hogy segítsünk a partnereknek és az ügyfeleknek a bizalmi kapcsolaton alapuló üzleti tevékenységben, további ügyféladatokat kérünk 2021. március 25-ig.

### <a name="impacted-audience"></a>Érintett célközönség

Felhőszolgáltató (CSP) közvetlen számlázási partnerek és közvetett szolgáltatók, akik új vagy meglévő ügyfelekkel vannak a következő szakaszban felsorolt országokban

### <a name="details"></a>Részletek

A Microsoft megbízhatósági kapcsolaton fut. Elkötelezettek vagyunk amellett, hogy megfelelő, biztonságos és biztonságos ügyfél-ellenőrzési módszert biztosítsunk az ügyfél-előfizetések tranzakciója során a CSP-programban. 2021. március 25-én bevezetünk egy API- és felhasználói felületi (UI) fejlesztéseket Partnerközpont, amelyek hatással lesznek az alábbi két feltételnek megfelelő partnerekre:

1. A partner közvetlen számlázási kapcsolattal rendelkezik a Microsofttal (ami azt jelenti, hogy a partner közvetlen számlázási partner vagy közvetett szolgáltató).

2. A partner az alábbi országokban lévő új vagy meglévő ügyfelekkel működik együtt:

    - Thaiföld
    - Vietnam
    - Törökország
    - Lengyelország
    - Dél-afrikai Köztársaság
    - India
    - Brazília
    - Irak
    - Mianmar
    - Dél-Szudán
    - Szaúd-Arábia
    - Egyesült Arab Emírségek
    - Venezuela

A feltételeknek megfelelő partnereknek be kell majd nyújtaniuk az ügyfél céges regisztrációs azonosítóját **(más** néven az ügyfél szervezeti **INN-ét)** és telefonszámát, amikor új ügyfeleket regisztrálnak vagy módosítják a meglévő ügyféladatokat.  Ezek a partnerek **középső nevet** is megadhatnak az ügyfél számára.

Vegye figyelembe, hogy a céges regisztrációs azonosító hozzáadásakor az üzleti adóazonosítót kell használnia, nem az ügyfél személyes azonosítóját.

Azok a partnerek, akik az alábbi országokban lévő új vagy meglévő ügyfelekkel üzleti partnereket hoznak létre, már elő vannak útjára 2020 novemberében egy korábbi kiadással.

- Örményország
- Azerbajdzsán
- Belarusz
- Magyarország
- Kazahsztán
- Kirgizisztán
- Moldova
- Oroszország
- Tádzsikisztán
- Ukrajna
- Üzbegisztán

A világ többi részén az ügyfelekkel való együttműködésre 2021. március 25-én lehetősége  lesz megadni az ügyfelek céges regisztrációs azonosítóját, telefonszámát és középső nevét opcionális részletekként. 

### <a name="next-steps"></a>Következő lépések

- Részletesebb útmutatásért tekintse át a műszaki dokumentációt és a dedikált [partnergyűjteményben](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) található gyakori kérdéseket.

- Készüljön fel arra, hogy a módosításokat a Partnerközpont API és a webes felhasználói felület használatával építse be. Az API/SDK-k elérhetők lesznek a teszteléshez.

- Az új ügyfelek be- és módosításakor küldje el a további adatokat.

- Ha vezérlőpult-szállító (CPV) megoldást használ, tekintse meg a CPV-t.

### <a name="questions"></a>Kérdése van?

Ha bármilyen kérdése van a jogi azonosítóval (más néven INN-rel vagy TIN-sel) kapcsolatban, forduljon az adótanácshoz vagy a helyi adóhivatalhoz. A Microsoft nem tud útmutatást nyújtani az adózási kérdésekkel kapcsolatban.

Ha támogatásra van szüksége a Microsofttal kapcsolatos műveleteihez, [nyisson meg egy szolgáltatáskérést.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>A 2021. március 1-jén végleges szoftverárlistán tett javítások

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-23
- Ajánlatok/piacok

### <a name="impacted-audience"></a>Érintett célközönség

Közvetlen szolgáltatók és közvetlen számlázási partnerek, akik állandó szoftvereket tranzakcióznak a Felhőszolgáltató programjában 

### <a name="details"></a>Részletek

A 2021. március 1-jén közzétett végleges szoftverek árlistja olyan piacokat is tartalmazott, amelyekre nem kellett volna. A végleges szoftverárak listája 2021. március 17-én frissült a javításokkal. Ezek a javítások csak a következőre voltak alkalmazhatók:

- Termékazonosító: DF77X4D43RKT 
- Terméknév: Windows 10 Home termék pro verziófrissítése a Microsoft 365 business termékhez
- Eltávolított vagy nem támogatott piacok: AE, AF, AL, AM, AO, BA,ZŐ, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Ezek a módosítások csak a fenti termékre vonatkoznak. Más termékeknél nem voltak javítások. 

### <a name="next-steps-and-resources"></a>Következő lépések és erőforrások

- A folyamatos szoftvereket tranzakció partnereknek le kell töltenie a legújabb végleges szoftverárlistát.
- A [kétbetűs](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) rövidítés országokra való rövidítésének felhasználóbarát leképezéséhez tekintse meg a régió országkódját.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> SDK-kiadás a .NET Standardon (1.17.0-s verzió)

### <a name="categories"></a>Kategóriák

- Dátum: 2021. 03. 23.

- Képességek
 
### <a name="impacted-audience"></a>Érintett célközönség

A CSP-programban részt vevő közvetlen számlázási partnerek és közvetett szolgáltatók, akik az Partnerközpont .NET SDK-t használják.

### <a name="details"></a>Részletek

2020. március 23-án a partnerek elkezdik letölteni a [MicrosoftPartnerCenter.NETSDK (NuGet gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), valamint frissített nyilvános Partnerközpont SDK [GitHub-minták.](https://github.com/Microsoft/Partner-Center-DotNet-Samples) Ez a verzió a következő metódusok frissítéseit tartalmazza:

#### <a name="audit-updated-new-operation-types"></a>Audit frissítve: Új művelettípusok

Új [művelettípusok hozzáadva annak](https://docs.microsoft.com/partner-center/develop/auditing-resources) tudatában, hogy az ügyfél mikor hagyta jóvá és szüntette meg a DAP-t.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Audit frissítve: Új erőforrás- és művelettípusok

Új [erőforrás- és művelettípusok hozzáadva](https://docs.microsoft.com/partner-center/develop/auditing-resources) az ügyfél címtárszerepkör-forgatókönyvének támogatásához.

- Új erőforrástípus: "CustomerDirectoryRole"

- Az "AddUserMember" és a "RemoveUserMember" művelettípusok

#### <a name="sdk-updates-to-customer-accounts"></a>SDK-frissítések az ügyfélfiókok számára

- GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus támogatása

- GET /customers/{customer-tenant-id}/qualifications

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>További módosítások

A következő változások az új kereskedelem részeként érhetők el, és jelenleg csak az M365/D365 Új kereskedelmi felhasználói élmény technikai előzetes kiadásának partnerei számára érhetők el meghívással. Azok a partnerek, akik nem részei az Új kereskedelem technikai előzetes kiadásának, nem láthatják a hatásokat, és visszamenőlegesen kompatibilisnek kell lenniük.

- Katalógusváltozások:

  - GET /products/{termékazonosító}/skus/{sku-id}

- Vásárlás és kezelés:
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Következő lépések

- Töltse le a [MicrosoftPartnerCenter.NETSDK legújabb verzióját (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- A [GitHub-minták letöltése és áttekintése](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>CSP kereskedelmi piactéri ajánlat és FY21 CSP-ösztönzők jogosult ajánlatokhoz

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-18
- Képességek

### <a name="impacted-audience"></a>Érintett célközönség

Közvetett szolgáltatók és közvetlen számlázási partnerek a Felhőszolgáltató programjában 

### <a name="details"></a>Részletek

A Felhőszolgáltató program közvetett szolgáltatói és közvetlen számlázási partnerei értékesíthet harmadik féltől származó ajánlatokat, és ösztönző ösztönzőt kaphatnak a Partnerközpont vagy a Azure Portal. Az ösztönző a jogosult ajánlatok kiszámlázott értékesítésének **2021. június 30-ig lesz elérhető.**  

Folytassa a lenti, CSP kereskedelmi piactéri ajánlatra vonatkozó ösztönzővel kapcsolatos további tanulást, és vegye fel a kapcsolatot az ügyfelekkel még ma, hogy azonosítsa a megfelelő ajánlatokat, amelyek lehetővé teszik a folyamatos sikerüket és a digitális átalakulást.

A független szoftverszállítók (ISV-k) segítségével a legújabb IaaS- és SaaS-megoldásokat kínáljuk a Microsoft ügyfeleinek. Az ISV-közzétevőknek lehetősége van engedélyezni az ajánlataik értékesítését a Microsoft partnercsatornáján keresztül. Az ösztönzőre jogosult ajánlataink két kategóriába sorolhatók:

- Válassza az Azure IP-cím alapú közös értékesítés incentivált állapotú SaaS- és IaaS-ajánlatokat. 

- A Teamsbe integrált SaaS-alkalmazások vagy legalább Microsoft 365 alkalmazások, például a PowerPoint, a Word, az Excel, az Outlook vagy a SharePoint.

### <a name="next-steps-and-resources"></a>Következő lépések és erőforrások

- Ismerje meg, hogyan szerezhet [partneri ösztönzőket](https://partner.microsoft.com/membership/partner-incentives) a jogosult Marketplace-alkalmazások értékesítéséhez az ösztönzőre jogosult alkalmazásokhoz. Az új ajánlatok hozzáadása havonta történik.  
- [Felhőszolgáltató partneri ösztönzőerőforrások közvetlen számlázása](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Felhőszolgáltató közvetett szolgáltatói ösztönzőerőforrások](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Tekintse át ezt [a bemutatót,](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) ha többet szeretne megtudni a kereskedelmi piactéren elérhető alkalmazások értékesítésről. További forrásokat itt [is meg lehet nézni.](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/) 
- Ismerkedés a kereskedelmi piactér-katalógussal [Partnerközpont](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) vagy [Azure Portal](https://ms.portal.azure.com/#home)
- Alkalmazások [integrálása](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) a vállalat piacterébe API-k használatával
- Érdeklődjön azokkal a isvv-ekkel, amelyek érdeklik az üzletben
- A közvetett szolgáltatóknak API-k használatával kell integrálni az integrációt, és útmutatást kell adni a viszonteladóknak az értékesíthető alkalmazásokhoz

### <a name="questions"></a>Kérdése van?  

Ebben [a cikkben áttekintheti](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) a kereskedelmi piacteret a Partnerközpont.

Ha további segítségre van szüksége, hozzon létre egy támogatási kérést a Partnerközpont. További információ: [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium ajánlat elnevezése és előfeltétel-frissítése

### <a name="categories"></a>Kategóriák

- Dátum: 2021. 03. 18.
- Képességek

### <a name="summary"></a>Összefoglalás

A 2021. április 1-i végleges árlista frissülni fog, hogy érthetőbb legyen az egyes Power BI Premium ajánlatokkal kapcsolatos elnevezési és/vagy előfeltétel-információk.

### <a name="impacted-audience"></a>Érintett célközönség

Felhőszolgáltató (CSP) közvetlen és közvetett partnerek

### <a name="details"></a>Részletek

A 2021. április 1- és 2021-es végleges árlista frissül, hogy érthetőbb legyen az egyes Power BI Premium ajánlatok elnevezési és/vagy előfeltétel-információi.

A végleges árlista frissítésig az ebben a szakaszban található információk alapján győződjön meg arról, hogy a megfelelő termék van megrendelve.

Az alábbi részletek az érintett termékváltozatot és előfeltétel-részleteket mutatják be.

| Ajánlat megjelenítendő neve a március 1-i árlista előzetes kiadásában |  Frissített ajánlat megjelenítendő neve az április 1-i végleges árlistán| Ajánlat azonosítója |
| ------ | ----------- | ----------- |
| Power BI Premium felhasználónkénti Add-On (nonprofit személyzet díjszabása)  |  Power BI Premium felhasználónkénti Add-On **(Office) (Nonprofit** személyzet díjszabása)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Az ügyfeleknek az alábbi előfeltételek bármelyikével kell előfeltételt adniuk az ajánlat megvásárlásához:

| Ajánlat megjelenítendő neve | Ajánlat azonosítója |
| ------ | ----------- |
| Microsoft 365 E5 (nonprofit alkalmazottak díjszabása)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 beállítása hangkonferencia nélkül (nonprofit alkalmazottak díjszabása)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (Nonprofit személyzet díjszabása)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Az Office 365 E5 próbaverziója (nonprofit személyzet díjszabása)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 audiokonferencia nélkül (nonprofit személyzet díjszabása)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

A következő Power BI Premium ajánlathoz előfeltétel szükséges a vásárláshoz:

| Ajánlat megjelenítendő neve | Ajánlat azonosítója |
| ------ | ----------- |
|   Power BI Premium felhasználónkénti Add-On (nonprofit személyzet díjszabása)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Az ügyfeleknek a következő előfeltételre van szüksége az ajánlat megvásárlásához:

| Ajánlat megjelenítendő neve | Ajánlat azonosítója |
| ------ |----------|
| Power BI Pro (Nonprofit személyzet díjszabása)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Következő lépések

Tekintse át a témakör erőforrásait, és ossza meg ezt az információt a szervezet megfelelő érdekelt felével.  

### <a name="questions"></a>Kérdése van?

Ha kérdései vannak ezekkel az ajánlatokkal kapcsolatban, tekintse meg az érintett Yammer-közösségeket. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Az F3 Microsoft 365 márciusi árának frissítései

### <a name="categories"></a>Kategóriák

- Dátum: 2021. 03. 16.
- Ajánlatok/piacok

### <a name="summary"></a>Összefoglalás

A 2021. márciusi díjszabás helytelenül lett kijavítva a Microsoft 365 font (GBP) és az euro (EUR) esetében.

### <a name="impacted-audience"></a>Érintett célközönség

Az F3 Microsoft 365 2021. március 1. és 2021. március 17. között gb/s-ban vagy EUR-ban megvásárlási Felhőszolgáltató (CSP) keretében.

### <a name="details"></a>Részletek

A Microsoft megoldotta az F3 Microsoft 365 díjszabását. A helytelen árak a GBP és az EUR esetében voltak, és csak a 2021. március 1. és 2021. március 17. között vásárolt ajánlatok esetében. Az érintett ajánlatok és pénznemek listája alább látható. 

| Ajánlat neve | Pénznem | Ajánlat azonosítója | Anyagazonosító |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (Rendszer) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (Kereskedelmi) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
A márciusi és áprilisi licencelési alapárak listája március 16-án, 17:00-kor frissült a csendes-óceáni téli idő szerint.

### <a name="next-steps"></a>Következő lépések

- A partnereknek újra le kell töltenie az aktuális licencalapú árlistát (március és áprilisi előzetes verzió) ezekkel az árkorrekcióval, ha van ilyen.  
- A Microsoft az elkövetkező hetekben e-mailben kapcsolatba lép az érintett partnerekkel, hogy tájékoztassa őket az érintett tranzakciók kijavítása során szükséges további lépésekről.

### <a name="questions"></a>Kérdése van?

További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeket.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Jogi vállalat nevének frissítése a Partnerközpont

### <a name="categories"></a>Kategóriák

- Dátum: 2021.03. 16.
- Drive Efficiency & Scale

### <a name="summary"></a>Összefoglalás

2021 márciusában Microsoft Partner Network (MPN) partnerek és Felhőszolgáltató (CSP) közvetett viszonteladók frissítheti jogi vállalatuk nevét a Partnerközpont.

### <a name="impacted-audience"></a>Érintett célközönség

MPN-partnerek és közvetett CSP-viszonteladók (nem vonatkoznak a közvetlen csp-számlázási partnerekre)

### <a name="details"></a>Részletek

2021 márciusánaktól az MPN-partnerek és a közvetett CSP-viszonteladók a vállalatuk jogi nevét a Partnerközpont, önkiszolgáló módon frissítheti. Ezzel az új funkcióval a partnereknek többé nem kell támogatási jegyet Partnerközpont a vállalatuk nevének frissítéséhez. Ez jelentős időt takarít meg a partnerek számára ezen tevékenységek végrehajtása során. 

További információ: [A jogi üzleti profil frissítése.](../update-your-partner-profile.md#update-your-legal-business-profile)

>[!NOTE]
>Győződjön meg arról, hogy a jogi üzleti profiljában a vállalat neve nem tartalmaz helyesírási hibákat és rövidítéseket, és pontosan megegyezik a hivatalos vállalati üzleti regisztrációs rekordokkal. A szervezeti profil frissítésével kapcsolatos további információkért lásd: [A szervezeti profil ellenőrzése.](../update-your-partner-profile.md#update-your-legal-business-profile)

### <a name="next-steps"></a>Következő lépések

Ossza meg ezt az információt a szervezeten belül, hogy a megfelelő csapat áttekintheti és frissítheti a folyamatait.

### <a name="questions"></a>Kérdése van?

További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeket.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Frissítés a Felhőszolgáltató (CSP) program fejlődése és az Open License program változásai

### <a name="categories"></a>Kategóriák

- Dátum: 2021. 03. 15.
- Képességek

### <a name="summary"></a>Összefoglalás

Az új kereskedelmi és közszférában elérhető folyamatos szoftveres ajánlatok a Felhőszolgáltató (CSP) programba, az Open Licensing Program változásaival együtt stb.

### <a name="impacted-audience"></a>Érintett célközönség

A kereskedelmi terjesztők és a felügyelt viszonteladók, akik az Open License programon keresztül értékesítik őket, valamint minden CSP-partner, amely állandó szoftvereket értékesít

### <a name="details"></a>Részletek

2020 szeptemberében [a](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) Microsoft bejelentette a digitális átalakulási folyamat lépéseit, hogy bővítse a CSP-program partnereinek lehetőségeit, beleértve a helyszíni szoftverek elérhetőségét a partnerek számára. Ezek a változások lehetővé teszik a partnerek számára, hogy a felhőszolgáltató szoftverlicenceinek segítségével bővíthétsék a munkájukat, és sikerre jutnak napjaink felhőalapú világában. Emellett lehetővé teszi az ügyfelek felhőre való áttérését is, és a partnerek számára a hibrid felhőalapú ügyfélkörnyezetekhez szükséges rugalmasságot biztosítják.

A digitális átalakítás folytatásaként bejelentjük a következő változásokat:

- 2021. július 1.: Az Open License program árlistába nem kerülnek új termékkódok, termékek vagy promóciók.

- 2021. július 7.: Két kereskedelmi ajánlat, a Get Genuine Windows és az Visual Studio Professional, valamint a közszférában elérhető ajánlatok (kormányzati, oktatási és nonprofit – lásd a [bejelentést)](./2020-december.md#9)bekerülnek a CSP folyamatos szoftverár-listájára.  Az árlista a Partnerközpont Értékesítés > Díjszabási ajánlatok [& oldalának](https://partnercenter.microsoft.com/pcv/sales) Szoftver szakaszában található, és ezen a napon lesz újból közzétenve.

A CSP-program fejlődésével és az Open License program változásaival kapcsolatos részletekért tekintse meg az alábbi **Következő lépéseket.**

### <a name="next-steps"></a>További lépések:

- CSP-program fejlődése: Tekintse át a folyamatos szoftvert a Felhőszolgáltató [készültségi](https://partner.microsoft.com/resources/collection/software-in-csp#/) anyagokban. Ezzel a [készenlét-leképezésvel](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) gyorsan megkeresheti a szerepkörének megfelelő információkat.

- Open License program módosításai: Tekintse át a [CSP-program](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) fejlődését és az Open License program módosításainak készültségi anyagát. Ezzel a [készenlét-leképezéspel](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) gyorsan megkeresheti a szerepkörének megfelelő információkat.

### <a name="questions"></a>Kérdések

További kérdésekért tekintse meg a megfelelő CSP Yammer-közösségeket.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Frissítés egy korábbi bejelentésre: Premium Assessments, a Compliance Manager bővítménye

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-15
- Vállalkozás fejlesztése

### <a name="summary"></a>Összefoglalás

A próbaverziós ajánlatoknak nem kellett volna szerepelve az árlistában, és el lesznek távolítva.

### <a name="impacted-audience"></a>Érintett célközönség

A partnerek tranzakciós Felhőszolgáltató

### <a name="details"></a>Részletek

A próbaverziós ajánlatoknak nem kellett volna szerepelniük az árlistában. Ezek el lesznek távolítva a 2021. május 1-i árlistáról.

Az eredeti bejelentés itt [van.](./2021-february.md#4)

### <a name="additional-resources"></a>További források

- [Microsoft 365 E5 biztonság és megfelelőség](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Értékelések összeállítása és kezelése a Microsoft Compliance Managerben – Microsoft 365 megfelelőség](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Következő lépések

Tekintse át a témakörre vonatkozó forrásokat, és ossza meg ezt az információt a szervezet megfelelő érdekelt felével.

### <a name="questions"></a>Kérdése van?

Az ajánlatokkal kapcsolatos kérdésekért tekintse meg az érintett Yammer-közösségeket.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Megoldások miminálása egy kereskedelmi partnertől (OCP) piaci útjára (GTM) a Microsoft kereskedelmi piacterére

### <a name="categories"></a>Kategóriák

- Dátum: 2021. 03. 12.
- Képességek

### <a name="summary"></a>Összefoglalás

2021. március 29-től korlátozott, piacra piacra ható (GTM) One Commercial Partner (OCP) képességeket fog tapasztalni. Javasoljuk, hogy megoldásait a kereskedelmi piactérre mi célra Partnerközpont.

### <a name="impacted-audience"></a>Érintett célközönség

Megoldások közös értékesítése az OCP GTM-megoldásokkal

### <a name="details"></a>Részletek

2020 decemberével kezdtük meg a Microsoft OCP GTM eszközével és a Microsoft kereskedelmi piacterével való Partnerközpont. Ez az átállás kibővíti a kereskedelmi piactér képességeit, ahol megoldásait ügyfelek milliói számára mutathatja be, kétirányúan oszthatja meg a lehetőségeket más Microsoft- és partner értékesítőkkel, és közösen innovatív megoldásokat értékesíthet.

Az átváltás következő mérföldköve 2021. március 29-én lesz. Ez az, amikor korlátozott OCP GTM-képességeket fog tapasztalni, és egyes mezők írásra válnak. Ha jelenleg együtt értékesít az OCP GTM megoldásaival, javasoljuk, hogy megoldásait a kereskedelmi piactérre miminálja, hogy kihasználja annak képességeit, és egyszerűsítse a közzétételi élményt. 

A kereskedelmi piactérre való Partnerközpont az értékesítések közzétételi folyamatának elsődleges célhelyét. A microsoftos termékekhez használt csatornákon és termékeken keresztül a megoldásokat a megosztott ügyfelekkel összekapcsolva tovább tudja növekedni vállalkozását. [További információ a kereskedelmi piactérről.](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)

### <a name="next-steps"></a>Következő lépések

- Ha még nem költözte át a megoldásait, kövesse az [](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) átváltási útmutató utasításait, vagy tekintse meg a részletes videó oktatóanyagot az összes migrálási tevékenység befejezéséhez és a megoldás(ok) kereskedelmi piactéren való közzétételének elkezdéséért. [](/azure/marketplace/co-sell-solution-migration)

- Az OCP GTM korlátozott képességeivel kapcsolatos kérdésekért tekintse meg a Microsoft kereskedelmi piactéren való közzétételre vonatkozó, közös értékesítésre [vonatkozó követelményeket](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf). (Lásd az "OCP GTM korlátozott képességei 2021. március 29-től kezdődően" című szakaszt.)

### <a name="questions"></a>Kérdése van?

Ha [kérdése](https://partner.microsoft.com/support/?stage=1) van, vagy további információra van szüksége, forduljon az ügyfélszolgálathoz.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Az új kereskedelmi élmény bővítése az Azure-Felhőszolgáltató (CSP) programjában Az Azure és Oroszország között

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-10
- Képességek

### <a name="impacted-audience"></a>Érintett célközönség

Minden orosz partner a Felhőszolgáltató (CSP) programon keresztül.

### <a name="details"></a>Részletek

2021. március 10-től izgatottan várjuk, hogy bejelentjük, hogy a CSP új kereskedelmi élménye elérhető az **Azure-ban Oroszországban.** Ez a felhasználói élmény leegyszerűsíti és javítja az ügyfelek Azure-szolgáltatások vásárlásának és használatának módját. Emellett konzisztens nézetet biztosít a CSP-program partnerei számára az Azure-díjszabásról az értékesítések között, usd-díjszabást a globális konzisztenciához, a számlázási dátumok igazításához, valamint hozzáférést a Azure Cost Management.

### <a name="next-steps"></a>Következő lépések

Számos forrás áll rendelkezésre, amelyek bemutatják az azure-beli kereskedelmi élményt és további információkat érhetők el. A CSP programfrissítések erőforrás-katalógusában megtalálja a legújabb gyakori kérdések, bemutatók, videók és [egyéb részleteket.](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Partnerközpont szoftverlicenc-kulcs használata és a fulfillment letöltése

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-04
- Képességek

### <a name="summary"></a>Összefoglalás

A Partnerközpont szoftverletöltési és -licenckulcs-teljesítési képességet visszaállította.

### <a name="impacted-audience"></a>Érintett célközönség

Minden Felhőszolgáltató (CSP) partner, amely folyamatos és kiszolgáló-előfizetési szoftverrendeléseket tranzakcióz a Partnerközpont

### <a name="details"></a>Részletek

A partneri visszajelzésekre válaszul visszaállítjuk a Partnerközpont fulfillment képességet a szoftver- és licenckulcsok beszerzésére a folyamatos és kiszolgálói előfizetési szoftverrendelések esetén. A rendszer a 2021. január 19-i eltávolítás előtt visszaállítja az előző állapotát. (Lásd a [bejelentést.)](2020-september.md#17)

Vegye figyelembe, hogy a szoftverlicenc-kulcsok és a letöltési hivatkozások értékesek és rendkívül hasznosak a szellemi tulajdont hasznos eszközökként. Ha kiszivárognak, gyorsan kimerülnek az aktiválási korlátaik, és negatív ügyfél- és partnerélményt okozhatnak.

### <a name="next-steps"></a>Következő lépések

Tekintse át a következő forrásokat a használati utasításokért és a szoftverkulcsok terjesztésével kapcsolatos fontos útmutatásért:

- [Helyszíni szoftverek eladása a CSP-programon keresztül](../csp-on-premise-software.md)
- [Partnerközpont kereskedelmi műveletek útmutatóját](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (lásd a szoftverkulcsok terjesztésével **kapcsolatos útmutatót).**

### <a name="questions"></a>Kérdése van?

Ha további kérdései vannak a közleményről, tekintse meg a kapcsolódó Yammer-közösségeket.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Az ügyletek mi áttelepítése a Partner Sales Connectből (PSC) egy Partnerközpont

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-04
- Képességek

### <a name="summary"></a>Összefoglalás

A Partner Sales Connect (PSC) 2021. március 31-től csak olvasási hozzáférésre lesz áttűnve, ezért azt kérjük, hogy kezdje meg az ügyletek PSC-ről Partnerközpont.

### <a name="impacted-audience"></a>Érintett célközönség

PSC-ügyleteket kötött partnerek

### <a name="details"></a>Részletek

A növekedés iránti közös elkötelezettségünk részeként a **Microsofttal** való közös értékesítéssel felfedezheti, biztosíthatja szakértelmét, és megnövelheti az ügyféligényét a pozitív ügyfél-eredmények érdekében.  Az átlagos üzlet a szokásosnál **3,5-szer** gyorsabb, így az Partnerközpont-ban történő közös értékesítési élmény kezelése lehetővé teszi az értékesítést a közvetlen ügyfél-, partner- és Microsoft-értékesítői csatornákon, és a teljes ajánló folyamatot egyetlen helyen kezelheti.

A **PSC** **2021. március 31-től** csak olvasási hozzáférésre fog áttűnni, ezért arra kérjük, hogy kezdje meg a Partnerközpont, és hozzáférjen a következő képességbeli fejlesztésekhez:  

- **Pontosabb útválasztást** nyújt a Microsofttal a megfelelő értékesítőnek a szükséges segítség típusa alapján.
- **Előzetes ajánlat jogosultságának** ellenőrzése az ösztönzőre jogosult megoldásokhoz és az ISV Connect program feltételeinek teljesítéséhez, leegyszerűsítve a jóváhagyási folyamatot és a végső igazolást (POE).
- **Zökkenőmentes felhasználói élmény** az összes közös értékesítési lehetőség és az értékesítési minősített érdeklődők egyetlen helyen való kezeléséhez.

Nemrég új funkciókkal bővült a Partnerközpont, hogy segítséget nyújtsunk az áthelyezéshez:

- [Tömeges műveletek az együttműködési lehetőségekhez](../bulk-operations.md)
- [Az ügylet migrálási funkciója](../psc-to-pc.md) (lásd a **PSC-ügyletek migrálási** szakaszát.)

A Partnerközpont értékesítési csapatai több ideje lesz arra, hogy az érdeklődők és lehetőségek árnyalása, az üzletek lezárása és a tartós ügyfélkapcsolatok létrehozása legyen a középpontban.

### <a name="next-steps"></a>Következő lépések

Az Partnerközpont [útmutató](../psc-to-pc.md) segítségével végigvezetheti az ügylet PSC-ről Partnerközpont.

### <a name="questions"></a>Kérdése van?

További kérdésekért forduljon a támogatási [szolgálathoz.](https://partner.microsoft.com/support/?stage=1)

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Új Microsoft Dynamics 365-termékek és -ajánlatok, amelyek 2021. április 1-én érhetők el

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-04
- Képességek

### <a name="summary"></a>Összefoglalás

2021. április 1-től a Microsoft számos új terméket és ajánlatot fog kínálni a Felhőszolgáltató (CSP) programhoz.

### <a name="impacted-audience"></a>Érintett célközönség

Az összes partner, aki a Felhőszolgáltató (CSP) programon keresztül megy keresztül

### <a name="details"></a>Részletek

2021. április 1-től a Microsoft a következő új termékeket és ajánlatokat bocsátja ki:

- Power BI Premium felhasználónként
- Customer Voice and Marketing USL geo- és szegmensbővítés

**Power BI Premium felhasználónként**

A Microsoft bemutatja az első felhasználónkénti Power BI Premium ajánlatát. Power BI Premium jelenleg csak kapacitási szerkezetben értékesítik. Power BI Premium felhasználónkénti hozzáférés a vállalati üzletiintelligencia- (BI-) és elemzési képességekhez. A rugalmas egyéni helylicencek kis- és középvállalatok számára is használhatók.

Az [ajánlatról Power BI tekintse](/power-platform-release-plan/2020wave2/power-bi/planned-features) át a következő kiadási részleteket: .


**Ajánlat részletei**

Vegye figyelembe, hogy az ajánlat neve kissé eltér az árlista előzetes kiadásának nevétől.

| Ajánlat neve | Ajánlat azonosítója |
| ------ |----------- |
| Power BI Premium felhasználónként | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium oktatók felhasználónkénti száma | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium felhasználónkénti diákoknak | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium (Nonprofit személyzet díjszabása) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium felhasználónkénti Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium felhasználónkénti Add-On oktatóknak | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium felhasználónkénti Add-On diákoknak | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium felhasználónkénti Add-On (nonprofit személyzet díjszabása) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Customer Voice and Marketing USL geo- és szegmensbővítés**

A 2020. decemberi bevezetés után a Dynamics 365 Customer Voice and Marketing USL-ajánlatok módosultak, hogy új országokat, valamint további nonprofit és oktatási termékkódokat adjanak hozzá.

| Ajánlat neve | Ajánlat azonosítója |
| ------ |----------- |
| Dynamics 365 Customer Voice USL (nonprofit személyzet díjszabása) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice USL oktatóknak | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Ezekről az ajánlatokról az alábbi oldalakon talál további információt:

- [A Dynamics 365 Customer Service Voice kezdőlapja](https://dynamics.microsoft.com/customer-voice/overview/)
- [A Dynamics 365 Marketing kezdőlapja](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Következő lépések

Tekintse át az ebben a témakörben található forrásokat, és ossza meg ezt az információt a szervezet megfelelő érdekelt felével.  

### <a name="questions"></a>Kérdése van?

Az ajánlatokkal kapcsolatos kérdésekért tekintse meg az érintett Yammer-közösségeket. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> A Microsoft Univerzális nyomtatás egyes csomagokban már elérhető

### <a name="categories"></a>Kategóriák

- Dátum: 2021-03-33
- Képességek

### <a name="summary"></a>Összefoglalás

A Microsoft Univerzális nyomtatás 2021. március 1-től elérhető lesz a tranzakciós lehetőségek Microsoft 365 csomagokban és önálló bővítményként.

### <a name="impacted-audience"></a>Érintett célközönség

Az összes partner, aki a Felhőszolgáltató (CSP) programon keresztül megy keresztül

### <a name="details"></a>Részletek

[Univerzális nyomtatás](https://aka.ms/universalprint) egy Microsoft 365 nyomtatószolgáltatás, amely megszünteti a helyszíni nyomtatókiszolgálók szükségét, és lehetővé teszi, hogy a Windows-eszközök Azure-ban regisztrált nyomtatókra nyomtattassanak. A tranzakció 2021. március 1-től lesz elérhető.

A dolgozóknak előnyére válik az illesztőprogram nélküli nyomtatás, a helyalapú nyomtatófelderítés, valamint az intuitív, tanuláshoz nem használható nyomtatási élmény. Az azure Azure Active Directory (Azure AD) szolgáltatáshoz csatlakozott eszközök a meglévő Azure AD-beli hitelesítő adatokat használják a biztonságos nyomtatáshoz. A rendszergazdák a nyomtatást a Azure Portal kezelhetik, és könnyedén csatlakoztathatják a natív támogatással Univerzális nyomtatás. Univerzális nyomtatás nem kompatibilis nyomtatókkal is telepíthetők Univerzális nyomtatás összekötője szoftverrel.

Univerzális nyomtatás a Windows E3, A3, E5 és A5 rendszerekre való indításkor, valamint az Microsoft 365 BP, F3, E3, A3, E5 és A5 rendszerekre.  

**Ajánlat részletei**

Vegye figyelembe, hogy az ajánlat neve kissé eltér az árlista előzetes kiadásának nevétől.

| Ajánlat neve | Ajánlat azonosítója | Anyagazonosító |
| ------ |----------- |----------- |  
| Univerzális nyomtatás bővítmény (500 feladat) – Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Univerzális nyomtatás mennyiségi bővítmény (500 feladat) oktatók számára – Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Univerzális nyomtatás bővítmény (500 feladat) – Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Univerzális nyomtatás bővítmény (500 feladat) oktatók számára – Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Következő lépések

Ismerkedjen meg az árlistával és a Univerzális nyomtatás [áttekintésével.](/universal-print/fundamentals/universal-print-whatis) Ossza meg ezt az információt a szervezet összes megfelelő kapcsolattartóval.

### <a name="questions"></a>Kérdése van?

Ha kérdései vannak ezekkel az ajánlatokkal kapcsolatban, tekintse meg az érintett Yammer-közösségeket.
