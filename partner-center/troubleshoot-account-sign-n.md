---
title: A fiók vagy az MPN-Partnerközpont beállításával kapcsolatos hibák elhárítása
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: A regisztrálással kapcsolatos problémák elhárítása a Partnerközpont. Választ ad a fizetési módok kihívásaira, a jelszavakkal való elsiklott jelszavakra és egyéb problémákra.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431755"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>A fiók beállításával vagy az MPN megújításával kapcsolatos problémák elhárítása

**Megfelelő szerepkörök:** Globális rendszergazdai | MPN-partneri rendszergazda
 
Íme néhány javaslat a fiók beállításakor felmerülő gyakori problémák Partnerközpont elhárításához.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Mi történik, ha a vállalati Partner Membership Center, és nem szerkeszti a céges adatokat mezőit?

Olyan esetekben, amikor a vállalat már jelen van a Partnerközpont-ban (például egy Felhőszolgáltató-fiók (CSP-fiók) – egy csak olvasható képernyő jelenik meg. Ezen a képernyőn a cég összes adata megjelenik, ahogyan az a Partnerközpont.

Ezen a képernyőn nem módosíthatja a részleteket. Ez a tervezéstől és nem a hibától áll.

A folytatáshoz válassza az **Elfogadás,** majd a Folytatás **lehetőséget.**


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Ha az it-részleg kikapcsolta **a Regisztráció** Partnerközpont

Ez az üzenet azért jelenik meg, mert a felhasználók letiltották a regisztrációt, vagy mert a regisztráció le van tiltva a Azure Active Directory (AD) bérlőn. Az Azure AD-fiók globális rendszergazdája a következő PowerShell-parancs futtatásával engedélyezheti a szükséges funkciókat:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

További információ: [Önkiszolgáló regisztráció.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Elfelejtette a jelszavát

Ha elfelejtette a jelszavát, a bejelentkezési oldalon válassza a Nem lehet hozzáférni a **fiókjához?** lehetőséget. Ezzel a beállítással alaphelyzetbe állíthatja a jelszavát, vagy megkérheti a globális rendszergazdát, hogy rendeljen hozzá új hitelesítő adatokat.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Az "Mondja el a cégét" képernyőn "Hiba történt" hibaüzenet jelenik meg

Ez a hibaüzenet általában akkor jelenik meg, ha véletlenül speciális karaktereket, szóközöket vagy országkódot használ a vállalati telefonszámban. A Telefonszám mezőben megadott érték legfeljebb 10 karaktert tartalmazhat.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>A hitelkártya-vásárláskor a következő hibaüzenet jelenik meg: "A rendelést elutasította a rendszer. Kérjük, ellenőrizze az adatait"


A jogi személy helyett mindig a hitelkártyája címének megfelelő címet használja. Győződjön meg arról is, hogy az irányítószám helyes, és megfelel a használt címnek.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Szeretne váltani az offline fizetésről az online fizetési módra 

Le kell mondania az eredeti rendelést, és újra kell azt használnia az előnyben részesített fizetési mód használatával.

Rendelés visszavonása:

1. A Partnerközpont válassza a **Tagsági ajánlatok** lapot.

2. Válassza a **Rendelés visszavonása lehetőséget**

3. Megjelenik egy megerősítési ablak, és meg kell erősítenie a kezdeti rendelés lemondását.

## <a name="next-steps"></a>Következő lépések

- [Partnerközponti fiók kezelése](partner-center-account-setup.md)
- [A számla és a felderítési fájl olvasása](read-your-bill.md)
