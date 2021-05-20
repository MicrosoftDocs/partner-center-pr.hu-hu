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
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Windows Autopilot-profilok használata új eszközökön az ügyfél kezdőélményének testreszabásához

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Globális rendszergazdai | Értékesítési ügynök | Felhasználókezelő rendszergazda

Ha ügyféleszközöket felügyel, előfordulhat, hogy testre kell szabni a felhasználói élményt (OOBE). Az új eszközöket előre konfigurálhatja Windows Autopilot profilokkal, mielőtt az eszközöket az ügyfeleknek szállítja, és új profilokat alkalmazhat az ügyfelek által már megvásárolt eszközökre. 

Vegye figyelembe, hogy az EM-ek elkezdték az Autopilot-eszközdobozon kívüli fuvarlevélcímkét is, amely megjeleníti az eszköz termékkulcs-azonosítóját **(PKID).**  Ez az egydimenziós, olvasható vonalkód lehetővé teszi az lefelé irányuló partnerek számára, hogy anélkül regisztrálják az eszközöket az Autopilotra, hogy le kell mondaniuk az eszköz(ük)ről, és alternatív módszerrel be kell gyűjteni az eszközazonosítót.

Ez a cikk bemutatja, hogyan hozhat létre és alkalmazhat AutoPilot-profilokat a Partnerközpont.

Ha még nem ismeri az Autopilotot, tekintse át az alábbi cikkekben található információkat:

