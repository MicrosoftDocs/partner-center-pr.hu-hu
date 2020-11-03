---
title: Az eszköz beépített felületének testreszabása
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Az ügyfél új eszközének továbbítása előtt a Windows Autopilot-profilokkal testreszabhatja vagy előre konfigurálhatja az eszköz beépített élményét (OOBE).
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 0ae61db0ca040afe67faa3a0883ea033b8f67562
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528502"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="b413c-103">Windows Autopilot-profilok használata új eszközökön az ügyfél kezdőélményének testreszabásához</span><span class="sxs-lookup"><span data-stu-id="b413c-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="b413c-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="b413c-104">**Applies to**</span></span>

- <span data-ttu-id="b413c-105">CSP Direct – számlázási partnerek, közvetett szolgáltatók és közvetett viszonteladók</span><span class="sxs-lookup"><span data-stu-id="b413c-105">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="b413c-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="b413c-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b413c-107">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="b413c-107">Admin agent</span></span>
- <span data-ttu-id="b413c-108">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="b413c-108">Global admin</span></span>
- <span data-ttu-id="b413c-109">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="b413c-109">Sales agent</span></span>
- <span data-ttu-id="b413c-110">Felhasználói felügyeleti rendszergazda</span><span class="sxs-lookup"><span data-stu-id="b413c-110">User management admin</span></span>

<span data-ttu-id="b413c-111">Ha az ügyfeleket felügyeli, előfordulhat, hogy testre kell szabnia az ügyfél felhasználói számára a beépített (OOBE) élményt.</span><span class="sxs-lookup"><span data-stu-id="b413c-111">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="b413c-112">Előre konfigurálhatja az új eszközöket a Windows Autopilot-profilokkal, mielőtt az eszközöket az ügyfeleknek kézbesíti, és új profilokat alkalmazzon az ügyfelek számára már megvásárolt eszközökre.</span><span class="sxs-lookup"><span data-stu-id="b413c-112">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="b413c-113">Vegye figyelembe, hogy a számítógépgyártók megkezdték az eszköz **termékkulcs-azonosítóját (PKID)** megjelenítő, az Autopilot-eszközön kívüli szállítási címkét is.</span><span class="sxs-lookup"><span data-stu-id="b413c-113">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)** .</span></span>  <span data-ttu-id="b413c-114">Ez az 1 dimenziós, olvasható vonalkód olyan alsóbb szintű partnereket biztosít, amelyek lehetővé teszik, hogy az eszköz (ek) bevonása nélkül regisztrálják az eszközöket, és más módon betakarították az eszköz AZONOSÍTÓját.</span><span class="sxs-lookup"><span data-stu-id="b413c-114">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="b413c-115">Ez a cikk bemutatja, hogyan hozhat létre és alkalmazhat Autopilot-profilokat az eszközökön a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="b413c-115">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="b413c-116">Ha még nem ismeri az Autopilot-t, tekintse át a következő cikkekben található információkat:</span><span class="sxs-lookup"><span data-stu-id="b413c-116">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="b413c-117">A Windows Autopilot áttekintése</span><span class="sxs-lookup"><span data-stu-id="b413c-117">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="b413c-118">Útmutató a robotpilóta üzembe helyezéséhez</span><span class="sxs-lookup"><span data-stu-id="b413c-118">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="b413c-119">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="b413c-119">Overview</span></span>

