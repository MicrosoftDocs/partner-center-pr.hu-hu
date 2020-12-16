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
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="4d491-103">Többtényezős hitelesítés beállítása a saját felhasználókhoz</span><span class="sxs-lookup"><span data-stu-id="4d491-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="4d491-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="4d491-104">**Appropriate roles**</span></span>

- <span data-ttu-id="4d491-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="4d491-105">Global admin</span></span>

<span data-ttu-id="4d491-106">A kiemelt prioritások közé tartozik a nagyobb adatvédelmi védelem és biztonság.</span><span class="sxs-lookup"><span data-stu-id="4d491-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="4d491-107">Tudjuk, hogy a legjobb védelem a megelőzés, és hogy csak olyan erősek vagyunk, mint a leggyengébb kapcsolatunk.</span><span class="sxs-lookup"><span data-stu-id="4d491-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="4d491-108">Ezért van szükségünk arra, hogy az ökoszisztémánk mindenki számára elérhető legyen, és biztosítsuk a megfelelő biztonsági védelem biztosítását.</span><span class="sxs-lookup"><span data-stu-id="4d491-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="4d491-109">Javasoljuk, hogy az összes partner számára engedélyezze a többtényezős hitelesítés (MFA) használatát a partner bérlője felhasználói számára.</span><span class="sxs-lookup"><span data-stu-id="4d491-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="4d491-110">Multi-Factor Authentication hozzáadása a felhasználók számára</span><span class="sxs-lookup"><span data-stu-id="4d491-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="4d491-111">A feladat elvégzéséhez a vállalat globális rendszergazdájának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="4d491-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="4d491-112">Az Azure AD-bérlőhöz való hozzáadásakor a legegyszerűbben engedélyezheti az MFA használatát a felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="4d491-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="4d491-113">Jelentkezzen be a [Azure Portalba](https://portal.azure.com) , majd lépjen a **felhasználói felügyelet** gombra.</span><span class="sxs-lookup"><span data-stu-id="4d491-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="4d491-114">Válassza a **többtényezős hitelesítés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4d491-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="4d491-115">Válassza ki az engedélyezni kívánt felhasználót, majd válassza az **Engedélyezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4d491-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="4d491-116">Ez lehetővé teszi az MFA használatát ehhez a felhasználóhoz.</span><span class="sxs-lookup"><span data-stu-id="4d491-116">This will enable MFA for this user.</span></span> <span data-ttu-id="4d491-117">Az Engedélyezve beállítás azt jelenti, hogy a rendszer az első bejelentkezéskor kéri a felhasználót, hogy állítson be MFA-ellenőrzést.</span><span class="sxs-lookup"><span data-stu-id="4d491-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="4d491-118">Ezt követően a bejelentkezéskor a rendszer arra kéri, hogy adja meg a nekik küldött kódot e-mailben vagy szöveges üzenetben (attól függően, hogy melyiket beállították).</span><span class="sxs-lookup"><span data-stu-id="4d491-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Az ellenőrzés módjának meghatározása":::

>[!NOTE]
><span data-ttu-id="4d491-120">Az MFA használatára **kényszerítheti** a felhasználókat, hogy a fenti lépéseket követve, a **kikényszerítés** lehetőség választásával.</span><span class="sxs-lookup"><span data-stu-id="4d491-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="4d491-121">További információért olvassa el a [felhasználónkénti Azure-multi-Factor Authentication engedélyezése a bejelentkezési események biztonságossá tételéhez](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates)című témakört.</span><span class="sxs-lookup"><span data-stu-id="4d491-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="4d491-122">Az összes felhasználó **le van tiltva**.</span><span class="sxs-lookup"><span data-stu-id="4d491-122">All users start out **Disabled**.</span></span> <span data-ttu-id="4d491-123">Ha felhasználónkénti Azure-Multi-Factor Authentication regisztrálja a felhasználókat, az állapotuk **engedélyezve** értékre vált.</span><span class="sxs-lookup"><span data-stu-id="4d491-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="4d491-124">Ha az engedélyezett felhasználók bejelentkeznek, és elvégzik a regisztrációs folyamatot, az állapotuk **kényszerítve** értékűre vált.</span><span class="sxs-lookup"><span data-stu-id="4d491-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="4d491-125">További lépések</span><span class="sxs-lookup"><span data-stu-id="4d491-125">Next steps</span></span>

- [<span data-ttu-id="4d491-126">Szerepkörök és engedélyek hozzárendelése a felhasználókhoz</span><span class="sxs-lookup"><span data-stu-id="4d491-126">Assign roles and permissions to users</span></span>](permissions-overview.md)

