---
title: Áttelepítés a Partner Sales Connectből (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan mikolhatja át a Microsoft-partnerek a Partner Sales Connect (PSC) Partnerközpont microsoftos értékesítők által küldött ügyleteket hozhatnak létre és kezelhet.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 584f8a7f2794cb64be49fe7f790904eff50c4c26
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855105"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Útmutató a Partner Sales Connectről (PSC) Partnerközpont (PC) származó partnerek közös értékesítéséhez

**Megfelelő szerepkörök:** Fiók-rendszergazdai | Ajánlói rendszergazdai | Partner Sales Connect (PSC) értékesítői | Partner Sales Connect (PSC) rendszergazdai | Partner Sales Connect (PSC) üzletvezető

Ez a cikk útmutatást nyújt a Partner Sales Connectből a Partnerközpont-be mirating partnerek számára, hogy továbbra is létrehozva és kezelve tudják kezelni az értékesítési Partnerközpont.

>[!Note]
> Ha azért van itt, mert szalagcímet látott a PSC-ről a migrálásról, jó helyen van. Ez az útmutató nem vonatkozik a megoldásértékelési (SA) és OEM-licencelési üzleti partnerekre, akik PSC-kkel kapcsolatos ügyleteiket kezelik.

>[!Important]
> 2021. április 1-től a vállalat nem hozhat létre és nem szerkeszthet ügyleteket a PSC-ben. **Továbbra is letöltheti a meglévő ügyleti adatokat a PSC tömeges exportálási képességével. Emellett a [PSC-ről is](psc-to-pc.md#psc-deals-migration) át lehet Partnerközpont ezt követően.** <br><br> Ha vannak olyan ügyletek, amelyeken aktívan dolgozik, és az IP-alapú közös értékesítésre alkalmas megoldásokat tartalmaznak, két lehetőség közül választhat: <br><br> 1. Az ajánlatot 2021. március 31. előtt jelölje meg megnyertként és teljes üzletregisztrációként a PSC-ben. <br> 2. [Az ügyleteket](psc-to-pc.md#psc-deals-migration) át kell Partnerközpont, hogy több ideje munkához jut a ügyleten és elkezdeni az ügylet regisztrációját.

Mint tudja, a vállalat **2021. április 30.** után elveszíti a PSC-hozzáférését. Azonban itt is megtalál mindent, amit el szeretne Partnerközpont, például közös értékesítést hozhat létre, kezelheti az ügyleteket, és a Microsoft értékesítői által elküldött ügyletekre is feltehet bizonyosokat.

Lesznek azonban különbségek. Az alábbi útmutató segítségével zökkenőmentesebb és egyszerűbben Partnerközpont a folyamatra való átállást.

## <a name="before-you-move-things-you-need-to-know"></a>Mielőtt továbblép, a szükséges dolgok

### <a name="if-you-are-a-psc-admin"></a>Ha Ön PSC-rendszergazda

- A szolgáltatásba való bejelentkezéshez munkahelyi [e-Partnerközpont.](https://partner.microsoft.com/)
- Állítsa be a fiókját a fiókadminisztr Partnerközpont [segítségével.](permissions-overview.md)
- Ebből a dokumentumból megtudhatja, hogyan értékesít Partnerközpont 2016.
- Állítson be felhasználói fiókokat a Partnerközpont PSC-felhasználók (Rendszergazda, Ajánlatkezelő és Értékesítő szerepkör) számára, és rendeljen hozzájuk [ajánlói rendszergazdai szerepköröket.](permissions-overview.md)

>[!IMPORTANT]
> Győződjön meg arról, hogy a PSC szalagcímen látható MPN-azonosító elérhető az MPN-helyek listájában a Partnerközpont.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="A PSC szalagcímet bemutató kép, ahol a partnerek megtalálják az MPN-azonosítót.":::

 Annak ellenőrzéséhez, hogy az MPN-azonosító mpN-helyként jelenik-e [](https://partner.microsoft.com/dashboard)meg, jelentkezzen be Partnerközpont a Partnerközpont-irányítópultra, majd válassza a Beállítások  (fogaskerék ikon) lehetőséget a képernyő jobb felső részén, majd a Fiókbeállítások **lehetőséget.** A második szintű, bal oldali navigációs  menüben válassza a Helyek lehetőséget a fiókhoz társított összes MPN-Partnerközpont és hely listájának.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Ha Ön PSC-üzletvezető vagy értékesítő

- Az irányítópultra való bejelentkezéshez munkahelyi e-Partnerközpont [szüksége.](https://partner.microsoft.com/dashboard)
- Ha nem munkahelyi fiókot használ a PSC-ben, vagy a munkahelyi e-mail-címe nem a partnervállalatnál van, forduljon a PSC-rendszergazdához a fiók beállításával kapcsolatban.
- Ellenőrizze a PSC-rendszergazdával, hogy Partnerközpont fiók beállítása befejeződött-e, függetlenül attól, hogy milyen fiókot használ a PSC-be való bejelentkezéshez.
- Ellenőrizze, hogy rendelkezik-e hozzáféréssel Partnerközpont és a Hivatkozások szakaszhoz.
- Olvassa el ezt a dokumentumot a munkafolyamatok és a változások Partnerközpont.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>A PSC rendszergazdájaként ezek a következő lépések

A bal Partnerközpont menüben válassza a **Hivatkozások** lehetőséget. Ellenőrizze, hogy hozzáfér-e a Hivatkozási oldalakhoz.

  >[!Note]
  > Előfordulhat, hogy ki kell jelentkeznie a Partnerközpont, majd újra be kell jelentkeznie a hitelesítő adatok frissítéshez a Hivatkozási lapokhoz való hozzáféréshez.

Ha nem látja a  Hivatkozások lehetőséget a Partnerközpont menüjében vagy a Hivatkozásokkal kapcsolatos oldalakon, lépjen kapcsolatba a cég fiókadminisztrátával, és kérje meg, hogy adjon hozzáférést a Hivatkozások lehetőséghez és a kapcsolódó területhez. [](permissions-overview.md) 

A céges fiókadminisztrát a következővel találhatja meg:

1. Válassza **a Fiókbeállítások** lehetőséget a jobb felső sarokban található fogaskerék ikonnal Partnerközpont irányítópulton.

1. A **bal oldali** navigációs menüben válassza a Felhasználókezelés lehetőséget.

1. A felhasználólista tetején válassza a Szűrő **legördülő** menüt. Módosítsa a beállítást **Fiók-rendszergazda beállításra.**

   A lapon megjelenik az összes fiók-rendszergazda a megfelelő e-mail-címmel. Küldje el e-mailben az egyiket, és kérje meg, hogy rendelje hozzá a ajánlói rendszergazdai szerepkört a munkahelyi fiókjához.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="A partnerbeállítások felhasználókezelési oldalán a fiók-rendszergazdákat bemutató kép.":::

>[!Important]
>- Ha a szerepköre csak a felhasználók PSC-ben való felügyeletét foglalja magában, kérje meg a vállalat fiókadminisztrátusát, hogy rendeljen Önnek fiókadminisztr Partnerközpont. [](permissions-overview.md#manage-mpn-membership-and-your-company) 
>- Ha a szerepköre magában foglalja az együttműködési lehetőségek felügyeletét is, kérje meg, hogy legyen hozzárendelve a [ajánlói rendszergazdai szerepkörhöz.](permissions-overview.md#manage-referrals)
> - A PSC-rendszergazdák között is jó ötlet egy változáskezelési vezetőt kijelölni. Ezzel megakadályozhatja, hogy minden PSC-rendszergazdának külön-külön el kell érnie Partnerközpont fiók rendszergazdáit. Ehelyett a változáskezelési vezető lehet az elsődleges személy, aki a fiók Partnerközpont dolgozik.

## <a name="user-migration"></a>Felhasználók migrálása

Miután beállította a fiókját az Partnerközpont-ban, az Együttműködési lehetőségek oldalon található felhasználóáttelepítési varázslóval automatikusan hozzárendelheti a Partnerközpont-szerepköröket a vállalat alkalmazottaihoz.

>[!Note]
> A felhasználóáttelepítést csak a vállalat [fiókadminisztrai](permissions-overview.md#manage-mpn-membership-and-your-company) hajthatja végre. Ha még nincs fiók-rendszergazdai szerepköre, a felhasználóáttelepítési varázsló segítségével keressen egy fiók-rendszergazdát, aki segíthet a felhasználói fiókok beállításában.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="A felhasználóáttelepítési varázslót bemutató kép.":::

A fiók rendszergazdái a PSC felhasználóáttelepítési varázsló hivatkozását látják az együttműködési lehetőségek oldalán a hivatkozások útmutatója mellett. A hivatkozásra kattintva kezdeményezhetik a felhasználó migrálását. A felhasználók migrálásának kezdeményezésére a rendszergazdák kiválaszthatják a hivatkozást. Ezt a felhasználóáttelepítési lépést többször is elvégezheti, amíg az összes felhasználóhoz hozzá nem rendelik a megfelelő szerepköröket a Partnerközpont.

A felhasználóáttelepítési táblázat a következő részleteket tartalmazza:

- Felhasználói fiók – Az alkalmazott e-mail-azonosítója
- PSC-partnerfiók – Az a fiók, amelyhez az alkalmazott társítva van a PSC-ban
- PSC felhasználói szerepkör – A PSC-hez rendelt három szerepkör egyike.
- PC MPN helye – Az a hely, ahol a felhasználó releváns számítógép-szerepköröket kap. A PSC-partnerfiók MPN-ével megkeresheti a megfelelő MPN-helyet a Partnerközpont engedélyek hozzárendelésére. A vOrg MPN-azonosítót a teljes szervezet jelöli.
- Pc-s felhasználói szerepkör – Az alkalmazottak a PSC felhasználói szerepköreik alapján vannak hozzárendelve. A PSC rendszergazdája a PC-n ajánlói rendszergazdai szerepköröket kap. Az értékesítő a PC-n a ajánlói felhasználói szerepkört fogja hozzárendelni. További információ a pc-szerepkörökről és arról, hogy az ezekkel a szerepkörökkel rendelkező felhasználók mire használhatjanak a Partnerközpontban [itt](permissions-overview.md#manage-referrals)
- PC AAD-bérlő – az a bérlő, amelyhez a felhasználók hozzá vannak rendelve a Partnerközpont
- Állapot – A migrálás állapotát három lehetséges állapot jelzi
    - **Nincs migrálva** – A felhasználóhoz nincs hozzárendelve számítógép-hivatkozási szerepkör
    - **Migrált** – A felhasználó migrálva lett, és a megfelelő szerepkör van hozzárendelve a táblázatban látható módon
    - **Hiba** – A migrálás valamilyen hiba miatt nem fejeződött be

Előfordulhat, hogy a migrálás sikertelen, és hibákat eredményezhet. Íme néhány ok, amiért a migrálás hibát okozhat, és néhány módszer a probléma megoldására:

1. Előfordulhat, hogy a PSC-felhasználók nem munkahelyi fiókot használnak.

2. Előfordulhat, hogy a PSC-felhasználó a fiókban használttól eltérő tartományból származó fiókot Partnerközpont.

   Az 1. és 2. forgatókönyvhöz kapcsolódó hibák elhárításához kérje meg a felhasználót, hogy jelentkezzen be Partnerközpont az Azure AD-bérlőhöz csatolt munkahelyi fiókjával. A [globális rendszergazda segíthet.](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles)
   
   A globális rendszergazda megkeresi: 
   - Jelentkezzen be a Partnerközpont [irányítópultra,](https://partner.microsoft.com/dashboard) és válassza a fiókbeállítások **lehetőséget** a jobb felső sarokban lévő fogaskerék ikonnal.
   - Válassza **a Felhasználókezelés** lehetőséget a második szintű, bal oldali navigációs sávon.
   - A felhasználói lista tetején válassza  a Szűrő legördülő menüt, és módosítsa a globális **rendszergazda lehetőséget.** Az oldal ezután megjeleníti az összes globális rendszergazdát a megfelelő e-mail-címekkel. Kérje meg az egyiket, hogy rendelje hozzá a munkahelyi fiókjához a ajánlói rendszergazdai szerepkört.
   
      A globális rendszergazda létrehozhat egy új felhasználói fiókot az Azure AD-bérlőben, vagy vendégfelhasználói hozzáférést rendelhet a tartományi fiók más felhasználóihoz. Miután beállította a fiókokat a PSC-üzletvezetők és -felhasználók számára, be  kell jelentkezniük az Partnerközpont-be, a bal oldali navigációs menüben válassza a Ajánlók lehetőséget, és ellenőrizze, hogy látják-e a Ajánlók oldalt.

3. A felhasználóhoz már hozzárendelt hivatkozási szerepkör van hozzárendelve a Partnerközpont.
    - Ellenőrizheti a felhasználó meglévő szerepkörét. A képernyő jobb felső sarkában Partnerközpont **a Beállítások** (fogaskerék ikon), majd a **Fiókbeállítások lehetőséget.** Amikor megjelenik egy második bal oldali navigációs menü, válassza a **Felhasználókezelés** lehetőséget, és keresse meg a felhasználót.

## <a name="psc-deals-migration"></a>PSC-ügyletek migrálása

Miután befejezte a felhasználóáttelepítést, az Együttműködési lehetőségek oldalon található ügylet-migrálási varázslóval átveszi a PSC-ről a PC-re az összes jogosult nyitott ügyletet. **Az ügyletek migrálási hivatkozása csak a teljes szervezeti hatókörrel felhozott javaslati rendszergazdák számára lesz látható Partnerközpont.** Az Együttműködési lehetőségek lap jobb felső oldalán található **"PSC- deal migration" (PSC-ajánlat áttelepítése)** hivatkozás, amely megnyitja az ajánlatáttelepítési varázslót.

Az ajánlat migrálásának megkezdése előtt olvassa el ezt a szakaszt.

**Jogosult a migrálásra**

Csak néhány ügylet jogosult a PSC-ről a PC-re való migrálásra. Ez a migrálási varázsló arra készült, hogy segítsen a partnereknek Partnerközpont ahol továbbra is aktívan dolgoznak az ügyfelekkel az ügylet lezárásán. **Csak a 2020. január 1-től nyílt állapotban létrehozott, érvényes partnerfiók-adatokkal (érvényes MPN-azonosítóval) létrehozott ügyletek jogosultak a migrálásra, az ügylet regisztrálása nem.**

**Nem jogosult migrálásra**

- A megoldásértékelési ajánlatok nem jogosultak az ügylet migrálásra
- Az OEM-licencelési üzleti ajánlatok nem jogosultak az ügylet migrálásra
- A PSC-ban megnyertként megjelölt bármely ajánlat nem migrálásra jogosult. Az ügyletregisztrációt, ha jogosult a megnyertként megjelölt ügyletekre, a PSC-ban kell végrehajtani.

## <a name="pre-requisites-for-deal-migration"></a>Az üzletbe való migrálás előfeltételei

Az ügylet PC-ről való migrálásának megkezdése előtt kövesse az alábbi utasításokat a PSC-ügyletek sikeres migráláshoz való beállításhoz.

1. Erről a migrálásról a vállalat összes értékesítési csapatának nyitott ügyleteken dolgozó tagja értesül.
2. Az értékesítési csapat tagjai arra vannak betanítva, hogy Partnerközpont az üzletkezeléshez.
3. Az ügylet tartalmazza az összes szükséges információt az alábbiakban leírtak szerint.
    - Az ügyfél céges adatai, beleértve a nevet és a címet
    - Az ügyfél kapcsolattartási adatai, ha közös értékesítésről van szó
    - Legalább egy megoldás
    - Legalább egy csapattag a részletekkel – vezetéknév, vezetéknév, e-mail-azonosító és telefonszám
    - Az üzlet értéke
    - Az üzletzárás becsült dátuma
    - Partneri megjegyzések

A PSC tömeges letöltési és feltöltési képességeivel az ügylet összes hiányzó részletét hozzáadhatja az összes jogosult ügylethez.

>[!Note]
> Az üzlet migrálása akkor is sikeres lesz, ha a fenti előfeltételek nem teljesülnek. Az üzlet állapotát azonban nem módosíthatja, ha a fent említett kötelező mezők bármelyike Partnerközpont nem érhető el. Ezután meg kell adnia az összes szükséges információt, amely hiányzik a Partnerközpont, hogy elkezdhet dolgozni velük. **Erősen ajánlott megtisztítani a PSC-re jogosult ügyleteket, mielőtt a Partnerközpont.**

Az üzlet migrálásának Partnerközpont egykattintásos folyamatként van felépítve. Ha a vállalata készen áll a jogosult ajánlatok milegályán, csak kattintson az **"Ügylet áttelepítése"** gombra. **Nem választhatja ki a PSC-ről átemelni kívánt ügyleteket. Ha nem szeretne átemelni egyetlen ügyletet sem a Partnerközpont, a migrálás megkezdése előtt helyezze át őket a PSC lezárt állapotába.**

>[!Note]
> A migrálás kezdeményezése után akár 24 órát is igénybe vehet, hogy az ügylet **migrálva legyen.**

A migrálás befejezése után a szalagcím-üzenet állapota a migrálási jelentésre mutató hivatkozással fejeződik be. Töltse le a jelentést a PSC-ről PC-re migrált ügyletek részleteinek megtekintéséhez.

A jelentés az alábbi adatokat tartalmazza.

1. **Partnerközpont-azonosító** – A Partnerközpont a kapcsolattartó összes ügyletének egyedi azonosítója. Két ügyletet kötünk – egyet a partnernek, egyet pedig a Microsoftnak egy közös értékesítésben a Partnerközpont.
2. **Partnerközpont hivatkozásazonosító** – A partnerhez tartozó Partnerközpont egyedi azonosítója a partnerhez tartozó üzletben.
3. **Az üzlet neve** – Az üzlet psc-hez megadott azonosítója.
4. **PSC-ajánlat azonosítója** – Az üzlet PSC-hez megadott egyedi azonosítója.
5. **Errors** (Hibák) – jelzi, hogy van-e hiba egy adott üzlet áttelepítése során.

A sikeresen migrált ügyletek nem lesznek láthatók a PSC-ben. Továbbra is dolgozhat a PC-n migrált ügyletekkel, beleértve az ügylet pc-n való regisztrációját is. Az együttműködési ügyletek microsoftos értékesítőivel való interakciók nem módosulnak.

A PSC-ről migrált ügyletek az ügylet forrása alapján a Bejövő és Kimenő lapokon lesznek elérhetők. A vállalat által megosztott összes ügylet elérhető lesz a Kimenő lapon, a Microsoft által kezdeményezett ügyletek pedig a bejövő Partnerközpont. A migrálás után kétféle ügylet jön létre.

1. **Közös értékesítés –** A PSC-ban közös értékesítésként megjelölt ügyletek a következőben fognak létrejönni: közös értékesítés az Partnerközpont.
2. **Partner által vezetett ügyletek** – Az együtt értékesítésként nem megjelölt ügyletek partner által irányított ügyletekként lesznek létrehozva a Partnerközpont. A partner által vezetett ügyletek láthatók a Microsoft értékesítői számára, és frissíthetőek közös értékesítésre, mielőtt elérné a terminálállapotot (megnyert, elveszett). A partner által vezetett ügyletek akkor is jogosultak az ügylet regisztrálásra, ha az ügyletben van ösztönzőre jogosult megoldás.

>[!Important]
> Ha olyan hiba történik, amely miatt egyes ügyleteket nem lehetett migrálni, az ügylet migrálását a **"Migrálási ügyletek"** gombra kattintva kezdeményezheti. Csak akkor lesz engedélyezve, ha még van néhány jogosult ügylet migrálva. Ez akkor is hasznos lehet, ha az áttérési fázisban néhány új ügylet jön létre a PSC-ban az ügylet migrálásának megkezdése után.

Az összes ügylet sikeres migrálása után egy **"No deals to migrate"** (Nincs migrálható ügylet) felirat jelenik meg, amely letiltja a **"Migrálható ügyletek"** **gombot.**

A felhasználók migrálásának és/vagy a migrálás végrehajtásához használja az alábbi útmutatót a migrálási stratégia eldöntésében:

Ha a vállalata partnerfejlesztési vezetővel (PDM) rendelkezik – Ha Partnerközpont-fiókja be van állítva, és a felhasználók átkerültek, és szerepkörökkel és engedélyekkel rendelkezik, áthelyezheti az értékesítési tevékenységeket a Partnerközpont. Tájékoztassa a PDM-et a váltásról ahelyett, hogy megvárja a migrálás befejezésének határidejét, ami lehetővé teszi, hogy az összes új ügylet a Partnerközpont.

>[!Note]
>A váltás után csak a PSC-hez kötött meglévő aktív ügyleteket tudja majd használni. Nem hozhat létre új ügyleteket, és nem fogadhat el semmilyen ügyletet a Microsoft értékesítőitől a PSC-ban.

Ha a vállalata nem áll a PDM-ben – Győződjön meg arról, hogy az összes felhasználó beállította és ellenőrizte az összes felhasználói fiókot. A PSC egy e-mailben és egy szalagcímen értesítést kap arról, hogy pontosan mikor kezdheti el az értékesítést a Partnerközpont. Ne feledje, hogy továbbra is kezelnie kell a PSC-hez már meglévő aktív ügyleteket.

>[!Important]
> 2021. április 30-ig regisztrálhatja a megnyertként megjelölt ügyleteket.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>A PSC-rendszergazdák, a PSC-üzletvezetők és a PSC-értékesítők következő lépései

Megtudhatja, hogyan értékesítsen együtt a Partnerközpont.
Ez egy fontos lépés, amely segít felkészülni a közös értékesítésre a Partnerközpont. A munkafolyamatok és a változások Partnerközpont, így azonnal hatékonyan együtt értékesíthet. Először olvassa el teljesen ezt a dokumentumot. Az Együttműködési élmény katalógusban is elérhető egy jó [erőforráskészlet.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-pc-workflows"></a>A PSC- és a PC-munkafolyamatok közötti főbb különbségek

|**Forgatókönyv**|**Partner Sales Connect**|**Partnerközpont**|
|-----|:-----|:-----|
|Felhasználói szerepkörök|A PSC rendszergazdai, üzletkezelői és értékesítői szerepkörökkel rendelkezik.|A PC-nek [csak olyan hivatkozási rendszergazdai](permissions-overview.md#manage-referrals) szerepköre van, amely olvasási és írási engedélyt is biztosít minden ügylethez.|
|A Microsoft meghívása egy közös értékesítésre|A Microsoft értékesítője kezdeményezte, a partner nem kér explicit kérdést.|A partnernek explicit kérést [kell tennie,](manage-co-sell-opportunities.md#add-solutions) ha egy Microsoft-értékesítői segítségre van szüksége egy adott ajánlathoz. A Microsoft Értékesítő elutasíthatja a kérelmet.|
|Lejárat|Az üzlet lejáratának nincs fogalma.|A partner bejövő ügyleti szerződése 14 nap múlva lejár, ha a partner nem fogadja el őket. Ugyanez vonatkozik a partnerek kimenő ügyletire is, amikor lejárt állapotba kerülnek, ha a Microsoft-értékesítő 14 napon belül nem foglalkozik velük.|
|A Microsoft értékesítőinek adatai|Azonnal látható, amint létrejön egy üzlet.|A Microsoft Értékesítő adatait csak akkor osztják meg a Partnerrel, ha az értékesítő elfogadja a partnertől származó közös értékesítésre vonatkozó meghívót.|
|[Privát folyamat](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Nem érhető el.|A partnerek megoszthatják a folyamatukat anélkül, hogy rálátást adnak a Microsoft értékesítőinek.|
|Megoldások|Az egy árlistához tartozó megoldások hozzáadhatóak az ajánlathoz.|A partnerek [az](manage-co-sell-opportunities.md#add-solutions) alábbi listákhoz tartozó megoldásokat adhatnak hozzá. a) Saját megoldások b) A Microsoft saját katalógusából származó megoldások (a PSC tranzakciós ügyleti szerepkörhöz hasonlóan) és c) más külső partnerektől származó közös értékesítésű megoldások (hasonlóan a PSC ISV Deal szerepkörhöz).|
|Ajánlat-hozzárendelés|Csak a hozzárendelt értékesítő megtekintheti az ügyleteket, és el is cselekedhet.|A csapattagok hozzáadhatóak az ügylethez, hogy megadják az ügyleten dolgozó személyeket. Ez nem gátolja meg, hogy más ajánlói rendszergazdák megtekintsék az ügyleteket, vagy azok alapján cselekednek.|
|Ügyfélszervezet|Szabad űrlap szövegbevitele.|Az ügyfél szervezetében [a](manage-co-sell-opportunities.md#select-your-customer) D&[B](https://www.dnb.com/) adatbázisban kereshet, ha csak begépel néhány karaktert. A rendszer automatikusan kitölti a jogi nevet és a címet a választás alapján.|
|Ügyfélkapcsolat|Nem kötelező.|Privát folyamatok megosztásához nem kötelező. Kötelező, ha a Microsoft értékesítője részt vesz egy közös értékesítésre vonatkozó kérelemben.|
|Nyilvános API|Nem érhető el.|[Nyilvános API](/partner/develop/referrals) a hivatkozások programozott Partnerközpont kezeléséhez.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>A PSC mezőinek leképezés a megfelelő mezőkre a Partnerközpont

Ez a szakasz összehasonlítja a PSC-hez látható kiválasztott képernyőképeket (vagy "térképeket") az Partnerközpont lehetőségek szakasz megfelelő nézetével.

Az egyes képernyőképpárok számokkal, sárga színekkel vagy piros színekkel ékesednek:

- **Mit jelentenek a sárga körök?** Minden PSC-képernyőképen először számokkal, sárga körök jelennek meg. Ezután egy olyan társalkalmazást Partnerközpont alatta, amely számos azonos számmal jelenik meg.

   Ha meg kell tudni, hogy a PSC minden mezője vagy attribútuma hogyan van megfeleltetve a megfelelőjüknek a Partnerközpont, akkor a két kapcsolódó képernyőképen egyezést kell látnia a számokkal összetört körökkel. Például az elsőben a számos, sárga "1" gombra, a PSC képernyőképen a másodikban a számmal és a sárga "1"-re, Partnerközpont alatta látható.

- **Mit jelent a piros kör?** Ha egy képernyőképen piros kör látható, az azt jelzi, hogy a PSC mező nem érhető el a Partnerközpont.

A PSC-Partnerközpont mezőleképezések a következő területekhez jelennek meg:

1. Az együttműködési lehetőségek alapértelmezett nézetében Partnerközpont lehetőségekhez hozzárendelt PSC-kezdőlap
1. A Partnerközpont nézetre leképezett PSC rácsnézet
1. A psc-üzlet részleteinek nézete, amely az Partnerközpont részletező nézetre van leképezve
1. A PSC Termékek hozzáadása nézete, amely a Partnerközpont megoldások hozzáadása nézetre van leképezve
1. A Felhasználókezelés nézetre leképezett PSC Partnerközpont nézet
1. A szerepkör-hozzárendelési nézetre leképezett PSC Partnerközpont szerepkör-hozzárendelési nézet
1. A nyilvános Partnerközpont nézetre leképezett PSC-értesítések nézet

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 – A psc kezdőlapja az Partnerközpont lehetőségek alapértelmezett nézetében

Hasonlítsa össze a PSC felső képernyőképe és az alatta lévő Partnerközpont köröket. Az egyező számok azt mutatják, hogy hol található a PSC-hez kapcsolódó szolgáltatás vagy Partnerközpont. A piros körök azt jelzik, hogy nincs Partnerközpont egyező mező.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="A Partner Sales Connect kezdőlapja és az értékesítési lehetőségek alapértelmezett nézete közötti mezőleképezéseket bemutató Partnerközpont." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 – A nyilvános Partnerközpont nézetre leképezett PSC rácsnézet

Hasonlítsa össze a PSC felső képernyőképe és az alatta lévő Partnerközpont köröket. Az egyező számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a Partnerközpont. A piros körök azt jelzik, hogy nincs Partnerközpont egyező mező.  

> [!NOTE]
> A képernyőképek alatt egyéb szempontok is megjelennek.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="A Partner Sales Connect (PSC) rácsnézet és az Partnerközpont mezőleképezését bemutató kép." lightbox="images/pscmigration/grid-view-expanded.png":::

**Speciális szempontok:**

- A PSC-hez Partnerközpont listanézet nincs.  Az összes ügylet a legutóbbi fogadott vagy létrehozott dátum alapján van felsorolva, az ügyfél adataival és az ügylet típusával együtt. Alapértelmezés szerint a nézet első üzlete van kiválasztva. A PSC táblaformátumban megjelenő értékek nagy része a PC-n az üzlet részletes nézetében érhető el.
- Az ajánlati szerepkör nem kötelező mező a PC-n. Egyik munkafolyamatban sem jelenik meg és nem rögzíti. A Microsoft értékesítői oldalán automatikusan lesz származtatva az üzlethez hozzáadott megoldások alapján.
- Az utolsó módosítás dátuma nem jelenik meg a PC-n a hivatkozás részleteit tartalmazó oldalon. A partnerek a rendezés funkcióval rendezheti az ügyleteket az utolsó frissítés dátuma alapján.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 – A PSC-ajánlat részleteinek nézete a Partnerközpont

Hasonlítsa össze a fenti (PSC) képernyőfelvételen található egyező, számokkal Partnerközpont köröket. Az egyező számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a Partnerközpont. A piros körök azt jelzik, hogy nincs egyező mező vagy terület a Partnerközpont.

> [!NOTE]
> A képernyőképek alatt egyéb szempontok is megjelennek.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="A Partner Sales Connect (PSC) deal details (Partner Sales Connect) és a Partnerközpont részletek nézete közötti mezőleképezéseket bemutató kép." lightbox="images/pscmigration/deal-details-expanded.png":::

**Különleges szempontok:**

- A partnerek a partneri ajánlat részletező nézetének Szerkesztés gombját választva szerkeszthetik az ajánlatot (6). A Szerkesztés gomb kiválasztása után az összes mező szerkeszthetővé válik. Ezután mentheti vagy megszakíthatja az üzleten történt módosításokat.
- Nincs lehetőség arra, hogy duplikáltként zárja be az ajánlatot a Partnerközpont.
- Az Ügyfél eredménye nem érhető el a Partnerközpont. Az ügyfél-interakciókra vonatkozó összes részlet frissíthető a PC Megjegyzések szakaszában.
- A megoldás becsült lejárati dátuma csak oem IOT-ügyletekhez érhető el a Partnerközpont. Ezek az információk nem jelennek meg más üzlettípusoknál.
- A számítógépen nincs szükség licencprogramra. Ez az információ automatikusan kikövetkeztetve lesz az ajánlatban kiválasztott megoldások alapján.

>[!Note]
>Az így megnyertként vagy elveszettként megjelölt dealek később nem szerkeszthetők. Körültekintően járjon el, amikor egy ajánlatot az alábbi terminál államok egyikében mozgat.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 – A PSC "Termékek hozzáadása" nézete, Partnerközpont "Megoldások hozzáadása" nézetre van leképezve

Hasonlítsa össze a fenti (PSC) képernyőfelvételen található egyező, számmal Partnerközpont köröket. Az egyező számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a Partnerközpont. A piros körök azt jelzik, hogy nincs egyező mező vagy terület a Partnerközpont.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Kép a Partner Sales Connect (PSC) termék hozzáadása nézete és a megoldás Partnerközpont mezőleképezései között." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 – Felhasználókezelés a PSC-ben és Partnerközpont

Hasonlítsa össze a fenti (PSC) képernyőfelvételen található egyező, számmal Partnerközpont köröket. Az egyező számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a Partnerközpont. A piros körök azt jelzik, hogy nincs egyező mező vagy terület a Partnerközpont.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="A Partner Sales Connect (PSC) felhasználókezelési kezdőlapja és a Partnerközpont Felhasználókezelés lap nézete közötti mezőleképezéseket bemutató kép a Fiókbeállítások területen."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 – Felhasználói szerepkör-hozzárendelés a PSC-ben és Partnerközpont

Hasonlítsa össze a fenti (PSC) képernyőfelvételen található egyező, számmal Partnerközpont köröket. Az egyező számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a Partnerközpont. A piros körök azt jelzik, hogy nincs egyező mező vagy terület a Partnerközpont.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="A Partner Sales Connect (PSC) szerepkör-hozzárendelési nézete és a szerepkör-hozzárendelési nézet Partnerközpont mezőleképezéseket bemutató kép." lightbox="images/pscmigration/roles-expanded.png":::

**Speciális szempontok:**

- A PSC-rendszergazda egyenértékű szerepköre a fiók rendszergazdai szerepköre a Partnerközpont.
- Az értékesítésben csak egy szerepkör Partnerközpont az értékesítések kezeléséhez. Ez a szerepkör a ajánlói rendszergazdai szerepkör.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 – Értesítések a PSC-ben és a Partnerközpont

Hasonlítsa össze a fenti (PSC) képernyőfelvételen található egyező, számokkal Partnerközpont köröket. Az egyező számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a Partnerközpont. A piros körök azt jelzik, hogy nincs egyező mező vagy terület a Partnerközpont.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="A Partner Sales Connect (PSC) értesítései és a Partnerközpont közötti leképezést bemutató kép."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Áthelyezés PSC-ről Partnerközpont - Gyakori kérdések

A következő szakaszok választ adnak a migrálásra vonatkozó gyakori kérdésekre.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 – Mit tegyek, ha nem tudok hozzáférni a Partnerközpont?

A szerepkörök hozzárendelését a "Nincs hozzáférés" oldalon felsorolt rendszergazdákhoz használhatja. A hivatkozások [](permissions-overview.md#manage-referrals) szakaszban olvasási és írási engedélyhez a ajánlói rendszergazdai szerepkörre lesz szüksége. Ha csak az üzleti profilokat kezeli, szüksége lesz az üzleti profil rendszergazdai szerepkörre a Partnerközpontban.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Kép a felhasználói élményről a Partnerközpont.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 – Ki adhat hozzáférést a Partnerközpont?

A [fiókadminisztrátor](permissions-overview.md#manage-mpn-membership-and-your-company) hozzáférést adhat a Hivatkozások laphoz. A fiókadminisztrát úgy találhatja meg, hogy a jobb felső sarokban lévő fogaskerék ikonon a Fiókbeállítások Partnerközpont [gombra.](https://partner.microsoft.com/dashboard)  Ezután válassza **a Felhasználókezelés** lehetőséget a második szintű, bal oldali navigációs sávon. A felhasználói lista tetején válassza  a Szűrő legördülő menüt, és módosítsa a fiókrendszergazdára.  A lapon megjelenik az összes fiók-rendszergazda a megfelelő e-mail-címmel. Kérje meg az egyiket, hogy rendelje hozzá a munkahelyi fiókjához a ajánlói rendszergazdai szerepkört.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 – A fiókhoz az +új üzlet gomb szürkével van kiszürkülve. Mit kell tennem az ügyletek létrehozásának elkezdenie?

Ez csak akkor fordul elő, ha nincsenek olyan, az MPN-szervezethez csatolt, közös értékesítésre kész megoldások, amelyek a Partnerközpont. Forduljon a PDM-hez a megoldások MPN-azonosítójának kijavítása érdekében, vagy hozzon létre egy támogatási jegyet, amely a következő problémát említi: "Az új ajánlat gomb szürkével ki van szürkülve a PSC-migrálás után."

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 – Hozzárendelhet-e ügyletet egy adott személyhez a szervezetből, például a PSC-hez?

A csapattagokat hozzárendelheti egy adott ajánlathoz. Nem tiltja le, hogy más ajánlási rendszergazdák megtekintsék ezeket az ügyleteket, vagy azok alapján cselekednek.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 – Van nézet az összes hozzárendelt ügyletről?

Használhatja a kedvencek funkciót, amely egy felhasználói szintű lap. Megjelölhet minden olyan ügyletet, amely kedvencként van kiosztva, így gyorsan hozzáférhet az ajánlatokhoz.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 – Van csak olvasható nézet az ügylethez?

Nem, a hivatkozások szakaszban nem látható az ajánlatok írásra vonatkozó nézete. Minden ajánlási rendszergazda teljes olvasási és írási hozzáféréssel rendelkezik az összes ügylethez.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 – Hogyan regisztrálok egy ajánlatot, miután megnyertként jelölem meg?

Ha az üzlet megfelel az alábbi feltételeknek, egy előugró ablak jelenik meg, amely elindítja az [ajánlat regisztrációját.](./register-deals.md)

- Az ajánlathoz egy ösztönzőnek megfelelő megoldás is csatolva van.
- A Microsoft értékesítője vagy meghívása az ajánlatban való részvételre.
- A Microsoft-kártya Elfogadva vagy Megnyerve állapotban van a Partnerközpont.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 – Hibaüzenetet kapok, amikor kiválasztom az "+Új ajánlat regisztrálása" gombot az Ajánlat regisztrálása szakaszban. Hogyan regisztrálom az ügyletemet?

Az **+Új** üzlet regisztrálása gombot csak azok a partnerek használják, akik regisztrálva vannak az ISV Connect programban egy olyan üzlet regisztrálása érdekében, amely nem kínál megfelelő Partnerközpont. Az együttműködési lehetőséggel kapcsolatos ügyletek regisztrálásakor előugró ablak jelenik meg, ha az ügyletet megnyertként jelöli meg, és megfelel az ügylet regisztrációja feltételeinek.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 – Kötelező az ügyfélszervezet hozzáadása?

Igen, az [ügyfélszervezet hozzáadása](./manage-co-sell-opportunities.md#select-your-customer) kötelező a Partnerközpont. Először is kezdje azzal, hogy rákeres arra a helyre, ahol az ügyfél található. A saját adatai alapján; Meg lehet adni pontosan az épület nevét, vagy csak meg kell adni a város adatait. A szervezeti keresés lekéri a megadott névnek megfelelő összes jogi személy adatait, így Önnek nem kell megadnia a címadatokat. A rendszer automatikusan kitölti az adatokat a kiválasztott szervezet alapján.

### <a name="10---are-customer-contact-details-mandatory"></a>10 – Kötelező az ügyfél kapcsolattartási adatai?

A [létrehozott üzlet](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) típusától függ. Ha csak megosztja a folyamatot, és nincs szüksége segítségre a Microsoft értékesítési szervezettől, dönthet úgy, hogy nem adja meg az ügyfél kapcsolattartási adatait. Ha olyan közös értékesítést használ, amelyben aktívan segítséget kér a Microsoft értékesítőjától, meg kell adnia az ügyfél kapcsolattartási adatait. Az ügyfél kifejezett beleegyezését kell kérnie, mielőtt közös értékesítésre vonatkozó kérelmet hoz létre a partnerközpontban.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 – Hány megoldást adhatok hozzá egy üzlethez?

Egy üzlethez akár 50 megoldást is hozzáadhat (a PSC-hez hasonló "termékekhez". A PSC-től eltérően vegyesen használhatja saját, közös értékesítésre jogosult megoldásait, a Microsoft első féltől származó termékkódokat és más, harmadik féltől származó, közös értékesítésre jogosult megoldásokat. A Partnerközpontban nincs kiválasztható vagy elérhető üzleti szerepkör. A Microsoft termékváltozatai esetén mennyiséget és árat is hozzáadhat az ajánlathoz hozzáadott minden egyes termékváltozathoz.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 – Mikor tudom meg a Microsoft értékesítőinek adatait az üzlet létrehozása után?

A Microsoft értékesítői csak akkor vannak kiosztva, ha pontosan megfeleltetve a Microsoft oldalán az adott értékesítő személyének az üzlet létrehozásakor a súgóra vonatkozó követelményt. A Microsoft értékesítői a hozzárendelést követően is elfogadják vagy elutasítják az együttműködési meghívót. Az ajánlatot csak akkor frissítjük a Microsoft értékesítői kapcsolattartási adataival, ha egy értékesítő elfogadta az értékesítésre vonatkozó meghívót. A Microsoft értékesítőinek az üzletre vonatkozó SLA 14 nap. Ez ugyanaz az SLA, mint amit a partnereknek el kell látnia, mielőtt lejárt állapotba kerül.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 – Hol található a lehetőségazonosító?

A PSC lehetőségazonosítója megegyezik a PC-n az ajánlatazonosítóval. Bármely üzlet megnyitásakor az üzlet neve mellett találja az üzletazonosítót.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14 – Hogyan férhet hozzá a PDM a pc-hez?

Partnerközpont a PDM-ek nem érhetik el közvetlenül a PSC-től eltérően. Ezt a képességet többféle módon is engedélyezheti, amelyekről alább olvashat.

- OCP-elemzések – Ha a PDM-ek csak a velük kapcsolatos ügyleteket és előrehaladást nézik meg, az OCP Insights portál használatával megtekinthetik a szervezet nézetét. Ez egy belső eszköz, és csak PDM-hez érhető el. Vegye figyelembe, hogy az OCP-elemzések nem érhetők el a vállalat felhasználói számára.
- Vendégfelhasználó a Partnerközpont – PDM-fiókját vendégfelhasználóként adhatja hozzá a partnerközpontban, és hozzárendelheti hozzájuk a hivatkozási rendszergazdai szerepkört, hogy megtekintse a hivatkozásokat, és az alapján @microsoft.com cselekedjen.
- Új [felhasználó](./create-user-accounts-and-set-permissions.md#add-a-new-user) létrehozása a bérlőben – Létrehozhat egy új felhasználót a saját bérlőjében, és megoszthatja ezeket az adatokat a PDM-ben, hogy megtekintse a fiókjában más ajánló felhasználókhoz hasonló hivatkozásokat, és az alapján cselekedjen.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>A helyes MPN-azonosító megkeresása, ha a PSC-fiók nincs érvényes MPN-hez társítva

Ha azért van itt, mert egy szalagcímet látott a PSC-ban, amely a "PSC érvénytelen MPN-azonosító társítási problémáját" említi, jó helyen van. Előfordulhat, hogy a fiókja érvénytelen MPN-azonosítóhoz lett kapcsolva a következő okok miatt

- A vállalata nem Partnerközpont fiókkal.
- A PDM hibát vétett a fiók MPN-azonosítójának a belső rendszerekben történő megadásakor, amelyek a PSC-fiókot a Partnerközpont (MPNID) fiókhoz csatolják.
- A vállalat nem fejeződött be a Partner Membership Center (PMC) számítógépről a számítógépre való migrálás során.

Először keresse meg a megfelelő MPN-azonosítót az alábbi lépésekben

- Jelentkezzen be Partnerközpont fiókjába
- Az MPN-azonosító megkereséhez használja [a](./partner-center-account-setup.md#locate-your-mpn-id) fiókbeállítások dokumentációjában található útmutatást.

Az alábbi képernyőképen a pontos hely látható, ahol az MPN-Partnerközpont található

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="A fiókbeállításokat bemutató kép, ahol a partner megtalálja az MPN-azonosítóját."  lightbox="images/pscmigration/findingMPNID.png":::

Next (Tovább)

- Ha PDM-et használ, kérje meg, hogy javítsa ki az MPN-azonosítót a partnerközpont fiókjából a megfelelő MPN-azonosítóval.
- Ha nem pdm-et használ, küldjön egy e-mailt a PSC szalagcímen megadott címre, a PSC-szalagcímben látható PSC-fiókinformációkkal és a partnerközpont fiókjából származó helyes MPN-azonosítóval.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Forrásforrások, amelyek segítségével létrehozhatja és kezelheti a Partnerközpont

Ha még nem elolvasta az értékesítéshez kapcsolódó súgótémakört, az alábbi forrásokkal kezelheti a partnerközpontban kötött ügyleteket.

|**Ehhez**   |**Olvassa el ezt**   |
|-----------------------|:-----------------------|
|Az együttműködési lehetőségek lapfülei és navigációs oldalának ismertetése|[Navigálás az együtt értékesítéssel kapcsolatos szakaszban](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Ügyfélszervezet kiválasztása a D&B listából |[Válassza ki az ügyfelet](./manage-co-sell-opportunities.md#select-your-customer)|
|Az üzlet részletei szakaszban található mezők módosítása|[Az üzlet részletei](./manage-co-sell-opportunities.md#deal-details)|
|A csapattagok hozzáadása egy ajánlatcsapathoz|[Alkalmazottak hozzáadása](./manage-co-sell-opportunities.md#add-team-members)|
|Reagálás egy közös értékesítésre|[Társadékalékok kezelése](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|A következőben megnyert ügyletek regisztrálása Partnerközpont |[Új ajánlat regisztrálása](./register-deals.md)
|Hivatkozási elemzések lekért és a hivatkozások útjára vonatkozó információk |[Javaslatelemzések](./referral-insights.md)
|Üzleti profil létrehozása és kezelése|[Üzleti profil kezelése](./create-a-marketing-profile.md)
|Érdeklődők kezelése az üzleti profilhoz |[Érdeklődők kezelése](./manage-leads.md)|

## <a name="next-steps"></a>Következő lépések


- [Partner Sales Connect egy Partnerközpont munkafüzethez](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) – munkafüzet, amely a partnerek értékesítési folyamatait és szerepköreit az új értékesítési folyamatokhoz igazítja a Partnerközpont és a Partner Sales Connect segítségével.
- [Partnerközpont üzemeltetési](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) útmutató – útmutató egy üzemeltetési modell Partnerközpont az érdeklődők vagy az együttműködési lehetőségek kezeléséhez és az ügyletek regisztrálása érdekében.
- [Ajánláskezelési pakli](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) – részletes vizualizációval szemléltetett utasítás az érdeklődők és az együttműködési lehetőségek kezeléséhez a Partnerközpont.
- [Közzététel és kezelés](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) a kereskedelmi piactéren – részletesen ábrázolt utasítás az ajánlatok létrehozásához, kezeléséhez és közzétételéhez Partnerközpont kereskedelmi piactéren.