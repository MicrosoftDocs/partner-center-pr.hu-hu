---
title: Partnerekre vonatkozó biztonsági követelmények
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bevezeti a partnerekre vonatkozó biztonsági követelményeket a többtényezős hitelesítés (MFA) engedélyezéséhez és a biztonságos alkalmazásmodell bevezetéséhez.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 201ea34d30814974936da032805f1ee7dfa590be
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145847"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Biztonsági követelmények a Partnerközpont vagy Partnerközpont API-k használatával

**Megfelelő szerepkörök:** Minden Partnerközpont felhasználó

Ez a cikk ismerteti a Felhőszolgáltató-programban részt vevő tanácsadók, Vezérlőpult-szállítók és partnerek kötelező biztonsági követelményeit, valamint a hitelesítési lehetőségeket és egyéb biztonsági szempontokat. Az adatvédelmi védelem és a biztonság az egyik legfontosabb prioritásunk. Tudjuk, hogy a legjobb védelem a megelőzés, és hogy csak annyira vagyunk erősek, mint a leggyengébbek. Ezért van szükség arra, hogy az ökoszisztémánkban mindenki cselekedjen, és megfelelő biztonsági védelmi intézkedésekre legyen szükség.

## <a name="mandatory-security-requirements"></a>Kötelező biztonsági követelmények

Azok a partnerek, akik nem valósítják meg a kötelező biztonsági követelményeket, nem hajtanak végre tranzakciót a Felhőszolgáltató programban, és nem kezelhetik az ügyfélbérlőket delegált rendszergazdai jogosultságokkal. Emellett azok a partnerek, akik nem valósítják meg a biztonsági követelményeket, veszélynek lehetnek kitéve a programokban való részvételüknek. A partnerbiztonsági követelményekhez társított feltételek hozzá vannak adva a Microsoft Partnerszerződés. A tanácsadókhoz kapcsolódóan ugyanezek a szerződéses követelmények lesznek érvényesek.

Az Ön és ügyfelei védelme érdekében a partnereknek azonnal el kell látnia a következő műveleteket:  

1. **Engedélyezze a többtényezős hitelesítést (MFA)** a partnerbérlő összes felhasználói fiókja esetében. Az MFA-t a partnerbérlő(k) összes felhasználói fiókján kényszerítnie kell. Az MFA-nak meg kell vitatni a felhasználókat, amikor bejelentkeznek a Microsoft kereskedelmi felhőszolgáltatásba, vagy amikor api-kon keresztül Felhőszolgáltató tranzakciót Partnerközpont keresztül.

2. **A biztonságos alkalmazásmodell keretrendszerének elfogadása.** Az api-Partnerközpont integrált partnereknek be kell fogadniuk a biztonságos alkalmazásmodell [keretrendszert](/partner-center/develop/enable-secure-app-model) minden alkalmazáshoz és felhasználói hitelesítési modellhez.

    > [!IMPORTANT]
    > Határozottan javasoljuk, hogy a partnerek implementálják az biztonságos alkalmazásmodell-t a Microsoft API-val ( például Azure Resource Manager vagy Microsoft Graph) való integrációhoz, vagy ha az automatizálást( például a PowerShellt) felhasználói hitelesítő adatok használatával használják, hogy elkerülhető legyen az MFA kényszerítésében kimaradás.

Ezek a biztonsági követelmények segítenek megvédeni az infrastruktúrát, és megvédeni az ügyfelek adatait a potenciális biztonsági kockázatoktól, például a lopások vagy más csalási incidensek azonosításától.  

## <a name="implementing-multi-factor-authentication"></a>Többtényezős hitelesítés megvalósítása

A partner biztonsági követelményeinek való megfeleléshez implementálja és kényszerítenie kell az MFA-t a partnerbérlő minden felhasználói fiókjához. Ezt a következő módokon lehet megtenni:

