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
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702892"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Az MPN-fiók helyének kezelése és hely hozzáadása (törlése)


**Megfelelő szerepkörök**

- Globális rendszergazda
- Fiókadminisztrátor

A hely MPN-azonosítója azonosítja a vállalat minden egyes helyét. A hely MPN-azonosítójával regisztrál az ösztönzőprogramokba, tranzakciókat Felhőszolgáltató (CSP) és egyéb üzleti tranzakciókat. A globális MPN-azonosítót nem tranzakciós tevékenységekhez, például támogatási kérelmekhez használjuk.

## <a name="the-following-scenario-is-typical"></a>A következő forgatókönyv jellemző:

A Contoso globális partnerfiókkal (PGA) rendelkezik az Egyesült Királyságban. A PGA a regisztrált jogi vállalkozásuk, és globális MPN-azonosítóját az összes nem tranzakciós üzlet felügyeletére használják. A Contoso emellett partnerihely-fiókokkal (PLA) is rendelkezik, amelyek egyenértékűek az Egyesült Királyság, Franciaország és az Egyesült Államok más helyeiben található leányvállalatokkal vagy részlegekkel. Az MPN-fiók struktúrájában ezek a PLA-k egyedi hely MPN-azonosítókként vannak ábrázolva. A PLA-k tranzakciós üzleti tevékenységhez, például CSP- vagy ösztönzőprogramokhoz használhatók. A kifizetések adott helyekhez vannak kötve. 

>[!NOTE]
>Egy CSP-bérlő és egy MPN-helyazonosító között 1–1 kapcsolat áll elő.

:::image type="content" source="images/locations/locations1.png" alt-text="Az MPN-helyek szerkezete":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Új fiók csp-vállalkozáshoz való hozzáadásának előfeltételei

Új VÁLLALATI CSP-fiók hozzáadásához először is meg kell bizonyosodni arról, hogy teljesülnek az előfeltételek.

1. A CSP-üzletnek abban az országban kell lennie, ahol az MPN-azonosítót el szeretné látni. Új MPN-hely létrehozásához olvassa el alább az "MPN-hely hozzáadása" adatokat.
  
