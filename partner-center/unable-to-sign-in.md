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
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a><span data-ttu-id="a3171-103">A partner Center bejelentkezési problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="a3171-103">Troubleshoot sign-in issues for Partner Center</span></span>

<span data-ttu-id="a3171-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="a3171-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a3171-105">A partner Centerben érdekelt összes partner</span><span class="sxs-lookup"><span data-stu-id="a3171-105">All partners interested in Partner Center</span></span>

<span data-ttu-id="a3171-106">Ez a cikk a partneri központ gyakori bejelentkezési problémáinak megoldásait tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="a3171-106">This article contains solutions for common sign-in issues for Partner Center.</span></span>

## <a name="youve-forgotten-your-password-for-partner-center"></a><span data-ttu-id="a3171-107">Elfelejtette a partner központ jelszavát</span><span class="sxs-lookup"><span data-stu-id="a3171-107">You've forgotten your password for Partner Center</span></span>

<span data-ttu-id="a3171-108">Ha elfelejtette a jelszavát, és nem tud bejelentkezni a partneri központba, forduljon az ügyfélszolgálathoz.</span><span class="sxs-lookup"><span data-stu-id="a3171-108">If you have forgotten your password and can't sign into Partner Center, contact Support.</span></span> <span data-ttu-id="a3171-109">Keresse meg a megfelelő kapcsolatot az [üzleti termékek támogatásához](/microsoft-365/admin/contact-support-for-business-products).</span><span class="sxs-lookup"><span data-stu-id="a3171-109">Find the appropriate contact at [Support for Business Products](/microsoft-365/admin/contact-support-for-business-products).</span></span>

<span data-ttu-id="a3171-110">Ha MPN-partner, kérje meg a globális rendszergazdát, hogy hozzon létre egy új jelszót.</span><span class="sxs-lookup"><span data-stu-id="a3171-110">If you're an MPN partner, ask your Global admin to create a new password for you.</span></span> <span data-ttu-id="a3171-111">Ha a CSP közvetett viszonteladó, kérje meg a közvetett szolgáltatót, hogy hozzon létre egy új globális rendszergazdát az Azure AD-bérlőn, vagy hozzon létre egy új jelszót a meghatalmazott rendszergazdai jogosultságok használatával.</span><span class="sxs-lookup"><span data-stu-id="a3171-111">If you're a CSP Indirect reseller, ask your Indirect provider to create a new Global admin for you on your Azure AD tenant or create a new password for you using their delegated admin privileges.</span></span>

<span data-ttu-id="a3171-112">Ha többet szeretne megtudni arról, hogy miként állíthatja vissza a jelszavát, és hogyan érheti el a munkahelyi fiókjához való hozzáférést, olvassa el [a munkahelyi vagy iskolai jelszó alaphelyzetbe állítása biztonsági adatok használatával](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)című témakört.</span><span class="sxs-lookup"><span data-stu-id="a3171-112">To learn more about how you can reset your password and regain access to your work account, read [Reset your work or school password using security info](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).</span></span>

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a><span data-ttu-id="a3171-113">A partner Centerben nem tekintheti meg és nem kezelheti a várt oldalakat és képességeket</span><span class="sxs-lookup"><span data-stu-id="a3171-113">You can't view or manage the expected pages or capabilities in Partner Center</span></span>

<span data-ttu-id="a3171-114">A partner Centerben lévő lapok elérését a hozzárendelt szerepkörök vezérlik.</span><span class="sxs-lookup"><span data-stu-id="a3171-114">Access to pages in Partner Center is controlled by the roles that you're assigned.</span></span> <span data-ttu-id="a3171-115">A hozzárendelt szerepkörök megtekintéséhez a partner Centerben válassza a beállítások ikont, válassza a **Fiókbeállítások** lehetőséget, majd a Fiókbeállítások területen válassza a **felhasználói kezelés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a3171-115">To check which roles you're assigned, in Partner Center select the Settings icon, select **Account settings**, and then in Account settings, select **User management**.</span></span> <span data-ttu-id="a3171-116">A Search (keresés) mezőbe írja be a nevét, majd tekintse meg az eredményeket.</span><span class="sxs-lookup"><span data-stu-id="a3171-116">In Search, type your name and then view the results.</span></span>

