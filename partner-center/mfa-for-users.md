---
title: Többtényezős hitelesítés beállítása a saját felhasználókhoz
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Megtudhatja, hogyan állíthatja be alkalmazottait az MFA-val
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cdb83c8b58b75606275c9773cba79eba75d5d0d
ms.sourcegitcommit: 7cc83714e17337b472727819243f98c84ae181ba
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/22/2021
ms.locfileid: "112450805"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Többtényezős hitelesítés beállítása a saját felhasználókhoz

**Megfelelő szerepkörök:** Globális rendszergazda

A nagyobb adatvédelmi védelem és biztonság az egyik legfontosabb prioritásunk. Tudjuk, hogy a legjobb védelem a megelőzés, és hogy csak annyira vagyunk erősek, mint a leggyengébbek. Ezért van szükség arra, hogy az ökoszisztémánkban mindenki cselekedjen, és megfelelő biztonsági védelmi intézkedésekre legyen szükség. Határozottan javasoljuk, hogy minden partner engedélyezze a többtényezős hitelesítést (MFA) a partnerbérlő felhasználói számára. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Többtényezős hitelesítés hozzáadása a felhasználók számára

A feladat végrehajtásához a vállalat globális rendszergazdának kell lennie.

Az MFA engedélyezése a legegyszerűbb a felhasználók számára, amikor hozzáadja őket az Azure AD-bérlőhöz.

1. Jelentkezzen be a [Azure Portal,](https://portal.azure.com) majd a **Felhasználókezelés felületre.**
1. Válassza **a Többtényezős hitelesítés lehetőséget.**
1. Válassza ki az engedélyezni kívánt felhasználót, majd válassza az **Engedélyezés lehetőséget.**

Ez engedélyezi az MFA-t a felhasználó számára. Az Engedélyezve beállítás azt jelenti, hogy a felhasználónak be kell állítania az MFA-ellenőrzést, amikor először jelentkezik be. Ezt követően a bejelentkezés után meg kell adniuk egy kódot, amelyet e-mailben vagy szöveges üzenetben (a beállításuktól függően) biztosítanak.  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Adja meg az ellenőrzés mikéntját.":::

>[!NOTE]
>Kényszerítheti **a felhasználókat** az MFA használatára a fenti lépésekkel, majd a **Kényszerítés lehetőség kiválasztásával.** További információ: [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates)(Felhasználónkénti Azure Multi-Factor Authentication engedélyezése a bejelentkezési események biztonságának érdekében). 

Minden felhasználó a Disabled (Letiltva) **indítást indítja** el. Amikor felhasználónkénti vagy többtényezős Azure Active Directory regisztrál felhasználókat, az állapotuk Engedélyezve **lesz.** Ha az engedélyezett felhasználók bejelentkeznek és befejezik a regisztrációs folyamatot, az állapotuk **Kényszerítve állapotra változik.** 

## <a name="next-steps"></a>Következő lépések

- [Szerepkörök és engedélyek hozzárendelése a felhasználókhoz](permissions-overview.md)