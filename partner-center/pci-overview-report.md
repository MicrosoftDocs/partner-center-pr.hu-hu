---
title: Partnerközpont Insights áttekintési irányítópultja
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pillanatképet készíthet arról, hogyan használja az értékesítést és az üzembe helyezést, az ügyfélnövekedést és a bevételnövekedést licencekkel, előfizetésekkel és az Azure-használattal.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14d280a65fa7c72ed382fd8b27e0354a4aa9e190
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120817"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>A Partnerközpont Insightsban elérhető Partnerközpont irányítópult-jelentések
 
**Megfelelő szerepkörök**

- Globális rendszergazda
- Rendszergazdai ügynök
- Jelentésmegjelenítő
- Vezetői jelentésmegjelenítő

Az Elemzések áttekintése irányítópult pillanatképet biztosít a fő teljesítménymutatókról, például az ügyfelekről, az előfizetésekről, az Azure consumption Revenue -ről és a Licencekről. A következő diagramokat az Áttekintés jelentésben ábrázolhatja.

- Összefoglalás  
- Az ügyfelek, előfizetések és licencek földrajzi eloszlése  
- Ügyfelek növekedési trendje 
- Előfizetések növekedési trendje 
- Az Azure felhasznált bevételnövekedési trendje 
- Licencnövekedési trend 

## <a name="summary"></a>Összefoglalás

Az Összefoglalás az ügyfelekkel, a Azure-viszonteladásból származó bevétel (ACR), az eladott előfizetésekkel, az aktív előfizetésekkel és az üzembe helyezett licencekkel kapcsolatos információkat tartalmaz. 

:::image type="content" source="images/pci/summary.png" alt-text="Összesítő licencek":::

Az Összefoglalás egyes szakaszokkal kapcsolatos további információk a következőkben találhatóak.

### <a name="customers"></a>Ügyfelek

Az **Ügyfelek** terület a következőket tartalmazza:

- A vállalathoz legalább egy aktív előfizetéssel társított ügyfelek aktuális száma különböző forrásmegjelölési típusokon és az összes felhőalapú terméken keresztül.
- Az ügyfelek százalékos növekedése a kiválasztott dátumtartományban.
- A mikrodiagram a kiválasztott dátumtartományon belüli ügyfélszám havi trendjét mutatja.

### <a name="azure-consumed-revenue-acr"></a>Azure-viszonteladásból származó bevétel (ACR)

Az **Azure-viszonteladásból származó bevétel (ACR)** terület a következőket tartalmazza:

- A Azure-viszonteladásból származó bevétel dátumtartományhoz rendelt összes Azure-viszonteladásból származó bevétel (USD-ban).
- A kijelölt dátumtartományhoz rendelt ACR százalékos növekedése vagy csökkenése (AZ USA $-ban).
- A mikrodiagram a kiválasztott dátumtartományhoz rendelt ACR US$ havi trendjét mutatja be 

> [!NOTE]
> Azure-viszonteladásból származó bevétel (ACR) adatai a Vezetői jelentésmegjelenítő szerepkörhöz rendelt felhasználók számára érhetők el 
 
### <a name="subscriptions-sold"></a>Eladott előfizetések

A **Summary (Összefoglalás) oldalon** található Subscriptions sold (Eladott előfizetések) terület a következőket tartalmazza:

- Az Ön által eladott vagy kezelt (aktív és inaktív) felhőalapú termék-előfizetések aktuális teljes száma.  
- Az előfizetések százalékos növekedése vagy csökkenése a kiválasztott dátumtartományban.
- A mikrodiagram az összes előfizetés havi trendjét mutatja a kiválasztott dátumtartományra.

### <a name="active-subscriptions"></a>Aktív előfizetések

Az **Összefoglalás területen az** Aktív előfizetések terület a következőket tartalmazza:

- A felhőalapú termék-előfizetések aktuális száma a termék-telemetria alapján mért aktív használattal. Ez az Azure-előfizetések esetében nem tartalmazza az összes próba-előfizetést.  
- Az aktív előfizetések százalékos növekedése a kiválasztott dátumtartományban.
- A mikrodiagram az aktív előfizetések havi trendjét mutatja a kiválasztott dátumtartományra.
 
### <a name="licenses-deployed"></a>Üzembe helyezett licencek

Az **Összefoglalás területen a** telepített licencek terület a következőket tartalmazza:
 
- Az ügyfél-előfizetésben üzembe helyezett összes felhőalapú terméklicenc száma a kiválasztott időszakban. 
- A licencek százalékos növekedése vagy csökkenése a kiválasztott dátumtartományban. 
- A mikrodiagram a hozzárendelt licencek számának havi trendjét jeleníti meg a kiválasztott dátumtartományban.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Az ügyfelek, előfizetések és licencek földrajzi eloszlése

Ez a nézet az összes ügyfél, előfizetés és licenc földrajzi eloszlása az ügyfél országa szerint. A különböző lapokat kiválasztva megtekintheti ezeket az elemzéseket a térképen. Megkeresheti és kiválaszthatja a rács egyik országát a térkép helyének nagyításához. A térképen a Kezdőlap gomb megnyomásával visszaállítható az eredeti nézet. Az egyes fülek (például ügyfelek, előfizetések) ikonra kattintva megjelenik az egyes országok metrikaértéke, valamint az ország teljes összegének százalékos értéke.  

:::image type="content" source="images/pci/geosummary.png" alt-text="Földrajzi összefoglalás":::

## <a name="customers-growth-trend"></a>Ügyfelek növekedési trendje

A kiválasztott dátumtartomány összes ügyfélszámának havi trendje. Az X tengely a kiválasztott dátumtartomány hónapját, az Y tengely pedig az adott hónap összes ügyfélszámát jelöli. 

:::image type="content" source="images/pci/customergrowth.png" alt-text="ügyfelek növekedési trendje":::

## <a name="subscriptions-growth-trend"></a>Előfizetések növekedési trendje

Ez jelzi az ügyfél-előfizetések számának trendjét a kiválasztott dátumtartományra. Az X tengely a kiválasztott dátumtartomány hónapjait, az Y tengely pedig a kiválasztott termék előfizetési számát jelöli. Görgessen végig a diagram tetején található csúszkán a diagram adott időszakra való nagyításhoz. 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="Előfizetés növekedési trendje":::

## <a name="azure-consumed-revenue-growth-trend"></a>Azure-viszonteladásból származó bevétel trend

Az Azure által a kiválasztott dátumtartományhoz rendelt, az Azure által felhasznált US$ bevétel havi trendje. Az X tengely a kiválasztott dátumtartomány hónapját jelöli, az Y tengely pedig az Azure teljes felhasznált bevételét (US$) az Ön számára a hónap során.

> [!NOTE]
> Azure-viszonteladásból származó bevétel (ACR) csak a Vezetői jelentésmegjelenítő szerepkörhöz rendelt felhasználók számára lesz látható. 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Azure-használat":::

## <a name="licenses-growth-trend"></a>Licencnövekedési trend
 
Az összes ügyfél által a kiválasztott dátumtartományon belül hozzárendelt licencek trendje. Az X tengely a kiválasztott dátumtartomány hónapjait, az Y tengely pedig a kiválasztott termék licencszámát jelöli. Görgessen végig a diagram tetején található csúszkán a diagram adott időszakra való nagyításhoz.  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="licencek":::

## <a name="next-steps"></a>Következő lépések

További jelentésekért lásd: [Partnerközpont Insights.](partner-center-insights.md)
