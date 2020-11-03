---
title: Partneri biztonsági követelmények
ms.topic: article
ms.date: 10/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bevezeti a többtényezős hitelesítés (MFA) engedélyezéséhez szükséges partneri követelményeket, és elfogadja a biztonságos alkalmazás modelljének keretrendszerét.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 361a36adf40af67769a9a24ba1c485f2ad95b98c
ms.sourcegitcommit: 8a4a3de728532533276a88b1fd40c82b7a4ebb15
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/06/2020
ms.locfileid: "92530217"
---
# <a name="partner-security-requirements-for-partners-using-partner-center-or-partner-center-apis"></a>Partneri biztonsági követelmények a partner Center vagy a partner Center API-kat használó partnereknek

**A következőkre vonatkozik**

- A Cloud Solution Provider program összes partnere
  - Közvetlen számla
  - Közvetett szolgáltató
  - Közvetett viszonteladó
- A Vezérlőpult összes szállítója
- Minden tanácsadó

**Megfelelő felhasználók**

- Az összes engedélyezett felhasználó, beleértve a vendég felhasználókat

A kiemelt prioritások közé tartozik a nagyobb adatvédelmi védelem és biztonság. Tudjuk, hogy a legjobb védelem a megelőzés, és hogy csak olyan erősek vagyunk, mint a leggyengébb kapcsolatunk. Ezért van szükségünk arra, hogy az ökoszisztémánk mindenki számára elérhető legyen, és biztosítsuk a megfelelő biztonsági védelem biztosítását. A partnerek és az ügyfelek védelme érdekében az Advisors, a Vezérlőpult-szállítók és a felhőalapú megoldás-szolgáltatói programban részt vevő partnerek számára kötelező biztonsági követelményeket vezetünk be.

## <a name="overview"></a>Áttekintés

A partnerek számára szükséges a többtényezős hitelesítés kikényszerítve a partner bérlő összes felhasználói fiókjához. A partneri biztonsági követelményekhez társított feltételek hozzá lettek adva a Microsoft partneri szerződéshez. Az Advisors-hez kapcsolódóan ugyanazok a szerződéses követelmények lesznek érvényben.

Azok a partnerek, akik nem alkalmazzák a kötelező biztonsági követelményeket, nem tudnak majd tranzakciót végezni a felhőalapú megoldás-szolgáltatói programban, vagy a meghatalmazott rendszergazdai jogosultságokat kihasználó ügyfél-bérlőket a követelmények érvénybe léptetése után kezelhetik. Emellett a biztonsági követelményeket nem megvalósító partnerek is felhasználhatják a programban való részvételüket.  

Az Ön és ügyfelei elleni védelem érdekében a partnereknek azonnal a következő műveleteket kell elvégezniük:  

1. **Engedélyezze a multi-Factor Authentication (MFA) használatát a partner bérlő összes felhasználói fiókjához** . A partneri bérlő (k) összes felhasználói fiókját a többtényezős hitelesítésnek (MFA) kell kiadnia, amikor bejelentkeznek a Microsoft kereskedelmi Cloud Services szolgáltatásba, vagy ha a felhőalapú megoldás-szolgáltatói programban a partner Centerben vagy API-n keresztül végeznek tranzakciókat.

2. **Fogadja el a biztonságos alkalmazás modelljének keretrendszerét** . Fogadja el a biztonságos alkalmazás modelljének keretrendszerét. A partner Center API-val integráló összes partnernek el kell fogadnia a biztonságos alkalmazás-modell keretrendszert minden alkalmazás + felhasználói hitelesítési modell alkalmazáshoz.

    > [!IMPORTANT]
    > Azt javasoljuk, hogy a partnerek a biztonságos alkalmazás modellt implementálják egy olyan Microsoft API-val való integrációhoz, mint például a Azure Resource Manager, a Microsoft Graph, vagy az automatizálás, például a PowerShell használata felhasználói hitelesítő adatok használatával, hogy elkerülje az MFA kényszerített megszakadását.

A Multi-Factor Authentication (MFA) engedélyezése és a biztonságos alkalmazás-modell keretrendszer bevezetésével megvédheti infrastruktúráját, és biztosíthatja az ügyfelek adatait az esetleges biztonsági kockázatokkal szemben, például a lopás vagy más csalás elleni incidensek azonosítása érdekében.  

