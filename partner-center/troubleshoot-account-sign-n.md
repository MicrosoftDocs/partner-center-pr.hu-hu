---
title: A fiók vagy az MPN-Partnerközpont beállításával kapcsolatos hibák elhárítása
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: A regisztrálással kapcsolatos problémák elhárítása a Partnerközpont. A válaszok számos más kérdésre is választ adnak a fizetési módok, a jelszavakkal való elfelejtés és egyéb problémák esetén.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686262"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="70884-104">A fiók beállításával vagy az MPN megújításával kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="70884-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="70884-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="70884-105">**Appropriate roles**</span></span>

- <span data-ttu-id="70884-106">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="70884-106">Global admin</span></span>
- <span data-ttu-id="70884-107">MPN-partneri rendszergazda</span><span class="sxs-lookup"><span data-stu-id="70884-107">MPN partner admin</span></span>
 
<span data-ttu-id="70884-108">Íme néhány javaslat a fiók beállításakor felmerülő gyakori problémák Partnerközpont elhárításához.</span><span class="sxs-lookup"><span data-stu-id="70884-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="70884-109">Mi történik, ha a vállalati Partner Membership Center, és nem szerkeszti a céges adatokat mezőit?</span><span class="sxs-lookup"><span data-stu-id="70884-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="70884-110">Olyan esetekben, amikor a vállalat már jelen van a Partnerközpont (például CSP-fiók) – egy csak olvasható képernyő jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="70884-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="70884-111">Ezen a képernyőn a cég összes adata megjelenik, ahogyan az a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="70884-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="70884-112">Ezen a képernyőn nem módosíthatja a részleteket.</span><span class="sxs-lookup"><span data-stu-id="70884-112">You can't change the details on this screen.</span></span> <span data-ttu-id="70884-113">Ez a tervezéstől és nem a hibától áll.</span><span class="sxs-lookup"><span data-stu-id="70884-113">This is by design and not an error.</span></span>

<span data-ttu-id="70884-114">A **folytatáshoz válassza az Elfogadás** és a **Folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="70884-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="70884-115">Ha az it-részleg kikapcsolta **a Regisztráció** Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="70884-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="70884-116">Ez az üzenet azért jelenik meg, mert a virtuális felhasználók le vannak tiltva, vagy mert a regisztráció le van tiltva az Azure AD-bérlőn.</span><span class="sxs-lookup"><span data-stu-id="70884-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="70884-117">Az Azure AD-fiók globális rendszergazdája a következő PowerShell-parancs futtatásával engedélyezheti a szükséges funkciókat:</span><span class="sxs-lookup"><span data-stu-id="70884-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="70884-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="70884-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="70884-119">További információ: [Önkiszolgáló regisztráció.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="70884-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="70884-120">Elfelejtette a jelszavát</span><span class="sxs-lookup"><span data-stu-id="70884-120">You forgot your password</span></span>

<span data-ttu-id="70884-121">Ha elfelejtette a jelszavát, válassza a Nem tudja elérni a **fiókját?** hivatkozást a bejelentkezési oldalon.</span><span class="sxs-lookup"><span data-stu-id="70884-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="70884-122">Ezzel a lehetőséggel új jelszót kérhet, vagy megkérheti a globális rendszergazdát, hogy rendeljen hozzá új hitelesítő adatokat.</span><span class="sxs-lookup"><span data-stu-id="70884-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="70884-123">Az "Mondja el a cégét" képernyőn "Hiba történt" hibaüzenet jelenik meg</span><span class="sxs-lookup"><span data-stu-id="70884-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="70884-124">Ez a hibaüzenet általában akkor jelenik meg, ha véletlenül speciális karaktereket, szóközöket vagy országkódot használ a vállalati telefonszámban.</span><span class="sxs-lookup"><span data-stu-id="70884-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="70884-125">A Telefonszám mezőben megadott érték legfeljebb 10 karaktert tartalmazhat.</span><span class="sxs-lookup"><span data-stu-id="70884-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="70884-126">A hitelkártya-vásárláshoz a következő hibaüzenet jelenik meg: "A rendelést elutasította a rendszer.</span><span class="sxs-lookup"><span data-stu-id="70884-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="70884-127">Kérjük, ellenőrizze az adatait"</span><span class="sxs-lookup"><span data-stu-id="70884-127">Please verify your information”</span></span>


<span data-ttu-id="70884-128">Mindig a hitelkártyához tartozó címet használja a jogi személy helyett.</span><span class="sxs-lookup"><span data-stu-id="70884-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="70884-129">Győződjön meg arról is, hogy az irányítószám helyes, és megfelel a használt címnek.</span><span class="sxs-lookup"><span data-stu-id="70884-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="70884-130">Váltani szeretne az offline fizetésről az online fizetési módra</span><span class="sxs-lookup"><span data-stu-id="70884-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="70884-131">Le kell mondania az eredeti rendelést, és újra kell azt használnia az előnyben részesített fizetési mód használatával.</span><span class="sxs-lookup"><span data-stu-id="70884-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="70884-132">Rendelés visszavonása:</span><span class="sxs-lookup"><span data-stu-id="70884-132">To cancel an order:</span></span>

1. <span data-ttu-id="70884-133">Válassza **a Tagsági ajánlatok** lapot az irányítópulton.</span><span class="sxs-lookup"><span data-stu-id="70884-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="70884-134">Válassza a **Rendelés visszavonása lehetőséget**</span><span class="sxs-lookup"><span data-stu-id="70884-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="70884-135">Megjelenik egy megerősítési ablak, és meg kell erősítenie a kezdeti rendelés lemondását.</span><span class="sxs-lookup"><span data-stu-id="70884-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="70884-136">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="70884-136">Next steps</span></span>

- [<span data-ttu-id="70884-137">Partnerközponti fiók kezelése</span><span class="sxs-lookup"><span data-stu-id="70884-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="70884-138">A számla és a felderítési fájl olvasása</span><span class="sxs-lookup"><span data-stu-id="70884-138">How to read your bill and recon file</span></span>](read-your-bill.md)
