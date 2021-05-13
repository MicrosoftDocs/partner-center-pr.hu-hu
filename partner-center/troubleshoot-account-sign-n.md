---
title: A fiók vagy az MPN-Partnerközpont beállításával kapcsolatos hibák elhárítása
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: A regisztrálással kapcsolatos problémák elhárítása a Partnerközpont. Választ ad a fizetési módok kihívásaira, a jelszavak kifelejtésére stb.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854689"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="63c9f-104">A fiók beállításával vagy az MPN megújításával kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="63c9f-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="63c9f-105">**Megfelelő szerepkörök:** Globális rendszergazdai | MPN-partner rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="63c9f-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="63c9f-106">Íme néhány javaslat a fiók beállításakor felmerülő gyakori problémák Partnerközpont elhárításához.</span><span class="sxs-lookup"><span data-stu-id="63c9f-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="63c9f-107">Mi történik, ha a vállalati Partner Membership Center, és nem szerkeszti a céges adatokat mezőit?</span><span class="sxs-lookup"><span data-stu-id="63c9f-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="63c9f-108">Ha a vállalat már jelen van a Partnerközpont (például CSP-fiók) – csak olvasható képernyő jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="63c9f-108">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="63c9f-109">Ezen a képernyőn a cég összes adata megjelenik, ahogyan az a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="63c9f-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="63c9f-110">Ezen a képernyőn nem módosíthatja a részleteket.</span><span class="sxs-lookup"><span data-stu-id="63c9f-110">You can't change the details on this screen.</span></span> <span data-ttu-id="63c9f-111">Ez tervezésből áll, és nem hiba.</span><span class="sxs-lookup"><span data-stu-id="63c9f-111">This is by design and not an error.</span></span>

<span data-ttu-id="63c9f-112">A **folytatáshoz válassza az Elfogadás** **és** a Folytatás lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="63c9f-112">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="63c9f-113">Ha az IT-részleg kikapcsolta a Regisztráció a **Partnerközpont**</span><span class="sxs-lookup"><span data-stu-id="63c9f-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="63c9f-114">Ez az üzenet azért jelenik meg, mert a virtuális felhasználók le vannak tiltva, vagy mert a regisztráció le van tiltva az Azure AD-bérlőn.</span><span class="sxs-lookup"><span data-stu-id="63c9f-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="63c9f-115">Az Azure AD-fiók globális rendszergazdája a következő PowerShell-parancs futtatásával engedélyezheti a szükséges funkciókat:</span><span class="sxs-lookup"><span data-stu-id="63c9f-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="63c9f-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="63c9f-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="63c9f-117">További információ: [Önkiszolgáló regisztráció.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="63c9f-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="63c9f-118">Elfelejtette a jelszavát</span><span class="sxs-lookup"><span data-stu-id="63c9f-118">You forgot your password</span></span>

<span data-ttu-id="63c9f-119">Ha elfelejtette a jelszavát, válassza a Nem tudja elérni a **fiókját?** hivatkozást a bejelentkezési oldalon.</span><span class="sxs-lookup"><span data-stu-id="63c9f-119">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="63c9f-120">Ezzel a lehetőséggel új jelszót kérhet, vagy megkérheti a globális rendszergazdát, hogy rendeljen hozzá új hitelesítő adatokat.</span><span class="sxs-lookup"><span data-stu-id="63c9f-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="63c9f-121">Az "Mondja el a cégét" képernyőn "Hiba történt" hibaüzenet jelenik meg</span><span class="sxs-lookup"><span data-stu-id="63c9f-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="63c9f-122">Ez a hibaüzenet általában akkor jelenik meg, ha véletlenül speciális karaktereket, szóközöket vagy országkódot használ a vállalati telefonszámban.</span><span class="sxs-lookup"><span data-stu-id="63c9f-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="63c9f-123">A Telefonszám mezőben megadott érték legfeljebb 10 karaktert tartalmazhat.</span><span class="sxs-lookup"><span data-stu-id="63c9f-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="63c9f-124">A hitelkártya-vásárláskor a következő hibaüzenet jelenik meg: "A rendelést elutasította a rendszer.</span><span class="sxs-lookup"><span data-stu-id="63c9f-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="63c9f-125">Kérjük, ellenőrizze az adatait"</span><span class="sxs-lookup"><span data-stu-id="63c9f-125">Please verify your information”</span></span>


<span data-ttu-id="63c9f-126">A jogi személy helyett mindig a hitelkártyája címének megfelelő címet használja.</span><span class="sxs-lookup"><span data-stu-id="63c9f-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="63c9f-127">Győződjön meg arról is, hogy az irányítószám helyes, és megfelel a használt címnek.</span><span class="sxs-lookup"><span data-stu-id="63c9f-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="63c9f-128">Szeretne váltani az offline fizetésről az online fizetési módra</span><span class="sxs-lookup"><span data-stu-id="63c9f-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="63c9f-129">Le kell mondania az eredeti rendelést, és újra kell azt használnia az előnyben részesített fizetési mód használatával.</span><span class="sxs-lookup"><span data-stu-id="63c9f-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="63c9f-130">Rendelés visszavonása:</span><span class="sxs-lookup"><span data-stu-id="63c9f-130">To cancel an order:</span></span>

1. <span data-ttu-id="63c9f-131">Válassza **a Tagsági ajánlatok** lapot az irányítópulton.</span><span class="sxs-lookup"><span data-stu-id="63c9f-131">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="63c9f-132">Válassza a **Rendelés visszavonása lehetőséget**</span><span class="sxs-lookup"><span data-stu-id="63c9f-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="63c9f-133">Megjelenik egy megerősítési ablak, és meg kell erősítenie a kezdeti rendelés lemondását.</span><span class="sxs-lookup"><span data-stu-id="63c9f-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="63c9f-134">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="63c9f-134">Next steps</span></span>

- [<span data-ttu-id="63c9f-135">Partnerközponti fiók kezelése</span><span class="sxs-lookup"><span data-stu-id="63c9f-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="63c9f-136">A számla és a felderítési fájl olvasása</span><span class="sxs-lookup"><span data-stu-id="63c9f-136">How to read your bill and recon file</span></span>](read-your-bill.md)
