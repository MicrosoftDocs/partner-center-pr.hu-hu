---
title: A partner Center-fiók vagy az MPN megújítási problémáinak beállításával kapcsolatos hibák elhárítása
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: A partner Centerbe való regisztráció során felmerülő problémák elhárítása. Válaszok a fizetési módokkal, a Felejtési jelszavakkal és egyebekkel kapcsolatos problémákra.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d80651c4e5e4afb476dada388f23c118e0bdf25
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768703"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>A Fiókbeállítások vagy az MPN megújítási problémáinak elhárítása


**Megfelelő szerepkörök**

- Globális rendszergazda
- MPN-partner rendszergazdája 
 
Íme néhány javaslat a partner Center-fiók beállításakor felmerülő gyakori problémák elhárításához.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Mi történik, ha a Partner tagsági központjából telepít át, és nem szerkesztheti a vállalati adatok mezőit

Azokban az esetekben, amikor a vállalata már rendelkezik jelenléttel a partner Centerben (például egy CSP-fiók), csak olvasható képernyő jelenik meg. Ezen a képernyőn jelennek meg a vállalatra vonatkozó összes információ a partner Centerben.

Ezen a képernyőn nem módosítható a részletek. Ez a kialakítás és nem egy hiba.

Válassza az **elfogadás** lehetőséget, és folytassa a **folytatást** .


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Ha az informatikai részleg kikapcsolta a **partner Centerre való regisztrációt**

Ez az üzenet jelenik meg, mert a vírusos felhasználók le vannak tiltva, vagy mert a vírusos regisztráció le van tiltva az Azure AD-bérlőn. Az Azure AD-fiók globális rendszergazdája a következő PowerShell-parancs futtatásával engedélyezheti a szükséges szolgáltatásokat:

**Set-Msolcompanysettings parancsmagjával-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

További tudnivalókért olvassa el az [önkiszolgáló regisztrációt](/azure/active-directory/users-groups-roles/directory-self-service-signup)ismertető témakört.

## <a name="you-forgot-your-password"></a>Elfelejtette a jelszavát

Ha elfelejtette a jelszavát, jelölje be a **nem érhető el a fiókja?** hivatkozásra a bejelentkezési oldalon. Ezzel a beállítással visszaállíthatja a jelszavát, vagy megkérheti a globális rendszergazdát, hogy rendeljen új hitelesítő adatokat.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>A "tudnivalók a vállalatról" képernyőn "hiba történt" hibaüzenet jelenik meg

Ez a hibaüzenet általában akkor jelenik meg, ha a céges telefonszámon véletlenül speciális karaktereket, szóközöket vagy országkódot használ. A telefonszám mezőben megadott érték legfeljebb 10 karakterből állhat.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>A bankkártya vásárlása egy hibaüzenetet kap arról, hogy "a megrendelés elutasítása megtörtént. Kérjük, ellenőrizze az adatait "


A jogi személy helyett mindig a hitelkártyájának megfelelő címeket használja. Győződjön meg arról is, hogy a zip-kód helyes, és megfelel a használt címnek.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Offline fizetésről online fizetési módra szeretne váltani 

Az előnyben részesített fizetési mód használatával meg kell szakítania az eredeti rendelést, és újra kell vásárolnia azt.

Megrendelés megszakítása:

1. Válassza a **tagsági ajánlatok** fület az irányítópulton.

2. **Megszakított megrendelés** kiválasztása

3. Ekkor megjelenik egy megerősítési ablak, és meg kell erősítenie a kezdeti sorrend megszakításához.

## <a name="next-steps"></a>Következő lépések

- [Partnerközponti fiók kezelése](partner-center-account-setup.md)
- [A Bill és a Recon-fájl beolvasása](read-your-bill.md)
