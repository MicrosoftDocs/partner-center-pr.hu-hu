---
title: Partneri központ – CloudAscent-feljelentési jelentések
description: Ismerje meg a CloudAscent-felkészítési jelentéseket a partner Centerben. Az ügyfél által a Microsoft-termékek megvásárlására való hajlamával kapcsolatos információkat tartalmaz.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: fd017884c29df3874a06e8c4213c6fe5f05a8995
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530577"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>A CloudAscent-jelentések elérhetők a partner Center irányítópultján

**Megfelelő szerepkörök**
- Executive Report Viewer
- Jelentés megjelenítője

A partneri központ irányítópultja a CloudAscent programból letölthető, a rendelkezésre bocsátó adatokra vonatkozó adatait biztosítja. Az adatkezelési szolgáltatás a Microsoft-termékek vásárlásához szükséges ügyfeleket jeleníti meg.  Ez a cikk ismerteti az adatbontást, a pontozás használatát, valamint azt, hogy mit jelent.

## <a name="summary-definitions"></a>Összefoglaló definíciók

- **SMC-ügyfelek** – ez az ügyfelek teljes száma a felszállási letöltésekben.  Az ügyfeleket a Record partner azonosítja.
- **Lejárati szerződések** – az aktuális pénzügyi évben a lejáró szerződések számát biztosítjuk.
- **Lejáró bevétel** – a lejáró szerződésekhez kapcsolódó bevétel.
- **Nyissa meg a lejáró bevételt** – a nyitott lejáró szerződésekhez kapcsolódó bevételt.

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Képernyőkép az ügyfelek lehetőségeinek összefoglaló irányítópultról.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB-szegmentálás

A kis-és közepes méretű üzleti (SMB) szegmensek további három különálló alszegmensre oszlanak.

1. A legtöbbet nem **felügyelt** legfontosabb SMB-ügyfelek a Microsoft legnagyobb lehetőségével rendelkeznek. A legnépszerűbb nem felügyelt ügyfelek a felügyelt fiókokhoz hasonló jellemzőkkel rendelkeznek, nagyszámú alkalmazottal, nagy informatikai költségvetéssel és költve, valamint nagy mennyiségű lehetséges bevétel a Microsoft számára.

   A legfelső szintű felügyelet nélküli két módszert definiáljuk:

   - **Leggyakoribb nem felügyelt felhasználó** – a 300 vagy több alkalmazottat tartalmazó fiókokat tartalmaz. A User-Based-fiókok kiváló célokat szolgálnak az első vásárláshoz, vagy a felhasználó-alapú előfizetési termékek, például a M365, a D365 vagy a Surface bővítéséhez.
   - **Top nem felügyelt számítási alapú** – a $10k-nál nagyobb Azure-potenciállal rendelkező fiókokat tartalmaz. A számítási alapú fiókok közé tartozik a meglévő Azure. a jövőbeli éves potenciállal rendelkező fiókok és az Azure-t még nem megvásárló fiókok, de a $10k-nál nagyobb kapacitással rendelkeznek.

2. A **Medium Business** a meglévő ügyfeleket és a 25 – 300 alkalmazottat foglalkoztató fiókokat tartalmaz.

3. A **kisvállalkozások több** mint 25 alkalmazottal rendelkező fennmaradó vállalatot foglalnak magukban.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Képernyőkép az ügyfelek lehetőségeinek összefoglaló irányítópultról.":::

A nem **felügyelt** és **közepes méretű üzleti** Alszegmensek magas élettartamú (LTV) ügyfeleket képviselnek a Microsoft és a Microsoft partnerei számára. Ezért ezek a szegmensek a növekedésre összpontosítanak. Ebben a két alszegmensben jobb helyzetben vagyunk a szoftvercsatorna beolvasásához a M365, a D365/Azure üzletági (LOB) alkalmazásokkal folytatott további bevételekhez, valamint a Microsoft magas LTV megvalósításához.

Napjainkban a lehetőség két kulcsfontosságú területtel rendelkezik – 1. ügyfelünk bővíti a növekedést; 2. Habár a M365-hez vezető felhőalapú szoftvercsatornák beszerzése nagy lehetőséget biztosítunk a D365 és az Azure-ban.

A következő képernyőkép a három SMB-alszegmenst és a piacra optimalizált útvonalakat mutatja. A CloudAscent rangsorolja az összes nem felügyelt és közepes üzleti fiók profilkészítését, pontozását és modellezését.

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Képernyőkép az ügyfelek lehetőségeinek összefoglaló irányítópultról.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

Az SMB gépi tanulási technológiát használ a legfelső szintű nem felügyelt és közepes üzleti szegmensen belüli értékesítési és marketing-ügyfelek előrejelzéséhez. Hogyan történik a jelek begyűjtése és a szolgáltatásokra vonatkozó javaslatok bekapcsolása?

- **Adatgyűjtés** : a webes beolvasók több milliárd ügyfél-jelet vizsgálnak és gyűjtenek a vállalati tartományok pingelésével és a figyeléssel: blogbejegyzések, sajtóközlemények, közösségi streamek és technikai fórumok.  Az összegyűjtött jeleken kívül a firmographics információkat a belső és külső forrásokból is gyűjtjük, például a D&B, a Microsoft belső előfizetése és a tranzakciós adatok.

