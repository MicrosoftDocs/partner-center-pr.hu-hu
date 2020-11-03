---
title: Partneri biztonsági követelmények állapota
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg az új kötelező követelményeket, amelyek növelik az Advisors, a Vezérlőpult-szállítók és a partnerek biztonságát a Cloud Solution Provider programban.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 1b6c2d56a0747ddf2bd1a821886e371ed698a4a1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528527"
---
# <a name="partner-security-requirements-status---get-answers-and-check-reports-about-current-status"></a>Partneri biztonsági követelmények állapot – válaszok beolvasása és a jelenlegi állapottal kapcsolatos jelentések megtekintése

**A következőkre vonatkozik**

- A Cloud Solution Provider program összes partnere
  - Közvetlen számla
  - Közvetett szolgáltató
  - Közvetett viszonteladó
- A Vezérlőpult összes szállítója
- Minden tanácsadó

**Megfelelő felhasználók**
- Az összes engedélyezett felhasználó, beleértve a vendég felhasználókat

A kiemelt prioritások közé tartozik a nagyobb adatvédelmi védelem és biztonság. Tudjuk, hogy a legjobb védelem a megelőzés, és hogy csak olyan erősek vagyunk, mint a leggyengébb kapcsolatunk. Ezért van szükségünk arra, hogy az ökoszisztémánk mindenki számára megfelelő biztonsági védelmet biztosítson. A partnerek és az ügyfelek védelme érdekében az Advisors, a Vezérlőpult-szállítók és a felhőalapú megoldás-szolgáltatói programban részt vevő partnerek számára kötelező biztonsági követelményeket vezetünk be.

2019. augusztus 1-től minden partnernek ki kell kényszeríteni a többtényezős hitelesítést a partner bérlője minden felhasználója, beleértve a szolgáltatásfiókok szolgáltatást is. Az új biztonsági házirendekkel kapcsolatos további információkért olvassa el a [partneri biztonsági követelmények](partner-security-requirements.md)című témakört.

Azt szeretnénk biztosítani, hogy minden felhasználó rendelkezik MFA-kihívással minden egyes hitelesítéshez. Ez a következő módszerek egyikével valósítható meg:

- prémium szintű Azure AD megvalósítása annak biztosítása érdekében, hogy az MFA minden felhasználónál érvényben legyen
- Az [Azure ad biztonsági Alapértelmezések](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) implementálása
- Harmadik féltől származó megoldás megvalósítása az MFA minden felhasználó számára való betartatása érdekében

## <a name="partner-security-requirements-status"></a>Partneri biztonsági követelmények állapota

Ez a jelentés segítséget nyújt a biztonsági követelmények állapotának ellenőrzésében azáltal, hogy megtekinti, hol lehet rövid. A nyomon követés rendszeresen frissül.

>[!NOTE]
>A partneri biztonsági követelmények állapotjelentés csak a partner Centerben támogatott. Az Egyesült Államok kormánya vagy Microsoft Cloud Németország Microsoft Cloud nem érhető el. Azt javasoljuk, hogy a szuverén felhő (21Vianet, USA kormánya és Németország) által lebonyolított összes partner azonnal alkalmazza ezeket az új biztonsági követelményeket. Ezeknek a partnereknek azonban nincs szükségük az új biztonsági követelmények teljesítésére, 2019. augusztus 1-jétől érvényesek. A Microsoft további részleteket biztosít a szuverén felhőkre vonatkozó biztonsági követelmények végrehajtásával kapcsolatban a jövőben.

## <a name="multi-factor-authentication-mfa-report"></a>Jelentés a többtényezős hitelesítéshez (MFA)

A partneri központ MFA-jelentése a partnerek MFA-implementációjának betekintését nyújtja, mivel kétféle mérőszámot biztosít az MFA-konfiguráció és a CSP-bérlő partner Center-tevékenységei alapján: 

