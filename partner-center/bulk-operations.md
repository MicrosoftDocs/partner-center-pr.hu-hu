---
title: Közös értékesítés tömeges exportálása és importálása Excel-/CSV-fájlokkal a hivatkozásokban
description: Megtudhatja, hogyan tölthet le, hozhat létre vagy frissíthet együttműködési lehetőségeket Excel- (CSV-) fájlokkal a Partnerközpont
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: af567b9b8b36841b6e6fd7e18a34e1c4b6b81f2e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149162"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Tömeges műveletek az együttműködési lehetőségekhez vesszővel elválasztott értékeket (CSV) használó fájlok használatával

**Megfelelő szerepkörök:** Ajánlói rendszergazdai | Ajánlói felhasználó

A nagyvállalatok tömeges Partnerközpont segítenek a vállalatnak az együttműködési lehetőségek adatainak exportálásában és importálásában. Az **Oldalcím szalagcím** jobb felső  részen keresse meg az importálási és exportálási hivatkozásokat az Együttműködési lehetőségek oldalon.  A hivatkozási **rendszergazdai és** a **ajánlói** felhasználói engedélyekkel rendelkező felhasználók is használhatjak ezt a funkciót.

> [!IMPORTANT]
> A tömeges importáláson keresztül végzett létrehozási/frissítési műveletek nem visszafordíthatók. Nagy számú rekord módosításakor vagy létrehozásakor körültekintően járjon el. Az üzlet létrehozása után csak a mezők egy része módosítható. **Semmilyen művelet nem engedélyezett, ha bármely üzlet elér egy terminálállapotot, például elutasítva,lejárt,megnyert/elveszett.**

## <a name="export-co-sell-opportunities"></a>Közös értékesítés lehetőségeinek exportálása

Az alábbi információk az exportálási funkciót ismertetik:

