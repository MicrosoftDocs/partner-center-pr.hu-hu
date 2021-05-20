---
title: Az eszközök "be nem verekedő" élményének testreszabása
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Az ügyfél új eszközének kézbesítése előtt Windows Autopilot-profilokkal testreszabhatja vagy előre konfigurálhatja az eszköz használatra előtti élményét (OOBE).
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149825"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="b3f7c-103">Windows Autopilot-profilok használata új eszközökön az ügyfél kezdőélményének testreszabásához</span><span class="sxs-lookup"><span data-stu-id="b3f7c-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="b3f7c-104">**Megfelelő szerepkörök:** Rendszergazdai ügynök | Globális rendszergazdai | Értékesítési ügynök | Felhasználókezelő rendszergazda</span><span class="sxs-lookup"><span data-stu-id="b3f7c-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | User management admin</span></span>

<span data-ttu-id="b3f7c-105">Ha ügyféleszközöket felügyel, előfordulhat, hogy testre kell szabni a felhasználói élményt (OOBE).</span><span class="sxs-lookup"><span data-stu-id="b3f7c-105">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="b3f7c-106">Az új eszközöket előre konfigurálhatja Windows Autopilot profilokkal, mielőtt az eszközöket az ügyfeleknek szállítja, és új profilokat alkalmazhat az ügyfelek által már megvásárolt eszközökre.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-106">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="b3f7c-107">Vegye figyelembe, hogy az EM-ek elkezdték az Autopilot-eszközdobozon kívüli fuvarlevélcímkét is, amely megjeleníti az eszköz termékkulcs-azonosítóját **(PKID).**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-107">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="b3f7c-108">Ez az egydimenziós, olvasható vonalkód lehetővé teszi az lefelé irányuló partnerek számára, hogy anélkül regisztrálják az eszközöket az Autopilotra, hogy le kell mondaniuk az eszköz(ük)ről, és alternatív módszerrel be kell gyűjteni az eszközazonosítót.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-108">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="b3f7c-109">Ez a cikk bemutatja, hogyan hozhat létre és alkalmazhat AutoPilot-profilokat a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="b3f7c-110">Ha még nem ismeri az Autopilotot, tekintse át az alábbi cikkekben található információkat:</span><span class="sxs-lookup"><span data-stu-id="b3f7c-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="b3f7c-111">A Windows Autopilot áttekintése</span><span class="sxs-lookup"><span data-stu-id="b3f7c-111">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="b3f7c-112">Útmutató az Autopilot üzembe helyezéséhez</span><span class="sxs-lookup"><span data-stu-id="b3f7c-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="b3f7c-113">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="b3f7c-113">Overview</span></span>

