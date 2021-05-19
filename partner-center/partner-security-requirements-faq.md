---
title: Partnerekre vonatkozó biztonsági követelmények – gyakori kérdések
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gyakori kérdések a partnerek biztonsági követelményeiről – mik ezek, hogyan valósítják meg azokat a partnerek, és hogyan tudhatja, hogy teljesültek-e.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 174c56ce9bb5fb3d9d92c1ef18af73479619f4bb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145881"
---
# <a name="common-questions-about-partner-security-requirements"></a>A partnerek biztonsági követelményeivel kapcsolatos gyakori kérdések

**Megfelelő szerepkörök:** Minden Partnerközpont felhasználó

Ez a cikk a partnerbiztonsági követelményekkel kapcsolatos néhány gyakori [kérdésre ad választ.](partner-security-requirements.md)

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>Mik a partnerekre vonatkozó biztonsági követelmények, és miért érdemes azokat a partnerek megvalósítani?

A nagyobb és folyamatos biztonsági és adatvédelmi védelmi intézkedések az egyik legfontosabbak, és továbbra is segítünk a partnereknek az ügyfeleik és bérlőik védelmében. Továbbra is kifinomultabb, egyre több biztonsági támadást látunk, amelyek elsősorban az identitásbiztonsági incidensekkel kapcsolatosak. Mivel a megelőző intézkedések kulcsfontosságú szerepet játszanak a biztonsági támadások elleni [](partner-security-requirements.md) általános védelmi stratégiában, 2019-ben bevezettük a kötelező biztonsági követelményeket. A Felhőszolgáltató (CSP) programban részt vevő összes partnernek, Vezérlőpult szállítónak és tanácsadónak meg kell felelnie a követelményeknek a megfelelőség érdekében.

### <a name="what-are-the-key-timelines-and-milestones"></a>Mik a legfontosabb ütemtervek és mérföldkövek?

Az e biztonsági követelményekhez kapcsolódó feltételeket, beleértve az ütemterveket és a mérföldköveket is, az [Microsoft Partnerszerződés.](microsoft-partner-agreement.md) Ezeket a biztonsági követelményeket a lehető leghamarabb implementálja, hogy összhangban maradjon a CSP-programban való részvételével.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Mi történik, ha nem implementáljam ezeket a partnerbiztonsági követelményeket?

A Microsoft Partnerszerződés megköveteli a többtényezős hitelesítést a felhasználói fiókoknál, és a biztonságos alkalmazásmodellt kell használnia a Partnerközpont API-val való interakcióhoz. 

Azok a partnerek, akik nem tartják be ezeket a biztonsági eljárásokat, elveszítheti a CSP-programban való tranzakciós képességüket, vagy ügyfélbérlőket kezelhetnek rendszergazdai jogosultságok delegálásával.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>A biztonsági követelmények az összes földrajzi régióra vonatkoznak?

Igen, a biztonsági követelmények minden földrajzi régióra érvényesek. Határozottan javasoljuk, hogy a szuverén felhőn (AZ EGYESÜLT Államok kormányán és Németországán) keresztül tranzakciós partnerek azonnal léptethét léptesd be ezeket az új biztonsági követelményeket. Ezek a partnerek azonban jelenleg nem szükségesek a biztonsági követelmények követelményeknek való megfeleléshez. A Microsoft a jövőben további részleteket nyújt a szuverén felhőkre vonatkozó biztonsági követelmények betartatásával kapcsolatban.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Lehetséges kizárást kapni egy fiókhoz?

Nem, nem lehet kizárni egyetlen felhasználói fiókot sem a többtényezős hitelesítés (MFA) kényszerítés alól. Mivel a partneri jogosultságok rendkívül magas szintűek, a Microsoft Partnerszerződés megköveteli a többtényezős hitelesítést a partnerbérlő minden felhasználói fiókjához.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Hogyan, hogy megfeleltem-e a partnerek biztonsági követelményeinek?

Végezze el a következő lépéseket:

- Meg kell felelnie a partner biztonsági követelményeiben felvázolt [összes követelménynek.](partner-security-requirements.md)
- Gondoskodnia kell arról, hogy a partnerbérlő összes felhasználói fiókja többtényezős hitelesítéssel rendelkezik.