- Legfeljebb **5000** rekordot exportálhat az **exportálási gombra kattintva.**
- A letöltött ügyletek a hozzáférési szinteken alapulnak. A javaslati rendszergazdák és a javaslati felhasználók különböző eredményeket kapnak a hatókörüktől és a csapattagokként való felvételüktől függően. További információ a [hivatkozási engedélyekről.](permissions-overview.md#manage-referrals)
- Az exportálási függvény figyelembe veszi az együttműködési lehetőségek oldalának aktuális lapját és az alkalmazott szűrőket.
- Létrejön egy CSV-fájl, amely az alkalmazott szűrőkön alapuló összes adatot tartalmaz.
- A rekordok letöltése akár egy percet is igénybe vehet.
- Nem kell megvárni a letöltési művelet befejezését. A fájl akkor is letölti a fájlt, ha Partnerközpont más oldalakra navigál, amint az exportálási függvény befejeződött.
- A letöltött fájlt újra felhasználhatja az üzlet részleteinek módosításához és feltöltéséhez a rekordok frissítéséhez.

## <a name="import-co-sell-opportunities"></a>Közös értékesítés lehetőségeinek importálása

- Legfeljebb **1000** rekordot hozhat létre vagy frissíthet az importálási funkcióval.
- A sablont sablon nélkül is felépítheti, ha letölti a sablont az importálási oldal Partnerközpont.
- Az Exportálás funkcióval a meglévő rekordokat is letöltheti és frissítheti.
- Ha a fájl több mint 1000 rekordot tartalmaz, nem lehet feldolgozni.
- A fájl feldolgozása után az utolsó folyamatfájlkártyán megjelenik egy összegzés, amely a létrehozott, frissített és nem feldolgozott hivatkozások számát mutatja.
- Letöltheti a feldolgozott rekordok adatait, kijavíthatja a hibákat, és feltöltheti ugyanazt a fájlt az előző futtatás során meghiúsult rekordok létrehozásához vagy frissítéséhez. **Távolítsa el az összes sikeres rekordot a fájlból az előző futtatás során meghiúsult javított rekordok feltöltése előtt.**
- További megoldások hozzáadásához adjon hozzá további oszlopokat az 1. megoldás mellé, és használja az oszlopnevet X megoldásként, ahol az X a megoldás számát jelöli az üzletben. Például 2. megoldás, 3. megoldás.
- Egy üzlethez akár 50 megoldást is hozzáadhat.
- Ha további csapattagokat szeretne hozzáadni, adjon hozzá további oszlopokat az 1. csapattag mellett, és használja az oszlop nevét X csapattagként, ahol X jelöli a csapattag számát az ajánlatban. Például: 2. csapattag, 3. csapattag.
- Egy üzlethez legfeljebb 50 csapattag adhat hozzá.

> [!NOTE]
> Nem kell megvárni a feldolgozás befejezését. A feldolgozás befejezése után a legutóbb feldolgozott fájl adatai letölthetők lesznek. **1000 rekordot feltöltő fájlok feltöltése akár 10 percig is eltarthat.**

> [!IMPORTANT]
> Olvassa el figyelmesen az utasításokat, és ellenőrizze az alábbi táblázatban található oszlopok formátumát, mielőtt CSV-fájlokkal hoz létre vagy frissít egy ügyletet a Partnerközpont.

|**Oszlop neve**|**Kötelező?**|**Leírás**|**Mintaérték(ék)**|
|-----|:-----|:---------|:---|
Hibák|No|A hivatkozásokra vonatkozó létrehozási/frissítési műveletekkel kapcsolatos hibák ebben az oszlopban szerepelnek. Ha több hiba is történik, mindegyiket pontosvessző választja el egymástól.|Kötelező mező, 1. megoldás hiányzik|
Engagement-azonosító|No|A kötelezettségvállalási azonosítót a Microsoft partnerközpont ajánlási rendszere generálja. Új ajánlás létrehozásához nem szükséges. Ha rekordot frissít, használhatja a meglévő engagement-azonosítót.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Javaslatok azonosítója|No|A hivatkozásazonosítót a Microsoft Partnerközpont ajánlórendszere generálja. Új ajánlás létrehozásához nem szükséges. Ha meglévő rekordot frissít, töltse ki a hivatkozás azonosítójával.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Üzlet neve|Yes|A referenciaként szolgál az ajánlat rövid neve.|Az Egyesült Királyság tavaszi ajánlata
Ügyfél neve|Yes|Az ügyfél vállalatának neve. A Microsoft oldalán a szervezet jogi nevét használhatja a gyors egyeztetéshez.|Contoso Corporation
1. ügyfélcímsor|Yes|Az ügyfélvállalat 1. címsora. |One Contoso Way
Ügyfélcím 2. sor|No|Az ügyfélvállalat 2. címsora.|NE 148 utca
Ügyfélváros|Yes|Az a város, ahol az ügyfélszervezet található.|Redmond
Ügyfél állapota|No|Az ügyfél szervezetének helyének állapota.|Washington
Ügyfél irányítószáma|No|Annak a régiónak az irányítószáma, ahol az ügyfélszervezet található.|98052
Ügyfél országa|Yes|Ország/régió, ahol az ügyfélszervezet található. Használja az itt említett kétbetűs [országkódokat.]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|USA
Ügyfél D-U-N-S azonosítója|No|Próbálja meg lekérni az ügyfélszervezet CÉGES AZONOSÍTÓját. Ez segít a Microsoft oldalán található ügyfélszervezet gyorsabb egyeztetésében, ami gyorsabb értékesítői hozzárendelést nyújt. A TUDS-azonosítót ingyenesen le tudja szerezni erről a [webhelyről.](https://www.dnb.com/duns-number/lookup.html)|81466849
Ügyfél kapcsolattartója – vezetéknév|Függ|Az első név csak akkor kötelező, ha microsoftos segítségre van szüksége. Az ügyfélszervezet elsődleges kapcsolattartója, amely ezen az ajánlaton dolgozik.|John
Ügyfél kapcsolattartási vezetékneve|Függ|A vezetéknév csak akkor kötelező, ha segítségre van szüksége a Microsofttól. Az ezen az ajánlaton dolgozó ügyfélszervezet elsődleges kapcsolattartója vezetékneve.|Ügyfél
Ügyfél kapcsolattartási telefonszáma|Függ|A telefonszám csak akkor kötelező, ha Microsoft-segítségre van szüksége. Az ezen az ajánlaton dolgozó ügyfélszervezet elsődleges kapcsolattartója telefonszáma.|9999999999
Ügyfél kapcsolattartási e-mail-címe|Függ|Az e-mail-cím csak akkor kötelező, ha segítségre van szüksége a Microsofttól. Az ezen az ajánlaton dolgozó ügyfélszervezet elsődleges kapcsolattartója e-mail-címe.|john.customer@contoso.com
Partneri ajánlás állapota|Yes|Az üzlet állapotát jelzi a vállalat szemszögéből. Kötelező, ha hivatkozásokat próbál létrehozni vagy módosítani. Ha **új** ajánlatot próbál létrehozni, használja az Új használhatja. Az elfogadott értékeket itt [dokumentáljuk.](/partner/develop/referral-resources#referralstatus)|Aktív
Partneráttételi alállapotok|Yes|Az üzlet pontos állapotát jelzi. Ha **új ajánlatot** próbál létrehozni, használja az Accepted (Elfogadva) használhatja. Akkor is szükséges, ha egy meglévő ajánlást módosít. Az elfogadott értékeket itt [dokumentáljuk.](/partner/develop/referral-resources#referralsubstatus)|Elfogadva
Microsoft-ajánlás állapota|Függ|A Microsoftnak segítségkérést kérő, közös értékesítésre vonatkozó kérés állapotát jelzi. Ez egy csak olvasható mező. Az adatok importálása során a mezőben történt minden módosítás figyelmen kívül lesz hagyva.| Függőben
Elutasítva/Elveszett ok|Függ| Ezt az információt csak akkor kell megadnia, ha a mező alállapotát Elutasítva vagy Elveszett állapotra módosítja. Ezt az oszlopot figyelmen kívül hagyhatja. <br/> **Adjon meg egy számot az alábbi beállítások alapján** <br/><br/> **1**– A projekt költségvetése nem megfelelő  <br/> **2**– Az ügyfél nem válaszolt  <br/> **3**– Az ügyfél egy másik szállítót választott  <br/> **4** – Az ügyfélkövetelmények nem teljesülnek  <br/> **5** – Nem ügyfél <br/> **6**– A javasolt idővonal túl rövid volt <br/> **7** – Jelentés visszaélésként, levélszemétként vagy adathalászatként <br/> **8** – Egyéb |6|
Értékesítési fázis|No|Ez a mező jelzi a hivatkozás részletes értékesítési szakaszát. Az értékesítési szakaszokról itt olvashat [bővebben](./manage-co-sell-opportunities.md)|40
A mennyiség becsült értéke|Yes|Az üzlet értéke az ügyféllel folytatott kezdeti beszélgetések alapján. Ez módosítható, amíg az ajánlat el nem éri az egyik megnyert vagy **elveszett** **terminál-államot.**|12563
Pénznem|Yes|Az a pénznem, amelyben az ajánlat értéke meg van adva. A pénznemkódokat itt [találja:](https://en.wikipedia.org/wiki/ISO_4217).|USD
Becsült bezárás dátuma|Yes|Az ajánlat becsült lezáró dátuma az ügyféllel folytatott kezdeti beszélgetések alapján, HH/DD/YYYY formátumban. <br/> **A dátumnak UTC időzónában kell lennie. A felhasználói felületen megjelenő Partnerközpont honosított időzónákon alapulnak. A felhasználói felület +/- egy napos eltérést Partnerközpont, ha azt az ajánlást keresi, amelynek a dátumát AZ UTC időzóna szerint határozza meg.**|1/30/2020
CRM-azonosító|No|Az adott ajánlás azonosítója a CRM-rendszerben, ha van ilyen. Ez egy szabad űrlap szövegbeviteli mezője.|34234324-sdfsdf-345345-sfd
Marketingkampány azonosítója|No|Ez a mező jelzi a marketingkampányt, amely ennek az adott ajánlásnak az eredménye volt. Általában a megtérülés kiszámításához használatos|BingSummer2020
Jegyzetek|No|Részletes megjegyzések a hivatkozással kapcsolatos frissítésekről|Ez egy minta megjegyzés
Microsoft-segítségre van szükség?|Yes|Ezzel jelezheti, hogy szeretné-e, ha a Microsoft segíthet önnek az együttműködési kérelem igénylésében|Yes
Milyen konkrét segítségre van szüksége a Microsoftnak?|Függ|A Microsoft hat különböző módon segíthet Önnek. Ez csak akkor érvényes, ha az Igen lehetőséget választja a "Microsoft-segítségre van szükség? " <br/> **Adjon meg egy számot az alábbi beállítások alapján** <br/><br/> **1**– Számítási feladat – adott értékajánlat  <br/> **2**– Ügyfél technikai architektúrája  <br/> **3**– Koncepció igazolása /Bemutató  <br/> **4**– Ajánlatok és licencelés  <br/> **5**– Bejegyzés – sikeres értékesítési ügyfél  <br/> **6**– Általános vagy egyéb|1|
Megosztás a Microsoft értékesítési csapatával|Yes|Ezzel jelezheti, hogy meg szeretné-e osztani az üzlet részleteit a Microsoft értékesítési csapatával. Ez csak akkor érvényes, ha a Nem lehetőséget választja a "Microsoft-segítségre van szükség? "|Yes
Megjegyzések a Microsofthoz|No|A Microsoftnak adott megjegyzések, ha segítségre van szüksége a Microsofttól|Segítségre van szüksége egy Contoso-ügyfél poC-hez?
Ügyfél-/partnerkapcsolat megosztásának beleegyezése|Yes|Járuljon hozzá az ügyfél kapcsolattartási adatainak és a céges alkalmazottak kapcsolattartási adatainak megosztásához, akik az ajánlaton dolgoznak. **Az ügyletek nem lesznek létrehozva vagy frissítve, ha ebben az oszlopban a Nem lehetőséget választja.** |Yes
1\. megoldás|Yes|Megoldásazonosító (kötelező), Az a pénznem (nem kötelező), amelyben az ajánlat értéke meg van adva. A pénznemkódokat [itt,](https://en.wikipedia.org/wiki/ISO_4217)a termékváltozat árát (nem kötelező) és a termékváltozat mennyiségét (nem kötelező) találja  |SOL-1234-PQRS, USD, 10, 100
1. csapattag|Yes|A megfelelő csapattag vezetékneve, vezetékneve, mobilszáma és e-mail-azonosítója.| Bob, Partner, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Következő lépések

Az ilyen összekötőket Partnerközpont együtt értékesítheti a Microsofttal az Ön CRM-rendszereiből.

- [Közös értékesítés összekötő a Dynamics 365 CRM-hez – Áttekintés](connector-dynamics.md)
- [Salesforce CRM-hez készült közös értékesítési összekötő – áttekintés](connector-salesforce.md)
