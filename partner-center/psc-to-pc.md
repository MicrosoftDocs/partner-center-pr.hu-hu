---
title: Áttelepítés partner Sales-kapcsolatról (PSC)
ms.topic: article
ms.date: 08/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy a Microsoft-partnerek hogyan telepíthetik át a partneri értékesítési összekötőt a partneri központba, és hogyan hozhatók létre vagy kezelhetők a Microsoft-értékesítők
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc131991826a6428d613aa34e2e99c19e3efde05
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528483"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Útmutató a partneri értékesítési kapcsolódásról (PSC) áthelyezett partneri központhoz (számítógép) való közös értékesítéshez

**A következőkre vonatkozik**

- Partnerközpont

**Megfelelő szerepkörök**

- Fiókadminisztrátor
- Ajánlói rendszergazda
- Partner Sales-csatlakozási (PSC) értékesítő
- Partner Sales csatlakozási (PSC) rendszergazda
- Partner Sales csatlakozási (PSC) Deal Manager

Amint tudja, a vállalata a 2020-as december 31-ig elveszíti a PSC-hez való hozzáférést. Azonban mindent megtalál, amit szeretne, hogy közös értékesítési ajánlatokat hozzon létre, kezelje az ajánlatokat, és a Microsoft-értékesítők által a partner Centerben eljuttatott ajánlatokat is végrehajtja. A következő útmutatások azonban megtalálhatók, és az alábbi útmutató segítséget nyújt a partneri központ zökkenőmentesebb és egyszerű továbbításához.

>[!Important]
> Ha azért van itt, mert az áttelepítéssel kapcsolatban egy, a PSC-ben megjelenő szalagcím található, akkor Ön a megfelelő helyen található. Ez az útmutató nem alkalmazható megoldás-értékelési (SA) és OEM IOT-partnerek számára, akik a PSC-ben lévő ügyleteit kezelik.

## <a name="before-you-move-things-you-need-to-know"></a>Mielőtt továbblép, meg kell ismernie a szükséges dolgokat

### <a name="if-you-are-psc-admin"></a>Ha a PSC rendszergazdája

