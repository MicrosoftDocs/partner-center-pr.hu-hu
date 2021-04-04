---
title: Partneri biztonsági követelmények
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A a többtényezős hitelesítés (MFA) engedélyezéséhez és a biztonságos alkalmazás modell-keretrendszerének elfogadásához szükséges partneri biztonsági követelményeket ismerteti.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b7fa76999d2e071f80c0175a8dfcbc1afe527bfc
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087059"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>A partner Center vagy a partner Center API-k használatára vonatkozó biztonsági követelmények

**Megfelelő szerepkörök**

- Minden partner Center-felhasználó

Ez a cikk ismerteti az Advisors, a Vezérlőpult-szállítók és a felhőalapú megoldás-szolgáltatói programban részt vevő partnerek kötelező biztonsági követelményeit, valamint a hitelesítési lehetőségeket és az egyéb biztonsági szempontokat. Az adatvédelmi óvintézkedések és a biztonság a legfontosabb prioritások közé tartozik. Tudjuk, hogy a legjobb védelem a megelőzés, és hogy csak olyan erősek vagyunk, mint a leggyengébb kapcsolatunk. Ezért van szükségünk arra, hogy az ökoszisztémánk mindenki számára elérhető legyen, és biztosítsuk a megfelelő biztonsági védelem biztosítását.

## <a name="mandatory-security-requirements"></a>Kötelező biztonsági követelmények

Azok a partnerek, akik nem alkalmazzák a kötelező biztonsági követelményeket, nem tudnak majd tranzakciót végezni a felhőalapú megoldás-szolgáltató programban, vagy a delegált rendszergazdai jogosultságokkal kezelhetik az ügyfelek bérlőit. Emellett a biztonsági követelményeket nem megvalósító partnerek is felhasználhatják a programban való részvételüket. A partneri biztonsági követelményekhez társított feltételek hozzá lettek adva a Microsoft partneri szerződéshez. Az Advisors-hez kapcsolódóan ugyanazok a szerződéses követelmények lesznek érvényben.

Az Ön és ügyfelei elleni védelem érdekében a partnereknek azonnal a következő műveleteket kell elvégezniük:  

1. **Engedélyezze a többtényezős hitelesítést (MFA) a partner bérlő összes felhasználói fiókjához**. Az MFA-t a partneri bérlő (k) összes felhasználói fiókján ki kell kényszeríteni. A felhasználókat az MFA-nak kell kiadnia, amikor bejelentkeznek a Microsoft kereskedelmi Cloud Services szolgáltatásba, vagy amikor a partner Centerben vagy API-n keresztül végeznek a felhőalapú megoldás-szolgáltatói programban.

2. **Fogadja el a biztonságos alkalmazás modelljének keretrendszerét**. A partner Center API-kkal való integráció összes partnerének el kell fogadnia az alkalmazás-és a felhasználói hitelesítési modell alkalmazásaihoz szükséges [biztonságos Application Model keretrendszert](/partner-center/develop/enable-secure-app-model) .

    > [!IMPORTANT]
    > Erősen ajánljuk, hogy a partnerek a biztonságos alkalmazás modellt implementálják a Microsoft API-val való integrációhoz, például Azure Resource Manager vagy Microsoft Graph, vagy ha az automatizálást, például a PowerShellt felhasználói hitelesítő adatok használatával használják, az MFA kikényszerített megszakadásának elkerülése érdekében.

Ezek a biztonsági követelmények segítik az infrastruktúra védelmét és az ügyfelek adatainak védelmét az esetleges biztonsági kockázatokkal szemben, például a lopás vagy más csalás elleni incidensek azonosítása érdekében.  

## <a name="implementing-multi-factor-authentication"></a>A többtényezős hitelesítés megvalósítása

A partnerek biztonsági követelményeinek való megfelelés érdekében az MFA-t a partner bérlője minden felhasználói fiókjához be kell vezetnie és ki kell kényszeríteni. Ezt a következő módokon teheti meg:

