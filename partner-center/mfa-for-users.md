---
title: Többtényezős hitelesítés beállítása a saját felhasználókhoz
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Ismerje meg, hogyan állíthatja be alkalmazottait az MFA-val
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 37373c032dc34315c0e3274987805d7518d0b595
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276603"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Többtényezős hitelesítés beállítása a saját felhasználókhoz

**Megfelelő szerepkörök:** Globális rendszergazda

A nagyobb adatvédelmi védelem és biztonság az egyik legfontosabb prioritásunk. Tudjuk, hogy a legjobb védelem a megelőzés, és hogy csak annyira vagyunk erősek, mint a leggyengébbek. Ezért van szükség arra, hogy az ökoszisztémánkban mindenki cselekedjen, és gondoskodik a megfelelő biztonsági védelemről. Határozottan javasoljuk, hogy minden partner engedélyezze a többtényezős hitelesítést (MFA) a partnerbérlő felhasználói számára. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Többtényezős hitelesítés hozzáadása a felhasználók számára

A feladat végrehajtásához a vállalat globális rendszergazdának kell lennie.

Az MFA engedélyezése a legegyszerűbb a felhasználók számára, amikor hozzáadja őket az Azure AD-bérlőhöz.

1. Jelentkezzen be a [Azure Portal,](https://portal.azure.com) majd válassza a **Felhasználókezelés et.**
1. Válassza **a Többtényezős hitelesítés lehetőséget.**
1. Válassza ki az engedélyezni kívánt felhasználót, majd válassza az **Engedélyezés lehetőséget.**

Ez engedélyezi az MFA-t a felhasználó számára. Az engedélyezve azt jelenti, hogy a felhasználónak be kell állítania az MFA-ellenőrzést az első bejelentkező alkalommal. Ezt követően a bejelentkezés után meg kell adniuk egy kódot, amelyet e-mailben vagy szöveges üzenetben (attól függően, hogy melyiket beállította).  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Adja meg az ellenőrzés mikéntját.":::

>[!NOTE]
>Kényszerítheti **a felhasználókat** az MFA használatára a fentiekben leírt lépésekkel, majd a **Kényszerítés lehetőség kiválasztásával.** További információ: [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates)(Felhasználónkénti Azure Multi-Factor Authentication engedélyezése a bejelentkezési események biztonságának érdekében). 

Minden felhasználó a Disabled (Letiltva) **indítást indítja** el. Amikor felhasználónkénti vagy többtényezős Azure Active Directory regisztrál felhasználókat, az állapotuk **Engedélyezve lesz.** Ha engedélyezve van a felhasználók bejelentkezése és a regisztrációs folyamat befejezése, az állapotuk **Kényszerítve állapotra változik.** 

## <a name="next-steps"></a>Következő lépések

- [Szerepkörök és engedélyek hozzárendelése a felhasználókhoz](permissions-overview.md)