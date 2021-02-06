---
title: Kifizetések és adóprofilok a Partnerközpontban
ms.topic: how-to
ms.date: 11/12/2020
description: Létrehozhatja és kezelheti a kifizetési és az adózási profilt, így Ön fizethet az ösztönzőkért. Ide tartozik a különböző profilok létrehozása, kezelése és használata.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 282fdacc8689ff71e885a2f0ea01ce9570611707
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624238"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Ösztönzők létrehozása és kezelése a partner Centerben


**Megfelelő szerepkörök:**

- Ösztönzők rendszergazdája
- Fiókadminisztrátor
- Globális rendszergazda

Ahhoz, hogy megkaphassa az egy adott MPN-helyhez tartozó ösztönzőprogramok kifizetését, be kell fejeznie a regisztrációt úgy, hogy a programhoz és az MPN-helyhez egy érvényes kifizetési és adóprofilt társít. A Microsoft ezt a kifizetési és adóprofilt a kifizetésekhez fogja használni. Az ösztönzőprogram szabályaitól függően lehetséges elektronikus banki átutalás vagy jóváírási értesítés használata is a kifizetéshez. 

## <a name="roles-currencies-and-other-microsoft-programs"></a>Szerepkörök, pénznemek és egyéb Microsoft-programok

Fontos megérteni az alábbi információkat, mielőtt megkezdi a befizetést és az adózási profilt.

### <a name="roles-and-permissions"></a>Szerepkörök és engedélyek

Az ösztönző befizetések esetén a banki és adózási információk megadásához ösztönző rendszergazdának kell lennie. Ha Ön MPN/fiók rendszergazdája, rendeljen hozzá önmagát és/vagy kollégáját, hogy az ösztönözze a rendszergazdát.

Ha ösztönző rendszergazdai jogosultságokat kell kérnie, forduljon az MPN-rendszergazdához vagy a globális rendszergazdához. A [partner Center irányítópultra](https://partner.microsoft.com/dashboard/)való bejelentkezéssel megállapíthatja, hogy kik a vállalatnál vannak ezek a szerepkörök. Kattintson a jobb felső sarokban található **Beállítások** ikonra, válassza a **felhasználói kezelés** , majd a globális rendszergazda szűrése lehetőséget.

Ösztönzők a felhasználók megtekinthetik az ösztönző bevételeket és a fizetési adatokat és jelentéseket, de nem szerkeszthetik a bank és az adó adatait.

### <a name="choose-your-disbursement-currency"></a>Válassza ki a kifizetés pénznemét

Az ösztönző kifizetések a fizetési profil beállításakor kiválasztott pénznemben történnek. A fizetések kiszámítása a Microsoft által havonta beállított árfolyamon történik. A kiválasztott pénznem miatt az érték változásaiért felelős lesz.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Különböző profilok használata különböző Microsoft-programokhoz

Ha a vállalata több ösztönző programban is regisztrálva van, használhatja ugyanazt a fizetési fiókot, vagy választhat, hogy különböző fizetési fiókokat szeretne használni a különböző programokhoz.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Kifizetési és adózási profilok létrehozása és kezelése a partner Centerben

Az alábbi szakasz végigvezeti a fizetési és adózási profilok a partner Centerben való létrehozásának és kezelésének folyamatán.

>[!IMPORTANT]
>A fizetési profilok a partner Centerben való létrehozásához és kezeléséhez ösztönző rendszergazdának kell lennie. Az ösztönző szerepköröket minden egyes, az egyes ösztönző programok alá tartozó MPN-helyhez hozzá kell rendelni. Az ösztönző rendszergazdák a partner Centerben való hozzáadásával kapcsolatos további információkért lásd: [felhasználói fiókok létrehozása](create-user-accounts-and-set-permissions.md).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>A partner Center kifizetési és adózási szakaszának elérése

1. Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard/) a Azure Active Directory-(Azure ad-) fiókkal (vállalati fiókkal) vagy a megfelelő e-mail-címmel, ha az egyik hozzá lett rendelve.

   - Egy Azure AD-fiókban több tartomány is regisztrálható. Forduljon a globális rendszergazdához, és állapítsa meg, hogy mely tartományok vannak társítva.
   - Ha csak a tartományba tud bejelentkezni @onmicrosoft.com , lépjen kapcsolatba a fiók rendszergazdájával, és adjon hozzá további tartományokat az Azure ad-fiókhoz.
   - Ha a rendszer kéri, hogy válassza a munkahelyi vagy **iskolai fiók** vagy a **személyes fiók** lehetőséget, válassza a **munkahelyi vagy iskolai fiók** lehetőséget.

2. Kattintson a fogaskerék ikonra a **Beállítások** menü megnyitásához, majd válassza a **Fiókbeállítások** lehetőséget.

3. A **Fiókbeállítások** menüben válassza a **kifizetés és az adó** lehetőséget. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Kifizetési és adózási profilok társítása az egyes programokhoz