Annak érdekében, hogy azonosítsuk azokat a fő [](https://partner.microsoft.com/commerce/security/compliance) területeket, ahol műveleteket lehet végrehajtani, a biztonsági követelmények állapotjelentését biztosítjuk, amely a Partnerközpont.

Az állapotjelentéssel kapcsolatos további információkért lásd a [partnerek biztonsági követelményeinek állapotát.](partner-security-compliance.md)

## <a name="required-actions"></a>Szükséges műveletek

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Melyek a követelményeknek való megfeleléshez szükséges legfontosabb műveletek?

A CSP program összes partnerének (közvetlen számla, közvetett szolgáltató és közvetett viszonteladó), tanácsadónak és Vezérlőpult beszállítónak meg kell felelnie a követelményeknek.

1. **MFA kényszerítés minden felhasználó számára**

    A CSP-program összes partnerének, tanácsadójának és Vezérlőpult beszállítójának kötelező az MFA kényszerítve a partnerbérlő összes felhasználója számára.

    További szempontok:

    - A közvetett szolgáltatóknak közvetett viszonteladókkal kell együtt dolgozniuk a Partnerközpont ha még nem tette meg, és arra kell ösztönözniük a viszonteladókat, hogy felelniük kell a követelményeknek.
    - Az Azure MFA ingyenesen elérhetővé válik a partnerbérlő összes felhasználója számára az Azure AD biztonsági alapértelmezései alapján, az időalapú egyszeres jelszavakat (TOTP) támogató hitelesítő alkalmazás egyetlen ellenőrzési módszerével.
    - További ellenőrzési módszerek érhetők el a prémium szintű Azure Active Directory [](/azure/active-directory/fundamentals/active-directory-get-started-premium) SKUS-okkal, ha más módszerekre, például telefonhívásra vagy SMS-üzenetre van szükség.
    - A partnerek harmadik féltől származó MFA-megoldást is használhatnak minden fiókhoz a Microsoft kereskedelmi felhőszolgáltatáshoz való hozzáféréskor.

2. **Az biztonságos alkalmazásmodell keretrendszerének elfogadása**

    Minden olyan partnernek, amely api-k (például Azure Resource Manager, Microsoft Graph, Partnerközpont API stb.) használatával fejlesztett egyéni integrációt, vagy egyéni automatizálást [](/partner-center/develop/enable-secure-app-model) valósított meg olyan eszközökkel, mint a PowerShell, be kell fogadnia az biztonságos alkalmazásmodell-keretrendszert a Microsoft-felhőszolgáltatásokkal való integrációhoz. Ennek elmulasztása az MFA üzembe helyezése miatt kimaradást okozhat. Az alábbi források áttekintést és útmutatást nyújtanak a modell alkalmazásával kapcsolatban.

    - [biztonságos alkalmazásmodell áttekintés](/partner-center/develop/enable-secure-app-model)
    - [Partnerközpont: biztonságos alkalmazásmodell útmutató](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partnerek a CSP-programban: .NET-mintakód az biztonságos alkalmazásmodell](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partnerek a CSP-programban: Java-mintakód az biztonságos alkalmazásmodell](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Partnerközpont hitelesítési dokumentum](/partner-center/develop/partner-center-authentication)
    - [Partnerközpont PowerShell Multi-Factor Authentication (MFA) dokumentációja](/powershell/partnercenter/multi-factor-auth)

    Ha a keretrendszer bevezetésével kapcsolatos vezérlőpultot használ, forduljon a szállítóhoz biztonságos alkalmazásmodell kapcsolatban.

    A vezérlőpult szállítóinak [](enroll-as-cpv.md) elő kell állítaniuk Partnerközpont a vezérlőpult szállítóiként, és azonnal el kell kezdeniük ennek a követelménynek a megvalósítását. Tekintse meg a [Partnerközpont: biztonságos alkalmazásmodell keretrendszert.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) A vezérlőpult szállítóinak el kell fogadniuk és kezelniük kell a CSP-partnerek hozzájárulását a hitelesítő adatok helyett, és minden meglévő CSP-partner hitelesítő adatait véglegesen el kell véglegesen kiürítenie.

## <a name="multi-factor-authentication"></a>Többtényezős hitelesítés

### <a name="what-is-multi-factor-authentication-mfa"></a>Mi az a többtényezős hitelesítés (MFA)?

Az MFA egy biztonsági mechanizmus, amely több kötelező biztonsági és érvényesítési eljáráson keresztül hitelesíti az egyéneket. Úgy működik, hogy a következő hitelesítési módszerek közül kettő vagy több szükséges:

- Valami, amit ismer (általában jelszó)
- Valami, ami az Ön számára van (egy megbízható eszköz, amely nem egyszerűen duplikálható, például telefon)
- Valami, ami Ön (biometrikus)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Milyen költséggel jár az MFA engedélyezése?

A Microsoft az Azure AD biztonsági alapértelmezések implementációja révén költség nélkül biztosítja az MFA-t. Az MFA ezen verziójának használatával elérhető egyetlen ellenőrzési lehetőség a hitelesítő alkalmazás. Ha telefonhívásra vagy SMS-üzenetre [](/azure/active-directory/fundamentals/active-directory-get-started-premium) van szükség, akkor prémium szintű Azure Active Directory licenc szükséges. Másik lehetőségként egy harmadik féltől származó megoldással is biztosíthatja az MFA-t a partnerbérlő minden felhasználója számára – ebben az esetben az Ön felelőssége, hogy biztosítsa az MFA-megoldás kikényszerülét és a megfelelőséget.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Milyen műveleteket kell tennem, ha már van MFA-megoldásom?

Ezen biztonsági követelmények alapján a partnerbérlő felhasználóinak MFA-hitelesítést kell végezniük a Microsoft kereskedelmi felhőszolgáltatáshoz való hozzáféréskor. Ezeknek a követelményeknek a teljesítéséhez harmadik féltől származó megoldások is használhatók. A Microsoft már nem biztosít ellenőrzési tesztelést a független identitásszolgáltatók számára a Azure Active Directory. A termék együttműködésének tesztelésére tekintse meg ezeket az [irányelveket.](https://www.microsoft.com/download/details.aspx?id=56843)

> [!IMPORTANT]
> Harmadik féltől származó megoldás használata esetén fontos ellenőrizni, hogy a megoldás kiíratja-e az MFA-értéket tartalmazó hitelesítési módszerre (AMR) vonatkozó jogcímet. A [harmadik féltől](/powershell/partnercenter/test-partner-security-requirements) származó megoldás várt jogcímének ellenőrzésével kapcsolatos részletekért tekintse meg a Partnerbiztonsági követelmények tesztelése.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Több partnerbérlőt használok a tranzakcióhoz. Mindegyiken implementáljam az MFA-t?

Igen, az MFA-t a CSP-programhoz Azure Active Directory Advisor-programhoz társított összes bérlőhöz ki kell kényszeríte. A licenc prémium szintű Azure Active Directory vásárláshoz minden egyes bérlőben Azure Active Directory licenccel kell Azure Active Directory felhasználók számára. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>A partnerbérlőm minden felhasználói fiókjának kötelezően ki kell kényszerítve az MFA-t?

Igen, minden felhasználónak ki kell kényszerítve az MFA-t. Ha azonban az Azure AD alapértelmezett biztonsági beállításokat használja, nincs szükség további műveletre, mivel ez a funkció minden felhasználói fiók esetében kényszeríti az MFA-t. A biztonsági alapértékek engedélyezése ingyenes és egyszerű módja annak, hogy a felhasználói fiókok MFA-kompatibilisek, és ne legyen hatással az MFA kényszerítésében.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Közvetlen számlázási partner vagyok a Microsoftnál. Mit kell tennem?

A közvetlen számlázási Felhőszolgáltató a partnerbérlő minden felhasználója számára kötelezően ki kell kényszerítenie az MFA-t.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Közvetett viszonteladó vagyok, és csak terjesztőként tudok tranzakciót. Továbbra is engedélyezni kell az MFA-t?

Minden közvetett viszonteladónak kötelező az MFA-t kikényszerítenie a partnerbérlő minden felhasználója számára. A közvetett viszonteladónak engedélyeznie kell az MFA-t.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Nem használom a Partnerközpont API-t. Továbbra is implementáljam az MFA-t?

Igen, ez a biztonsági követelmény minden felhasználóra, beleértve a partner-rendszergazdai felhasználókat és a partnerbérlő végfelhasználóira vonatkozó követelményeket.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Mely külső gyártók nyújtanak MFA-megoldásokat a Azure Active Directory?

Az MFA-szállítók és -megoldások áttekintésekor a partnereknek gondoskodniuk kell arról, hogy a választott megoldás kompatibilis legyen a Azure Active Directory.

A Microsoft a továbbiakban nem biztosít ellenőrzési tesztelést független identitásszolgáltatók számára, hogy azok kompatibilisek Azure Active Directory. Ha tesztelni szeretné a terméket az együttműködési képesség szempontjából, tekintse meg ezeket az [irányelveket.](https://www.microsoft.com/download/details.aspx?id=56843)

További információkért tekintse meg az [Azure AD összevonás kompatibilitási listáját.](/azure/active-directory/hybrid/how-to-connect-fed-compatibility)

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Hogyan tesztelheti az MFA-t az integrációs tesztkészletben?

Engedélyezni kell az Azure AD biztonsági alapértelmezések funkcióját, vagy használhat egy harmadik féltől származó, összevonást használó megoldást.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Befolyásolja az MFA engedélyezése, hogy hogyan kommunikálok az ügyfél bérlőjéhez?

Nem. Ezeknek a biztonsági követelményeknek a teljesítése nincs hatással az ügyfelek kezelésére. A delegált felügyeleti műveletek végrehajtása nem szakad meg.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Az ügyfeleimre vonatkoznak a partnerek biztonsági követelményei?

Nem szükséges megkövetelni az MFA kényszerítését az ügyfél Azure AD-bérlőiben minden felhasználónál. Javasoljuk azonban, hogy minden ügyféllel együtt döntse el, hogyan tudja a legjobban megvédeni a felhasználóit.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Kizárható-e egy felhasználó az MFA-követelményből?

Nem, a partnerbérlőben minden felhasználónak, beleértve a szolgáltatásfiókokat is, az MFA használatával kell hitelesítenie.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Vonatkoznak a partnerbiztonsági követelmények az integrációs védőfalra?

Igen, a partnerbiztonsági követelmények az integrációs védőfalra vonatkoznak. Ez azt jelenti, hogy a megfelelő MFA-megoldást kell megvalósítania az integrációs védőfal bérlő felhasználói számára. Javasoljuk, hogy implementálja az Azure AD alapértelmezett biztonsági beállításokat az MFA-hoz.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Hogyan(vészhelyzeti) fiókot konfigurál?

Az ajánlott eljárás egy vagy két vészelérési fiók létrehozása, amely megakadályozza, hogy véletlenül kizárják őket az Azure AD-bérlőből. A partner biztonsági követelményeinek megfelelően minden felhasználónak MFA használatával kell hitelesítenie magát. Ez a követelmény azt jelenti, hogy módosítania kell egy vészelérési fiók definícióját. Ez lehet egy olyan fiók, amely külső megoldást használ az MFA-hez.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Szükség Active Directory összevonási szolgáltatás (ADFS) a harmadik féltől származó megoldás használata esetén?

Nem, nem szükséges külön Active Directory összevonási szolgáltatás (ADFS) használata, ha harmadik féltől származó megoldást használ. Javasoljuk, hogy a megoldás gyártójával együtt döntse el, milyen követelmények vonatkoznak a megoldásra.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Követelmény az Azure AD alapértelmezett biztonsági alapértelmezésének engedélyezése?

Nem, nem kötelező engedélyezni az Azure AD alapértelmezett biztonsági beállítását.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Használható feltételes hozzáférés az MFA-követelménynek való megfelelőséghez?

Igen, feltételes hozzáféréssel kényszerítheti az MFA-t a partnerbérlő minden felhasználójára, beleértve a szolgáltatásfiókokat is. Mivel azonban partnerként rendkívül magas jogosultsági szintű, ügyelnünk kell arra, hogy minden felhasználónak minden egyes hitelesítéshez MFA-kihívása legyen. Ez azt jelenti, hogy nem fogja tudni használni a feltételes hozzáférés funkcióját, amely megkerüli az MFA követelményét.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Hatással lesznek a Azure AD Connect által használt szolgáltatásfiókra a partner biztonsági követelményei?

Nem, az Azure AD Connect által használt szolgáltatásfiókra nem lesznek hatással a partner biztonsági követelményei. Ha az MFA kényszerítés Azure AD Connect problémákat tapasztal a hitelesítéssel kapcsolatban, nyisson meg egy technikai támogatási kérést a Microsoft ügyfélszolgálatával.

## <a name="secure-application-model"></a>biztonságos alkalmazásmodell

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Kiknek érdemes a biztonságos alkalmazásmodellt a követelményeknek megfelelően befogadni?

A Microsoft egy biztonságos, skálázható keretrendszert vezet be a többtényezős hitelesítést használó Felhőszolgáltató-partnerek és Vezérlőpult-szállítók (CPV) hitelesítéséhez. További információért tekintse meg a biztonságos alkalmazásmodell [útmutatót.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) Minden olyan partnernek, amely api-k (például Azure Resource Manager, Microsoft Graph, Partnerközpont API stb.) használatával fejlesztett egyéni integrációt, vagy egyéni automatizálást [](/partner-center/develop/enable-secure-app-model) valósított meg olyan eszközökkel, mint a PowerShell, be kell fogadnia az biztonságos alkalmazásmodell-keretrendszert a Microsoft-felhőszolgáltatásokkal való integrációhoz.

### <a name="what-is-the-secure-application-model"></a>Mi a biztonságos alkalmazásmodell?

A Microsoft egy biztonságos, skálázható keretrendszert vezet be a Felhőszolgáltató-partnerek és Vezérlőpult-szállítók (CPV) hitelesítéséhez, amely a Multi-Factor Authenticationt használja. További információt [biztonságos alkalmazásmodell útmutatóban.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)  

### <a name="how-do-i-implement-the-secure-application-model"></a>Hogyan implementálja a biztonságos alkalmazásmodell?

Minden olyan partnernek, aki api-k (például Azure Resource Manager, Microsoft Graph, Partnerközpont API stb.) használatával fejlesztett egyéni integrációt, vagy egyéni automatizálást valósított meg olyan eszközökkel, mint a PowerShell, be kell fogadnia az [biztonságos alkalmazásmodell](/partner-center/develop/enable-secure-app-model) keretrendszert a Microsoft-felhőszolgáltatásokkal való integrációhoz. Ennek elmulasztása az MFA üzembe helyezése miatt kimaradást okozhat. Az alábbi források áttekintést és útmutatást nyújtanak a modell alkalmazásával kapcsolatban.

- [biztonságos alkalmazásmodell áttekintés](/partner-center/develop/enable-secure-app-model)
- [Partnerközpont: biztonságos alkalmazásmodell útmutató](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partnerek a CSP-programban: .NET-mintakód az biztonságos alkalmazásmodell](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partnerek a CSP-programban: Java-mintakód a biztonságos alkalmazásmodell](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Partnerközpont dokumentum](/partner-center/develop/partner-center-authentication)
- [Partnerközpont PowerShell Multi-Factor Authentication (MFA) dokumentum](/powershell/partnercenter/multi-factor-auth)

Ha vezérlőpultot használ, akkor a szállítóval kell egyeztetni a biztonságos alkalmazásmodell bevezetéséről.

A vezérlőpult szállítóinak [](enroll-as-cpv.md) elő kell állítaniuk Partnerközpont a vezérlőpult szállítóiként, és azonnal el kell kezdeniük ennek a követelménynek a megvalósítását. Tekintse meg a [Partnerközpont: biztonságos alkalmazásmodell keretrendszert.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) A vezérlőpult szállítóinak el kell fogadniuk és kezelniük kell a CSP-partnerek hozzájárulását a hitelesítő adatok helyett, és az összes meglévő CSP-partner hitelesítő adatait véglegesen ki kell kiürítenünk.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>A biztonságos alkalmazásmodell csak a Partnerközpont API/SDK esetében kell megvalósítani?

Ha minden felhasználói fiókra többtényezős hitelesítést kényszerít ki, az hatással lesz a nem interaktív módon futtatni kívánt automatizálásra vagy integrációra. Bár a partnerbiztonsági követelmények megkövetelik a biztonságos alkalmazásmodell engedélyezését a Partnerközpont API-hoz, arra is használható, hogy az automatizálással és integrációval második hitelesítési tényezőre legyen szükség.

>[!Note] 
>Az elért erőforrásoknak támogatniuk kell a hozzáférési jogkivonat-alapú hitelesítést.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Automatizálási eszközöket használok, például a PowerShellt. Hogyan implementálja a biztonságos alkalmazásmodell?

Akkor kell implementálja a biztonságos alkalmazásmodell ha az automatizálás nem interaktív módon, és a hitelesítéshez felhasználói hitelesítő adatokra támaszkodik. Lásd: [biztonságos alkalmazásmodell | Partnerközpont a Keretrendszer](/powershell/partnercenter/multi-factor-auth) implementálja a PowerShellt.  

>[!Note] 
>Nem minden automatizálási eszköz teszi lehetővé a hozzáférési jogkivonatokkal való hitelesítést. Ha segítségre van szüksége a [Partnerközpont csoportban,](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) tegye közzé az üzenetet. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Milyen felhasználói hitelesítő adatokat kell megadnia az alkalmazás rendszergazdájának a hozzájárulási folyamat végrehajtásakor?

Javasoljuk, hogy olyan szolgáltatásfiókot használjon, amely a legkevesebb kiemelt jogosultsággal rendelkezik. A Partnerközpont API-val kapcsolatban olyan fiókot kell használnia, amely az Értékesítési ügynök vagy a Rendszergazdai ügynökök szerepkörhöz van hozzárendelve.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Miért ne adja meg az alkalmazás-rendszergazda a globális rendszergazdai felhasználói hitelesítő adatokat a hozzájárulási folyamat végrehajtásakor?

Ajánlott a legkevésbé emelt szintű identitást használni.  Ez csökkenti a kockázatokat. Nem ajánlott olyan fiókot használni, amely globális rendszergazdai jogosultságokkal rendelkezik, mert ez a szükségesnél több engedélyt biztosít.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>CSP-partner vagyok. Hogyan, hogy a Vezérlőpult szállítóm (CPV) dolgozik-e a megoldás megvalósításán vagy sem?

A Felhőszolgáltató (CSP) programban való tranzakcióhoz Vezérlőpult CPV-megoldást használó partnereknek az Ön felelőssége, hogy kapcsolatba ássa a CPV-vel.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Ki az a Vezérlőpult szállító (CPV)?

A Vezérlőpult szállító egy független szoftverszállító, amely CSP-partnerek által használható alkalmazásokat fejleszt a Partnerközpont API-jával való integrációhoz. A Vezérlőpult szállító nem CSP-partner, aki közvetlen hozzáféréssel rendelkezik a Partnerközpont irányítópultjához vagy API-jához. Részletes leírást a következő útmutatóban Partnerközpont: Biztonságos alkalmazások [modell útmutatója.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)

### <a name="i-am-a-cpv-how-do-i-enroll"></a>CPV vagyok. Hogyan van regisztrálva?

A vezérlőpult szállítójaként (CPV) való regisztráláshoz kövesse az itt található [irányelveket.](enroll-as-cpv.md)

A CPV-knek kapcsolatba kell lépniük a kapcsolattal, hogy megkapják a regisztrációs hivatkozást, és meg kell adniuk egy Microsoft-alkalmazott szponzorát, aki üzleti kapcsolatban áll a CPV-vel, vagy ismeri [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) a vállalkozását. Például egy partnerfejlesztési vezető (PDM).

Miután regisztrált a Partnerközpont és regisztrálta az alkalmazásokat, hozzáférhet a Partnerközpont API-khoz. Ha Ön új CPV- Partnerközpont kapja meg a sandbox adatait. Miután Microsoft CPV-ként regisztrált, és elfogadta a CPV-szerződést, a következőt teheti:

1. Több-bérlős alkalmazás kezelése (alkalmazások hozzáadása a Azure Portal és alkalmazások regisztrálása és regisztrációjának Partnerközpont).

   >[!Note]
   >A CPV-knek regisztrálniuk kell az Partnerközpont, hogy engedélyt kapnak Partnerközpont API-kra. Az alkalmazásoknak a Azure Portal való hozzáadása önmagában nem engedélyezi a CPV-alkalmazásokat Partnerközpont API-k számára.

1. A CPV-profil megtekintése és kezelése.

1. Megtekintheti és kezelheti a CPV-képességekhez hozzáféréssel bíró felhasználókat. A CPV-k csak globális rendszergazdai szerepkört kaphatnak.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>A következőt Partnerközpont SDK. Az SDK automatikusan be fogja biztonságos alkalmazásmodell?

Nem, kövesse az útmutatóban megadott [biztonságos alkalmazásmodell.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Létrehozhatok frissítési jogkivonatot a biztonságos alkalmazásmodellhez olyan fiókokkal, amelyeken nincs engedélyezve az MFA?

Igen, a frissítési jogkivonatok olyan fiókkal is generálhatóak, amely nem rendelkezik kötelezően az MFA-val. Ez azonban kerülendő. Az MFA-t nem engedélyező fiókkal létrehozott jogkivonatok az MFA követelményei miatt nem fognak tudni hozzáférni az erőforrásokhoz.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Hogyan szerezze be az alkalmazás a hozzáférési jogkivonatot, ha engedélyezem az MFA-t?

Kövesse az útmutatóban [biztonságos alkalmazásmodell útmutatót,](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) amely részletesen ismerteti ennek a lépését, miközben megfelel az új biztonsági követelményeknek. A .NET-mintakódot [](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) itt, a Java-mintakódot pedig itt [találja.](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>CPV-ként létrehozhatok Azure AD-alkalmazást a CPV-bérlőnkben vagy a CSP-partner bérlőjeként?

A CPV-nek létre kell hoznia a Azure Active Directory-alkalmazást a CPV-ként való regisztrációjukhoz társított bérlőben.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Olyan CSP vagyok, amely csak alkalmazáshitelesítést használ. Módosítanom kell valamit?

A csak alkalmazáson belüli hitelesítés nincs hatással, mivel a rendszer nem használja a felhasználói hitelesítő adatokat hozzáférési jogkivonat kéréséhez. Ha a felhasználói hitelesítő adatok meg vannak osztva, akkor a vezérlőpultok szállítóinak (CPV-knek) be kell tartaniuk a [biztonságos alkalmazásmodell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) keretrendszert, és véglegesen ki kell tisztítaniuk a meglévő partneri hitelesítő adataikat.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>CPV-ként az alkalmazás csak hitelesítési stílusát használva kaphatok hozzáférési jogkivonatokat?

Nem, Vezérlőpult szállítói partnerek nem tudják használni az alkalmazás csak hitelesítési stílusát hozzáférési jogkivonatok kéréséhez a partner nevében. Implementálja a biztonságos alkalmazásmodellt, amely az alkalmazást és a felhasználóhitelesítési stílust használja.

## <a name="technical-enforcement"></a>Technikai kényszerítési

### <a name="what-is-the-activation-of-security-safeguards"></a>Mi a biztonsági védelmi intézkedések aktiválása?

A Felhőszolgáltató (CSP) programban részt vevő összes partnernek, a Vezérlőpult Vendors (CPV-knek) és az Advisornak implementálja a kötelező biztonsági követelményeket a megfelelőség érdekében.

A további védelem biztosítása érdekében a Microsoft megkezdte a biztonsági védelmi intézkedések aktiválását, amely segít a partnereknek a bérlőik és ügyfeleik védelmében a többtényezős hitelesítés (MFA) ellenőrzését a jogosulatlan hozzáférés megakadályozása érdekében.  

Sikeresen befejeztünk egy rendszergazdai (AOBO) képességek aktiválását az összes partnerbérlő számára. A partnerek és ügyfelek 2020. 2. negyedévét célzó további védelem érdekében megkezdjük az aktiválást a CSP-ben az Partnerközpont-tranzakciókhoz, így segítünk a partnereknek megvédeni vállalatukat és ügyfeleiket az identitáslopásos incidensek ellen.

További információkért lásd a partnerbérlő többtényezős [hitelesítésének (MFA) frissítését.](partner-security-requirements-mandating-mfa.md)

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Külső MFA-megoldást használok, és le vagyok tiltva. Mit tegyek?

Annak ellenőrzéséhez, hogy a fiók többtényezős hitelesítése igényelte-e az erőforrásokhoz való hozzáférést, ellenőrizni fogjuk a hitelesítési módszerre vonatkozó hivatkozási jogcímet annak ellenőrzésére, hogy az MFA szerepel-e a listán. [](https://tools.ietf.org/html/rfc8176) Egyes külső megoldások nem állítják ki ezt a jogcímet, vagy nem tartalmazzák az MFA-értéket. Ha a jogcím hiányzik, vagy az MFA-érték nem szerepel a listában, akkor nincs mód annak megállapítására, hogy a hitelesített fiók többtényezős hitelesítést igényelt-e. A külső megoldás szállítójával együtt kell meghatároznia, hogy milyen műveleteket kell tenni, hogy a megoldás kiadja a hitelesítési módszerre vonatkozó referenciaigénylést.

Ha [nem biztos abban,](/powershell/partnercenter/test-partner-security-requirements) hogy a harmadik féltől származó megoldás a várt jogcímet állítja-e ki, tekintse meg a Partnerbiztonsági követelmények tesztelése.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>Az MFA nem támogatja az ügyfél AOBO-t használó támogatását. Mit tegyek?

A rendszer ellenőrzi a partnerbiztonsági követelmények technikai érvényesítését, ha a hitelesített fióknál többtényezős hitelesítést kérnek. Ha a fiók még nem volt, akkor a rendszer átirányítja a bejelentkezési oldalra, és újra kéri a hitelesítést. További tapasztalatokat és útmutatást a partnerbérlői dokumentáció többtényezős [hitelesítésének (MFA)](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) a használatával kapcsolatos dokumentációjában talál. Ha a tartomány nincs összefésülve, a sikeres hitelesítés után a rendszer kérni fogja a többtényezős hitelesítés beállítását. Ennek befejezése után az AOBO használatával kezelheti az ügyfeleket. Ha a tartomány összevont, gondoskodnia kell arról, hogy a fiók többtényezős hitelesítést igényel.

## <a name="security-defaults-transition"></a>Biztonsági alapértékek váltása

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Hogyan lehet átváltanom az alapkonfigurációról az alapértelmezett biztonsági szabályokra vagy más MFA-megoldásokra?

Azure Active Directory (Azure AD) ["alapkonfiguráció"](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) szabályzatai el vannak távolítva, és a "biztonsági alapértékek" váltják fel, amely egy átfogóbb védelmi szabályzatkészlet Az Ön és ügyfelei számára. [A biztonsági alapértelmezések](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) segíthetnek megvédeni a szervezetet az identitáslopásos biztonsági támadásoktól.

A többtényezős hitelesítés (MFA) implementációja el lesz távolítva az alapkonfiguráció szabályzatának kiesása miatt, ha még nem tért át az alapkonfigurációról az alapértelmezett biztonsági szabályzatra vagy más MFA-implementációra. [](partner-security-requirements.md#implementing-multi-factor-authentication) A partnerbérlőkben az MFA által védett műveleteket végző felhasználókat a rendszer az MFA-ellenőrzés elvégzésére kéri. A részletesebb útmutatást itt [tekintse át.](partner-security-requirements-mandating-mfa.md)
A megfelelőség és a fennakadások minimalizálása érdekében a következő műveletek egyikét kell követnie:

- Váltás az alapértelmezett biztonsági beállításokra
    - A biztonsági alapértelmezett házirend az egyik lehetőség, amelynél a partnerek dönthetnek az MFA implementáljanak. Alapszintű biztonságot kínál többletköltségek nélkül.
    - Ismerje meg, hogyan engedélyezheti az MFA-t a szervezet számára az Azure AD-val, és tekintse át az alapértelmezett biztonsági [szempontokat.](partner-security-requirements.md#security-defaults)
    - Engedélyezze az alapértelmezett biztonsági szabályzatot, ha az megfelel az üzleti igényeinek.
- Váltás feltételes hozzáférésre
    - Ha a biztonsági alapértelmezett szabályzat nem megfelelő az igényeinek, engedélyezze a feltételes hozzáférést. További információért tekintse át az Azure AD feltételes hozzáférés dokumentációját.

## <a name="key-resources"></a>Fő erőforrások

### <a name="how-to-get-started"></a>Első lépések

- [Partnerekre vonatkozó biztonsági követelmények: részletes útmutató.](partner-security-requirements.md)
- Kérdéseit és visszajelzéseit ebben a [Partnerközpont biztonsági útmutatási csoportban küldheti el.](https://aka.ms/MPCSecurityGuidance)
- Részt vehet a partneri munkaidőben és webináriumban. A részletes [ütemezést és erőforrásokat itt ellenőrizheti.](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)

### <a name="resources-for-adopting-secure-application-model"></a>Források a biztonságos alkalmazásmodellek alkalmazásához

- [biztonságos alkalmazásmodell áttekintés](/partner-center/develop/enable-secure-app-model)
- [Partnerközpont: biztonságos alkalmazásmodell útmutató](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partnerek a CSP-programban: .NET-mintakód az biztonságos alkalmazásmodell](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partnerek a CSP-programban: Java-mintakód a biztonságos alkalmazásmodell](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Partnerközpont dokumentum](/partner-center/develop/partner-center-authentication)
- [Partnerközpont PowerShell Multi-Factor Authentication (MFA) dokumentum](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Támogatás

### <a name="where-can-i-get-support"></a>Hol kaphatok támogatást?

Ha a biztonsági követelményeknek megfelelő támogatási forrásokkal rendelkezik, ha speciális támogatással rendelkezik a partnerek számára (ASfP), forduljon a Service Account Managerhez; a Premier szintű támogatás szerződéshez (PSfP) való csatlakozáshoz forduljon a Service Account Managerhez és a műszaki fiókkezelőhöz.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Hogyan információ és támogatás a biztonságos alkalmazásmodell-keretrendszer alkalmazásához?

A technikai terméktámogatási lehetőségek Azure Active Directory MPN-előnyei között érhetők el. Azok a partnerek, akik aktív ASfP- vagy PSfP-előfizetéshez férnek hozzá, a társított fiókkezelőjükkel (SAM/TAM) dolgozhatnak, hogy a lehető legjobban megértsék a számukra elérhető lehetőségeket.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Hogyan kapcsolatba lépni az ügyfélszolgálattal, ha nem tudok hozzáférni Partnerközpont?

Ha egy MFA-probléma miatt elveszíti a hozzáférést, lépjen kapcsolatba a bérlő globális rendszergazdával. A belső IT-részleg meg tudja majd mondani, hogy ki a globális rendszergazda. 

Ha elfelejtette a jelszavát, [segítségért](unable-to-sign-in.md) olvassa el a Nem lehet bejelentkezni részt.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Hol találhatok további információt a gyakori technikai problémákról?

A gyakori technikai problémákra vonatkozó információk a partnerbiztonsági követelmények között találhatók, Partnerközpont API-kat Partnerközpont [partnerek számára](partner-security-requirements.md)