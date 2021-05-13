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
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a><span data-ttu-id="65f53-103">Bejelentkezési problémák elhárítása Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="65f53-103">Troubleshoot sign-in issues for Partner Center</span></span>

<span data-ttu-id="65f53-104">**Megfelelő szerepkörök:** Minden partner, aki érdeklődik a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="65f53-104">**Appropriate roles**: All partners interested in Partner Center</span></span>

<span data-ttu-id="65f53-105">Ez a cikk a bejelentkezések gyakori bejelentkezési problémáinak megoldásait Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="65f53-105">This article contains solutions for common sign-in issues for Partner Center.</span></span>

## <a name="youve-forgotten-your-password-for-partner-center"></a><span data-ttu-id="65f53-106">Elfelejtette a jelszó Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="65f53-106">You've forgotten your password for Partner Center</span></span>

<span data-ttu-id="65f53-107">Ha elfelejtette a jelszavát, és nem tud bejelentkezni a Partnerközpont, forduljon az ügyfélszolgálathoz.</span><span class="sxs-lookup"><span data-stu-id="65f53-107">If you have forgotten your password and can't sign into Partner Center, contact Support.</span></span> <span data-ttu-id="65f53-108">Keresse meg a megfelelő kapcsolattartót [a Támogatási üzleti termékeknél.](/microsoft-365/admin/contact-support-for-business-products)</span><span class="sxs-lookup"><span data-stu-id="65f53-108">Find the appropriate contact at [Support for Business Products](/microsoft-365/admin/contact-support-for-business-products).</span></span>

<span data-ttu-id="65f53-109">Ha Ön MPN-partner, kérje meg globális rendszergazdáját, hogy hozzon létre egy új jelszót.</span><span class="sxs-lookup"><span data-stu-id="65f53-109">If you're an MPN partner, ask your Global admin to create a new password for you.</span></span> <span data-ttu-id="65f53-110">Ha Ön közvetett CSP-viszonteladó, kérje meg közvetett szolgáltatóját, hogy hozzon létre egy új globális rendszergazdát az Azure AD-bérlőn, vagy hozzon létre egy új jelszót az Ön számára a delegált rendszergazdai jogosultságai használatával.</span><span class="sxs-lookup"><span data-stu-id="65f53-110">If you're a CSP Indirect reseller, ask your Indirect provider to create a new Global admin for you on your Azure AD tenant or create a new password for you using their delegated admin privileges.</span></span>

