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
ms.openlocfilehash: 2cdb63c8f7e29fc8a56e920b587e47c382c6eacb
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086957"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>A CloudAscent-jelentések elérhetők a partner Center irányítópultján

**Megfelelő szerepkörök**

- Executive Report Viewer
- Jelentés megjelenítője

A partneri központ irányítópultja a CloudAscent programból letölthető, a rendelkezésre bocsátó adatokra vonatkozó adatait biztosítja. Az adatkezelési szolgáltatás a Microsoft-termékek vásárlásához szükséges ügyfeleket jeleníti meg.  Ez a cikk ismerteti az adatbontást, a pontozás használatát és azt, hogy mit jelent.

## <a name="summary-definitions"></a>Összefoglaló definíciók

- **SMC-ügyfelek**– ez az ügyfelek teljes száma a felszállási letöltésekben.  Az ügyfeleket a Record partner azonosítja.
- **Lejárati szerződések**– az aktuális pénzügyi évben a lejáró szerződések számát biztosítjuk.
- **Lejáró bevétel**– a lejáró szerződésekhez kapcsolódó bevétel.
- **Nyissa meg a lejáró bevételt**– a nyitott lejáró szerződésekhez kapcsolódó bevételt.

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Képernyőkép az ügyfelek lehetőségeinek összefoglaló irányítópultról.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB-szegmentálás

A kis-és közepes méretű üzleti (SMB) szegmensek további három különálló alszegmensre oszlanak.

1. A legtöbbet nem **felügyelt** legfontosabb SMB-ügyfelek a Microsoft legnagyobb lehetőségével rendelkeznek. A legnépszerűbb nem felügyelt ügyfelek a felügyelt fiókokhoz hasonló jellemzőkkel rendelkeznek, nagyszámú alkalmazottal, nagy informatikai költségvetéssel és költve, valamint nagy mennyiségű lehetséges bevétel a Microsoft számára.

   A legfelső szintű felügyelet nélküli két módszert definiáljuk:

   - **Leggyakoribb nem felügyelt felhasználó**– a 300 vagy több alkalmazottat tartalmazó fiókokat tartalmaz. A User-Based-fiókok kiváló célokat szolgálnak az első vagy a felhasználó-alapú előfizetési termékek, például a Microsoft 365, a Dynamics 365 vagy a Surface kibővítéséhez.
   - **Top nem felügyelt számítási alapú** – a $10k-nál nagyobb Azure-potenciállal rendelkező fiókokat tartalmaz. A számítási alapú fiókok közé tartozik a meglévő Azure. a jövőbeli éves potenciállal rendelkező fiókok és az Azure-t még nem megvásárló fiókok, de a $10k-nál nagyobb kapacitással rendelkeznek.

2. A **Medium Business** a meglévő ügyfeleket és a 25 – 300 alkalmazottat foglalkoztató fiókokat tartalmaz.

3. A **kisvállalkozások több** mint 25 alkalmazottal rendelkező fennmaradó vállalatot foglalnak magukban.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Ügyfél által SMC-típus.":::

A nem **felügyelt** és **közepes méretű üzleti** Alszegmensek magas élettartamú (LTV) ügyfeleket képviselnek a Microsoft és a Microsoft partnerei számára. Emiatt ezek a szegmensek a növekedéshez való összpontosítása. Ebben a két alszegmensben jobb helyzetben vagyunk, hogy beszerezzük a szoftvercsatornát Microsoft 365okkal, a D365/Azure üzletági (LOB) alkalmazások további bevételeit, és magas LTV a Microsoft számára.

Napjainkban a lehetőség két kulcsfontosságú területtel rendelkezik – 1. ügyfelünk bővíti a növekedést; 2. a D365 és az Azure-ban nagy lehetőségünk van arra, hogy jól beszerezzük a Microsoft 365hoz vezető felhőalapú szoftvercsatornát.

A következő képernyőkép a három SMB-alszegmenst és a piacra optimalizált útvonalakat mutatja. A CloudAscent rangsorolja az összes nem felügyelt és közepes üzleti fiók profilkészítését, pontozását és modellezését.

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Képernyőkép az SMB-alszegmensekről.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

Az SMB gépi tanulási technológiát használ a legfelső szintű nem felügyelt és közepes üzleti szegmensen belüli értékesítési és marketing-ügyfelek előrejelzéséhez. Hogyan történik a jelek begyűjtése és a szolgáltatásokra vonatkozó javaslatok bekapcsolása?