- A [partner központba](https://partner.microsoft.com/)való bejelentkezéshez munkahelyi e-mail-címre van szüksége.
- Állítsa be a fiókját a partner Center- [fiók rendszergazdája](permissions-overview.md)segítségével.
- A jelen dokumentum elolvasásával megtudhatja, hogyan értékesítheti a partner Centerben.
- Hozzon létre felhasználói fiókokat a partner Centerben az összes PSC-felhasználóhoz (rendszergazdai, Deal Manager-és eladói szerepkörök), és rendeljen hozzájuk [hivatkozási rendszergazdai szerepköröket](permissions-overview.md).

>[!Important]
> Győződjön meg arról, hogy a PSC-szalagcímben megjelenő MPN-azonosító elérhető a fiókpartner MPN-helyeinek listájában. A partner Centerben ellenőrizheti, hogy a "Fiókbeállítások" és a "[Locations](manage-locations.md)" lehetőséggel megkeresi a partner Center-fiókhoz társított összes MPNs listáját.

 :::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="A PSC-bannert bemutató kép, amelyben a partnerek megtalálják az MPN-azonosítót.":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>Ha a PSC Deal Manager vagy az eladó

- A [partner központba](https://partner.microsoft.com/)való bejelentkezéshez munkahelyi e-mailre van szükség.
- Ha nem munkahelyi fiókot használ a PSC-ben, vagy a munkahelyi e-mail-címe egy másik cég, mint a partner vállalat, forduljon a PSC rendszergazdához a fiók beállítása című súgóban.
- Forduljon a PSC rendszergazdájához, ha a partner Center-fiók beállítása a PSC-be való bejelentkezéshez használt fióktól függetlenül befejeződött.
- Ellenőrizze, hogy rendelkezik-e hozzáféréssel a partner központhoz és az átirányítási szakaszhoz.
- Olvassa el ezt a dokumentumot a munkafolyamatok és a partneri központ változásainak megismeréséhez.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>A PSC-ben rendszergazdaként ezek a következő lépések

Ha nem látja az átirányítások lapot:

- A vállalat [globális rendszergazdája](permissions-overview.md) hozzáférést biztosíthat az átirányítások lapjához. A globális rendszergazda kereséséhez lépjen a partneri beállítások elemre a partneri központ jobb felső sarkában található fogaskerék ikonra kattintva. A bal oldali navigációs sáv második szintjén válassza a felhasználó-kezelés lapot. Kattintson a lap jobb felső sarkában található "minden felhasználó" kifejezésre, és váltson a "globális rendszergazdák" elemre. A lap ezután megjeleníti az összes globális rendszergazdát a hozzájuk tartozó e-mail-azonosítókkal. Vegye fel velük a kapcsolatot a munkahelyi fiókjához való "Ajánlói rendszergazda" hozzáférés beszerzéséhez.

>[!Important]
> Ha a szerepkör csak a PSC-ben lévő felhasználókat kezeli, akkor a [fiók rendszergazdája](permissions-overview.md#manage-mpn-membership-and-your-company) szerepkört kaphat a partner Centerben. Ha a szerepköre magában foglalja a közös értékesítési lehetőségek kezelését is, akkor az [átirányítási rendszergazdai](permissions-overview.md#manage-referrals) szerepkört kell beszereznie. Emellett a PSC-rendszergazdák egy változási felügyeletet is kijelölnek, hogy a partner Center-fiók rendszergazdájával működjenek együtt a fiók rendszergazdái a PC-n.

 :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="A PSC-bannert bemutató kép, amelyben a partnerek megtalálják az MPN-azonosítót." elemre.
- A globális rendszergazda létrehozhat egy új felhasználói fiókot az Azure AD-bérlőben, vagy hozzárendelheti a vendég felhasználói hozzáférését a többi tartományi fiók felhasználóinak.
- Miután a fiókok be lettek állítva az összes PSC Deal Managerhez és felhasználóhoz, be kell jelentkezniük a partner központba, a bal oldali navigációs oldalon a referral (átirányítás) lapra, és ellenőrizze, hogy láthatják-e az átirányítási lapokat.

Ha a vállalata rendelkezik PDM – ha a partner Center-fiókja be van állítva, és a felhasználók áthelyezték és rendelkeznek szerepkörökkel és engedélyekkel, áthelyezheti a közös értékesítési tevékenységeket a partner központba. Tájékoztassa a PDM, hogy ne várjon, amíg az áttelepítés befejeződik, és így az összes új ügylet a fiókpartner-központba kerül.
>[!Note]
>Ha elvégezte ezt a kapcsolót, akkor csak a PSC meglévő aktív ajánlatait fogja tudni fellépni. Nem hozhat létre új ajánlatokat, és nem kap ajánlatokat a Microsoft-értékesítők által a PSC-ben.

Ha a vállalat nem rendelkezik PDM – győződjön meg arról, hogy az összes felhasználói fiók be van állítva és ellenőrizhető az összes felhasználó számára. A rendszer e-mailben és egy, a PSC-n lévő szalagcímben értesíti a pontos dátumról, amikor a partner Centerben megkezdi a közös értékesítést. Ne feledje, hogy továbbra is a PSC-ben meglévő aktív ajánlatokat kell kezelnie.

>[!Important]
>Az aktív ajánlatokat a rendszer nem telepíti át a számítógépre. Az ajánlatok bezárásához és regisztrálásához 2020 december 31-ig tart.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>A PSC-rendszergazdák, a PSC Deal managerek és a PSC-értékesítők következő lépései

Ismerje meg, hogyan értékesítheti közösen a partner centert.
Ez egy fontos lépés, amelynek segítségével előkészítheti a partneri központ közös értékesítését. Ismerje meg a munkafolyamatokat és a partneri központban bekövetkező változásokat, hogy az első naptól kezdve hatékonyan el tudja végezni a közös értékesítést. Első lépésként olvassa el a dokumentumot teljesen. Egy jó készlet is elérhető a [közös értékesítés élmény](https://aka.ms/cosellexperience)-katalógusában.

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

## <a name="psc-and-partner-center-field-mapping"></a>A PSC és a partner Center mező leképezése

Ez a szakasz a PSC és a partner Center közötti attribútumok pontos leképezését mutatja be. A PSC-ben minden képernyő összehasonlítható a partner Center közös értékesítés lehetőségei című szakasz megfelelő nézetével. 

>[!Note]
>A PSC-screenshotokban található sárga buborékok számait követve keresse meg a partner Center megfelelő attribútumát. A piros buborékok azt jelzik, hogy a iktatott nem érhető el a partner Centerben.

**A fiókpartner kezdőlapja és a közös értékesítési lehetőségek alapértelmezett nézete a partner Centerben**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="A PSC-bannert bemutató kép, amelyben a partnerek megtalálják az MPN-azonosítót.":::

**A PSC Grid nézet és a partner Center Deal nézete**

- Nincs listanézet a partner Centerben, például a PSC-ben.  Az összes ajánlat a legfrissebb fogadott vagy létrehozott dátum alapján jelenik meg, az ügyfél adataival és az üzlet típusával. Alapértelmezés szerint a nézet első üzlete van kiválasztva. A PSC tábla formátumában megjelenő értékek többsége a számítógép üzletének részletes nézetében érhető el.
- Az üzlet szerepkör nem kötelező mező a PC-ben. Egyik munkafolyamatban sem jelenik meg és nem rögzíthető. A rendszer automatikusan származtatja a Microsoft Eladó oldalán az üzlethez hozzáadott megoldások alapján.
- Az utolsó módosítás dátuma nem jelenik meg a számítógép hivatkozó részletek lapján. A partnerek a rendezés funkció segítségével rendezik az ajánlatokat az utolsó frissítés dátuma alapján.

 :::image type="content" source="images/pscmigration/gridview.png" alt-text="A PSC-bannert bemutató kép, amelyben a partnerek megtalálják az MPN-azonosítót.":::

**A PSC és a partner Center részletek nézete**

- A partnerek szerkeszthetik az üzletet a partner Deal részletes nézetének Szerkesztés gombjára kattintva (6). Ha a Szerkesztés gombra kattint, a rendszer az összes mezőt kijelöli, és megszakítja az üzletben végzett módosítások mentését vagy megszüntetését.
- A partner Centerben nem lehet lezárva az ügyletet ismétlődőként.
- Az ügyfél kimenetele nem érhető el a partner Centerben. Az ügyfél-interakciókkal kapcsolatos összes adat a számítógép megjegyzések szakaszában frissíthető.
- A megoldás bezárásának becsült dátuma csak a IOT lévő OEM-ajánlatok esetében érhető el. Más típusú ügyletek esetében nem jelenik meg.
- A licencelési program nem szükséges a PC-n. Az üzletben kiválasztott megoldások alapján automatikusan következtetünk.

>[!Note]
>A megnyert vagy elveszettként megjelölt ügyletek nem szerkeszthetők post. Körültekintően járjon el, amikor egy üzletet az egyik terminál-állapotba helyez át.

 :::image type="content" source="images/pscmigration/dealdetails.png" alt-text="A PSC-bannert bemutató kép, amelyben a partnerek megtalálják az MPN-azonosítót." nézete**

 :::image type="content" source="images/pscmigration/products.png" alt-text="A PSC-bannert bemutató kép, amelyben a partnerek megtalálják az MPN-azonosítót.":::

**Felhasználói felügyelet a PSC-ben és a partner Centerben**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="A PSC-bannert bemutató kép, amelyben a partnerek megtalálják az MPN-azonosítót.":::

**Felhasználói szerepkör-hozzárendelés a PSC-ben és a partner Centerben**

- A PSC rendszergazda ezzel egyenértékű szerepköre a fiók rendszergazdai szerepköre a partner Centerben.
- A partner Centerben csak egyetlen szerepkör található a közös értékesítések kezelésére, amely az Ajánlói rendszergazdai szerepkör.

 :::image type="content" source="images/pscmigration/roles.png" alt-text="A PSC-bannert bemutató kép, amelyben a partnerek megtalálják az MPN-azonosítót.":::

**Értesítések a PSC-ben és a partner Centerben**

 :::image type="content" source="images/pscmigration/notifications.png" alt-text="A PSC-bannert bemutató kép, amelyben a partnerek megtalálják az MPN-azonosítót.":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Áthelyezés a PSC-ből a partneri központba – gyakori kérdések

**Első. Mi a teendő, ha nem férnek hozzá a partner Centerhez?**

A hozzárendelt szerepkörök beszerzéséhez a "nincs hozzáférés" lapon felsorolt rendszergazdákat is felveheti. Az átirányítások szakaszban az olvasási és írási engedélyek "[hivatkozó rendszergazdai](permissions-overview.md#manage-referrals)" szerepkörre lesz szüksége. Ha csak üzleti profilokat kezel, akkor az "üzleti profil rendszergazdája" szerepkörre lesz szüksége a partner Centerben.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="A PSC-bannert bemutató kép, amelyben a partnerek megtalálják az MPN-azonosítót." csak azon partnerek általi használatra használható, akik regisztrálva vannak az ISV-összekötő programban, és nem regisztrálhatnak egy üzletet a partner Centerben a megfelelő közös értékesítési lehetőségekkel. Ha a regisztráláshoz közös értékesítési lehetőség van, akkor megjelenik egy előugró ablak, ha a Deal megjelölése megnyertként van megjelölve, és megfelel a Deal regisztráció feltételeinek.

**Q9. Kötelező felvenni egy ügyfél-szervezetet?**

Igen, az [ügyfél-szervezet](./manage-co-sell-opportunities.md#select-your-customer) hozzáadása kötelező a partner Centerben. Először keresse meg azt a helyet, ahol az ügyfél helye van. A részletek alapján; konkrétan megadhatja a pontos épület nevét, vagy csak a város részleteit. A szervezet keresési szolgáltatás beolvassa az összes olyan jogi entitást, amely megfelel a megadott névnek, így nem kell megadnia a címet. A rendszer a kiválasztott szervezet alapján automatikusan kitölti az összes adatot.

**Q10. Az ügyfél elérhetőségi adatai kötelezőek?**

A létrehozandó [alku típusától](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) függ. Ha csak a folyamatot osztja meg, és nem igényel segítséget a Microsoft értékesítési szervezettől, dönthet úgy is, hogy nem adja meg az ügyfél kapcsolattartási adatait. Ha olyan közös értékesítést szeretne, ahol aktívan keres segítséget a Microsoft értékesítőtől, meg kell adnia az ügyfél kapcsolattartási adatait. Hozzon létre explicit beleegyezést az ügyféltől, mielőtt közös értékesítési kérést hozna létre a partner Centerben.

**Q11. Hány megoldást vehetek fel egy üzletbe?**

Akár 50 megoldást is hozzáadhat (hasonló a PSC-termékekhez) egy üzlethez. A PSC-től eltérően a saját közös értékesítésre jogosult megoldásaival, a Microsoft első féltől származó SKU-val és más, harmadik féltől származó, közös értékesítésre jogosult megoldásokat használhat. Nincs olyan üzletbeli szerepkör, amelyet ki kell választani, vagy elérhetőnek kell lennie a partner Centerben. A Microsoft SKU-ban opcionálisan hozzáadhat mennyiségeket és árat az üzlethez hozzáadott összes SKU-hoz.

**K12. Honnan tudhatom meg, hogy a Microsoft-értékesítő adatai egy üzlet létrehozása után?**

A Microsoft-értékesítők csak akkor vannak hozzárendelve, ha megfelelnek a Microsoft oldalon a megfelelő értékesítő személysel való üzlet létrehozásakor feltételnek. A Microsoft Sellers még a hozzárendelést követően is választhat, hogy elfogadja vagy elutasítja a közös értékesítés meghívását. Az üzletet csak akkor fogja frissíteni, ha a közös értékesítési meghívást egy értékesítő fogadja el. A Microsoft-értékesítők által az üzletre vonatkozó SLA 14 nap. Ez ugyanaz az SLA, amelyet a partnereknek az ügylet lejárta előtt kell cselekedniük, mielőtt lejár az állapot.

**Q13. Hol találom a lehetőség AZONOSÍTÓját?**

A PSC-ben a lehetőség azonosítója megegyezik a számítógépen található üzlet-AZONOSÍTÓval. Az ügylet neve melletti üzlet-azonosítót az üzlet megnyitásakor is megtalálhatja.

**Q14. Hogyan érhetik el a PDM a számítógéphez?**

A PDM nem érhető el közvetlenül a PSC-től eltérően. A funkció engedélyezéséhez több lehetőség is van, amelyek az alábbiakban láthatók.

- OCP-információ – ha & a PDM csak a velük kapcsolatos előrehaladást tekinti át, akkor a OCP-betekintő portál használatával megszerezheti a szervezet nézetét. Ez egy belső eszköz, és csak a PDM számára érhető el. Vegye figyelembe, hogy a OCP-eredmények a vállalat felhasználói számára nem érhetők el.
- Vendég felhasználó a partner Centerben – a PDM @microsoft.com fiókját vendég felhasználóként hozzáadhatja a partner Centerben, és hozzárendelheti a hozzájuk hivatkozó rendszergazdai szerepkört, így megtekintheti és elvégezheti az átirányítást.
- [Új felhasználó](./create-user-accounts-and-set-permissions.md#add-a-new-user) létrehozása a bérlőben – létrehozhat egy új felhasználót a saját bérlőben, és megoszthatja ezeket az adatokat a PDM, így megtekintheti és elvégezheti a fiókban lévő többi hivatkozó felhasználóhoz hasonló hivatkozásokat.

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

## <a name="additional-resources"></a>További források

- [Partneri értékesítések kapcsolódás a partneri központ munkafüzetéhez](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) – munkafüzet a partnerek értékesítési folyamatainak és szerepköreinek az új értékesítési folyamatokkal való összehangolásához a partner Center és a partner Sales-kapcsolat használatával.
- A [partner Center közös értékesítéssel kapcsolatos útmutatója](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) – útmutató egy működési modell azonosításához a partner centeren keresztül az érdeklődők felügyeletéhez, illetve a lehetőségek közös értékesítéséhez és regisztrálásához.
- [Ajánlói felügyelet](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) – részletes útmutató az érdeklődők kezeléséhez és a partneri központon keresztüli lehetőségek közös értékesítéséhez.
- [Közzététel és felügyelet a kereskedelmi piactéren](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) – részletes útmutató a kereskedelmi piactéren a partner Center segítségével történő létrehozásához, kezeléséhez és közzétételéhez.