<span data-ttu-id="65f53-111">A jelszó visszaállításáról és a munkahelyi fiókhoz való hozzáférés visszaszerzésével kapcsolatos további információkért olvassa el a Következőt: Munkahelyi vagy iskolai jelszó visszaállítása [biztonsági adatok használatával.](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="65f53-111">To learn more about how you can reset your password and regain access to your work account, read [Reset your work or school password using security info](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).</span></span>

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a><span data-ttu-id="65f53-112">Nem tudja megtekinteni vagy kezelni a várt oldalakat vagy képességeket a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="65f53-112">You can't view or manage the expected pages or capabilities in Partner Center</span></span>

<span data-ttu-id="65f53-113">A hozzáférés a Partnerközpont a hozzárendelt szerepkörök vezérlik.</span><span class="sxs-lookup"><span data-stu-id="65f53-113">Access to pages in Partner Center is controlled by the roles that you're assigned.</span></span> <span data-ttu-id="65f53-114">A hozzárendelt szerepkörök ellenőrzéséhez válassza Partnerközpont beállítások ikont, válassza a Fiókbeállítások lehetőséget, majd a Fiókbeállítások között válassza a **Felhasználókezelés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="65f53-114">To check which roles you're assigned, in Partner Center select the Settings icon, select **Account settings**, and then in Account settings, select **User management**.</span></span> <span data-ttu-id="65f53-115">A Keresés mezőbe írja be a nevét, majd tekintse meg az eredményeket.</span><span class="sxs-lookup"><span data-stu-id="65f53-115">In Search, type your name and then view the results.</span></span>

<span data-ttu-id="65f53-116">Ha nem tudja megtekinteni vagy kezelni a várt kompetenciákat, ügyfeleket, ösztönzőket vagy felhasználókat, próbálkozzon a következő megoldásokkal:</span><span class="sxs-lookup"><span data-stu-id="65f53-116">If you aren't able to view or manage the competencies, customers, incentives, or users that you expect, try the following solutions:</span></span>

- <span data-ttu-id="65f53-117">Az MPN, a CSP és a hivatkozások képességeihez való hozzáféréshez forduljon a globális rendszergazdához vagy a fiókadminisztrához. További információ a szerepkörökről és az Partnerközpont által a szerepkörök hozzárendelése & [felhasználókhoz.](permissions-overview.md)</span><span class="sxs-lookup"><span data-stu-id="65f53-117">For access to the capabilities of MPN, CSP, and Referrals, contact your Global admin or Account admin. To learn more about roles and the tasks they enable in Partner Center, see [Assign roles & permissions to users](permissions-overview.md).</span></span>
- <span data-ttu-id="65f53-118">A kereskedelmi piactér és a Windows & Xbox, az Office Store, a Microsoft Edge és a Hardverfejlesztői programok funkcióihoz való hozzáféréshez lépjen kapcsolatba a szervezet Tulajdonos vagy Vezető szerepkörével.</span><span class="sxs-lookup"><span data-stu-id="65f53-118">For access to the capabilities of the Commercial Marketplace and the Windows & Xbox, Office Store, Microsoft Edge, and Hardware developer programs, contact the person in the Owner or Manager role in your organization.</span></span> <span data-ttu-id="65f53-119">További információ a szerepkörökről és engedélyekről: Kereskedelmi piactéri fiók [kezelése a Microsoft Partnerközpont.](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)</span><span class="sxs-lookup"><span data-stu-id="65f53-119">To learn more about roles and permissions, see [How to manage a commercial marketplace account in Microsoft Partner Center](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span></span>

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a><span data-ttu-id="65f53-120">Az ajánlat vagy az előnyök nem látszanának a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="65f53-120">You can’t see your offer or benefits in Partner Center</span></span>

<span data-ttu-id="65f53-121">Győződjön meg arról, hogy a megfelelő hitelesítő adatokat használja a bejelentkezéshez.</span><span class="sxs-lookup"><span data-stu-id="65f53-121">Confirm that you are using the correct credentials to sign in.</span></span> <span data-ttu-id="65f53-122">Előfordulhat például, hogy a munkahelyi és a személyes fiókjai ugyanúgy néznek ki (például ), de az egyik lehet egy Ön által létrehozott személyes fiók, egy másik pedig az Ön nevében beállított üzleti abc@contoso.com fiók.</span><span class="sxs-lookup"><span data-stu-id="65f53-122">For example, your work and personal accounts may look the same (such as abc@contoso.com), but one may be a personal account that you created and another may be a business account set up on your behalf.</span></span> <span data-ttu-id="65f53-123">Ebben az esetben, ha bejelentkezett, de nem tudja megtekinteni az MPN-hez, a CSP-hez és a kereskedelmi piactérhez kapcsolódó várt képességeket, próbálja meg kiválasztani a munkahelyi fiókját.</span><span class="sxs-lookup"><span data-stu-id="65f53-123">In this case, if you are signed in, but are unable to view expected capabilities related to MPN, CSP, Commercial Marketplace, try selecting your work account.</span></span>

## <a name="next-steps"></a><span data-ttu-id="65f53-124">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="65f53-124">Next steps</span></span>

- [<span data-ttu-id="65f53-125">Fiókadatok ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="65f53-125">Verify your account information</span></span>](verification-responses.md)
- [<span data-ttu-id="65f53-126">Saját jelszó visszaállítása</span><span class="sxs-lookup"><span data-stu-id="65f53-126">Reset my password</span></span>](reset-my-pasword.md)
- [<span data-ttu-id="65f53-127">Új felhasználói jelszó beállítása</span><span class="sxs-lookup"><span data-stu-id="65f53-127">Reset a user password</span></span>](reset-a-user-password.md)