### <a name="mfa-configuration-on-a-csp-tenant"></a>MFA-konfiguráció CSP-bérlőn

Ez a metrika a CSP-bérlőn napi rendszerességgel rögzített és jelentett MFA-konfigurációhoz kapcsolódik. Az engedélyezett felhasználói fiókok százalékos arányát az MFA által kényszerített, ezen MFA- [Beállítások](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started)használatával méri. Például:

- A contoso egy 110 felhasználói fiókkal rendelkező CSP-partner a bérlőben, a felhasználói fiókok közül 10 le van tiltva. 
- Az 100-as számú felhasználói fiókból a 90 a megadott [MFA-beállítások](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started)használatával érvényesíti az MFA-t. Ezért a metrika 90%-ot mutat. 

### <a name="partner-center-activities-with-mfa"></a>Partner Center-tevékenységek MFA-val

Minden alkalommal, amikor az alkalmazottak bejelentkeznek a partneri központba, vagy az API-kon keresztül, a partner centeren keresztül kapnak vagy küldenek adatküldést, a biztonsági állapotuk kihívást jelent, és nyomon követik azokat. A biztonsági állapot nyomon követésében is szerepelnek az alkalmazásai és a Vezérlőpult gyártói alkalmazásai is. A megjelenített állapot az elmúlt hét napban van megadva.

#### <a name="mfa-verification-completed-by-users"></a>Az MFA ellenőrzése a felhasználók által befejeződött

Ez a metrika a partneri központ irányítópultján lévő tevékenységekhez kapcsolódik. Az MFA-ellenőrzést végző felhasználók által végrehajtott műveletek százalékos arányát méri. Például:

- A contoso egy CSP-partner, amelyben két rendszergazdai ügynök, Jane és John található.
- Az első napon Jane bejelentkezett a partner Center irányítópultra az MFA-ellenőrzés nélkül, és három műveletet hajtott végre.
- A második napon John bejelentkezett a fiókpartner-irányítópultra az MFA-ellenőrzés nélkül, és öt műveletet hajtott végre.
- A harmadik napon Jane bejelentkezett a partner Center-irányítópultra az MFA-ellenőrzés és két művelet végrehajtásával.
- A fennmaradó négy napon belül nem történt művelet az ügynöktől.
- A 7 napos ablakban végrehajtott 10 műveletből kettőt a felhasználó MFA-ellenőrzéssel végzett. A metrika ezért 20%-ot mutat.

Az **MFA nélküli fájlkiszolgáló-kérések** használatával megtudhatja, hogy melyik felhasználó jelentkezett be a fiókpartner-irányítópultra az MFA-ellenőrzés nélkül, valamint a legutóbbi látogatás időpontját a jelentéskészítési időszak során.

#### <a name="appuser-authentication"></a>Alkalmazás + felhasználói hitelesítés

Ez a mérőszám a partner Center API-kérelmek alkalmazás-és felhasználói hitelesítéssel végzett használatával kapcsolatos. A hozzáférési jogkivonattal rendelkező, MFA-jogcímeket használó API-kérelmek százalékos arányát méri. Például:

- A fabrikam egy CSP-partner, és egy CSP-alkalmazással rendelkezik, amely az alkalmazás és a felhasználó hitelesítését, valamint az alkalmazáson belüli hitelesítési módszereket használja.
- Az alkalmazás első napján három API-kérelmet készítettek, amelyeket az alkalmazások és a felhasználók hitelesítési módszere által az MFA ellenőrzése nélkül kapott hozzáférési jogkivonat támogat.
- A második napon az alkalmazás öt API-kérelmet készített, amelyeket egy csak az alkalmazáson alapuló hitelesítéssel kapott hozzáférési jogkivonat támogat.
- A harmadik napon az alkalmazás két API-kérést hajtott végre, amelyeket egy, az App + felhasználói hitelesítési módszer és az MFA-hitelesítés használatával kapott hozzáférési jogkivonat támogat.
- A fennmaradó négy napon belül nem történt művelet az ügynöktől.
- A második nap öt API-kérelmét, amelyet csak az alkalmazáson belüli hitelesítéssel kapott hozzáférési jogkivonat támogat, a rendszer kihagyja a metrikát, mivel nem használja fel a felhasználói hitelesítő adatokat. A fennmaradó öt műveletből közül kettőt az MFA-ellenőrzéssel kapott hozzáférési jogkivonat támogat. Ezért a metrika 40%-ot mutat.

