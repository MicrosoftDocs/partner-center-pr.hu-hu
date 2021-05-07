---
title: Kifizetési fiók és & beállítása – Microsoft kereskedelmi piactér
description: Ha pénzt szeretne kapni a kereskedelmi piactéren elérhető ajánlat értékesítéseiből, megtudhatja, hogyan állíthatja be kifizetési fiókját, és töltheti ki a szükséges adó űrlapokat.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 12/10/2019
ms.openlocfilehash: 8f680753216ea9cd515c8082495b390c7bf95a62
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702807"
---
# <a name="set-up-your-payout-account-and-tax-forms"></a>Kifizetési számla és űrlapok beállítása

**Megfelelő szerepkörök**

- Fiókadminisztrátor
- Globális rendszergazda

Ahhoz, hogy pénzt kapjon a kereskedelmi piactéren elérhető ajánlat értékesítéseiből, be kell állítania a kifizetési fiókját, és ki kell töltenie a szükséges [adózási űrlapokat a Partnerközpont.](https://partner.microsoft.com/dashboard)

Ha csak ingyenes ajánlatokat tervez listába állítani (és nem tervez alkalmazáson belüli vásárlásokat kínálni vagy Microsoft Advertising-t használni), nem kell kifizetési fiókot beállítania vagy adó űrlapokat kitöltenie. Ha később meggondolja magát, és úgy dönt, hogy ajánlatokat (vagy bővítményeket) szeretne értékesíteni, beállíthatja a kifizetési fiókját, és kitöltheti az adó űrlapokat. A kifizetési fiók és az adóprofil befejezéséig nem küldhet be fizetős ajánlatokat vagy bővítményeket.

> [!NOTE]
> Bizonyos piacokon a közzétevők csak ingyenes ajánlatot küldhetnek be. Ha a fiókja regisztrálva van ezen piacok egyikében, nem lesz lehetősége kifizetési számla beállítására.

A fiók beállítása után két dolgot kell megtennie ahhoz, hogy ajánlatot (vagy bővítményeket) értékesítsen a kereskedelmi piactéren:

- [Töltse ki az adó űrlapokat](#tax-forms)
- [Kifizetési fiók beállítása](#payout-account)

> [!NOTE]
> További részleteket arról, hogy hogyan és mikor fizeti ki az ajánlata pénzét: Fizetés a kereskedelmi [piactéren.](marketplace-get-paid.md)

## <a name="tax-forms"></a>Adózási űrlapok

Az adóprofilt és az  adózási űrlapokat az alkalmazás Kifizetés és adó oldalán Partnerközpont. A szervezet engedélyei határozzák meg a látható profilokat és információkat.

### <a name="create-or-update-your-tax-profile"></a>Adóprofil létrehozása vagy frissítése

Először létre kell hoznia egy adóprofilt, és hozzá kell rendelnie a programban részt vett programokhoz. Az alábbi lépésekkel hozhatja létre vagy frissítheti *adóprofilját a* Partnerközpont. Az adó űrlapokat elektronikus úton is beküldheti az Partnerközpont irányítópultján; A legtöbb esetben nem kell űrlapokat kinyomtatni és leveleket küldeni.

> [!IMPORTANT]
> A különböző országokra és régiókra különböző adózási követelmények vonatkoznak. Az, hogy pontosan mennyi adót kell fizetnie, az ajánlat értékesítésének országától és régióitól függ. A [microsoftos Microsoft Azure Marketplace](https://go.microsoft.com/fwlink/p/?LinkID=699560) közzétevői szerződésében találhatja meg, hogy a Microsoft mely országokra/régiókra vonatkozó adózási Más országokban/régiókban– a regisztráció helyétől függően – előfordulhat, hogy közvetlenül a helyi adószolgáltatónak kell átcsoportosoznia az értékesítéseket, és adóhasználatot kell használnia az ajánlat értékesítéséhez. Emellett előfordulhat, hogy az ön által kapott alkalmazásértékesítési bevétel bevételként is adózható. Határozottan javasoljuk, hogy lépjen kapcsolatba az országa vagy régiója megfelelő hatóságával, amely a legjobban segíthet meghatározni a megfelelő adózási adatokat a kereskedelmi piactér tevékenységeihez.

1. A Partnerközpont [jobb](https://partner.microsoft.com/dashboard)felső sarkában  válassza a Beállítások fogaskerék ikont, majd a **Fiókbeállítások lehetőséget.**

2. A bal oldali navigációs menüben válassza a **Kifizetés és adó** lehetőséget, majd a Kifizetések és **adó-hozzárendelések elemet.**

3. Válassza ki azt a program- és értékesítőazonosító-kombinációt, amelyhez adózási adatokat szeretne konfigurálni.

4. Ha meglévő adóprofilt szeretne használni, válassza ki azt a legördülő menüből. Ellenkező esetben válassza az **Új profil létrehozása lehetőséget, majd** nyomja le a Submit **(Küldés) gombot.** Meg fog jelenni az adóprofilok oldala.

5. Az **adóinformációk** szerkesztéséhez kattintson a Szerkesztés gombra.

6. Válassza ki a megfelelő választógombot, és ha a rendszer kéri, válassza ki az országot/régiót. Ez a lépés határozza meg azt a Microsoft üzleti entitást, amely a fiókon történő kifizetéshez lesz használva.

7. A 6. lépésben kiválasztott beállításoktól függően a rendszer kérni fogja, hogy adja meg az országhoz/régióhoz szükséges adózási információkat.

   > [!NOTE]
   > A kereskedelmi piactéren elérhető bármely ajánlat vagy bővítmény értékesítéshez Egyesült Államok országtól/régiótól függetlenül ki kell töltenie egy adóbevallási űrlapot. Azok a közzétevők, Egyesült Államok megfelelnek bizonyos követelményeknek, ki kell tölteniük egy IRS W-9 űrlapot. A Egyesült Államok közzétevőknek ki kell tölteniük az IRS W-8 űrlapot. Ezeket az űrlapokat online is kitöltheti az adóprofil kitöltése után.

### <a name="withholding-rates"></a>Visszatartott díjak

Az adó űrlapokon bekért információ határozza meg a megfelelő adóelőleg-mértéket. A visszatartott díj csak a vállalaton Egyesült Államok; az Usa-on kívüli helyekre történő értékesítések nem vonatkoznak visszatartott értékesítésre. A visszatartott díjak eltérőek, de a legtöbb, a Egyesült Államok regisztráló közzétevő esetén az alapértelmezett díjszabás 30%. Lehetősége van csökkenteni ezt a mértéket, ha országa/régiója elfogadta a bevételi adó mértékét a Egyesült Államok.

### <a name="tax-treaty-benefits"></a>Adódedékok előnyei

Ha kívül esik a Egyesült Államok, kihasználhatja az adóelőnyt. Ezek az előnyök országonként/régiónként eltérőek lehetnek, és lehetővé tehetik a kereskedelmi piactéren visszatartott adó összegének csökkentését. Az adókedvezményeket a W-8BEN űrlap II. részének kitöltésével igényelheti. Javasoljuk, hogy kommunikáljon az ország vagy régió megfelelő erőforrásaival annak megállapításához, hogy ezek az előnyök érvényesek-e Az Ön számára.

> [!NOTE]
> A Egyesült Államok azonosító szám (vagy ITIN) nem szükséges a Microsofttól való kifizetéshez vagy az adóval kapcsolatos előnyök igényléséhez.

## <a name="payout-account"></a>Kifizetési számla

A kifizetési számla az a bankszámla, amelyre az értékesítésből származó bevételeket küldjük. A Profil lapon megadott összes fizetési fiókot megtekintheti.

> [!NOTE]
> Egyes piacokon a PayPal használható a kifizetési fiókjához. További részleteket az alábbi [PayPal-adatokban](#paypal-info) talál, hogy a PayPal támogatott-e egy adott piacon. [](payment-thresholds-methods-timeframes.md)

### <a name="create-a-payment-profile"></a>Fizetési profil létrehozása

1. A [Partnerközpont](https://partner.microsoft.com/dashboard)jobb felső **sarkában** válassza a Beállítások fogaskerék ikont, majd a **Fiókbeállítások lehetőséget.**
2. A Kifizetés és *adó fejléc* alatt válassza a Kifizetési **és adóprofil-hozzárendelés lehetőséget.**

    > [!NOTE]
    > Mivel ezek bizalmas adatok, előfordulhat, hogy a rendszer arra kéri, hogy jelentkezzen be újra.

3. Válassza ki a konfigurálni kívánt fizetési módot.

4. Válasszon ki egy meglévő fizetési profilt, vagy válassza **az Új** fizetési profil létrehozása lehetőséget egy új profil létrehozásához a kiválasztott fizetési módhoz.

### <a name="create-a-bank-based-payment-profile"></a>Bankalapú fizetési profil létrehozása

Ha úgy választotta, hogy egy banki fiókot használ a kifizetések fogadásához, a következő folyamattal konfigurálhatja a banki fiókját.

1. A *Bankprofil lapon* adja meg a bank szükséges adatait.
2. Adja meg a bankszámla adatait.

    > [!NOTE]
    > A fiókadatokhoz használt mezők csak alfanumerikus karaktereket fogadnak el.

3. Adja meg a személyes adatokat.
4. A *Profil-hozzárendelés oldalon* válassza ki azt a pénznemet, amit a kifizetések kiállításakor használni szeretne.

    > [!WARNING]
    > Győződjön meg arról, hogy a bank elfogadja a kiválasztott kifizetési pénznemet.

5. Minden olyan programhoz ki kell választania egy fizetési profilt, amely részt vesz, de ugyanazt a profilt több programhoz is használhatja.

6. A módosítások mentéshez válassza a Küldés lehetőséget.

   > [!NOTE]
   > A Microsoft akár 48 órát is igénybe vehet, hogy érvényesítse az Ön profiljában található adatokat. Ha a folyamat befejeződött, *az ellenőrzési állapot* Complete (Kész) állapotot fog **mutatni**

A kifizetés sikeres voltának biztosítása érdekében győződjön meg a következőről:

- A **kifizetési fiókjához** megadott fióktulajdonosi névnek Partnerközpont meg kell egyezésnek lennie a fiókjához társított névvel. Ha például a bankszámla neve tartalmaz egy középső nevet, adjon hozzá egy középső nevet a **fióktulajdonos nevéhez.**
- A kifizetéseket a rendszer közvetlenül a Microsofttól az Ön fiókjába, USD pénznemben továbbítja.
- A latin Partnerközpont beírt banki adatokat a rendszer cirill karakterekre fordítja le.

### <a name="editing-existing-payment-profiles"></a>Meglévő fizetési profilok szerkesztése

Szerkesztheti a meglévő fizetési profilokat, ha módosításokat kell vagy helytelen információkat kell kijavítani.

1. A [Partnerközpont](https://partner.microsoft.com/dashboard)jobb felső **sarkában** válassza a Beállítások fogaskerék ikont, majd a **Fiókbeállítások lehetőséget.**

2. A Kifizetés és *adó fejléc* alatt válassza a Kifizetési **és adóprofilok lehetőséget.**

3. A fizetési profilok és azok állapota is megjelenik. Keresse meg a szerkeszteni kívánt profilt, és válassza a **szerkesztés lehetőséget** a jobb oldalon

> [!IMPORTANT]
> A kifizetési fiók módosítása legfeljebb egy fizetési ciklussal késleltetheti a kifizetéseket. Ez a késés azért következik be, mert ellenőrizni kell a fiók változását, ahogyan azt a kifizetési fiók első beállításakor is tette. A teljes összeget a fiók ellenőrzése után is kifizeti. az aktuális fizetési ciklushoz esedékes kifizetések a következő fizetési ciklushoz lesznek hozzáadva. További [információ: Fizetés a kereskedelmi piactéren.](marketplace-get-paid.md)

### <a name="paypal-info"></a>PayPal-adatok

Egyes országokban és régiókban a PayPal-adatok megadásával hozhat létre fizetési fiókot. Mielőtt azonban fizetési fiókként a PayPal lehetőséget választanának:

- Ellenőrizze [a fizetési küszöbértékeket,](payment-thresholds-methods-timeframes.md) a módszereket és az időkereteket annak ellenőrzéséhez, hogy a PayPal támogatott fizetési mód-e az Ön országában vagy régiójában.
- Tekintse át az alábbi gyakori kérdések közül. Az adott helyzettől függően előfordulhat, hogy a PayPal nem a legmegfelelőbb fizetési mód az Ön számára, és egy banki fiókot is előnyben részesíthet.

Gyakori kérdések a PayPal fizetési módként való használatával kapcsolatban:

- **Milyen PayPal-beállításokra van szükségem a kifizetések fogadása érdekében?** Győződjön meg arról, hogy PayPal-fiókja nem blokkolja az eCheck kifizetéseket. Ezt a beállítást a PayPal Fizetési fogadási beállításai lapján lehet kezelni. További információért lásd a [PayPal fiókbeállítási](https://go.microsoft.com/fwlink/?linkid=2162542) oldalát.

- **Támogatott az országom/régióm?** A [Fizetési küszöbértékek, módszerek](payment-thresholds-methods-timeframes.md) és időkeretek alatt kideríti, hol támogatott a PayPal fizetési mód.

- **A PayPal-fiókomnak ugyanabban az országban vagy régióban kell regisztrálva lennie, mint a Partnerközpont fiókom?** Nem. PayPal-fiók beállításakor elfogadhatja az alapértelmezett konfigurációt. Más országokkal/régiókkal és pénznemekkel nem lehet probléma, kivéve, ha bizonyos pénznemekben letiltotta a fizetést. Ezt a beállítást a PayPal Payment Receiving Preferences (Fizetési módok fogadása) lapján lehet kezelni.

- **Manuálisan kell elfogadnom a PayPal-kifizetéseket?** Nem. A PayPal-fiókok alapértelmezés szerint úgy vannak beállítva, hogy a felhasználóknak manuálisan el kell fogadniuk a kifizetéseket, ami azt jelenti, hogy ha 30 napon belül nem fogadja el a kifizetést, a rendszer visszaadja azt. Ezt a beállítást a "Kérdezzen" beállítás kikapcsolásával módosíthatja a PayPal További beállítások oldalán.

- **Milyen pénznemeket támogat a PayPal?** Az aktuális listát a [PayPal támogatási](https://developer.paypal.com/docs/classic/api/currency-codes/#paypal) oldalán láthatja

### <a name="specific-requirements-for-certain-countriesregions"></a>Bizonyos országokra/régiókra vonatkozó konkrét követelmények

Egyes országokban és régiókban a kifizetési fiókokra vonatkozó további követelményeket is be kell tartani. Ha Egyesült Államok, Oroszország vagy Oroszország területén rendelkezik helyiekkel, vegye figyelembe az alábbi követelményeket.

#### <a name="pakistan"></a>Pakisztán

A Form-R egy banki szabályozási követelmény. A rendeltetése és oka, hogy a ki nem számlált összeget ki kell használni. Ezért minden olyankor, amikor jogosult a Microsoft havi kifizetésre, be kell nyújtania egy R űrlapot a banknak, mielőtt a kifizetést kiadhatja a fiókjába. A Form-R másolatának beszerzéséhez lépjen kapcsolatba a helyi bankfiókkal.

Minden hónapban be kell nyújtania egy Form-R űrlapot a bankjának, hogy jogosult legyen kifizetésre. Ha például az év minden hónapját kifizetésre számítja, 12-szer kell beküldődnie az R űrlapot (havonta egyszer).

Miután a kifizetést elküldték a banknak, 30 napja van az R űrlap beküldre. Ha az összeget nem 30 napon belül beküldik, a rendszer visszaküldi az összeget a Microsoftnak.

#### <a name="russia"></a>Oroszország

Ha Ön egy olyan közzétevő, aki Oroszországban él, előfordulhat, hogy dokumentációt kell nyújtania a banknak, mielőtt a bankja a számlájára helyezi a összeget. Ha jogosult a fizetésre, a következő dokumentációt fogjuk biztosítani egy e-mail-üzenetben:

- Elfogadási tanúsítvány (AC) – a fiókba átvitt kifizetések mennyiségét tartalmazza.
- [Microsoft Azure Marketplace Közzétevői](https://go.microsoft.com/fwlink/p/?LinkID=699560)  szerződés – a közzétevői szerződés aláírt másolata, amelyről számlálót kell aláírni.

A kifizetés sikeres voltának biztosítása érdekében győződjön meg a következőről:

- A **kifizetési számlán** megadott fióktulajdonosi névnek pontosan Partnerközpont kell lennie a bankszámlaszámhoz társított névnek. Ha például a fióknév tartalmaz egy középső nevet, adjon hozzá egy középső nevet a **fióktulajdonos nevéhez.**
- A kifizetéseket a rendszer közvetlenül a Microsofttól a microsoftos számlára, a microsoftos pénznemben utalja át.
- A rendszer a latin Partnerközpont megadott banki adatokat cirill karakterekre fordítja le.
- A kifizetéseket nem bankkártya, csak egy banki számlára kell fizetni.

#### <a name="ukraine"></a>Ukrajna

Ha Ön közzétevő, és az Egyesült Államok területén él, előfordulhat, hogy dokumentációt kell nyújtania a banknak, mielőtt a bankja a számlájára helyezi a összeget. Ha jogosult a fizetésre, a következő dokumentációt fogjuk biztosítani egy e-mail-üzenetben:

- Elfogadási tanúsítvány (AC) – a fiókba átvitt kifizetések mennyiségét tartalmazza.
- [Microsoft Azure Marketplace Közzétevői](https://go.microsoft.com/fwlink/p/?LinkID=699560) szerződés – a közzétevői szerződés aláírt másolata, amelyről számlálót kell aláírni.
- Módosítási szerződés (AA) – ezt a dokumentumot a bank használhatja a kifizetési összeg azonosításához.

A Microsoft mindhárom dokumentumot biztosítja az első kifizetési kísérletkor. Minden további kifizetés esetén csak az AC-dokumentumot kapja meg. Őrizze meg az ADA- és AA-dokumentumokat arra az esetre, ha szüksége lenne rájuk, hogy jövőbeli kifizetéseket kapjanak a banktól.

### <a name="create-a-paypal-payment-profile"></a>PayPal fizetési profil létrehozása

Ha úgy választotta, hogy egy banki fiókot használ a kifizetések fogadásához, a következő folyamattal konfigurálhatja a banki fiókját.

1. A *PayPal lapon* adja meg a PayPal-fiókjával kapcsolatos szükséges adatokat.
2. Adja meg a PayPal-fiók adatait.

    > [!NOTE]
    > A fiókadatokhoz használt mezők csak alfanumerikus karaktereket fogadnak el.

3. Adja meg a személyes adatokat.
4. A *Profil-hozzárendelés oldalon* válassza ki azt a pénznemet, amit a kifizetések kiállításakor használni szeretne.
5. Minden olyan programhoz ki kell választania egy fizetési profilt, amely részt vesz, de ugyanazt a profilt több programhoz is használhatja.
6. A módosítások mentéshez válassza a Küldés lehetőséget.

## <a name="next-steps"></a>Következő lépések

[Fizetés fogadása a kereskedelmi piactéren](marketplace-get-paid.md)
