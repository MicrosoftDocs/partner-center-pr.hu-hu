---
title: Nem lehet bejelentkezni a partner központba
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Hárítsa el a lehetséges okokat, és Ismerje meg a megoldásait, ha nem tud bejelentkezni a partner Centerbe – további információ a jelszavak alaphelyzetbe állításáról, a szerepkörök ellenőrzéséről és a hitelesítő adatok ellenőrzéséről
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266571"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>A partner Center bejelentkezési problémáinak elhárítása

**Megfelelő szerepkörök**

- A partner Centerben érdekelt összes partner

Ez a cikk a partneri központ gyakori bejelentkezési problémáinak megoldásait tartalmazza.

## <a name="youve-forgotten-your-password-for-partner-center"></a>Elfelejtette a partner központ jelszavát

Ha elfelejtette a jelszavát, és nem tud bejelentkezni a partneri központba, forduljon az ügyfélszolgálathoz. Keresse meg a megfelelő kapcsolatot az [üzleti termékek támogatásához](/microsoft-365/admin/contact-support-for-business-products).

Ha MPN-partner, kérje meg a globális rendszergazdát, hogy hozzon létre egy új jelszót. Ha a CSP közvetett viszonteladó, kérje meg a közvetett szolgáltatót, hogy hozzon létre egy új globális rendszergazdát az Azure AD-bérlőn, vagy hozzon létre egy új jelszót a meghatalmazott rendszergazdai jogosultságok használatával.

Ha többet szeretne megtudni arról, hogy miként állíthatja vissza a jelszavát, és hogyan érheti el a munkahelyi fiókjához való hozzáférést, olvassa el [a munkahelyi vagy iskolai jelszó alaphelyzetbe állítása biztonsági adatok használatával](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)című témakört.

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>A partner Centerben nem tekintheti meg és nem kezelheti a várt oldalakat és képességeket

A partner Centerben lévő lapok elérését a hozzárendelt szerepkörök vezérlik. A hozzárendelt szerepkörök megtekintéséhez a partner Centerben válassza a beállítások ikont, válassza a **Fiókbeállítások** lehetőséget, majd a Fiókbeállítások területen válassza a **felhasználói kezelés** lehetőséget. A Search (keresés) mezőbe írja be a nevét, majd tekintse meg az eredményeket.

Ha nem tudja megtekinteni vagy kezelni a felszámított kompetenciákat, ügyfeleket, ösztönzőket vagy felhasználókat, próbálkozzon a következő megoldásokkal:

- Az MPN, CSP és Referral képességeinek eléréséhez forduljon a globális rendszergazdához vagy a fiók rendszergazdájához. Ha többet szeretne megtudni a szerepkörökről és az általuk engedélyezett feladatokról a partner Centerben, tekintse meg a [szerepkörök & a felhasználók számára](permissions-overview.md)című témakört.
- A kereskedelmi piactér és a Windows & Xbox, az Office áruház, a Microsoft Edge és a hardveres fejlesztői programok képességeinek eléréséhez vegye fel a kapcsolatot a szervezet tulajdonosi vagy felettesi szerepkörével. További információ a szerepkörökről és az engedélyekről: [kereskedelmi Piactéri fiók kezelése a Microsoft partner Centerben](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Nem tekintheti meg az ajánlatát vagy előnyeit a partner Centerben

Győződjön meg arról, hogy a megfelelő hitelesítő adatokat használja a bejelentkezéshez. Előfordulhat például, hogy a munkahelyi és a személyes fiókok ugyanúgy néznek ki (például abc@contoso.com :), de lehet, hogy egy személyes fiók, amelyet Ön hozott létre, és egy másik, az Ön nevében létrehozott üzleti fiók is. Ebben az esetben, ha bejelentkezett, de nem tudja megtekinteni az MPN-vel, a CSP-vel, a kereskedelmi Piactérsel kapcsolatos várt képességeket, próbálja meg kiválasztani a munkahelyi fiókját.

## <a name="next-steps"></a>Következő lépések

- [Fiókadatok ellenőrzése](verification-responses.md)
- [Saját jelszó visszaállítása](reset-my-pasword.md)
- [Új felhasználói jelszó beállítása](reset-a-user-password.md)