<span data-ttu-id="b413c-120">A Windows Autopilot szolgáltatással a partner Centerben egyéni profilokat hozhat létre az ügyfél-eszközökre való alkalmazáshoz.</span><span class="sxs-lookup"><span data-stu-id="b413c-120">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="b413c-121">A cikk közzétételének időpontjában a következő Profilbeállítások voltak elérhetők:</span><span class="sxs-lookup"><span data-stu-id="b413c-121">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="b413c-122">Adatvédelmi beállítások kihagyása.</span><span class="sxs-lookup"><span data-stu-id="b413c-122">Skip privacy settings.</span></span> <span data-ttu-id="b413c-123">Ez a választható Autopilot-profil beállítása lehetővé teszi, hogy a szervezetek ne kérdezzenek adatvédelmi beállításokat az OOBE folyamat során.</span><span class="sxs-lookup"><span data-stu-id="b413c-123">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="b413c-124">Tiltsa le a helyi rendszergazdai fiók létrehozását az eszközön.</span><span class="sxs-lookup"><span data-stu-id="b413c-124">Disable local admin account creation on the device.</span></span> <span data-ttu-id="b413c-125">A szervezetek eldönthetik, hogy az eszközt beállító felhasználónak rendszergazdai hozzáféréssel kell rendelkeznie a folyamat befejeződése után.</span><span class="sxs-lookup"><span data-stu-id="b413c-125">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="b413c-126">Eszköz automatikus beállítása munkahelyi vagy iskolai rendszerhez.</span><span class="sxs-lookup"><span data-stu-id="b413c-126">Automatically set up device for work or school.</span></span> <span data-ttu-id="b413c-127">Az Autopilot szolgáltatásban regisztrált összes eszköz automatikusan figyelembe veszi a munkahelyi vagy iskolai eszközöket, ezért a rendszer nem kérdezi le ezt a kérdést az OOBE-folyamat során.</span><span class="sxs-lookup"><span data-stu-id="b413c-127">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="b413c-128">Hagyja ki a Cortana, a OneDrive és az OEM-regisztráció beállítási lapjait.</span><span class="sxs-lookup"><span data-stu-id="b413c-128">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="b413c-129">Az Autopilot-ben regisztrált összes eszköz automatikusan kihagyja ezeket a lapokat a kezdőélmény (OOBE) folyamat során.</span><span class="sxs-lookup"><span data-stu-id="b413c-129">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="b413c-130">Végfelhasználói licencszerződés (EULA) kihagyása.</span><span class="sxs-lookup"><span data-stu-id="b413c-130">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="b413c-131">A Windows 10 1709-es verziójától kezdve a szervezetek dönthetnek úgy, hogy kihagyják az OOBE folyamat során bemutatott EULA-oldalt.</span><span class="sxs-lookup"><span data-stu-id="b413c-131">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="b413c-132">Tekintse meg a [Windows Autopilot végfelhasználói licencszerződését](#windows-autopilot-eula-dismissal) , amely fontos információkat nyújt a végfelhasználói licencszerződés oldalának a Windows telepítőben való kihagyása során.</span><span class="sxs-lookup"><span data-stu-id="b413c-132">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="b413c-133">Az alábbi profil- és eszközfelügyeleti engedélyek és korlátozások érvényesek:</span><span class="sxs-lookup"><span data-stu-id="b413c-133">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="b413c-134">A CSP-partnerek továbbra is felügyelhetik az Autopilot-profilokat azon meglévő ügyfelek esetében, akikkel viszonteladói kapcsolatban vannak, még akkor is, ha az ügyfelek eltávolították a partner delegált rendszergazdai jogosultságait.</span><span class="sxs-lookup"><span data-stu-id="b413c-134">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="b413c-135">Felügyelheti az Ön által hozzáadott ügyfelek meglévő eszközeit.</span><span class="sxs-lookup"><span data-stu-id="b413c-135">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="b413c-136">Nem felügyelhet olyan eszközöket, amelyeket az ügyfél töltött fel a Microsoft Store Vállalatoknak áruházba vagy a Microsoft Intune-portálra.</span><span class="sxs-lookup"><span data-stu-id="b413c-136">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="b413c-137">Autopilot-profilok létrehozása és kezelése a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="b413c-137">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="b413c-138">A partner Centerben létrehozhat Windows Autopilot Deployment-profilokat, és alkalmazhatja azokat az eszközökre.</span><span class="sxs-lookup"><span data-stu-id="b413c-138">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="b413c-139">Csak rendszergazdai ügynökök hozhatnak létre és alkalmazhatnak profilokat.</span><span class="sxs-lookup"><span data-stu-id="b413c-139">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="b413c-140">Új Autopilot-profil létrehozása</span><span class="sxs-lookup"><span data-stu-id="b413c-140">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="b413c-141">Válassza ki az **ügyfelek** elemet a partner központ menüben, majd válassza ki azt az ügyfelet, amelyhez az Autopilot-profilt létrehozza.</span><span class="sxs-lookup"><span data-stu-id="b413c-141">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="b413c-142">Az ügyfél részletei lapon válassza az **eszközök** elemet.</span><span class="sxs-lookup"><span data-stu-id="b413c-142">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="b413c-143">A **Windows Autopilot-profilok** területen válassza az **új profil hozzáadása** elemet.</span><span class="sxs-lookup"><span data-stu-id="b413c-143">Under **Windows Autopilot profiles** select **Add new profile** .</span></span>

4. <span data-ttu-id="b413c-144">Adja meg a profil nevét és leírását, majd konfigurálja az OOBE beállításait.</span><span class="sxs-lookup"><span data-stu-id="b413c-144">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="b413c-145">A következő lehetőségek közül választhat:</span><span class="sxs-lookup"><span data-stu-id="b413c-145">Choose from:</span></span>  

   - <span data-ttu-id="b413c-146">Adatvédelmi beállítások kihagyása a telepítőben</span><span class="sxs-lookup"><span data-stu-id="b413c-146">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="b413c-147">Helyi rendszergazdai fiók letiltása a telepítőben</span><span class="sxs-lookup"><span data-stu-id="b413c-147">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="b413c-148">Lapok automatikus kihagyása a telepítőben</span><span class="sxs-lookup"><span data-stu-id="b413c-148">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="b413c-149">( *Automatikusan kiválasztja a munkahelyi vagy iskolai telepítést* , és *kihagyhatja a Cortana, a ONEDRIVE és az OEM-regisztráció beállítási lapjait* )</span><span class="sxs-lookup"><span data-stu-id="b413c-149">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages* )</span></span>
  
   - <span data-ttu-id="b413c-150">Végfelhasználói licencszerződés (EULA) kihagyása</span><span class="sxs-lookup"><span data-stu-id="b413c-150">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="b413c-151">Tekintse meg a [Windows Autopilot végfelhasználói licencszerződését](#windows-autopilot-eula-dismissal) , amely fontos információkat nyújt a végfelhasználói licencszerződés oldalának a Windows telepítőben való kihagyása során.</span><span class="sxs-lookup"><span data-stu-id="b413c-151">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="b413c-152">Ha elkészült, válassza a **Küldés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b413c-152">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="b413c-153">Autopilot-profil alkalmazása az ügyfelek eszközeire</span><span class="sxs-lookup"><span data-stu-id="b413c-153">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="b413c-154">Az alábbi utasítások feltételezik, hogy már hozzáadta az ügyfél eszközeit a partner központhoz, és hozzáfér az eszközök listájához.</span><span class="sxs-lookup"><span data-stu-id="b413c-154">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="b413c-155">Ha még nem adta hozzá az ügyfél eszközeit, kövesse az [eszközök hozzáadása az ügyfél fiókjához](#add-devices-to-a-customers-account) című témakör utasításait, majd kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="b413c-155">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="b413c-156">Miután létrehozott egy Autopilot-profilt az ügyfél számára, azt alkalmazhatja az ügyfél eszközeire.</span><span class="sxs-lookup"><span data-stu-id="b413c-156">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="b413c-157">Válassza ki az **ügyfelek** elemet a partner központ menüből, majd válassza ki azt az ügyfelet, amelyhez az Autopilot-profilt létrehozta.</span><span class="sxs-lookup"><span data-stu-id="b413c-157">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="b413c-158">Az ügyfél részletei lapon válassza az **eszközök** elemet.</span><span class="sxs-lookup"><span data-stu-id="b413c-158">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="b413c-159">A **profilok alkalmazása az eszközökre** területen válassza ki azokat az eszközöket vagy eszközöket, amelyekhez profilt kíván hozzáadni, majd válassza a **profil alkalmazása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b413c-159">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile** .</span></span> <span data-ttu-id="b413c-160">Az imént alkalmazott profil megjelenik a **profil** oszlopban.</span><span class="sxs-lookup"><span data-stu-id="b413c-160">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="b413c-161">Az alábbi lépéseket követve ellenőrizheti, hogy a profil alkalmazása sikeres lesz-e az eszközön.</span><span class="sxs-lookup"><span data-stu-id="b413c-161">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="b413c-162">a.</span><span class="sxs-lookup"><span data-stu-id="b413c-162">a.</span></span>  <span data-ttu-id="b413c-163">Csatlakoztasson egy eszközt a hálózathoz, és kapcsolja be.</span><span class="sxs-lookup"><span data-stu-id="b413c-163">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="b413c-164">b.</span><span class="sxs-lookup"><span data-stu-id="b413c-164">b.</span></span>  <span data-ttu-id="b413c-165">Ellenőrizze, hogy megjelenik-e a megfelelő OOBE-képernyők (ha vannak ilyenek).</span><span class="sxs-lookup"><span data-stu-id="b413c-165">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="b413c-166">c.</span><span class="sxs-lookup"><span data-stu-id="b413c-166">c.</span></span>  <span data-ttu-id="b413c-167">Ha az OOBE-folyamat leáll, állítsa alaphelyzetbe az eszközt a gyári alapértelmezett beállításokkal, és készítse elő azt egy új felhasználó számára.</span><span class="sxs-lookup"><span data-stu-id="b413c-167">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="b413c-168">Autopilot-profil eltávolítása az ügyfél eszközéről</span><span class="sxs-lookup"><span data-stu-id="b413c-168">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="b413c-169">Válassza ki az **ügyfelek** elemet a partner központ menüből, majd válassza ki azt az ügyfelet, amelyhez az Autopilot-profilt létrehozta.</span><span class="sxs-lookup"><span data-stu-id="b413c-169">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="b413c-170">Az ügyfél részletei lapon válassza az **eszközök** elemet.</span><span class="sxs-lookup"><span data-stu-id="b413c-170">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="b413c-171">A **profilok alkalmazása az eszközökre** területen válassza ki azokat az eszközöket, amelyekről el szeretné távolítani a profilt, majd válassza a **profil eltávolítása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b413c-171">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile** .</span></span>

   >[!NOTE]
   ><span data-ttu-id="b413c-172">Ha eltávolít egy profilt egy eszközről, a rendszer nem törli a profilt a listából.</span><span class="sxs-lookup"><span data-stu-id="b413c-172">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="b413c-173">Ha törölni szeretne egy profilt, kövesse az [Autopilot-profil frissítése vagy törlése](#update-or-delete-an-autopilot-profile)című témakör utasításait.</span><span class="sxs-lookup"><span data-stu-id="b413c-173">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="b413c-174">Autopilot-profil frissítése vagy törlése</span><span class="sxs-lookup"><span data-stu-id="b413c-174">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="b413c-175">Ha egy ügyfél szeretné módosítani a beépített felhasználói élményt az eszközök számukra való elszállítása után, módosíthatja a profilt a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="b413c-175">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="b413c-176">Amikor az ügyfél eszköze csatlakozik az internethez, az a legújabb profilt fogja letölteni az OOBE folyamat során.</span><span class="sxs-lookup"><span data-stu-id="b413c-176">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="b413c-177">Továbbá, amikor egy ügyfél visszaállítja az eszközt a gyári alapértelmezett beállításokra, az eszköz újra letölti a legújabb profilt az OOBE folyamat során.</span><span class="sxs-lookup"><span data-stu-id="b413c-177">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="b413c-178">Válassza az **ügyfelek** lehetőséget a partner központ menüben, majd válassza ki azt az ügyfelet, aki szeretné módosítani az Autopilot-profilt.</span><span class="sxs-lookup"><span data-stu-id="b413c-178">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="b413c-179">Az ügyfél részletei lapon válassza az **eszközök** elemet.</span><span class="sxs-lookup"><span data-stu-id="b413c-179">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="b413c-180">A **Windows Autopilot-profilok** alatt válassza ki a frissíteni kívánt profilt.</span><span class="sxs-lookup"><span data-stu-id="b413c-180">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="b413c-181">Végezze el a szükséges módosításokat, majd kattintson a **Submit (Küldés** ) gombra.</span><span class="sxs-lookup"><span data-stu-id="b413c-181">Make the required changes and then select **Submit** .</span></span>

<span data-ttu-id="b413c-182">A profil törléséhez válassza a **Profil törlése** elemet a lap jobb felső sarkában.</span><span class="sxs-lookup"><span data-stu-id="b413c-182">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="b413c-183">Eszközök hozzáadása az ügyfél fiókjához</span><span class="sxs-lookup"><span data-stu-id="b413c-183">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="b413c-184">Az értékesítési ügynökök és a felügyeleti ügynökök hozzáadhatnak eszközöket az ügyfél fiókjához.</span><span class="sxs-lookup"><span data-stu-id="b413c-184">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="b413c-185">Ahhoz, hogy egyéni Autopilot-profilokat lehessen alkalmazni az ügyfél-eszközökre, el kell tudnia érni az ügyfél eszközének listáját.</span><span class="sxs-lookup"><span data-stu-id="b413c-185">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="b413c-186">Ha azt tervezi, hogy az OEM-név, a sorozatszám és a modell kombinációját használja, vegye figyelembe a következő korlátozásokat:</span><span class="sxs-lookup"><span data-stu-id="b413c-186">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="b413c-187">Ez a rekord csak az újabb eszközök (4k-kivonatok) esetében működik, és a 128B-kivonatok (RS2 és korábbi eszközök) esetében nem támogatott.</span><span class="sxs-lookup"><span data-stu-id="b413c-187">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="b413c-188">A rekord regisztrálása megkülönbözteti a kis-és nagybetűket, ezért a fájlban lévő adatoknak ***pontosan*** az OEM-szolgáltató (hardver szolgáltató) által biztosított modell-és gyártói neveket kell tartalmazniuk.</span><span class="sxs-lookup"><span data-stu-id="b413c-188">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="b413c-189">Kövesse az alábbi utasításokat, ha eszközöket szeretne hozzáadni az ügyfél fiókjához a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="b413c-189">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="b413c-190">Válassza az **ügyfelek** lehetőséget a partner központ menüben, majd válassza ki azt az ügyfelet, amelynek az eszközeit kezelni szeretné.</span><span class="sxs-lookup"><span data-stu-id="b413c-190">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="b413c-191">Az ügyfél részletei lapon válassza az **eszközök** elemet.</span><span class="sxs-lookup"><span data-stu-id="b413c-191">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="b413c-192">A **profilok alkalmazása eszközökön** válassza az **eszközök hozzáadása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b413c-192">Under **Apply profiles to devices** select **Add devices** .</span></span>

4. <span data-ttu-id="b413c-193">Adja meg az eszközök listájának nevét, majd kattintson a **Tallózás** gombra az ügyfél listájának (. csv fájlformátum) a partner központba való feltöltéséhez.</span><span class="sxs-lookup"><span data-stu-id="b413c-193">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="b413c-194">Ezt a. csv-fájlt az eszköz megvásárlásával kell megkapnia.</span><span class="sxs-lookup"><span data-stu-id="b413c-194">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="b413c-195">Ha nem kapott. csv fájlt, létrehozhat egyet saját maga az [eszközök hozzáadása a Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)szolgáltatáshoz című témakör lépéseit követve.</span><span class="sxs-lookup"><span data-stu-id="b413c-195">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="b413c-196">Töltse fel a. csv fájlt, majd kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="b413c-196">Upload the .csv file and then select **Save** .</span></span>

<span data-ttu-id="b413c-197">Ha a .csv fájl feltöltésekor hibaüzenetet kap, ellenőrizze a fájlformátumot.</span><span class="sxs-lookup"><span data-stu-id="b413c-197">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="b413c-198">Használhat csak hardverkivonatot, vagy az OEM-nevet, sorozatszámot és modellt (ebben az oszlopsorrendben), vagy a Windows-termékazonosítót.</span><span class="sxs-lookup"><span data-stu-id="b413c-198">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="b413c-199">Az **eszközök hozzáadása** elem melletti hivatkozásra kattintva a minta. csv fájlt is használhatja.</span><span class="sxs-lookup"><span data-stu-id="b413c-199">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="b413c-200">A CSV-fájlnak a következőhöz hasonlónak kell kinéznie:</span><span class="sxs-lookup"><span data-stu-id="b413c-200">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="b413c-201">**Eszköz sorozatszáma, Windows-termékazonosító, hardver-kivonat, gyártó neve, eszköz modellje**</span><span class="sxs-lookup"><span data-stu-id="b413c-201">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="b413c-202">**{serialNumber},,, Microsoft Corporation, Surface laptop**</span><span class="sxs-lookup"><span data-stu-id="b413c-202">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="b413c-203">A "gyártó neve" és az "eszköz modellje" megkülönbözteti a kis-és nagybetűket.</span><span class="sxs-lookup"><span data-stu-id="b413c-203">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="b413c-204">Ha nem tudja, hogy a gyártó neve és az eszköz modellje melyik értéket adja meg, a megfelelő értékek összegyűjtéséhez futtassa a következőt az eszközön:</span><span class="sxs-lookup"><span data-stu-id="b413c-204">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="b413c-205">Windows Autopilot EULA – elbocsátás</span><span class="sxs-lookup"><span data-stu-id="b413c-205">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="b413c-206">FONTOS INFORMÁCIÓK</span><span class="sxs-lookup"><span data-stu-id="b413c-206">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="b413c-207">A Windows Autopilot lehetővé teszi a Windows testreszabott telepítésének konfigurálását az ügyfelek számára felügyelt eszközökön.</span><span class="sxs-lookup"><span data-stu-id="b413c-207">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="b413c-208">Ha az ügyfél erre jogosult, letilthatja vagy elrejtheti a felhasználók számára általában a Windows beállításakor megjelenő olyan beállítási képernyőket, mint a végfelhasználói licencszerződés (végfelhasználói licencszerződés) elfogadási képernyője.</span><span class="sxs-lookup"><span data-stu-id="b413c-208">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="b413c-209">Ennek a funkciónak a használatával Ön vállalja, hogy letiltja vagy elrejti azokat a képernyőket, amelyek a feltételek bejelentését vagy elfogadását biztosítják a felhasználóknak továbbá, hogy az ügyfél nevében (akár egy szervezetnek, akár egy adott felhasználónak), beleegyezik a hirdetménybe, és elfogad minden olyan feltételt, amely az Ön ügyfelére érvényes.</span><span class="sxs-lookup"><span data-stu-id="b413c-209">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="b413c-210">Ez magában foglalja a licenchez tartozó használati feltételek és kikötések megkötését, ha az eszköz használatával nem szünteti meg vagy nem rejti el a felhasználót.</span><span class="sxs-lookup"><span data-stu-id="b413c-210">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="b413c-211">Előfordulhat, hogy az ügyfél nem használja a Windows szoftvert ezeken az eszközökön, ha az ügyfél a Microsofttól vagy a licencelt forgalmazótól kapott licenccel nem rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="b413c-211">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>