Ha szeretné megismerni, hogy mely alkalmazás-és felhasználói tevékenységek eredményezik a nem 100%-ot ezen a metrikán, használja a következő fájlokat:

- Az **API-kérelmek összefoglalása** az alkalmazás általános MFA-állapotának megismeréséhez.
- Az **összes API-kérés** a bérlő felhasználói által benyújtott egyes API-kérelmek részleteinek megismerése érdekében az eredmény legfeljebb 10 000 a legutóbbi, a jobb letöltési élményhez.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>Mi a teendő, ha az MFA-jelentéshez tartozó mérőszámok nem 100%

Előfordulhat, hogy a partneri központ MFA-jelentésében szereplő mérőszámok nem lehetnek 100%-ban az MFA-t megvalósító partnereink számára. A következő szempontokat érdemes figyelembe venni.

> [!NOTE]
> Dolgoznia kell a szervezete azon felhasználóinak, akik már ismerik az Identitáskezelés és az MFA-megvalósítást a partner bérlője számára.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>Az MFA-t implementálta a partner bérlője számára?

Ha nem, először az MFA-t kell megvalósítani a partner bérlője számára. Az MFA megvalósításával kapcsolatos részletekért tekintse meg a [partner biztonsági követelményét](partner-security-requirements.md)ismertető cikket.

### <a name="have-you-only-recently-completed-mfa-implementation"></a>Csak a közelmúltban végezte el az MFA-implementációt?

A metrikák napi rendszerességgel vannak kiszámítva, és figyelembe veszik az elmúlt hét napban végrehajtott műveleteket. Ha csak a közelmúltban végezte el az MFA-implementációt a partner bérlője számára, akkor a metrikák nem lehetnek 100%-ban.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>Ki lett zárva néhány felhasználói fiók az MFA-implementációból?

Ismerje meg, hogy az aktuális MFA-implementáció az összes felhasználói fiókra vonatkozik-e, vagy csak néhányat. Egyes MFA-megoldások házirend-alapúak, és támogatják a felhasználók kizárását, míg másoknak felhasználói alapon explicit módon engedélyeznie kell az MFA-t. Győződjön meg arról, hogy a jelenlegi MFA-implementációból nem kizárt felhasználó. Minden olyan felhasználói fiók, amely ki van zárva, és bejelentkezik a partner központba a CSP-vel kapcsolatos tevékenységek elvégzéséhez, a metrikák nem lehetnek 100%-ra.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>Az MFA csak bizonyos feltételek teljesülése esetén szükséges?

Ismerje meg, hogy az aktuális implementáció csak bizonyos körülmények között érvényesíti az MFA-t. Egyes MFA-megoldások rugalmasságot biztosítanak, hogy csak bizonyos feltételek teljesülése esetén lehessen érvényesíteni az MFA-t. A felhasználó például ismeretlen eszközről vagy ismeretlen helyről férhet hozzá. Az a felhasználó, aki engedélyezve van az MFA számára, de nem szükséges az MFA-ellenőrzés elvégzéséhez a partner központhoz való hozzáféréskor, a metrikák nem lehetnek 100%-ban.

