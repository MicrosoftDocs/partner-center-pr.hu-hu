---
title: Telephelyek kezelése a partneri fiókban
ms.topic: how-to
ms.date: 11/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Ismerje meg, hogyan vehet fel új helyet, és hogyan használják a Location MPN ID-t az ösztönző programok, a CSP-üzleti, az előfizetések és az egyéb tranzakciók során.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 03c4fb5a4adeb49602fe3736971e140ac6da6f4f
ms.sourcegitcommit: 245b4792e8221468f781f6effd1c9b23be05499a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/24/2020
ms.locfileid: "95514799"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Az MPN-fiók helyeinek kezelése és új hely hozzáadása

**A következőre érvényes:**

- Partnerközpont

**Megfelelő szerepkörök**

- Globális rendszergazda
- Fiókadminisztrátor

A hely MPN-azonosítója azonosítja a vállalat minden egyes helyét. Az MPN-azonosítót a következő helyen regisztrálhatja az ösztönző programokban: a Cloud Solution Provider (CSP) üzletág és más üzleti tranzakciók. A globális MPN-azonosító a nem tranzakciós tevékenységek, például a támogatási kérelmek esetében használatos.

## <a name="the-following-is-a-typical-scenario"></a>A következő tipikus forgatókönyv:

A contoso az Egyesült királyságbeli partneri globális fiókkal (PGA) rendelkezik. Ez a regisztrált jogi üzleti tevékenység, globális MPN-azonosítója pedig az összes nem tranzakciós üzlet kezelésére szolgál. A contoso az Egyesült Királyság, Franciaország és az Egyesült Államok területén is rendelkezik leányvállalatokkal vagy részlegekkel egyenértékű partneri hellyel (PLA). Az MPN-fiók struktúrájában ezek a PLAsok egyedi Location MPN-azonosítóként jelennek meg. A PLAs a tranzakciós vállalkozások, például a CSP-vagy ösztönző programok esetében használatos. A kifizetések adott helyszínekhez vannak kötve. 

>[!NOTE]
>1-1 kapcsolat van a CSP-bérlő és az MPN-hely azonosítója között.

:::image type="content" source="images/locations/locations1.png" alt-text="MPN-helyszínek szerkezete":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>Előfeltételek egy új hely megadásához a CSP vállalat számára

Új CSP üzleti hely hozzáadásához több előfeltétel van:

1. Rendelkeznie kell egy Location MPN-AZONOSÍTÓval abban az országban, ahol üzleti tevékenységet kíván végezni.

1. Szüksége lesz egy új Azure AD-bérlőre a [vállalati régióban](regional-authorization-overview.md) , amely még nincs regisztrálva a CSP-ben. Hozza létre ezt a tanúsítványt a CSP-ben való regisztráláskor.
 
3. Az új HRE-bérlő használatával regisztráljon a CSP programba a régióban.
Jogi cég adatainak megadása, beleértve a jogi cég nevét, a lakcímét, az elsődleges kapcsolattartási adatokat. Ez a fiók ellenőrzés alá kerül, ezért mindenképpen adjon meg érvényes információt.

>[!NOTE] 
 >Ne felejtse el bejelentkezni az **új** Azure ad-bérlő **új** hitelesítő adataival. Ne használja a meglévő hitelesítő adatait, mert a partneri központ már rendelkezik fiókkal.

4. Fogadja el a Microsoft partneri szerződést, és aktiválja a fiókot.

## <a name="add-an-mpn-location"></a>MPN-hely hozzáadása

1. Jelentkezzen be az MPN-fiókkal a partner Centerben. Az MPN-fióknak globális rendszergazdai vagy fiók-rendszergazdai jogosultságokkal kell rendelkeznie. 

1. A **beállítás ikonban** válassza ki a **szervezet beállításait**.

2. Válassza a **jogi** lehetőséget, majd válassza a **helyszínek lehetőséget.**

3. Válassza a **hely hozzáadása** lehetőséget, és szúrja be a vállalathoz hozzáadni kívánt hely, valamint a helyhez tartozó elsődleges kapcsolattartó címe adatait.

> [!NOTE]
> Miután hozzáadta a helyet a partner Centerben, nem távolítható el. Ha a megfelelő MPN-azonosítót használta a bejelentkezéshez, az **MPN** a partner Center bal oldali menüjében jelenik meg.

## <a name="change-global-partner-account-location"></a>Globális partneri fiók helyének módosítása

1. Az **[üzleti helyszíneken](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** tekintse meg a helyek listáját, és győződjön meg arról, hogy a kívánt hely szerepel a jogi személy listáján. Ha nem, adja hozzá.

   :::image type="content" source="images/accountsettings/location1.png" alt-text="A partner Center-fiókok helyei lap képernyőképe az összes aktuális hely listájáról.":::

2. Válassza a **jogi** lehetőséget, majd válassza a **jogi üzleti profil frissítése** elemet.
  
3. Válassza ki a régiót és a jogi személyt, és **küldje** el.

  
## <a name="next-steps"></a>Következő lépések

- További információ az [ellenőrzési folyamatról](verification-responses.md).
