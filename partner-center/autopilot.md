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
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Windows Autopilot-profilok használata új eszközökön az ügyfél kezdőélményének testreszabásához

**A következőkre vonatkozik**

- CSP Direct – számlázási partnerek, közvetett szolgáltatók és közvetett viszonteladók

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Globális rendszergazda
- Értékesítési ügynök
- Felhasználói felügyeleti rendszergazda

Ha az ügyfeleket felügyeli, előfordulhat, hogy testre kell szabnia az ügyfél felhasználói számára a beépített (OOBE) élményt. Előre konfigurálhatja az új eszközöket a Windows Autopilot-profilokkal, mielőtt az eszközöket az ügyfeleknek kézbesíti, és új profilokat alkalmazzon az ügyfelek számára már megvásárolt eszközökre. 

Vegye figyelembe, hogy a számítógépgyártók megkezdték az eszköz **termékkulcs-azonosítóját (PKID)** megjelenítő, az Autopilot-eszközön kívüli szállítási címkét is.  Ez az 1 dimenziós, olvasható vonalkód olyan alsóbb szintű partnereket biztosít, amelyek lehetővé teszik, hogy az eszköz (ek) bevonása nélkül regisztrálják az eszközöket, és más módon betakarították az eszköz AZONOSÍTÓját.

Ez a cikk bemutatja, hogyan hozhat létre és alkalmazhat Autopilot-profilokat az eszközökön a partner Centerben.

Ha még nem ismeri az Autopilot-t, tekintse át a következő cikkekben található információkat:

