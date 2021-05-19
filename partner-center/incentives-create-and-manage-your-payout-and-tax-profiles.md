---
title: Kifizetések és adóprofilok a Partnerközpontban
ms.topic: how-to
ms.date: 04/15/2021
description: A kifizetési és adóprofil létrehozása és kezelése, hogy fizetős fizetést kap az ösztönzők munkához. Ide tartozik a különböző profilok létrehozása, kezelése és használata.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: b167b0e65f3339a29f0227f6135ed70931300d8e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152154"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Ösztönzők kifizetési és adóprofiljainak létrehozása és kezelése a Partnerközpont

**Megfelelő szerepkörök:** Ösztönzők rendszergazdai | Fiók-rendszergazdai | Globális rendszergazda

Ahhoz, hogy megkaphassa az egy adott MPN-helyhez tartozó ösztönzőprogramok kifizetését, be kell fejeznie a regisztrációt úgy, hogy a programhoz és az MPN-helyhez egy érvényes kifizetési és adóprofilt társít. A Microsoft ezt a kifizetési és adóprofilt a kifizetésekhez fogja használni. Az ösztönzőprogram szabályaitól függően lehetséges elektronikus banki átutalás vagy jóváírási értesítés használata is a kifizetéshez. 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a>Szerepkörök, pénznemek és több Microsoft-ösztönzőprogram

A kifizetési és adóprofil használatának első lépése előtt fontos, hogy megértse az alábbi információkat.

### <a name="roles-and-permissions"></a>Szerepkörök és engedélyek

Az ösztönzők rendszergazdájának kell lennie ahhoz, hogy bank- és adóinformációkat adjon meg az ösztönző kifizetésekhez. Ha Ön MPN-/fiókrendszergazda, hozzárendelheti saját magát és/vagy egy munkatársát az ösztönzők rendszergazdájának.

Ha ösztönzőrendszergazdai engedélyeket kell kérnie, lépjen kapcsolatba az MPN-rendszergazdával vagy a globális rendszergazdával. A cégen belül ki rendelkezik ezekkel a szerepkörökkel, ha bejelentkezik a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard/) A jobb **felső sarokban** található Beállítások ikonra kattintva válassza a **Felhasználókezelés** lehetőséget, majd szűrjön a Globális rendszergazda elemre.

Ösztönzők A felhasználók megtekinthetik az ösztönző bevételeit, fizetési adatait és jelentéseit, de nem szerkeszthetik a banki és adóadatokat.

### <a name="choose-your-disbursement-currency"></a>A kifizetés pénznemének kiválasztása

Az ösztönzők kifizetése a fizetési profil beállításakor kiválasztott pénznemben történik. A kifizetések kiszámítása a Microsoft által havonta beállított árfolyam alapján történik. Ön lesz a felelős az értékeknek a kiválasztott pénznem miatt történt változásaiért.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Különböző Profilok használata különböző Microsoft-programokhoz

Ha a vállalata több ösztönzőprogramban is regisztrálva van, mindegyikhez használhatja ugyanazt a fizetési fiókot, vagy különböző programokhoz különböző fizetési fiókokat használhat.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Kifizetési és adóprofilok létrehozása és kezelése a Partnerközpont

Az alábbi szakaszok a fizetési és adóprofilok létrehozásának és kezelésének folyamatát ismertetik a Partnerközpont.

>[!IMPORTANT]
>A kifizetési és adóprofilok létrehozásához vagy kezeléséhez ösztönzőrendszergazdának kell lennie a Partnerközpont. Az ösztönzői szerepköröket minden egyes ösztönzőprogramban minden MPN-helyhez hozzá kell rendelni. További információ az ösztönzőrendszergazdák hozzáadásáról a Partnerközpont: [Felhasználói fiókok létrehozása.](create-user-accounts-and-set-permissions.md)

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Hozzáférés a kifizetési és adószakaszhoz a Partnerközpont

