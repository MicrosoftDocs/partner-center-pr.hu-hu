---
title: Telephelyek kezelése a partneri fiókban
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Ismerje meg, hogyan vehet fel új helyet, és hogyan használják a Location MPN ID-t az ösztönző programok, a CSP-üzleti, az előfizetések és az egyéb tranzakciók során.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005902"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Az MPN-fiók helyeinek kezelése és hely hozzáadása (törlése)


**Megfelelő szerepkörök**

- Globális rendszergazda
- Fiókadminisztrátor

A hely MPN-azonosítója azonosítja a vállalat minden egyes helyét. Az MPN-azonosítót a következő helyen regisztrálhatja az ösztönző programokban: a Cloud Solution Provider (CSP) üzletág és más üzleti tranzakciók. A globális MPN-azonosító a nem tranzakciós tevékenységek, például a támogatási kérelmek esetében használatos.

## <a name="the-following-is-a-typical-scenario"></a>A következő tipikus forgatókönyv:

A contoso az Egyesült királyságbeli partneri globális fiókkal (PGA) rendelkezik. Ez a regisztrált jogi üzleti tevékenység, globális MPN-azonosítója pedig az összes nem tranzakciós üzlet kezelésére szolgál. A contoso az Egyesült Királyság, Franciaország és az Egyesült Államok területén is rendelkezik leányvállalatokkal vagy részlegekkel egyenértékű partneri hellyel (PLA). Az MPN-fiók struktúrájában ezek a PLAsok egyedi Location MPN-azonosítóként jelennek meg. A PLAs a tranzakciós vállalkozások, például a CSP-vagy ösztönző programok esetében használatos. A kifizetések adott helyszínekhez vannak kötve. 

>[!NOTE]
>1-1 kapcsolat van a CSP-bérlő és az MPN-hely azonosítója között.

:::image type="content" source="images/locations/locations1.png" alt-text="MPN-helyszínek szerkezete":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Előfeltételek új fiók hozzáadásához a CSP vállalat számára

Új CSP üzleti fiók hozzáadásához először győződjön meg arról, hogy teljesítette az előfeltételeket.

1. Rendelkeznie kell egy Location MPN-AZONOSÍTÓval abban az országban, ahol a CSP vállalatot szeretné elvégezni. Új MPN-hely létrehozásához olvassa el az alábbi "MPN-hely hozzáadása" című szakaszt.
  
1. Új CSP közvetett viszonteladói regisztrációjának létrehozásához olvassa el a [közvetett szolgáltatók használata](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Ne felejtse el bejelentkezni az **új** CSP-fiók **új** hitelesítő adataival. Ne használja a meglévő hitelesítő adatait, mert a partneri központ már rendelkezik fiókkal.

2. Fogadja el a Microsoft partneri szerződést, és aktiválja a fiókot.

1. Ha közvetlen számlás partnerként szeretne regisztrálni, olvassa el [a közvetlen számlázási partnereinkre vonatkozó követelményeket](direct-partner-new-requirements.md)

## <a name="view-your-mpn-locations"></a>MPN-hely megtekintése

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/home) az MPN-fiókja hitelesítő adataival. (Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól) 
 
1. A **Beállítások** ikonban válassza a **Fiókbeállítások**, **szervezeti profil**, **jogi** lehetőséget. 

1. A **partner** lapon ellenőrizze, hogy nincs-e szalagcím-hibaüzenet, amely arra kéri, hogy javítsa az áttelepített helyet a PMC-ból. Ha van, kövesse az utasításokat, és javítsa ki ezeket a helyszíneket. 

3. Ha nem jelenik meg hibaüzenet, a  **Beállítások** területen válassza a  **Fiókbeállítások**, **szervezeti profil**, **azonosítók** lehetőséget.

4. Keresse meg a "location" típusú MPN-azonosítót, amely megfelel a CSP-fiók országának, és használja az alábbi kereséshez és a társítás befejezéséhez.

5. Ha nem találja a használni kívánt CSP-fióknak megfelelő Location MPN-azonosítót, új helyet is hozzáadhat, amely új MPN-azonosítót hoz létre. Lásd: **MPN-hely hozzáadása** alább.

## <a name="add-an-mpn-location"></a>MPN-hely hozzáadása

1. Jelentkezzen be az MPN-fiókkal a partner Centerben. (Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól). Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell rendelkeznie. 

1. A **Beállítások ikonban** válassza ki a **Fiókbeállítások** elemet, majd válassza a **szervezeti profil** lehetőséget.

2. Válassza a **jogi** lehetőséget, majd a **partner** lapon válassza az **üzleti helyek lehetőséget,** majd kattintson a **hely hozzáadása** lehetőségre.

3. Adja meg a szükséges adatokat, beleértve az üzleti nevet, a lakcímet és a kapcsolattartót a vállalatához hozzáadni kívánt helyhez.
 
1. Kattintson a **hely hozzáadása** gombra. Ekkor létrejön egy új MPN-azonosító az új helyhez, amelyet a CSP-tranzakciókhoz és-ösztönzőkhöz használhat.

:::image type="content" source="images/legal-biz.png" alt-text="Új jogi üzleti tevékenység hozzáadása":::

> [!NOTE]
> Miután hozzáadta a helyet a partner Centerben, nem távolíthatja el. Ha a megfelelő MPN-azonosítót használta a bejelentkezéshez, az **MPN** a partner Center bal oldali menüjében jelenik meg.

## <a name="delete-a-location"></a>Hely törlése

Ha törölni szeretne egy helyet a fiókjából, kapcsolatba kell lépnie a [partner támogatási szolgálatával](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b). Győződjön meg arról, hogy tisztában van a művelet hatásával. A törölt helyeket nem lehet beolvasni, és az adott MPN-azonosítóhoz kapcsolódó minden adat már nem ismerhető fel, vagy nem lesz aktív a vállalatnál.

## <a name="change-country-of-partner-global-account"></a>Partner globális fiók országának módosítása 

1. Jelentkezzen be az MPN-fiókkal a partner Centerben. (Az MPN hitelesítő adatai eltérőek lehetnek a CSP hitelesítő adataitól). Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell rendelkeznie. 

2. A **partner** lapon lépjen az **üzleti helyek** elemre, és ellenőrizze a helyek listáját, és győződjön meg arról, hogy az Ön által használt hely szerepel a jogi személy listáján. 
 
1. Hely hozzáadásához kattintson a **hely hozzáadása** lehetőségre, és a kilépéskor adja meg a szükséges adatokat, beleértve az üzleti nevét, a lakcímét és az elsődleges kapcsolattartót a vállalatához hozzáadni kívánt helyhez. 
 
1. Válassza az ország **/régió** legördülő lista melletti **ország módosítása** lehetőséget, és kövesse a lépéseket. 

:::image type="content" source="images/lbp.png" alt-text="Jogi üzleti profilra vonatkozó adatvesztés":::

5. Kattintson a **Mentés** gombra.

6. Az MPN globális fiók országa az új jogi országra lesz módosítva.
  
## <a name="next-steps"></a>Következő lépések

- További információ az [ellenőrzési folyamatról](verification-responses.md).
