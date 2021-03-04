---
title: Tömeges műveletek Excel-fájlokon keresztül az átirányítási műveletekben
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan tölthet le, hozhat létre vagy frissíthet közös értékesítési lehetőségeket Excel-fájlok használatával
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: d601fec4bbdaad72f02c16b399cc320cc607d8ed
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756058"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-valuecsv-files"></a>Tömeges műveletek a vesszővel tagolt (CSV) fájlok használatával történő közös értékesítési lehetőségekhez

**Megfelelő szerepkörök**

- Ajánlói rendszergazda
- Hivatkozó felhasználók

A partner Centerben végzett tömeges műveletek segítenek a vállalatnak a közös értékesítési lehetőségek adatait exportálni és importálni. Navigáljon a közös értékesítési lehetőségek oldalára, ahol megtalálhatja az importálási és exportálási hivatkozásokat a lap cím szalagcímének jobb felső részén. Az **átirányítási** és a **hivatkozói felhasználói** engedélyekkel rendelkező felhasználók ezt a funkciót használhatják.

> [!IMPORTANT]
> A tömeges importáláson keresztül végzett létrehozási/frissítési műveletek nem vonhatók vissza. Ha nagy mennyiségű rekordot módosít vagy hoz létre, körültekintően járjon el. Egy üzlet létrehozása után csak a mezők egy részhalmazát lehet módosítani. **Egyetlen művelet sem lesz engedélyezve, ha bármely üzlet olyan terminál-állapotot ér el, mint a visszautasított/lejárt/megnyert/elveszett.**

## <a name="exporting-co-sell-opportunities"></a>Közös értékesítési lehetőségek exportálása

Alább láthatók az exportálási funkciók részletei

