---
title: Biztonsági követelmények állapotjelentése
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan ellenőrizheti, hogy a biztonsági követelmények megfelelnek-e a biztonsági követelmények állapotjelentésének, és hogyan Partnerközpont MFA-jelentésnek
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: a429706848a469aace2704d4eaf3d57898ae578f
ms.sourcegitcommit: d96ad93449da4c914becfffab167cdc1aa165ada
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/25/2021
ms.locfileid: "112915626"
---
# <a name="security-requirements-status-report"></a>Biztonsági követelmények állapotjelentése

**Megfelelő szerepkörök:** CPV-rendszergazdai | Globális rendszergazda

Ez a cikk a biztonsági követelmények állapotjelentését ismerteti a Partnerközpont. Ez a jelentés metrikákat biztosít a partnerbérlő felhasználói számára a többtényezős hitelesítés (MFA) partnerbiztonsági követelményeinek való megfelelésről. [](partner-security-requirements.md)

A jelentés eléréséhez a [következő](https://partner.microsoft.com/dashboard)Partnerközpont: **Beállítások**  >  **Fiókbeállítások**  >  **Biztonsági követelmények állapota.** A jelentés naponta frissül, és az elmúlt hét nap bejelentkezési adatait tükrözi.

>[!NOTE]
>A biztonsági követelmények állapotjelentése csak a Partnerközpont. Nem érhető el a Microsoft Cloud for US Government Microsoft Cloud Germany szolgáltatásban. Határozottan javasoljuk, hogy a szuverén felhőn (az Egyesült Államok kormányán és Németországon) keresztül tranzakciós partnerek azonnal elfogadják ezeket az új biztonsági követelményeket. Ezek a partnerek azonban jelenleg nem szükségesek az új biztonsági követelmények követelményeknek való megfeleléshez. A Microsoft a jövőben további részleteket nyújt a szuverén felhőkre vonatkozó biztonsági követelmények betartatásával kapcsolatban.

## <a name="security-status-metrics"></a>Biztonsági állapot mérőszámai

A biztonsági követelmények állapotjelentése betekintést nyújt a partnerek MFA-jának megvalósításába, valamint metrikákat biztosít az MFA konfigurációjára és Partnerközpont partnerbérlőkre vonatkozó tevékenységekre. A következő szakaszok részletesebben ismertetik ezeket a metrikákat.

### <a name="mfa-configuration-on-a-partner-tenant"></a>MFA-konfiguráció egy partnerbérlőn

Az **MFA-val** rendelkező engedélyezett felhasználói fiókok százalékos aránya az itt felsorolt beállításokkal kényszerítve metrikát jeleníti meg azon partnerbérlő engedélyezett felhasználói fiókjainak százalékos arányát, amelyek esetében az MFA kényszerítve van. Ezen [MFA-beállítások egyikének használatával biztosíthatja](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) a megfelelőséget. A rendszer naponta rögzíti és jelenti az adatokat. Például:

- A Contoso egy CSP-partner 110 felhasználói fiókkal a bérlőben, és ezek közül 10 le van tiltva. 
- A 100 felhasználói fiók közül 90 van kikényszeríteni az MFA-t a megadott [MFA-beállításokkal.](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) Ezért a metrika 90%-ot mutat. 

### <a name="partner-center-requests-with-mfa"></a>Partnerközpont MFA-val

Minden alkalommal, amikor az alkalmazottak bejelentkeznek Partnerközpont, vagy API-kon keresztül leküldenek vagy elküldenek adatokat a Partnerközpont biztonsági állapotuk ellenőrzése és nyomon követése is meg lesz függetlenül egymástól. A biztonsági állapot nyomon követésének része az alkalmazások és a vezérlőpult szállítói alkalmazásai is. Ezek az adatok az **MFA-val** Partnerközpont kérelmek százalékos aránya metrikákban jelennek meg, és az elmúlt hét napot tükrözik.

#### <a name="dashboard-mfa-verification"></a>Irányítópult MFA-ellenőrzése

A **portálon Partnerközpont metrika** az irányítópulton belüli Partnerközpont kapcsolódik. Az MFA-ellenőrzést végzett felhasználók által végzett műveletek százalékos arányát méri. Például:

- A Contoso egy CSP-partner két rendszergazdai ügynökkel, Jane és Johnnal.
- Az első nap Jane bejelentkezett az irányítópultra Partnerközpont MFA-ellenőrzés nélkül, és három műveletet végzett.
- A második napon John bejelentkezett az irányítópultra Partnerközpont MFA-ellenőrzés nélkül, és öt műveletet végzett.
- A harmadik napon Jane bejelentkezett az Partnerközpont MFA-ellenőrzéssel, és két műveletet végzett.
- Egyik ügynök sem műveleteket készített a hátralévő négy napban.
- A hétnapos ablak 10 művelete közül kettőt A felhasználó készített MFA-ellenőrzéssel. Ezért a metrika 20%-ot mutat.

Az **MFA** nélküli fájlportál-kérésekkel megértheti, hogy melyik felhasználó jelentkezett be az Partnerközpont irányítópultra MFA-ellenőrzés nélkül, és hogy mikor történt az utolsó látogatás a jelentéskészítési időszakban.

#### <a name="appuser-mfa-verification"></a>Alkalmazás+felhasználó MFA-ellenőrzése

Az **API-n vagy SDK-n keresztüli metrika** az App+User api-kérelmeken keresztüli app+Partnerközpont kapcsolódik. MFA-jogcímet használó hozzáférési jogkivonat használatával lekért API-kérések százalékos arányát méri. Például:

- A Fabrikam egy CSP-partner, és olyan CSP-alkalmazással rendelkezik, amely az App+User hitelesítési és a csak az alkalmazásra vonatkozó hitelesítési módszereket vegyesen használja.
- Az első napon az alkalmazás három API-kérést adott le, amelyeket egy MFA-ellenőrzés nélküli App+User hitelesítési módszerrel kapott hozzáférési jogkivonat adott vissza.
- A második napon az alkalmazás öt API-kérést készített, amelyeket egy csak alkalmazáshitelesítéssel kapott hozzáférési jogkivonattal tettek elérhetővé.
- A harmadik napon az alkalmazás két API-kérést adott le, amelyeket egy, az App+User hitelesítési módszer és az MFA-ellenőrzés használatával kapott hozzáférési jogkivonat adott vissza.
- Egyik ügynök sem műveleteket készített a hátralévő négy napban.
- A második napon a csak alkalmazáshitelesítéssel kapott hozzáférési jogkivonattal visszacsatolt öt API-kérelem kimarad a metrikákból, mivel nem használ felhasználói hitelesítő adatokat. A fennmaradó öt művelet közül kettőt egy MFA-ellenőrzéssel kapott hozzáférési jogkivonattal egészül ki. Ezért a metrika 40%-ot mutat.

Ha szeretné tudni, hogy mely App+user tevékenységek esetén nem 100%-os a metrika, használjon fájlokat:

- **API-kérések összegzése** az MFA általános állapotának alkalmazás szerint való áttekintéshez.
- **A** bérlő felhasználói által lekért API-kérések részleteinek ért minden API-kérelem esetén az eredmény legfeljebb 10 000 legutóbbi kérésre van korlátozva a jobb letöltési élmény érdekében.

## <a name="actions-for-mfa-status-below-100"></a>Műveletek 100% alatti MFA-állapothoz

Egyes MFA-hitelesítést megvalósító partnerek 100% alatti jelentésmetrikákat láthatnak. Hogy megértsük, miért érdemes megfontolni néhány tényezőt.

> [!NOTE]
> A szervezet egyik olyan személyével kell dolgoznia, aki ismeri a partnerbérlő identitáskezelését és MFA-implementációját.

### <a name="implemented-mfa-for-your-partner-tenant"></a>MFA megvalósítása a partnerbérlő számára

A megfelelőség eléréséhez implementálja az MFA-t a partnerbérlő számára. További információ az MFA implementálásról: Az API-k Partnerközpont vagy Partnerközpont [való használatának biztonsági követelményei.](partner-security-requirements.md)

>[!NOTE]
> Az MFA-metrikákat a rendszer naponta számítja ki, és figyelembe veszi az elmúlt hét napban végrehajtott műveleteket. Ha csak a közelmúltban implementálta az MFA-t a partnerbérlőjéhez, előfordulhat, hogy a metrikák még nem mutatják a 100%-ot.

### <a name="verify-mfa-on-all-user-accounts"></a>MFA ellenőrzése az összes felhasználói fiókon

Annak eldöntése, hogy a jelenlegi MFA-implementáció az összes felhasználói fiókot lefedi-e, vagy csak néhányat. Egyes MFA-megoldások házirendalapúak, és támogatják a felhasználók kizárását, míg másokhoz szükség lehet az MFA felhasználónkénti explicit engedélyezésére. Ellenőrizze, hogy nem zárt-e ki felhasználót a jelenlegi MFA-implementációból. Bármely felhasználói fiók, amely ki van zárva, és Partnerközpont csp-, CPV- vagy Advisor-tevékenység végrehajtásához bejelentkezik, a metrikák nem lesznek 100%-osak.

### <a name="review-your-mfa-conditions"></a>Az MFA-feltételek áttekintése

Annak eldöntése, hogy a jelenlegi implementáció csak bizonyos feltételek mellett kényszeríti-e az MFA-t. Egyes MFA-megoldások csak bizonyos feltételek teljesülését biztosítják az MFA kényszerítésében. A felhasználó például ismeretlen eszközről vagy ismeretlen helyről fér hozzá. Ha egy felhasználó engedélyezi az MFA-t, de nem szükséges az MFA-ellenőrzést végrehajtania a Partnerközpont elérésekor, akkor a metrikák nem lesznek 100%-osak.

>[!NOTE]
>Fontos megjegyezni, hogy azok a partnerek, akik az Azure AD biztonsági alapértelmezéseivel valósítják meg az MFA-t, fontos megjegyezni, hogy a nem rendszergazdai felhasználói fiókok esetében a többtényezős hitelesítés a kockázat alapján lesz kényszerítve. A rendszer csak a kockázatos bejelentkezési kísérletek során kéri a felhasználóktól az MFA-t (például ha a felhasználó egy másik helyről jelentkezik be). Emellett a felhasználóknak legfeljebb 14 napjuk lesz az MFA-regisztrációra. Azok a felhasználók, akik nem fejezték be az MFA-regisztrációt, nem fognak MFA-ellenőrzést végrehajtani a 14 napos időszakban. Ezért a metrikák várhatóan nem lesznek 100%-osak az olyan partnereknél, akik az Azure AD biztonsági alapértelmezéseivel valósítják meg az MFA-t.

### <a name="review-third-party-mfa-configurations"></a>Külső MFA-konfigurációk áttekintése

Ha külső MFA-megoldást használ, határozza meg, hogyan integrálja azt az Azure AD-val. Általában két módszer létezik, például az összevonás és az egyéni vezérlők:

* **Identitás-összevonás** – Amikor az Azure AD hitelesítési kérelmet kap, az Azure AD átirányítja a felhasználót az összevont identitásszolgáltatóhoz hitelesítésre. Sikeres hitelesítés esetén az összevont identitásszolgáltató visszairányítja a felhasználót az Azure AD-be egy SAML-jogkivonattal együtt. Ahhoz, hogy az Azure AD felismerje, hogy a felhasználó MFA-ellenőrzést végzett az összevont identitásszolgáltatóval való hitelesítéskor, az SAML-jogkivonatnak tartalmaznia kell az *authenticationmethodsreferences* jogcímet *(multipleauthn értékkel).* Ellenőrizze, hogy az összevont identitásszolgáltató támogatja-e az ilyen jogcímek kiállítását. Ha igen, ellenőrizze, hogy az összevont identitásszolgáltató konfigurálva van-e erre. Ha a jogcím hiányzik, az Azure AD (és ezért Partnerközpont) nem fogja tudni, hogy a felhasználó végzett MFA-ellenőrzést, és hiányzik a jogcím, ami azt okozhatja, hogy a metrika nem 100%.

* **Egyéni vezérlő** – Az Azure AD egyéni vezérlő nem használható annak azonosítására, hogy egy felhasználó végzett-e MFA-ellenőrzést külső MFA-megoldáson keresztül. Ennek eredményeképpen minden olyan felhasználó, aki egyéni vezérlővel végzett MFA-ellenőrzést, mindig úgy jelenik meg az Azure AD-ban (Partnerközpont), mint aki nem végzett MFA-ellenőrzést. Ahol lehetséges, javasoljuk, hogy az Azure AD-val való integrációkor váltson az Identity Federationre, és ne az Egyéni vezérlőre.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Annak azonosítása, hogy mely felhasználók jelentkeznek be Partnerközpont MFA nélkül

Hasznos lehet azonosítani, hogy mely felhasználók jelentkeznek be a Partnerközpont MFA-ellenőrzés nélkül, és ellenőrizni, hogy az aktuális MFA-implementációban vannak-e. Az Azure AD bejelentkezési jelentéssel kiderítheti, hogy a felhasználó [végzett-e MFA-ellenőrzést](/azure/active-directory/reports-monitoring/concept-sign-ins) vagy sem. Az Azure AD bejelentkezési jelentése jelenleg csak olyan partnerek számára érhető el, akik előfizetettek az prémium szintű Azure AD-ra vagy bármely O365-termékváltozatra, beleértve a prémium szintű Azure AD -t (például EMS).

## <a name="next-steps"></a>Következő lépések

- [Partnerközpont biztonsági útmutatási csoport közössége](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [A Partnerközpont biztonsági követelményei](partner-security-requirements.md)
- [Partnerközpont biztonsági követelményekkel kapcsolatos gyakori kérdések](partner-security-requirements-faq.yml)
