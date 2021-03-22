---
title: A partner Center-fiók vagy az MPN megújítási problémáinak beállításával kapcsolatos hibák elhárítása
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: A partner Centerbe való regisztráció során felmerülő problémák elhárítása. Válaszok a fizetési módokkal, a Felejtési jelszavakkal és egyebekkel kapcsolatos problémákra.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d80651c4e5e4afb476dada388f23c118e0bdf25
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768703"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="35ba8-104">A Fiókbeállítások vagy az MPN megújítási problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="35ba8-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="35ba8-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="35ba8-105">**Appropriate roles**</span></span>

- <span data-ttu-id="35ba8-106">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="35ba8-106">Global admin</span></span>
- <span data-ttu-id="35ba8-107">MPN-partner rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="35ba8-107">MPN partner admin</span></span> 
 
<span data-ttu-id="35ba8-108">Íme néhány javaslat a partner Center-fiók beállításakor felmerülő gyakori problémák elhárításához.</span><span class="sxs-lookup"><span data-stu-id="35ba8-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="35ba8-109">Mi történik, ha a Partner tagsági központjából telepít át, és nem szerkesztheti a vállalati adatok mezőit</span><span class="sxs-lookup"><span data-stu-id="35ba8-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="35ba8-110">Azokban az esetekben, amikor a vállalata már rendelkezik jelenléttel a partner Centerben (például egy CSP-fiók), csak olvasható képernyő jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="35ba8-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="35ba8-111">Ezen a képernyőn jelennek meg a vállalatra vonatkozó összes információ a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="35ba8-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="35ba8-112">Ezen a képernyőn nem módosítható a részletek.</span><span class="sxs-lookup"><span data-stu-id="35ba8-112">You can't change the details on this screen.</span></span> <span data-ttu-id="35ba8-113">Ez a kialakítás és nem egy hiba.</span><span class="sxs-lookup"><span data-stu-id="35ba8-113">This is by design and not an error.</span></span>

<span data-ttu-id="35ba8-114">Válassza az **elfogadás** lehetőséget, és folytassa a **folytatást** .</span><span class="sxs-lookup"><span data-stu-id="35ba8-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="35ba8-115">Ha az informatikai részleg kikapcsolta a **partner Centerre való regisztrációt**</span><span class="sxs-lookup"><span data-stu-id="35ba8-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="35ba8-116">Ez az üzenet jelenik meg, mert a vírusos felhasználók le vannak tiltva, vagy mert a vírusos regisztráció le van tiltva az Azure AD-bérlőn.</span><span class="sxs-lookup"><span data-stu-id="35ba8-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="35ba8-117">Az Azure AD-fiók globális rendszergazdája a következő PowerShell-parancs futtatásával engedélyezheti a szükséges szolgáltatásokat:</span><span class="sxs-lookup"><span data-stu-id="35ba8-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="35ba8-118">**Set-Msolcompanysettings parancsmagjával-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="35ba8-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="35ba8-119">További tudnivalókért olvassa el az [önkiszolgáló regisztrációt](/azure/active-directory/users-groups-roles/directory-self-service-signup)ismertető témakört.</span><span class="sxs-lookup"><span data-stu-id="35ba8-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="35ba8-120">Elfelejtette a jelszavát</span><span class="sxs-lookup"><span data-stu-id="35ba8-120">You forgot your password</span></span>

<span data-ttu-id="35ba8-121">Ha elfelejtette a jelszavát, jelölje be a **nem érhető el a fiókja?** hivatkozásra a bejelentkezési oldalon.</span><span class="sxs-lookup"><span data-stu-id="35ba8-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="35ba8-122">Ezzel a beállítással visszaállíthatja a jelszavát, vagy megkérheti a globális rendszergazdát, hogy rendeljen új hitelesítő adatokat.</span><span class="sxs-lookup"><span data-stu-id="35ba8-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="35ba8-123">A "tudnivalók a vállalatról" képernyőn "hiba történt" hibaüzenet jelenik meg</span><span class="sxs-lookup"><span data-stu-id="35ba8-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="35ba8-124">Ez a hibaüzenet általában akkor jelenik meg, ha a céges telefonszámon véletlenül speciális karaktereket, szóközöket vagy országkódot használ.</span><span class="sxs-lookup"><span data-stu-id="35ba8-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="35ba8-125">A telefonszám mezőben megadott érték legfeljebb 10 karakterből állhat.</span><span class="sxs-lookup"><span data-stu-id="35ba8-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="35ba8-126">A bankkártya vásárlása egy hibaüzenetet kap arról, hogy "a megrendelés elutasítása megtörtént.</span><span class="sxs-lookup"><span data-stu-id="35ba8-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="35ba8-127">Kérjük, ellenőrizze az adatait "</span><span class="sxs-lookup"><span data-stu-id="35ba8-127">Please verify your information”</span></span>


<span data-ttu-id="35ba8-128">A jogi személy helyett mindig a hitelkártyájának megfelelő címeket használja.</span><span class="sxs-lookup"><span data-stu-id="35ba8-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="35ba8-129">Győződjön meg arról is, hogy a zip-kód helyes, és megfelel a használt címnek.</span><span class="sxs-lookup"><span data-stu-id="35ba8-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="35ba8-130">Offline fizetésről online fizetési módra szeretne váltani</span><span class="sxs-lookup"><span data-stu-id="35ba8-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="35ba8-131">Az előnyben részesített fizetési mód használatával meg kell szakítania az eredeti rendelést, és újra kell vásárolnia azt.</span><span class="sxs-lookup"><span data-stu-id="35ba8-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="35ba8-132">Megrendelés megszakítása:</span><span class="sxs-lookup"><span data-stu-id="35ba8-132">To cancel an order:</span></span>

1. <span data-ttu-id="35ba8-133">Válassza a **tagsági ajánlatok** fület az irányítópulton.</span><span class="sxs-lookup"><span data-stu-id="35ba8-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="35ba8-134">**Megszakított megrendelés** kiválasztása</span><span class="sxs-lookup"><span data-stu-id="35ba8-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="35ba8-135">Ekkor megjelenik egy megerősítési ablak, és meg kell erősítenie a kezdeti sorrend megszakításához.</span><span class="sxs-lookup"><span data-stu-id="35ba8-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="35ba8-136">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="35ba8-136">Next steps</span></span>

- [<span data-ttu-id="35ba8-137">Partnerközponti fiók kezelése</span><span class="sxs-lookup"><span data-stu-id="35ba8-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="35ba8-138">A Bill és a Recon-fájl beolvasása</span><span class="sxs-lookup"><span data-stu-id="35ba8-138">How to read your bill and recon file</span></span>](read-your-bill.md)
