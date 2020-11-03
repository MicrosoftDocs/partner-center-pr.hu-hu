---
title: MFA előírása a partner bérlője számára
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan biztosíthatja az ügyfelek erőforrásaihoz való hozzáférést a partneri bérlők számára az MFA meghatalmazása révén. Példákat tartalmaz.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a85a7e415eac7f54ccd52302e350ce20de9856d
ms.sourcegitcommit: 0cea15df24a6a1b310535eb1cb5e167dc2248a95
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/16/2020
ms.locfileid: "92530444"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>A többtényezős hitelesítés (MFA) meghatalmazása a partner bérlője számára

**A következőkre vonatkozik**

- A Cloud Solution Provider program összes partnere
  - Közvetlen számla
  - Közvetett szolgáltató
  - Közvetett viszonteladó
- Minden tanácsadó

**Érintett szerepkörök**

- Felügyeleti ügynök
- Értékesítési ügynök
- Segélyszolgálat ügynöke
- Számlázási adminisztrátor
- Globális rendszergazda

Ennek a funkciónak a célja, hogy segítse a partnereknek az ügyfelek erőforrásaihoz való hozzáférésüket a hitelesítő adatok biztonsága miatt.
A partnerek számára szükséges a többtényezős hitelesítés (MFA) betartatása a partner bérlőn lévő összes felhasználói fiókhoz, beleértve a vendég felhasználót is, ezzel a funkcióval a partneri szerepkörök a következő területekre vonatkozó MFA-ellenőrzés elvégzésére lesznek felhatalmazva:

- [A partneri központ irányítópultja](#partner-center-dashboard)
- [Partnerközpont API](#partner-center-api)
- [Partner által delegált felügyelet](#partner-delegated-administration)

A legfontosabb prioritások közé tartozik a nagyobb és folyamatos biztonsági és adatvédelmi védelem, és továbbra is segítjük a partnereknek az ügyfelek és a bérlők védelmét. A Cloud Solution Provider (CSP) programban résztvevő összes partner, a Vezérlőpult-szállítók (CPVs) és a tanácsadók a megfelelő állapotba kell léptetni a [partneri biztonsági követelményeket](partner-security-requirements.md) .

A Microsoft megkezdte a további biztonsági óvintézkedések aktiválását a partnerek bérlői számára. A biztonsági óvintézkedések aktiválása lehetővé teszi a partnerek számára, hogy a többtényezős hitelesítés (MFA) hitelesítésének megkövetelésével biztonságossá tehetik a bérlőket és ügyfeleiket a jogosulatlan hozzáférés megakadályozása érdekében.

Sikeresen elvégezte az aktiválást a partner által delegált felügyeleti képességekhez az összes partner bérlőhöz. Ha további segítségre van szükség a partnereknek és az ügyfeleknek a 2020. május 1-től való védelméhez, megkezdjük a partner Center-tranzakciók aktiválását a CSP-ben, így a partnerek megvédik a vállalatokat és az ügyfeleket az identitás-lopással kapcsolatos incidensekkel

Ez a dokumentáció a partnerek számára biztosít részletes tapasztalatokat és útmutatást a biztonsági óvintézkedések aktiválásával kapcsolatban.

## <a name="partner-center-dashboard"></a>A partneri központ irányítópultja

A partner Center irányítópultjának bizonyos oldalai MFA-védelemmel lesznek ellátva, beleértve a következőket:

- Az **ügyfelek** lap összes lapja, például az összes olyan oldal, amely a következő URL-címen érhető el: https://partner.microsoft.com/commerce/*
- A **támogatási > Customer requests** lapon lévő összes oldal, például az oldalon elérhető oldal https://partner.microsoft.com/dashboard/support/csp/customers/*
- Számlázási oldal

Ha megpróbál hozzáférni ezekhez a lapokhoz, és korábban még nem fejezte be az MFA-ellenőrzést, erre lesz szüksége.

> [!NOTE]
> A partner Center más oldalai, például az áttekintő lap, Service Health állapot-ellenőrzési lap nem lesz MFA-védelemmel ellátva.

A következő felhasználói típusok jogosultak az MFA-védelemmel ellátott lapok elérésére, ezért a funkció hatással van rájuk


| MFA által védett lapok       | Rendszergazdai ügynökök      |  Értékesítési ügynökök     |   Segélyszolgálat-ügynökök     | Globális rendszergazda      |  Számlázási adminisztrátor     | 
|---    |---    |---    |---    |---    |---    |
| Az ügyfelek lap összes lapja      |   x    |    x   |  x     |       |       |
| Az összes oldal a támogatási > az ügyfelek kérései lapon     | x      |       |    x   |       |       |
| Számlázási oldal     |   x    |       |       |    x   |   x    |

## <a name="examples-showing-how-verification-works"></a>Példák az ellenőrzés működésére

Az ellenőrzés működésének szemléltetéséhez vegye figyelembe az alábbi két példát.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>1. példa: a partner implementálta az Azure AD MFA-t

1. Jane a CSP contoso esetében működik. A contoso az Azure Active Directory (Azure AD) MFA használatával implementálta az MFA-t a contoso partner bérlője alá tartozó összes felhasználó számára.

2. Jane új böngésző-munkamenetet indít el, és navigál a partner Center irányítópult áttekintés lapjára (amely nem MFA-védelemmel ellátott). A partner Center átirányítja Jane-t az Azure AD-be a bejelentkezéshez.

3. A contoso meglévő Azure AD MFA-beállítása miatt Jane szükséges az MFA-ellenőrzés elvégzéséhez. A sikeres bejelentkezés és az MFA-ellenőrzés után Jane átirányítja a partneri központ irányítópultjának áttekintés lapjára.

4. Jane megpróbál hozzáférni a partner Center egyik MFA-védelemmel ellátott lapjához. Mivel Jane már végrehajtotta az MFA-ellenőrzést a korábbi bejelentkezések során, Jane elérheti az MFA által védett oldalt anélkül, hogy újra kellene mennie az MFA-ellenőrzésen.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>2. példa: a partner harmadik féltől származó MFA-t alkalmazott az identitás-összevonás használatával

1. A Trent a CSP Wingtip működik. A Wingtip a harmadik féltől származó MFA-t használó Wingtip-partneri bérlőn belül minden felhasználó számára implementálta a többtényezős hitelesítést, amely az Azure AD-vel integrált identitás-összevonással.

2. A Trent új böngésző-munkamenetet indít el, és megnyitja a partneri központ irányítópultjának áttekintés lapját (amely nem MFA-védelemmel ellátott). A partner Center átirányítja a Trentot az Azure AD-be a bejelentkezéshez.

3. Mivel a Wingtip rendelkezik a telepítő identitás-összevonásával, az Azure AD átirányítja a Trentot az összevont identitás-szolgáltatóhoz a bejelentkezés és az MFA-ellenőrzés befejezéséhez. A sikeres bejelentkezés és az MFA-ellenőrzés után a Trent át lesz irányítva az Azure AD-be, majd a partner központ irányítópultjának áttekintés lapjára.

4. A Trent megpróbál hozzáférni a partner Center egyik MFA-védelemmel ellátott lapjához. Mivel a Trent már végrehajtotta az MFA-ellenőrzést a korábbi bejelentkezések során, a Trent el tudja érni az MFA által védett oldalt anélkül, hogy újra kellene mennie az MFA-ellenőrzésen.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>3. példa: a partner nem implementálta az MFA-t

1. John együttműködik a CSP Fabrikam-vel. A fabrikam nem implementálta az MFA-t a fabrikam partner bérlője alatt álló bármely felhasználó számára.

2. John új böngésző-munkamenetet indít el, és a partner Center irányítópult áttekintés lapjára navigál (amely nem MFA-védelemmel ellátott). A partner Center átirányítja John-t az Azure AD-be a bejelentkezéshez.

3. Mivel a fabrikam nem implementálta az MFA-t, John nem szükséges az MFA-ellenőrzés elvégzéséhez. A sikeres bejelentkezés után John átirányítja a partneri központ irányítópultjának áttekintés lapjára.

4. John megpróbál hozzáférni a partner Center egyik MFA-védelemmel ellátott lapjához. Mivel John nem fejezte be az MFA-ellenőrzést, a partner Center átirányítja John-t az Azure AD-ba az MFA-ellenőrzés elvégzéséhez. Mivel az MFA betöltéséhez először János szükséges, John is [regisztrálni kell az MFA](#mfa-registration-experience)-hoz. A sikeres MFA-regisztráció és az MFA-ellenőrzés után John mostantól hozzáférhet az MFA által védett oldalhoz.

5. Egy másik nappal azelőtt, hogy minden felhasználónál a fabrikam implementálja az MFA-t, John elindítja az új böngésző-munkamenetet, és a partner Center irányítópult áttekintés lapjára navigál (amely nem MFA-védelemmel ellátott). A partner Center átirányítja John-t az Azure AD-be, hogy MFA-kérés nélkül jelentkezzen be. 

6. John megpróbál hozzáférni a partner Center egyik MFA-védelemmel ellátott lapjához. Mivel John nem fejezte be az MFA-ellenőrzést, a partner Center átirányítja John-t az Azure AD-ba az MFA-ellenőrzés elvégzéséhez. Mivel John regisztrálta az MFA-t, ezért csak az MFA-ellenőrzés befejezését kéri.

> [!NOTE]
>Művelet: a vállalati rendszergazdának most már a partner Center által javasolt [beállításokkal](partner-security-requirements.md#actions-that-you-need-to-take) kell implementálnia az MFA-t.

## <a name="partner-center-api"></a>Partnerközpont API

A partner Center API a csak az alkalmazáson belüli hitelesítést és az alkalmazás-és felhasználói hitelesítést is támogatja. 

Az alkalmazás és a felhasználó hitelesítésének használatakor a partneri központban az MFA-hitelesítésre lesz szükség. Pontosabban, amikor egy partner alkalmazás API-kérést szeretne küldeni a partneri központnak, a kérelem engedélyezési fejlécében szerepelnie kell egy hozzáférési jogkivonatnak. 

> [!NOTE]
>A [Secure Application Model](/partner-center/develop/enable-secure-app-model) egy biztonságos, méretezhető keretrendszer a CSP-partnerek hitelesítéséhez és a Microsoft Azure MFA-architektúrán keresztüli CPVs a partner Center API meghívásakor, mielőtt engedélyezi az MFA használatát a bérlőn. 

Ha a partneri központ az App + felhasználói hitelesítés használatával kapott hozzáférési jogkivonattal kap API-kérelmet, a partner Center API az *MFA* -érték jelenlétét fogja ellenőriznie a *hitelesítési módszer hivatkozása (AMR)* jogcímben. JWT-dekóder használatával ellenőrizheti, hogy egy hozzáférési jogkivonat tartalmazza-e a várt hitelesítési módszer hivatkozási (AMR) értékét, vagy sem:

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

Ha az érték megtalálható, a partner Center megállapítja, hogy az MFA-ellenőrzés befejeződött, és feldolgozza az API-kérést. Ha az érték nincs jelen, a partner Center API a következő választal utasítja el a kérelmet:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

App-Only hitelesítés használatakor a App-Only hitelesítést támogató API-k folyamatosan működnek, és nem igényelnek MFA-t.

## <a name="partner-delegated-administration"></a>Partner által delegált felügyelet

### <a name="using-service-portals"></a>Szolgáltatás-portálok használata

A partneri fiókok, beleértve a felügyeleti ügynököket és a segélyszolgálat-ügynököket, a partner meghatalmazott rendszergazdai jogosultságokkal kezelhetik az ügyfelek erőforrásait a Microsoft Online Services portálon, a parancssori felületen (CLI) és az API-kon keresztül (az App + felhasználói hitelesítés használatával).

Ha a Microsoft Online Services portálokat a partner által delegált rendszergazdai jogosultságokkal (rendszergazdai nevén) használja az ügyfelek erőforrásainak kezeléséhez, számos ilyen portálhoz szükség van a partner fiókra az interaktív hitelesítéshez, és az ügyfél-Azure Active Directory bérlő beállítása hitelesítési környezetként – a partneri fióknak be kell jelentkeznie az ügyfél-bérlőbe.

Amikor Azure Active Directory megkapja az ilyen hitelesítési kérelmeket, a partner fiókjának az MFA-ellenőrzés elvégzéséhez szüksége lesz. Két lehetséges felhasználói élmény van, attól függően, hogy a partner fiók felügyelt vagy összevont identitás-e:

- Ha a partner fiók **felügyelt** identitás, Azure Active Directory közvetlenül az MFA-ellenőrzés elvégzésére kéri a felhasználót. Ha a partner fiók még nincs regisztrálva az MFA-ban Azure Active Directory előtt, a rendszer kérni fogja a felhasználótól, hogy először az [MFA-regisztrációt végezze](#mfa-registration-experience) el.

- Ha a partner fiók **összevont** identitás, a felhasználói élmény attól függ, hogy a partner rendszergazdája hogyan konfigurálta az összevonást Azure Active Directoryban. Az Azure Active Directory-ben való összevonás beállításakor a partner rendszergazdája jelezheti, hogy Azure Active Directory, hogy az összevont identitás-szolgáltató támogatja-e az MFA-t. Ha igen, Azure Active Directory átirányítja a felhasználót az összevont identitás-szolgáltatóra az MFA-ellenőrzés elvégzéséhez. Ellenkező esetben a Azure Active Directory közvetlenül az MFA-ellenőrzés elvégzésére kéri a felhasználót. Ha a partner fiók még nincs regisztrálva az MFA-ban Azure Active Directory előtt, a rendszer kérni fogja a felhasználótól, hogy először az [MFA-regisztrációt végezze](#mfa-registration-experience) el.

Az általános élmény hasonló ahhoz a forgatókönyvhöz, amelyben egy végfelhasználói bérlő implementálta az MFA-t a rendszergazdái számára. Például az ügyfél bérlője engedélyezte az [Azure ad biztonsági alapértékeit](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), így minden rendszergazdai jogosultsággal rendelkező fióknak be kell jelentkeznie az ügyfél-bérlőbe az MFA-ellenőrzéssel, beleértve a felügyeleti ügynököket és a segélyszolgálat-ügynököket. Tesztelési célból a partnerek engedélyezhetik az [Azure ad biztonsági alapértelmezéseit](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) az ügyfél bérlőben, majd megpróbálják használni a partner által delegált rendszergazdai jogosultságokat az ügyfél bérlőhöz való hozzáféréshez.

> [!NOTE]
> Nem minden Microsoft Online Services-portálon kell partneri fiókokat bejelentkeznie az ügyfél bérlője számára, amikor a partner meghatalmazott rendszergazdai jogosultságokkal férnek hozzá az ügyfelek erőforrásaihoz. Ehelyett csak a partner bérlője számára kell bejelentkezniük. Ilyen például az Exchange felügyeleti központ. Az idő múlásával elvárjuk, hogy a portálon partneri fiókokat kelljen bejelentkezniük az ügyfél bérlője számára a meghatalmazott rendszergazdai jogosultságok használatakor.

### <a name="using-service-apis"></a>A Service API-k használata

Bizonyos Microsoft Online Services API-k (például Azure Resource Manager, Azure AD Graph, Microsoft Graph stb.) támogatják a partner meghatalmazott rendszergazdai jogosultságokat használó partnereket az ügyfelek erőforrásainak programozott kezeléséhez. Ezen API-kkal delegált rendszergazdai jogosultságok kihasználása érdekében a partner alkalmazásnak tartalmaznia kell egy hozzáférési jogkivonatot az API-kérelem engedélyezési fejlécében, ahol a hozzáférési jogkivonatot a partner felhasználói fiókkal kell megszereznie az Azure AD-vel való hitelesítéshez, és az ügyfél Azure AD-készletét hitelesítési környezetként kell beállítani. A partneri alkalmazásnak egy partner-felhasználói fiókkal kell bejelentkeznie az ügyfél bérlője számára.

Ha az Azure AD például hitelesítési kérést kap, az Azure AD-nek szüksége lesz a partner felhasználói fiókra az MFA-ellenőrzés elvégzéséhez. Ha a partner felhasználói fiók korábban nem regisztrált az MFA-ra, a rendszer először a felhasználói fiókot fogja kérni az MFA-regisztráció befejezéséhez.

A funkció hatással van minden olyan partneri alkalmazásra, amely ezen API-k használatával van integrálva a partner által delegált rendszergazdai jogosultságokkal. Annak biztosítása érdekében, hogy a partner alkalmazások továbbra is működjenek az API-k megszakítása nélkül:

- A partnernek kerülnie kell a nem interaktív felhasználói hitelesítési módszer használatát az Azure AD-vel a hozzáférési jogkivonat beszerzéséhez. Ha nem interaktív felhasználói hitelesítési módszert használ, például a [jelszó áramlását](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), az Azure ad nem fogja tudni bekérni a felhasználót az MFA-ellenőrzés elvégzésére. A partnernek az interaktív felhasználói hitelesítési módszer (például az [OpenID Connect flow](/azure/active-directory/develop/v1-protocols-openid-connect-code) ) használatára kell váltania.

- Az interaktív felhasználói hitelesítési módszer során a partnernek olyan partner felhasználói fiókot kell használnia, amely már engedélyezve van az MFA-hoz. Azt is megteheti, hogy ha az Azure AD-t kéri, a partner az MFA-regisztráció és az MFA-ellenőrzés befejeződik a bejelentkezés során.

- Ez hasonló ahhoz a forgatókönyvhöz, amelyben egy végfelhasználói bérlő implementálta az MFA-t a rendszergazdái számára. Például az ügyfél bérlője engedélyezte az [Azure ad biztonsági alapértékeit](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), így az összes rendszergazdai jogosultsággal rendelkező felhasználói fióknak az MFA-hitelesítéssel kell bejelentkeznie az ügyfél-bérlőbe, beleértve a felügyeleti ügynököket és az ügyfélszolgálati ügynököt. Tesztelési célból a partnerek engedélyezhetik az [Azure ad biztonsági alapértelmezéseit](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) az ügyfél-bérlőben, majd megpróbálják használni a partner által delegált rendszergazdai jogosultságokat az ügyfél-bérlő programozott eléréséhez.

### <a name="mfa-registration-experience"></a>MFA-regisztrációs élmény

Az MFA ellenőrzése során, ha a partner fiók még korábban nem regisztrált az MFA-ban, az Azure AD kéri a felhasználót, hogy először az MFA-regisztrációt végezze el:

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA-regisztráció 1. lépés":::

A **tovább** gombra kattintás után a rendszer megkéri a felhasználót, hogy válasszon az ellenőrzési módszerek listájáról.

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA-regisztráció 1. lépés":::

A sikeres regisztráció után a felhasználónak a felhasználó által választott ellenőrzés alapján be kell fejeznie az MFA-ellenőrzést.

## <a name="request-for-technical-exception"></a>Technikai kivételre vonatkozó kérelem

A partnerek technikai kivételt alkalmazhatnak az MFA-ellenőrzés letiltásához, ha technikai problémák léptek fel a Microsoft Online Services szolgáltatással, és nincs megvalósítható megoldás vagy megoldás. Mielőtt ezt megtenné, tekintse át a következő fejezeteket:

- [A partnerek által jelentett gyakori problémák listája](#list-of-common-issues-reported-by-partners)
- [Technikai kivételre vonatkozó kérelem beküldése](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>A partnerek által jelentett gyakori problémák listája
A technikai kivétel alkalmazása előtt tekintse át a többi partner által jelentett gyakori problémák listáját, és Ismerje meg, hogy érvényesek-e a technikai kivételek.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>1. probléma: a partnernek több időre van szüksége az MFA megvalósításához a partnerek ügynökei számára
Egy partner nem indult el, vagy még mindig folyamatban van az MFA bevezetésének folyamata a partnerek ügynökei számára, akiknek szükségük van a Microsoft Online Services portálokhoz való hozzáférésre a partner által delegált rendszergazdai jogosultságokkal az ügyfelek erőforrásainak kezelése A partnernek több időre van szüksége az MFA megvalósításának elvégzéséhez. A probléma a technikai kivétel érvényes oka?

**Válasz** : nem. A partnernek tervbe kell vennie az MFA megvalósítását a felhasználók számára a fennakadás elkerülése érdekében.

> [!NOTE]
> Annak ellenére, hogy a partner nem implementálta az MFA-t a partnerek ügynökei számára, a partner ügynökök továbbra is hozzáférhetnek a Microsoft Online Services-portálokhoz a partner által delegált rendszergazdai jogosultságok használatával, ha az ügyfél bérlője számára történő bejelentkezéskor a rendszer felszólítja az MFA regisztrálására Az MFA-regisztráció befejezése nem engedélyezi automatikusan a felhasználót az MFA-hoz.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>2. probléma: a partner nem implementálta az MFA-t a delegált rendszergazdai jogosultságokat nem használó felhasználói fiókok esetében
A partnerek olyan felhasználókkal rendelkeznek, akik nem igénylik a Microsoft Online Services portálok hozzáférését a partneri erőforrások kezeléséhez a partner által delegált rendszergazdai jogosultságok használatával. A partner az MFA bevezetésének folyamata a felhasználók számára, és több időre van szüksége a befejezéshez. A probléma a technikai kivétel érvényes oka?

**Válasz** : nem. Mivel ezek a felhasználói fiókok nem használnak partneri delegált rendszergazdai jogosultságokat az ügyfelek erőforrásainak kezeléséhez, nem kell bejelentkezniük az ügyfél bérlője számára. Az Azure AD nem fogja érinteni az MFA-ellenőrzést igénylő bejelentkezést az ügyfél bérlője számára.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>3. probléma: a partner nem implementálta az MFA-t a felhasználói szolgáltatásfiókok számára
Egy partnernek van néhány felhasználói fiókja a partner bérlőben, amelyet az eszközök a szolgáltatásfiókokként használnak. Ezek alacsony jogosultsági szintű fiókok, amelyek nem igénylik a hozzáférési partneri központ és a Microsoft Online Services portálok számára az ügyfelek erőforrásainak a meghatalmazott rendszergazdai jogosultságokkal történő kezelését. A probléma a technikai kivétel érvényes oka?

**Válasz** : nem. Mivel ezek a felhasználói fiókok nem használnak partneri delegált rendszergazdai jogosultságokat az ügyfelek erőforrásainak kezeléséhez, nem kell bejelentkezniük az ügyfél bérlője számára. Az Azure AD nem fogja érinteni az MFA-ellenőrzést igénylő bejelentkezést az ügyfél bérlője számára.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>4. probléma: a partner nem tudja megvalósítani az MFA-t az MS hitelesítő alkalmazás használatával
Egy partner "tiszta asztali" szabályzattal rendelkezik, amely nem teszi lehetővé, hogy az alkalmazottak a saját mobil eszközeiket a munkaterületre hozzanak. A személyes mobileszközök elérésének hiányában az alkalmazottak nem telepíthetik az MS hitelesítő alkalmazást, amely az Azure AD biztonsági Alapértelmezések által támogatott egyetlen MFA-ellenőrzés. A probléma a technikai kivétel érvényes oka?

**Válasz** : nem, ez a technikai kivétel nem érvényes oka. A partnernek a következő alternatívákat kell figyelembe vennie, hogy alkalmazottaik továbbra is elvégezzenek MFA-ellenőrzést a partneri központ elérésekor:
- A partner regisztrálhat prémium szintű Azure AD vagy harmadik féltől származó, az Azure AD-vel kompatibilis MFA-megoldásokra is, amelyek további ellenőrzési módszereket is biztosíthatnak.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>5. probléma: a partner nem tudja megvalósítani az MFA-t az örökölt hitelesítési protokollok használata miatt
A partner rendelkezik olyan partneri ügynökökkel, akik továbbra is örökölt hitelesítési protokollokat használnak, amelyek nem kompatibilisek az MFA-val. Például a felhasználók továbbra is az Outlook 2010-et használják, amely örökölt hitelesítési protokollokon alapul. Ha engedélyezi az MFA-t ezen partnerek ügynökei számára, az örökölt hitelesítési protokollok használatát megszakítja.

**Válasz** : nem, ez a technikai kivétel nem érvényes oka. A partnereknek határozottan javasoljuk, hogy az örökölt hitelesítési protokollok használatát a lehetséges biztonsági következmények miatt eltérjenek, mivel ezeket a protokollokat nem lehet az MFA-ellenőrzéssel védeni, és sokkal érzékenyebbek a hitelesítő adatok biztonságára. Ha az örökölt hitelesítési protokollok használatából való elmozdulás nem lehetséges, a partnereknek érdemes megfontolniuk a prémium szintű Azure AD regisztrálását, amely támogatja az alkalmazások jelszavainak használatát. Az alkalmazás jelszavai egyszeri, rendszer által generált jelszavak, és általában erősebbek, mint az emberi által generált jelszavak. Az alkalmazás jelszavainak használatával a partnerek az MFA-t implementálják a felhasználók számára, miközben az alkalmazás jelszavait csak az örökölt hitelesítési protokollok esetében érik el.

Olvassa el az [alapszintű hitelesítésről és az Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) -ról szóló bejegyzést, amelyből megismerheti az Outlookhoz való örökölt hitelesítés támogatásának legújabb tervét, és kövesse az [Exchange csapat blogját](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) a közelgő Hírek beszerzéséhez. 

> [!NOTE]
> Annak ellenére, hogy a partner nem implementálta az MFA-t a partnerek ügynökei számára, a partner ügynökök továbbra is hozzáférhetnek a Microsoft Online Services-portálokhoz a partner által delegált rendszergazdai jogosultságok használatával, ha az ügyfél bérlője számára történő bejelentkezéskor a rendszer felszólítja az MFA regisztrálására Az MFA-regisztráció befejezése nem engedélyezi automatikusan a felhasználót az MFA-hoz.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>6. probléma: a partner olyan harmadik féltől származó MFA-t implementált, amelyet az Azure AD nem ismer fel
Egy harmadik féltől származó MFA-megoldást használó partner az MFA-t implementálta a felhasználók számára. A partner azonban nem tudja megfelelően konfigurálni a harmadik féltől származó MFA-megoldást az Azure AD-be való továbbításra, hogy a felhasználó hitelesítése során az MFA ellenőrzése befejeződött. Ez a technikai kivétel érvényes oka?

**Válasz** : igen, ezt a problémát a technikai kivétel érvényes okaként lehet figyelembe venni. A technikai kivételre vonatkozó kérelem elküldése előtt erősítse meg a harmadik féltől származó MFA-megoldás szolgáltatóját, hogy az MFA-megoldás nem konfigurálható úgy, hogy az *authenticationmethodsreferences* -jogcímet ( *multipleauthn* értékkel) az Azure ad-be, hogy az MFA-ellenőrzés a felhasználó hitelesítése során is befejeződik. A technikai kivételre vonatkozó kérelem elküldésekor meg kell adnia a használatban lévő harmadik féltől származó MFA-megoldás részleteit, és jeleznie kell az integrációs módszert (például az identitás-összevonás vagy az egyéni Azure AD-vezérlő használata), és a következő információkat kell megadnia a technikai kivételi kérelemben a támogató dokumentumként:

- A harmadik féltől származó MFA-konfigurációk.

- A harmadik féltől származó MFA-kompatibilis fiók által futtatott [partneri biztonsági követelmények tesztelésének](/powershell/partnercenter/test-partner-security-requirements) eredménye.

- Az Ön által használt, harmadik féltől származó MFA-megoldás megvásárlási sorrendje.

### <a name="how-to-submit-a-request-for-technical-exception"></a>Technikai kivételre vonatkozó kérelem beküldése

Technikai kivételre vonatkozó kérelem küldése:

1. Jelentkezzen be a partner Center szolgáltatásba globális rendszergazdai vagy rendszergazdai ügynökként.

2. Hozzon létre egy új partneri szolgáltatási kérelmet a **Support**  >  **partneri támogatási kérelmek** támogatásához, majd az **új kérelem** lehetőségre kattintva.

3. **MFA-kérelem** keresése a keresőmezőbe; vagy válassza a **CSP** kategóriából lehetőséget, majd válassza a **fiókok, előkészítés, hozzáférés** a témához lehetőséget, majd válassza az **MFA – kérelem** az altémakörből, majd a **következő lépés** lehetőséget.

4. Adja meg a technikai kivételt kérő szolgáltatás beküldéséhez kért adatokat, majd kattintson a **Submit (Küldés** ) gombra.

A Microsoft akár három munkanapot is igénybe vehet, hogy választ adjon a technikai kivételre vonatkozó kérelemre.