- Az Exportálás gombra kattintva **legfeljebb 5000 rekordot** lehet exportálni.
- A letöltött ajánlatok a hozzáférési szintek alapján lesznek elérhetők. Az átirányítási rendszergazdák és a hivatkozó felhasználók különböző eredményekhez juthatnak a hatókörük és a csoport tagjaiként való bevonásuk alapján. További információ az [átirányítási engedélyekről](permissions-overview.md#manage-referrals).
- Az exportálási függvény beolvassa a közös értékesítés lehetőségei lap aktuális lapját, valamint az alkalmazott szűrőket.
- A rendszer létrehoz egy CSV-fájlt, amely az alkalmazott szűrők alapján minden adattal rendelkezik.
- A rekordok letöltése akár egy percet is igénybe vehet.
- Nem kell megvárnia, amíg a letöltési művelet befejeződik. Még ha a partner Center más oldalaira is navigál, a fájl letöltése az exportálási funkció befejeződése után azonnal megtörténik.
- Újra felhasználhatja a letöltött fájlt, hogy módosítsa az ügylet részleteit, és feltöltse a rekordok frissítéséhez.

## <a name="importing-co-sell-opportunities"></a>Közös értékesítési lehetőségek importálása

- Az importálási funkcióval **legfeljebb 1000 rekordot** lehet létrehozni vagy frissíteni.
- A sablon létrehozásához töltse le a sablont az importálás lapról a partner Center webhelyen.
- Az exportálás funkció használatával letöltheti a meglévő rekordokat, és frissítheti azokat.
- Ha a fájl több mint 1000 rekordot tartalmaz, nem dolgozható fel.
- A fájl feldolgozása után a rendszer összefoglalja, hogy a létrehozott, frissített és nem feldolgozott hivatkozások száma megjelenik-e az utolsó folyamat-fájl kártyán.
- Letöltheti a feldolgozott rekordok részleteit, kijavíthatja a hibákat, és feltöltheti ugyanazt a fájlt az előző futtatás során meghiúsult rekordok létrehozásához vagy frissítéséhez. **Távolítsa el az összes sikeres rekordot a fájlból, mielőtt feltölti az előző futtatás során meghiúsult javított rekordokat.**
- További megoldások hozzáadásához vegyen fel további oszlopokat az 1. megoldás mellett, és használja az oszlop nevét X megoldásként, ahol az X az üzletben található megoldás számát jelöli. Példa: 2. megoldás, 3. megoldás.
- Akár 50 megoldást is hozzáadhat egy üzlethez.
- További csapattagok hozzáadásához vegyen fel további oszlopokat az 1. csoport mellé, és használja az oszlop nevét az X csapat tagjaként, ahol az X az üzletben lévő csapattagok számát jelöli. Például a 2. csapattag, a 3. csapat tagja.
- Akár 50 csapat tagjait is hozzáadhat egy üzlethez.

> [!NOTE]
> Nem kell megvárnia, amíg a feldolgozás befejeződik. Az utolsó feldolgozott fájl részletei a feldolgozás befejeződése után lesznek elérhetők a letöltéshez. **Ha 1000-rekorddal tölt fel fájlokat, akár 10 percet is igénybe vehet.**

> [!IMPORTANT]
> Olvassa el figyelmesen az összes utasítást, és tekintse meg az egyes oszlopok formátumát az alábbi táblázatból, mielőtt a partner Centerben CSV-fájlokat használó ajánlatokat hozna létre vagy frissít.

|**Oszlop neve**|**Kötelező?**|**Leírás**|**Minta értéke (i)**|
|-----|:-----|:---------|:---|
Hibák|Nem|Ebben az oszlopban hibák léptek fel, ha a létrehozási/frissítési műveletekhez kapcsolódóan a. r. t. t és az átirányítási műveletek is megjelennek. Ha több hiba van, mindegyiket pontosvesszővel elválasztva fogja megjelenni.|A kötelezően megadandó 1. megoldás hiányzik|
Engagement-azonosító|Nem|Az engagement-azonosítót a Microsoft partner Center Referrals rendszer hozza létre. Az új hivatkozó létrehozásához nem szükséges. Rekord frissítésekor használhatja a meglévő engagement-azonosítót.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Javaslatok azonosítója|Nem|Az átirányítási azonosítót a Microsoft partner Center átirányítási rendszere hozza létre. Az új hivatkozó létrehozásához nem szükséges. Ha meglévő rekordot frissít, töltse ki az átirányítási AZONOSÍTÓval.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Osztás neve|Igen|A hivatkozáshoz tartozó ajánlat rövid neve.|Egyesült Királyság tavaszi akciója
Ügyfél neve|Igen|Az ügyfél vállalatának neve. A Microsoft oldalának gyors megfeleltetéséhez használja a szervezet jogi nevét.|Contoso Corporation
Ügyfél címe 1. sor|Igen|Az ügyfél vállalatának 1. sora. |Egy contoso módszer
Ügyfél címe 2. sor|Nem|Az ügyfél vállalatánál 2. sor.|NE 148 utca
Customer City|Igen|Az a város, ahol az ügyfél szervezete található.|Redmond
Ügyfél állapota|Nem|Az az állapot, amelyben az ügyfél szervezete található.|Washington
Ügyfél postai irányítószáma|Nem|Azon régió irányítószáma, ahol az ügyfél szervezete található.|98052
Ügyfél országa|Igen|Az az ország/régió, ahol az ügyfél szervezete található. Használja az [itt]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)említett két betűs országkód-kódokat.|USA
Ügyfél – D-U-N-S azonosító|Nem|Próbálja meg beolvasni az ügyfél-szervezet DUNS-AZONOSÍTÓját. Ez segít az ügyfél-szervezet gyorsabb egyeztetésében a Microsoft oldalán, ami segít a gyorsabb eladó-hozzárendelésben. A jelen [webhelyről](https://www.dnb.com/duns-number/lookup.html)ingyenesen beszerezheti a Duns ID-t.|81466849
Ügyfél kapcsolattartójának keresztneve|Függ|Az utónév csak akkor kötelező, ha Microsoft súgóra van szüksége. Az ügyfél szervezete által az adott üzleten dolgozó elsődleges partner utóneve.|John
Ügyfél kapcsolattartójának vezetékneve|Függ|A vezetéknevet csak akkor kötelező megadni, ha Microsoft súgóra van szüksége. Az ügyfél-szervezetnél az adott üzletben dolgozó elsődleges partner vezetékneve.|Ügyfél
Ügyfél kapcsolattartási telefonszáma|Függ|A telefonszám csak akkor kötelező, ha Microsoft súgóra van szüksége. Az adott üzletben dolgozó, az ügyfél szervezete által használt elsődleges partner telefonszáma.|9999999999
Ügyfél kapcsolattartási e-mail-címe|Függ|Az e-mail-cím megadása csak akkor kötelező, ha Microsoft súgóra van szüksége. Az ügyfél munkahelyén dolgozó elsődleges partner e-mail-címe.|john.customer@contoso.com
Partneri hivatkozó állapota|Igen|A vállalat szemszögéből vonatkozó üzlet állapotát jelzi. Szükséges, ha egy hivatkozót próbál létrehozni vagy módosítani. Ha új üzletet próbál létrehozni, használja az **új** lehetőséget. Az elfogadott [értékek dokumentálva](/partner/develop/referral-resources#referralstatus)vannak.|Aktív
Partner átirányítási alállapota|Igen|Az üzlet pontos állapotát jelzi. Ha új üzletet próbál létrehozni, **fogadja el** a használatát. Akkor is szükség van rá, ha módosít egy meglévő átirányítást. Az elfogadott [értékek dokumentálva](/partner/develop/referral-resources#referralsubstatus)vannak.|Elfogadva
A Microsoft Referral állapota|Függ|Megadja a Microsoft segítségét kérő közös értékesítési kérelem állapotát. Ez egy írásvédett mező. A rendszer figyelmen kívül hagyja az adatimportálás során a mezőben történt módosításokat.| Függőben
Elutasított/elveszett ok|Függ| Ezeket az adatokat csak akkor kell megadnia, ha a mező alállapotát elutasította vagy elvesztettre módosítja. Ezt az oszlopot nem lehet figyelmen kívül hagyni. <br/> **Adjon meg egy számot az alábbi lehetőségek alapján** <br/><br/> **1**– a projekt költségvetése nem megfelelő  <br/> **2**– az ügyfél nem válaszolt  <br/> **3**– az ügyfél másik gyártót választott  <br/> **4** – nem teljesített ügyfél-követelmény  <br/> **5** – nem ügyfél <br/> **6**– a javasolt idővonal túl rövid volt <br/> **7** – visszaélésként, levélszemétként vagy adathalászatként való jelentés <br/> **8** – egyebek |6|
Értékesítési fázis|Nem|Ez a mező jelzi az átirányítás részletes értékesítési szakaszát. További információ az [értékesítési szakaszokról](./manage-co-sell-opportunities.md)|40
Becsült mennyiség értéke|Igen|"Az üzlet értéke az ügyféllel való kezdeti beszélgetések alapján. Ez csak akkor módosítható, ha az üzlet eléri az egyik terminál-állapotot| Megnyert vagy elveszett. "|12563
Pénznem|Igen|Az a pénznem, amelyben a rendszer megadta a Deal értéket. [Itt](https://en.wikipedia.org/wiki/ISO_4217)megtekintheti a pénznemkódot.|USD
Becsült záró dátum|Igen|Az ügylet becsült zárási dátuma az ügyféllel való kezdeti beszélgetések alapján hh/nn/éééé formátumban. <br/> **A dátumnak UTC időzónában kell lennie. A partner Center felhasználói felületén megjelenő dátumok a honosított időzónán alapulnak. A partneri központ felhasználói felületén +/-egynapos különbség lehet, ha azt az áttételt keresi, amelyhez az UTC időzónában megadott dátumot adta meg.**|1/30/2020
CRM-AZONOSÍTÓ|Nem|Az adott hivatkozás azonosítója a CRM-rendszerben, ha van ilyen. Ez egy ingyenes űrlap szöveges beviteli mező.|34234324-sdfsdf-345345-Evi
Marketingkampány azonosítója|Nem|Ebben a mezőben a marketing kampány látható, amely az adott átirányítást eredményezte. Általában a ROI számításához használatos|BingSummer2020
Jegyzetek|Nem|Az átirányítással kapcsolatos frissítéseket jelző részletes megjegyzések|Ez egy minta Megjegyzés
Microsoft Súgó szükséges?|Igen|Ezzel a beállítással jelezheti, hogy a Microsoft segíteni kíván-e a közös értékesítésre vonatkozó kérelem elvégzésében|Igen
Milyen konkrét segítséget nyújt a Microsoft?|Függ|A Microsoft által felhasználható hat különböző módszer egyike. Ez csak akkor alkalmazható, ha a nem lehetőséget választja a "Microsoft Súgó szükséges?" kérdésre? " <br/> **Adjon meg egy számot az alábbi lehetőségek alapján** <br/><br/> **1**– munkaterhelés-specifikus érték kiosztása  <br/> **2**– ügyfél-technikai architektúra  <br/> **3**– a koncepció/demo bizonyítása  <br/> **4**– idézőjelek és licencelés  <br/> **5**– értékesítés utáni ügyfél sikeressége  <br/> **6**– általános vagy egyéb|1|
Megosztás a Microsoft értékesítési csapatával|Igen|Ez azt jelzi, hogy meg kívánja-e osztani a Microsoft értékesítési csapatával való alku részleteit, vagy sem. Ez csak akkor alkalmazható, ha a nem lehetőséget választja a "Microsoft Súgó szükséges?" kérdésre? "|Igen
Megjegyzések a Microsoftnak|Nem|A Microsoftnak adott megjegyzések, ha segítségre van szüksége a Microsofttól|Segítségre van szüksége a contoso-ügyfélhez
Ügyfél/partner kapcsolat megosztásának beleegyezike|Igen|Az ügyfél kapcsolattartási adatainak és a vállalat alkalmazottainak megosztható kapcsolattartási adataival az üzleten dolgozik. **Az ajánlatok nem jönnek létre vagy nem frissülnek, ha a nem lehetőséget választja ehhez az oszlophoz.** |Igen
1\. megoldás|Igen|A megoldás azonosítója (kötelező), a pénznem (nem kötelező), amelyben az üzlet értékét megadta. [Itt](https://en.wikipedia.org/wiki/ISO_4217)megtalálhatja a pénznemkódot, a SKU árát (opcionális) és az SKU mennyiségét (nem kötelező)  |SOL-1234-PQRS, USD, 10, 100
1. csapat tagja|Igen|Az adott csapattag vezetékneve, vezetékneve, mobil száma és e-mail-azonosítója.| Bob, partner, 999999, Bob.partner@Contoso.com