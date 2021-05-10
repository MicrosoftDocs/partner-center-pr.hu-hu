---
title: A fiók vagy az MPN-Partnerközpont beállításával kapcsolatos hibák elhárítása
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: A regisztrálással kapcsolatos problémák elhárítása a Partnerközpont. A válaszok számos más kérdésre is választ adnak a fizetési módok, a jelszavakkal való elfelejtés és egyéb problémák esetén.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686262"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>A fiók beállításával vagy az MPN megújításával kapcsolatos problémák elhárítása


**Megfelelő szerepkörök**

- Globális rendszergazda
- MPN-partneri rendszergazda
 
Íme néhány javaslat a fiók beállításakor felmerülő gyakori problémák Partnerközpont elhárításához.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Mi történik, ha a vállalati Partner Membership Center, és nem szerkeszti a céges adatokat mezőit?

Olyan esetekben, amikor a vállalat már jelen van a Partnerközpont (például CSP-fiók) – egy csak olvasható képernyő jelenik meg. Ezen a képernyőn a cég összes adata megjelenik, ahogyan az a Partnerközpont.

Ezen a képernyőn nem módosíthatja a részleteket. Ez a tervezéstől és nem a hibától áll.

A **folytatáshoz válassza az Elfogadás** és a **Folytatás** lehetőséget.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Ha az it-részleg kikapcsolta **a Regisztráció** Partnerközpont

Ez az üzenet azért jelenik meg, mert a virtuális felhasználók le vannak tiltva, vagy mert a regisztráció le van tiltva az Azure AD-bérlőn. Az Azure AD-fiók globális rendszergazdája a következő PowerShell-parancs futtatásával engedélyezheti a szükséges funkciókat:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

További információ: [Önkiszolgáló regisztráció.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Elfelejtette a jelszavát

Ha elfelejtette a jelszavát, válassza a Nem tudja elérni a **fiókját?** hivatkozást a bejelentkezési oldalon. Ezzel a lehetőséggel új jelszót kérhet, vagy megkérheti a globális rendszergazdát, hogy rendeljen hozzá új hitelesítő adatokat.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Az "Mondja el a cégét" képernyőn "Hiba történt" hibaüzenet jelenik meg

Ez a hibaüzenet általában akkor jelenik meg, ha véletlenül speciális karaktereket, szóközöket vagy országkódot használ a vállalati telefonszámban. A Telefonszám mezőben megadott érték legfeljebb 10 karaktert tartalmazhat.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>A hitelkártya-vásárláshoz a következő hibaüzenet jelenik meg: "A rendelést elutasította a rendszer. Kérjük, ellenőrizze az adatait"


Mindig a hitelkártyához tartozó címet használja a jogi személy helyett. Győződjön meg arról is, hogy az irányítószám helyes, és megfelel a használt címnek.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Váltani szeretne az offline fizetésről az online fizetési módra 

Le kell mondania az eredeti rendelést, és újra kell azt használnia az előnyben részesített fizetési mód használatával.

Rendelés visszavonása:

1. Válassza **a Tagsági ajánlatok** lapot az irányítópulton.

2. Válassza a **Rendelés visszavonása lehetőséget**

3. Megjelenik egy megerősítési ablak, és meg kell erősítenie a kezdeti rendelés lemondását.

## <a name="next-steps"></a>Következő lépések

- [Partnerközponti fiók kezelése](partner-center-account-setup.md)
- [A számla és a felderítési fájl olvasása](read-your-bill.md)
