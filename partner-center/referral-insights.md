---
title: Javaslati megállapítások lekérése
ms.topic: article
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Tekintse át rendszeresen a hivatkozások elemzési adatait a Partnerközpont, hogy lássa a trendeket az üzleti célok elérése érdekében.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a8227fecae05d3752d65651dea4cdc62c9ea672
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120851"
---
# <a name="get-referral-insights-in-partner-center-and-find-out-how-your-referrals-are-doing"></a>A hivatkozások elemzésének Partnerközpont és a hivatkozások ismereti

**Megfelelő szerepkörök**

- Ajánlói rendszergazda

A **Hivatkozások Elemzés** szakaszában  található Együttműködési lehetőségek oldalon megtekintheti, hogyan állnak az ajánlások. Ezeket a metrikákat rendszeresen áttekintve azonosíthatja a trendeket vagy a figyelmet igényelő területeket, és elkezdi elérni az üzleti céljait.

Az Együttműködési lehetőségek elemzési adataihoz a Partnerközpont menüben válassza a Hivatkozások > **Analytics > lehetőségek lehetőséget.**

> [!Important]
> Az üzlettípus szűrője előre alkalmazva van, és **az** összes adathoz az értékesítés típusa van kiválasztva. Távolítsa el a szűrőt, ha a privát és a partner által vezetett ügyletekhez kapcsolódó adatokat szeretné elárolni.

## <a name="apply-filters"></a>Szűrők alkalmazása

Az Együttműködési lehetőségek  oldal tetején kiválaszthatja azt az időszakot, amelyre vonatkozóan meg szeretné jelenni az adatokat. Az alapértelmezett beállítás **a 3M** (három hónap), de választhatja azt is, hogy hat hónapig, vagy inkább egy évig mutatja az adatokat. Az Egyéni lehetőséget **választva** egy adott időszakban az összes ajánló adatait is láthatja.

A Szűrők  gombra kattintva megnyithatja a panelt, amely lehetővé teszi az oldalon található összes adat szűrését az Ügyfél neve, Ország, Az ajánlat típusa, az Ajánlat iránya, a Megoldás neve és az Állapot alapján. Az alábbiakban ezeknek a szűrőknek a részletei olvashatók.

- **Ügyfél neve:** Az alapértelmezett érték **a Mind**, de az adatokat egy vagy több kiválasztott ügyfélre korlátozhatja.
- **Ország:** Az alapértelmezett érték **a Mind**, de az adatokat a kiválasztott ügyfél egy vagy több országára korlátozhatja.
- **Ügylet típusa:** Az  alapértelmezett érték az Közös értékesítés, de választhatja az Összes lehetőséget, vagy a választás alapján korlátozhatja az adatokat privát vagy partner által irányított ügyletekre.
- **Az üzlet iránya** Az alapértelmezett **érték a Mind**, de az  adatokat korlátozhatja bejövő (ön által kapott) vagy kimenő (elküldött) hivatkozásokra. 
- **Megoldás neve:** Az alapértelmezett érték **a Mind**, de az adatokat korlátozhatja olyan hivatkozásokra, amelyek egy vagy több kiválasztott megoldást tartalmaznak.
- **Állapot:** Az alapértelmezett érték a **Mind,** de az adatokat korlátozhatja olyan hivatkozásokra, amelyek egy vagy több hivatkozási állapottípust tartalmaznak, például a létrehozott, elfogadott, elutasított, lejárt, elveszett és megnyert adatokat.

Az alább felsorolt diagramok adatai a dátumtartományt és a kiválasztott szűrőket tükrözik, kivéve az alább látható módon. Egyes szakaszok további szűrők, például egy adott megoldás szűrését is lehetővé teszik.

## <a name="referrals-summary"></a>A hivatkozások összegzése

Ez a kártya áttekintést nyújt az együttműködési lehetőségekről.

A diagramon az Dealek teljes száma, a megnyert összegek, az elveszettek száma és a kiválasztott időszakra vonatkozó ügylet teljes mennyisége (USD-ben) látható.

