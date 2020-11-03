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
ms.openlocfilehash: d990a2cb4dcb69dfc76e8a4f0d40fd4912b4f8a0
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530456"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="59b45-104">A Fiókbeállítások vagy az MPN megújítási problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="59b45-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="59b45-105">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="59b45-105">**Applies to**</span></span>

- <span data-ttu-id="59b45-106">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="59b45-106">Partner Center</span></span>
 
<span data-ttu-id="59b45-107">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="59b45-107">**Appropriate roles**</span></span>

- <span data-ttu-id="59b45-108">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="59b45-108">Global admin</span></span>
- <span data-ttu-id="59b45-109">MPN-partner rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="59b45-109">MPN partner admin</span></span> 
 
<span data-ttu-id="59b45-110">Íme néhány javaslat a partner Center-fiók beállításakor felmerülő gyakori problémák elhárításához.</span><span class="sxs-lookup"><span data-stu-id="59b45-110">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="59b45-111">Mi történik, ha a Partner tagsági központjából telepít át, és nem szerkesztheti a vállalati adatok mezőit</span><span class="sxs-lookup"><span data-stu-id="59b45-111">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="59b45-112">Azokban az esetekben, amikor a vállalata már rendelkezik jelenléttel a partner Centerben (például CSP-fiók) – egy írásvédett képernyő jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="59b45-112">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="59b45-113">Ezen a képernyőn jelennek meg a vállalatra vonatkozó összes információ a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="59b45-113">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="59b45-114">Ezen a képernyőn nem módosítható a részletek.</span><span class="sxs-lookup"><span data-stu-id="59b45-114">You can't change the details on this screen.</span></span> <span data-ttu-id="59b45-115">Ez a kialakítás és nem egy hiba.</span><span class="sxs-lookup"><span data-stu-id="59b45-115">This is by design and not an error.</span></span>

<span data-ttu-id="59b45-116">Válassza az **elfogadás** lehetőséget, és folytassa a **folytatást** .</span><span class="sxs-lookup"><span data-stu-id="59b45-116">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="59b45-117">Ha az informatikai részleg kikapcsolta a **partneri központ regisztrációját** .</span><span class="sxs-lookup"><span data-stu-id="59b45-117">If the IT department has turned off **sign up for Partner Center** .</span></span>

<span data-ttu-id="59b45-118">Ez az üzenet jelenik meg, mert a vírusos felhasználók le vannak tiltva, vagy mert a vírusos regisztráció le van tiltva az Azure AD-bérlőn.</span><span class="sxs-lookup"><span data-stu-id="59b45-118">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="59b45-119">Az Azure AD-fiók globális rendszergazdája a következő PowerShell-parancs futtatásával engedélyezheti a szükséges szolgáltatásokat:</span><span class="sxs-lookup"><span data-stu-id="59b45-119">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="59b45-120">**Set-Msolcompanysettings parancsmagjával-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="59b45-120">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="59b45-121">További információért olvassa el az [önkiszolgáló regisztrációt](/azure/active-directory/users-groups-roles/directory-self-service-signup) ismertető témakört.</span><span class="sxs-lookup"><span data-stu-id="59b45-121">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="59b45-122">Elfelejtette a jelszavát</span><span class="sxs-lookup"><span data-stu-id="59b45-122">You forgot your password</span></span>

<span data-ttu-id="59b45-123">Ha elfelejtette a jelszavát, jelölje be a **nem érhető el a fiókja?** hivatkozásra a bejelentkezési oldalon.</span><span class="sxs-lookup"><span data-stu-id="59b45-123">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="59b45-124">Ezzel a beállítással visszaállíthatja a jelszavát, vagy megkérheti a globális rendszergazdát, hogy rendeljen új hitelesítő adatokat.</span><span class="sxs-lookup"><span data-stu-id="59b45-124">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-scree-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="59b45-125">A "mondja el a céget" sziklatörmelék "hiba történt" hibaüzenetet kap.</span><span class="sxs-lookup"><span data-stu-id="59b45-125">On the “Tell us about your company” scree, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="59b45-126">Ez a hibaüzenet általában akkor jelenik meg, ha a céges telefonszámon véletlenül speciális karaktereket, szóközöket vagy országkódot használ.</span><span class="sxs-lookup"><span data-stu-id="59b45-126">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="59b45-127">A telefonszám mezőben megadott érték legfeljebb 10 karakterből állhat.</span><span class="sxs-lookup"><span data-stu-id="59b45-127">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="59b45-128">A bankkártya vásárlása egy hibaüzenetet kap arról, hogy "a megrendelés elutasítása megtörtént.</span><span class="sxs-lookup"><span data-stu-id="59b45-128">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="59b45-129">Kérjük, ellenőrizze az adatait "</span><span class="sxs-lookup"><span data-stu-id="59b45-129">Please verify your information”</span></span>


<span data-ttu-id="59b45-130">A jogi személy helyett mindig a hitelkártyájának megfelelő címeket használja.</span><span class="sxs-lookup"><span data-stu-id="59b45-130">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="59b45-131">Győződjön meg arról is, hogy a zip-kód helyes, és megfelel a használt címnek.</span><span class="sxs-lookup"><span data-stu-id="59b45-131">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="59b45-132">Offline fizetésről online fizetési módra szeretne váltani</span><span class="sxs-lookup"><span data-stu-id="59b45-132">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="59b45-133">Az előnyben részesített fizetési mód használatával meg kell szakítania az eredeti rendelést, és újra kell vásárolnia azt.</span><span class="sxs-lookup"><span data-stu-id="59b45-133">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="59b45-134">Megrendelés megszakítása:</span><span class="sxs-lookup"><span data-stu-id="59b45-134">To cancel an order:</span></span>

1. <span data-ttu-id="59b45-135">Válassza a **tagsági ajánlatok** fület az irányítópulton.</span><span class="sxs-lookup"><span data-stu-id="59b45-135">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="59b45-136">**Megszakított megrendelés** kiválasztása</span><span class="sxs-lookup"><span data-stu-id="59b45-136">Select **Cancel order**</span></span>

3. <span data-ttu-id="59b45-137">Ekkor megjelenik egy megerősítési ablak, és meg kell erősítenie a kezdeti sorrend megszakításához.</span><span class="sxs-lookup"><span data-stu-id="59b45-137">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="59b45-138">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="59b45-138">Next steps</span></span>

- [<span data-ttu-id="59b45-139">Partnerközponti fiók kezelése</span><span class="sxs-lookup"><span data-stu-id="59b45-139">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="59b45-140">A Bill és a Recon-fájl beolvasása</span><span class="sxs-lookup"><span data-stu-id="59b45-140">How to read your bill and recon file</span></span>](read-your-bill.md)