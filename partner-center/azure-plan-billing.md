---
title: Azure-csomag számlázása – számla & recon files
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan férhet hozzá és értheti meg az Azure-csomag számlázásával kapcsolatos számla- és egyeztetési fájlstruktúrát.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c7c06f5ed7b147625afb5020f63ead411ef58fa8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551520"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Új kereskedelmi felület a CSP-ben – Azure-számlázás 

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Globális rendszergazda

Ez a cikk azt ismerteti, hogyan férhet hozzá az Azure-csomag számlázásához kapcsolódó számla- és egyeztetési fájlstruktúrához, és hogyan értheti meg azt. Az Azure-csomag szerinti számlázás egy egyszerűsített számlázási élmény, amely egy igazított egyetlen számlázási dátumot és egy naptári hónapalapú számlázási időszakot használ.

## <a name="summary-of-billing-essentials"></a>A számlázással kapcsolatos alapvető információk összegzése

- **Számla dátuma:** A számla és az egyeztetési fájl a következő időpontig Partnerközpont (UTC) éjfélig lesz elérhető a Partnerközpont irányítópultján/API-ján.

- **Számlázási időszak:** A számla számlázási időszaka a naptári hónaphoz igazodik, például: 10/1-10/31, 11/1-11/30.

- **Díjak szolgáltatási időszaka:** A díjak a naptári hónaphoz igazodnak. Ha például a számlázott partner azure-szolgáltatásokat ad hozzá egy Azure-csomagon keresztül 10/15-én, és az ügyfél 10/15-én kezdi meg az Azure-szolgáltatások használatának elkezdét, akkor a kiszámlázott partner a 10/15–31 szolgáltatási időszakra vonatkozóan a 10/10/31-es szolgáltatási időszakra vonatkozóan a 11/8-as ügyfélfelhasználásra vonatkozóan kap számlát/recont. A következő hónap 12/8-án generált számlája tartalmazza a 11/1–11/31 szolgáltatási időszakra vonatkozó díjakat.

- **Számlás fizetési időszak:** 60 nap.

- **Számla** pénzneme: 2021. január 28-tól kezdődően azok az EU-/EFTA- és Egyesült Királyság-régióban lévő partnerek, akik új ügyfelekkel és meglévő CSP-ügyfelekkel vásárolnak új kereskedelmi ajánlatokat 2020. május 11. előtt, a partneri hely pénznemében lesznek számlázva. Az EU-n/EFTA-n és az Egyesült Királyságon kívül található partnerek számlázása továbbra is a partnerhely pénznemében történik.

- **Partneri ösztönzők:** A számlázási hónap végével 45 nappal fizették ki.

## <a name="access-your-invoices-and-reconciliation-files"></a>Hozzáférés a számlákhoz és az egyeztetési fájlokhoz

A vállalat globális rendszergazdája vagy számlázási rendszergazdája e-mailt kap, ha a számla készen áll a megtekintésre.

A számla és az egyeztetési fájl elérése:

1. Jelentkezzen be a Partnerközpont [irányítópultjába](https://partner.microsoft.com/dashboard/).

2. A Partnerközpont válassza a Számlázás **lehetőséget.**

3. Válassza a Recurring (Ismétlődő) **és** **az One-time (Egyszeri) lapfület,** valamint a kívánt pénznemet.

   :::image type="content" source="images/azure/billing3.png" alt-text="Számlázási.":::

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

- B előfizetés –ResourceGroup 1 – Azure SQL (erőforrás) – DTU-fogyasztásmérő – VPN Gateway (erőforrás) – VPN-átjáró mérő

    - ResourceGroup 2
        - Virtual Network felület (erőforrás)
            - Nincs számlázási mérő

## <a name="read-the-invoice"></a>A számla olvasása

1. A számla legkésőbb az egyes hónap végéig lesz elérhető.

2. A partnereknek 60 napjuk van a kifizetés visszafizetésére.

3. A számlázási időszak egy adott naptári hónapra vonatkozik, például: 10.1-10.31.

4. A díjak a kiigazítások nettó összegei (az összeg a "felügyelt szolgáltatások partneri jóváírásának nettó összege").

5. További számlázási részletekért tekintse át a számla recon fájlját és a napi névleges használati adatokat tartalmazó fájlt.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Számla.":::

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

  - A 7/8-tól 7/31-ig felügyelt szolgáltatások partneri jóváírásának mérőja (vegye figyelembe, hogy a tényleges egységár a kiskereskedelmi ár és a partneri jóváírások összege). 

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a>Számla az ügyfél pénznemében

Az Azure-csomagon keresztüli Azure-szolgáltatások díjszabása AMERIKAI DOLLÁRban történik, és a számlázás az ügyfél országának hozzárendelt pénznemében történik. Ha a számlázási pénznem nem USD, akkor a felhasznált átváltási díj a számla utolsó oldalán jelenik meg. Az FX-árfolyamok meghatározása havonta történik, és az alábbi számlán lesz alkalmazva. Az ország pénznemek teljes listájáért tekintse meg az új kereskedelmi ajánlatok országonkénti elérhetőségét és az ügyfél [pénznemmátrixát.](https://go.microsoft.com/fwlink/?linkid=2112354)

A Microsoft egy előre meghatározott átváltási árfolyamot alkalmaz az alap USD-árakra, hogy az egyes naptári hónapban megvásárolt vagy felhasznált Azure-szolgáltatások teljes díjára vonatkozzon. A havi átváltási árfolyam a Thomson Reuters által (általában) az előző hónap vége előtt két munkanap, 16:00-kor (GMT) közzétett árfolyam. 

**Például:** A Microsoft decemberi árfolyama a Thomson Reuters középárfolyama november 29-én vagy körül lenne egy adott pénznemben. Ez a díj az ebben a pénznemben történt összes vásárlásra alkalmazva lesz december 1-től december 31-ig. 

## <a name="azure-reservations"></a>Azure Reserved Virtual Machine Instances


Ha [Azure-foglalásokat vásárol](azure-reservations.md) egy Azure-csomagon keresztül, választhat egy egyszeres vagy havi számlázást.


## <a name="azure-spending"></a>Azure-költség

A rendszer frissíti a meglévő Azure-kiadásokat, hogy támogassa az új Azure-csomag számlázását a Partnerközpont. Ez lehetővé teszi a partnerek számára a következőt:

- Az ügyfélszinten beállított költségvetéssel kapcsolatos riasztások megtekintése, kezelése és fogadása 

- Egy Azure-csomag összes becsült kiadásának megtekintése (erőforrás- és fogyasztásmérő-szint szerint bontva)

Mivel az Azure-szolgáltatások Azure-csomagon keresztüli számlázási modellje használat utáni használat, a vártnál nagyobb számla elkerülése érdekében a partnerek havi költségvetést alkalmazhatnak, és nyomon követhetik a használat százalékos arányát. A költségvetés egyszerre egy ügyfélre vagy több ügyfélre is alkalmazható. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure-kiadások.":::

## <a name="next-steps"></a>Következő lépések

- Tekintse meg a partneri jóváírás (PEC) kiszámításának módját. Jelentkezzen be az Partnerközpont [irányítópultra,](https://partner.microsoft.com/dashboard/) és keresse meg az elérhető árlistát.

- Tudnivalók az [Azure-csomag megvásárlásáról](purchase-azure-plan.md)

- Tekintse meg a CSP új kereskedelmi [élményének árlistát](azure-plan-price-list.md)