- [A Windows Autopilot áttekintése](/windows/deployment/windows-10-auto-pilot)
- [Útmutató a robotpilóta üzembe helyezéséhez](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Áttekintés

A Windows Autopilot szolgáltatással a partner Centerben egyéni profilokat hozhat létre az ügyfél-eszközökre való alkalmazáshoz. A cikk közzétételének időpontjában a következő Profilbeállítások voltak elérhetők:

- Adatvédelmi beállítások kihagyása. Ez a választható Autopilot-profil beállítása lehetővé teszi, hogy a szervezetek ne kérdezzenek adatvédelmi beállításokat az OOBE folyamat során.

- Tiltsa le a helyi rendszergazdai fiók létrehozását az eszközön. A szervezetek eldönthetik, hogy az eszközt beállító felhasználónak rendszergazdai hozzáféréssel kell rendelkeznie a folyamat befejeződése után.

- Eszköz automatikus beállítása munkahelyi vagy iskolai rendszerhez. Az Autopilot szolgáltatásban regisztrált összes eszköz automatikusan figyelembe veszi a munkahelyi vagy iskolai eszközöket, ezért a rendszer nem kérdezi le ezt a kérdést az OOBE-folyamat során.

- Hagyja ki a Cortana, a OneDrive és az OEM-regisztráció beállítási lapjait. Az Autopilot-ben regisztrált összes eszköz automatikusan kihagyja ezeket a lapokat a kezdőélmény (OOBE) folyamat során.

- Végfelhasználói licencszerződés (EULA) kihagyása. A Windows 10 1709-es verziójától kezdve a szervezetek dönthetnek úgy, hogy kihagyják az OOBE folyamat során bemutatott EULA-oldalt. Tekintse meg a [Windows Autopilot végfelhasználói licencszerződését](#windows-autopilot-eula-dismissal) , amely fontos információkat nyújt a végfelhasználói licencszerződés oldalának a Windows telepítőben való kihagyása során.

Az alábbi profil- és eszközfelügyeleti engedélyek és korlátozások érvényesek:

- A CSP-partnerek továbbra is felügyelhetik az Autopilot-profilokat azon meglévő ügyfelek esetében, akikkel viszonteladói kapcsolatban vannak, még akkor is, ha az ügyfelek eltávolították a partner delegált rendszergazdai jogosultságait.

- Felügyelheti az Ön által hozzáadott ügyfelek meglévő eszközeit.

- Nem felügyelhet olyan eszközöket, amelyeket az ügyfél töltött fel a Microsoft Store Vállalatoknak áruházba vagy a Microsoft Intune-portálra.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Autopilot-profilok létrehozása és kezelése a partner Centerben

A partner Centerben létrehozhat Windows Autopilot Deployment-profilokat, és alkalmazhatja azokat az eszközökre.

>[!NOTE]
>Csak rendszergazdai ügynökök hozhatnak létre és alkalmazhatnak profilokat.

### <a name="create-a-new-autopilot-profile"></a>Új Autopilot-profil létrehozása

1. Válassza ki az **ügyfelek** elemet a partner központ menüben, majd válassza ki azt az ügyfelet, amelyhez az Autopilot-profilt létrehozza.

2. Az ügyfél részletei lapon válassza az **eszközök** elemet.

3. A **Windows Autopilot-profilok** területen válassza az **új profil hozzáadása** elemet.

4. Adja meg a profil nevét és leírását, majd konfigurálja az OOBE beállításait. A következő lehetőségek közül választhat:  

   - Adatvédelmi beállítások kihagyása a telepítőben

   - Helyi rendszergazdai fiók letiltása a telepítőben
  
   - Lapok automatikus kihagyása a telepítőben<br>
        ( *Automatikusan kiválasztja a munkahelyi vagy iskolai telepítést* , és *kihagyhatja a Cortana, a ONEDRIVE és az OEM-regisztráció beállítási lapjait* )
  
   - Végfelhasználói licencszerződés (EULA) kihagyása<br> 
       >[!IMPORTANT] 
       >Tekintse meg a [Windows Autopilot végfelhasználói licencszerződését](#windows-autopilot-eula-dismissal) , amely fontos információkat nyújt a végfelhasználói licencszerződés oldalának a Windows telepítőben való kihagyása során.

5. Ha elkészült, válassza a **Küldés** lehetőséget.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Autopilot-profil alkalmazása az ügyfelek eszközeire

>[!NOTE]
>Az alábbi utasítások feltételezik, hogy már hozzáadta az ügyfél eszközeit a partner központhoz, és hozzáfér az eszközök listájához. Ha még nem adta hozzá az ügyfél eszközeit, kövesse az [eszközök hozzáadása az ügyfél fiókjához](#add-devices-to-a-customers-account) című témakör utasításait, majd kövesse az alábbi lépéseket.

Miután létrehozott egy Autopilot-profilt az ügyfél számára, azt alkalmazhatja az ügyfél eszközeire.

1. Válassza ki az **ügyfelek** elemet a partner központ menüből, majd válassza ki azt az ügyfelet, amelyhez az Autopilot-profilt létrehozta.

2. Az ügyfél részletei lapon válassza az **eszközök** elemet.

3. A **profilok alkalmazása az eszközökre** területen válassza ki azokat az eszközöket vagy eszközöket, amelyekhez profilt kíván hozzáadni, majd válassza a **profil alkalmazása** lehetőséget. Az imént alkalmazott profil megjelenik a **profil** oszlopban.

4. Az alábbi lépéseket követve ellenőrizheti, hogy a profil alkalmazása sikeres lesz-e az eszközön.

    a.  Csatlakoztasson egy eszközt a hálózathoz, és kapcsolja be.

    b.  Ellenőrizze, hogy megjelenik-e a megfelelő OOBE-képernyők (ha vannak ilyenek).

    c.  Ha az OOBE-folyamat leáll, állítsa alaphelyzetbe az eszközt a gyári alapértelmezett beállításokkal, és készítse elő azt egy új felhasználó számára.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Autopilot-profil eltávolítása az ügyfél eszközéről

1. Válassza ki az **ügyfelek** elemet a partner központ menüből, majd válassza ki azt az ügyfelet, amelyhez az Autopilot-profilt létrehozta.

2. Az ügyfél részletei lapon válassza az **eszközök** elemet.

3. A **profilok alkalmazása az eszközökre** területen válassza ki azokat az eszközöket, amelyekről el szeretné távolítani a profilt, majd válassza a **profil eltávolítása** lehetőséget.

   >[!NOTE]
   >Ha eltávolít egy profilt egy eszközről, a rendszer nem törli a profilt a listából. Ha törölni szeretne egy profilt, kövesse az [Autopilot-profil frissítése vagy törlése](#update-or-delete-an-autopilot-profile)című témakör utasításait.

### <a name="update-or-delete-an-autopilot-profile"></a>Autopilot-profil frissítése vagy törlése

Ha egy ügyfél szeretné módosítani a beépített felhasználói élményt az eszközök számukra való elszállítása után, módosíthatja a profilt a partner Centerben.

Amikor az ügyfél eszköze csatlakozik az internethez, az a legújabb profilt fogja letölteni az OOBE folyamat során. Továbbá, amikor egy ügyfél visszaállítja az eszközt a gyári alapértelmezett beállításokra, az eszköz újra letölti a legújabb profilt az OOBE folyamat során.

1. Válassza az **ügyfelek** lehetőséget a partner központ menüben, majd válassza ki azt az ügyfelet, aki szeretné módosítani az Autopilot-profilt.

2. Az ügyfél részletei lapon válassza az **eszközök** elemet.

3. A **Windows Autopilot-profilok** alatt válassza ki a frissíteni kívánt profilt. Végezze el a szükséges módosításokat, majd kattintson a **Submit (Küldés** ) gombra.

A profil törléséhez válassza a **Profil törlése** elemet a lap jobb felső sarkában.

### <a name="add-devices-to-a-customers-account"></a>Eszközök hozzáadása az ügyfél fiókjához

>[!NOTE]
>Az értékesítési ügynökök és a felügyeleti ügynökök hozzáadhatnak eszközöket az ügyfél fiókjához.

Ahhoz, hogy egyéni Autopilot-profilokat lehessen alkalmazni az ügyfél-eszközökre, el kell tudnia érni az ügyfél eszközének listáját.

Ha azt tervezi, hogy az OEM-név, a sorozatszám és a modell kombinációját használja, vegye figyelembe a következő korlátozásokat:

- Ez a rekord csak az újabb eszközök (4k-kivonatok) esetében működik, és a 128B-kivonatok (RS2 és korábbi eszközök) esetében nem támogatott.

- A rekord regisztrálása megkülönbözteti a kis-és nagybetűket, ezért a fájlban lévő adatoknak ***pontosan*** az OEM-szolgáltató (hardver szolgáltató) által biztosított modell-és gyártói neveket kell tartalmazniuk.

Kövesse az alábbi utasításokat, ha eszközöket szeretne hozzáadni az ügyfél fiókjához a partner Centerben.

1. Válassza az **ügyfelek** lehetőséget a partner központ menüben, majd válassza ki azt az ügyfelet, amelynek az eszközeit kezelni szeretné.

2. Az ügyfél részletei lapon válassza az **eszközök** elemet.

3. A **profilok alkalmazása eszközökön** válassza az **eszközök hozzáadása** lehetőséget.

4. Adja meg az eszközök listájának nevét, majd kattintson a **Tallózás** gombra az ügyfél listájának (. csv fájlformátum) a partner központba való feltöltéséhez.

    >[!NOTE]
    >Ezt a. csv-fájlt az eszköz megvásárlásával kell megkapnia. Ha nem kapott. csv fájlt, létrehozhat egyet saját maga az [eszközök hozzáadása a Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)szolgáltatáshoz című témakör lépéseit követve.  

5. Töltse fel a. csv fájlt, majd kattintson a **Mentés** gombra.

Ha a .csv fájl feltöltésekor hibaüzenetet kap, ellenőrizze a fájlformátumot. Használhat csak hardverkivonatot, vagy az OEM-nevet, sorozatszámot és modellt (ebben az oszlopsorrendben), vagy a Windows-termékazonosítót. Az **eszközök hozzáadása** elem melletti hivatkozásra kattintva a minta. csv fájlt is használhatja.

A CSV-fájlnak a következőhöz hasonlónak kell kinéznie:

> **Eszköz sorozatszáma, Windows-termékazonosító, hardver-kivonat, gyártó neve, eszköz modellje**

> **{serialNumber},,, Microsoft Corporation, Surface laptop**

>[!NOTE]
> A "gyártó neve" és az "eszköz modellje" megkülönbözteti a kis-és nagybetűket.

Ha nem tudja, hogy a gyártó neve és az eszköz modellje melyik értéket adja meg, a megfelelő értékek összegyűjtéséhez futtassa a következőt az eszközön:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA – elbocsátás

### <a name="important-information"></a>FONTOS INFORMÁCIÓK

A Windows Autopilot lehetővé teszi a Windows testreszabott telepítésének konfigurálását az ügyfelek számára felügyelt eszközökön. Ha az ügyfél erre jogosult, letilthatja vagy elrejtheti a felhasználók számára általában a Windows beállításakor megjelenő olyan beállítási képernyőket, mint a végfelhasználói licencszerződés (végfelhasználói licencszerződés) elfogadási képernyője.

Ennek a funkciónak a használatával Ön vállalja, hogy letiltja vagy elrejti azokat a képernyőket, amelyek a feltételek bejelentését vagy elfogadását biztosítják a felhasználóknak továbbá, hogy az ügyfél nevében (akár egy szervezetnek, akár egy adott felhasználónak), beleegyezik a hirdetménybe, és elfogad minden olyan feltételt, amely az Ön ügyfelére érvényes. Ez magában foglalja a licenchez tartozó használati feltételek és kikötések megkötését, ha az eszköz használatával nem szünteti meg vagy nem rejti el a felhasználót. Előfordulhat, hogy az ügyfél nem használja a Windows szoftvert ezeken az eszközökön, ha az ügyfél a Microsofttól vagy a licencelt forgalmazótól kapott licenccel nem rendelkezik.