>[!NOTE]
>Azon partnereink számára, akik az Azure AD biztonsági alapértékei segítségével implementálták az MFA-t, fontos megjegyezni, hogy a nem rendszergazdai jogú felhasználói fiókok esetében a többtényezős hitelesítés a kockázat alapján lesz kikényszerítve. A rendszer csak a kockázatos bejelentkezési kísérletek során kéri a felhasználókat az MFA-ra (például a felhasználó egy másik helyről jelentkezik be). Emellett a felhasználók legfeljebb 14 napig regisztrálhatnak az MFA-ra. Azok a felhasználók, akik nem teljesítik az MFA-regisztrációt, nem lesznek felszámítva az MFA-ellenőrzésre a 14 napos időszakban. Ezért az is előfordulhat, hogy a metrikák nem lehetnek 100%-ban olyan partnereink számára, akik az Azure AD biztonsági alapértékeit használva implementálták az MFA-t.

### <a name="are-you-using-third-party-mfa-solution"></a>Harmadik féltől származó MFA-megoldást használ?

Ha harmadik féltől származó MFA-megoldást használ, azonosítsa, hogyan integrálja azt az Azure AD-vel. Általánosságban két módszer létezik, például az összevonás és az egyéni vezérlők:

* **Identitás-összevonás** – ha az Azure ad hitelesítési kérelmet kap, az Azure ad átirányítja a felhasználót az összevont identitás-szolgáltatóba a hitelesítéshez. A sikeres hitelesítés után az összevont identitás-szolgáltató átirányítja a felhasználót az Azure AD-re, és egy SAML-tokent is. Ahhoz, hogy az Azure AD felismerje, hogy a felhasználó az összevont identitás-szolgáltatóhoz való hitelesítés során az MFA-ellenőrzés befejeződött, az SAML-jogkivonatnak tartalmaznia kell a *authenticationmethodsreferences* jogcímet ( *multipleauthn* ). Győződjön meg arról, hogy az összevont identitás-szolgáltató támogatja-e a jogcímek kiállítását. Ha igen, ellenőrizze, hogy az összevont identitás-szolgáltató konfigurálva van-e. Ha a jogcím hiányzik, az Azure AD (és így a partner központ) nem fogja tudni, hogy a felhasználó az MFA-ellenőrzés befejezése után hiányzik a jogcím, a metrika nem lehet 100%.

* **Egyéni vezérlő** – az Azure ad egyéni vezérlője nem használható annak azonosítására, hogy egy felhasználó egy harmadik féltől származó MFA-megoldáson keresztül végezte-e az MFA-ellenőrzést. Ennek eredményeképpen minden olyan felhasználó, aki az MFA-ellenőrzést egy egyéni vezérlőn végezte el, mindig az Azure AD-ben fog megjelenni (és a partneri központban), mivel nem fejeződött be az MFA-ellenőrzés. Ha lehetséges, javasoljuk, hogy az Azure AD-vel való integráció során egyéni vezérlőként váltson az identitás-összevonás használatára.

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>Annak meghatározása, hogy mely felhasználók jelentkezett be a partner központba MFA nélkül

Hasznos lehet megállapítani, hogy mely felhasználók jelentkeznek be a partneri központba az MFA-ellenőrzés nélkül, és hogy a jelenlegi MFA-implementációban ellenőrizze őket. Az [Azure ad bejelentkezési jelentés](/azure/active-directory/reports-monitoring/concept-sign-ins) használatával megtudhatja, hogy a felhasználó teljesítette-e az MFA-ellenőrzést. Az Azure AD bejelentkezési jelentés jelenleg csak olyan partnereink számára érhető el, akik prémium szintű Azure ADre vagy bármely O365 SKU-ra előfizetettek, beleértve a prémium szintű Azure AD (például EMS).

## <a name="next-steps"></a>Következő lépések

- [A partner Center biztonsági Orientációs csoportjának közössége](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [A partneri központ biztonsági követelményei](partner-security-requirements.md)
- [A partner Center biztonsági követelményei – gyakori kérdések](partner-security-requirements-faq.md)