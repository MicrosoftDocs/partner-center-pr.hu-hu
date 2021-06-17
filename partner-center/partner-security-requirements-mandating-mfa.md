---
title: Többtényezős hitelesítés (MFA) engedélyezése a partnerbérlő számára
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan segít az MFA-hitelesítés a partnerbérlők számára az ügyfélerőforrásokhoz való hozzáférés biztonságossá szolgáltatásában. Mintaforgatókönyveket tartalmaz.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fe1d894ec933072a64f2abdfbb795b6ef046168
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276008"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Többtényezős hitelesítés (MFA) engedélyezése a partnerbérlő számára

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Értékesítési ügynök | Az | Számlázási rendszergazdai | Globális rendszergazda

Ez a cikk részletes példákat és útmutatást tartalmaz a többtényezős hitelesítés (MFA) az Partnerközpont. A funkció célja, hogy segítsen a partnereknek biztosítani az ügyfelek erőforrásaihoz való hozzáférésüket a hitelesítő adatokkal szemben. A partnereknek kötelezően ki kell kényszeríteeik az MFA-t a partnerbérlőben az összes felhasználói fiókra, beleértve a vendégfelhasználókat is. A felhasználók számára a következő területeken kell végrehajtaniuk az MFA-ellenőrzést:

- [Partnerközpont irányítópult](#partner-center-dashboard)
- [Partnerközpont API](#partner-center-api)
- [Partner delegált felügyelete](#partner-delegated-administration)

A nagyobb és folyamatos biztonság és adatvédelem védelme az egyik legfontosabb prioritás, és továbbra is segítünk a partnereknek az ügyfeleik és bérlőik védelmében. A Felhőszolgáltató (CSP) programban részt vevő összes partnernek, a Vezérlőpult-szállítóknak (CPV-knek) és a tanácsadóknak implementálja a partnerbiztonsági követelményeket a megfelelőség érdekében. [](partner-security-requirements.md)

Annak érdekében, hogy a partnerek megvédjék vállalatukat és ügyfeleiket az identitáslopástól és a jogosulatlan hozzáféréstől, további biztonsági védelmi funkciókat aktiváltunk a partnerbérlők számára, amelyek kötelezően megszabadulnak és ellenőrzik az MFA-t. 

## <a name="partner-center-dashboard"></a>Partnerközpont irányítópult

Az irányítópult egyes Partnerközpont MFA-védelem alatt áll, beleértve a következőket:

- Az Ügyfelek lap **összes** oldala, például az összes olyan oldal, amely a következő URL-címen keresztül érhető el: https://partner.microsoft.com/commerce/*
- A Támogatási kérések > **lapon** található összes oldal, például az https://partner.microsoft.com/dashboard/support/csp/customers/*
- Számlázási oldal

Az alábbi táblázatban látható, hogy mely felhasználótípusok férhetnek hozzá ezekhez az MFA által védett lapokhoz (és melyekre éppen ezért hatással van ez a funkció).


| MFA által védett oldal       | Rendszergazdai ügynökök      |  Értékesítési ügynökök     |   Helpdesk-ügynökök     | Globális rendszergazda      |  Számlázási adminisztrátor     | 
|---    |---    |---    |---    |---    |---    |
| Minden oldal az Ügyfelek lapon      |   x    |    x   |  x     |       |       |
| Az Ügyfélszolgálati kérések > lap összes oldala     | x      |       |    x   |       |       |
| Számlázási oldal     |   x    |       |       |    x   |   x    |

Ha ezen oldalak bármelyikét próbálja elérni, és még nem végzett MFA-ellenőrzést korábban, akkor ezt önnek kell megtennie. A lap más Partnerközpont, például az Áttekintés vagy az Állapot Service Health nem igénylik az MFA-t.

## <a name="verification-examples"></a>Ellenőrzési példák

Az alábbi példákból szemléltetheti, hogyan működik Partnerközpont ellenőrzés az irányítópulton.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>1. példa: A partner már megvalósította Azure AD MFA

1. Jane a Contoso CSP-nek dolgozik. A Contoso a Contoso partnerbérlőben található összes felhasználója számára megvalósította az MFA-t Azure Active Directory (Azure AD) MFA használatával.

2. Jane elindít egy új böngésző-munkamenetet, és Partnerközpont irányítópult áttekintő oldalára (amely nem MFA-védelem alatt van). Partnerközpont átirányítja Jane-t az Azure AD-be a bejelentkezéshez.

3. A Contoso meglévő Azure AD MFA miatt Jane-nek el kell látnia az MFA-ellenőrzést. Sikeres bejelentkezés és MFA-ellenőrzés esetén Jane vissza lesz irányítva Partnerközpont irányítópult áttekintő oldalára.

4. Jane megpróbál hozzáférni az MFA által védett oldalakhoz a Partnerközpont. Mivel Jane már befejezte az MFA-ellenőrzést a korábbi bejelentkezés során, anélkül is hozzáférhet az MFA által védett oldalhoz, hogy újra el kellene mennie az MFA-ellenőrzésen.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>2. példa: A partner külső MFA-t valósított meg identitás-összevonás használatával

1. A Trent a CSP Wingtipnek dolgozik. A Wingtip minden felhasználója számára megvalósítottA MFA-t a Wingtip partnerbérlőben külső MFA használatával, amely identitás-összevonáson keresztül van integrálva az Azure AD-be.

2. A Trent elindít egy új böngésző-munkamenetet, és Partnerközpont irányítópult áttekintő oldalára (amely nem MFA-védelem alatt van). Partnerközpont átirányítja a Trentet az Azure AD-be a bejelentkezéshez.

3. Mivel a Wingtip identitás-összevonást is beállít, az Azure AD átirányítja a Trentet az összevont identitásszolgáltatóhoz a bejelentkezés és az MFA-ellenőrzés ellenőrzésére. Sikeres bejelentkezés és MFA-ellenőrzés esetén a Trent vissza lesz irányítva az Azure AD-be, majd Partnerközpont irányítópult áttekintő oldalára.

4. A Trent megpróbálja elérni az MFA által védett oldalak valamelyikét a Partnerközpont. Mivel a Trent már befejezte az MFA-ellenőrzést a korábbi bejelentkezés során, a Trent anélkül is hozzáférhet az MFA által védett oldalhoz, hogy újra el kellene mennie az MFA-ellenőrzésen.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>3. példa: A partner nem valósított meg MFA-t

1. John a Fabrikam CSP-nek dolgozik. A Fabrikam egyetlen felhasználó számára sem valósított meg MFA-t a Fabrikam-partnerbérlőben.

2. John elindít egy új böngésző-munkamenetet, és Partnerközpont irányítópult áttekintő oldalára (amely nem MFA-védelem alatt van). Partnerközpont átirányítja Johnt az Azure AD-be a bejelentkezéshez.

3. Mivel a Fabrikam nem valósított meg MFA-t, Johnnak nem kell végrehajtania az MFA-ellenőrzést. A sikeres bejelentkezés után John vissza lesz irányítva Partnerközpont irányítópult áttekintő oldalára.

4. John megpróbálja elérni az MFA által védett oldalak valamelyikét a Partnerközpont. Mivel John még nem végzett MFA-ellenőrzést, a Partnerközpont átirányítja Johnt az Azure AD-be az MFA-ellenőrzés befejezéséhez. Mivel ez az első alkalom, amikor Johnnak kötelező végrehajtania az MFA-t, johnnak is regisztrálnia kell [az MFA-hoz.](#mfa-registration-experience) A sikeres MFA-regisztráció és MFA-ellenőrzés után John hozzáférhet az MFA által védett oldalhoz.

5. Egy másik nap, mielőtt a Fabrikam MFA-t hozna létre bármely felhasználó számára, John elindít egy új böngésző-munkamenetet, és az Partnerközpont irányítópult áttekintő oldalára navigál (amely nem MFA-védelem alatt van). Partnerközpont átirányítja Johnt az Azure AD-be, hogy MFA-kérés nélkül jelentkezzen be. 

6. John megpróbálja elérni az MFA által védett oldalak valamelyikét a Partnerközpont. Mivel John még nem végzett MFA-ellenőrzést, a Partnerközpont átirányítja Johnt az Azure AD-be az MFA-ellenőrzés befejezéséhez. Mivel John regisztrálta az MFA-t, most csak az MFA-ellenőrzés befejezésére kérik fel.

> [!NOTE]
>Művelet: A vállalati rendszergazdák három [lehetőség közül választhatnak az](partner-security-requirements.md#implementing-multi-factor-authentication) MFA megvalósítására.

## <a name="partner-center-api"></a>Partnerközpont API

A Partnerközpont API a csak alkalmazás-hitelesítést és az App+User hitelesítést is támogatja. 

Az App+User hitelesítés használata esetén a Partnerközpont MFA-ellenőrzést fog igényelni. Pontosabban, ha egy partneralkalmazás API-kérést szeretne küldeni a Partnerközpont-nek, tartalmaznia kell egy hozzáférési jogkivonatot a kérés Engedélyezési fejlécében. 

> [!NOTE]
>Az [biztonságos alkalmazásmodell keretrendszer](/partner-center/develop/enable-secure-app-model) egy méretezhető keretrendszer a CSP-partnerek és CPV-k hitelesítésére az Microsoft Azure MFA architektúrán keresztül az Partnerközpont API-k hívhatóságakor. Ezt a keretrendszert implementálja, mielőtt engedélyezi az MFA-t a bérlőn. 

Amikor Partnerközpont api-kérést kap egy App+User hitelesítéssel kapott hozzáférési jogkivonattal, az Partnerközpont API ellenőrzi, hogy az *MFA* értéke jelen van-e a hitelesítési módszerre vonatkozó referencia *(AMR) jogcímben.* JWT-dekóder használatával ellenőrizheti, hogy egy hozzáférési jogkivonat tartalmazza-e a várt hitelesítési módszerre (AMR) vonatkozó értéket:

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Ha az érték jelen van, a Partnerközpont, hogy az MFA-ellenőrzés befejeződött, és feldolgozza az API-kérést. Ha az érték nincs jelen, a Partnerközpont API a következő válaszban elutasítja a kérést:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Ha App-Only hitelesítést használ, az App-Only hitelesítést támogató API-k MFA nélkül is folyamatosan működnek.

## <a name="partner-delegated-administration"></a>Partner delegált felügyelete

A partnerfiókok, beleértve a rendszergazdai ügynököket és a támogatási ügynököket, a partner delegált rendszergazdai jogosultságai segítségével kezelhetik az ügyfélerőforrásokat a Microsoft Online Services portálján, a parancssori felületen (CLI) és API-kon keresztül (alkalmazás-felhasználó hitelesítéssel).

### <a name="using-service-portals"></a>Szolgáltatásportálok használata

Amikor a Microsoft Online Services portálokat a Partner delegált rendszergazdai jogosultságai (rendszergazda– meghatalmazás) használatával fér hozzá az ügyfélerőforrások kezeléséhez, ezen portálok nagy része megköveteli a partnerfiók interaktív hitelesítését, az ügyfél Azure AD-bérlője pedig hitelesítési környezetként van beállítva – a partnerfióknak be kell jelentkeznie az ügyfélbérlőbe.

Amikor az Azure AD ilyen hitelesítési kéréseket kap, a partnerfióknak el kell fogadnia az MFA-ellenőrzést. Két felhasználói élmény lehetséges attól függően, hogy a partnerfiók felügyelt vagy összevont identitás:

- Ha **a** partnerfiók felügyelt identitás, az Azure AD közvetlenül kérni fogja a felhasználót az MFA-ellenőrzés befejezésére. Ha a partnerfiók korábban még nem regisztrált az MFA-ba az Azure AD-ban, a rendszer először az [MFA-regisztráció befejezését kéri](#mfa-registration-experience) a felhasználótól.

- Ha **a** partnerfiók összevont identitás, a felhasználói élmény attól függ, hogy a partner-rendszergazda hogyan konfigurálta az összevonást az Azure AD-ban. Az Azure AD-beli összevonás beállításakor a partner-rendszergazda jelezheti az Azure AD-nek, hogy az összevont identitásszolgáltató támogatja-e az MFA-t. Ha igen, az Azure AD átirányítja a felhasználót az összevont identitásszolgáltatóhoz az MFA-ellenőrzés ellenőrzésére. Ellenkező esetben az Azure AD közvetlenül kérni fogja a felhasználót az MFA-ellenőrzés befejezésére. Ha a partnerfiók korábban még nem regisztrált az MFA-ba az Azure AD-ban, a rendszer először az [MFA-regisztráció befejezését kéri](#mfa-registration-experience) a felhasználótól.

Az általános élmény hasonló ahhoz a forgatókönyvhöz, amelyben egy végfelhasználói bérlő több hitelesítést valósított meg a rendszergazdák számára. Az ügyfélbérlő például engedélyezte az [Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)alapértelmezett biztonsági beállításokat, ami megköveteli az összes rendszergazdai jogosultsággal rendelkező fióktól, hogy MFA-ellenőrzéssel jelentkezzen be az ügyfélbérlőbe, beleértve a rendszergazdai ügynököket és az ügyfélszolgálati ügynököket is. Tesztelési célból a partnerek engedélyezhetik az [Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) alapértelmezett biztonsági beállításokat az ügyfélbérlőben, majd megpróbálnak partner delegált felügyeleti jogosultságokkal hozzáférni az ügyfélbérlőhöz.

> [!NOTE]
> Nem minden Microsoft Online Service Portalon van szükség partnerfiókra az ügyfélbérlőbe való bejelentkezéshez, amikor partner delegált rendszergazdai jogosultságokkal fér hozzá az ügyfélerőforrásokhoz. Ehelyett csak a partnerfiókokat kell bejelentkezniük a partnerbérlőbe. Ilyen például az Exchange felügyeleti központ. Idővel arra számítunk, hogy ezek a portálok megkövetelik, hogy a partnerfiókok jelentkezzenek be az ügyfélbérlőbe a partner delegált rendszergazdai jogosultságai használata esetén.

### <a name="using-service-apis"></a>Szolgáltatási API-k használata

Egyes Microsoft Online Services API-k (például Azure Resource Manager, Azure AD Graph, Microsoft Graph stb.) támogatják a partner delegált rendszergazdai jogosultságokat használó partnereket az ügyfelek erőforrásainak programozott kezeléséhez. Ha partner delegált rendszergazdai jogosultságokat használ ezekkel az API-okkal, a partneralkalmazásnak tartalmaznia kell egy hozzáférési jogkivonatot az API-kérelem engedélyezési fejlécében, ahol a hozzáférési jogkivonatot úgy kérheti le, hogy egy partneri felhasználói fiókkal hitelesíti az Azure AD-t, és az ügyfél Azure AD-t használ hitelesítési környezetként. A partneralkalmazásnak be kell jelentkeznie egy partner felhasználói fiókkal az ügyfélbérlőbe.

Amikor az Azure AD megkapja a hitelesítési kérést, az Azure AD megköveteli a partner felhasználói fiókjától az MFA-ellenőrzés befejezését. Ha a partner felhasználói fiókja még nem regisztrált az MFA-hoz, a rendszer először az MFA-regisztráció befejezését kéri a felhasználói fióktól.

Ez a funkció minden olyan partneralkalmazásra hatással van, amely partner delegált rendszergazdai jogosultságokkal van integrálva ezekkel az API-okkal. Annak biztosítása érdekében, hogy a partneralkalmazások megszakítás nélkül továbbra is együtt tudjanak működni ezekkel az API-okkal:

- A partnernek kerülnie kell a nem interaktív felhasználói hitelesítési módszer használatát az Azure AD-val a hozzáférési jogkivonat beszerzéséhez. Nem interaktív felhasználói hitelesítési módszer, [](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)például jelszófolyam használata esetén az Azure AD nem fogja tudni kérni a felhasználót az MFA-ellenőrzés befejezésére. A partnernek interaktív felhasználóhitelesítési módszerre kell váltania, például OpenID Connect [folyamat használatával.](/azure/active-directory/develop/v1-protocols-openid-connect-code)

- Az interaktív felhasználóhitelesítési módszer során a partnernek olyan partneri felhasználói fiókot kell használnia, amely már engedélyezve van az MFA-hitelesítéshez. Ha az Azure AD kéri, a partner használhatja az MFA-regisztrációt és az MFA-ellenőrzést a bejelentkezés során.

- Ez hasonló ahhoz a forgatókönyvhöz, amelyben egy végfelhasználói bérlő MFA-t valósított meg a rendszergazdák számára. Az ügyfélbérlő például engedélyezte az [Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)alapértelmezett biztonsági beállításokat, amely megköveteli az összes rendszergazdai jogosultsággal rendelkező felhasználói fióktól, hogy MFA-ellenőrzéssel jelentkezzen be az ügyfélbérlőbe, beleértve a rendszergazdai ügynököket és az ügyfélszolgálati ügynököket is. Tesztelési célból a partnerek engedélyezhetik az [Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) alapértelmezett biztonsági beállításokat az ügyfélbérlőben, majd megpróbálnak partner delegált felügyeleti jogosultságokkal programozott módon hozzáférni az ügyfélbérlőhöz.

### <a name="mfa-registration-experience"></a>MFA-regisztrációs élmény

Ha az MFA ellenőrzése során a partnerfiók még nem regisztrált az MFA-ba, az Azure AD először kérni fogja a felhasználót, hogy töltse ki az MFA-regisztrációt:

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA-regisztráció – 1. lépés.":::

A Tovább **gombra** kattintva a felhasználónak választania kell az ellenőrzési módszerek listájából.

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA-regisztráció – 2. lépés.":::

Sikeres regisztráció esetén a felhasználónak el kell látnia az MFA-ellenőrzést a felhasználó által kiválasztott ellenőrzés alapján.
 
## <a name="list-of-common-issues"></a>Gyakori problémák listája

Mielőtt műszaki kivételt kérelmez [az](#how-to-submit-a-request-for-technical-exception) MFA-követelmény alól, tekintse át a más partnerek által jelentett gyakori problémák listáját, és ellenőrizze, hogy a kérelem érvényes-e.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>1. probléma: A partnernek több időre van szüksége az MFA partnerügynökök számára való megvalósításához
A partner még nem indult el, vagy még folyamatban van az MFA megvalósítása az olyan partnerügynökeik számára, akiknek hozzáférésre van szükségük a Microsoft Online Services portálhoz a partner delegált felügyeleti jogosultságai használatával az ügyfélerőforrások kezeléséhez. A partnernek több időre van szüksége az MFA implementáció végrehajtásához. Ez a probléma a technikai kivétel oka?

**Válasz:** Nem. A partnernek a fennakadások elkerülése érdekében meg kell tervezni az MFA implementését a felhasználók számára.

> [!NOTE]
> Annak ellenére, hogy a partner nem valósított meg MFA-t a partnerügynökeikhez, a partnerügynökök továbbra is hozzáférhetnek a Microsoft Online Services portálhoz a partner delegált felügyeleti jogosultságai segítségével, feltéve, hogy az ügyfélbérlőbe való bejelentkezés során a rendszer kéri az MFA-regisztrációt és MFA-ellenőrzést. Az MFA-regisztráció elvégzése nem engedélyezi automatikusan a felhasználó számára az MFA-t.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>2. probléma: A partner nem valósított meg MFA-t olyan felhasználói fiókok esetében, amelyek nem delegált rendszergazdai jogosultságokat használnak
A partnereknek vannak olyan felhasználói a partnerbérlőikben, akiknek nincs szükségük Microsoft Online Services portálok elérésére az ügyfélerőforrások partner delegált felügyeleti jogosultságokkal való kezeléséhez. A partner ezen felhasználók MFA-nak való megvalósításán van folyamatban, és több időre van szüksége a folyamat befejezéséhez. Ez a probléma a technikai kivétel oka?

**Válasz:** Nem. Mivel ezek a felhasználói fiókok nem használják a partner delegált felügyeleti jogosultságait az ügyfélerőforrások kezeléséhez, nem kell bejelentkezniük az ügyfélbérlőbe. Ezekre nem lesz hatással az, hogy az Azure AD MFA-ellenőrzést igényel az ügyfélbérlőbe való bejelentkezés során.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>3. probléma: A partner nem valósított meg MFA-t a felhasználói szolgáltatásfiókok esetében
A partnernek van néhány felhasználói fiókja a partnerbérlőiben, amelyeket az eszközök szolgáltatásfiókokként használnak. Ezek alacsony jogosultsági szintű fiókok, amelyek nem igényelnek Partnerközpont microsoft online szolgáltatási portálokat az ügyfélerőforrások partner delegált felügyeleti jogosultságokkal való kezeléséhez. Ez a probléma a technikai kivétel oka?

**Válasz:** Nem. Mivel ezek a felhasználói fiókok nem használják a partner delegált felügyeleti jogosultságait az ügyfélerőforrások kezeléséhez, nem kell bejelentkezniük az ügyfélbérlőbe. Ezekre nem lesz hatással az, hogy az Azure AD MFA-ellenőrzést igényel az ügyfélbérlőbe való bejelentkezés során.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>4. probléma: A partner nem implementálja az MFA-t az MS Authenticator alkalmazással
A partnerek "tiszta asztalra" vonatkozó szabályzatot tartalmaznak, amely nem teszi lehetővé, hogy az alkalmazottak a saját mobileszközeiket a munkahelyükre hozzák. A személyes mobileszközeikhez való hozzáférés nélkül az alkalmazottak nem telepítik az MS Authenticator alkalmazást, amely az Azure AD biztonsági alapértelmezései által támogatott egyetlen MFA-ellenőrzés. Ez a probléma a technikai kivétel oka?

**Válasz:** Nem, ez nem a technikai kivétel érvényes oka. A partnernek érdemes megfontolni a következő alternatívákat, hogy az alkalmazottak továbbra is el tudjanak mélyedni az MFA-ellenőrzésen, amikor Partnerközpont:
- A partner emellett regisztrálhat prémium szintű Azure AD külső MFA-megoldásokra (az Azure AD-val kompatibilis), amelyek további ellenőrzési módszereket biztosítanak.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>5. probléma: A partner az örökölt hitelesítési protokollok használata miatt nem tudja megvalósítani az MFA-t
A partner rendelkezik néhány olyan partnerügynökkel, akik továbbra is régi hitelesítési protokollokat használnak, amelyek nem kompatibilisek az MFA-kompatibilisekkel. A felhasználók például továbbra is az Outlook 2010-et használják, amely örökölt hitelesítési protokollon alapul. Ha ezen partnerügynökök számára engedélyezi az MFA-t, azzal megzavarhatja az örökölt hitelesítési protokollok használatát.

**Válasz:** Nem, ez nem a technikai kivétel érvényes oka. Határozottan javasoljuk a partnereknek, hogy a potenciális biztonsági következmények miatt ne használják az örökölt hitelesítési protokollokat, mivel ezek a protokollok nem védhetőek MFA-ellenőrzéssel, és sokkal inkább ki vannak téve a hitelesítő adatok biztonságának. Ha az örökölt hitelesítési protokollok használata nélkül nem lehetséges, a partnereknek érdemes lehet feliratkozni a prémium szintű Azure AD-re, amely támogatja az alkalmazásjelszavak használatát. Az alkalmazásjelszavak a rendszer által létrehozott egyszer létrehozott jelszavak, és általában erősebbek, mint az emberek által létrehozott jelszavak. Az alkalmazásjelszavak használatával a partnerek MFA-t valósítanak meg a felhasználók számára, miközben az örökölt hitelesítési protokollok esetén az alkalmazásjelszavakra visszatérve.

Olvassa el az Alapszintű [hitelesítéssel](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) és az Exchange Online-sal kapcsolatos bejegyzést, amelyből a legújabb terv szerint támogatja az Outlook örökölt hitelesítését, és kövesse az Exchange csapat [blogját](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) a közelgő hírek lekértért cikkéhez. 

> [!NOTE]
> Annak ellenére, hogy a partner nem valósított meg MFA-t a partnerügynökeikhez, a partnerügynökök továbbra is hozzáférhetnek a Microsoft Online Services portálhoz a partner delegált felügyeleti jogosultságai segítségével, feltéve, hogy az ügyfélbérlőbe való bejelentkezés során a rendszer kéri az MFA-regisztrációt és MFA-ellenőrzést. Az MFA-regisztráció elvégzése nem engedélyezi automatikusan a felhasználó számára az MFA-t.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>6. probléma: A partner olyan külső MFA-t valósított meg, amelyet az Azure AD nem ismer fel
Egy partner MFA-t valósított meg a felhasználók számára egy külső MFA-megoldással. A partner azonban nem tudja megfelelően konfigurálni a külső MFA-megoldást ahhoz, hogy továbbítja az Azure AD-nek, hogy az MFA-ellenőrzés a felhasználó hitelesítése során befejeződött. Ez a technikai kivétel oka?

**Válasz:** Igen, ez a probléma a technikai kivétel érvényes oka lehet. Technikai kivételre vonatkozó kérelem elküldése előtt ellenőrizze a külső MFA-megoldás szolgáltatójánál, hogy az MFA-megoldás nem konfigurálható úgy, hogy a *hitelesítésimetódosreferences* jogcímet *(multipleauthn* értékkel) az Azure AD-be küldje, jelezve, hogy az MFA-ellenőrzés a felhasználó hitelesítése során befejeződött. Technikai kivételre vonatkozó kérelem elküldésekor meg kell adnia a használt külső MFA-megoldás részleteit, meg kell adnia az integráció módszerét (például identitás-összevonás vagy az Azure AD egyéni vezérlő használata révén), valamint meg kell adnia a következő információkat a technikai kivételkérésben támogató dokumentumként:

- A külső MFA-konfigurációk.

- A külső [](/powershell/partnercenter/test-partner-security-requirements) MFA-kompatibilis fiók által futtatott partnerbiztonsági követelmények tesztelésének eredménye.

- Az Ön által használt vagy használni tervező, harmadik féltől származó MFA-megoldás megrendelése.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Technikai kivételre vonatkozó kérés elküldése

A partnerek technikai kivételt alkalmazhatnak az MFA-ellenőrzés mellőzése érdekében, ha technikai problémákba ütköznek a Microsoft Online Servicesben, és nincs megvalósítható megoldás vagy áthidaló megoldás. Ezt megelőzően tekintse át [az előző](#list-of-common-issues) szakaszban gyakori problémák listáját.

Technikai kivételre vonatkozó kérelem elküldése:

1. Jelentkezzen be az Partnerközpont globális rendszergazdaként vagy rendszergazdai ügynökként.

2. Hozzon létre egy új partnerszolgáltatás-kérelmet a Támogatási partner támogatási kérései között, majd   >   válassza az Új **kérés gombra.**

3. Keressen rá az **MFA kifejezésre – Kivétel kérése a** keresőmezőben; vagy válassza **a CSP** lehetőséget a Kategóriából, majd válassza a **Fiókok, Beléptető,** Hozzáférés témakörből lehetőséget, majd válassza az **MFA –** Kivétel kérése lehetőséget az altopikus részből, majd válassza a következő **lépést.**

4. Adja meg a műszaki kivételre vonatkozó szolgáltatáskérés elküldését kért adatokat, majd válassza a **Submit (Küldés) lehetőséget.**

A Microsoft akár három munkanapot is átvehet, hogy választ adjon egy műszaki kivételre vonatkozó kérésre.

## <a name="next-steps"></a>Következő lépések

 - [Partnerbiztonsági követelmények állapota](partner-security-compliance.md)