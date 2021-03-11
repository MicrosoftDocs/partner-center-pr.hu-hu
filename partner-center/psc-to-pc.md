---
title: Áttelepítés partner Sales-kapcsolatról (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy a Microsoft-partnerek hogyan telepíthetik át a partneri értékesítési összekötőt a partneri központba, és hogyan hozhatók létre vagy kezelhetők a Microsoft-értékesítők
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: adbe4bf9fd329f7443608dd1a1e123208212ef43
ms.sourcegitcommit: 26095af7950817099764bf47370cb3e77e0dce7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "102770274"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Útmutató a partneri értékesítési kapcsolódásról (PSC) áthelyezett partneri központhoz (számítógép) való közös értékesítéshez

**Megfelelő szerepkörök**

- Fiókadminisztrátor
- Ajánlói rendszergazda
- Partner Sales-csatlakozási (PSC) értékesítő
- Partner Sales csatlakozási (PSC) rendszergazda
- Partner Sales csatlakozási (PSC) Deal Manager

Ez a cikk útmutatást nyújt a partneri értékesítési partnerektől a partneri központhoz való áttelepítéshez, így továbbra is létrehozhatnak és kezelhetnek közös értékesítési ajánlatokat a partner Centerben.

>[!Note]
> Ha azért van itt, mert az áttelepítéssel kapcsolatban egy, a PSC-ben megjelenő szalagcím található, akkor Ön a megfelelő helyen található. Ez az útmutató nem alkalmazható a megoldás-értékelési (SA) és az OEM licencelési üzleti partnerek számára, akik a PSC-ben lévő ügyleteket kezelik.

>[!Important]
> 2021. április 1-től a vállalat nem tudja létrehozni vagy szerkeszteni a PSC-t. **A meglévő ajánlatok adatai továbbra is letölthetők a PSC tömeges exportálási funkciójával. Ezen dátum után a PSC-ről a partneri központba is [áttelepítheti a nyitott ajánlatokat](psc-to-pc.md#psc-deals-migration) .** <br><br> Ha vannak olyan ügyletek, amelyekben aktívan dolgozik, és az IP-címek közös értékesítését ösztönző megoldásokat tartalmaz, két lehetőség közül választhat: <br><br> 1. adja meg az ügyletet megnyertként, és fejezze be az ügylet regisztrációját a PSC-ben, a 2021 március 31-ig. <br> 2. [telepítse át az ajánlatokat](psc-to-pc.md#psc-deals-migration) a partneri központba, így több időt kell igénybe vennie a Deal és a Deal regisztráció megkezdéséhez.

Amint tudja, a **vállalat a 2021. április 30-ig elveszíti a PSC-hez való hozzáférést**. Azonban továbbra is mindent megtalál, amit szeretne tenni a partner Centerben, mint például a közös értékesítési ajánlatok létrehozása, az ajánlatok kezelése és a Microsoft-értékesítők által eljuttatott ajánlatok.

Azonban eltérőek lesznek. A következő útmutató segítséget nyújt a partneri központ gördülékenyebb és egyszerűbb átállásához.

## <a name="before-you-move-things-you-need-to-know"></a>Mielőtt továbblép, meg kell ismernie a szükséges dolgokat

### <a name="if-you-are-a-psc-admin"></a>Ha Ön PSC-rendszergazda

- A [partner központba](https://partner.microsoft.com/)való bejelentkezéshez munkahelyi e-mailre van szükség.
- Állítsa be a fiókját a partner Center- [fiók rendszergazdája](permissions-overview.md)segítségével.
- A jelen dokumentum elolvasásával megtudhatja, hogyan értékesítheti a partner Centerben.
- Hozzon létre felhasználói fiókokat a partner Centerben az összes PSC-felhasználóhoz (rendszergazdai, Deal Manager-és eladói szerepkörök), és rendelje hozzá az [Ajánlói rendszergazdai szerepköröket](permissions-overview.md).

>[!IMPORTANT]
> Győződjön meg arról, hogy a PSC-szalagcímben látható MPN-azonosító elérhető a fiókpartner MPN-helyeinek listájában.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="A PSC-bannert bemutató kép, amelyben a partnerek megtalálják az MPN-azonosítót.":::

 Annak ellenőrzéséhez, hogy az MPN-azonosító fiókpartner-helyként jelenik-e meg, jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard), majd válassza a **Beállítások** (a fogaskerék ikon) lehetőséget a képernyő jobb felső részén, majd a **Fiókbeállítások** menüpontot. A második szint bal oldali navigációs menüjében válassza a **helyszínek** elemet a partner Center-fiókhoz társított MPN-azonosítók és-helyszínek listájának megtekintéséhez.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Ha Ön a PSC Deal Manager vagy az értékesítő

- A partner Center [irányítópultra](https://partner.microsoft.com/dashboard)való bejelentkezéshez szüksége van egy munkahelyi e-mailre.
- Ha nem munkahelyi fiókot használ a PSC-ben, vagy a munkahelyi e-mail-címe egy másik cég, mint a partner vállalat, forduljon a PSC rendszergazdához a fiók beállítása című súgóban.
- Forduljon a PSC rendszergazdájához, ha a partner Center-fiók beállítása a PSC-be való bejelentkezéshez használt fióktól függetlenül befejeződött.
- Ellenőrizze, hogy rendelkezik-e hozzáféréssel a partner központhoz és az átirányítási szakaszhoz.
- Olvassa el ezt a dokumentumot a munkafolyamatok és a partneri központ változásainak megismeréséhez.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>A PSC-ben rendszergazdaként ezek a következő lépések

A partneri központ bal oldali navigációs menüjében válassza az **átirányítási** lehetőséget. Erősítse meg, hogy hozzáfér az átirányítási lapokhoz.

  >[!Note]
  > Előfordulhat, hogy ki kell jelentkeznie a partneri központból, és újra be kell jelentkeznie, hogy frissítse a hitelesítő adatait az átirányítási lapokhoz való hozzáféréshez.

Ha nem látja az **átirányítási** lehetőséget a partner Center menüjében vagy az átirányítással kapcsolatos lapokon, lépjen kapcsolatba a vállalati [fiók rendszergazdájával](permissions-overview.md) , és kérje meg őket, hogy hozzáférést biztosítson az **átirányítási** lehetőségek és a kapcsolódó területek számára.

A vállalati fiók rendszergazdájának megkeresése:

1. Válassza ki a **Fiókbeállítások** elemet a központ irányítópultjának jobb felső sarkában található fogaskerék ikonra kattintva.

1. A második szintű, bal oldali navigációs menüből válassza a **felhasználói kezelés** lehetőséget.

1. A felhasználók listájának tetején válassza a **szűrő** legördülő menüt. Módosítsa a **fiók rendszergazdája** beállítást.

   A lap megjeleníti az összes fiók rendszergazdáját a hozzájuk tartozó e-mail-címükkel. Küldje el az egyiket, és kérje meg őket, hogy rendelje hozzá az Ajánlói rendszergazdai szerepkört a munkahelyi fiókjához.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="A partner-beállítások felhasználói kezelés lapján található fiók-rendszergazdákat bemutató kép.":::

>[!Important]
>- Ha a szerepkör csak a PSC-felhasználók felügyeletét foglalja magában, kérje meg a vállalat fiókjának rendszergazdáját, hogy rendelje hozzá a [fiók rendszergazdai](permissions-overview.md#manage-mpn-membership-and-your-company) szerepkörét a partner Centerben. 
>- Ha a szerepköre magában foglalja a közös értékesítési lehetőségek kezelését is, kérje meg, hogy rendelje hozzá az [Ajánlói rendszergazdai](permissions-overview.md#manage-referrals) szerepkört.
> - Érdemes kinevezni egy módosítási kezelési érdeklődőt is a PSC-rendszergazdák közé. Ezzel megakadályozza, hogy az összes PSC-rendszergazda külön-külön elérje a partner Center-fiók rendszergazdáit. Ehelyett a Change Management vezető a partner Center-fiók rendszergazdájával dolgozó elsődleges személy lehet.

## <a name="user-migration"></a>Felhasználói áttelepítés

Miután beállította a fiókját a partner Centerben, a közös értékesítési lehetőségek lapon a felhasználói áttelepítési varázsló használatával automatikusan hozzárendelheti a partner Center-szerepköröket a vállalat alkalmazottaihoz.

>[!Note]
> A felhasználók áttelepítését csak a vállalata [fiók-rendszergazdái](permissions-overview.md#manage-mpn-membership-and-your-company) tudják elvégezni. Ha nem rendelkezik fiók-rendszergazdai szerepkörrel, keresse meg a fiók rendszergazdáját, aki segítségére lehet a felhasználói fiókok beállításában a felhasználói áttelepítési varázsló segítségével.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="A felhasználó áttelepítési varázslóját ábrázoló kép.":::

A fiókok rendszergazdái a PSC felhasználói áttelepítési varázsló hivatkozását fogják látni az átirányítási útmutató melletti közös értékesítési lehetőségek lapon. A hivatkozásra kattintva elindíthatják a felhasználók áttelepítését. A felhasználók áttelepítésének elindításához a rendszergazdák kiválaszthatják a hivatkozást. Ezt a felhasználói áttelepítési lépést többször is elvégezhetik, amíg minden felhasználó hozzá nem rendeli a megfelelő szerepköröket a partner Centerben.

A felhasználó áttelepítési táblája a következő adatokat tartalmazza:

- Felhasználói fiók – az alkalmazott E-mail azonosítója
- PSC-partner fiók – az a fiók, amelyhez az alkalmazott társítva van a PSC-ben
- PSC felhasználói szerepkör – a PSC-ben hozzárendelt három szerepkör egyike.
- SZÁMÍTÓGÉP MPN-helye – az a hely, amelyhez a felhasználó megkapja a megfelelő számítógép-szerepköröket. A PSC fiókpartner MPN a fiókpartner megfelelő MPN-helyének megkeresésére szolgál az engedélyek kiosztásához. A teljes szervezet a vOrg MPN-azonosítót jelöli.
- SZÁMÍTÓGÉP-felhasználói szerepkör – az alkalmazottak PSC felhasználói szerepköreik alapján rendelnek hozzá szerepköröket. A PSC-ben a rendszergazda az Ajánlói rendszergazdai szerepköröket rendeli hozzá a SZÁMÍTÓGÉPekhez. Az értékesítőhöz az átirányítási felhasználói szerepkör lesz hozzárendelve a PC-n. További információ a számítógép-szerepkörökről, valamint arról, hogy az ezekkel a szerepkörökkel rendelkező felhasználók milyen műveleteket végezhetnek a [partner Centerben](permissions-overview.md#manage-referrals)
- PC HRE-bérlő – az a bérlő, amelyhez a felhasználók hozzá vannak rendelve a partner Centerben
- Állapot – az áttelepítés állapotának három lehetséges állapota van
    - **Nincs áttelepítve** – a felhasználónak nincs hozzárendelve számítógép-átirányítási szerepköre
    - **Migrált** – a rendszer sikeresen áttelepítette a felhasználót a táblázatban látható módon hozzárendelt megfelelő szerepkörrel.
    - **Hiba** – egy hiba miatt nem lehet befejezni az áttelepítést

Időnként előfordulhat, hogy az áttelepítés meghiúsul, és hibákat eredményezhet. Íme néhány ok, amiért az áttelepítés hibát okozhat, és néhány módszer a probléma megoldására:

1. A PSC-felhasználók nem munkahelyi fiókot is használhatnak.

2. Előfordulhat, hogy a PSC-felhasználó olyan tartományból származó fiókot használ, amely eltér a partner Centerben használttól.

   Az 1. és a 2. forgatókönyvekkel kapcsolatos hibák elhárításához kérje meg a felhasználót, hogy jelentkezzen be a Partnervállalatba az Azure AD-bérlőhöz csatlakoztatott munkahelyi fiókjával. A [globális rendszergazda](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) segítséget nyújthat.
   
   A globális rendszergazda megkeresése: 
   - Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard) , és válassza a **Fiókbeállítások** lehetőséget a jobb felső sarokban található fogaskerék ikonra.
   - A második szintű, bal oldali navigációs sávon válassza a **felhasználói kezelés** lehetőséget.
   - A felhasználók listájának tetején válassza a **szűrő** legördülő menüt, és módosítsa a **globális rendszergazda** beállítást. A lap ezután megjeleníti az összes globális rendszergazdát a megfelelő e-mail-címükkel. Kérje meg az egyiket, hogy rendelje hozzá az Ajánlói rendszergazdai szerepkört a munkahelyi fiókjához.
   
      A globális rendszergazda létrehozhat egy új felhasználói fiókot az Azure AD-bérlőben, vagy hozzárendelheti a vendég felhasználói hozzáférését a többi tartományi fiók felhasználóinak. Miután a fiókok be lettek állítva az összes PSC Deal Managerhez és felhasználóhoz, be kell jelentkezniük a partner központba, a bal oldali navigációs menüből válassza a **hivatkozók** lehetőséget, és erősítse meg, hogy láthatják az átirányítási lapokat.

3. A felhasználónak már van hozzárendelve egy átirányítási szerepkör a partner Centerben.
    - Ellenőrizheti a felhasználó meglévő szerepkörét. A partner központ jobb felső sarkában válassza a **Beállítások** (a fogaskerék ikon), majd a **Fiókbeállítások** lehetőséget. Amikor megjelenik a bal oldali navigációs menü, válassza a **felhasználók kezelése** lehetőséget, és keresse meg a felhasználót.

## <a name="psc-deals-migration"></a>A PSC-ajánlatok migrálása

A felhasználók áttelepítésének befejezése után a közös értékesítés lehetőségei lapon a Deals Migration (ajánlatok áttelepítése) varázslót használhatja a PSC-ről a számítógépre irányuló összes jogosult nyitott ajánlat létrehozásához. **A Deals áttelepítési hivatkozás csak a teljes szervezeti hatókörrel rendelkező hivatkozó rendszergazdák számára lesz látható a partner Centerben.** A közös értékesítési lehetőségek oldal jobb felső sarkában a **"PSC Deal Migration"** nevű hivatkozás jelenik meg, amely megnyitja az üzlet áttelepítési varázslóját.

Az ügylet áttelepítésének megkezdése előtt olvassa el ezt a szakaszt.

**Áttelepítésre jogosult**

Csak néhány ajánlat jogosult a PSC-ről a PC-re való áttelepítésre. Ez az áttelepítési varázsló úgy van felépítve, hogy segítse a partnereket abban, hogy az üzletük lezárásához aktívan használják a partneri központot. **Csak a nyílt állapotú, az 2020-as és az érvényes partneri fiók részleteivel (érvényes MPN-AZONOSÍTÓval) létrehozott, de nem az ügyletekhez való regisztrációra jogosult ügyletek telepíthetők.**

**Nem jogosult az áttelepítésre**

- A megoldás-értékelési ajánlatok nem jogosultak az üzlet áttelepítésére
- Az OEM licencelési üzleti ajánlatok nem jogosultak az üzlet áttelepítésére
- A PSC-ben megnyertként megjelölt összes ügylet nem jogosult az áttelepítésre. Az ügylet regisztrálása, ha jogosult a megnyertként megjelölt ajánlatokra, a PSC-ben kell befejezni.

## <a name="pre-requisites-for-deal-migration"></a>Az üzlet áttelepítéséhez szükséges előfeltételek

Mielőtt elindítja az ügylet áttelepítését a SZÁMÍTÓGÉPRŐL, kövesse az alábbi utasításokat a PSC-beli ajánlatok sikeres áttelepítéshez való beállításához.

1. A vállalaton belül a nyitott ajánlatokon dolgozó összes értékesítési csapat tagja tájékoztatja erről az áttelepítésről.
2. A Sales csapat tagjai a partner Center for Deal-felügyelet használatára vannak kiképezve.
3. Az ajánlatok az alább leírtak szerint rendelkeznek az összes szükséges információval.
    - Az ügyfél vállalatának adatai, beleértve a nevet és a címeket
    - Az ügyfél elérhetőségi adatai, ha közös értékesítéssel foglalkoznak
    - Legalább egy megoldás
    - Legalább egy csapattag az összes adattal: Utónév, vezetéknév, e-mail azonosító és telefonszám
    - Ügylet értéke
    - Becsült mennyiség záró dátuma
    - Partneri megjegyzések

A PSC tömeges letöltés és feltöltés funkciója segítségével hozzáadhatja az összes hiányzó részletet az üzletben az összes jogosult ajánlathoz.

>[!Note]
> Az üzlet áttelepítése akkor is sikeres lesz, ha a fenti előfeltételek nem teljesülnek. Az ügylet állapota azonban nem módosítható, ha a fentiekben említett kötelező mezők bármelyike nem érhető el a partner Centerben. Ezután meg kell adnia az összes szükséges információt a partner Centerben, hogy megkezdje a munkát. **Nyomatékosan javasoljuk, hogy a PSC-re való Migrálás előtt tisztítsa meg a jogosult ajánlatokat a partneri központba.**

A partner Centerben a Deal Migrálás Egy kattintásos élményre épül. Mindössze annyit kell tennie, hogy az **"ajánlatok áttelepítésére"** gombra kattint, miután a vállalat készen áll a jogosult ajánlatok áttelepítésére. **A PSC-ből áttelepíteni kívánt ajánlatokat nem választhatja ki. Ha nem szeretne áttelepíteni semmilyen ajánlatot a partneri központba, az áttelepítés megkezdése előtt helyezze át őket a PSC-ben lezárt állapotba.**

>[!Note]
> Az áttelepítés megkezdése után **akár 24 óráig is eltarthat, amíg a rendszer áttelepíti az ajánlatokat**.

Az áttelepítés befejezését követően a szalagcím üzenet állapota módosul, és az áttelepítési jelentésre mutató hivatkozás is megjelenik. Töltse le a jelentést, és tekintse meg a PSC-ről a számítógépre migrált ajánlatok részleteit.

A jelentés az alábbi részleteket tartalmazza.

1. A **partner Center ENGAGEMENT azonosítója** – a partneri központban lévő egyedi azonosító a engagement összes ajánlata esetében. A partner Centerben két üzlet létezik – egyet a partnerhez, egyet a Microsofthoz.
2. A partneri **központ hivatkozási azonosítója** – a partner központ egyedi azonosítója a partnerhez tartozó üzlethez.
3. A PSC-ben lévő üzlet **neve** – azonosító.
4. **PSC Deal ID** – az üzlethez tartozó PSC egyedi azonosítója.
5. **Hibák** – jelezheti, hogy hiba történt egy adott üzlet áttelepítése során.

Az összes sikeresen áttelepített ajánlat nem lesz látható a PSC-ben. Továbbra is dolgozhat az áttelepített ügyleteken a SZÁMÍTÓGÉPeken, beleértve az üzlet regisztrációjának befejezését a számítógépen. A közös értékesítéssel foglalkozó Microsoft-értékesítők közötti interakciók nem változnak.

A PSC-ről áttelepített ajánlatok a bejövő és kimenő lapokon lesznek elérhetők az üzlet forrása alapján. A vállalat által megosztott összes ügylet elérhető lesz a kimenő lapon, a Microsoft által kezdeményezett ajánlatok pedig a partner központ bejövő lapján lesznek elérhetők. A Migrálás után két típusú ügylet lesz létrehozva.

1. **Közös értékesítéssel** foglalkozó ajánlatok – a PSC-ben közös értékesítésre jelölt ajánlatok a partnervállalat közös értékesítéssel foglalkozó ajánlatával lesznek létrehozva.
2. **Partner által vezetett ajánlatok** – a partner-központba nem kerülő partnerek által vezetett ajánlatokként létrehozott ajánlatok. A partner által vezetett ajánlatok láthatók a Microsoft-értékesítők számára, és a terminál állapotának (megnyert, elveszett) elérése előtt is frissíthetők a közös értékesítési ajánlatokra. Emellett a partner által vezetett ügyletek is jogosultak az ügyletekre, ha az üzletben ösztönző jogosult megoldás van.

>[!Important]
> Ha olyan hibák merülnek fel, amelyek miatt egyes ajánlatok nem telepíthetők át, **akkor az ügylet áttelepítése gombra kattintva újra elindíthatja az üzlet áttelepítését**. A szolgáltatás csak akkor lesz engedélyezve, ha van még egy jogosult ügylet, amely még nem telepíthető át. Ez abban az esetben is hasznos lehet, ha olyan átmeneti fázisban van, ahol az üzlet áttelepítése után a PSC-ben egyre több új ajánlat jön létre.

Ha az összes ajánlat sikeresen át lett telepítve, akkor a " **nincsenek áttelepíthető ajánlatok** " felirat jelenik meg a **letiltott** **"ajánlatok átmigrálása"** gombbal.

A felhasználók migrálása és/vagy a Migrálás befejezése után az alábbi útmutatást követve döntse el az áttelepítési stratégiát:

Ha a vállalata rendelkezik egy partner Development Managerrel (PDM) – Ha a partner Center-fiókja be van állítva, és a felhasználók áthelyezték a szerepköröket és engedélyeket, áthelyezheti a közös értékesítési tevékenységeket a partner központba. Tájékoztassa a PDM, hogy ne várjon, amíg az áttelepítés befejeződik, és így az összes új ügylet a fiókpartner-központba kerül.

>[!Note]
>Ha elvégezte ezt a kapcsolót, akkor csak a PSC meglévő aktív ajánlatait fogja tudni fellépni. Nem hozhat létre új ajánlatokat, és nem kap ajánlatokat a Microsoft-értékesítők által a PSC-ben.

Ha a vállalat nem rendelkezik PDM – győződjön meg arról, hogy az összes felhasználói fiók be van állítva és ellenőrizhető az összes felhasználó számára. A rendszer e-mailben és egy, a PSC-n lévő szalagcímben értesíti a pontos dátumról, amikor a partner Centerben megkezdi a közös értékesítést. Ne feledje, hogy továbbra is a PSC-ben meglévő aktív ajánlatokat kell kezelnie.

>[!Important]
> A megnyertként megjelölt ajánlatokat a 2021. április 30-ig kell regisztrálni.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>A PSC-rendszergazdák, a PSC Deal managerek és a PSC-értékesítők következő lépései

Ismerje meg, hogyan értékesítheti közösen a partner centert.
Ez egy fontos lépés, amelynek segítségével előkészítheti a partneri központ közös értékesítését. Ismerje meg a munkafolyamatokat és a partneri központban bekövetkező változásokat, hogy azonnal együtt lehessen értékesíteni. Első lépésként olvassa el a dokumentumot teljesen. Egy jó készlet is elérhető a [közös értékesítés élmény](https://aka.ms/cosellexperience)-katalógusában.

## <a name="major-differences-between-psc-and-pc-workflows"></a>Fő különbségek a PSC és a PC-munkafolyamatok között

|**Forgatókönyv**|**Partner Sales-kapcsolat**|**Partnerközpont**|
|-----|:-----|:-----|
|Felhasználói szerepkörök|A PSC rendszergazdai, Deal Manager-és eladói szerepkörökkel rendelkezik.|A SZÁMÍTÓGÉPnek csak a [hivatkozó rendszergazdai](permissions-overview.md#manage-referrals) szerepköre van, amely olvasási és írási engedélyt is biztosít az összes ajánlathoz.|
|A Microsoft meghívása közös értékesítési ajánlaton keresztül|A Microsoft eladója kezdeményezte, nincs kifejezett kérdés a partnertől.|A partnernek [explicit kérést](manage-co-sell-opportunities.md#add-solutions) kell elvégeznie, ha egy üzlethez egy Microsoft-értékesítő segítségre van szüksége. A Microsoft Seller lehetőséget nyújt a kérés elutasítására.|
|Lejárat|Az alku fogalma nem jár le.|A partneri bejövő ügyletek 14 nap múlva lejárnak, ha a partner nem fogadja el őket. Ugyanez vonatkozik a partner kimenő ajánlatokra is, amelyekben a lejárt állapotba léphetnek, ha a Microsoft Seller 14 napon belül nem végez rájuk.|
|Microsoft Seller – részletek|Az üzlet létrehozásakor azonnal látható lesz.|A Microsoft értékesítő adatai csak akkor vannak megosztva a partnerekkel, ha az eladó kifejezetten elfogadja a partnertől való közös értékesítés meghívását.|
|[Privát folyamat](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Nem érhető el.|A partnerek a Microsoft-értékesítők láthatósága nélkül oszthatják meg a folyamatokat.|
|Megoldások|A csak egy árlistát tartalmazó megoldások egy üzlethez adhatók hozzá.|A partner hozzáadhat olyan [megoldásokat](manage-co-sell-opportunities.md#add-solutions) , amelyek a következő listához tartoznak. a) a Microsoft első féltől származó katalógusának (a PSC tranzakciós ügyleti szerepkörhöz hasonlóan) és a c) megoldásai a más, harmadik féltől származó partnereinktől származó megoldások közös értékesítéssel (a PSC-beli ISV-k szerepéhez hasonlóan).|
|Ügylet-hozzárendelés|Csak a hozzárendelt eladó tekinthet meg és járhat el az ajánlatokban.|A csoporttagok hozzáadhatók egy üzlethez, hogy megadják az üzleten dolgozó személyeket, és nem blokkolja a más hivatkozó rendszergazdákat az ilyen ügyletek megtekintésével vagy működésével kapcsolatban.|
|Ügyfél szervezete|Szabad formátumú szöveges bejegyzés.|Csak néhány karakter beírásával kereshet az [ügyfél szervezetében](manage-co-sell-opportunities.md#select-your-customer) a [D&B adatbázison](https://www.dnb.com/) . A jogi név és a címek a választás alapján automatikusan fel lesznek töltve.|
|Ügyfél elérhetősége|Nem kötelező.|Nem kötelező a magánhálózati folyamat megosztásához. Kötelező, ha a Microsoft értékesítőt közös értékesítésre kérik.|
|Nyilvános API|Nem érhető el.|[Nyilvános API](/partner/develop/referrals) a partner Center-hivatkozások programozott kezeléséhez.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>A PSC mezőinek leképezése a partner Center megfelelő mezőire

Ez a szakasz összehasonlítja a PSC-hez kiválasztott képernyőképeket a partner Center közös értékesítési lehetőségek szakaszának megfelelő nézetével.

A képernyőképek egyes párokban számozott, sárga vagy piros kör jelenik meg:

- **Mit jelent a sárga körök?** Az egyes PSC-képernyőképeken a számozott, sárga körök jelennek meg. Ezután megtalálhatja az alatta lévő partneri központ képernyőképét, amely számos azonos számmal rendelkezik.

   Ha szeretné megtekinteni, hogy a PSC-ban lévő egyes mezők vagy attribútumok hogyan képezik a partneri központban lévő összes mező értékét, akkor a két és kapcsolódó képernyőképek együttesen egyeznek a számozott körök Például egyezik a számozott, sárga "1" értékkel az első, PSC képernyőképen a számozott, sárga "1" a másodikban, a partner központ képernyőképe.

- **Mit jelent a piros kör?** Ha egy képernyőképen egy piros kör jelenik meg, az azt jelzi, hogy a PSC mező nem érhető el a partner Centerben.

A PSC-to-partner központ mezők leképezései a következő területekre mutatnak:

1. PSC Kezdőlap a partner Center közös értékesítési lehetőségeihez – alapértelmezett nézet
1. A partner Center Deal nézethez leképezett PSC Grid nézet
1. A PSC Deal részletek nézete a partner Center Deal részletek nézetére van leképezve
1. PSC Hozzáadás a partner Centerhez hozzárendelt termékek nézet
1. A partner Center felhasználói felügyelet nézethez hozzárendelt PSC felhasználói felügyelet nézet
1. PSC felhasználói szerepkör-hozzárendelés nézet a partner Center szerepkör-hozzárendelés nézethez rendelve
1. A partner Center értesítéseinek nézetére leképezett PSC-értesítések nézet

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 – PSC Kezdőlap a partneri központ közös értékesítési lehetőségeinek alapértelmezett nézetéhez rendelve

Hasonlítsa össze a megfelelő, számozott köröket a felső PSC képernyőkép és a partner központ képernyőképe között. A megfelelő számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a partner Centerben. A piros körök azt jelzik, hogy nincs megfelelő partneri központ mező.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Az a kép, amely a partner Sales-kapcsolat kezdőlapja és az együttes értékesítési lehetőségek a partner Centerben való társításának alapértelmezett nézetét mutatja." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 – a partneri központ Deal nézetéhez hozzárendelt PSC Grid nézet

Hasonlítsa össze a megfelelő, számozott köröket a felső PSC képernyőkép és a partner központ képernyőképe között. A megfelelő számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a partner Centerben. A piros körök azt jelzik, hogy nincs megfelelő partneri központ mező.  

> [!NOTE]
> Egyéb megfontolások a képernyőképek alatt jelennek meg.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Az a kép, amely a partner értékesítési összekötő (PSC) rács nézete és a partner Center Deal nézet közötti mező-hozzárendeléseket mutatja." lightbox="images/pscmigration/grid-view-expanded.png":::

**Speciális szempontok:**

- Nincs listanézet a partner Centerben, például a PSC-ben.  Az összes ajánlat a legfrissebb fogadott vagy létrehozott dátum alapján jelenik meg, az ügyfél adataival és az üzlet típusával. Alapértelmezés szerint a nézet első üzlete van kiválasztva. A PSC tábla formátumában megjelenő értékek többsége a számítógép üzletének részletes nézetében érhető el.
- Az üzlet szerepkör nem kötelező mező a PC-ben. Nem jelenik meg vagy nem rögzíthető a munkafolyamatokban. A rendszer automatikusan származtatja a Microsoft Eladó oldalán az üzlethez hozzáadott megoldások alapján.
- Az utolsó módosítás dátuma nem jelenik meg a számítógép hivatkozó részletek lapján. A partnerek a rendezés funkció segítségével rendezik az ajánlatokat az utolsó frissítés dátuma alapján.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 – PSC Deal részletek nézet leképezve a partneri központhoz

Hasonlítsa össze a megfelelő, számozott köröket a felső (PSC) képernyőképen az alatta lévő partner Center képernyőképen. A megfelelő számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a partner Centerben. A piros körök azt jelzik, hogy nincs megfelelő mező vagy munkaterület a partner Centerben.

> [!NOTE]
> Egyéb megfontolások a képernyőképek alatt jelennek meg.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Az a kép, amely a partner Sales-kapcsolat (PSC) és a partner Center Deal részletek nézete közötti mező-hozzárendeléseket mutatja." lightbox="images/pscmigration/deal-details-expanded.png":::

**Speciális szempontok:**

- A partnerek szerkeszthetik az üzletet a partner Deal részletes nézetének Szerkesztés gombjára kattintva (6). Miután kiválasztotta a Szerkesztés gombot, az összes mező szerkeszthető lesz. Ezután lehetősége van menteni vagy megszakítani az üzletben végzett módosításokat.
- A partner Centerben nem lehet lezárva az ügyletet ismétlődőként.
- Az ügyfél kimenetele nem érhető el a partner Centerben. Az ügyfél-interakciókkal kapcsolatos összes adat a számítógép megjegyzések szakaszában frissíthető.
- A megoldás bezárásának becsült dátuma csak a IOT lévő OEM-ajánlatok esetében érhető el. Ezek az információk nem jelennek meg más típusú ügyletekhez.
- A licencelési program nem szükséges a PC-n. Ezek az információk automatikusan következtetni az üzletben kiválasztott megoldások alapján.

>[!Note]
>A megnyert vagy elveszettként megjelölt ügyletek később nem szerkeszthetők. Körültekintően járjon el, amikor egy üzletet az egyik terminál-állapotba helyez át.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 – a "termékek hozzáadása" nézet hozzárendelve a "megoldások hozzáadása" nézethez

Hasonlítsa össze a megfelelő, számozott köröket a felső (PSC) képernyőképen az alatta lévő partner Center képernyőképen. A megfelelő számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a partner Centerben. A piros körök azt jelzik, hogy nincs megfelelő mező vagy munkaterület a partner Centerben.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Az a kép, amely a partner Sales-összekötő (PSC) a termékek hozzáadása és a partner Center – megoldások hozzáadása nézet közötti leképezéseket mutatja." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 – felhasználói felügyelet a PSC-ben és a partner Centerben

Hasonlítsa össze a megfelelő, számozott köröket a felső (PSC) képernyőképen az alatta lévő partner Center képernyőképen. A megfelelő számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a partner Centerben. A piros körök azt jelzik, hogy nincs megfelelő mező vagy munkaterület a partner Centerben.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Az a kép, amely a partner Sales-kapcsolat (PSC) felhasználói kezelés kezdőlapja és a fiókpartner felhasználói kezelés lapja közötti, a Fiókbeállítások területen található leképezéseket jeleníti meg."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 – felhasználói szerepkör-hozzárendelés a PSC-ben és a partner Centerben

Hasonlítsa össze a megfelelő, számozott köröket a felső (PSC) képernyőképen az alatta lévő partner Center képernyőképen. A megfelelő számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a partner Centerben. A piros körök azt jelzik, hogy nincs megfelelő mező vagy munkaterület a partner Centerben.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="A partner értékesítési csatlakozási (PSC) szerepkör-hozzárendelési nézet és a partner Center szerepkör-hozzárendelési nézet közötti mező-hozzárendeléseket bemutató kép." lightbox="images/pscmigration/roles-expanded.png":::

**Speciális szempontok:**

- A PSC rendszergazda ezzel egyenértékű szerepköre a fiók rendszergazdai szerepköre a partner Centerben.
- A partneri központban csak egyetlen szerepkör létezik a közös értékesítések kezelésére. Ez a szerepkör az Ajánlói rendszergazdai szerepkör.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 – értesítések a PSC-ben és a partner Centerben

Hasonlítsa össze a megfelelő, számozott köröket a felső (PSC) képernyőképen az alatta lévő partner Center képernyőképen. A megfelelő számok megmutatják, hol található a PSC-hez kapcsolódó szolgáltatás vagy attribútum a partner Centerben. A piros körök azt jelzik, hogy nincs megfelelő mező vagy munkaterület a partner Centerben.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="A partner értékesítési csatlakozási (PSC) értesítések és a partner Center értesítések nézet közötti leképezést ábrázoló kép."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Áthelyezés a PSC-ből a partneri központba – gyakori kérdések

A következő fejezetek az áttelepítéssel kapcsolatos gyakori kérdésekre válaszolnak.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 – Mi a teendő, ha nem férnek hozzá a partner Centerhez?

A hozzárendelt szerepkörök beszerzéséhez a "nincs hozzáférés" lapon felsorolt rendszergazdákat is felveheti. Az átirányítások szakaszban az [átirányítási rendszergazdai](permissions-overview.md#manage-referrals) szerepkörre lesz szüksége az olvasási és írási engedélyekhez. Ha csak üzleti profilokat kezel, akkor az üzleti profil rendszergazdai szerepkörére lesz szüksége a partner Centerben.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Az a kép, amely a partner Centerben nem fér hozzá a hozzáférési élményhez.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 – kik biztosíthatnak hozzáférést a partner központ átirányítások szakaszához?

A [fiók rendszergazdája](permissions-overview.md#manage-mpn-membership-and-your-company) hozzáférést biztosíthat az átirányítások lapjához. A fiók rendszergazdájának megkereséséhez válassza a **Fiókbeállítások** elemet a partner Center [irányítópultjának](https://partner.microsoft.com/dashboard)jobb felső sarkában található fogaskerék ikonra. Ezután a második szintű, bal oldali navigációs sávon válassza a **felhasználói kezelés** lehetőséget. A felhasználók listájának tetején válassza a **szűrő** legördülő menüt, és módosítsa a **fiók rendszergazdája** beállítást. A lap megjeleníti az összes fiók rendszergazdáját a hozzájuk tartozó e-mail-címükkel. Kérje meg az egyiket, hogy rendelje hozzá az Ajánlói rendszergazdai szerepkört a munkahelyi fiókjához.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 – az + új Deal gomb szürkén jelenik meg a fiókban. Mit kell tennem az ajánlatok létrehozásának megkezdéséhez?

Ez csak akkor történik meg, ha nincs olyan, a partner Centerben használt MPN-szervezethez csatlakoztatott, közös értékesítésre kész megoldás. Kérje meg a PDM, hogy kijavítsa a megoldások MPN-AZONOSÍTÓját, vagy hozzon létre egy támogatási jegyet, amely megemlíti a problémát: "az új Deal gomb szürkén jelenik meg a PSC-áttelepítés után".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 – Hogyan rendelhetek hozzá olyan ajánlatokat egy adott személyhez, mint például a PSC?

A csapat tagjait hozzárendelheti egy adott üzlethez. Nem akadályozza meg, hogy a többi hivatkozó rendszergazda megtekintse vagy ellássa ezeket az ajánlatokat.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 – megtekinthető az összes általam kiosztott ajánlat?

Használhatja a Kedvencek funkciót, amely egy felhasználói szintű lap. Megadhatja az összes olyan ajánlatot, amely a kedvencekhez van rendelve, hogy gyorsan hozzáférhessen az ajánlatokhoz.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 – van-e írásvédett nézet a Deals szolgáltatásokhoz?

Nem, az átirányítások szakaszban nem található az ajánlatok írásvédett nézete. Minden hivatkozó rendszergazdának teljes olvasási és írási hozzáférése lesz az összes ajánlathoz.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 – hogyan regisztrálhatok egy üzletet a megnyert megjelölése után?

Ha az üzlet megfelel az alábbi feltételeknek, megjelenik egy előugró ablak, amely az [üzlet regisztrációjának](./register-deals.md)megkezdését mutatja be.

- Az üzlethez egy ösztönző jogosult megoldás van társítva.
- A Microsoft eladó felkérést kap az üzletben való részvételre, vagy meghívta Önt az üzletre.
- A Microsoft Card a partner Centerben elfogadott vagy megnyert állapotban van.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 – hibaüzenet jelenik meg, ha a Deal regisztráció szakaszban az "+ új ügylet regisztrálása" gombot választom. Hogyan regisztrálhatom az ajánlatokat?

Az **+ új ügylet regisztrálása** gombot csak azok a partnerek használhatják, akik az ISV kapcsolódási programban regisztrálva vannak a partner Centerben nem megfelelő közös értékesítési lehetőséggel. Ha a regisztráláshoz közös értékesítési lehetőség van, akkor megjelenik egy előugró ablak, ha a Deal megjelölése megnyertként van megjelölve, és megfelel a Deal regisztráció feltételeinek.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 – kötelező-e az ügyfél-szervezet hozzáadása?

Igen, az [ügyfél-szervezet](./manage-co-sell-opportunities.md#select-your-customer) hozzáadása kötelező a partner Centerben. Először keresse meg azt a helyet, ahol az ügyfél helye van. A részletek alapján; konkrétan megadhatja a pontos épület nevét, vagy csak a város részleteit. A szervezet keresési szolgáltatás beolvassa az összes olyan jogi entitást, amely megfelel a megadott névnek, így nem kell megadnia a címet. A rendszer a kiválasztott szervezet alapján automatikusan kitölti az összes adatot.

### <a name="10---are-customer-contact-details-mandatory"></a>10 – az ügyfél elérhetőségi adatai kötelezőek?

A létrehozandó [alku típusától](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) függ. Ha csak a folyamatot osztja meg, és nem igényel segítséget a Microsoft értékesítési szervezettől, dönthet úgy is, hogy nem adja meg az ügyfél kapcsolattartási adatait. Ha olyan közös értékesítést szeretne, ahol aktívan keres segítséget a Microsoft értékesítőtől, meg kell adnia az ügyfél kapcsolattartási adatait. Hozzon létre explicit beleegyezést az ügyféltől, mielőtt közös értékesítési kérést hozna létre a partner Centerben.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 – hány megoldást vehetek fel egy üzletbe?

Akár 50 megoldást is hozzáadhat (hasonló a PSC-termékekhez) egy üzlethez. A PSC-től eltérően a saját közös értékesítésre jogosult megoldásaival, a Microsoft első féltől származó SKU-val és más, harmadik féltől származó, közös értékesítésre jogosult megoldásokat használhat. Nincs olyan üzletbeli szerepkör, amelyet ki kell választani, vagy elérhetőnek kell lennie a partner Centerben. A Microsoft SKU-ban opcionálisan hozzáadhat mennyiségeket és árat az üzlethez hozzáadott összes SKU-hoz.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 – Mikor jelenik meg a Microsoft-értékesítő részletei az alku létrehozása után?

A Microsoft-értékesítők csak akkor vannak hozzárendelve, ha megfelelnek a Microsoft oldalon a megfelelő értékesítő személysel való üzlet létrehozásakor feltételnek. A Microsoft Sellers még a hozzárendelést követően is választhat, hogy elfogadja vagy elutasítja a közös értékesítés meghívását. Az üzletet csak akkor fogja frissíteni, ha a közös értékesítési meghívást egy értékesítő fogadja el. A Microsoft-értékesítők által az üzletre vonatkozó SLA 14 nap. Ez ugyanaz az SLA, amelyet a partnereknek az ügylet lejárta előtt kell cselekedniük, mielőtt lejár az állapot.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 – Hol találhatom meg a lehetőség AZONOSÍTÓját?

A PSC-ben a lehetőség azonosítója megegyezik a számítógépen található üzlet-AZONOSÍTÓval. Az ügylet neve melletti üzlet-azonosítót az üzlet megnyitásakor is megtalálhatja.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14 – Hogyan szerezhetem be a PDM a számítógéphez?

A PDM nem érhető el közvetlenül a PSC-től eltérően. A funkció engedélyezéséhez több lehetőség is van, amelyek az alábbiakban láthatók.

- OCP-információ – ha a PDM csak a velük kapcsolatos ajánlatokat és előrehaladást tekinti meg, akkor a OCP-betekintő portál használatával megszerezheti a szervezet nézetét. Ez egy belső eszköz, és csak a PDM számára érhető el. Vegye figyelembe, hogy a OCP-eredmények a vállalat felhasználói számára nem érhetők el.
- Vendég felhasználó a partner Centerben – a PDM @microsoft.com fiókját vendég felhasználóként hozzáadhatja a partner Centerben, és hozzárendelheti a hozzájuk hivatkozó rendszergazdai szerepkört, így megtekintheti és elvégezheti az átirányítást.
- [Új felhasználó](./create-user-accounts-and-set-permissions.md#add-a-new-user) létrehozása a bérlőben – létrehozhat egy új felhasználót a saját bérlőben, és megoszthatja ezeket az adatokat a PDM, így megtekintheti és elvégezheti a fiókban lévő többi hivatkozó felhasználóhoz hasonló hivatkozásokat.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>A helyes MPN-azonosító megkeresése, ha a PSC-fiókja nincs érvényes MPN-hez társítva

Ha azért van itt, mert a PSC-ben a "PSC érvénytelen MPN-azonosító társítása" problémára hivatkozik, akkor Ön a megfelelő helyen található. Lehet, hogy a fiókja a következő okok miatt érvénytelen MPN-AZONOSÍTÓhoz lett társítva

- A vállalat nem rendelkezik partneri központ-fiókkal.
- A PDM hibát vétett a fiók MPN-AZONOSÍTÓjának beírásakor a belső rendszerekben, amelyek a PSC-fiókját a partner Center-fiókhoz (MPNID) kapcsolják.
- A vállalat nem végezte el az áttelepítést a partner Membership Center (PMC) rendszerről a számítógépre.

Először keresse meg a megfelelő MPN-azonosítót az alábbi lépések végrehajtásával

- Jelentkezzen be a partner Center-fiókjába
- Az MPN-azonosító megkereséséhez használja a [Fiókbeállítások dokumentációjában](./partner-center-account-setup.md#locate-your-mpn-id) megadott útmutatót.

Alább látható egy képernyőkép, amely a partner Center MPN-AZONOSÍTÓjának pontos helyét jeleníti meg

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="A fiók beállításait tartalmazó kép, ahol a partner megtalálja az MPN-AZONOSÍTÓját."  lightbox="images/pscmigration/findingMPNID.png":::

Next (Tovább)

- Ha rendelkezik PDM, kérje meg őket, hogy az MPN-azonosítót a partner Center-fiók megfelelő MPN-azonosítójával javítsa ki.
- Ha még nem rendelkezik PDM, küldjön egy e-mailt a PSC-szalagcímben megadott címre, és a PSC-fiók információit és a partner Center-fiókja helyes MPN-AZONOSÍTÓját is.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Erőforrások, amelyek segítenek az ajánlatok létrehozásában és kezelésében a partner Centerben

Ha még nem olvasta el a közös értékesítéssel foglalkozó témaköröket, a következő források segítenek a partner Centerbeli ajánlatok kezelésében.

|**Ehhez**   |**Olvassa el ezt**   |
|-----------------------|:-----------------------|
|A lapok és a navigáció megismerése a közös értékesítés lehetőségei oldalon|[Navigálás a közös értékesítés szakaszban](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|A D&B listából válassza ki az ügyfél szervezetét |[Válassza ki az ügyfelet](./manage-co-sell-opportunities.md#select-your-customer)|
|A mezők módosítása a Deal details szakaszban|[A Deal részletei](./manage-co-sell-opportunities.md#deal-details)|
|Csapat tagjainak hozzáadása egy alku csapathoz|[Alkalmazottak hozzáadása](./manage-co-sell-opportunities.md#add-team-members)|
|Válasz a közös értékesítésre|[Közös értékesítési ajánlatok kezelése](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Regisztrálja a partner Centerben megnyert ajánlatokat |[Új üzlet regisztrálása](./register-deals.md)
|Áttekintő elemzések beszerzése és az átirányítások megismerése |[Javaslatelemzések](./referral-insights.md)
|Üzleti profil létrehozása és kezelése|[Üzleti profil kezelése](./create-a-marketing-profile.md)
|Az üzleti profilhoz tartozó érdeklődők kezelése |[Érdeklődők kezelése](./manage-leads.md)|

## <a name="next-steps"></a>Következő lépések


- [Partneri értékesítések kapcsolódás a partneri központ munkafüzetéhez](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) – munkafüzet a partnerek értékesítési folyamatainak és szerepköreinek az új értékesítési folyamatokkal való összehangolásához a partner Center és a partner Sales-kapcsolat használatával.
- A [partner Center közös értékesítéssel kapcsolatos útmutatója](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) – útmutató egy működési modell azonosításához a partner centeren keresztül az érdeklődők felügyeletéhez, illetve a lehetőségek közös értékesítéséhez és regisztrálásához.
- [Ajánlói felügyelet](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) – részletes útmutató az érdeklődők kezeléséhez és a partneri központon keresztüli lehetőségek közös értékesítéséhez.
- [Közzététel és felügyelet a kereskedelmi piactéren](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) – részletes útmutató a kereskedelmi piactéren a partner Center segítségével történő létrehozásához, kezeléséhez és közzétételéhez.