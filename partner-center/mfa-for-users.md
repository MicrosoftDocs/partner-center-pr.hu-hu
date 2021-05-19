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
ms.openlocfilehash: 5173526d0f65623311d5cd3a1061e8b9e93e9bb9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151627"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="6ebcc-103">Többtényezős hitelesítés beállítása a saját felhasználókhoz</span><span class="sxs-lookup"><span data-stu-id="6ebcc-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="6ebcc-104">**Megfelelő szerepkörök:** Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="6ebcc-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="6ebcc-105">A nagyobb adatvédelmi védelem és biztonság az egyik legfontosabb prioritásunk.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="6ebcc-106">Tudjuk, hogy a legjobb védelem a megelőzés, és hogy csak annyira vagyunk erősek, mint a leggyengébbek.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="6ebcc-107">Ezért van szükség arra, hogy az ökoszisztémánkban mindenki cselekedjen, és megfelelő biztonsági védelmi intézkedésekre legyen szükség.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="6ebcc-108">Határozottan javasoljuk, hogy minden partner engedélyezze a többtényezős hitelesítést (MFA) a partnerbérlő felhasználói számára.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="6ebcc-109">Többtényezős hitelesítés hozzáadása a felhasználók számára</span><span class="sxs-lookup"><span data-stu-id="6ebcc-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="6ebcc-110">A feladat végrehajtásához a vállalat globális rendszergazdának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="6ebcc-111">Az MFA-t a legkönnyebb engedélyezni a felhasználók számára, amikor hozzáadja őket az Azure AD-bérlőhöz.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="6ebcc-112">Jelentkezzen be a [Azure Portal,](https://portal.azure.com) majd a **Felhasználókezelés felületre.**</span><span class="sxs-lookup"><span data-stu-id="6ebcc-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="6ebcc-113">Válassza **a Többtényezős hitelesítés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6ebcc-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="6ebcc-114">Válassza ki az engedélyezni kívánt felhasználót, majd válassza az **Engedélyezés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6ebcc-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="6ebcc-115">Ez engedélyezi az MFA-t a felhasználó számára.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-115">This will enable MFA for this user.</span></span> <span data-ttu-id="6ebcc-116">Az Engedélyezve beállítás azt jelenti, hogy a felhasználónak be kell állítania az MFA-ellenőrzést, amikor először jelentkezik be.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="6ebcc-117">Ezt követően a bejelentkezés után meg kell adniuk egy kódot, amelyet e-mailben vagy szöveges üzenetben (a beállításuktól függően) biztosítanak.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Az ellenőrzés ellenőrzésére való beállítás megadása":::

>[!NOTE]
><span data-ttu-id="6ebcc-119">Kényszerítheti **a felhasználókat** az MFA használatára a fenti lépésekkel, majd a **Kényszerítés lehetőség kiválasztásával.**</span><span class="sxs-lookup"><span data-stu-id="6ebcc-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="6ebcc-120">További információ: [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates)(Felhasználónkénti Azure Multi-Factor Authentication engedélyezése a bejelentkezési események biztonságának érdekében).</span><span class="sxs-lookup"><span data-stu-id="6ebcc-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="6ebcc-121">Minden felhasználó a Disabled (Letiltva) **indítást indítja** el.</span><span class="sxs-lookup"><span data-stu-id="6ebcc-121">All users start out **Disabled**.</span></span> <span data-ttu-id="6ebcc-122">Amikor felhasználónkénti vagy többtényezős Azure Active Directory regisztrál felhasználókat, az állapotuk Engedélyezve **lesz.**</span><span class="sxs-lookup"><span data-stu-id="6ebcc-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="6ebcc-123">Ha az engedélyezett felhasználók bejelentkeznek és befejezik a regisztrációs folyamatot, az állapotuk **Kényszerítve állapotra változik.**</span><span class="sxs-lookup"><span data-stu-id="6ebcc-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="6ebcc-124">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="6ebcc-124">Next steps</span></span>

- [<span data-ttu-id="6ebcc-125">Szerepkörök és engedélyek hozzárendelése a felhasználókhoz</span><span class="sxs-lookup"><span data-stu-id="6ebcc-125">Assign roles and permissions to users</span></span>](permissions-overview.md)