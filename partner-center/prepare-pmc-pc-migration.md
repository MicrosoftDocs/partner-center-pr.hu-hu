---
title: Áthelyezés a Partner Membership Center
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Tekintse át a hasznos információkat és a gyakori kérdéseket, mielőtt a vállalatot át Partner Membership Center a Partnerközpont.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 7f533240d5236f03fe277d4c6dfa02ed1c58b63c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855012"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Készüljön fel a pmc Partner Membership Center ről a Partnerközpont

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Értékesítési ügynök | Rendszergazdai ügynök

A tagságkezelést a Partner Membership Center (PMC)-ről a Partnerközpont - a Microsofttal való üzleti kapcsolat egyetlen célhelyre való áthelyezéséhez. Azt szeretnénk, hogy a Partnerközpont a lehető leghatékonyabb és könnyebb legyen. Azonosítottunk néhány olyan területet, ahol a Partnerközpont eltér a PMC-től, és úgy gondoljuk, hogy az áthelyezés előtt szeretnénk megérteni és felkészülni rájuk.

## <a name="account-and-identity-setup"></a>Fiók és identitás beállítása

A fiók és az identitás beállításával kapcsolatos gyakori kérdésekre alább talál választ.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Mi az Azure Active Directory (Azure AD) munkahelyi fiókja?

Az Azure-beli munkahelyi fiók a vállalat dedikált és elkülönített virtuális reprezentációja az Azure nyilvános felhőben, amely akkor jön létre, amikor előfizet egy Microsoft-felhőszolgáltatásra, például az Azure-ra, az Microsoft Intune-re vagy az Office 365-re.

A munkahelyi fiókjában vannak az Azure AD-felhasználók, valamint azokkal kapcsolatos információk – az e-mail-címük, jelszavuk, profiladatok, engedélyek stb. A munkahelyi fiók csoportokat, alkalmazásokat és a vállalat biztonságával kapcsolatos egyéb információkat is tartalmaz. 

A munkahelyi e-mail-címe az Azure Active Directory-bérlő része. Ha fiókkal rendelkezik a Partnerközpont szüksége lesz egy AAD-bérlőre. A címtárral kapcsolatos további Azure Active Directory [a Címtár létrehozása az Azure AD-ban.](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)

A Partnerközpont a munkahelyi e-mail-címével fog bejelentkezni a fiókjába, nem a személyes e-mail-címére.

- A munkahelyi fiók: john@contoso.com
- Az Ön személyes fiókja: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Melyik fiókkal kell bejelentkeznie a Partnerközpont, ha microsoftos AAD-bérlővel rendelkezik (például Az Office 365-höz), és rendelkezik bérlővel a CSP-vállalkozáshoz is?

Bejelentkezhet a Partnerközpont CSP-fiókkal vagy az MPN munkahelyi e-mail-fiókjával. Ha a CSP munkahelyi e-mail-címének használatával jelentkezik be, az irányítópult bal oldali navigációs sávján az MPN- és a CSP-program adatai is megjelennek. Ha az MPN Azure AD-bérlő munkahelyi e-mail-címére jelentkezik be, csak az MPN-program adatai fognak látni. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Ha nem szeretné a meglévő Office 365 Azure AD-bérlőt használni az Partnerközpont-hez, létrehozhat egy új bérlőt a PMC-ről való áttelepítés előtt.