1. Új regisztráció létrehozásához CSP Indirect Reseller: Közvetett [szolgáltatókkal való munka](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Ne felejtsen el bejelentkezni az **új** CSP-fiók új hitelesítő adataival.  Ne használja a meglévő hitelesítő adatait, mert Partnerközpont a rendszer felismeri, hogy már rendelkezik fiókkal.

2. Fogadja el Microsoft Partnerszerződés és aktiválja a fiókot.

1. Ha közvetlen számlázási partnerként szeretne regisztrálni, olvassa el a [Következőt: A közvetlen számlázási partnerekre vonatkozó követelmények](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>MPN-helyek megtekintése és frissítése

1. Jelentkezzen be az Partnerközpont [irányítópultra](https://partner.microsoft.com/dashboard/home) az MPN-fiókja hitelesítő adataival. (Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól) 
 
1. A Beállítások **ikonon** válassza a **Fiókbeállítások,** Szervezeti **profil,** **Jogi lehetőséget.** 

1. A **Partner lapon** ellenőrizze, hogy nem jelenik-e meg szalagcímes hibaüzenet, amely a PMC-ről migrált helyek kijavításán kéri.  Ha a helyek nem megfelelően vannak beállítva a PMC-n, és még nem voltak pc-re állítva, frissítenie kell ezeket a helyeket.

:::image type="content" source="images/locations/location-two.png" alt-text="A képernyőkép bemutatja, hogyan frissítheti a helyet.":::
 
4.  A **PMC-helyek áttekintése képernyőn** válassza a Frissítés **lehetőséget.**
Frissítse a következő mezőket:

- **Név mező:** Győződjön meg arról, hogy a vállalat helyének neve helyes. Ha duplikált hiba jelenik meg, próbáljon meg átváltást például a Contoso-ről a Contoso, Inc. fiókra.

- **Jogi személy mező:** Győződjön meg arról, hogy azt a jogi entitást választotta ki, amelyhez a hely kötődik

- **Az 1. & 2. mező:** Győződjön meg arról, hogy a cím helyes

- **City & State/Province (Állam/Tartomány)** mezőkben: Győződjön meg arról, hogy a város és az állam/tartomány közötti kombináció helyes. Vannak országok, ahol a State/Province (Állam/Tartomány) kiválasztására vonatkozó legördülő menüt kell alkalmazni, és más országokban a mezőt manuálisan kell beszúrni.

- **IRÁNYÍTÓSZÁM mező:** Győződjön meg arról, hogy az Irányítószám mező megfelel a megadott országnak, régiónak, városnak vagy címnek.

- **Elsődleges kapcsolattartási adatok mezői:** Győződjön meg arról, hogy az első és a vezetéknév mező ki van töltve, és hogy a megadott e-mail-cím munkahelyi e-mail-cím, nem pedig személyes cím (például @outlook.com , @live.com stb.)

- **Telefonszám mező:** Győződjön meg arról, hogy a Telefonszám NEM tartalmaz speciális karaktereket, szóközöket vagy országkódot. A Telefonszám mezőben megadott érték mindig legfeljebb 10 karaktert tartalmazhat.

5. Ha nem jelenik meg hibaüzenet, akkor a Beállítások lapon válassza a Fiókbeállítások, a Szervezeti **profil,** az **Azonosítók lehetőséget.**

6. Keresse meg a "Hely" típusú MPN-azonosítót, amely megfelel a CSP-fiók országának, és használja a társítás befejezéséhez.

7. Ha nem találja a használni kívánt CSP-fióknak megfelelő hely MPN-azonosítót, hozzáadhat egy új helyet, amely létrehoz egy új MPN-azonosítót. Lásd **alább az MPN-hely hozzáadását.**

## <a name="add-an-mpn-location"></a>MPN-hely hozzáadása

1. Jelentkezzen be az MPN-fiókkal a Partnerközpont. (Az MPN hitelesítő adatai különbözhetnek a CSP hitelesítő adataitól) . Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultsággal kell lennie. 

1. A Beállítások **ikonra kattintva** válassza a **Fiókbeállítások,** majd a Szervezeti **profil lehetőséget.**

2. Válassza **a Jogi** lehetőséget, majd a Partner **lapon** válassza az Üzleti **helyek lehetőséget,** majd kattintson a Hely **hozzáadása elemre.**

3. Adja meg a szükséges adatokat, beleértve a vállalathoz hozzáadni kívánt hely nevét, címét és kapcsolattartóját.
 
1. Kattintson **a Hely hozzáadása elemre.** Ezzel létrehoz egy új MPN-azonosítót az új helyhez, amelyet a CSP-tranzakciókhoz és -ösztönzőkhez használhat.

:::image type="content" source="images/legal-biz.png" alt-text="Új jogi vállalkozás hozzáadása":::

> [!NOTE]
> Miután hozzáadott egy helyet a Partnerközpont, nem távolíthatja el. Ha a megfelelő **MPN-azonosítót** használta a bejelentkezéshez Partnerközpont az MPN megjelenik a bal oldali menüben.

## <a name="add-the-registration-number-id"></a>A regisztrációs szám azonosítójának hozzáadása

Ha Ön közvetett szolgáltató, közvetlen számlázási partner vagy közvetett viszonteladó, és a következő országokban új vagy meglévő ügyfelekkel üzleti kapcsolatban áll, meg kell adnia a vállalat regisztrációs azonosítószámait. Ha az az ország, ahol a vállalkozása található, nem szerepel az alábbi listában, a regisztrációs azonosító megadása nem kötelező.

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

Egy hely fiókból való törléséhez fel kell vennie a kapcsolatot a [partnertámogatással.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b) Győződjön meg arról, hogy megértette ennek a műveletnek a hatását. Törölt helyek nem olvashatók be, és az adott MPN-azonosítóhoz kötődő adatokat a rendszer nem ismeri fel és nem aktív a vállalatnál.

## <a name="change-country-of-partner-global-account"></a>Partner globális fiókjának országának módosítása 

1. Jelentkezzen be az MPN-fiókkal a Partnerközpont. (Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól) . Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell lennie. 

2. A **Partner lapon** válassza az Üzleti **helyek** lapot, és ellenőrizze a helyek listáját, és ellenőrizze, hogy a jogi személyként kívánt hely szerepel-e a listán. 
 
1. Hely hozzáadásához kattintson **az Add a location**(Hely hozzáadása) elemre, majd a úszó menüben adja meg a szükséges adatokat, beleértve a vállalathoz hozzáadni kívánt hely üzleti nevét, címét és elsődleges kapcsolattartóját. 
 
1. Válassza **az Ország/régió** legördülő lista Melletti Ország **módosítása** lehetőséget, és kövesse a lépéseket. 

:::image type="content" source="images/lbp.png" alt-text="Jogi üzleti profil adatainak úszó panele":::

5. Kattintson a **Mentés** gombra.

6. Az MPN globális fiók országa az új jogi országra változik.
  
## <a name="next-steps"></a>Következő lépések

- Ismerje meg az [ellenőrzési folyamatot.](verification-responses.md)
