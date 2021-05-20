---
title: Azure-csomag számlázása – számla & recon fájlok
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan férhet hozzá az Azure-csomag számlázásához kapcsolódó számla- és egyeztetési fájlstruktúrához, és hogyan értheti meg azt.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ab086a4d15d16f094e33d19b81f1c93711916dc
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201425"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Új kereskedelmi felület a CSP-ben – Azure-számlázás 

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Globális rendszergazda

Ez a cikk bemutatja, hogyan férhet hozzá az Azure-csomag számlázásához kapcsolódó számla- és egyeztetési fájlstruktúrához, és hogyan értheti meg azt. Az Azure-csomag szerinti számlázás egy egyszerűsített számlázási élmény, amely egy igazított egy számlázási dátumon és naptári hónapalapú számlázási időszakon alapul.

## <a name="summary-of-billing-essentials"></a>A számlázás alapvető adatainak összefoglalása

- **Számla dátuma:** A számla és az egyeztetési fájl a következő időpontig Partnerközpont (UTC) éjfélig lesz elérhető az irányítópulton/API-n.

- **Számlázási időszak:** A számla számlázási időszaka a naptári hónaphoz van igazítva, például: 10/1-10/31, 11/1-11/30.

- **Díjak szolgáltatási időszaka:** A díjak a naptári hónaphoz igazodnak. Ha például a kiszámlázott partner 10/15-én azure-csomagon keresztül ad hozzá Azure-szolgáltatásokat, és az ügyfél 10/15-én kezdi meg az Azure-szolgáltatások használatának elkezdét, akkor a számlázott partner a 10/15–31 szolgáltatási időszak ügyfélfelhasználása alapján a 11/10/31-es időszakban kapja meg a számlát/felderítést. A következő hónap 12/8-án generált számlája a 11/1– 11/31 szolgáltatási időszak összes díját tartalmazza.

- **Számlás fizetési időszak:** Net 60 nap.

- **Számla** pénzneme: 2021. január 28-tól az EU/EFTA és az Egyesült Királyság régió azon partnerei, akik új ügyfelekkel és meglévő CSP-ügyfelekkel vásárolnak új kereskedelmi ajánlatokat 2020. május 11. előtt először, a partnerhelyi pénznemben számlázjuk ki a vásárlásokat. Az EU-n/EFTA-n és az Egyesült Királyságon kívüli partnerek számlázása továbbra is partneri pénznemben történik.

- **Partneri ösztönzők:** A számlázási hónap végével fizetett 45 nap.

## <a name="access-your-invoices-and-reconciliation-files"></a>Hozzáférés a számlákhoz és az egyeztetési fájlokhoz

A vállalat globális rendszergazdája vagy számlázási rendszergazdája e-mailt kap, ha a számla készen áll a megtekintésre.

A számla és az egyeztetési fájl elérése:

