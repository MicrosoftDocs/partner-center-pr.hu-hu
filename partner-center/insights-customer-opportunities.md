---
title: Partnerközpont Elemzések – CloudAscent Propensity-jelentések
description: További információ a CloudAscent propensity jelentésekről a Partnerközpont. Információkat tartalmaz arról, hogy az ügyfél hogyan nem tud Microsoft-termékeket vásárolni.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 6916d44e3f028fbfd788d3bee54671dbadd874d1
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376810"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Az irányítópulton elérhető CloudAscent propensity Partnerközpont jelentéseket

**Megfelelő szerepkörök:** Vezetői jelentésmegjelenítő | Jelentésmegjelenítő

A Partnerközpont irányítópult letölthető propenitási adatokat biztosít a CloudAscent programból. Az adatok azt mutatják, hogy az ügyfelek milyen valószínűséggel vásárolhatnak Microsoft-termékeket.  Ez a cikk az adatok lebontását, a pontozás használatát és azt ismerteti, hogy mit jelent.

## <a name="summary-definitions"></a>Összefoglaló definíciók

- **SMC-ügyfelek**– Ez a propensitásletöltésben található ügyfelek teljes száma.  Az ügyfeleket a rekordpartner azonosítja.
- **Szerződések lejárata**– Az aktuális pénzügyi évben meg kell adtunk a lejáró szerződések számát.
- Open Expiring Revenue (Nyitott **lejáró bevétel)**– A nyitott lejáró szerződésekhez kapcsolódó bevétel.

:::image type="content" source="images/insights/customer-opportunity-1.png" alt-text="Képernyőkép az Ügyfelek lehetőségek összegzése irányítópultról.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB-szegmentálás

A kis- és középvállalati (SMB) szegmens három különálló alszegmensre oszlik.

1. **A leggyakoribb nem nem használt ügyfelek** közé tartozik a legnagyobb SMB-ügyfelek, akik a legtöbb lehetőséget kínálják a Microsoft számára. A tipikus nem felügyelt ügyfelek hasonló jellemzőkkel rendelkeznek, mint a felügyelt fiókok, sok alkalmazottal, nagy mennyiségű it-költségvetéssel és kiadással, valamint nagy mennyiségű potenciális bevétellel a Microsoft számára.

   A Nem felső szintű nem hatót kétféleképpen definiáljuk:

   - **A legkorrektebb** felhasználóalapú – 300 vagy több alkalmazottal rendelkező fiókokat tartalmaz. User-Based fiókok kiváló célok az első vásárláshoz vagy a felhasználóalapú előfizetési termékek, például a Microsoft 365, a Dynamics 365 vagy a Surface bővítéséhez.
   - **Top Unmanaged Compute Based** –, amely 10 ezer dollárnál nagyobb Azure-beli potenciális fiókokat tartalmaz. A számítási alapú fiókok tartalmazzák a meglévő Azure-t. a jelentős jövő évi potenciális fiókokkal és olyan fiókokkal, amelyek még nem vásárolják meg az Azure-t, de 10 ezer dollárnál nagyobbak az Azure-ra vonatkozó lehetőségeik.

2. **A Medium Business** a meglévő ügyfeleket és a 25–300 alkalmazottal rendelkező potenciális ügyfeleket tartalmazza.

3. **A kisvállalatok** 10–25 alkalmazottal dolgozó vállalkozásokat foglalnak magába.

4. **A Nagyon kisvállalatok** 1–9 alkalmazottal dolgozó vállalkozásokat foglalnak magába.

:::image type="content" source="images/insights/customer-opportunity-2.png" alt-text="Ügyfél SMC-típus szerint.":::

**A nem és**  a közepes üzleti alszegetmények a Microsoft és a Microsoft partnerei számára jelentős élettartamú (LTV) ügyfeleket képviselnek. Emiatt ezek a szegmensek a növekedést hajtó fő területek. Ebben a két alszegegben jobb helyzetben vagyunk, hogy a szoftvercsatornát az Microsoft 365-val szerezjük be, további bevételt szerezünk a D365/Azure üzletági (LOB) alkalmazásokkal, és magas LTV-t szeretnénk megvalósítani a Microsoft számára.

Jelenleg két fő lehetőségünk van: 1. az ügyfél növekedést ad hozzá; 2. míg a felhőbeli szoftvercsatornákat jól Microsoft 365, a Dynamics 365-ben és az Azure-ban nagy lehetőségünk van.

Az alábbi képernyőkép a négy SMB-alszegmentet ábrázolja. A CloudAscent rangsorolnia kell az összes legfontosabb nem nem és közepes üzleti fiók profilkészítését, pontozását és modellezését.

:::image type="content" source="images/insights/customer-opportunity-3.png" alt-text="Az SMB-alszegmentek képernyőképe.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

Az SMB gépi tanulási technológiával használja az értékesítési és marketing ügyfél-előrejelzéseket a nem használt és közepes üzleti szegmensben. Hogyan gyűjti és váltja fel a jeleket a propensitásra vonatkozó javaslatokké?

- **Adatgyűjtés:** A webbejárási webbejárások több milliárd ügyféljelet vizsgálnak és gyűjtenek a vállalati tartományok pingelése, a blogbejegyzések figyelése, a kiadások, a közösségi streamek és a technikai fórumok segítségével.  Az összegyűjtött jelek mellett a firmographics információkat belső és külső forrásokból is gyűjti a rendszer, például a D&B, a Microsoft belső előfizetési és tranzakciós adataiból.