- **Machine learning** : a rendszer a jeleket a gépi tanulási modellbe helyezi, amely strukturált adatkészletet hoz létre az értékesítések és a marketing-előrejelzések alapján minden ügyfél számára a felhőalapú termék és a fürt számára.  Minden ügyfél egy, a Microsoft legfontosabb SMB-modelljét használja, amely meghatározza az ügyfél illeszkedését, valamint a gépi tanulási algoritmusokat, amelyek az ügyfél online viselkedését a szándék szerint határozzák meg. A pontozás olyan fürtökbe van egyesítve, amelyekben az ügyfél a Microsoft Cloud termékek megvásárlására való hajlamot jeleníti meg.

- **Optimalizálás** : a Machine Learningrendszer optimalizálja a modelleket úgy, hogy a tranzakciós adatokat havonta és az előfizetési adatokat negyedévente felhasználva.  A nyerési/adatvesztési művelettel a Machine Learning módosítja az algoritmusokat, és ellenőrzi, hogy a modellek a várt módon működnek-e a fürt ajánlásainak összehasonlításával a MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Képernyőkép az ügyfelek lehetőségeinek összefoglaló irányítópultról.":::

## <a name="cloudascent-propensity"></a>CloudAscent-hajlam

Hogyan jönnek létre a megfogalmazási javaslatok?

A webes bejárásokkal és a különböző forrásokból származó adatokkal gyűjtött jelek használatával konszolidáljuk a firmographics-adatokat és az ügyfél közösségi médiájának jelzéseit.  A pontozás ezeket a jeleket és az adatelemzési modelleket használja az illesztési és pontozási modellekhez.

1. Ügyfél-fiókhoz igazítás

   - A firmographics definiáló belső és külső adatpontok.

   - Az illeszkedő pontozás a legjobb SMB modell használatával hasonlítja össze az ügyfeleket, és megtudhatja, hogy lehetséges-e a Microsoft Cloud termékekhez való illeszkedés.

   - Az illesztési pontozás negyedévente frissül

2. Vevői fiók leképezése

   - A közösségi médiával és az ügyfél online viselkedésével kapcsolatos jelek határozzák meg a szándékot.

   - A leképezési pontozás a fürtök definiálására alkalmas.

   - A szándékok pontozása havonta frissül.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Képernyőkép az ügyfelek lehetőségeinek összefoglaló irányítópultról.":::

3. Fürtözés

   A megfelelő és a szándékú jelek összevonása egy fürtözési pontszámba történik. A CloudAscent négy fürttel rendelkezik:

      - Azonnali működés – értékesítésre kész ügyfelek
      - Kiértékelés – marketing-Ready ügyfelek
      - Ápolás – a tudatosságnövelő kampányok
      - Nevelés – képzés és monitorozás a szándékkal

   A fürtözés lehetővé teszi a felhasználók számára, hogy meghatározott ügyfeleket célozzanak értékesítési és marketing kezdeményezésekhez szegmens tényezők alapján, például: termék, Geo, iparág és vertikális.

   A CloudAscent-munkafüzetek megosztó **modell** lapja megosztja a hajlamot és a becsült szóköz bevételt. A Fit és a szándék fürtözésének definiálásához végezze el a következő lépéseket:

      1. A ML-modellek használatával először a 100-es skálán számítjuk ki az ügyfél-igazítási pontszámot és a szándék pontszámát.  A pontos pontszámok ML modellek alapján változnak.  Példa az alábbi pontszámokra:

         |**Besorolás**|**Pontszám**|
         |---------|:---------|
         |Magas|75 – 100|
         |Közepes|55 – 74|
         |Alacsony|30 - 54|
         |Nagyon alacsony|0 - 29|

      2. A fenti szabály használatával a vállalatokat magas, közepes, alacsony és nagyon alacsony értékre osztályozjuk mind az ügyfél, mind a szándékos jelzések esetében.

      3. Az ügyfél-igazítási és szándéki jeleket egy 2D-mátrixban ábrázoljuk, amely a hajlamot jelképező minden metszettel rendelkezik.     Például: nagy teljesítményű + magas szándékú = a1, amely a legmagasabb szintű hajlamot jelöli.

      4. Végül ezek a szegmensek csoportosítva alkotják a fürtöket.  Például: a1, a2, a3, a4, a jogszabály most fürt.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Képernyőkép az ügyfelek lehetőségeinek összefoglaló irányítópultról.":::

   Ezen ügyfelek esetében javasoljuk, hogy most célozza meg a célzást, és értékelje az ügyfeleket.

## <a name="cloudascent-products--models"></a>CloudAscent-termékek & modellek

A következő ábra az egyes CloudAscent-modellekre vonatkozó nézeteket tartalmazza:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Képernyőkép az ügyfelek lehetőségeinek összefoglaló irányítópultról.":::

A szóközökből álló modellek olyan meglévő Microsoft-ügyfelek számára készült előrejelzésekből állnak, amelyek nem rendelkeznek termékkel és/vagy a nettó új potenciális ügyfelekkel.

A upsell-modellek a tranzakciós adataival jósolják meg az Azure-ban és az M365-ban felhasználható upsell-t.

Az EOS a Win 7, az Office 2010, a SQL Server és a Windows Server rendszerű ügyfeleket is megosztja a szolgáltatással. Az EOS-adatok az MS Sales szolgáltatásból vannak leküldve, és az CloudAscent-modellezési modellezéssel, ahol elérhető. Az EOS-adatforgalom a modern és az Azure Sales szolgáltatásban is működik.