## <a name="actions-that-you-need-to-take"></a>Szükséges műveletek

A partneri biztonsági követelményeknek való megfelelés érdekében a többtényezős hitelesítést be kell kényszeríteni a partner bérlő minden felhasználói fiókjához. Ezt a következő módokon teheti meg:

- Az [Azure ad biztonsági Alapértelmezések](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)implementálása.

- Prémium szintű Azure Active Directory megvásárlása minden felhasználói fiókhoz. További információ: [felhőalapú Azure multi-Factor Authentication-telepítés tervezése](/azure/active-directory/authentication/howto-mfa-getstarted).

- Harmadik féltől származó megoldás használata a többtényezős hitelesítés kikényszeríthető a partner bérlője minden felhasználói fiókjához. Annak biztosítása érdekében, hogy a megoldás megadja a várt megoldást, tekintse meg [a biztonsági követelmények betartatásának módját](#how-the-requirements-will-be-enforced).

> [!NOTE]
> Bár a többtényezős hitelesítés nem kötelező a szuverén felhő (21Vianet, USA kormánya és Németország) esetében, kifejezetten ajánlott ezeket a biztonsági követelményeket alkalmazni.

## <a name="security-defaults"></a>Alapértelmezett biztonsági szabályok

A biztonsági alapértelmezett beállítások házirend az a [lehetőség](#actions-that-you-need-to-take) , hogy a partnerek az üzleti igényektől függően az MFA-t a biztonsági követelmények alapján implementálják. Alapszintű biztonsági szintet biztosít, külön díj nélkül. Tekintse át, hogyan engedélyezheti az MFA-t a szervezete számára az Azure AD-vel és az alábbi legfontosabb megfontolásokkal a biztonsági alapértékek engedélyezése előtt.

- Az alapházirendek a következő néhány hónapra érvényesek, és a rendszer február 2020 végén elavult célzást biztosít.

- Azoknak a partnereknek, akik már elfogadták az alapházirendeket, lépéseket kell tenniük a biztonsági alapbeállításokra való áttéréshez.

- A biztonsági alapértékek az előzetes verzióra vonatkozó alapszabályzatok általánosan elérhető cseréje. Miután egy partner engedélyezte a biztonsági beállításokat, többé nem fogja tudni engedélyezni az alapkonfiguráció-házirendeket.

- A biztonsági beállításokkal minden házirend egyszerre lesz engedélyezve.

- A [feltételes hozzáférést](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)használó partnereink esetében a [biztonsági beállítások nem lesznek elérhetők](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Jelenleg nem kényszeríti ki a régi hitelesítés blokkolását a partnerek számára. Mivel azonban a feltört identitásokkal kapcsolatos legtöbb esemény a régi hitelesítést használó bejelentkezési kísérletekből származik, a partnereknek ösztönözniük kell a régebbi protokolloktól való elmozdulást.

- Azure AD Connect szinkronizálási fiók ki van zárva a biztonsági alapértékek közül.

- Részletes információkért olvassa el [a multi-Factor Authentication engedélyezése a szervezet számára](/azure/active-directory/authentication/concept-mfa-get-started) és [Azure Active Directory biztonsági Alapértelmezések](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)című témakört.

> [!NOTE]
> Az Azure AD biztonsági Alapértelmezések az alapkonfiguráció-védelmi szabályzatok egyszerűsített fejlődése. Ha már engedélyezte az alapkonfiguráció-védelmi házirendeket, akkor erősen ajánlott a biztonsági beállítások engedélyezése.

Az alapkonfiguráció házirendjeiről a biztonsági alapbeállításokra való áttéréshez olvassa el [a mi a biztonsági alapértékek?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

### <a name="consideration"></a>Megfontolandó

Mivel ezek a követelmények a partner bérlő összes felhasználói fiókjára érvényesek, több dolgot is figyelembe kell vennie a zökkenőmentes üzembe helyezés érdekében, beleértve a felhasználói fiókok azonosítását olyan Azure Active Directoryban, amelyek nem képesek a többtényezős hitelesítés végrehajtására, valamint a szervezet által használt olyan alkalmazásokra és eszközökre, amelyek nem támogatják a modern hitelesítést.

A művelet végrehajtása előtt javasoljuk, hogy azonosítsa a következőket:

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Van olyan alkalmazás vagy eszköz, amely nem támogatja a modern hitelesítés használatát?

Ha kikényszeríti a többtényezős hitelesítés örökölt hitelesítési protokollait, például az IMAP, a POP3, az SMTP stb. protokollt, a rendszer letiltja a többtényezős hitelesítés használatát. Ha ezt a korlátozást szeretné kezelni, az alkalmazás [jelszavaként](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) ismert funkció is használható annak biztosítására, hogy az alkalmazás vagy az eszköz továbbra is hitelesítve legyen. Tekintse át az [itt](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) dokumentált alkalmazás-jelszavak használatának szempontjait annak megállapításához, hogy használhatók-e a környezetben.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Az Office 365-et használó felhasználók a partner bérlőhöz társított licencekkel rendelkeznek?

A megoldások megvalósítása előtt azt javasoljuk, hogy állapítsa meg, hogy a partner bérlője hány Microsoft Office-verziót használ. Lehetséges, hogy a felhasználók kapcsolódási problémákba ütköznek az alkalmazásokkal, például az Outlookkal. A többtényezős hitelesítés kényszerítése előtt fontos, hogy az Outlook 2013 SP1 vagy újabb verziót használja, és hogy a szervezete számára engedélyezve legyen a modern hitelesítés. További információt a [modern hitelesítés engedélyezése az Exchange Online-ban](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) című témakörben talál.

Ha engedélyezni szeretné a modern hitelesítést a Windows rendszerű eszközökön, amelyek Microsoft Office 2013 telepítve vannak, akkor két beállításkulcsot kell létrehoznia. Lásd: [az Office 2013 modern hitelesítésének engedélyezése Windows-eszközökön](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Van olyan szabályzat, amely megakadályozza, hogy a felhasználók a mobileszközök használata közben használják a mobil eszközeiket?

Fontos, hogy azonosítsa a vállalati szabályzatot, amely megakadályozza, hogy az alkalmazottak a mobileszközök használatát használják, mivel ez befolyásolhatja az Ön által megvalósított multi-Factor Authentication megoldást. Léteznek olyan megoldások, mint például az [Azure ad biztonsági Alapértelmezések](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)implementációja, amely csak a hitelesítő alkalmazás használatát teszi lehetővé ellenőrzés céljából. Ha a szervezet rendelkezik olyan házirenddel, amely megakadályozza a mobileszközök használatát, vegye figyelembe az alábbi lehetőségek egyikét:

- A biztonságos rendszeren futtatható, időalapú egyszeri jelszó (TOTP) alkalmazás üzembe helyezése

- Egy külső gyártótól származó megoldás implementálása, amely a legmegfelelőbb ellenőrzési lehetőséget biztosító partner-bérlő minden felhasználói fiókjánál érvényesíti a többtényezős hitelesítést.

- [Prémium szintű Azure Active Directory](https://azure.microsoft.com/pricing/details/active-directory/) licencek vásárlása az érintett felhasználók számára

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Milyen automatizálásra vagy integrációra van szükség a felhasználói hitelesítő adatok kihasználása a hitelesítéshez?

Mivel a követelmény az, hogy minden felhasználónál, például a szolgáltatásfiókoknál érvényesítse az MFA-t a partneri címtárban, minden olyan automatizálást vagy integrációt érint, amely a hitelesítés felhasználói hitelesítő adatait használja. Ezért fontos, hogy azonosítsa, hogy mely fiókokat használják ezekben a helyzetekben. Tekintse meg az alábbi, példákban szereplő alkalmazások vagy szolgáltatások listáját:

- A Vezérlőpult az ügyfelek nevében való kiépítésére használatos

- Integráció bármely olyan platformmal, amely a számlázáshoz használatos (a CSP programhoz kapcsolódik) és az ügyfelek támogatásához

- Az az, AzureRM, Azure AD, MS online stb. modulokat használó PowerShell-parancsfájlok

A fenti lista nem átfogó. Ezért fontos, hogy teljes körű értékelést végezzen a környezetben található bármely alkalmazásról vagy szolgáltatásról, amely kihasználja a hitelesítéshez szükséges felhasználói hitelesítő adatokat. Ha a többtényezős hitelesítésre vonatkozó követelményt szeretné megküzdeni, akkor a [biztonságos alkalmazás modelljének keretrendszerében](/partner-center/develop/enable-secure-app-model) kell megvalósítani az útmutatást, ahol lehetséges.

## <a name="accessing-your-environment"></a>A környezet elérése

Ha szeretné jobban megismerni, hogy mi vagy kik hitelesítik a többtényezős hitelesítés során, javasoljuk, hogy tekintse át a bejelentkezési tevékenységet. A prémium szintű Azure Active Directory használatával kihasználhatja a bejelentkezési jelentést. További információkat [a Azure Active Directory portál bejelentkezési tevékenységek jelentéseiben](/azure/active-directory/reports-monitoring/concept-sign-ins) talál. Ha nem rendelkezik prémium szintű Azure Active Directorytel, vagy ha a PowerShell használatával szeretné megszerezni ezt a lehetőséget, a [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity)  parancsmagot a [partner Center PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) -modulból kell kihasználnia.

## <a name="how-the-requirements-will-be-enforced"></a>A követelmények betartatása

A partneri biztonsági követelményeket a Azure Active Directory fogja kikényszeríteni, a partner központban pedig az MFA-jogcím meglétének ellenőrzésével annak azonosítására, hogy a multi-Factor Authentication ellenőrzése megtörtént. 2019. november 18-án a Microsoft további biztonsági óvintézkedéseket (korábbi nevén "technikai kényszerítést") aktivál a partnerek bérlői számára. 

Aktiváláskor a partner bérlőben lévő felhasználókat a rendszer kéri a többtényezős hitelesítés (MFA) ellenőrzésének elvégzésére, amikor a (z) (AOBO) műveletekhez rendszergazdai jogosultságot hajt végre. A biztonsági óvintézkedések hatókörét továbbra is kiterjesztjük további forgatókönyvekre és felhasználói szerepkörökre, és a partnerek számára előzetes értesítéseket biztosítunk. További információkért tekintse meg ezt a dokumentumot, amely gyakran frissül. Azok a partnerek, akik nem teljesítik a követelményeket, a lehető leghamarabb végre kell hajtaniuk ezeket a mértékeket az üzleti fennakadások elkerülése érdekében. 

Ha Azure Multi-Factor Authentication vagy Azure AD-beli biztonsági beállításokat használ, nincs szükség további műveletekre.

Harmadik féltől származó multi-Factor Authentication megoldás használata esetén előfordulhat, hogy az MFA-jogcímet nem lehet kibocsátani. Ha ez a jogcím hiányzik, Azure Active Directory nem fogja tudni megállapítani, hogy a többtényezős hitelesítés megkérdőjelezte-e a hitelesítési kérést. Ha szeretné megtudni, hogyan ellenőrizheti a megoldás a várt jogcímet, olvassa el [a partneri biztonsági követelmények tesztelését](/powershell/partnercenter/test-partner-security-requirements)ismertető témakört. 

> [!IMPORTANT]
> Ha a külső gyártótól származó megoldás nem adja ki a várt jogcímet, akkor a megoldást fejlesztő gyártóval kell dolgoznia, hogy meghatározza, milyen műveleteket kell végrehajtania.

## <a name="resources-and-support"></a>Források és támogatás

Tekintse meg a következő forrásokat a támogatáshoz és a mintakód:

- A [partner Center biztonsági Orientációs csoport közössége](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): a partner Center biztonsági Orientációs csoport közössége egy online közösség, ahol megismerheti a közelgő eseményeket, és felteheti az esetlegesen felmerülő kérdéseket.
- [Partneri központ .net-minták](https://github.com/microsoft/partner-center-dotnet-samples): Ez a GitHub-adattár a .NET használatával fejlesztett mintákat tartalmaz, amelyek bemutatják, hogyan implementálhatja a biztonságos alkalmazás modell-keretrendszerét.
- A [partneri központ Java-mintái](https://github.com/microsoft/partner-center-java-samples): Ez a GitHub-tárház a Java használatával fejlesztett mintákat tartalmaz, amelyek bemutatják, hogyan valósítható meg a biztonságos alkalmazás modelljének keretrendszere.
- [Partner Center PowerShell – multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): ez a multi-Factor Authentication cikk részletesen ismerteti, hogyan valósítható meg a Secure Application Model Framework a PowerShell használatával.