- Implementálja [Azure Active Directory (Azure AD) alapértelmezett biztonsági beállítását.](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) További információt a következő [szakaszban láthat.](#security-defaults)

- Vásároljon prémium szintű Azure Active Directory felhasználói fiókokhoz. További információ: [Az Azure AD Multi-Factor Authentication üzembe helyezésének megterve.](/azure/active-directory/authentication/howto-mfa-getstarted)

- Egy külső megoldással kényszerítsen MFA-t a partnerbérlőben minden felhasználói fiókra. Annak érdekében, hogy a megoldás biztosítani tudja a várt megoldást, tekintse meg a biztonsági követelmények [kényszerítését.](#how-the-requirements-are-enforced)

> [!NOTE]
> Bár a többtényezős hitelesítés nem kötelező a szuverén felhőkhöz (az EGYESÜLT Államok kormányához és Németországhoz), erősen ajánlott ezeket a biztonsági követelményeket befogadni.

### <a name="security-defaults"></a>Alapértelmezett biztonsági szabályok

Az MFA-követelmények megvalósításához a partnerek választhatják az egyik lehetőséget, hogy engedélyezik az alapértelmezett biztonsági beállításokat az Azure AD-ban. A biztonsági alapértelmezések alapszintű biztonságot nyújtanak többletköltség nélkül. Az alapértelmezett biztonsági beállítások engedélyezése előtt tekintse át, hogyan engedélyezheti az MFA-t a szervezet számára az Azure AD-val, valamint az alábbi főbb szempontokat.

- Az alapkonfiguráció-szabályzatokat befogadó partnereknek meg kell lépéseket kell elfogadnia a biztonsági alapértékre való áttérés érdekében.

- A biztonsági alapértelmezések az előzetes verzió alapkonfiguráció-szabályzatának általánosan elérhető helyettesítői. Ha egy partner engedélyezi az alapértelmezett biztonsági beállításokat, nem fogja tudni engedélyezni az alapkonfiguráció-szabályzatokat.

- A biztonsági alapértelmezések esetén az összes szabályzat egyszerre lesz engedélyezve.

- A feltételes hozzáférést [használó partnerek esetén](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)a [biztonsági alapértelmezések nem lesznek elérhetők.](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults)

- Jelenleg nem tiltjuk le az örökölt hitelesítést. Mivel azonban a sérült identitásokkal kapcsolatos legtöbb esemény az örökölt hitelesítést használó bejelentkezési kísérletből ad vissza, a partnereknek ajánlott elmozdulni ezekről a régebbi protokollokról.

- Azure AD Connect szinkronizálási fiók ki van zárva az alapértelmezett biztonsági beállításokból.

Részletes információ: [Overview of Azure AD Multi-Factor Authentication for your organization (Az Azure AD Multi-Factor Authentication](/azure/active-directory/authentication/concept-mfa-get-started) áttekintése a szervezet számára) és [What are security defaults?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)(Mik az alapértelmezett biztonsági beállítások?).

> [!NOTE]
> Az Azure AD biztonsági alapértelmezései az alapkonfiguráció védelmi szabályzatok egyszerűsített fejlődését szolgálják. Ha már engedélyezte az alapkonfiguráció védelmi szabályzatokat, erősen ajánlott engedélyezni az alapértelmezett [biztonsági beállításokat.](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)

## <a name="implementation-considerations"></a>Implementálási szempontok

Mivel ezek a követelmények a partnerbérlőben az összes felhasználói fiókra vonatkoznak, a zökkenőmentes üzembe helyezés érdekében több dolgot is figyelembe kell vennie. Azonosítsa például azokat az Azure AD-beli felhasználói fiókokat, amelyek nem tudnak MFA-műveleteket végezni, valamint a szervezetben azokat az alkalmazásokat és eszközöket, amelyek nem támogatják a modern hitelesítést.

Mielőtt bármilyen műveletet végrehajtana, javasoljuk, hogy végezze el az alábbi ellenőrzést. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Rendelkezik olyan alkalmazással vagy eszközzel, amely nem támogatja a modern hitelesítés használatát?

Az MFA kényszerítéskor az örökölt hitelesítés olyan protokollokat használ, mint az IMAP, a POP3, az SMTP és mások, mert azok nem támogatják az MFA-t. Ennek a korlátozásnak a kezelése érdekében használja az [alkalmazásjelszavak](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) funkciót annak biztosítására, hogy az alkalmazás vagy az eszköz továbbra is hitelesítve legyen. Tekintse át [az alkalmazásjelszavak használatának szempontjait,](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) és állapítsa meg, hogy használhatók-e a környezetben.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Rendelkezik olyan Office 365-felhasználókkal, akik a partnerbérlőhöz társított licencekkel rendelkezik?

A megoldások megvalósítása előtt javasoljuk, hogy határozza meg, hogy a partnerbérlő Microsoft Office mely verzióit használják a felhasználók. A felhasználók tapasztalni fogják az Outlookhoz hasonló alkalmazások csatlakozási problémáit. Az MFA kényszerítés előtt fontos, hogy az Outlook 2013 SP1 vagy újabb verziójával használja, és hogy a szervezetben engedélyezve legyen a modern hitelesítés. További információ: [Modern hitelesítés engedélyezése az Exchange Online-ban.](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) 

A 2013-as Microsoft Office windowsos eszközök modern hitelesítésének engedélyezéséhez két beállításkulcsot kell létrehoznia. Lásd: [Enable Modern Authentication for Office 2013 on Windows devices (Modern hitelesítés engedélyezése Az Office 2013-ban Windows-eszközökön).](/office365/admin/security-and-compliance/enable-modern-authentication)

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Van olyan szabályzat, amely megakadályozza, hogy a felhasználók a mobileszközeiket használják munka közben?

Fontos azonosítani azokat a vállalati szabályzatokat, amelyek megakadályozzák, hogy az alkalmazottak mobileszközt használjanak munka közben, mert ez befolyásolja a megvalósított MFA-megoldást. Vannak olyan megoldások, mint például az [Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)alapértelmezett biztonsági alapértelmezésének implementációja, amelyek csak hitelesítő alkalmazás használatát teszik lehetővé az ellenőrzéshez. Ha a szervezete olyan szabályzatot használ, amely megakadályozza a mobileszközök használatát, fontolja meg az alábbi lehetőségek egyikét:

- Biztonságos rendszeren futtatható, időalapú, egyszeres alapjelszó-alkalmazást (TOTP) helyezhet üzembe.

- Implementáljon egy külső megoldást, amely kikényszeríteni az MFA-t a partnerbérlőben minden olyan felhasználói fiókhoz, amely a legmegfelelőbb ellenőrzési lehetőséget biztosítja.

- Vásároljon [prémium szintű Azure Active Directory](https://azure.microsoft.com/pricing/details/active-directory/) licenceket az érintett felhasználók számára.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Milyen automatizálást vagy integrációt kell használnia a felhasználói hitelesítő adatok hitelesítéséhez?

Mivel az MFA-t minden felhasználóra, így a szolgáltatásfiókra is kényszerítjük a partnerkönyvtárban, ez hatással lesz minden olyan automatizálásra vagy integrációra, amely felhasználói hitelesítő adatokat használ a hitelesítéshez. Ezért fontos azonosítani az ilyen helyzetekben használt fiókokat. Tekintse meg a mintaalkalmazások vagy -szolgáltatások alábbi listáját, és vegye figyelembe a következőket:

- Az erőforrásoknak az ügyfelek nevében történő építésére használt vezérlőpult

- Integráció a számlázáshoz használt platformokkal (mivel az a CSP-programhoz kapcsolódik) és az ügyfelek támogatása

- Az Az, az AzureRM, az Azure AD, az MS Online és más modulokat felhasználó PowerShell-szkriptek

A fenti lista nem átfogó. Ezért fontos, hogy a környezetében minden olyan alkalmazást vagy szolgáltatást teljes körűen kiértékelésnek végezzen, amely felhasználói hitelesítő adatokat használ a hitelesítéshez. Az MFA követelményeivel való versengeni kívánás érdekében az útmutatót a biztonságos alkalmazásmodell [keretrendszerben kell](/partner-center/develop/enable-secure-app-model) megvalósítani, ahol lehetséges.

## <a name="accessing-your-environment"></a>A környezet elérése

Javasoljuk, hogy tekintse át a bejelentkezési tevékenységet, hogy jobban megértse, mit vagy ki hitelesít az MFA-hoz való kérdés nélkül. A prémium szintű Azure Active Directory használhatja a bejelentkezési jelentést. További információ erről a témáról: Bejelentkezési tevékenységre vonatkozó jelentések a [Azure Active Directory portálon.](/azure/active-directory/reports-monitoring/concept-sign-ins) Ha nem prémium szintű Azure Active Directory, vagy a bejelentkezési tevékenység PowerShellen keresztüli beszerzését keresi, akkor a Partnerközpont [PowerShell-modul](https://www.powershellgallery.com/packages/PartnerCenter/) [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) parancsmagját kell használnia.

## <a name="how-the-requirements-are-enforced"></a>A követelmények betartatásának a végrehajtása

A partnerbiztonsági követelményeket az Azure AD kényszeríti ki, Partnerközpont az MFA-igény ellenőrzésével ellenőrzi, hogy az MFA-ellenőrzés történt-e. 2019. november 18-tól a Microsoft további biztonsági védelmi funkciókat (korábbi nevén "technikai kényszerítési") aktivált a partnerbérlők számára.

Aktiváláskor a partnerbérlő felhasználóinak el kell végezniük az MFA-ellenőrzést, amikor bármilyen rendszergazdai (AOBO) műveletet hajt végre az Partnerközpont portálon, vagy ha Partnerközpont API-kat hívnak meg. További információkért lásd: Többtényezős hitelesítés [(MFA) használata a partnerbérlőben.](partner-security-requirements-mandating-mfa.md) 

Azok a partnerek, akik nem teljesék a követelményeket, a lehető leghamarabb végre kell hajtaniuk ezeket a intézkedéseket az üzletkimaradások elkerülése érdekében. Ha többtényezős hitelesítést Azure Active Directory Az Azure AD biztonsági alapértelmezései szerint használja, nincs szükség további műveletekre.

Ha külső MFA-megoldást használ, előfordulhat, hogy az MFA-igény nem lesz kibocsátva. Ha ez a jogcím hiányzik, az Azure AD nem fogja tudni megállapítani, hogy a hitelesítési kérést az MFA igényelte-e. További információ arról, hogyan ellenőrizheti, hogy a megoldás a várt jogcímet állítja-e [ki: Testing the Partner Security Requirements (A partnerbiztonsági követelmények tesztelése).](/powershell/partnercenter/test-partner-security-requirements) 

> [!IMPORTANT]
> Ha a harmadik féltől származó megoldás nem állítja ki a várt jogcímet, akkor a megoldás gyártójával kell együtt eldöntenie, milyen műveleteket kell tenni.

## <a name="resources-and-samples"></a>Források és minták

Támogatásért és mintakódért tekintse meg az alábbi forrásforrásokat:

- [Partnerközpont Biztonsági](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)útmutatási csoport közössége: Az Partnerközpont Security Guidance Group közössége egy online közösség, ahol megismerheti a közelgő eseményeket, és fel is teheti a kérdéseit.
- [Partnerközpont .NET-minták:](https://github.com/microsoft/partner-center-dotnet-samples)Ez a GitHub-adattár .NET használatával fejlesztett mintákat tartalmaz, amelyek bemutatják, hogyan implementálható a biztonságos alkalmazásmodell keretrendszer.
- [Partnerközpont](https://github.com/microsoft/partner-center-java-samples)Java-minták: Ez a GitHub-adattár Java használatával fejlesztett mintákat tartalmaz, amelyek bemutatják, hogyan implementálható a biztonságos alkalmazásmodell keretrendszer.
- [Partnerközpont PowerShell – Többtényezős](/powershell/partnercenter/multi-factor-auth)hitelesítés: Ez a többtényezős hitelesítést tartalmazó cikk részletesen bemutatja, hogyan valósíthatja meg a biztonságos alkalmazásmodell keretrendszert a PowerShell használatával.

## <a name="next-steps"></a>Következő lépések

- [Többtényezős hitelesítés (MFA) engedélyezése a partnerbérlő számára](partner-security-requirements-mandating-mfa.md)