<span data-ttu-id="b3f7c-114">A Windows Autopilot funkcióval Partnerközpont egyéni profilokat hozhat létre az ügyféleszközökre való alkalmazáshoz.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="b3f7c-115">A cikk közzétételekor a következő profilbeállítások voltak elérhetők:</span><span class="sxs-lookup"><span data-stu-id="b3f7c-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="b3f7c-116">Hagyja ki az adatvédelmi beállításokat.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-116">Skip privacy settings.</span></span> <span data-ttu-id="b3f7c-117">Ez a választható Autopilot-profilbeállítás lehetővé teszi, hogy a szervezetek ne kérdezzenek az adatvédelmi beállításokról az OOBE folyamat során.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="b3f7c-118">Tiltsa le a helyi rendszergazdai fiók létrehozását az eszközön.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="b3f7c-119">A szervezetek eldöntheti, hogy az eszközt berakó felhasználó rendszergazdai hozzáféréssel rendelkezik-e a folyamat befejezése után.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="b3f7c-120">Az eszköz automatikus beállítása munkahelyi vagy iskolai alkalmazáshoz.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="b3f7c-121">Az Autopilotban regisztrált összes eszköz automatikusan munkahelyi vagy iskolai eszköznek minősül, ezért ezt a kérdést a rendszer nem fogja feltetetni az OOBE folyamat során.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="b3f7c-122">A Cortana,a OneDrive és az OEM regisztrációs oldalának kihagyása.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="b3f7c-123">Az Autopilottal regisztrált összes eszköz automatikusan kihagyja ezeket az oldalakat a be nem lépő felhasználói élmény (OOBE) folyamata során.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="b3f7c-124">Hagyja ki a végfelhasználói licencszerződést (EULA).</span><span class="sxs-lookup"><span data-stu-id="b3f7c-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="b3f7c-125">A Windows 10 1709-es verziójától kezdődően a szervezetek dönthetnek úgy, hogy kihagyják az OOBE folyamat során bemutatott EULA oldalt.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="b3f7c-126">A [Windows Autopilot eula dismissal (A EULA](#windows-autopilot-eula-dismissal) elvetését lásd alább) oldalon fontos információkat olvashat a EULA oldal kihagyásával kapcsolatban a Windows beállítása során.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="b3f7c-127">Az alábbi profil- és eszközfelügyeleti engedélyek és korlátozások érvényesek:</span><span class="sxs-lookup"><span data-stu-id="b3f7c-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="b3f7c-128">A CSP-partnerek továbbra is felügyelhetik az Autopilot-profilokat azon meglévő ügyfelek esetében, akikkel viszonteladói kapcsolatban vannak, még akkor is, ha az ügyfelek eltávolították a partner delegált rendszergazdai jogosultságait.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="b3f7c-129">Felügyelheti az Ön által hozzáadott ügyfelek meglévő eszközeit.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="b3f7c-130">Nem felügyelhet olyan eszközöket, amelyeket az ügyfél töltött fel a Microsoft Store Vállalatoknak áruházba vagy a Microsoft Intune-portálra.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-130">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="b3f7c-131">AutoPilot-profilok létrehozása és kezelése a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="b3f7c-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="b3f7c-132">A Partnerközpont létrehozhat telepítési Windows Autopilot profilokat, és alkalmazhatja őket az eszközökre.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="b3f7c-133">Profilokat csak rendszergazdai ügynökök hozhatnak létre és alkalmazhatnak.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="b3f7c-134">Új AutoPilot-profil létrehozása</span><span class="sxs-lookup"><span data-stu-id="b3f7c-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="b3f7c-135">Válassza **az Ügyfelek** Partnerközpont menüből, majd válassza ki azt az ügyfelet, aki számára létrehozza az Autopilot-profilt.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="b3f7c-136">Az ügyfél részletek lapján válassza az Eszközök **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b3f7c-137">A **Windows Autopilot profilok alatt válassza** az Új profil hozzáadása **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="b3f7c-138">Adja meg a profil nevét és leírását, majd konfigurálja az OOBE-beállításokat.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="b3f7c-139">A következő lehetőségek közül választhat:</span><span class="sxs-lookup"><span data-stu-id="b3f7c-139">Choose from:</span></span>  

   - <span data-ttu-id="b3f7c-140">Az adatvédelmi beállítások kihagyása a telepítőben</span><span class="sxs-lookup"><span data-stu-id="b3f7c-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="b3f7c-141">Helyi rendszergazdai fiók letiltása a telepítőben</span><span class="sxs-lookup"><span data-stu-id="b3f7c-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="b3f7c-142">Oldalak automatikus kihagyása a telepítőben</span><span class="sxs-lookup"><span data-stu-id="b3f7c-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="b3f7c-143">(Tartalmazza *a munkahelyi vagy iskolai beállítások* automatikus kiválasztását és a Cortana, a OneDrive és az OEM regisztrációs *oldalának kihagyása adatokat)*</span><span class="sxs-lookup"><span data-stu-id="b3f7c-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="b3f7c-144">Végfelhasználói licencszerződés (EULA) kihagyása</span><span class="sxs-lookup"><span data-stu-id="b3f7c-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="b3f7c-145">A [Windows Autopilot eula dismissal (A EULA](#windows-autopilot-eula-dismissal) elvetését lásd alább) oldalon fontos információkat olvashat a EULA oldal kihagyásával kapcsolatban a Windows beállítása során.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="b3f7c-146">Ha **elkészült, válassza** a Küldés lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="b3f7c-147">Autopilot-profil alkalmazása az ügyféleszközökre</span><span class="sxs-lookup"><span data-stu-id="b3f7c-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="b3f7c-148">Az alábbi utasítások feltételezik, hogy már hozzáadta az ügyfél eszközeit a Partnerközpont, és hozzáférhet az eszközlistához.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="b3f7c-149">Ha még nem adott hozzá az ügyfél eszközeit, [](#add-devices-to-a-customers-account) kövesse az Eszközök hozzáadása az ügyfél fiókjához lépéseit, majd kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="b3f7c-150">Miután létrehozott egy AutoPilot-profilt egy ügyfél számára, alkalmazhatja azt az ügyfél eszközeire.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="b3f7c-151">Válassza **az Ügyfelek** Partnerközpont menüből, majd válassza ki azt az ügyfelet, aki számára létrehozta az AutoPilot-profilt.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="b3f7c-152">Az ügyfél részletek lapján válassza az Eszközök **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b3f7c-153">A **Profilok alkalmazása eszközökre alatt** válassza ki azokat az eszközöket vagy eszközcsoportokat, amelyekhez profilokat kíván hozzáadni, majd válassza a Profil alkalmazása **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="b3f7c-154">Az előbb alkalmazott profil megjelenik a **Profil oszlopban.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="b3f7c-155">Kövesse az alábbi lépéseket annak ellenőrzéséhez, hogy a profil sikeresen alkalmazva lesz-e az eszközön.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="b3f7c-156">a.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-156">a.</span></span>  <span data-ttu-id="b3f7c-157">Csatlakoztassa az eszközt a hálózathoz, és kapcsolja be.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="b3f7c-158">b.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-158">b.</span></span>  <span data-ttu-id="b3f7c-159">Ellenőrizze, hogy megjelennek-e a megfelelő OOBE-képernyők (ha vannak).</span><span class="sxs-lookup"><span data-stu-id="b3f7c-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="b3f7c-160">c.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-160">c.</span></span>  <span data-ttu-id="b3f7c-161">Ha az OOBE folyamat leáll, állítsa vissza az eszközt a gyári alapértelmezett beállításokra, hogy előkészítse egy új felhasználó számára.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="b3f7c-162">AutoPilot-profil eltávolítása az ügyfél eszközéről</span><span class="sxs-lookup"><span data-stu-id="b3f7c-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="b3f7c-163">Válassza **az Ügyfelek** Partnerközpont menüből, majd válassza ki azt az ügyfelet, aki számára létrehozta az AutoPilot-profilt.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="b3f7c-164">Az ügyfél részletek lapján válassza az Eszközök **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b3f7c-165">A **Profilok alkalmazása eszközökre alatt** válassza ki azokat az eszközöket, amelyekről el szeretné távolítani a profilt, majd válassza a Profil eltávolítása **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="b3f7c-166">Egy profil eszközről való eltávolítása nem törli a profilt a listából.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="b3f7c-167">Ha törölni szeretne egy profilt, kövesse az [AutoPilot-profil](#update-or-delete-an-autopilot-profile)frissítésére vagy törlésére vonatkozó utasításokat.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="b3f7c-168">AutoPilot-profil frissítése vagy törlése</span><span class="sxs-lookup"><span data-stu-id="b3f7c-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="b3f7c-169">Ha egy ügyfél módosítani szeretné a már nem használható eszközöket, miután Ön kiszállította őket, a profilt a következő Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="b3f7c-170">Amikor az ügyfél eszköze csatlakozik az internethez, letölti a legújabb profilverziót az OOBE folyamat során.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="b3f7c-171">Emellett minden alkalommal, amikor egy ügyfél visszaállít egy eszközt az alapértelmezett gyári beállításokra, az eszköz az OOBE folyamat során ismét letölti a legújabb profilverziót.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="b3f7c-172">Válassza **az Ügyfelek** Partnerközpont menüből, majd válassza ki azt az ügyfelet, aki módosítani szeretné az AutoPilot-profilt.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="b3f7c-173">Az ügyfél részletek lapján válassza az Eszközök **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b3f7c-174">A **Windows Autopilot profilok alatt** válassza ki a frissíteni kívánt profilt.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="b3f7c-175">Tegye meg a szükséges módosításokat, majd válassza a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="b3f7c-176">A profil törléséhez válassza a **Profil** törlése lehetőséget az oldal jobb felső sarkában.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="b3f7c-177">Eszközök hozzáadása az ügyfél fiókjához</span><span class="sxs-lookup"><span data-stu-id="b3f7c-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="b3f7c-178">Az értékesítési ügynökök és a rendszergazdai ügynökök eszközöket adhatnak az ügyfél fiókjához.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="b3f7c-179">Mielőtt egyéni Autopilot-profilokat alkalmazhat az ügyféleszközökre, hozzá kell férnie az ügyfél eszközlistához.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="b3f7c-180">Ha oem-nevet, sorozatszámot és modellkombinációt tervez használni, vegye figyelembe az alábbi korlátozásokat:</span><span class="sxs-lookup"><span data-stu-id="b3f7c-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="b3f7c-181">Ez a rekord csak újabb eszközök esetében működik (például 4k-os hashes), és nem támogatott 128b-os (RS2- és korábbi) eszközökhöz.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="b3f7c-182">A rekordregisztráció megkülönbözteti a kis- és nagybetűket, ezért  a fájlban szereplő adatoknak pontosan az OEM-szolgáltató (hardverszolgáltató) által megadott modell- és gyártónevekkel kell megegyeznie.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="b3f7c-183">Kövesse az alábbi utasításokat, ha eszközöket szeretne hozzáadni egy ügyfél fiókjához a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="b3f7c-184">Válassza **az Ügyfelek** Partnerközpont, majd válassza ki azt az ügyfelet, akinek az eszközeit kezelni szeretné.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="b3f7c-185">Az ügyfél részletek lapján válassza az Eszközök **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="b3f7c-186">A Profilok **alkalmazása eszközökre alatt válassza** az Eszközök hozzáadása **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="b3f7c-187">Adja meg az eszközlista nevét, majd a Tallózás gombra kattintva töltse fel az ügyfél listáját (.csv fájlformátumban) Partnerközpont. </span><span class="sxs-lookup"><span data-stu-id="b3f7c-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="b3f7c-188">Ezt a .csv-fájlt az eszköz megvásárlásakor kellett megkapni.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="b3f7c-189">Ha nem kapott .csv-fájlt, létrehozhat egyet saját maga is az [Eszközök](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)hozzáadása a fájlhoz Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="b3f7c-190">Töltse fel a .csv-fájlt, majd válassza a **Mentés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="b3f7c-191">Ha a .csv fájl feltöltésekor hibaüzenetet kap, ellenőrizze a fájlformátumot.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="b3f7c-192">Használhat csak hardverkivonatot, vagy az OEM-nevet, sorozatszámot és modellt (ebben az oszlopsorrendben), vagy a Windows-termékazonosítót.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="b3f7c-193">Eszközlista létrehozásához használhatja az Eszközök hozzáadása melletti  hivatkozásból származó .csv-mintafájlt is.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="b3f7c-194">A .csv-fájlnak így kell kinéznie:</span><span class="sxs-lookup"><span data-stu-id="b3f7c-194">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="b3f7c-195">**Eszköz sorozatszáma,Windows-termékazonosító,Hardver kivonata,Gyártó neve,Eszközmodell**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-195">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="b3f7c-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="b3f7c-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="b3f7c-197">A "Gyártó neve" és az "Eszközmodell" megkülönbözteti a kis- és nagybetűket.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-197">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="b3f7c-198">Ha nem tudja, hogy milyen értéket kell tenni a Gyártó neve és az Eszközmodell mezőben, ezt az eszközön futtatva összegyűjtheti a megfelelő értékeket:</span><span class="sxs-lookup"><span data-stu-id="b3f7c-198">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="b3f7c-199">Windows Autopilot EULA elvetését</span><span class="sxs-lookup"><span data-stu-id="b3f7c-199">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="b3f7c-200">FONTOS INFORMÁCIÓK</span><span class="sxs-lookup"><span data-stu-id="b3f7c-200">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="b3f7c-201">Windows Autopilot segítségével testreszabott Windows-telepítéseket konfigurálhatja az ügyfelek számára ön által felügyelt eszközökön.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-201">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="b3f7c-202">Ha az ügyfél erre jogosult, letilthat vagy elrejthet bizonyos beállítási képernyőket, amelyek általában jelennek meg a felhasználók számára a Windows beállításakor, beleértve a végfelhasználói licencszerződés (EULA) elfogadási képernyőjét.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-202">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="b3f7c-203">A függvény használatával Ön beleegyezik abba, hogy a feltételek elfogadására vagy elfogadására tervezett képernyők mellőzése vagy elrejtése azt jelenti, hogy megfelelő beleegyezést és engedélyt szerzett az ügyféltől a feltételek elrejtéséhez, és Hogy Ön az ügyfél nevében (akár egy szervezet, akár adott esetben egy egyéni felhasználó) elfogadja az értesítéseket, és elfogadja az ügyfélre vonatkozó feltételeket.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-203">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="b3f7c-204">Ebbe beletartozik a licenc használati feltételeinek vagy az értesítésnek a szerződése, amely akkor jelenne meg a felhasználó számára, ha nem tiltja le vagy rejti el az eszközt használva.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-204">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="b3f7c-205">Az ügyfél nem használhatja a Windows-szoftvert ezen eszközökön, ha az ügyfél nem szerzett érvényes licencet a szoftverhez a Microsofttól vagy annak licencelt forgalmazóitól.</span><span class="sxs-lookup"><span data-stu-id="b3f7c-205">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>