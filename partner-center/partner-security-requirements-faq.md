---
title: A partnerek biztonsági követelményei – gyakori kérdések
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A partneri biztonsági követelményekkel kapcsolatos gyakori kérdések – Mik azok, hogyan valósítják meg a partnereket, és hogy Ön hogyan tudja elérni őket.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f2bf6823fdd976632fb8ad9c8f11ce99835d76a5
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087076"
---
# <a name="common-questions-about-partner-security-requirements"></a>A partneri biztonsági követelményekkel kapcsolatos gyakori kérdések

**Megfelelő szerepkörök**

- Minden partner Center-felhasználó

Ez a cikk a [partneri biztonsági követelményekkel](partner-security-requirements.md)kapcsolatos gyakori kérdésekre ad választ.

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>Mik a partneri biztonsági követelmények, és miért érdemes a partnereknek megvalósítani?

A legfontosabb prioritások közé tartozik a nagyobb és folyamatos biztonsági és adatvédelmi védelem, és továbbra is segítjük a partnereknek az ügyfelek és a bérlők védelmét. Továbbra is kifinomultabb, egyre növekvő számú biztonsági támadás jelenik meg, amelyek elsődlegesen a személyazonossággal kapcsolatos veszélyekkel kapcsolatos incidensekkel kapcsolatosak. Mivel a megelőző szabályozások kulcsszerepet játszanak egy általános védelmi stratégiában a biztonsági támadások meghiúsítása érdekében, a 2019-es [kötelező biztonsági követelmények](partner-security-requirements.md) bevezetve. A Cloud Solution Provider (CSP) program, a Vezérlőpult-szállítók és az Advisors szolgáltatásban részt vevő összes partnernek meg kell valósítania a követelményeknek megfelelő megfelelőséget.

### <a name="what-are-the-key-timelines-and-milestones"></a>Mik a legfontosabb ütemtervek és mérföldkövek?

Az ezekhez a biztonsági követelményekhez társított feltételek, beleértve az időkereteket és a mérföldköveket is, a [Microsoft partneri szerződés](microsoft-partner-agreement.md)tartalmazza. Ezeket a biztonsági követelményeket a lehető leghamarabb végre kell hajtania, hogy megfeleljen a CSP programban való részvételnek.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Mi történik, ha nem implementálom ezeket a partneri biztonsági követelményeket?

A Microsoft partneri szerződés megköveteli, hogy a többtényezős hitelesítést a felhasználói fiókoknál érvényesítse, és fogadja el a biztonságos alkalmazás modellt a partner Center API-val való interakcióhoz. 

Azok a partnerek, akik nem rendelkeznek ezekkel a biztonsági gyakorlattal, elveszítik a tranzakciót a CSP programban, vagy a rendszergazdai jogosultságok delegálásával kezelhetik az ügyfelek bérlőit.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>A biztonsági követelmények minden földrajzi régióra érvényesek?

Igen, a biztonsági követelmények minden földrajzi régióra érvényesek. Azt javasoljuk, hogy minden olyan partner, amely egy szuverén felhőn (USA-beli kormányzaton és Németországon) keresztül végez tranzakciót, azonnal alkalmazza ezeket az új biztonsági követelményeket. Ezek a partnerek azonban jelenleg nem szükségesek a biztonsági követelmények teljesítéséhez. A Microsoft további részleteket biztosít a szuverén felhőkre vonatkozó biztonsági követelmények végrehajtásával kapcsolatban a jövőben.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Lehetséges a fiók kizárása?

Nem, a többtényezős hitelesítés (MFA) érvényesítésének követelménye alól nem zárható ki semmilyen felhasználói fiók. A partnerek magas jogosultsági szintű jellege miatt a Microsoft partneri szerződés megköveteli, hogy a többtényezős hitelesítés kényszerítve legyen a partner bérlője minden felhasználói fiókjára.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Hogyan tudni, hogy teljesülnek-e a partneri biztonsági követelmények?

Végezze el a következő lépéseket:

- A [partneri biztonsági követelményekben](partner-security-requirements.md)ismertetett összes követelménynek meg kell felelnie.
- Gondoskodnia kell arról, hogy a partner bérlője összes felhasználói fiókja rendelkezzen a többtényezős hitelesítéssel.

