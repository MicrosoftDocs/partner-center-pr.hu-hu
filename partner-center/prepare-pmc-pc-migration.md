---
title: Áthelyezés a Partner tagsági központjából
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Tekintse át a hasznos információkat és a gyakori kérdéseket, mielőtt áthelyezi vállalatát a Partner tagsági központjából a partner központjába.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: be4250864bd07e555b0eb2079c28f3dfb4920805
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528535"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Felkészülés a partner Membership Center (PMC) és a partner Center közötti mozgásra

**Megfelelő szerepkörök**
- Globális rendszergazda
- Felhasználói rendszergazda
- Értékesítési ügynök
- Felügyeleti ügynök

A tagsági felügyeletet a partneri tagsági központból (PMC) helyezi át a partneri központba – ez az egyetlen cél a Microsofttal való üzleti kapcsolatok kezeléséhez. Azt szeretnénk, hogy a partner központhoz való áttérés a lehető leghatékonyabb és legegyszerűbb legyen. Azonosította azokat a területeket, ahol a partner központ eltér a PMCtól, és azt gondoljuk, hogy az áthelyezés előtt érdemes megismerni és előkészíteni őket.

## <a name="account-and-identity-setup"></a>Fiók és identitás beállítása

A fiók és az identitás beállításával kapcsolatos gyakori kérdésekre adott válaszokat alább találja.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Mi az Azure Active Directory (Azure AD) munkahelyi fiók?

Az Azure-beli munkahelyi fiók a vállalat dedikált és elszigetelt virtuális ábrázolása az Azure nyilvános felhőben, amely akkor jön létre, amikor előfizet egy Microsoft Cloud Service-re (például Azure, Microsoft Intune vagy Office 365).

Munkahelyi fiókja az Azure AD-felhasználókat és a rájuk vonatkozó információkat – az e-maileket, a jelszavakat, a profil adatait, az engedélyeket stb. – tárolja. A munkahelyi fiók a vállalatra és annak biztonságára vonatkozó csoportokat, alkalmazásokat és egyéb információkat is tartalmaz. 

Munkahelyi e-mail-címe az Azure Active Directory-bérlő részét képezi. Ahhoz, hogy fiókot lehessen létrehozni a partner Centerben, rendelkeznie kell egy HRE-Bérlővel. Azure Active Directoryról a [címtár létrehozása az Azure ad-ben](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)című témakörben olvashat bővebben.

A partner Centerben a munkahelyi e-mail-címét fogja használni, hogy ne a személyes e-mail-címére jelentkezzen be a fiókjába.

- Munkahelyi fiók: john@contoso.com
- Személyes fiók: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Milyen fiókkal kell bejelentkeznie a partneri központba, ha rendelkezik HRE-Bérlővel a Microsofttal (például Office 365), és Ön rendelkezik Bérlővel is a CSP vállalata számára?

A partner központba a CSP-fiókkal vagy az MPN munkahelyi e-mail-fiókjával lehet bejelentkezni. Ha úgy dönt, hogy bejelentkezik a CSP munkahelyi e-mail-címével, az irányítópult bal oldali navigációs felületén megjelenik az MPN és a CSP program információi is. Ha az MPN Azure AD-bérlő munkahelyi e-mail-címével jelentkezik be, csak az MPN-program adatait fogja látni. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Ha nem szeretné használni a meglévő Office 365 Azure AD-bérlőt a partneri központban, létrehozhat egy új bérlőt a PMC-ból való áttelepítés előtt.

