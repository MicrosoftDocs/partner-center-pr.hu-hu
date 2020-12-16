---
title: Többtényezős hitelesítés beállítása a saját felhasználókhoz
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Ismerje meg, hogyan állíthatja be az alkalmazottakat MFA-val
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/16/2020
ms.locfileid: "97579977"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Többtényezős hitelesítés beállítása a saját felhasználókhoz

**Megfelelő szerepkörök**

- Globális rendszergazda

A kiemelt prioritások közé tartozik a nagyobb adatvédelmi védelem és biztonság. Tudjuk, hogy a legjobb védelem a megelőzés, és hogy csak olyan erősek vagyunk, mint a leggyengébb kapcsolatunk. Ezért van szükségünk arra, hogy az ökoszisztémánk mindenki számára elérhető legyen, és biztosítsuk a megfelelő biztonsági védelem biztosítását. Javasoljuk, hogy az összes partner számára engedélyezze a többtényezős hitelesítés (MFA) használatát a partner bérlője felhasználói számára. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Multi-Factor Authentication hozzáadása a felhasználók számára

A feladat elvégzéséhez a vállalat globális rendszergazdájának kell lennie.

Az Azure AD-bérlőhöz való hozzáadásakor a legegyszerűbben engedélyezheti az MFA használatát a felhasználók számára.

1. Jelentkezzen be a [Azure Portalba](https://portal.azure.com) , majd lépjen a **felhasználói felügyelet** gombra.
1. Válassza a **többtényezős hitelesítés** lehetőséget.
1. Válassza ki az engedélyezni kívánt felhasználót, majd válassza az **Engedélyezés** lehetőséget.

Ez lehetővé teszi az MFA használatát ehhez a felhasználóhoz. Az Engedélyezve beállítás azt jelenti, hogy a rendszer az első bejelentkezéskor kéri a felhasználót, hogy állítson be MFA-ellenőrzést. Ezt követően a bejelentkezéskor a rendszer arra kéri, hogy adja meg a nekik küldött kódot e-mailben vagy szöveges üzenetben (attól függően, hogy melyiket beállították).  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Az ellenőrzés módjának meghatározása":::

>[!NOTE]
>Az MFA használatára **kényszerítheti** a felhasználókat, hogy a fenti lépéseket követve, a **kikényszerítés** lehetőség választásával. További információért olvassa el a [felhasználónkénti Azure-multi-Factor Authentication engedélyezése a bejelentkezési események biztonságossá tételéhez](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates)című témakört. 

Az összes felhasználó **le van tiltva**. Ha felhasználónkénti Azure-Multi-Factor Authentication regisztrálja a felhasználókat, az állapotuk **engedélyezve** értékre vált. Ha az engedélyezett felhasználók bejelentkeznek, és elvégzik a regisztrációs folyamatot, az állapotuk **kényszerítve** értékűre vált. 

## <a name="next-steps"></a>További lépések

- [Szerepkörök és engedélyek hozzárendelése a felhasználókhoz](permissions-overview.md)