- [Azure Active Directory (Azure ad) biztonsági Alapértelmezések](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)implementálása. További információk a [következő szakaszban](#security-defaults)olvashatók.

- Prémium szintű Azure Active Directory megvásárlása minden felhasználói fiókhoz. További információ: [Azure AD multi-Factor Authentication telepítésének megtervezése](/azure/active-directory/authentication/howto-mfa-getstarted).

- Egy harmadik féltől származó megoldással kényszerítheti ki az MFA használatát a partner bérlő minden felhasználói fiókjához. Annak biztosítása érdekében, hogy a megoldás megadja a várt megoldást, tekintse meg [a biztonsági követelmények betartatásának módját](#how-the-requirements-are-enforced).

> [!NOTE]
> Bár a többtényezős hitelesítés nem kötelező a szuverén felhő (USA kormánya és Németország) számára, kifejezetten ajánlott ezeket a biztonsági követelményeket alkalmazni.

### <a name="security-defaults"></a>Alapértelmezett biztonsági szabályok

Az egyik lehetőség, hogy a partnerek az MFA-követelmények megvalósítását is lehetővé teszik, az Azure AD biztonsági beállításainak engedélyezése. A biztonsági alapértékek alapszintű biztonsági szintet biztosítanak külön díj nélkül. Tekintse át, hogyan engedélyezheti az MFA-t a szervezete számára az Azure AD-vel, és az alábbi legfontosabb szempontokat a biztonsági beállítások engedélyezése előtt.

- Azoknak a partnereknek, akik már elfogadták az alapházirendeket, lépéseket kell tenniük a biztonsági alapbeállításokra való áttéréshez.

- A biztonsági alapértékek az előzetes verzióra vonatkozó alapszabályzatok általánosan elérhető cseréje. Miután egy partner engedélyezte a biztonsági beállításokat, többé nem fogja tudni engedélyezni az alapkonfiguráció-házirendeket.

- A biztonsági beállításokkal minden házirend egyszerre lesz engedélyezve.

- A [feltételes hozzáférést](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)használó partnereink esetében a [biztonsági beállítások nem lesznek elérhetők](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Jelenleg nem tudjuk letiltani a régi hitelesítést. Mivel azonban a feltört identitásokkal kapcsolatos legtöbb esemény a régi hitelesítést használó bejelentkezési kísérletből származik, a partnereknek ösztönözniük kell a régebbi protokolloktól való elmozdulást.

- Azure AD Connect szinkronizálási fiók ki van zárva a biztonsági alapértékek közül.

Részletes információk: az [Azure ad-multi-Factor Authentication áttekintése a szervezet számára](/azure/active-directory/authentication/concept-mfa-get-started) , és [Mik azok a biztonsági beállítások?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Az Azure AD biztonsági Alapértelmezések az alapkonfiguráció-védelmi szabályzatok egyszerűsített fejlődése. Ha már engedélyezte az alapkonfiguráció-védelmi házirendeket, akkor erősen ajánlott a [biztonsági beállítások](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)engedélyezése.

## <a name="implementation-considerations"></a>Implementálási szempontok

Mivel ezek a követelmények a partner bérlő összes felhasználói fiókjára érvényesek, több dolgot is figyelembe kell vennie a zökkenőmentes üzembe helyezés érdekében. Azonosíthatja például a felhasználói fiókokat az Azure AD-ben, amelyek nem tudják végrehajtani az MFA-t, valamint a szervezet olyan alkalmazásait és eszközeit, amelyek nem támogatják a modern hitelesítést.

A művelet végrehajtása előtt javasoljuk, hogy végezze el a következő érvényesítést. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Van olyan alkalmazás vagy eszköz, amely nem támogatja a modern hitelesítés használatát?

Ha kikényszeríti az MFA-t, az örökölt hitelesítés olyan protokollokat használ, mint például az IMAP, a POP3, az SMTP és mások, mivel nem támogatják az MFA-t. Ennek a korlátozásnak a megoldásához az alkalmazás [jelszavai](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) szolgáltatásával győződjön meg arról, hogy az alkalmazás vagy az eszköz továbbra is hitelesítve van. Tekintse át az [alkalmazások jelszavainak használatának szempontjait](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) annak meghatározásához, hogy használhatók-e a környezetben.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Rendelkezik a partner bérlőhöz társított licenccel rendelkező Office 365-felhasználókkal?

A megoldások megvalósítása előtt azt javasoljuk, hogy állapítsa meg, hogy a partner bérlője milyen verzióit használja a Microsoft Office felhasználók számára. Lehetséges, hogy a felhasználók kapcsolódási problémákba ütköznek az alkalmazásokkal, például az Outlookkal. Az MFA érvényesítése előtt fontos, hogy az Outlook 2013 SP1 vagy újabb verziót használja, és hogy a szervezete számára engedélyezve legyen a modern hitelesítés. További információ: [modern hitelesítés engedélyezése az Exchange Online-ban](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Ha olyan Windows rendszerű eszközökön kívánja engedélyezni a modern hitelesítést, amelyeken telepítve van a Microsoft Office 2013, akkor két beállításkulcsot kell létrehoznia. Lásd: [az Office 2013 modern hitelesítésének engedélyezése Windows-eszközökön](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Van olyan szabályzat, amely megakadályozza, hogy a felhasználók a mobileszközök használata közben használják a mobil eszközeiket?

Fontos, hogy azonosítsa a vállalati szabályzatot, amely megakadályozza, hogy az alkalmazottak a mobileszközök használatát használják, mivel ez hatással lesz az Ön által megvalósított MFA-megoldásra. Léteznek olyan megoldások, mint például az [Azure ad biztonsági Alapértelmezések](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)implementációja, amely csak a hitelesítő alkalmazás használatát teszi lehetővé ellenőrzés céljából. Ha a szervezet rendelkezik olyan házirenddel, amely megakadályozza a mobileszközök használatát, vegye figyelembe az alábbi lehetőségek egyikét:

- A biztonságos rendszeren futtatható, időalapú egyszeri jelszó (TOTP) alkalmazás üzembe helyezése.

- Hozzon létre egy külső gyártótól származó megoldást, amely az MFA-t kényszeríti a partner bérlő minden olyan felhasználói fiókjára, amely a legmegfelelőbb ellenőrzési lehetőséget biztosítja.

- [Prémium szintű Azure Active Directory](https://azure.microsoft.com/pricing/details/active-directory/) licencek vásárlása az érintett felhasználók számára.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Milyen automatizálásra vagy integrációra van szükség a felhasználói hitelesítő adatok kihasználása a hitelesítéshez?

Mivel az MFA-t minden felhasználó, például szolgáltatásfiókok esetében kikényszerítjük a partneri címtárban, ez hatással van minden olyan automatizálásra vagy integrációra, amely felhasználói hitelesítő adatokat használ a hitelesítéshez. Ezért fontos, hogy azonosítsa, hogy mely fiókokat használják ezekben a helyzetekben. Tekintse meg az alábbi, példákban szereplő alkalmazások vagy szolgáltatások listáját:

- A Vezérlőpult az ügyfelek nevében való kiépítésére használatos

- Integráció bármely olyan platformmal, amely a számlázáshoz használatos (a CSP programhoz kapcsolódik) és az ügyfelek támogatásához

- Az az, a AzureRM, az Azure AD, az MS online és más modulok használatát használó PowerShell-parancsfájlok

A fenti lista nem átfogó. Ezért fontos, hogy teljes körű értékelést végezzen a környezetben lévő bármely alkalmazásról vagy szolgáltatásról, amely felhasználói hitelesítő adatokat használ a hitelesítéshez. Az MFA követelményének megkövetelése érdekében a [biztonságos alkalmazás modelljének keretrendszerében](/partner-center/develop/enable-secure-app-model) kell megvalósítani az útmutatást, ahol lehetséges.

## <a name="accessing-your-environment"></a>A környezet elérése

Ha szeretné jobban megismerni, hogy mi vagy kik hitelesítik az MFA-t, akkor javasoljuk, hogy tekintse át a bejelentkezési tevékenységet. A prémium szintű Azure Active Directoryon keresztül használhatja a bejelentkezési jelentést. További információ erről a témáról: [bejelentkezési tevékenységek jelentései a Azure Active Directory portálon](/azure/active-directory/reports-monitoring/concept-sign-ins). Ha nem rendelkezik prémium szintű Azure Active Directorytel, vagy a bejelentkezési tevékenység PowerShell-lel való beszerzését keresi, akkor a [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) parancsmagot kell használnia a [partner Center PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) -modulból.

## <a name="how-the-requirements-are-enforced"></a>A követelmények betartatása

A partneri biztonsági követelményeket az Azure AD kényszeríti, a partner Center pedig pedig az MFA-jogcím meglétének ellenőrzésével ellenőrzi, hogy az MFA-ellenőrzés megtörtént-e. 2019. november 18-án a Microsoft aktiválta a további biztonsági óvintézkedéseket (korábbi nevén "technikai betartatás") a partnerek bérlői számára.

Aktiváláskor a partner bérlőben lévő felhasználókat arra kéri, hogy végezzenek el MFA-ellenőrzéseket, amikor a (z) (AOBO) műveletekkel, a partner Center portálhoz való hozzáféréssel vagy a partner Center API-k meghívásával végzik el a hitelesítést. További információ: [a többtényezős hitelesítés (MFA) megbízása a partner bérlője számára](partner-security-requirements-mandating-mfa.md). 

Azok a partnerek, akik nem teljesítik a követelményeket, a lehető leghamarabb végre kell hajtaniuk ezeket a mértékeket az üzleti fennakadások elkerülése érdekében. Ha Azure Active Directory Multi-Factor Authentication vagy az Azure AD biztonsági alapértékeit használja, nincs szükség további műveletekre.

Ha harmadik féltől származó MFA-megoldást használ, lehetséges, hogy az MFA-jogcímet nem lehet kibocsátani. Ha ez a jogcím hiányzik, az Azure AD nem fogja tudni megállapítani, hogy az MFA megkérdőjelezte-e a hitelesítési kérést. Ha szeretné megtudni, hogyan ellenőrizheti a megoldás a várt jogcímet, olvassa el [a partneri biztonsági követelmények tesztelését](/powershell/partnercenter/test-partner-security-requirements)ismertető témakört. 

> [!IMPORTANT]
> Ha a külső gyártótól származó megoldás nem adja ki a várt jogcímet, akkor a megoldást fejlesztő gyártóval kell dolgoznia, hogy meghatározza, milyen műveleteket kell végrehajtania.

## <a name="resources-and-samples"></a>Erőforrások és minták

Tekintse meg a következő forrásokat a támogatáshoz és a mintakód:

- A [partner Center biztonsági Orientációs csoport közössége](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): a partner Center biztonsági Orientációs csoport közössége egy online közösség, ahol megismerheti a közelgő eseményeket, és felteheti az esetlegesen felmerülő kérdéseket.
- [Partneri központ .net-minták](https://github.com/microsoft/partner-center-dotnet-samples): Ez a GitHub-adattár a .NET használatával fejlesztett mintákat tartalmaz, amelyek bemutatják, hogyan implementálhatja a biztonságos alkalmazás modell-keretrendszerét.
- A [partneri központ Java-mintái](https://github.com/microsoft/partner-center-java-samples): Ez a GitHub-tárház a Java használatával fejlesztett mintákat tartalmaz, amelyek bemutatják, hogyan valósítható meg a biztonságos alkalmazás modelljének keretrendszere.
- [Partner Center PowerShell – multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): ez a multi-Factor Authentication cikk részletesen ismerteti, hogyan valósítható meg a Secure Application Model Framework a PowerShell használatával.

## <a name="next-steps"></a>Következő lépések

- [A többtényezős hitelesítés (MFA) meghatalmazása a partner bérlője számára](partner-security-requirements-mandating-mfa.md)