Számos oka lehet annak, hogy nem kíván meglévő Azure AD-bérlőt használni a partner Center-fiók beállításához. Mielőtt megkezdené az áttelepítést a partneri központba, lépjen a [Azure Portal](https://ms.portal.azure.com/#home) egy új Azure ad-bérlő létrehozásához. Kövesse az [új bérlő létrehozása Azure Active Directoryban](/azure/active-directory/develop/quickstart-create-new-tenant)című témakör útmutatását. A partner Center-fiók beállításához használja az új HRE-bérlőt. A bérlő létrehozásához globális rendszergazdának kell lennie. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Felhasználói szerepkörök, beleértve a vendég felhasználói szerepköröket a partner Centerben

A partner központ különböző típusú szerepkörökkel rendelkezik, attól függően, hogy milyen típusú feladatok szükségesek. Vannak olyan szerepkörök, mint például a globális rendszergazda Azure AD-szerepkörök. Néhány szerepkör olyan programokra vonatkozik, mint például a Cloud Service Provider program vagy az ösztönzők, és vannak olyan szerepkörök, amelyek az MPN-re vonatkoznak. Ha szeretné megtudni, hogy mi az összes partner Center-szerepkör, olvassa el a [felhasználói szerepkörök és engedélyek kiosztása](permissions-overview.md)című témakört.

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>Mi történik a felhasználói szerepkörökkel, amikor a PMC-ből a partner központba költöznek?

Az MPN globális rendszergazdájának vagy elsődleges programjának az áttelepítést végző kapcsolatának kivételével a PMC összes felhasználója elveszíti a rendszergazdai szerepkörét. Az áttelepítést végző személynek hozzá kell rendelnie a szerepköröket a partner Centerben. A partner Center szerepkörei eltérnek a PMC szerepköreitől. A (z) [felhasználói szerepkörök és engedélyek kiosztása] (engedélyek – overview.md és a PMC közötti váltás a [partner Centerben](move-pmc-pc-map.md#user-roles) ) című cikkből tájékozódhat bővebben a partner Center felhasználói szerepköreiről.

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Mi a különbség a céges profil és az üzleti profil között?

A céges profil a vállalattal kapcsolatos információ, amely tartalmazza a címeket, a helyszíneket, az elsődleges kapcsolattartási, a banki és az adózási adatokat.

Az Ön üzleti profilja az, hogy Ön hogyan jeleníti meg az ügyfeleket, és egy marketing-oldal, amely megjeleníti a logóját, az üzleti fókusz részleteit, a szaktudását stb.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Mit jelent a fiók összevonása a fiókomhoz?

Ha ugyanazt az Azure AD-bérlőt használja több MPN-fiók áttelepítéséhez a partner Centerben, a rendszer automatikusan felismeri ezt, és megkéri a fiókok konszolidálását. Ez akkor is igaz, ha ugyanahhoz az Azure AD-bérlőhöz több tartomány van társítva. 

Továbbra is dönthet úgy, hogy különálló HRE-bérlők használatával áttelepíti a partneri központba, de ez a kompetenciák elkülönített kiértékelését és az extra vásárlási költségeket eredményezi. A fiókok konszolidálásával kapcsolatos további információkért olvassa el [a vállalati fiókok konszolidálása](consolidate-accounts.md) című témakört.

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Ha több HRE-Bérlővel és egyetlen MPN-fiókkal rendelkezem, akkor lehetséges, hogy összekapcsolja őket a partner Centerben?

Igen, a partner Centerben több Azure AD-bérlőt is csatolhat egyetlen partner Center-fiókhoz.
A fiókok konszolidálásával kapcsolatos további információkért olvassa el [a vállalati fiókok konszolidálása](consolidate-accounts.md) című témakört.

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Vannak korlátozások több Azure AD-bérlő egyetlen partner Center-fiókhoz való hozzáadására?

Ha az Azure AD-bérlő már társítva van egy meglévő partner Center-fiókhoz, akkor az nem rendelhető hozzá az új partner Center-fiókokhoz a több-bérlős szolgáltatás használatával. Egy másik lehetőség arra is, hogy az Azure AD-bérlő csak egy partner Center-fiókhoz társítható, de a partner Center-fiókhoz több bérlő is tartozhat.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft Partner Network (MPN) tagság migrálása 

Az MPN-tagság áttelepítésével kapcsolatos gyakori kérdésekre a következő válaszokat talál.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Kik végezhetik el az áttérést a PMC-ből a partner-központba?

A vállalat MPN globális rendszergazdája vagy az elsődleges program kapcsolata (ezt a két szerepkört gyakran ugyanaz a személy tartja) kezdeményezheti és elvégezheti az áthelyezést.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>Az áttelepítést végző személy lesz az elsődleges kapcsolattartó a vállalati jogi profilban a partner Centerben?

Nem feltétlenül szükséges azonban, hogy az elsődleges kapcsolattartónak olyan személynek kell lennie, akinek van engedélye a szerződések aláírására.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Áttelepíthetik a Microsoft MPN-tagságát?

Nem. A Microsoft nem tud segíteni a tagsági fiókjának a partner központba való áthelyezésében. A fiókját úgy kell áthelyeznie, hogy bejelentkezik a PMC szolgáltatásba a munkahelyi fiókjával (bejelentkezési hitelesítő adatokkal) az áttelepítési folyamat megkezdéséhez. Miután elvégezte a fiók áthelyezésének lépéseit, megkezdheti a tagság kezelését és a felhasználói szerepkörök és engedélyek hozzárendelését a csapathoz, hogy hozzáférhessenek az előnyökhöz, és segítsenek a tagság kezelésében. 

A Microsoft automatikusan áttelepíti az aktuális kompetenciákat, előnyöket, a tartózkodási hely adatait, a banki/adózási adatokat, valamint az MCP-társításokat, beleértve a partneri egyetemi hozzáférést is.

### <a name="how-will-the-renewal-policy-change"></a>Hogyan változik a megújítási szabályzat?

A partner Centerben a megújítási időszak a következő 30 napon keresztül érhető el az évfordulós időpontból.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>A kompetenciánk változatlan marad a partneri központba való áttérés után?

Igen, az áthelyezés a partneri központba nem érinti a kompetenciákat. Ha eltéréseket észlel, forduljon az [ügyfélszolgálathoz](https://partner.microsoft.com/support).

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Az előnyök (beleértve a Felhőbeli előnyöket, a technikai támogatást, a szoftverek előnyeit, a Visual studiót) változnak a költözés után?

A jogosult kedvezmények nem változnak. Ha eltéréseket észlel, forduljon az [ügyfélszolgálathoz](https://partner.microsoft.com/support).

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Meg kell-e adni Microsoft-fiókjaikat a Visual Studio előnyeinek kiosztásával?

Igen. A Visual Studio MSAs kiosztott előnyeit tiszteletben kell tartani és megőrizni. Ezeket a megújítást követően is megőrzi a rendszer a partner Centerben. Ha azonban eltávolít egy MSA-kiosztást a partnervállalat áttelepítése után, azt nem lehet ismét hozzáadni a partner központhoz.

A partner Centerben egy partner felveheti a munkahelyi fiókokat és a vendég felhasználói fiókokat, amelyek ugyanabból a bérlőből származnak, ahol az Azure AD-bérlőben a partner MSA MPN-rendszergazda. Ha a partner globális rendszergazda több Azure AD-bérlőben, és ezek a bérlők ugyanahhoz a partner Center-fiókhoz vannak társítva, akkor a partner az összes bérlőn elérhetővé teheti a felhasználók számára a Visual Studio előnyeit és az Azure használati alapú foglalásait.

Habár a vendég felhasználók a Visual studióhoz tartozó használati alapú előfizetéseket rendelhetik hozzá az MPN-rendszergazda vagy a globális rendszergazda számára, a vendég felhasználók nem tudnak bejelentkezni a MSA. A vendég felhasználóknak azonban be kell jelentkezniük az Azure-ba és a Visual studióba, hogy érvényesítsék és használják a hozzájuk rendelt előnyöket.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Hogyan kezeljük az MCP-társításokat és a partneri egyetemi hozzáférést?

A PMC-ből áthelyezett MCP-társítások nem változnak. A partner Centerre való áttérést követően azonban minden új alkalmazotthoz társítani kell a partner centert. A meglévő felhasználókra vonatkozó összes partneri egyetemi engedély továbbra is fennáll, de az új alkalmazottaknak [a képzési központban](https://partner.microsoft.com/training) kell megjelenniük a partneri Egyetem elérésének módjával kapcsolatban.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Hogyan az MCP-információk megtekintését a partneri központba való áttérés után?

Válassza ki a **kompetenciákat** a bal oldali navigációs panelen az irányítópulton. A **kompetenciák** lapon letöltheti a szaktudás jelentését. A szaktudás jelentés felsorolja azokat a felhasználókat, akik a partner központ kompetenciáinak és programjainak megfelelő képességeket szereztek be. Ha a felhasználók szaktudást szereztek, de ezek a képességek nem relevánsak a jelenleg használt kompetenciák szempontjából, nem fognak szerepelni a jelentésben.

### <a name="are-customer-references-used-in-partner-center"></a>A partner Centerben használják a Customer-referenciákat?

Nem szükséges, hogy az ügyfél-referenciák megfeleljenek a partnervállalat kompetenciával kapcsolatos követelményeinek.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>A Record Associations partnere a partner központba lép?

Igen, a rekord partnerének nincs változása. További információ a [partner azonosítójának az ügyfelekhez való összekapcsolásáról](/azure/billing/billing-partner-admin-link-started).

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Van-e hatása az ösztönzőkre a partneri központba való áttérés miatt?

Nem, a rendszer nem befolyásolja az ösztönzőket, ha a fiókját konszolidáló hely nélkül helyezte át. Ha a vállalat több fiókkal rendelkezik a PMC-ben, és ha a partneri központba költözik, globális fiókba kerül, nem fog csökkenni az ösztönzők, de az ösztönző kifizetése is késleltethető. 

Ha nem helyezi át az ösztönző programokban érintett összes PMC-fiókot, akkor leállíthatja az ezekhez a fiókokhoz kötött ösztönzők beszerzését.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Milyen ösztönző szerepkörök vannak a partner Centerben?

A fiókpartner ösztönző szerepkörei a helyükön alapulnak, és az ösztönzők rendszergazdai és ösztönző felhasználói. A szerepkörökkel kapcsolatos további információkért lásd: [felhasználói szerepkörök és engedélyek kiosztása](permissions-overview.md).

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>A rendszergazdák a globális és a hely szintjén is hozzárendelhetők?

Igen. Az ösztönző rendszergazdákat az összes hely ösztönző rendszergazdájának kiosztásával, vagy az egyes helyekhez saját ösztönző rendszergazda is tartozhat.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Az ösztönzők globális vagy tartózkodási szinten is megfizethetők?

Az ösztönzőket csak a hely szintjén kell fizetni.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>Milyen számú üzleti profil hozható létre?

A vállalat annyi üzleti profilt hozhat létre, amennyire szüksége van a vállalata érdekeinek teljes körű megjelenítéséhez. Minden üzleti profilban legfeljebb öt helyet listázhat, országonként egy helyet. Minden üzleti profil fogadhatja az egyes helyekre vonatkozó hivatkozásokat.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Hogyan lesznek hozzárendelve az átirányítások, milyen módosításokat várhatok el? Ha például globális vállalatom van az egyik piacon és más piacokon, akkor hogyan lesz hozzárendelve a hivatkozások?

Az átirányítások hozzárendelése az ügyfél által definiált keresési paraméterek alapján történik. Függetlenül attól, hogy rendelkezik-e egy vagy több hellyel, ha az ügyfelek egy kívánt helyet határoznak meg, és olyan üzlettel rendelkezik, amely megfelel a többi paraméternek, akkor az átirányításnak erre a helyre kell esnie.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Áttelepítik a partneri központba az Oroszországból. Hibaüzenetet kapok a web Directről. Hogyan folytatja az áttelepítést?

Ha hibaüzenet jelenik meg, mert részt vesz a webes Direct programban, tegye a következőket:

1. Jelentkezzen be a portálra. Azure.com, és hozzon létre egy új Azure AD-bérlőt. További információért olvassa el az [új Azure ad-bérlő létrehozása](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant)című témakört.

2. Miután létrehozta az új Azure AD-bérlőt, használja azt a Partner tagsági központból a partner központba való Migrálás vagy a partneri központ net-újdonságként való regisztrálásához.