1. Jelentkezzen be a Partnerközpont [irányítópultjába](https://partner.microsoft.com/dashboard/).

2. A Partnerközpont válassza a Számlázás **lehetőséget.**

3. Válassza a Recurring (Ismétlődő) **és** **az One-time (Egyszeri) lapfület,** valamint a kívánt pénznemet.

   :::image type="content" source="images/azure/billing3.png" alt-text="Számlázási":::

4. Válassza **a Számla** vagy az **Egyeztetési fájl lehetőséget.**  

   Az előzményszámlák és a recon-fájlok megtekintéséhez bontsa ki az alábbi Számlázási előzmények sort.

## <a name="understanding-usage-data"></a>A használati adatok ismertetése 

1. Az Azure-csomag a használat legfelső szintű vagy legfelső szintű tárolója. Minden használat egyetlen Azure-csomaghoz kötődik.

2. Egy csomagon belül egy vagy több Azure-előfizetés lesz. Ezek erőforrás-kezeléshez és üzembe helyezéshez használt tárolók. 

3. Az előfizetésen belül az erőforráscsoportok hozzáadhatók az erőforrások csoportosításához. Minden erőforrás egy erőforráscsoportba van telepítve. 

4. Ilyen erőforrás például a virtuális gépek és a tárfiókok. 

5. Erőforrás-kibocsátó mérők: A fogyasztásmérők egy erőforrás fogyasztásának mérései, és egy erőforrás több mérőre is kibocsáthat használatot. A mérőket egy Termékazonosító, SKUId és AvailabilityId azonosítja. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Az előfizetési erőforráscsoportok és a mérés hierarchiája

**Azure-fiók (bérlő)**

- A előfizetés
    - ResourceGroup 1
        - Virtuális gép (erőforrás)
            - Számítási fogyasztásmérő
        - Virtuális hálózat (erőforrás)
            - Nincs számlázási mérő

    - ResourceGroup 2
        - Virtuális gép (erőforrás)
            - Számítógép-fogyasztásmérő
        - prémium SSD lemez (erőforrás)
            - Tárolókapacitás-mérő
            - Tárolási műveletek mérő

- B előfizetés –ResourceGroup 1 – Azure SQL (erőforrás) – DTU-mérő – VPN Gateway (erőforrás) – VPN-átjáró mérő

    - ResourceGroup 2
        - Virtual Network felület (erőforrás)
            - Nincs számlázási mérő

## <a name="read-the-invoice"></a>A számla olvasása

1. A számla csak az egyes hónap első napján lesz elérhető.

2. A partnereknek 60 napjuk van a kifizetés visszafizetésére.

3. A számlázási időszak egy adott naptári hónapot fed le, például 10.1.10.31.

4. A díjak a kiigazítások nettó összege (az összeg a "felügyelt szolgáltatásokért kapott partneri jóváírás összege").

5. További számlázási részletekért tekintse át a számla recon fájlját és a napi névleges használati adatokat tartalmazó fájlt.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Számla":::

## <a name="read-the-invoice-reconciliation-file"></a>A számla egyeztetési fájl olvasása

1. Az egyes Azure-csomag- és fogyasztásmérő-kombinációk legfeljebb két számlázási svonalat használhatnak a felderítési fájlban.

2. Ha a fogyasztásmérő bármilyen típusú kedvezményre vagy jóváírásra (például rétegzett kedvezményekre vagy felügyelt szolgáltatásokhoz kapott partneri jóváírásra) jogosult az egész naptári hónapban, akkor a recon fájl csak egy számlázási sort fog tartalmazni. A **PriceAdjusmentDescription oszlop** a kedvezményre vagy a jóváírásra fog hivatkozni.

3. Ha egy adott fogyasztásmérőnek nincsenek kedvezményre vagy partneri jóváírásra jogosult erőforrásai, akkor a recon fájl csak egy számlázási sort fog tartalmazni, a tényleges egységár pedig a kiskereskedelmi ár lesz (amely az egységár).

4. Ha a fogyasztásmérő vagy az adott fogyasztásmérőt kibocsátó bármely erőforrás, amely a hónap egy részére felügyelt szolgáltatásokért kapott partneri jóváírásra van minősítve, a felderítési fájl két számlázási sort fog tartalmazni.  Az egyik vonal azokat a napokat jelenti, amelyekben a fogyasztásmérő minősített, a második pedig azokat a napokat jelenti, amelyek nem megfelelőek.

>[!NOTE]
>Az Azure-használatot az egyszeres vásárlási recon fájlban egyeztetheti. Ehhez keresse meg a napi rendszerességgel minősített használat felderítési fájlját, és keresse meg a SubscriptionID-t. Ez megjeleníti az Azure-csomag azonosítójával kapcsolatos összes költséget. Az Azure SubscriptionID jogosultságazonosítóként jelenik meg.

## <a name="read-the-daily-usage-file"></a>A napi használati adatok fájl olvasása

- Az Azure-csomag előfizetési mérőszámai napi szinten vannak minősítve és összesülve.

- **A felügyelt szolgáltatások partneri jóváírását** a rendszer naponta határozza meg és alkalmazza.

- Minden előfizetés-mérőnek van egy sora annak a hónapnak minden naphoz, ahol volt használat.

- Az alábbi példában:

  - A 7/1 és 7/3 között kezelt szolgáltatások partneri jóváírásának mérői (vegye figyelembe, hogy a tényleges egységár a kiskereskedelmi ár és a partneri jóváírás. 

  - A mérő nem  kapott partneri jóváírást a 7/4–7/7 között kezelt szolgáltatásokhoz (vegye figyelembe, hogy a tényleges egységár a kiskereskedelmi ár).

  - Partneri **jóváírásra** minősített mérő a 7/8– 7/31 között kezelt szolgáltatásokhoz (vegye figyelembe, hogy a tényleges egységár a kiskereskedelmi ár és a partneri jóváírások összege).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Számla az ügyfél pénznemében

Az Azure-csomagon keresztüli Azure-szolgáltatások díjszabása USD-ben történik, és a számlázás az ügyfél országának hozzárendelt pénznemében történik. Ha a számlázási pénznem nem USD, akkor a felhasznált átváltási díj a számla utolsó oldalán jelenik meg. Az FX díjszabását havonta határozzák meg, és az alábbi számlára alkalmazzák. Az ország pénznemek teljes listájáért tekintse meg az új kereskedelmi ajánlatok országonkénti elérhetőségét és az ügyfél [pénznemmátrixát.](https://go.microsoft.com/fwlink/?linkid=2112354)

A Microsoft a londoni tőzsdei árfolyamot követi átváltásként. Az árfolyamot használjuk, amely megegyezik a londoni tőzsdei árfolyamon a hónap utolsó üzleti napjára vonatkozó árfolyammal. Az FX díjszabása a hónap első napja előtti napon lesz frissítve és elérhető.

## <a name="azure-reservations"></a>Azure Reserved Virtual Machine Instances


Ha [Azure-csomagon keresztül](azure-reservations.md) vásárol Azure-foglalásokat, választhat egyszeres vagy havi számlázást.


## <a name="azure-spending"></a>Azure-költség

A rendszer frissíti a meglévő Azure-beli kiadásokat, hogy támogassa az új Azure-csomag számlázását a Partnerközpont. Ez lehetővé teszi a partnerek számára a következő eket:

- Ügyfélszinten beállított költségvetésre vonatkozó riasztások megtekintése, kezelése és fogadása 

- Egy Azure-csomag összes becsült kiadásának megtekintése (erőforrás- és fogyasztásmérői szint szerint bontva)

Mivel az Azure-szolgáltatások Azure-csomagon keresztüli számlázási modellje használat utáni használat, a vártnál nagyobb számla elkerülése érdekében a partnerek havi költségvetést alkalmazhatnak, és nyomon követhetik a használat százalékos arányát. A költségvetés egyszerre egy ügyfélre vagy több ügyfélre is alkalmazható. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure-költség":::

## <a name="next-steps"></a>Következő lépések

- A partneri jóváírás (PEC) kiszámításának módja. Jelentkezzen be a Partnerközpont [irányítópultra,](https://partner.microsoft.com/dashboard/) és keresse meg az elérhető árlistát.

- Tudnivalók az [Azure-csomag megvásárlásáról](purchase-azure-plan.md)

- Tekintse meg a CSP új kereskedelmi [élményének árlistát](azure-plan-price-list.md)
