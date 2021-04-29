---
title: Partnerközpont Insights – CloudAscent Propensity-jelentések
description: További információ a CloudAscent propensity jelentésekről a Partnerközpont. Arra vonatkozó információkat tartalmaz, hogy az ügyfelek hogyan nem vásárolhatnak Microsoft-termékeket.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 91f64faeec0b97be2797d489e152cb84cbb2e192
ms.sourcegitcommit: 8bd2e2f2f0f6bcd0fa202787df5b3c1f786f88f9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/29/2021
ms.locfileid: "108213446"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Az irányítópulton elérhető CloudAscent propensity Partnerközpont jelentéseket

**Megfelelő szerepkörök**

- Vezetői jelentésmegjelenítő
- Jelentésmegjelenítő

A Partnerközpont irányítópult letölthető propenitási adatokat biztosít a CloudAscent programból. Az adatok azt mutatják, hogy az ügyfelek milyen valószínűséggel vásárolhatnak Microsoft-termékeket.  Ez a cikk az adatok lebontását, a pontozás használatát és azt ismerteti, hogy mit jelent.

## <a name="summary-definitions"></a>Összegzési definíciók

- **SMC-ügyfelek**– Ez a propensitásletöltésben található ügyfelek teljes száma.  Az ügyfeleket a rekordpartner azonosítja.
- **Szerződések lejárata**– Az aktuális pénzügyi évben meg kell adtunk a lejáró szerződések számát.
- Open Expiring Revenue (Nyitott **lejáró bevétel)**– A nyitott lejáró szerződésekhez társított bevétel.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Képernyőkép az Ügyfelek lehetőségek összegzése irányítópultról.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB-szegmentálás

A kis- és középvállalati (SMB) szegmens három különálló alszegmensre oszlik.

1. **A leggyakoribb nem nem használt szolgáltatás a** Legnagyobb SMB-ügyfeleket tartalmazza, akik a legtöbb lehetőséget kínálják a Microsoft számára. A tipikus nem felügyelt ügyfelek hasonló jellemzőkkel rendelkeznek, mint a felügyelt fiókok, sok alkalmazottal, nagy it-költségkeretekkel és kiadásokkal, valamint nagy mennyiségű potenciális bevétellel a Microsoft számára.

   A nem nem felső szintűeket kétféleképpen definiáljuk:

   - **Top Unmanaged User Based**–, 300 vagy több alkalmazottal rendelkező fiókokat tartalmaz. User-Based fiókok kiváló célok az első alkalommal való vásárláshoz, illetve a felhasználóalapú előfizetési termékek (például a Microsoft 365, a Dynamics 365 vagy a Surface) bővítéséhez.
   - **Top Unmanaged Compute Based** ( Top Unmanaged Compute Based – Olyan fiókokat tartalmaz, amelyek azure-beli potenciálisan nagyobbak 10 ezer dollárnál). A számítási alapú fiókok tartalmazzák a meglévő Azure-t. a jelentős jövő évi potenciális fiókokkal és olyan fiókokkal, amelyek még nem vásárolják meg az Azure-t, de az Azure-ra több mint 10 ezer usd-t is el lehet látni.

2. **A Medium Business** a meglévő ügyfeleket és a 25–300 alkalmazottal rendelkező potenciális ügyfeleket tartalmazza.

3. **A kisvállalatok** 10–25 alkalmazottal dolgozó vállalkozásokat foglalnak magába.

4. **A Nagyon kisvállalatok** közé tartoznak az 1–9 alkalmazottal dolgozó üzletek.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Ügyfél SMC-típus szerint.":::

**A nem és a közepes** üzleti alkategóriák a Microsoft és a Microsoft partnerei számára jelentős élettartamú (LTV) ügyfeleket képviselnek.  Emiatt ezek a területek a növekedés fő területei ebben a szegmensben. Ebben a két alszegben jobb helyzetben vagyunk a szoftvercsatornák Microsoft 365-val való megszerzéséhez, a D365/Azure üzletági (LOB) alkalmazásokból való további bevételhez, és a Microsoft magas LTV-használatának szerzéséhez.

Jelenleg két fő lehetőségünk van: 1. az ügyfél növekedést ad hozzá; 2. míg a felhőbeli szoftvercsatornákat jól Microsoft 365, a Dynamics 365-ben és az Azure-ban nagy lehetőségünk van.

Az alábbi képernyőkép a négy SMB-alszegmentet ábrázolja. A CloudAscent rangsorolnia kell az összes legfontosabb nem nem és közepes üzleti fiók profilkészítését, pontozását és modellezését.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Az SMB-alszegmentek képernyőképe.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

Az SMB gépi tanulási technológiával használja az értékesítési és marketing ügyfél-előrejelzéseket a nem használt és közepes üzleti szegmensben. Hogyan gyűjti és váltja fel a jeleket a propensitási javaslatokké?

- **Adatgyűjtés:** A webbejárási webbejárások több milliárd ügyféljelet vizsgálnak és gyűjtenek a vállalati tartományok pingelése, a blogbejegyzések figyelése, a kiadások, a közösségi streamek és a technikai fórumok segítségével.  Az összegyűjtött jelek mellett a céges adatok olyan belső és külső forrásokból is gyűjtenek adatokat, mint a D&B, a Microsoft belső előfizetési és tranzakciós adatai.