A százalékos változási metrikák (piros vagy zöld színnel és  nyíljelzővel jelölve) jelzik a különbséget a kiválasztott dátumtartomány utolsó teljes hónapja és a tartomány első teljes hónapja **között.** Tegyük fel például, hogy az aktuális dátum június 15., és a **3 millió** szűrőt választotta az elmúlt három hónap adatainak megjelenítése érdekében. Ebben az esetben ezek a metrikák a májusi (a kiválasztott időszak utolsó teljes hónapja) és a március (a kiválasztott időszak első teljes hónapja) közötti különbséget mutatják, a kiválasztott dátumtartomány az elmúlt **3 millió,** az összehasonlítás a májusi és a márciusi adatok között lenne.

:::image type="content" source="images/referrals/cosellanalyticssummary.png" alt-text="Az együttműködési lehetőségek elemzésének összegző kártyáját bemutató kép.":::

## <a name="conversion-funnel"></a>Konverziós tölcsér

Ez a szakasz azt mutatja be, hogyan mozognak az ajánlatok az egyes államok között az életciklusuk során. A szakasz fő kimutatása alapján megtekintheti a teljes életciklust az ajánlat mennyisége és az üzlet USD-ben megadott értéke alapján. Az első szakasz az állapot és az deal típusa címkével van megcímkézve, így típus szerint vizuálisan is jelzi a kötetet vagy az értéket. Van egy korábbi szakasz is, a **Referrals**(Hivatkozások) is, amely jelzi, hogy milyen ügyleteket tett annak érdekében, hogy elfogadja vagy visszautasítsa őket, vagy hogy a jelentéshez kiválasztott időszakban megnyertként/elveszettként jelölje meg őket. Szűrők alkalmazásával megtekintheti az ügyletek előrehaladását az életciklusuk különböző szakaszaiban.

Az közös értékesítés bejövő ügyletei az Elfogadva, Elutasítva vagy Lejárt ügyletekbe egyesíthetők, mivel a partnereknek el kell fogadniuk vagy el kell utasítanunk a bejövő közös értékesítést.

:::image type="content" source="images/referrals/inbound.png" alt-text="Kép a bejövő hivatkozások államairól.":::

A partner által vezetett, a privát és az közös értékesítés kimenő ügyletei a Létrehozva típusba fognak egyesülni, mivel az ilyen típusú ügyleteket partnerek hoznak létre.

:::image type="content" source="images/referrals/outbound.png" alt-text="A kimenő hivatkozások államát bemutató kép.":::

:::image type="content" source="images/referrals/cosell-analytics-funnel-v2.png" alt-text="A hivatkozások konverziós tölcsérét bemutató kép.":::

## <a name="deals-by-geography"></a>Ajánlatok földrajzi hely szerint

Ez a szakasz azokat az országokat/régiókat mutatja be, ahonnan az ügylet érkezett, valamint az egyes országok/régiók részleteit. Az egyes országokra vonatkozó ajánlat részleteit táblázatos nézetben, valamint az összes ország térképnézetét is megtekintheti. Kiválaszthat egy adott országot a táblázatban, vagy kiválaszthatja a térképnézetet egy adott ország nagyításához.

:::image type="content" source="images/referrals/cosell-analytics-geo-distribution-v2.png" alt-text="A hivatkozások földrajzi eloszlását bemutató kép.":::

## <a name="deals-by-solutions"></a>Megoldások alapján kötött ügyletek

Ezen a diagramon láthatja, hogy mely megoldások vezetik a legtöbb ajánlást, és melyek a legnagyobb értékűek. A táblázat három kimutatást tartalmazza: Közös értékesítés, partner által vezetett és privát.
A kimutatás kiválasztása alapján a megoldás szerint összesítve láthatja az ügyletek teljesítményét.

> [!NOTE]
> Ha egy ajánlat több megoldást is tartalmaz, a táblázatban ugyanaz az üzlet szerepel, amely beleszámolt az összes megoldásba. Ne adja hozzá a megoldásokhoz kapcsolódó értékeket, és hasonlítsa össze őket más hivatkozókötet-metrikákkal. Ez a nézet segít megérteni a megoldás kimutatásának teljesítményét.

A táblázat tartalmazza az összes olyan ügyletet, amelyekben szerepel a megoldás, valamint az olyan államok, mint az megnyert ügyletek, az elveszett ügyletek, az ügyletek lejártak, valamint az összes megnyert és elveszett ügylet USD pénznemben. A tábla jobb oldalon található egy ügyleti trendgrafikon is, amely a kiválasztott megoldás alapján mutatja az összes ügylet számát és az ügylet usd pénznemben megnyert értékét. Az alapértelmezett beállítás az összes megoldás.