- **Machine Learning:** A jelek be vannak állítva a gépi tanulási modellbe, amely az értékesítési és marketing-előrejelzések strukturált adatkészletét adja ki minden ügyfél számára felhőalapú termék és fürt alapján.  Minden ügyfél pontozása a Microsoft legfelső szintű SMB-hez hasonló modellel van pontozással, amely meghatározza az ügyfél illeszkedési algoritmusát, valamint az ügyfél online viselkedését integráló gépi tanulási algoritmusokat szándékként definiálja. A pontozás olyan fürtökbe van egyesülve, amelyek megmutatják, hogy az ügyfél nem hajlandó Microsoft Cloud-termékeket vásárolni.

- **Optimalizálás:** A Machine Learning rendszer optimalizálja a modelleket a tranzakciós adatok havi és az előfizetési adatok negyedévente való fogyasztásával.  A nyerés/veszteség adatok használatával a Machine Learning beállítja az algoritmusokat, és ellenőrzi, hogy a modellek a várt módon működnek-e a fürtre vonatkozó javaslatok és az MSX-hez használt lehetőségek összehasonlításával.

:::image type="content" source="images/insights/customer-opportunity-4.png" alt-text="Képernyőkép az SMB gépi tanulásról.":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

Hogyan jön létre a propensitási javaslatok létrehozása?

A webes webbejárási eszközök és a különböző forrásokból származó adatok alapján gyűjtött jelek használatával konszolidáljuk a céges adatokat és az ügyfél közösségimédia-jeleit.  A pontozás ezeket a jeleket és adatokat használja összehasonlítási modellekben a szándékok illesztési és pontozási modelljeihez.

1. Ügyfélfiók illeszkedés

   - Belső és külső adatpontok, amelyek a céges adatokat határozzák meg.

   - A pontozás a legjobb SMB-hez hasonló modellt használ az ügyfelek összehasonlítására, és annak összehasonlítása érdekében, hogy azok megfelelőek-e a Microsoft Cloud-termékekhez.

   - A illeszkedés pontozása negyedévente frissül

2. Ügyfélfiók szándéka

   - A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot.

   - A szándékpontozás felül illeszkedik a fürtök meghatározásához.

   - A szándékpontozás havonta frissül.

   :::image type="content" source="images/insights/customer-opportunity-5.png" alt-text="CloudAscent SMB prediktív modellek.":::

3. Fürtözés

   Az illeszkedés és a szándék jelzése egy fürtözési pontszámba van összevonva. A CloudAscent négy fürtből rendelkezik:

      - Act Now – értékesítésre kész ügyfelek
      - Értékelés – marketingre kész ügyfelek
      - Figyelemfelkeltő kampányok
      - Oktatás – a szándék oktatása és figyelése

   A fürtözés lehetővé teszi, hogy a felhasználók adott ügyfeleket célozzanak meg értékesítési és marketinges kezdeményezésekhez olyan szegmenstényezők alapján, mint például a termék, a földrajzi hely, az iparág és a vertikális.

   A CloudAscent-munkafüzetek **Propensity Model (Propensity-modell)** lapja a propensitást és a becsült térbeli bevételt osztja meg. Az illeszkedés és a szándék fürtözésének meghatározásához a következő lépéseket kell végigmenni:

      1. A ML modellek használatával először 100-as skálán számítjuk ki a Customer Fit Score (Ügyfél illesztési pontszáma) és a intent Score (szándék pontszáma) értékeket.  A pontos pontszámok a modelltől függően ML változhatnak.  Példa pontszámok alább:

         |**Osztályozás**|**Pontszám**|
         |---------|:---------|
         |Magas|75 - 100|
         |Közepes|55 - 74|
         |Alacsony|30 - 54|
         |Nagyon alacsony|0 - 29|

      2. A fenti szabályt használva a vállalatokat magas, közepes, alacsony és nagyon alacsony besorolásúként soroljuk be mind az Ügyfél illeszkedési, mind a Szándékjelzők esetében.

      3. Az ügyfelek illeszkedési és szándékjeleit egy 2D-s mátrixon ábrázoljuk, és az egyes metszetek a szándékot jelképezik. Például: Magas illeszkedés + Magas szándék = A1, amely a legnagyobb propensitást képviseli.

      4. Végül ezek a szegmensek csoportosítva alkotnak fürtöt.  Például az A1, A2, A3, A4 az Act Now fürtöt alkotják.

         :::image type="content" source="images/insights/customer-opportunity-6.png" alt-text="CloudAscent-modellek.":::

   Javasoljuk, hogy ezeknél az ügyfeleknél az Act Now (Most járjon el) és a Evaluate customers (Ügyfelek kiértékelése) célcsoportot célozza meg.

## <a name="cloudascent-products--models"></a>CloudAscent-termékek & modellek

Az alábbi ábra a CloudAscent szolgáltatáson belüli egyes támogatói modelleket tartalmazza:

:::image type="content" source="images/insights/customer-opportunity-7.png" alt-text="CloudAscent propensity modell.":::

A téreltérmodellek olyan meglévő Microsoft-ügyfelek előrejelzései, akik nem tartalmaznak terméket, és/vagy nettó új potenciális ügyfelek.

Az upsell modellek tranzakciós adatok használatával jelezik előre az Azure-beli és a Microsoft 365 potenciálisan várható szolgáltatásokat.

Ezek az ügyfelek már az Azure-ral vagy a Microsoft 365 is rendelkezik, és az upsell modell azt mutatja, hogy valószínűleg többet fognak vásárolni a meglévő termékváltozatukból.

Az EOS a Win 7, Office 2010, SQL Server és Windows ügyfeleket is megosztja. Az EOS-adatokat a rendszer lekérte az MS Sales szolgáltatásból, és átfedi őket a CloudAscent propensity modellel, ha elérhető. Az EOS-adatok a Modern Workben és az Azure Salesben játszódnak.