- [A Windows Autopilot áttekintése](/windows/deployment/windows-10-auto-pilot)
- [Útmutató az Autopilot üzembe helyezéséhez](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Áttekintés

A Windows Autopilot funkcióval Partnerközpont egyéni profilokat hozhat létre az ügyféleszközökre való alkalmazáshoz. A cikk közzétételekor a következő profilbeállítások voltak elérhetők:

- Hagyja ki az adatvédelmi beállításokat. Ez a választható Autopilot-profilbeállítás lehetővé teszi, hogy a szervezetek ne kérdezzenek az adatvédelmi beállításokról az OOBE folyamat során.

- Tiltsa le a helyi rendszergazdai fiók létrehozását az eszközön. A szervezetek eldöntheti, hogy az eszközt berakó felhasználó rendszergazdai hozzáféréssel rendelkezik-e a folyamat befejezése után.

- Az eszköz automatikus beállítása munkahelyi vagy iskolai alkalmazáshoz. Az Autopilotban regisztrált összes eszköz automatikusan munkahelyi vagy iskolai eszköznek minősül, ezért ezt a kérdést a rendszer nem fogja feltetetni az OOBE folyamat során.

- A Cortana,a OneDrive és az OEM regisztrációs oldalának kihagyása. Az Autopilottal regisztrált összes eszköz automatikusan kihagyja ezeket az oldalakat a be nem lépő felhasználói élmény (OOBE) folyamata során.

- Hagyja ki a végfelhasználói licencszerződést (EULA). A Windows 10 1709-es verziójától kezdődően a szervezetek dönthetnek úgy, hogy kihagyják az OOBE folyamat során bemutatott EULA oldalt. A [Windows Autopilot eula dismissal (A EULA](#windows-autopilot-eula-dismissal) elvetését lásd alább) oldalon fontos információkat olvashat a EULA oldal kihagyásával kapcsolatban a Windows beállítása során.

Az alábbi profil- és eszközfelügyeleti engedélyek és korlátozások érvényesek:

- A CSP-partnerek továbbra is felügyelhetik az Autopilot-profilokat azon meglévő ügyfelek esetében, akikkel viszonteladói kapcsolatban vannak, még akkor is, ha az ügyfelek eltávolították a partner delegált rendszergazdai jogosultságait.

- Felügyelheti az Ön által hozzáadott ügyfelek meglévő eszközeit.

- Nem felügyelhet olyan eszközöket, amelyeket az ügyfél töltött fel a Microsoft Store Vállalatoknak áruházba vagy a Microsoft Intune-portálra.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>AutoPilot-profilok létrehozása és kezelése a Partnerközpont

A Partnerközpont létrehozhat telepítési Windows Autopilot profilokat, és alkalmazhatja őket az eszközökre.

>[!NOTE]
>Profilokat csak rendszergazdai ügynökök hozhatnak létre és alkalmazhatnak.

### <a name="create-a-new-autopilot-profile"></a>Új AutoPilot-profil létrehozása

1. Válassza **az Ügyfelek** Partnerközpont menüből, majd válassza ki azt az ügyfelet, aki számára létrehozza az Autopilot-profilt.

2. Az ügyfél részletek lapján válassza az Eszközök **lehetőséget.**

3. A **Windows Autopilot profilok alatt válassza** az Új profil hozzáadása **lehetőséget.**

4. Adja meg a profil nevét és leírását, majd konfigurálja az OOBE-beállításokat. A következő lehetőségek közül választhat:  

   - Az adatvédelmi beállítások kihagyása a telepítőben

   - Helyi rendszergazdai fiók letiltása a telepítőben
  
   - Oldalak automatikus kihagyása a telepítőben<br>
        (Tartalmazza *a munkahelyi vagy iskolai beállítások* automatikus kiválasztását és a Cortana, a OneDrive és az OEM regisztrációs *oldalának kihagyása adatokat)*
  
   - Végfelhasználói licencszerződés (EULA) kihagyása<br> 
       >[!IMPORTANT] 
       >A [Windows Autopilot eula dismissal (A EULA](#windows-autopilot-eula-dismissal) elvetését lásd alább) oldalon fontos információkat olvashat a EULA oldal kihagyásával kapcsolatban a Windows beállítása során.

5. Ha **elkészült, válassza** a Küldés lehetőséget.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Autopilot-profil alkalmazása az ügyféleszközökre

>[!NOTE]
>Az alábbi utasítások feltételezik, hogy már hozzáadta az ügyfél eszközeit a Partnerközpont, és hozzáférhet az eszközlistához. Ha még nem adott hozzá az ügyfél eszközeit, [](#add-devices-to-a-customers-account) kövesse az Eszközök hozzáadása az ügyfél fiókjához lépéseit, majd kövesse az alábbi lépéseket.

Miután létrehozott egy AutoPilot-profilt egy ügyfél számára, alkalmazhatja azt az ügyfél eszközeire.

1. Válassza **az Ügyfelek** Partnerközpont menüből, majd válassza ki azt az ügyfelet, aki számára létrehozta az AutoPilot-profilt.

2. Az ügyfél részletek lapján válassza az Eszközök **lehetőséget.**

3. A **Profilok alkalmazása eszközökre alatt** válassza ki azokat az eszközöket vagy eszközcsoportokat, amelyekhez profilokat kíván hozzáadni, majd válassza a Profil alkalmazása **lehetőséget.** Az előbb alkalmazott profil megjelenik a **Profil oszlopban.**

4. Kövesse az alábbi lépéseket annak ellenőrzéséhez, hogy a profil sikeresen alkalmazva lesz-e az eszközön.

    a.  Csatlakoztassa az eszközt a hálózathoz, és kapcsolja be.

    b.  Ellenőrizze, hogy megjelennek-e a megfelelő OOBE-képernyők (ha vannak).

    c.  Ha az OOBE folyamat leáll, állítsa vissza az eszközt a gyári alapértelmezett beállításokra, hogy előkészítse egy új felhasználó számára.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>AutoPilot-profil eltávolítása az ügyfél eszközéről

1. Válassza **az Ügyfelek** Partnerközpont menüből, majd válassza ki azt az ügyfelet, aki számára létrehozta az AutoPilot-profilt.

2. Az ügyfél részletek lapján válassza az Eszközök **lehetőséget.**

3. A **Profilok alkalmazása eszközökre alatt** válassza ki azokat az eszközöket, amelyekről el szeretné távolítani a profilt, majd válassza a Profil eltávolítása **lehetőséget.**

   >[!NOTE]
   >Egy profil eszközről való eltávolítása nem törli a profilt a listából. Ha törölni szeretne egy profilt, kövesse az [AutoPilot-profil](#update-or-delete-an-autopilot-profile)frissítésére vagy törlésére vonatkozó utasításokat.

### <a name="update-or-delete-an-autopilot-profile"></a>AutoPilot-profil frissítése vagy törlése

Ha egy ügyfél módosítani szeretné a már nem használható eszközöket, miután Ön kiszállította őket, a profilt a következő Partnerközpont.

Amikor az ügyfél eszköze csatlakozik az internethez, letölti a legújabb profilverziót az OOBE folyamat során. Emellett minden alkalommal, amikor egy ügyfél visszaállít egy eszközt az alapértelmezett gyári beállításokra, az eszköz az OOBE folyamat során ismét letölti a legújabb profilverziót.

1. Válassza **az Ügyfelek** Partnerközpont menüből, majd válassza ki azt az ügyfelet, aki módosítani szeretné az AutoPilot-profilt.

2. Az ügyfél részletek lapján válassza az Eszközök **lehetőséget.**

3. A **Windows Autopilot profilok alatt** válassza ki a frissíteni kívánt profilt. Tegye meg a szükséges módosításokat, majd válassza a **Küldés lehetőséget.**

A profil törléséhez válassza a **Profil** törlése lehetőséget az oldal jobb felső sarkában.

### <a name="add-devices-to-a-customers-account"></a>Eszközök hozzáadása az ügyfél fiókjához

>[!NOTE]
>Az értékesítési ügynökök és a rendszergazdai ügynökök eszközöket adhatnak az ügyfél fiókjához.

Mielőtt egyéni Autopilot-profilokat alkalmazhat az ügyféleszközökre, hozzá kell férnie az ügyfél eszközlistához.

Ha oem-nevet, sorozatszámot és modellkombinációt tervez használni, vegye figyelembe az alábbi korlátozásokat:

- Ez a rekord csak újabb eszközök esetében működik (például 4k-os hashes), és nem támogatott 128b-os (RS2- és korábbi) eszközökhöz.

- A rekordregisztráció megkülönbözteti a kis- és nagybetűket, ezért  a fájlban szereplő adatoknak pontosan az OEM-szolgáltató (hardverszolgáltató) által megadott modell- és gyártónevekkel kell megegyeznie.

Kövesse az alábbi utasításokat, ha eszközöket szeretne hozzáadni egy ügyfél fiókjához a Partnerközpont.

1. Válassza **az Ügyfelek** Partnerközpont, majd válassza ki azt az ügyfelet, akinek az eszközeit kezelni szeretné.

2. Az ügyfél részletek lapján válassza az Eszközök **lehetőséget.**

3. A Profilok **alkalmazása eszközökre alatt válassza** az Eszközök hozzáadása **lehetőséget.**

4. Adja meg az eszközlista nevét, majd a Tallózás gombra kattintva töltse fel az ügyfél listáját (.csv fájlformátumban) Partnerközpont. 

    >[!NOTE]
    >Ezt a .csv-fájlt az eszköz megvásárlásakor kellett megkapni. Ha nem kapott .csv-fájlt, létrehozhat egyet saját maga is az [Eszközök](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)hozzáadása a fájlhoz Windows Autopilot.  

5. Töltse fel a .csv-fájlt, majd válassza a **Mentés lehetőséget.**

Ha a .csv fájl feltöltésekor hibaüzenetet kap, ellenőrizze a fájlformátumot. Használhat csak hardverkivonatot, vagy az OEM-nevet, sorozatszámot és modellt (ebben az oszlopsorrendben), vagy a Windows-termékazonosítót. Eszközlista létrehozásához használhatja az Eszközök hozzáadása melletti  hivatkozásból származó .csv-mintafájlt is.

A .csv-fájlnak így kell kinéznie:

> **Eszköz sorozatszáma,Windows-termékazonosító,Hardver kivonata,Gyártó neve,Eszközmodell**

> **{serialNumber},,,Microsoft Corporation,Surface Laptop**

>[!NOTE]
> A "Gyártó neve" és az "Eszközmodell" megkülönbözteti a kis- és nagybetűket.

Ha nem tudja, hogy milyen értéket kell tenni a Gyártó neve és az Eszközmodell mezőben, ezt az eszközön futtatva összegyűjtheti a megfelelő értékeket:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA elvetését

### <a name="important-information"></a>FONTOS INFORMÁCIÓK

Windows Autopilot segítségével testreszabott Windows-telepítéseket konfigurálhatja az ügyfelek számára ön által felügyelt eszközökön. Ha az ügyfél erre jogosult, letilthat vagy elrejthet bizonyos beállítási képernyőket, amelyek általában jelennek meg a felhasználók számára a Windows beállításakor, beleértve a végfelhasználói licencszerződés (EULA) elfogadási képernyőjét.

A függvény használatával Ön beleegyezik abba, hogy a feltételek elfogadására vagy elfogadására tervezett képernyők mellőzése vagy elrejtése azt jelenti, hogy megfelelő beleegyezést és engedélyt szerzett az ügyféltől a feltételek elrejtéséhez, és Hogy Ön az ügyfél nevében (akár egy szervezet, akár adott esetben egy egyéni felhasználó) elfogadja az értesítéseket, és elfogadja az ügyfélre vonatkozó feltételeket. Ebbe beletartozik a licenc használati feltételeinek vagy az értesítésnek a szerződése, amely akkor jelenne meg a felhasználó számára, ha nem tiltja le vagy rejti el az eszközt használva. Az ügyfél nem használhatja a Windows-szoftvert ezen eszközökön, ha az ügyfél nem szerzett érvényes licencet a szoftverhez a Microsofttól vagy annak licencelt forgalmazóitól.