Számos oka lehet annak, ha nem szeretne meglévő Azure AD-bérlőt használni a Partnerközpont beállításhoz. Mielőtt megkezdi az áttelepítést a Partnerközpont, a Azure Portal [új](https://ms.portal.azure.com/#home) Azure AD-bérlő létrehozásához. Kövesse az Új bérlő [létrehozása a](/azure/active-directory/develop/quickstart-create-new-tenant)Azure Active Directory. Az új AAD-bérlővel beállíthatja a Partnerközpont fiókját. A bérlő létrehozásához globális rendszergazdának kell lennie. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Felhasználói szerepkörök, beleértve a vendégfelhasználói szerepköröket a Partnerközpont

Partnerközpont szerepkörtípusa a szükséges munkatípusoktól függően eltérő. Vannak olyan szerepkörök, mint például a globális rendszergazda, amelyek Azure AD-szerepkörök. Egyes szerepkörök csak programokra vonatkoznak, például a felhőszolgáltatói programra vagy az ösztönzőkre, és vannak olyan szerepkörök, amelyek az MPN-hez vannak. Ha meg szeretne tudni minden Partnerközpont szerepkörről, olvassa el a Felhasználói szerepkörök és engedélyek [hozzárendelése cikkeket.](permissions-overview.md)

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>Mi történik a felhasználók szerepköreivel, amikor a PMC-ről a Partnerközpont?

A PMC összes felhasználója elveszíti a rendszergazdai szerepkörét, kivéve az MPN globális rendszergazdai vagy elsődleges program kapcsolattartóját, aki a migrálást vezeti. Az áttelepítést lezáró személynek szerepköröket kell hozzárendelni a Partnerközpont. A szerepkörei Partnerközpont különböznek a PMC szerepköreitől. További információért olvassa el a [Felhasználói szerepkörök és engedélyek hozzárendelése] (permissions-overview.md és [Moving from PMC to Partnerközpont](move-pmc-pc-map.md#user-roles) to Partnerközpont (A felhasználói szerepkörök és engedélyek hozzárendelése] (permissions-overview.md és Moving from PMC to Partnerközpont ( Áthelyezés PMC-ről Partnerközpont.

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Mi a különbség a vállalati profilom és az üzleti profilom között?

A céges profil a vállalatra vonatkozó olyan információk, amelyek tartalmazzák a címet, a helyeket, az elsődleges kapcsolattartót, a bankot és az adózási adatokat.

Üzleti profiljával mutatja be magát az ügyfeleknek, és egy marketingoldalt, amely megjeleníti az emblémát, az üzleti fókusz részleteit, a szakértelmét stb.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Mit jelent a fiókkonszolidáció a fiókomra nézve?

Ha ugyanazt az Azure AD-bérlőt használja több MPN-fiók Partnerközpont-be való áttelepítéséhez, a rendszer automatikusan felismeri ezt, és megkéri, hogy vonja össze a fiókjait. Ez akkor is igaz, ha több tartomány van társítva ugyanhoz az Azure AD-bérlőhöz. 

Dönthet úgy is, hogy külön AAD Partnerközpont t használ, de vegye figyelembe, hogy ez a kompetenciák elkülönített kiértékelése és további vásárlási költségek mellett is jár. A fiókkonszolidációval kapcsolatos további információkért olvassa el [A vállalati fiókok konszolidálása](consolidate-accounts.md)

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Ha több AAD-bérlővel és egyetlen MPN-fiókkal is rendelkezik, összekapcsolni lehet őket egy Partnerközpont?

Igen, Partnerközpont több Azure AD-bérlőt is összekapcsolhat egyetlen Partnerközpont fiókkal.
A fiókkonszolidációval kapcsolatos további információkért olvassa el [A vállalati fiókok konszolidálása](consolidate-accounts.md)

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Vonatkozik korlátozás több Azure AD-bérlő hozzáadására egyetlen Partnerközpont fiókhoz?

Ha az Azure AD-bérlő már társítva van egy meglévő Partnerközpont-fiókkal, nem társítható új Partnerközpont-fiókokhoz a több-bérlős funkcióval. Úgy is fel lehet gondolni, hogy egy Azure AD-bérlő csak egy Partnerközpont-fiókhoz társítható, de egy Partnerközpont-fiókhoz több bérlő is társítható.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft Partner Network (MPN) tagságának áttelepítése 

Tekintse meg az alábbi válaszokat az MPN-tagság áttelepítésével kapcsolatos gyakori kérdésekre.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Ki végezheti el a PMC-ről a Partnerközpont?

A vállalat MPN globális rendszergazdája vagy a program elsődleges kapcsolattartója (ezt a két szerepkört gyakran ugyanaz a személy végzi) kezdeményezheti és végrehajthatja az áthelyezést.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>A migrálást befejező személy lesz az elsődleges kapcsolattartó a vállalat jogi profilján a Partnerközpont?

Az elsődleges kapcsolattartónak azonban nem feltétlenül kell olyannak lennie, aki engedéllyel rendelkezik a szerződések aláíráshoz.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Át tudja-e milálni a Microsoft az MPN-tagságomat?

Nem. A Microsoft nem tud segíteni a tagsági fiók partnerközpontba való áthelyezésében. A migrálási folyamat megkezdéséhez át kell áthelyezni a fiókját a PMC-be a munkahelyi fiókjával (bejelentkezési hitelesítő adatokkal). Miután befejezte a fiók áthelyezésének lépéseit, elkezdheti a tagság kezelését, és felhasználói szerepköröket és engedélyeket rendelhet a csapathoz, hogy hozzáférnek az előnyökhöz, és segítsenek a tagság kezelésében. 

A Microsoft automatikusan átemeli az aktuális kompetenciákat, előnyöket, helyadatokat, az ösztönzők banki/adóinformációit, valamint az MCP-társításokat, beleértve a Partner University-hozzáférést is.

### <a name="how-will-the-renewal-policy-change"></a>Hogyan változik a megújítási szabályzat?

Ebben Partnerközpont megújítási időszak az évforduló dátumáról a következő 30 napra esik.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>A kompetenciák változatlanok maradnak, miután áttértünk a Partnerközpont?

Igen, a kompetenciákra nem lesz hatással a Partnerközpont. Ha eltéréseket tapasztal, forduljon a támogatási [szolgálathoz.](https://partner.microsoft.com/support)

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Megváltoznak az előnyeim (beleértve a felhőbeli előnyöket, a műszaki támogatást, a szoftveres előnyöket Visual Studio) az áthelyezés után?

A jogosult előnyök nem változnak. Ha eltéréseket tapasztal, forduljon a támogatási [szolgálathoz.](https://partner.microsoft.com/support)

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Tiszteletben fogják-e Visual Studio kedvezményekkel rendelkező Microsoft-fiókokat?

Igen. Visual Studio MBA-k számára kiosztott előnyöket a program tiszteletben tartja és megőrzi. A megújítás után is megmaradnak a Partnerközpont. Ha azonban eltávolít egy MSA-foglalást az Partnerközpont-ban, nem használhatja újra a Partnerközpont.

Ebben Partnerközpont partner munkahelyi és vendégfelhasználói fiókokat adhat hozzá, amelyek MSA-k ugyanattól a bérlőtől, ahol a partner MPN-rendszergazda az Azure AD-bérlőben. Ha a partner több Azure AD-bérlő globális rendszergazdája, és ezek a bérlők ugyanannak az Partnerközpont-fióknak a fiókjához vannak társítva, akkor a partner hozzáadhat felhasználókat az összes bérlőhöz az Visual Studio előnyeihez és az Azure használatalapú foglalásaihoz.

Bár a vendégfelhasználókhoz az MPN-rendszergazda vagy a globális rendszergazda Visual Studio hozzárendelhet használatalapú előfizetéseket, a vendégfelhasználók nem Partnerközpont msa-val. A vendégfelhasználók azonban bejelentkeznek az Azure-ba, és Visual Studio és kihasználhatja a hozzárendelt előnyöket.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Hogyan kezelnünk kell az MCP-társításokat és a Partner University-hozzáférést?

A PMC-ről nem módosulnak az MCP-társítások. Az új alkalmazottakat azonban a Partnerközpont után a Partnerközpont. A Partner University meglévő felhasználókra vonatkozó összes engedélye megmarad, de az új alkalmazottaknak a képzési központba kell átmenni, hogy információt szerezzenek arról, hogyan lehet hozzáférni a Partner Universityhez. [](https://partner.microsoft.com/training)

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Hogyan MCP-információkat, miután továbblépek a Partnerközpont?

Az **irányítópult bal oldali** navigációs sávján válassza a Kompetenciák lehetőséget. A **Kompetenciák lapon** letöltheti a készségjelentést. A képességjelentés azokat a felhasználókat sorolja fel, akik az adott programon belül a megfelelő kompetenciákhoz és programokhoz Partnerközpont. Ha a felhasználók megszerezték a készségeiket, de ezek a készségek nem relevánsak az Ön által elért kompetenciák szempontjából, akkor nem fognak szerepelni a jelentésben.

### <a name="are-customer-references-used-in-partner-center"></a>Használnak ügyfélhivatkozásokat a Partnerközpont?

Nem, a kompetenciakövetelmények követelményeinek való megfeleléshez nincs szükség ügyfélreferenciákra a Partnerközpont.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>Át fog költözni a rekordtársítási partner Partnerközpont?

Igen, a Rekordpartner nem változik. További információ a [partnerazonosító az ügyfelekhez való csatolásával kapcsolatban.](/azure/billing/billing-partner-admin-link-started)

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Van hatással az ösztönzőkre a következőre való Partnerközpont?

Nem, az ösztönzőkre nincs hatással, ha a fiókját a helyek konszolidálása nélkül költözte át. Ha a vállalkozása több PMC-fiókkal rendelkezik, és a Partnerközpont-ba való áthelyezéskor úgy dönt, hogy egy globális fiókba konszolidálja azt, az ösztönzők nem lesznek veszteséggel, de az ösztönzők kifizetése késhet. 

Ha nem áthelyezi az összes olyan PMC-fiókot, amely részt vett az ösztönzőprogramokban, akkor leállíthatja az ezekhez a fiókokhoz kötődő bevételi ösztönzőket.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Mik az ösztönzők szerepkörei a Partnerközpont?

Az ösztönzők szerepkörei Partnerközpont helyalapúak, és az ösztönzők adminisztrátorát és az ösztönzők felhasználóját is tartalmazzák. A szerepkörökkel kapcsolatos további információkért lásd: Felhasználói [szerepkörök és engedélyek hozzárendelése.](permissions-overview.md)

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Hozzárendelhető-e az ösztönzőrendszergazdák globális és helyszinten?

Igen. Hozzárendelhet egy ösztönzők rendszergazdáját az összes helyhez, vagy minden helyhez saját ösztönzőrendszergazdát rendelhet hozzá.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Fizethet az ösztönzők globális vagy helyszinten?

Az ösztönzőket csak a hely szintjén fizetik ki.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>A hivatkozások esetében hány üzleti profilt hozhatunk létre?

A vállalata annyi üzleti profilt hozhat létre, amennyire csak szüksége van a vállalat érdeklődésének teljes körű létrehozására. Minden üzleti profilban legfeljebb öt helyet listához lehet listához, országonként egy helyet. Minden üzleti profil használhatja az egyes helyekre vonatkozó terjesztéseket.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Hogyan lesznek hozzárendelve a hivatkozások, milyen változásokra számíthatok? Ha például egy globális vállalatom van az egyik piacon és más piacokon is, hogyan lesznek kiosztva a hivatkozások?

A hivatkozások az ügyfél által megadott keresési paraméterek alapján vannak hozzárendelve. Függetlenül attól, hogy egy vagy több helyről van-e szó, ha az ügyfél megad egy kívánt helyet, és olyan vállalkozása van, amely megfelel a többi paraméternek, akkor a kérelem erre a helyre fog hivatkozni.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Átkullálok a Partnerközpont belülről. Hibaüzenetet kapok a Web Directtel kapcsolatban. Hogyan folytatja a migrálást?

Ha hibaüzenetet kap, mert részt vesz a Web Direct programban, tegye a következőket:

1. Jelentkezzen be a portálra. Azure.com, és hozzon létre egy új Azure AD-bérlőt. További információ: [Új Azure AD-bérlő létrehozása.](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant)

2. Miután létrehozta az új Azure AD-bérlőt, a használatával minkét Partner Membership Center-ről a Partnerközpont-re, vagy újként regisztrálható a Partnerközpont.