- **Machine Learning:** A jelek be vannak állítva a gépi tanulási modellbe, amely az egyes ügyfelekre vonatkozó értékesítési és marketing-előrejelzések strukturált adatkészletét adja vissza a felhőalapú termékek és fürtök alapján.  Minden ügyfél pontozása a Microsoft legfelső SMB-hez hasonló, az ügyfél illeszkedést meghatározó modelljével, az ügyfél online viselkedését integráló gépi tanulási algoritmusokkal pedig szándékként van meghatározva. A pontozás olyan fürtökbe van egyesülve, amelyek megmutatják, hogy az ügyfél nem hajlandó Microsoft Cloud-termékeket vásárolni.

- **Optimalizálás:** A Machine Learning optimalizálja a modelleket a tranzakciós adatok havi és az előfizetési adatok negyedévente való fogyasztásával.  A nyerés/veszteség adatok használatával a Machine Learning beállítja az algoritmusokat, és ellenőrzi, hogy a modellek a várt módon működnek-e, összehasonlítva a fürtre vonatkozó javaslatokat az MSX-hez használt lehetőségekkel.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Képernyőkép az SMB gépi tanulásról.":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

Hogyan jön létre a propensitási javaslatok létrehozása?

A webes webbejárási eszközök és a különböző forrásokból származó adatok alapján gyűjtött jelek használatával konszolidáljuk a céges adatokat és az ügyfél közösségimédia-jeleit.  A pontozás ezeket a jeleket és adatokat használja összehasonlítási modellekben a szándékok illesztési és pontozási modelljeihez.

1. Ügyfélfiók illeszkedés

   - Belső és külső adatpontok, amelyek a céges adatokat határozzák meg.

   - A illeszkedés pontozása a legjobb SMB-modellhez hasonlóan hasonlítja össze az ügyfeleket, és megnézi, hogy megfelelőek-e a Microsoft Cloud-termékekhez.

   - A illeszkedés pontozása negyedévente frissül

2. Ügyfélfiók szándéka

   - A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot.

   - A szándékpontozás felül megfelel a fürtök meghatározásának.

   - A szándékpontozás havonta frissül.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB prediktív modellek.":::

3. Fürtözés

   Az illesztési és szándékra vonatkozó jelek egy fürtözési pontszámban vannak összesíteni. A CloudAscent négy fürtből rendelkezik:

      - Act Now – értékesítésre kész ügyfelek
      - Értékelés – marketingre kész ügyfelek
      - Figyelemfelkeltő kampányok
      - Oktatás – szándék oktatása és figyelése

   A fürtözés lehetővé teszi, hogy a felhasználók adott ügyfeleket célozzanak meg értékesítési és marketinges kezdeményezésekhez olyan szegmenstényezők alapján, mint például a termék, a földrajzi hely, az iparág és a vertikális.

   A CloudAscent-munkafüzetek **Propensity Model (Propensity-modell)** lapja a propensitást és a becsült térbeli bevételt osztja meg. Az illeszkedés és a szándék fürtözésének meghatározásához a következő lépéseket kell végigmenni:

      1. Ml-modellek használatával először kiszámítjuk a Customer Fit Score (Ügyfél illesztési pontszáma) és a Intent Score (szándék pontszáma) értékeket egy 100-as skálán.  A pontos pontszámok az ML-modellektől függően változnak.  Példa pontszámok alább:

         |**Osztályozás**|**Pontszám**|
         |---------|:---------|
         |Magas|75 - 100|
         |Közepes|55 - 74|
         |Alacsony|30 - 54|
         |Nagyon alacsony|0 - 29|

      2. A fenti szabályt használva a vállalatokat magas, közepes, alacsony és nagyon alacsony besorolásúként osztályozjuk mind az ügyfél illeszkedési, mind a szándékjel alapján.

      3. Az ügyfelek illeszkedési és szándékjeleit egy 2D-s mátrixon ábrázoljuk, és minden metszet a nem megfelelőséget jelképez. Például: Magas illeszkedés + Magas szándék = A1, amely a legnagyobb propensitást képviseli.

      4. Végül ezek a szegmensek csoportosítva alkotnak fürtöt.  Például az A1, A2, A3, A4 az Act Now fürtöt alkotják.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent-modellek.":::

   Javasoljuk, hogy ezeknél az ügyfeleknél az Act Now (Most járjon el) és a Evaluate customers (Ügyfelek kiértékelése) célcsoportot célozza meg.

## <a name="cloudascent-products--models"></a>CloudAscent-termékek & modellek

Az alábbi ábra a CloudAscent szolgáltatáson belüli egyes támogatói modelleket tartalmazza:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent propensity modell.":::

A téreltérmodellek olyan meglévő Microsoft-ügyfelek előrejelzései, akik nem tartalmaznak terméket, és/vagy nettó új potenciális ügyfelek.

Az upsell modellek tranzakciós adatokkal jelezik előre az Azure-beli és a Microsoft 365 potenciális lehetőségeit.

Ezek az ügyfelek már most is az Azure-ral vagy a Microsoft 365, és az upsell modell azt mutatja, hogy valószínűleg többet fognak vásárolni a meglévő termékváltozatukból.

Az EOS a Win 7, az Office 2010, a SQL Server és a Windows Server esetében megosztja a szolgáltatásvégi (EOS) ügyfeleket. Az EOS-adatokat a rendszer lekérte az MS Sales szolgáltatásból, és átfedi őket a CloudAscent propensity modellel, ha elérhető. Az EOS-adatok a Modern Workben és az Azure Salesben játszódnak.