1. Jelentkezzen be a [partner Center irányítópultra](https://partner.microsoft.com/dashboard/), majd kattintson a fogaskerék ikonra a **Beállítások** menü megnyitásához. 

2. Válassza ki a **Fiókbeállítások** lehetőséget, bontsa ki a **kifizetés és adó szakaszt**, majd válassza a **kifizetés és az adó profil hozzárendelése** lehetőséget. 
   
   Ekkor megjelenik a programok listája. A profil részleteinek megtekintéséhez kattintson a program melletti nyílra. 

3. Az **adó-profil** legördülő menüben válassza ki a kívánt adózási profilt, vagy válassza az új profil létrehozása lehetőséget. Ha új profil létrehozását választja, akkor a megfelelő módon lesz átirányítva.  Válassza a Folytatás lehetőséget az előugró ablakban. Az új adózási profil létrehozásának folyamata alább látható.

4. Válassza a **fizetési mód** lehetőséget.

   - Ha az **elektronikus banki átutalást** fizetési módként választotta, válassza ki a kívánt fizetési profilt, vagy válassza az új profil létrehozása lehetőséget. Ha új profil létrehozását választja, akkor a megfelelő módon lesz átirányítva. Válassza a Folytatás lehetőséget az előugró ablakban. Az új fizetési profil létrehozásának folyamata alább látható.

   - Ha a fizetési mód mezőben a **jóváírási Megjegyzés** lehetőséget választotta, akkor végezze el az ellenőrzést. Ezzel megerősíti, hogy a hivatkozott SAP-szám a szervezethez tartozik.

    >[!NOTE]
    >Ha több Microsoft üzleti entitás van felsorolva, ki kell választania egy fizetési profilt az egyes entitásokhoz.

    >[!NOTE]
    >A fizetési mód rendelkezésre állása az ösztönző program szabályaitól függ.
    
5. Válassza ki a **pénznemet**.

6. Az összes fizetési mező kitöltése után válassza a **Küldés** lehetőséget.

## <a name="create-your-bank-profile"></a>A bank profiljának létrehozása

A banki profilok szervezeti szinten jönnek létre. Ez lehetővé teszi, hogy az egyik bank profilja több MPN-azonosító és egy szervezeten belüli ösztönző program között legyen hozzárendelve. A banki profil különböző országokban való alkalmazása kivételeket okozhat, mivel a különböző banki és adózási szabályok érvényesek.

>[!NOTE]
>A következő lapokon csillaggal rendelkező mezőket kell megadni. Ha nem tudja, mi a mező, válassza ki az információs ikont. 

1. A **részletek** lapon végezze el a következő mezőket: **profilnév:** adjon meg egy egyedi nevet a fizetési profil azonosításához.
    **Bankszámla helye:** Az ország, amelyben a vállalat bankja található.
    **Fizetési mód:** A partner központ előnyben részesített fizetési módja az elektronikus banki átutalás.

2. Kattintson a **Tovább** gombra.

3. A **Bankszámla** lapon adja meg az adatait. Az ezen az oldalon látható mezők országonként eltérőek lesznek. 

4. Kattintson a **Tovább** gombra.

5. A **kedvezményezett** lapon adja meg a megfelelő adatokat. A kedvezményezett az a személy, aki a vállalatnál kapcsolatba fog lépni, ha meg kell vitatnia a fiókját.

6. Ha a mezők befejeződik, válassza a **Befejezés** lehetőséget, majd válassza a **jóváhagyás** lehetőséget a banki profil létrehozásához.

A rendszer átirányítja a **kifizetési és adózási profilok** lapra. Az új profil állapota a **Microsoft-ellenőrzés függőben** állapotba kerül, amíg az ellenőrzés be nem fejeződik. Ez a folyamat akár 48 órát is igénybe vehet. Az érvényesítés befejezését követően a profil állapota vagy **jóváhagyása** vagy a **szükséges művelet** látható lesz. Ha **beavatkozás szükséges**, ismételje meg a fenti lépéseket a szükséges információk megadásakor. 

## <a name="create-your-tax-profile"></a>Az adózási profil létrehozása

A következő eljárással biztosíthatja a Microsoft számára a szervezete számára szükséges adózási adatokat. Az ebben a szakaszban szereplő lapok dinamikusak, és az adott országtól vagy régiótól függően változnak. Ha segítségre van szüksége a helyes adózási információk azonosításához, lépjen kapcsolatba az országa megfelelő kormányzati forrásaival.

Abban az esetben, ha a W8 vagy a W9 űrlap kitöltéséhez szükséges információkra van szüksége a partner vállalatok számára, a következő címek az IRS webhelyre kerülnek:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Csak a vállalat adatait adja meg. Soha ne adjon meg személyes adatokat.

1. Az **üzleti profil** lapon végezze el a szükséges mezőket, majd kattintson a **tovább** gombra. 

2. A **telepítés** lapon válassza ki a vállalatára vonatkozó beállítást.

   - Válassza ki a bal oldali lehetőséget, ha a vállalata csak a Egyesült Államokban van beépítve, vagy ha ez a profil egyedi.
   - Ha a vállalat a Egyesült Államokon kívül van beépítve, válassza a jobb oldali lehetőséget, majd válassza ki az országot/régiót a listából.

3. Kattintson a **Tovább** gombra. 

4. Az **adó állapota** lapon adja meg a szükséges adatokat, majd kattintson a **tovább** gombra. Az ezen a lapon lévő mezők országonként eltérőek lesznek. a részleteket. 

5. A **További dokumentáció** lapon a kötelező mezők és a **tovább** gombra. 

6. Válassza a **Tallózás** lehetőséget az országa vagy régiója számára szükséges dokumentumok feltöltéséhez. Ha megjelenik a dokumentum neve, válassza a **feltöltés** lehetőséget. 

7. Ha el kell távolítania a dokumentumot, válassza az **Eltávolítás** lehetőséget.

8. A mentéshez és a folytatáshoz kattintson a **Befejezés** gombra.

9. Válassza az előugró üzenet **megerősítés** elemét. Visszakerül a **kifizetés és az adó beállítása** lapra.

## <a name="next-steps"></a>Következő lépések

- [A kifizetésekkel és az adókkal kapcsolatos gyakori kérdések](payout-faq.md)
