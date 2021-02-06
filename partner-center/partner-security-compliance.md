---
title: Biztonsági követelmények – állapotjelentés
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan tekintheti meg a biztonsági követelmények megfelelőségét az állapotjelentés és a partner Center MFA-jelentés alapján
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f521e05fbf0b3a6c209a84ed9ab53d2502960a5
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624153"
---
# <a name="security-requirements-status-report"></a>Biztonsági követelmények – állapotjelentés

**Megfelelő szerepkörök**
- Vezérlőpult-szállítók
- Globális rendszergazdák

Ez a cikk ismerteti a biztonsági követelmények állapotáról szóló jelentést a partner Centerben. Ez a jelentés a partner bérlő felhasználói számára a többtényezős hitelesítés (MFA) [partneri biztonsági követelményeinek](partner-security-requirements.md) megfelelőségére vonatkozó mérőszámokat biztosít.

Ha ezt a jelentést szeretné elérni a [partner Centerben](https://partner.microsoft.com/dashboard), lépjen a **Beállítások**  >  **fiók beállításai**  >  **biztonsági követelmények állapot** elemre. A jelentés naponta frissül, és a bejelentkezési adatokat tükrözi az elmúlt hét napban.

>[!NOTE]
>A biztonsági követelmények állapotáról szóló jelentés csak a partner Centerben támogatott. Az Egyesült Államok kormánya vagy Microsoft Cloud Németország Microsoft Cloud nem érhető el. Azt javasoljuk, hogy a szuverén felhőn (USA-beli kormányzaton és Németországban) keresztül lebonyolított összes partner azonnal alkalmazza ezeket az új biztonsági követelményeket. Ezek a partnerek azonban jelenleg nem szükségesek az új biztonsági követelmények teljesítéséhez. A Microsoft további részleteket biztosít a szuverén felhőkre vonatkozó biztonsági követelmények végrehajtásával kapcsolatban a jövőben.

## <a name="security-status-metrics"></a>Biztonsági állapot metrikái

A biztonsági követelmények állapota jelentés betekintést nyújt a partneri MFA-megvalósításba, és metrikákat biztosít az MFA-konfiguráció és a partneri központ tevékenységeihez a partner bérlők esetében. A következő szakaszokban részletesen ismertetjük ezeket a metrikákat.

### <a name="mfa-configuration-on-a-partner-tenant"></a>MFA-konfiguráció egy partner bérlőn

Az **engedélyezett felhasználói fiókok metrikai százalékos aránya az MFA által kényszerített, az itt felsorolt lehetőségek használatával:** az engedélyezett felhasználói fiókok százalékos arányát jeleníti meg a partner bérlőn, amelyeken az MFA érvénybe lép. A megfelelőség érdekében a következő [MFA-beállítások](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) egyikét használhatja. Ezeket az adatkészleteket naponta rögzítik és jelentik. Például:

- A contoso egy 110 felhasználói fiókkal rendelkező CSP-partner a bérlőben, a felhasználói fiókok közül 10 le van tiltva. 
- Az 100-as számú felhasználói fiókból a 90 a megadott [MFA-beállítások](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started)használatával érvényesíti az MFA-t. Ezért a metrika 90%-ot mutat. 

### <a name="partner-center-requests-with-mfa"></a>Az MFA-val rendelkező partner Center-kérelmek

Minden alkalommal, amikor az alkalmazottak bejelentkeznek a partneri központba, vagy az API-kon keresztül, a partner centeren keresztül kapnak vagy küldenek adatküldést, a biztonsági állapotuk kihívást jelent, és nyomon követik azokat. A biztonsági állapot nyomon követésének része az alkalmazások és a Vezérlőpult gyártói alkalmazásai is. Ezek az adatok a **partner központ felé irányuló kérelmek százalékos arányában** jelennek meg az MFA-val, és az elmúlt hét napban jelennek meg.

#### <a name="dashboard-mfa-verification"></a>Irányítópult MFA-ellenőrzése

A **partner Center-portálon keresztüli** metrika a partneri központ irányítópultján lévő tevékenységekhez kapcsolódik. Az MFA-ellenőrzést végző felhasználók által végrehajtott műveletek százalékos arányát méri. Például:

- A contoso egy CSP-partner, amelyben két rendszergazdai ügynök, Jane és John található.
- Az első napon Jane bejelentkezett a partner Center irányítópultra az MFA-ellenőrzés nélkül, és három műveletet hajtott végre.
- A második napon John bejelentkezett a fiókpartner-irányítópultra az MFA-ellenőrzés nélkül, és öt műveletet hajtott végre.
- A harmadik napon Jane bejelentkezett a partner Center-irányítópultra az MFA-ellenőrzés és két művelet végrehajtásával.
- A fennmaradó négy napon belül nem történt művelet az ügynöktől.
- A 7 napos ablakban végrehajtott 10 műveletből kettőt a felhasználó MFA-ellenőrzéssel végzett. A metrika ezért 20%-ot mutat.

Az **MFA nélküli fájlkiszolgáló-kérések** használatával megtudhatja, hogy melyik felhasználó jelentkezett be a fiókpartner-irányítópultra az MFA-ellenőrzés nélkül, valamint a legutóbbi látogatás időpontját a jelentéskészítési időszak során.

#### <a name="appuser-mfa-verification"></a>Alkalmazás-és felhasználói MFA-ellenőrzés

Az **API-n vagy SDK-n keresztüli** metrika az App + felhasználói hitelesítéshez kapcsolódik a partner Center API-kéréseken keresztül. A hozzáférési jogkivonattal rendelkező, MFA-jogcímeket használó API-kérelmek százalékos arányát méri. Például:

- A fabrikam egy CSP-partner, és egy CSP-alkalmazással rendelkezik, amely az alkalmazás és a felhasználó hitelesítését, valamint az alkalmazáson belüli hitelesítési módszereket használja.
- Az alkalmazás első napján három API-kérelmet készítettek, amelyeket az alkalmazások és a felhasználók hitelesítési módszere által az MFA ellenőrzése nélkül kapott hozzáférési jogkivonat támogat.
- A második napon az alkalmazás öt API-kérelmet készített, amelyeket egy csak az alkalmazáson alapuló hitelesítéssel kapott hozzáférési jogkivonat támogat.
- A harmadik napon az alkalmazás két API-kérést hajtott végre, amelyeket egy, az App + felhasználói hitelesítési módszer és az MFA-hitelesítés használatával kapott hozzáférési jogkivonat támogat.
- A fennmaradó négy napon belül nem történt művelet az ügynöktől.
- A második nap öt API-kérelmét, amelyet csak az alkalmazáson belüli hitelesítéssel kapott hozzáférési jogkivonat támogat, a rendszer kihagyja a metrikát, mivel nem használja fel a felhasználói hitelesítő adatokat. A fennmaradó öt műveletből közül kettőt az MFA-ellenőrzéssel kapott hozzáférési jogkivonat támogat. Ezért a metrika 40%-ot mutat.

Ha szeretné megismerni, hogy mely alkalmazás-és felhasználói tevékenységek eredményezik a nem 100%-ot ezen a metrikán, használja a következő fájlokat:

- Az **API-kérelmek összefoglalása** az alkalmazás általános MFA-állapotának megismeréséhez.
- Az **összes API-kérés** a bérlő felhasználói által benyújtott egyes API-kérelmek részleteinek megismerése érdekében az eredmény legfeljebb 10 000 a legutóbbi, a jobb letöltési élményhez.

## <a name="actions-for-mfa-status-below-100"></a>MFA-állapotra vonatkozó műveletek 100%-ban

Egyes, MFA-t megvalósító partnerek a 100% alatti jelentés metrikáit láthatják. A következő szempontokat érdemes figyelembe venni.

> [!NOTE]
> Dolgoznia kell a szervezete azon felhasználóinak, akik már ismerik az Identitáskezelés és az MFA-megvalósítást a partner bérlője számára.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Implementált MFA a partner bérlője számára

A megfelelőség eléréséhez az MFA-t kell megvalósítani a partner bérlője számára. Az MFA megvalósításával kapcsolatos további információkért lásd: [a partner Center vagy a partner Center API-k használatának biztonsági követelményei](partner-security-requirements.md).

>[!NOTE]
> Az MFA-metrikák napi rendszerességgel vannak kiszámítva, és figyelembe veszik az elmúlt hét napban végrehajtott műveleteket. Ha csak a közelmúltban végezte el az MFA-implementációt a partner bérlője számára, akkor a metrikák még nem jelennek meg 100%-ban.

### <a name="verify-mfa-on-all-user-accounts"></a>Az MFA ellenőrzése az összes felhasználói fiókon

Ismerje meg, hogy az aktuális MFA-implementáció az összes felhasználói fiókra vonatkozik-e, vagy csak néhányat. Egyes MFA-megoldások házirend-alapúak, és támogatják a felhasználók kizárását, míg másoknak felhasználói alapon explicit módon engedélyeznie kell az MFA-t. Győződjön meg arról, hogy a jelenlegi MFA-implementációból nem kizárt felhasználó. Minden olyan felhasználói fiók, amely ki van zárva, és bejelentkezik a partner központba a CSP-, CPV-vagy Advisor-alapú tevékenységek elvégzéséhez, a metrikák nem lehetnek 100%-ban.

### <a name="review-your-mfa-conditions"></a>MFA-feltételek áttekintése

Ismerje meg, hogy az aktuális implementáció csak bizonyos körülmények között érvényesíti az MFA-t. Egyes MFA-megoldások rugalmasságot biztosítanak, hogy csak bizonyos feltételek teljesülése esetén lehessen érvényesíteni az MFA-t. A felhasználó például ismeretlen eszközről vagy ismeretlen helyről férhet hozzá. Az a felhasználó, aki engedélyezve van az MFA számára, de nem szükséges az MFA-ellenőrzés elvégzéséhez a partner központhoz való hozzáféréskor, a metrikák nem lehetnek 100%-ban.

>[!NOTE]
>Azon partnereink számára, akik az Azure AD biztonsági alapértékei segítségével implementálták az MFA-t, fontos megjegyezni, hogy a nem rendszergazdai jogú felhasználói fiókok esetében a többtényezős hitelesítés a kockázat alapján lesz kikényszerítve. A rendszer csak a kockázatos bejelentkezési kísérletek során kéri a felhasználókat az MFA-ra (például a felhasználó egy másik helyről jelentkezik be). Emellett a felhasználók legfeljebb 14 napig regisztrálhatnak az MFA-ra. Azok a felhasználók, akik nem teljesítik az MFA-regisztrációt, nem lesznek felszámítva az MFA-ellenőrzésre a 14 napos időszakban. Ezért az is előfordulhat, hogy a metrikák nem lehetnek 100%-ban olyan partnereink számára, akik az Azure AD biztonsági alapértékeit használva implementálták az MFA-t.

### <a name="review-third-party-mfa-configurations"></a>Harmadik féltől származó MFA-konfigurációk áttekintése

Ha harmadik féltől származó MFA-megoldást használ, azonosítsa, hogyan integrálja azt az Azure AD-vel. Általánosságban két módszer létezik, például az összevonás és az egyéni vezérlők:

* **Identitás-összevonás** – ha az Azure ad hitelesítési kérelmet kap, az Azure ad átirányítja a felhasználót az összevont identitás-szolgáltatóba a hitelesítéshez. A sikeres hitelesítés után az összevont identitás-szolgáltató átirányítja a felhasználót az Azure AD-re, és egy SAML-tokent is. Ahhoz, hogy az Azure AD felismerje, hogy a felhasználó az összevont identitás-szolgáltatóhoz való hitelesítés során az MFA-ellenőrzés befejeződött, az SAML-jogkivonatnak tartalmaznia kell a *authenticationmethodsreferences* jogcímet ( *multipleauthn*). Győződjön meg arról, hogy az összevont identitás-szolgáltató támogatja-e a jogcímek kiállítását. Ha igen, ellenőrizze, hogy az összevont identitás-szolgáltató konfigurálva van-e. Ha a jogcím hiányzik, az Azure AD (és így a partner központ) nem fogja tudni, hogy a felhasználó az MFA-ellenőrzés befejezése után hiányzik a jogcím, a metrika nem lehet 100%.

* **Egyéni vezérlő** – az Azure ad egyéni vezérlője nem használható annak azonosítására, hogy egy felhasználó egy harmadik féltől származó MFA-megoldáson keresztül végezte-e az MFA-ellenőrzést. Ennek eredményeképpen minden olyan felhasználó, aki az MFA-ellenőrzést egy egyéni vezérlőn végezte el, mindig az Azure AD-ben fog megjelenni (és a partneri központban), mivel nem fejeződött be az MFA-ellenőrzés. Ha lehetséges, javasoljuk, hogy az Azure AD-vel való integráció során egyéni vezérlőként váltson az identitás-összevonás használatára.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Annak meghatározása, hogy mely felhasználók jelentkezett be a partner központba MFA nélkül

Hasznos lehet megállapítani, hogy mely felhasználók jelentkeznek be a partneri központba az MFA-ellenőrzés nélkül, és hogy a jelenlegi MFA-implementációban ellenőrizze őket. Az [Azure ad bejelentkezési jelentés](/azure/active-directory/reports-monitoring/concept-sign-ins) használatával megtudhatja, hogy a felhasználó teljesítette-e az MFA-ellenőrzést. Az Azure AD bejelentkezési jelentés jelenleg csak olyan partnereink számára érhető el, akik prémium szintű Azure ADre vagy bármely O365 SKU-ra előfizetettek, beleértve a prémium szintű Azure AD (például EMS).

## <a name="next-steps"></a>Következő lépések

- [A partner Center biztonsági Orientációs csoportjának közössége](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [A Partnerközpont biztonsági követelményei](partner-security-requirements.md)
- [A partner Center biztonsági követelményei – gyakori kérdések](partner-security-requirements-faq.md)