1. Jelentkezzen be [az Partnerközpont irányítópultra](https://partner.microsoft.com/dashboard/) a Azure Active Directory-fiókjával (vállalati fiókkal), vagy a megfelelő e-mail-címmel, ha van hozzárendelve.

   - Egy Azure AD-fiókban több tartomány is regisztrálható. Lépjen kapcsolatba a globális rendszergazdával, és állapítsa meg, hogy mely tartományok vannak társítva.
   - Ha csak a tartománnyal tud bejelentkezni, és további tartományokra van szüksége, lépjen kapcsolatba a fiókadminisztrátával, és adjon hozzá további tartományokat az @onmicrosoft.com Azure AD-fiókhoz.
   - Ha a rendszer a  Munkahelyi vagy iskolai fiók vagy a Személyes fiók lehetőséget **kéri,** válassza a Munkahelyi vagy iskolai **fiók lehetőséget.**

2. Kattintson a fogaskerék ikonra a **Beállítások menü megnyitásához,** majd válassza a **Fiókbeállítások lehetőséget.**

3. A **Fiókbeállítások menüben** válassza a **Kifizetés és adó lehetőséget.**

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Kifizetési és adóprofilok hozzárendelése az egyes programokhoz

1. Jelentkezzen be a [Partnerközpont irányítópultjára,](https://partner.microsoft.com/dashboard/)majd válassza a fogaskerék ikont a **Beállítások menü megnyitásához.** 

2. Válassza **a Fiókbeállítások** lehetőséget, bontsa ki a **Kifizetés és adó szakaszt,** majd válassza a **Kifizetési és adóprofil-hozzárendelés lehetőséget.** 
   
   Megjelenik a programok listája. Válassza a program melletti nyilat a profil részleteinek kiválasztásához. 

3. Az **Adóprofil legördülő** menüben válassza ki a kívánt adóprofilt, vagy válassza az új profil létrehozása lehetőséget. Amikor kiválasztja az új profil létrehozása lehetőséget, a rendszer megfelelően átirányítja.  Válassza **a Folytatás** lehetőséget az előugró ablakban. Az új adóprofil létrehozásának folyamatát alább olvashatja.

4. Válassza **a Fizetési mód lehetőséget.**

   - Ha fizetési módként elektronikus **banki** átutalást választott, válassza ki a kívánt fizetési profilt, vagy válassza az Új profil létrehozása lehetőséget. Amikor kiválasztja az új profil létrehozására vonatkozó lehetőséget, a rendszer megfelelő módon átirányítja. Az előugró ablakban válassza a Folytatás lehetőséget. Az új fizetési profil létrehozásának folyamatát alább olvashatja.

   - Ha fizetési módként a **Credit Note** (Jóváírás) beállítást választotta, akkor töltse ki az ellenőrzést. Ez megerősíti, hogy a hivatkozott SAP-szám a szervezethez tartozik.

    >[!NOTE]
    >Ha több Microsoft üzleti entitás is szerepel a listán, mindegyik entitáshoz ki kell választania egy fizetési profilt.

    >[!NOTE]
    >A fizetési mód elérhetősége az ösztönzőprogram szabályaitól függ.

    - Ha a hely MPN-azonosítóját a Microsoft helyi leányvállalata fizeti ki egy adott ösztönzőprogramért, és engedélyezi az LRD (korlátozott kockázat terjesztője) jóváírási emlékeztetőt fizetési módként, akkor a fizetési profilja előre ki lesz töltve az LRD Credit Note fizetési mód használatával. A megfelelő ösztönzőprogramhoz és hely MPN-azonosítóhoz tartozó LRD-kreditjegy  fizetési mód sorában a Megerősítés vagy az Ellenőrzés szükséges állapot látható a fizetési profil szakaszban. 
    
       Válassza **az Ellenőrzés szükséges** lehetőséget a CSP-bérlő azonosítójának a hely MPN-hez és fizetési módhoz társított részleteinek megerősítéséhez és ellenőrzéséhez a jóváírási megjegyzés kifizetésének fogadására. A Jóváírás **részletei párbeszédpanelen** ellenőrizze, hogy a CSP-bérlő azonosítója és a megadott adatok helyesek-e. Ha egynél több bérlőazonosítót kap, gondosan válassza ki azt a CSP-bérlőazonosítót, amelyen kifizetéseket szeretne kapni. Ezután válassza a **Megerősítés** lehetőséget annak megerősítéséhez, hogy a vállalat adatai helyesek, és hogy az ösztönző kifizetését a kiválasztott CSP-bérlőazonosítóra kell fizetni.
 
      Ha a Megerősített állapot **látható,** a CSP-bérlőazonosító hozzárendelése befejeződött, és nincs szükség további műveletre. A hozzárendelés részleteinek megtekintése továbbra is a Megerősített lehetőséget választhatja.
   
      Az olyan országokban, amelyekben a partnereknek explicit módon kell kérelmezni az adómentesség kérelmezését, az ösztönzőprogram és a hely MPN adóprofil szakaszában lehet alkalmazni az adómentességet az adóprofil mellett. Ennek a jelölőnégyzetnek a beírása az ösztönző jóváírási megjegyzésére alkalmazza az adómentességi kedvezményeket. 
   
      Az LRD Credit Note fizetési mód jelenleg csak Ausztrália, Új-Zéland és Kanada partnerei számára érhető el a Microsoft Commerce Incentive programhoz. Ha Ön közvetlen számlázási partner vagy közvetett szolgáltató abban a három országban, amely regisztrálva van az MCI-programban, és nem látja az LRD-kreditek megjegyzését elérhető fizetési módként, ellenőrizze, hogy a bérlőazonosító társítva van-e a megfelelő partner MPN-helyfiókkal. Erről a szervezeti profil frissítésével kapcsolatos további információkért olvassa el a [következőt:](update-your-partner-profile.md).

    
5. Válassza a **Pénznem lehetőséget.**

6. Ha az összes fizetési mezőt kitöltötte, válassza a Küldés **lehetőséget.**

## <a name="set-up-a-default-bank-profile"></a>Alapértelmezett banki profil beállítása

Beállíthatja az alapértelmezett banki profilokat, és hozzárendelheti őket MPN-helyekhez. Ezeket az alapértelmezett profilokat a Microsoft az MPN-hely későbbi regisztrációihoz fogja használni. 

1. Jelentkezzen be a [Partnerközpont irányítópultjára,](https://partner.microsoft.com/dashboard/)majd válassza a fogaskerék ikont a **Beállítások menü megnyitásához.**   

2. Válassza **a Fiókbeállítások** lehetőséget, bontsa ki a **Kifizetés és adó** szakaszt, majd válassza a Kifizetési és **adóprofilok lehetőséget.** 

3. A **Fizetési profilok szakaszban válassza** az Alapértelmezett profilok **kezelése** lehetőséget. 

4. Alapértelmezett banki profil létrehozásához válassza az Alapértelmezett banki **profil hozzáadása lehetőséget.** 

5. Válasszon ki egy banki profilt a vállalata elérhető bankprofiljainak listájából, válassza ki a banki profilhoz használni kívánt pénznemet, majd válassza ki azon MPN-helyek listáját, amelyekre alkalmazni szeretné ezt az alapértelmezett profilt.

6. Miután **végzett** a kijelölésekkel, válassza a Kész lehetőséget. A Kész gomb addig nem kattintható, amíg az összes kötelező mező be nem fejeződött. 

>[!NOTE]
>Ugyanaz a bank- és pénznempár több helyre is alkalmazható. Ha a hely MPN-hez egyszer lett hozzárendelve alapértelmezett profil és pénznem kombináció, az a jövőben nem jelenik meg a hely legördülő menüben a későbbi alapértelmezett profil-hozzárendelések esetén. Ha törli az alapértelmezett kijelölést, a hely MPN újra megjelenik a későbbi alapértelmezett profil-hozzárendelések esetén. A rendszer minden banki profilt és pénznemet egyedi, szerkeszthető sorként ad hozzá.

7. Az összes szükséges módosítás hozzáadása után válassza a **Mentés lehetőséget.**  

## <a name="create-your-bank-profile"></a>A banki profil létrehozása

A banki profilok vállalati szinten vannak létrehozva. Ez lehetővé teszi, hogy egy banki profil több MPN-azonosítóhoz és ösztönzőprogramhoz legyen hozzárendelve a vállalaton belül. Előfordulhatnak kivételek, amikor a banki profilt különböző országokra alkalmazza, mivel különböző banki és adózási szabályok alkalmazhatók.

>[!NOTE]
>A következő oldalakon csillaggal kell megadni a mezőket. Ha nem tudja, mi az a mező, válassza az információs ikont. 

1. A Részletek **lapon töltse** ki a következő mezőket: **Profil neve:** Adjon meg egy egyedi nevet a fizetési profil azonosításához.
    **A bankszámla helye:** Az az ország, ahol a vállalata bankja található.
    **Fizetési mód:** Az előnyben részesített fizetési mód Partnerközpont az elektronikus banki átutalás.

2. Kattintson a **Tovább** gombra.

3. A **Bankfiók lapon** adja meg az adatait. Az ezen az oldalon megjelenő mezők országonként változnak. 

4. Kattintson a **Tovább** gombra.

5. A **Nagyaját lapon** adja meg a megfelelő adatokat. Az a személy a vállalatnál, akivel a bank kapcsolatba lép, ha meg kell vitatni a fiókját.

6. Ha a mezők elkészültek, válassza a  **Befejezés** lehetőséget, majd válassza a Megerősítés lehetőséget a banki profil létrehozásához.

A rendszer átirányítja a Kifizetési **és adóprofilok oldalra.** Az új profil állapota a **Függőben** lévő Microsoft-ellenőrzés állapotot fogja tükrözni, amíg az érvényesítés be nem fejeződik. Ez a folyamat akár 48 órát is igénybe vehet. Az érvényesítés befejezése után a profil  állapota Jóváhagyott vagy **Beavatkozás szükséges** lesz. Ha **beavatkozás szükséges,** ismételje meg a fenti lépéseket a szükséges információk megismétlve. 

## <a name="create-your-tax-profile"></a>Adóprofil létrehozása

Az alábbi eljárással adatokat szolgáltat a Microsoftnak a szervezet számára szükséges adóinformációkról. Az ebben a szakaszban található lapok dinamikusak, és országonként vagy régiónként változnak. Ha segítségre van szüksége a helyes adóinformációk azonosításához, lépjen kapcsolatba az ország megfelelő kormányzati forrásaival.

Az amerikai partnervállalatok esetén, ha információra van szüksége a W8- vagy W9-űrlapok kitöltésével kapcsolatban, az alábbi címek az IRS webhelyére lépnek:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Csak a vállalat adatait adja meg. Soha ne adjon meg személyes adatokat.

1. Az Üzleti **profil lapon** töltse ki a kötelező mezőket, majd válassza a Tovább **lehetőséget.** 

2. A Beállítás **lapon** válassza ki a vállalatára vonatkozó beállítást.

   - Válassza a bal oldali lehetőséget, ha a vállalat csak Egyesült Államok, vagy ha ez a profil egyéni felhasználó számára van be építve.
   - Válassza a jobb oldalon található lehetőséget, ha a vállalata az Egyesült Államok kívül van beépítve, majd válassza ki az országot/régiót a listából.

3. Kattintson a **Tovább** gombra. 

4. Az **Adóállapot lapon** adja meg a szükséges adatokat, majd válassza a Tovább **lehetőséget.** Az oldal mezői országonként változnak. a részleteket. 

5. A További **dokumentáció lapon** adja meg a kötelező mezőket, és válassza a **Tovább lehetőséget.** 

6. Válassza **a Tallózás** lehetőséget az ország vagy régió által kért dokumentumok feltöltéséhez. Amikor megjelenik a dokumentum neve, válassza a Feltöltés **lehetőséget.** 

7. Ha el kell távolítania a dokumentumot, válassza az Eltávolítás **lehetőséget.**

8. A mentéshez és a folytatáshoz válassza a **Befejezés lehetőséget.**

9. Válassza **a Megerősítés** lehetőséget az előugró üzenetben. A rendszer vissza fogja hozni a Kifizetés és adó beállítása **oldalra.**
 
## <a name="update-expired-tax-profiles"></a>Lejárt adóprofilok frissítése

1. Jelentkezzen be a [Partnerközpont irányítópultra,](https://partner.microsoft.com/dashboard/)majd válassza a fogaskerék ikont a **Beállítások menü megnyitásához.**

1. Válassza **a Fiókbeállítások** lehetőséget, bontsa ki a **Kifizetés és adó** szakaszt, majd válassza a Kifizetési és **adóprofil lehetőséget.**

1. Válassza az **Adóprofil lehetőséget.**

1. Ellenőrizze a **Lejárati dátum oszlopot,** és keresse meg a lejárt vagy hamarosan le fog járni adóprofilt.

1. Válassza a **Szerkesztés** elemet.

1. Az adóűrlap szakaszban frissítse az adózási űrlapokat az új adatok megsziva. 

## <a name="next-steps"></a>Következő lépések

- [Kifizetésekkel és adókkal kapcsolatos gyakori kérdések](payout-faq.md)