:::image type="content" source="images/referrals/cosell-analytics-solutions-v2.png" alt-text="A megoldások teljesítményét bemutató kép.":::

## <a name="declined--lost-reasons"></a>Elutasított & okok miatt

Ez a szakasz segít elemezni az okokat,  amelyek  miatt a vállalat elutasítottként vagy elveszettként jelöli meg az ügyleteket. Az ilyen ábrázolásokkal ugyanazok az okok állnak rendelkezésre, mint amit az értékesítők az üzlet elutasítása vagy csökkenése esetén választottak.

:::image type="content" source="images/referrals/cosellanalyticsreasons.png" alt-text="A partner által a visszautasítás vagy az üzlet elveszítés esetén kiválasztott okokat bemutató kép.":::

## <a name="comparison-charts"></a>Összehasonlító diagramok

Az összehasonlítási szakasz segítségével összehasonlíthatja a hivatkozásokhoz kapcsolódó adatokat több dimenzió alapján a mennyiség és az USD-kimutatásban megnyert ügyletérték alapján.
Az adatok összehasonlítására kiválasztható három dimenzió a következő:

- Ajánlat típusa
- Piacok
- Megoldások

Ha az ügylet típusa van kiválasztva, összehasonlíthatja a hivatkozási teljesítményét az együttműködési lehetőségek, a partner által irányított és a privát ügyletek tekintetében. A piacokon és a megoldásokban is három különböző lehetőség közül választhat a teljesítményük összehasonlítására. Az első diagram, amely egy sávdiagram, havi trend szerint adatokat tartalmaz a fő kimutatás alapján, amely a mennyiség vagy az ügylet megnyert értéke. A sávdiagramtól jobbra egy tortadiagram is látható, amely ugyanezen adatok százalékos eloszlását mutatja.

:::image type="content" source="images/referrals/cosell-analytics-compare-v2.png" alt-text="Az összehasonlítás szakaszt bemutató kép.":::

## <a name="raw-data-table"></a>Nyers adattábla

Az alábbi táblázat az együttműködési lehetőségekhez kapcsolódó összes nyers adattal  együtt segít gyorsan exportálni az adatokat az elvégezni kívánt részletes vagy egyéni elemzésekhez.

:::image type="content" source="images/referrals/cosellanalyticsrawdata.png" alt-text="A hivatkozások nyers adattábláját bemutató kép.":::

## <a name="no-data"></a>Nincs adat

Több oka is lehet annak, hogy az alábbihoz hasonló üres diagram jelenik meg az együtt értékesítés elemzésének elérésekor, az alábbiakban leírtak szerint.

- Ehhez a fiókhoz nincsenek adatok. Próbáljon meg ügyleteket létrehozni a jelentés feltöltéséhez.
- Hálózati kapcsolati probléma lépett fel. Ellenőrizze az internetkapcsolatot, és próbálkozzon újra.
- Az oldal az alapértelmezett szűrővel töltődik be az együttműködési ügyletekhez. Ha csak privát ügyleteket kínál, állítsa alaphelyzetbe az ügylettípus szűrőt.
- Nincsenek az alkalmazott szűrőknek megfelelő rekordok. Próbálkozzon a szűrők alaphelyzetbe állításával.
- A lehetőség állapotának módosítása és az elemzési jelentésben való frissítése között késés van. Ellenőrizze a jelentést 24 óra után.

:::image type="content" source="images/referrals/nodata.png" alt-text="Kép a hivatkozások adatmegjelenítésének mellőzését ábrázoló képről.":::

> [!NOTE]
> A **Javaslatelemzések** lapon csak a Partnerközpontban létrehozott javaslatok jelennek meg. Nem mutatja a Partner Sales [Connecten](psc-to-pc.md) vagy más mechanizmusokon keresztül létrehozott hivatkozások adatait.

> [!TIP]
> Az üzleti profil végrehajtásához tekintse meg az Üzleti profilokkal kapcsolatos elemzések oldalt [a](https://www.microsoft.com/solution-providers/home) Megoldásszolgáltatói élmény [megkereséséhez.](analyze-your-marketing-profile.md)