<span data-ttu-id="a3171-117">Ha nem tudja megtekinteni vagy kezelni a felszámított kompetenciákat, ügyfeleket, ösztönzőket vagy felhasználókat, próbálkozzon a következő megoldásokkal:</span><span class="sxs-lookup"><span data-stu-id="a3171-117">If you aren't able to view or manage the competencies, customers, incentives, or users that you expect, try the following solutions:</span></span>

- <span data-ttu-id="a3171-118">Az MPN, CSP és Referral képességeinek eléréséhez forduljon a globális rendszergazdához vagy a fiók rendszergazdájához. Ha többet szeretne megtudni a szerepkörökről és az általuk engedélyezett feladatokról a partner Centerben, tekintse meg a [szerepkörök & a felhasználók számára](permissions-overview.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="a3171-118">For access to the capabilities of MPN, CSP, and Referrals, contact your Global admin or Account admin. To learn more about roles and the tasks they enable in Partner Center, see [Assign roles & permissions to users](permissions-overview.md).</span></span>
- <span data-ttu-id="a3171-119">A kereskedelmi piactér és a Windows & Xbox, az Office áruház, a Microsoft Edge és a hardveres fejlesztői programok képességeinek eléréséhez vegye fel a kapcsolatot a szervezet tulajdonosi vagy felettesi szerepkörével.</span><span class="sxs-lookup"><span data-stu-id="a3171-119">For access to the capabilities of the Commercial Marketplace and the Windows & Xbox, Office Store, Microsoft Edge, and Hardware developer programs, contact the person in the Owner or Manager role in your organization.</span></span> <span data-ttu-id="a3171-120">További információ a szerepkörökről és az engedélyekről: [kereskedelmi Piactéri fiók kezelése a Microsoft partner Centerben](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span><span class="sxs-lookup"><span data-stu-id="a3171-120">To learn more about roles and permissions, see [How to manage a commercial marketplace account in Microsoft Partner Center](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span></span>

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a><span data-ttu-id="a3171-121">Nem tekintheti meg az ajánlatát vagy előnyeit a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="a3171-121">You can’t see your offer or benefits in Partner Center</span></span>

<span data-ttu-id="a3171-122">Győződjön meg arról, hogy a megfelelő hitelesítő adatokat használja a bejelentkezéshez.</span><span class="sxs-lookup"><span data-stu-id="a3171-122">Confirm that you are using the correct credentials to sign in.</span></span> <span data-ttu-id="a3171-123">Előfordulhat például, hogy a munkahelyi és a személyes fiókok ugyanúgy néznek ki (például abc@contoso.com :), de lehet, hogy egy személyes fiók, amelyet Ön hozott létre, és egy másik, az Ön nevében létrehozott üzleti fiók is.</span><span class="sxs-lookup"><span data-stu-id="a3171-123">For example, your work and personal accounts may look the same (such as abc@contoso.com), but one may be a personal account that you created and another may be a business account set up on your behalf.</span></span> <span data-ttu-id="a3171-124">Ebben az esetben, ha bejelentkezett, de nem tudja megtekinteni az MPN-vel, a CSP-vel, a kereskedelmi Piactérsel kapcsolatos várt képességeket, próbálja meg kiválasztani a munkahelyi fiókját.</span><span class="sxs-lookup"><span data-stu-id="a3171-124">In this case, if you are signed in, but are unable to view expected capabilities related to MPN, CSP, Commercial Marketplace, try selecting your work account.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a3171-125">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="a3171-125">Next steps</span></span>

- [<span data-ttu-id="a3171-126">Fiókadatok ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="a3171-126">Verify your account information</span></span>](verification-responses.md)
- [<span data-ttu-id="a3171-127">Saját jelszó visszaállítása</span><span class="sxs-lookup"><span data-stu-id="a3171-127">Reset my password</span></span>](reset-my-pasword.md)
- [<span data-ttu-id="a3171-128">Új felhasználói jelszó beállítása</span><span class="sxs-lookup"><span data-stu-id="a3171-128">Reset a user password</span></span>](reset-a-user-password.md)