- **Adatgyűjtés**: a webes beolvasók több milliárd ügyfél-jelet vizsgálnak és gyűjtenek a vállalati tartományok pingelésével és a figyeléssel: blogbejegyzések, sajtóközlemények, közösségi streamek és technikai fórumok.  Az összegyűjtött jeleken kívül a firmographics információkat a belső és külső forrásokból is gyűjtjük, például a D&B, a Microsoft belső előfizetése és a tranzakciós adatok.

- **Machine learning**: a rendszer a jeleket a gépi tanulási modellbe helyezi, amely strukturált adatkészletet hoz létre az értékesítések és a marketing-előrejelzések alapján minden ügyfél számára a felhőalapú termék és a fürt számára.  Minden ügyfél egy, a Microsoft legfontosabb SMB-modelljét használja, amely meghatározza az ügyfél illeszkedését, valamint a gépi tanulási algoritmusokat, amelyek az ügyfél online viselkedését a szándék szerint határozzák meg. A pontozás olyan fürtökbe van egyesítve, amelyekben az ügyfél a Microsoft Cloud termékek megvásárlására való hajlamot jeleníti meg.

- **Optimalizálás**: a Machine Learningrendszer optimalizálja a modelleket úgy, hogy a tranzakciós adatokat havonta és az előfizetési adatokat negyedévente felhasználva.  A nyerési/adatvesztési művelettel a Machine Learning módosítja az algoritmusokat, és ellenőrzi, hogy a modellek a várt módon működnek-e a fürt ajánlásainak összehasonlításával a MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Képernyőkép az SMB Machine learningről.":::

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

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB prediktív modellek.":::

3. Fürtözés

   A megfelelő és a szándékú jelek összevonása egy fürtözési pontszámba történik. A CloudAscent négy fürttel rendelkezik:

      - Azonnali működés – értékesítésre kész ügyfelek
      - Kiértékelés – marketing-Ready ügyfelek
      - Ápolás – a tudatosságnövelő kampányok
      - Nevelés – képzés és monitorozás a szándékkal

   A fürtözés lehetővé teszi a felhasználók számára, hogy meghatározott ügyfeleket célozzanak értékesítési és marketing kezdeményezésekhez szegmens tényezők alapján, például: termék, Geo, iparág és vertikális.

   A CloudAscent-munkafüzetek megosztó **modell** lapja megosztja a hajlamot és a becsült szóköz bevételt. A Fit és a szándék fürtözésének definiálásához végezze el a következő lépéseket:

      1. A ML-modellek használatával először a 100-es skálán számítjuk ki az ügyfél-igazítási pontszámot és a szándék pontszámát.  A pontos pontszámok ML modellek alapján változnak.  Példa az alábbi pontszámokra:

         |**Osztályozás**|**Pontszám**|
         |---------|:---------|
         |Magas|75 – 100|
         |Közepes|55 – 74|
         |Alacsony|30 - 54|
         |Nagyon alacsony|0 - 29|

      2. A fenti szabály használatával a vállalatokat magas, közepes, alacsony és nagyon alacsony értékre osztályozjuk mind az ügyfél, mind a szándékos jelzések esetében.

      3. Az ügyfél-igazítási és szándéki jeleket egy 2D-mátrixban ábrázoljuk, amely a hajlamot jelképező minden metszettel rendelkezik. Például: nagy teljesítményű + magas szándékú = a1, amely a legmagasabb szintű hajlamot jelöli.

      4. Végül ezek a szegmensek csoportosítva alkotják a fürtöket.  Például: a1, a2, a3, a4, a jogszabály most fürt.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent modellek.":::

   Ezen ügyfelek esetében javasoljuk, hogy most célozza meg a célzást, és értékelje az ügyfeleket.

## <a name="cloudascent-products--models"></a>CloudAscent-termékek & modellek

A következő ábra az egyes CloudAscent-modellekre vonatkozó nézeteket tartalmazza:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent-modellezési modell.":::

A szóközökből álló modellek olyan meglévő Microsoft-ügyfelek számára készült előrejelzésekből állnak, amelyek nem rendelkeznek termékkel és/vagy a nettó új potenciális ügyfelekkel.

A upsell-modellek tranzakciós adataikkal jósolják meg az Azure-ban és Microsoft 365 SKU-ban felhasználható upsell-t.

Az EOS a Windows 7, az Office 2010, a SQL Server és a Windows Server rendszerhez tartozó ügyfeleket osztja meg. Az EOS-adatok az MS Sales szolgáltatásból vannak leküldve, és az CloudAscent-modellezési modellezéssel, ahol elérhető. Az EOS-adatforgalom a modern és az Azure Sales szolgáltatásban is működik.
