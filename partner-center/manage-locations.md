---
title: Helyek kezelése a partnerfiókban
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Megtudhatja, hogyan adhat hozzá új helyet, és hogyan használja fel a hely MPN-azonosítóját az ösztönzőprogramokban, a CSP-üzletben, az előfizetésben és más tranzakciókban.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 13d6e7dc4722227035be2b24df48427f2008bb14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151780"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Az MPN-fiók helyének kezelése és hely hozzáadása (törlése)


**Megfelelő szerepkörök:** Globális rendszergazdai | Fiók rendszergazdája

A hely MPN-azonosítója azonosítja a vállalat egyes helyeket. A hely MPN-azonosítójával regisztrálható az ösztönzőprogramokba, tranzakciókat Felhőszolgáltató (CSP) és egyéb üzleti tranzakciókat. A globális MPN-azonosítót nem tranzakciós tevékenységekhez, például támogatási kérelmekhez használjuk.

## <a name="the-following-scenario-is-typical"></a>A következő forgatókönyv jellemző:

A Contoso globális partnerfiókkal (PGA) rendelkezik az Egyesült Királyságban. A PGA a regisztrált jogi vállalkozásuk, és annak globális MPN-azonosítóját az összes nem tranzakciós üzlet kezelésére használják. A Contoso emellett partnerhelyi fiókokkal (PLA) is rendelkezik, amelyek egyenértékűek az Egyesült Királyság, Franciaország és az USA más helyén található leányvállalatokkal vagy részlegekkel. Az MPN-fiók struktúrájában ezek a PLA-k egyedi hely MPN-azonosítókként vannak ábrázolva. A PLA-k tranzakciós üzleti tevékenységhez, például CSP-khez vagy ösztönzőprogramokhoz használhatók. A kifizetések adott helyekhez vannak kötve. 

>[!NOTE]
>Egy CSP-bérlő és egy MPN-helyazonosító között 1–1 kapcsolat áll elő.

:::image type="content" source="images/locations/locations1.png" alt-text="Az MPN-helyek struktúrája":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Új fiók csp-vállalkozáshoz való hozzáadásának előfeltételei

Új VÁLLALATI CSP-fiók hozzáadásához először is meg kell bizonyosodni arról, hogy teljesülnek az előfeltételek.

1. Egy hely MPN-azonosítóval kell lennie abban az országban, ahol CSP-vállalkozást szeretne. Új MPN-hely létrehozásához olvassa el alább az "MPN-hely hozzáadása" adatokat.
  
