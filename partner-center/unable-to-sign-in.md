---
title: Nem lehet bejelentkezni a Partnerközpont
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Elháríthatja a lehetséges okokat, és megismerheti a megoldásokat, amikor nem tud bejelentkezni a Partnerközpont – további információ a jelszavak alaphelyzetbe állításáról, a szerepkörök ellenőrzésről és a hitelesítő adatok ellenőrzésről.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f4af8c48e2bbe65f58549b542447c80b699332be
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818796"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Bejelentkezési problémák elhárítása Partnerközpont

**Megfelelő szerepkörök:** Minden partner, aki érdeklődik a Partnerközpont

Ez a cikk a bejelentkezések gyakori bejelentkezési problémáinak megoldásait Partnerközpont.

## <a name="youve-forgotten-your-password-for-partner-center"></a>Elfelejtette a jelszó Partnerközpont

Ha elfelejtette a jelszavát, és nem tud bejelentkezni a Partnerközpont, forduljon az ügyfélszolgálathoz. Keresse meg a megfelelő kapcsolattartót [a Támogatási üzleti termékeknél.](/microsoft-365/admin/contact-support-for-business-products)

Ha Ön MPN-partner, kérje meg globális rendszergazdáját, hogy hozzon létre egy új jelszót. Ha Ön közvetett CSP-viszonteladó, kérje meg közvetett szolgáltatóját, hogy hozzon létre egy új globális rendszergazdát az Azure AD-bérlőn, vagy hozzon létre egy új jelszót az Ön számára a delegált rendszergazdai jogosultságai használatával.

A jelszó visszaállításáról és a munkahelyi fiókhoz való hozzáférés visszaszerzésével kapcsolatos további információkért olvassa el a Következőt: Munkahelyi vagy iskolai jelszó visszaállítása [biztonsági adatok használatával.](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>Nem tudja megtekinteni vagy kezelni a várt oldalakat vagy képességeket a Partnerközpont

A hozzáférés a Partnerközpont a hozzárendelt szerepkörök vezérlik. A hozzárendelt szerepkörök ellenőrzéséhez válassza Partnerközpont beállítások ikont, válassza a Fiókbeállítások lehetőséget, majd a Fiókbeállítások között válassza a **Felhasználókezelés lehetőséget.** A Keresés mezőbe írja be a nevét, majd tekintse meg az eredményeket.

Ha nem tudja megtekinteni vagy kezelni a várt kompetenciákat, ügyfeleket, ösztönzőket vagy felhasználókat, próbálkozzon a következő megoldásokkal:

- Az MPN, a CSP és a hivatkozások képességeihez való hozzáféréshez forduljon a globális rendszergazdához vagy a fiókadminisztrához. További információ a szerepkörökről és az Partnerközpont által a szerepkörök hozzárendelése & [felhasználókhoz.](permissions-overview.md)
- A kereskedelmi piactér és a Windows & Xbox, az Office Store, a Microsoft Edge és a Hardverfejlesztői programok funkcióihoz való hozzáféréshez lépjen kapcsolatba a szervezet Tulajdonos vagy Vezető szerepkörével. További információ a szerepkörökről és engedélyekről: Kereskedelmi piactéri fiók [kezelése a Microsoft Partnerközpont.](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Az ajánlat vagy az előnyök nem látszanának a Partnerközpont

Győződjön meg arról, hogy a megfelelő hitelesítő adatokat használja a bejelentkezéshez. Előfordulhat például, hogy a munkahelyi és a személyes fiókjai ugyanúgy néznek ki (például ), de az egyik lehet egy Ön által létrehozott személyes fiók, egy másik pedig az Ön nevében beállított üzleti abc@contoso.com fiók. Ebben az esetben, ha bejelentkezett, de nem tudja megtekinteni az MPN-hez, a CSP-hez és a kereskedelmi piactérhez kapcsolódó várt képességeket, próbálja meg kiválasztani a munkahelyi fiókját.

## <a name="next-steps"></a>Következő lépések

- [Fiókadatok ellenőrzése](verification-responses.md)
- [Saját jelszó visszaállítása](reset-my-pasword.md)
- [Új felhasználói jelszó beállítása](reset-a-user-password.md)