Az olyan kulcsfontosságú területek azonosításához, ahol műveleteket hajthat végre, a partner centeren keresztül elérhető [biztonsági követelményekről szóló állapotjelentést](https://partner.microsoft.com/commerce/security/compliance) biztosítunk.

Az állapotjelentés részletes ismertetését a [partneri biztonsági követelmények állapotáról](partner-security-compliance.md)szóló témakörben tekintheti meg.

## <a name="required-actions"></a>Szükséges műveletek

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Milyen kulcsfontosságú műveleteket kell végrehajtani a követelmények teljesítése érdekében?

A CSP program összes partnere (a közvetlen számlázás, a közvetett szolgáltató és a közvetett viszonteladó), az Advisors és a Vezérlőpult gyártóinak meg kell felelniük a követelményeknek.

1. **MFA kikényszerítés minden felhasználó számára**

    A CSP program, az Advisors és a Vezérlőpult gyártóinak összes partnere köteles az MFA kikényszeríteni a partner bérlő összes felhasználója számára.

    További szempontok:

    - A közvetett szolgáltatóknak a közvetlen viszonteladókkal kell dolgozniuk a bevezetéshez a partner központba, ha még nem tették volna meg, és arra bátorítják a viszonteladókat, hogy megfeleljenek a követelményeknek.
    - Az Azure MFA-t a partner bérlő összes felhasználója ingyenesen elérhetővé teszi az Azure AD biztonsági alapértékek szolgáltatással, amely a hitelesítő alkalmazás egyetlen ellenőrzési módszere, amely támogatja az időalapú egyszeri jelszavakat (TOTP).
    - További ellenőrzési módszerek érhetők el az [prémium szintű Azure Active Directory](/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU-n keresztül, ha más módszerekkel, például telefonhívással vagy szöveges üzenettel kell rendelkezniük.
    - A partnerek harmadik féltől származó MFA-megoldást is használhatnak minden egyes fiókhoz a Microsoft kereskedelmi felhőalapú szolgáltatásaihoz való hozzáférés során.

2. **A biztonságos alkalmazás modell-keretrendszerének elfogadása**

    Minden olyan partner, aki bármely API-val (például Azure Resource Manager, Microsoft Graph, partner Center API stb.) fejlesztett ki egyéni integrációt, vagy az olyan eszközök használatával implementálta az egyéni automatizálást, mint amilyen a PowerShell, el kell fogadnia a [biztonságos alkalmazás-modell keretrendszert](/partner-center/develop/enable-secure-app-model) a Microsoft Cloud Services integrálásához. Ennek elmulasztása az MFA-telepítés miatt megszakadhat. A következő források áttekintést nyújtanak a modell bevezetésével kapcsolatban.

    - [Az alkalmazás-modell biztonságos áttekintése](/partner-center/develop/enable-secure-app-model)
    - [Partneri központ: az alkalmazás-modell biztonságos útmutatója](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partnerek a CSP programban: .NET-mintakód a biztonságos alkalmazás modelljének engedélyezéséhez](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partnerek a CSP programban: a biztonságos alkalmazás modelljét engedélyező Java-mintakód](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [A partneri központ hitelesítési dokumentuma](/partner-center/develop/partner-center-authentication)
    - [A partneri központ PowerShell-Multi-Factor Authentication (MFA) dokumentuma](/powershell/partnercenter/multi-factor-auth)

    Forduljon a szállítóhoz, ha a biztonságos Application Model-keretrendszer bevezetésére vonatkozó Vezérlőpultot használ.

    A Vezérlőpult gyártóinak be kell jelentkezniük a partner Centerbe a Vezérlőpulton, és [azonnal meg kell](enroll-as-cpv.md) kezdeni a követelmény megvalósítását. Tekintse át a következőt [: a partner Center biztonságos alkalmazás modelljének keretrendszere](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). A Vezérlőpult gyártóinak a hitelesítő adatok helyett el kell fogadniuk és kezelniük kell a CSP-partnerek beleértett hozzájárulásukat.

## <a name="multi-factor-authentication"></a>Többtényezős hitelesítés

### <a name="what-is-multi-factor-authentication-mfa"></a>Mi az a többtényezős hitelesítés (MFA)?

Az MFA egy biztonsági mechanizmus, amely többek között egy szükséges biztonsági és ellenőrzési eljárással hitelesíti a személyeket. Úgy működik, hogy a következő hitelesítési módszerek közül kettőt vagy többet igényel:

- Amit ismer (általában jelszó)
- Valami, ami rendelkezik (olyan megbízható eszköz, amely nem könnyen duplikált, például telefon)
- Egy dolog (biometria)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Mennyibe kerül az MFA engedélyezése?

A Microsoft az Azure AD biztonsági alapértékeinek megvalósítása révén díjmentesen biztosít MFA-t. Az MFA ezen verzióját használó egyetlen ellenőrzési lehetőség egy hitelesítő alkalmazás. Ha telefonhívást vagy SMS-üzenetet kell megadnia, akkor meg kell vásárolnia [prémium szintű Azure Active Directory](/azure/active-directory/fundamentals/active-directory-get-started-premium) licencet. Azt is megteheti, hogy egy harmadik féltől származó megoldást is biztosít, amely az MFA-t biztosítja a partner bérlő minden felhasználója számára – ebben az esetben az Ön felelőssége, hogy az MFA-megoldás érvénybe lépjen, és hogy megfelelő legyen.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Milyen műveleteket kell elvégeznie, ha már van egy MFA-megoldásom?

Ezekkel a biztonsági követelményekkel a partner bérlők felhasználóinak hitelesíteniük kell magukat az MFA használatával a Microsoft kereskedelmi felhőalapú szolgáltatásaihoz való hozzáféréskor. Ezen követelmények teljesítéséhez külső gyártótól származó megoldások is használhatók. A Microsoft már nem biztosít érvényesítési teszteket a független identitás-szolgáltatók számára a Azure Active Directory való kompatibilitás érdekében. A termék együttműködésének teszteléséhez tekintse meg az alábbi [irányelveket](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> Harmadik féltől származó megoldás használata esetén fontos ellenőrizni, hogy a megoldás kiállítja-e az MFA-értéket magában foglaló hitelesítési módszer-referenciát (AMR). Tekintse meg a [partneri biztonsági követelmények tesztelésével](/powershell/partnercenter/test-partner-security-requirements) kapcsolatos részleteket arról, hogy a harmadik féltől származó megoldás hogyan érvényesíti a várt jogcímet.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Több partneri bérlőt használok a Transact művelethez. Szükséges-e az MFA implementálása mind?

Igen, ki kell kényszeríteni az MFA-t a CSP programhoz vagy az Advisor programhoz társított minden Azure Active Directory bérlőhöz. Prémium szintű Azure Active Directory licenc megvásárlásához meg kell vásárolnia egy Azure Active Directory-licencet az egyes Azure Active Directory bérlők felhasználói számára. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Meg kell-e adni a partneri bérlő minden felhasználói fiókjának az MFA-t?

Igen, minden felhasználónak rendelkeznie kell MFA-érvényesítéssel. Ha azonban az Azure AD biztonsági alapértelmezéseit használja, akkor nincs szükség további műveletre, mert ez a szolgáltatás minden felhasználói fiók esetében kikényszeríti az MFA-t. A biztonsági alapértékek engedélyezése ingyenes és egyszerűen biztosítható, hogy a felhasználói fiókok MFA-kompatibilisek legyenek, és ne legyenek hatással az MFA betartatására.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Közvetlen számlás partner vagyok a Microsofttal. Mit kell tennem?

A közvetlen számlás felhőalapú megoldás-szolgáltató partnereinek az MFA-t kell kikényszeríteni a partner bérlő minden felhasználója számára.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Közvetett viszonteladó vagyok, és csak a terjesztői. Továbbra is engedélyezni kell az MFA használatát?

Minden közvetett viszonteladónak meg kell követelnie az MFA kikényszerített feltételeit a partner bérlő minden felhasználója számára. A közvetett viszonteladónak engedélyeznie kell az MFA-t.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Nem használom a partner Center API-t. Továbbra is szükség van az MFA megvalósítására?

Igen, ez a biztonsági követelmény minden felhasználóhoz, többek között a partner-rendszergazda felhasználókhoz és a partner bérlőhöz tartozó végfelhasználóhoz is vonatkozik.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Mely külső gyártóknak biztosítanak a Azure Active Directory kompatibilis MFA-megoldásokat?

Az MFA-szállítók és megoldások áttekintésekor a partnereknek biztosítaniuk kell, hogy az általuk választott megoldás kompatibilis legyen Azure Active Directorysal.

A Microsoft már nem biztosít érvényesítési teszteket a független identitás-szolgáltatók számára a Azure Active Directory való kompatibilitás érdekében. Ha tesztelni szeretné a terméket az együttműködéshez, tekintse meg ezeket az [irányelveket](https://www.microsoft.com/download/details.aspx?id=56843).

További információkért lásd az [Azure ad összevonási kompatibilitási listáját](/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Hogyan lehet tesztelni az MFA-t az integrációs homokozóban?

Az Azure AD biztonsági Alapértelmezések funkciójának engedélyezve kell lennie, vagy egy külső gyártótól származó, összevonást használó megoldást is használhat.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Az MFA engedélyezése befolyásolja az ügyfelek Bérlővel való együttműködését?

Nem. Ezeknek a biztonsági követelményeknek a teljesítése nem befolyásolja az ügyfelek kezelésének módját. A delegált felügyeleti műveletek végrehajtásának lehetősége nem lesz megszakítva.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Az ügyfeleim a partneri biztonsági követelmények hatálya alá esnek?

Nem szükséges, hogy az MFA-t az ügyfél Azure AD-bérlői minden felhasználója kikényszerítse. Javasoljuk azonban, hogy az egyes ügyfelekkel együttműködve határozza meg, hogyan védik a legjobban a felhasználókat.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Kizárható a felhasználók az MFA-követelmények alól?

Nem, minden felhasználónak, beleértve a szolgáltatásfiókot is, a partner bérlőn hitelesítenie kell magát az MFA használatával.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Érvényesek-e a partneri biztonsági követelmények az integrációs munkaterületre?

Igen, a partneri biztonsági követelmények érvényesek az integrációs munkaterületre. Ez azt jelenti, hogy a megfelelő MFA-megoldást kell megvalósítani a felhasználók számára az Integration sandbox-bérlőben. Javasoljuk, hogy az Azure AD biztonsági alapértelmezéseit az MFA biztosítására alkalmazza.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Hogyan beállítani a vészhelyzeti hozzáférési (break Glass) fiókot?

Az ajánlott eljárás az, hogy egy vagy két vészhelyzeti hozzáférési fiókot hozzon létre az Azure AD-bérlő véletlen kizárásának megakadályozása érdekében. A partneri biztonsági követelmények tekintetében minden felhasználó hitelesítése szükséges az MFA használatával. Ez a követelmény azt jelenti, hogy módosítania kell egy vészhelyzeti hozzáférési fiók definícióját. Ez lehet egy olyan fiók, amely egy külső gyártótól származó megoldást használ az MFA-hoz.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Szükséges-e a Active Directory összevonási szolgáltatás (ADFS), ha harmadik féltől származó megoldást használok?

Nem, nem szükséges Active Directory összevonási szolgáltatás (ADFS), ha harmadik féltől származó megoldást használ. Javasoljuk, hogy a megoldás gyártójával együttműködve határozza meg, hogy milyen követelmények vonatkoznak a megoldásra.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Követelmény az Azure AD biztonsági Alapértelmezések engedélyezése?

Nem, nincs szükség az Azure AD biztonsági Alapértelmezések engedélyezésére.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Használható-e feltételes hozzáférés az MFA-követelmények teljesítéséhez?

Igen, a feltételes hozzáférés használatával kényszerítheti az MFA használatát a partner bérlője minden felhasználója, beleértve a szolgáltatásfiókok szolgáltatást is. Mivel azonban a partnernek magas jogosultsági szintűnek kell lennie, biztosítania kell, hogy minden egyes felhasználónak legyen MFA-kihívása minden egyes hitelesítéshez. Ez azt jelenti, hogy nem fogja tudni használni a feltételes hozzáférés funkcióját, amely megkerüli az MFA követelményét.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Az Azure AD Connect által használt szolgáltatásfiók hatással van-e a partneri biztonsági követelményekre?

Nem, a Azure AD Connect által használt szolgáltatásfiók nem érinti a partner biztonsági követelményeit. Ha az MFA érvényesítésének eredményeképpen Azure AD Connect problémát tapasztal, a Microsoft támogatási szolgálatával nyisson meg egy technikai támogatási kérelmet.

## <a name="secure-application-model"></a>Biztonságos alkalmazás modellje

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Kinek kell elfogadnia a biztonságos alkalmazás modelljét a követelmények teljesítése érdekében?

A Microsoft egy biztonságos, méretezhető keretrendszert vezet be a (z) Multi-Factor Authenticationt használó Cloud Solution Provider (CSP) partnerek és a Vezérlőpult-szállítók (CPV) hitelesítéséhez. További információ: [Secure Application Model útmutató](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Minden olyan partner, aki bármely API-val (például Azure Resource Manager, Microsoft Graph, partner Center API stb.) fejlesztett ki egyéni integrációt, vagy az olyan eszközök használatával implementálta az egyéni automatizálást, mint amilyen a PowerShell, el kell fogadnia a [biztonságos alkalmazás-modell keretrendszert](/partner-center/develop/enable-secure-app-model) a Microsoft Cloud Services integrálásához.

### <a name="what-is-the-secure-application-model"></a>Mi a biztonságos alkalmazás modellje?

A Microsoft biztonságos, méretezhető keretrendszert vezet be a felhőalapú megoldások szolgáltatói (CSP) partnerei és a Vezérlőpult-szállítók (CPV) hitelesítéséhez, amely a Multi-Factor Authenticationt használja. További információkért tekintse meg a [Secure Application Model útmutatót](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) .  

### <a name="how-do-i-implement-the-secure-application-model"></a>Hogyan megvalósítani a biztonságos alkalmazás modelljét?

Minden olyan partner, aki bármely API-val (például Azure Resource Manager, Microsoft Graph, partner Center API stb.) fejlesztett ki egyéni integrációt, vagy az olyan eszközök használatával implementálta az egyéni automatizálást, mint amilyen a PowerShell, el kell fogadnia a [biztonságos alkalmazás-modell keretrendszert](/partner-center/develop/enable-secure-app-model) a Microsoft Cloud Services integrálásához. Ennek elmulasztása az MFA-telepítés miatt megszakadhat. A következő források áttekintést nyújtanak a modell bevezetésével kapcsolatban.

- [Az alkalmazás-modell biztonságos áttekintése](/partner-center/develop/enable-secure-app-model)
- [Partneri központ: az alkalmazás-modell biztonságos útmutatója](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partnerek a CSP programban: .NET-mintakód a biztonságos alkalmazás modelljének engedélyezéséhez](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partnerek a CSP programban: a biztonságos alkalmazás modelljét engedélyező Java-mintakód](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [A partneri központ hitelesítési dokumentuma](/partner-center/develop/partner-center-authentication)
- [A partneri központ PowerShell-Multi-Factor Authentication (MFA) dokumentuma](/powershell/partnercenter/multi-factor-auth)

Ha a Vezérlőpultot használja, a biztonságos Application Model-keretrendszer bevezetésével kapcsolatban konzultálnia kell a szállítóval.

A Vezérlőpult gyártóinak be kell jelentkezniük a partner Centerbe a Vezérlőpulton, és [azonnal meg kell](enroll-as-cpv.md) kezdeni a követelmény megvalósítását. Tekintse át a következőt [: a partner Center biztonságos alkalmazás modelljének keretrendszere](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). A Vezérlőpult gyártóinak a hitelesítő adatok helyett el kell fogadniuk és kezelniük kell a CSP-partnerek beleértett hozzájárulásukat.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>A biztonságos alkalmazás modelljét csak a partner Center API/SDK esetében kell megvalósítani?

A többtényezős hitelesítésnek az összes felhasználói fiókra való kényszerítésével hatással lesz a nem interaktív módon futtatandó automatizálásra vagy integrációra. Noha a partneri biztonsági követelmények megkövetelik, hogy engedélyezze a biztonságos alkalmazás modelljét a partner Center API számára, felhasználhatja az automatizálással és az integrációval kapcsolatos második hitelesítési tényező szükségességét.

>[!Note] 
>Az elérni kívánt erőforrásoknak támogatniuk kell a hozzáférés-jogkivonat-alapú hitelesítést.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Olyan Automation-eszközöket használok, mint például a PowerShell. Hogyan megvalósítani a biztonságos alkalmazás modelljét?

A biztonságos alkalmazás modelljét akkor kell megvalósítani, ha az automatizálást nem interaktív módon kívánja futtatni, és a hitelesítéshez szükséges felhasználói hitelesítő adatokra támaszkodik. Lásd: [Secure Application Model | A partner Center PowerShell](/powershell/partnercenter/multi-factor-auth) útmutatást nyújt a keretrendszer megvalósításához.  

>[!Note] 
>Nem minden Automation-eszköz biztosítja a hitelesítést a hozzáférési jogkivonatok használatával. Ha segítségre van szüksége annak megértéséhez, hogy milyen módosításokat kell végeznie, tegye közzé a [partner Center biztonsági útmutatást](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) tartalmazó csoportjának üzeneteit. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Milyen felhasználói hitelesítő adatok szükségesek az alkalmazás rendszergazdája számára az engedélyezési folyamat végrehajtásakor?

Javasoljuk, hogy olyan szolgáltatásfiókot használjon, amely a legalacsonyabb jogosultsági szintű engedélyekkel van társítva. A partner Center API-val kapcsolatban olyan fiókot kell használnia, amely az értékesítési ügynök vagy a rendszergazdai ügynökök szerepkörhöz van rendelve.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Miért adja meg az alkalmazás rendszergazdája a globális rendszergazdai hitelesítő adatokat az engedélyezési folyamat végrehajtásakor?

Ajánlott eljárás a legkevésbé privilegizált identitás használata.  Ez csökkenti a kockázatot. A globális rendszergazdai jogosultságokkal rendelkező fiók használata nem ajánlott, mert az a szükségesnél több engedélyt biztosít.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>CSP-partner vagyok. Hogyan tudni, hogy a Vezérlőpult gyártója (CPV) dolgozik-e a megoldás megvalósításán?

A Vezérlőpult gyártói (CPV) megoldását használó partnerek számára a Cloud Solution Provider (CSP) programban való használatért az Ön felelőssége, hogy konzultáljon a CPV-vel.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Ki a Vezérlőpult gyártója (CPV)?

A Vezérlőpult gyártója egy független szoftvergyártó, amely a CSP-partnerek által a partner Center API-kkal való integrációhoz használható alkalmazásokat fejleszt. A Vezérlőpult gyártója nem CSP-partner, közvetlen hozzáféréssel a partner Center irányítópulthoz vagy API-khoz. Részletes leírás érhető el a [partner Centerben: Secure Applications Model útmutató](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>CPV vagyok. Hogyan regisztrálni?

A Vezérlőpult-gyártó (CPV) beléptetéséhez kövesse az [itt](enroll-as-cpv.md)ismertetett útmutatást.

[CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com)A CPVs csatlakoznia kell a beléptetési hivatkozáshoz, és meg kell adnia egy olyan Microsoft-alkalmazott szponzort, aki üzleti kapcsolatban áll a CPV-vel, vagy ismeri a vállalatát. Például egy partner Development Manager (PDM).

Miután bejelentkezett a partner Centerben, és regisztrálja alkalmazásait, hozzáférhet a partner Center API-khoz. Ha új CPV-t használ, a rendszer egy fiókpartner-értesítésen keresztül kapja meg a homokozóban található adatokat. Miután Microsoft CPV-regisztrációt végzett, és elfogadta a CPV-szerződést, a következőket teheti:

1. Több-bérlős alkalmazás kezelése (alkalmazások hozzáadása a Azure Portalhoz, valamint alkalmazások regisztrálása és regisztrációjának törlése a partner Centerben).

   >[!Note]
   >A CPVs regisztrálnia kell az alkalmazásaikat a partner Centerben, hogy a partner Center API-jai engedélyezve legyenek. Az alkalmazások csak a Azure Portalhez való hozzáadása nem engedélyezi a CPV-alkalmazások számára a partner Center API-kat.

1. A CPV-Profil megtekintése és kezelése.

1. Megtekintheti és kezelheti azokat a felhasználókat, akiknek hozzáférésre van szükségük a CPV-képességekhez. A CPV-nak csak a globális rendszergazda szerepköre lehet.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>A partner Center SDK-t használom. Az SDK automatikusan elfogadja a biztonságos alkalmazás modelljét?

Nem, a [Secure Application Model útmutatójában](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)ismertetett útmutatást kell követnie.

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Létrehozhatok frissítési jogkivonatot a biztonságos alkalmazás modelljéhez olyan fiókokkal, amelyeken nincs engedélyezve az MFA?

Igen, a frissítési token olyan fiókkal hozható létre, amely nem rendelkezik az MFA kényszerített alkalmazásával. Ezt azonban el kell kerülni. Az MFA-t nem engedélyező fiók használatával generált tokenek az MFA követelményei miatt nem férhetnek hozzá az erőforrásokhoz.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Hogyan szerezhetem be az alkalmazás hozzáférési tokent, ha engedélyezzük az MFA használatát?

Követnie kell a [Secure Application Model útmutatót](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) , amely részletesen ismerteti az új biztonsági követelményeknek való megfelelést. Itt megtalálhatja a .NET-mintakód [itt](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) és a Java-mintakód [itt](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)látható.

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>CPV-ként hozzon létre egy Azure AD-alkalmazást a CPV-bérlőben vagy a CSP-partner bérlője?

A CPV-nak létre kell hoznia a Azure Active Directory alkalmazást a beléptetéshez a CPV-ként társított bérlőn.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Csak az alkalmazás hitelesítését használó CSP vagyok. Végre kell hajtani a módosításokat?

Az alkalmazás csak a hitelesítésre van hatással, mivel a felhasználói hitelesítő adatok nem használhatók hozzáférési jogkivonat igényléséhez. Ha a felhasználói hitelesítő adatok meg vannak osztva, akkor a Vezérlőpult szállítóinak (CPVs) el kell fogadniuk a [biztonságos alkalmazás-modell keretrendszert](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) , és ki kell üríteniük a meglévő partneri hitelesítő adatokat.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>A CPV használatával kihasználható az alkalmazás csak hitelesítési stílusa a hozzáférési jogkivonatok beszerzéséhez?

Nem, a Vezérlőpult gyártói partnerei nem tudják használni az alkalmazás csak hitelesítési stílusát, hogy hozzáférési jogkivonatokat kérjenek a partner nevében. Meg kell valósítaniuk a biztonságos alkalmazás modellt, amely az alkalmazás + felhasználó hitelesítési stílusát használja.

## <a name="technical-enforcement"></a>Technikai betartatás

### <a name="what-is-the-activation-of-security-safeguards"></a>Mi a biztonsági óvintézkedések aktiválása?

A Cloud Solution Provider (CSP) program, a Vezérlőpult-szállítók (CPVs) és az Advisors szolgáltatásban részt vevő összes partnernek meg kell valósítania a megfelelő biztonsági követelményeket.

További védelem biztosításához a Microsoft megkezdte a biztonsági óvintézkedések aktiválását, amelyek segítségével a partnerek a többtényezős hitelesítés (MFA) ellenőrzésének megkövetelésével védik a partnereket és ügyfeleiket a jogosulatlan hozzáférés megakadályozása érdekében.  

Sikeresen elvégezte az aktiválást az összes partner bérlője számára a rendszergazdai jogokkal rendelkező (AOBO) funkciók aktiválásához. Ha további segítségre van szükség a partnerek és az ügyfelek számára a Q2 CY2020 megcélzásához, megkezdjük a partner Center-tranzakciók aktiválását a CSP-ben, így a partnerek megvédik a vállalatokat és az ügyfeleket az identitás-lopással kapcsolatos incidensekkel

További információért látogasson el [a partner bérlő oldalának a többtényezős hitelesítés (MFA) meghatalmazása](partner-security-requirements-mandating-mfa.md) című oldalra.

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Harmadik féltől származó MFA-megoldást használok, és blokkolom, mit tegyek?

Annak ellenőrzéséhez, hogy az erőforrásokhoz való hozzáféréshez használt fiók a többtényezős hitelesítéshez lett-e kiválasztva, a [hitelesítési módszer hivatkozási](https://tools.ietf.org/html/rfc8176) jogcímet ellenőrzi, hogy az MFA megjelenjen-e a listáról. Egyes harmadik féltől származó megoldások nem állítják ki ezt a jogcímet, vagy nem tartalmazzák az MFA értékét. Ha a jogcím hiányzik, vagy az MFA értéke nem szerepel a felsorolásban, akkor nem lehet meghatározni, hogy a hitelesített fiókot a rendszer a többtényezős hitelesítéshez vitatta-e. A harmadik féltől származó megoldás gyártójával kell dolgoznia, hogy meghatározza, milyen műveleteket kell végrehajtania, hogy a megoldás kiadja a hitelesítési módszer hivatkozási jogcímet.

Ha nem biztos abban, hogy a harmadik féltől származó megoldás a várt jogcímet állítja-e ki, tekintse meg [a partneri biztonsági követelmények tesztelését](/powershell/partnercenter/test-partner-security-requirements) ismertető témakört.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>Az MFA blokkolja az ügyfelem a AOBO használatával való támogatását, mit tegyek?

A partneri biztonsági követelmények technikai kényszerítését a rendszer ellenőrzi, hogy a hitelesített fiókot a rendszer a többtényezős hitelesítéssel vitatta-e. Ha a fiók nem volt, a rendszer átirányítja a bejelentkezési oldalra, és megkéri, hogy ismételje meg a hitelesítést. Ebben a [többtényezős hitelesítésben (MFA) a partner bérlői](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) dokumentációjában további tapasztalat és útmutatás olvasható. Abban az esetben, ha a tartomány nem összevont, a sikeres hitelesítés után a rendszer felszólítja a többtényezős hitelesítés beállítására. Ha a művelet befejeződött, az ügyfelek az AOBO használatával kezelhetők. Abban a forgatókönyvben, amelyben a tartomány összevont, meg kell győződnie arról, hogy a fiók a többtényezős hitelesítés során kihívást jelent.

## <a name="security-defaults-transition"></a>Biztonsági alapértékek átmenete

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Hogyan válthatok az alapszabályzatok között a biztonsági alapértékekre vagy más MFA-megoldásokra?

A Azure Active Directory (Azure AD) "alapkonfiguráció [" házirendeket a rendszer eltávolítja, és lecseréli](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) a "biztonsági alapértékek" kifejezésre, amely átfogóbb védelmi szabályzatokat biztosít Önnek és ügyfeleinek. A [biztonsági alapértelmezett beállításokkal](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) megvédheti szervezetét az identitás-lopással kapcsolatos biztonsági támadásokkal szemben.

A többtényezős hitelesítés (MFA) implementációja törlődik az alapházirendek kivonása miatt, ha az alapszintű szabályzatok nem váltottak át a biztonsági alapértelmezett házirendre vagy [más MFA-megvalósítási lehetőségekre](partner-security-requirements.md#implementing-multi-factor-authentication). A partner bérlői által az MFA által védett műveleteket végző felhasználókat a rendszer az MFA-ellenőrzés elvégzésére kéri. Tekintse át a részletes útmutatót [itt](partner-security-requirements-mandating-mfa.md).
A megfelelő működéshez és a fennakadások minimalizálásához végezze el az alábbi műveletek egyikét:

- Váltás biztonsági alapértékekre
    - A biztonsági beállítások alapértelmezett házirendje az egyik lehetőség, amelyet a partnerek az MFA megvalósítására használhatnak. Alapszintű biztonsági szintet biztosít, külön díj nélkül.
    - Ismerje meg, hogyan engedélyezheti az MFA-t a szervezete számára az Azure AD-vel, és tekintse át a [biztonsági Alapértelmezések kulcsfontosságú szempontjai](partner-security-requirements.md#security-defaults)
    - Engedélyezze a biztonsági beállítások alapértelmezett házirendjét, ha az megfelel az Ön üzleti igényeinek.
- Áttérés a feltételes hozzáférésre
    - Ha a biztonsági alapértelmezett házirend nem az Ön igényeinek megfelelő, engedélyezze a feltételes hozzáférést. További információkért tekintse át az Azure AD feltételes hozzáférési dokumentációját.

## <a name="key-resources"></a>Fő erőforrások

### <a name="how-to-get-started"></a>Első lépések

- [Partneri biztonsági követelmények: lépésenkénti útmutató](partner-security-requirements.md).
- Kérdéseit és visszajelzéseit a [partner Center biztonsági Orientációs csoportjának](https://aka.ms/MPCSecurityGuidance)irányíthatja.
- Vegyen részt a közelgő partneri munkaidőben és a webes előadásokban. Itt tekintse meg a [részletes ütemtervet és erőforrásokat](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-adopting-secure-application-model"></a>A biztonságos alkalmazás modelljének elfogadására szolgáló erőforrások

- [Az alkalmazás-modell biztonságos áttekintése](/partner-center/develop/enable-secure-app-model)
- [Partneri központ: az alkalmazás-modell biztonságos útmutatója](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partnerek a CSP programban: .NET-mintakód a biztonságos alkalmazás modelljének engedélyezéséhez](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partnerek a CSP programban: a biztonságos alkalmazás modelljét engedélyező Java-mintakód](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [A partneri központ hitelesítési dokumentuma](/partner-center/develop/partner-center-authentication)
- [A partneri központ PowerShell-Multi-Factor Authentication (MFA) dokumentuma](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Támogatás

### <a name="where-can-i-get-support"></a>Hol kaphatok támogatást?

Ha támogatási forrásokat szeretne teljesíteni a biztonsági követelmények teljesítéséhez, ha a partnereknek speciális támogatással (ASfP) rendelkezik, forduljon a Service Account Managerhez; a partneri szerződéssel (PSfP) kapcsolatos Premier szintű támogatás forduljon a Service Account Managerhez és a technikai Account Managerhez.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Hogyan technikai információkat és támogatást nyújt a biztonságos Application Model-keretrendszer bevezetéséhez?

A Azure Active Directory technikai terméktámogatási lehetőségei az MPN előnyein keresztül érhetők el. Az aktív ASfP vagy PSfP-előfizetéshez hozzáféréssel rendelkező partnerek a hozzájuk tartozó beállítások megismerése érdekében a társított fiókkezelő (SAM/TAM) használatával is működhetnek.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Hogyan Kapcsolatfelvétel a támogatási szolgálattal, ha elveszítettem a partneri központhoz való hozzáférést?

Ha egy MFA-probléma miatt elveszíti a hozzáférést, forduljon a bérlő globális rendszergazdájához. A belső informatikai részleg tudni fogja, kik a globális rendszergazdája. 

Ha elfelejtette a jelszavát, a segítségért olvassa el a következőt: [nem sikerült bejelentkeznie](unable-to-sign-in.md) .

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Hol találhatok további információt a gyakori technikai problémákról?

A közös technikai problémákkal kapcsolatos információkat a partner [Center vagy a partner Center API-kat használó partnereknek szóló biztonsági követelményekben](partner-security-requirements.md) találja