1. Új regisztráció létrehozásához olvassa CSP Indirect Reseller [Közvetett szolgáltatókkal való munka részt.](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Ne felejtsen el bejelentkezni az **új** CSP-fiók új hitelesítő adataival.  Ne használja a meglévő hitelesítő adatait, mert Partnerközpont a rendszer felismeri, hogy már rendelkezik fiókkal.

2. Fogadja el Microsoft Partnerszerződés és aktiválja a fiókot.

1. Ha közvetlen számlázási partnerként szeretne regisztrálni, olvassa el a Következőt: A közvetlen számlázási [partnerekre vonatkozó követelmények](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>MPN-helyek megtekintése és frissítése

1. Jelentkezzen be az Partnerközpont [irányítópultra](https://partner.microsoft.com/dashboard/home) az MPN-fiókja hitelesítő adataival. (Az MPN hitelesítő adatai különbözhetnek a CSP hitelesítő adataitól) 
 
1. A Beállítások **ikonon** válassza a **Fiókbeállítások,** Szervezeti **profil,** **Jogi lehetőséget.** 

1. A **Partner lapon** ellenőrizze, hogy nincs-e szalagcím-hibaüzenet, amely arra kéri, hogy javítsa ki a PMC-ről migrált helyeket.  Ha a helyek nem megfelelően voltak beállítva a PMC-n, és még nem voltak pc-re állítva, frissítenie kell ezeket a helyeket.

:::image type="content" source="images/locations/location-two.png" alt-text="A képernyőkép bemutatja, hogyan frissítheti a helyet.":::
 
4.  A **PMC-helyek áttekintése képernyőn** válassza a Frissítés **lehetőséget.**
Frissítse a következő mezőket:

- **Név mező:** Győződjön meg arról, hogy a vállalat helyének neve helyes. Ha duplikált hiba jelenik meg, próbáljon meg például Contoso-ről Contoso, Inc-re vált.

- **Jogi személy mező:** Győződjön meg arról, hogy azt a jogi entitást választotta ki, amelyhez a hely kötődik

- **Az 1. & 2 mező:** Ellenőrizze, hogy a cím helyes-e

- **City & State/Province (Állam/Tartomány)** mezők: Győződjön meg arról, hogy a város és az állam/tartomány közötti kombináció helyes. Vannak országok, ahol az Állam/Tartomány kiválasztására vonatkozó legördülő menü érvényes, és más országokban a mezőt manuálisan kell beszúrni.

- **IRÁNYÍTÓSZÁM mező:** Győződjön meg arról, hogy az Irányítószám mező megfelel a megadott országnak, régiónak, városnak vagy címnek.

- **Elsődleges kapcsolattartási adatok mezői:** Győződjön meg arról, hogy az első és a vezetéknév mező ki van töltve, és hogy a megadott e-mail-cím munkahelyi e-mail-cím, nem pedig személyes cím (például @outlook.com , @live.com stb.)

- **Telefonszám mező:** Győződjön meg arról, hogy a Telefonszám NEM tartalmaz speciális karaktereket, szóközöket vagy országkódot. A Telefonszám mezőben megadott érték mindig legfeljebb 10 karaktert tartalmazhat.

5. Ha nem jelenik meg hibaüzenet, akkor a Beállítások lapon válassza a Fiókbeállítások, a Szervezeti **profil,** az **Azonosítók lehetőséget.**

6. Keresse meg a "Hely" típusú MPN-azonosítót, amely megfelel a CSP-fiók országának, és használja a társítás befejezéséhez.

7. Ha nem találja a használni kívánt CSP-fióknak megfelelő hely MPN-azonosítót, hozzáadhat egy új helyet, amely létrehoz egy új MPN-azonosítót. Lásd **alább az MPN-hely hozzáadását.**

## <a name="add-an-mpn-location"></a>MPN-hely hozzáadása

1. Jelentkezzen be az MPN-fiókkal a Partnerközpont. (Az MPN hitelesítő adatai különbözhetnek a CSP hitelesítő adataitól.) Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultsággal kell lennie. 

1. A Beállítások **ikonra kattintva** válassza a **Fiókbeállítások,** majd a Szervezeti **profil lehetőséget.**

2. Válassza **a Jogi** lehetőséget, majd a Partner **lapon** válassza az Üzleti **helyek,** majd a Hely **hozzáadása lehetőséget.**

3. Adja meg a szükséges adatokat, beleértve a vállalathoz hozzáadni kívánt hely nevét, címét és kapcsolattartóját.
 
1. Válassza **a Hely hozzáadása lehetőséget.** Ezzel létrehoz egy új MPN-azonosítót az új helyhez, amely a CSP-tranzakciókhoz és -ösztönzőkhez használható.

:::image type="content" source="images/legal-biz.png" alt-text="Új jogi vállalkozás hozzáadása":::

> [!NOTE]
> Miután hozzáadott egy helyet a Partnerközpont, nem távolíthatja el. Ha a megfelelő **MPN-azonosítót** használta a bejelentkezéshez Partnerközpont az MPN megjelenik a bal oldali menüben.

## <a name="add-the-registration-number-id"></a>A regisztrációs szám azonosítójának hozzáadása

Ha Ön közvetett szolgáltató, közvetlen számlázási partner vagy közvetett viszonteladó, és a következő országokban új vagy meglévő ügyfelekkel üzleti kapcsolatban áll, meg kell adnia a vállalat regisztrációs azonosítószámait. Ha az alábbi listán nem szerepel az üzleti tevékenység országa, a regisztrációs azonosító megadása nem kötelező.

- Örményország 
- Azerbajdzsán 
- Belarusz 
- Brazília 
- Magyarország 
- India 
- Irak 
- Kazahsztán 
- Kirgizisztán 
- Moldova 
- Mianmar 
- Lengyelország 
- Oroszország 
- Szaúd-Arábia 
- Dél-afrikai Köztársaság 
- Dél-Szudán  
- Tádzsikisztán 
- Thaiföld
- Törökország 
- Ukrajna 
- Egyesült Arab Emírségek 
- Üzbegisztán 
- Venezuela
- Vietnam 


További információkért olvassa el a [regisztrációs azonosító száminformációját.](reg-number-id.md)

## <a name="delete-a-location"></a>Hely törlése

Egy hely fiókból való törléséhez fel kell vennie a kapcsolatot a [partnertámogatással.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b) Győződjön meg arról, hogy megértette ennek a műveletnek a hatását. Törölt helyek nem olvashatók be, és az adott MPN-azonosítóhoz kötődő adatokat a rendszer többé nem ismeri fel vagy nem aktív a vállalatnál.

## <a name="change-country-of-partner-global-account"></a>Partner globális fiókjának országának módosítása 

1. Jelentkezzen be az MPN-fiókkal a Partnerközpont. (Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól.) Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell lennie. 

2. A **Partner lapon** válassza az Üzleti **helyek** lapot, és ellenőrizze a helyek listáját, és ellenőrizze, hogy a jogi személyként kívánt hely szerepel-e a listán. 
 
1. Hely hozzáadásához kattintson **az Add a location**(Hely hozzáadása) elemre, majd a úszó menüben adja meg a szükséges adatokat, beleértve a vállalathoz hozzáadni kívánt hely üzleti nevét, címét és elsődleges kapcsolattartóját. 
 
1. Válassza **az Ország/régió** legördülő lista melletti Ország **módosítása** lehetőséget, és kövesse a lépéseket. 

:::image type="content" source="images/lbp.png" alt-text="Jogi üzleti profil adatainak úszó panele":::

5. Kattintson a **Mentés** gombra.

6. Az MPN globális fiók országa az új jogi országra változik.
  
## <a name="next-steps"></a>Következő lépések

- Ismerje meg az [ellenőrzési folyamatot.](verification-responses.md)
