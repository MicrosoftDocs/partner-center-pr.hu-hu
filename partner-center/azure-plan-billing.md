---
title: Azure-csomag számlázása – & Recon-fájlok számlázása
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan érheti el és értelmezheti az Azure-csomag számlázásával kapcsolatos számlázási és egyeztetési adatstruktúrát.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 819f90ca9a8467de4a8001a1b10f8409d3fb1b81
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/28/2021
ms.locfileid: "98924997"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Új kereskedelmi felület a CSP-ben – Azure-számlázás 

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Számlázási adminisztrátor
- Globális rendszergazda

Ez a cikk azt ismerteti, hogyan érheti el és értelmezheti az Azure-csomag számlázásával kapcsolatos számlázási és egyeztetési fájlrendszert. Az Azure-csomag keretében történő számlázás egy egyszerűsített számlázási élmény, amely egy igazított, egyetlen számlázási dátummal és naptári hónapra alapuló számlázási időszakot használ.

## <a name="summary-of-billing-essentials"></a>A számlázási alapok összefoglalása

- **Számla dátuma**: a számla-és egyeztetési fájl elérhető lesz a partner Center irányítópultján/API-ban (UTC szerint éjfélkor).

- **Számla számlázási időszaka**: a számlázási időszak a naptári hónapra van igazítva, például 10/1-10/31, 11/1-11/30.

- Díjszabási **szolgáltatási időszakok**: a díjak a naptári hónapra lesznek igazítva. Ha például a számlázott partner Azure-szolgáltatásokat ad egy 10/15-es Azure-csomagon keresztül, és az ügyfél megkezdi az Azure-szolgáltatások az 10/15-on való felhasználását, akkor a számlázott partner a 11/8-as szolgáltatási 10/15-10/31 időszakra vonatkozó számlázást és felderítést is megkapja a-on. A következő havi számla, amelyet a 12/8-es előállítás fog generálni, a 11/1-11/31-es szolgáltatási időszakra vonatkozó összes díjat tartalmazza.

- **Számla fizetési ideje**: nettó 60 nap.

- **Számla pénzneme**: január 28-ig 2021, az EU/EFTA és az Egyesült Királyság régiójában lévő partnereink, akik új ügyfelekkel és meglévő CSP-ügyfelekkel vásárolnak új kereskedelmi ajánlatokat az első alkalommal, amikor a bérlők a 2020. május 11. előtt jöttek létre, a partneri hely pénznemében megjelenő vásárlásért kell fizetni. Az EU/EFTA és az Egyesült Királyság régióján kívüli partnerek továbbra is a partneri hely pénznemében lesznek számlázva.

- **Partneri ösztönzők**: a számlázási hónap végétől számított 45 nappal.

## <a name="access-your-invoices-and-reconciliation-files"></a>A számlák és a megbékélési fájlok elérése

A vállalat globális rendszergazdája vagy számlázási rendszergazdája e-mailt fog kapni, ha a számla készen áll a megtekintésre.

A számla és a megbékélési fájl elérése:

1. Jelentkezzen be a Partnerközpont [irányítópultjába](https://partner.microsoft.com/dashboard/).

2. A partner Center menüben válassza a **számlázás** lehetőséget.

3. Válassza ki az **ismétlődő** és az **egyszeri** , valamint a pénznemhez tartozó lapot.

   :::image type="content" source="images/azure/billing3.png" alt-text="számlázási":::

4. Válassza a **számla** vagy a **megbékélési fájl** elemet.  

   A korábbi számlák és a felderítési fájlok megtekintéséhez bontsa ki az alábbi számlázási előzmények sort.

## <a name="understanding-usage-data"></a>A használati adatok ismertetése 

1. Az Azure-csomag a legfelső szintű vagy legfelső szintű tároló a használathoz. Minden használat egyetlen Azure-csomaghoz van kötve.

2. Egy csomagon belül egy vagy több Azure-előfizetés lesz. Ezek az erőforrások kezeléséhez és üzembe helyezéséhez használt tárolók. 

3. Egy előfizetésen belül erőforráscsoportok hozzáadásával csoportosíthatja az erőforrásokat. Minden erőforrás üzembe helyezése egy erőforráscsoporthoz történik. 

4. Ilyenek például a virtuális gépek és a Storage-fiókok. 

5. Erőforrás-kibocsátó mérőszámok: a mérőórák egy erőforrás felhasználásának mérései, és egy erőforrás több fogyasztásmérőn is kibocsáthatja a használatot. A mérőórákat a termékkód, a SKUId és a AvailabilityId azonosítja. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Az előfizetési erőforráscsoportok és a mérések hierarchiája

**Azure-fiók (bérlő)**

- Előfizetés A
    - 1. ResourceGroup
        - Virtuális gép (erőforrás)
            - Számítási fogyasztásmérő
        - Virtuális hálózat (erőforrás)
            - Nincs számlázási fogyasztásmérő

    - 2. ResourceGroup
        - Virtuális gép (erőforrás)
            - Számítógép-fogyasztásmérő
        - Prémium SSD felügyelt lemez (erőforrás)
            - Tárolási kapacitás mérője
            - Tárolási műveleti fogyasztásmérő

- Előfizetés B-ResourceGroup 1 – Azure SQL (erőforrás) – DTU-mérő-VPN Gateway (erőforrás) – VPN Gateway-mérő

    - 2. ResourceGroup
        - Virtual Network csatoló (erőforrás)
            - Nincs számlázási fogyasztásmérő

## <a name="read-the-invoice"></a>A számla elolvasása

1. A számla az egyes hónapok nyolcadik napján nem lesz elérhető.

2. A partnereknek 60 napja van a fizetésre.

3. A számlázási időszak egy adott naptári hónapra vonatkozni fog, például 10/1-10/31.

4. A díjak nettó kiigazítások (az összeg a "partner által felügyelt szolgáltatások által kezelt kreditek" nettó mennyisége).

5. További számlázási részletekért tekintse át a számla-felderítési fájlt és a napi minősítésű használati fájlt.

   :::image type="content" source="images/azure/invoice1.png" alt-text="számla":::

## <a name="read-the-invoice-reconciliation-file"></a>A számlázási egyeztetési fájl elolvasása

1. Minden egyes Azure-csomag és-mérési kombináció legfeljebb két számlázási sorral rendelkezhet a Recon-fájlban.

2. Ha a mérőszám a teljes naptári hónapban bármilyen típusú kedvezményt vagy kreditet (például a többrétegű kedvezményeket vagy a partner által kezelt szolgáltatások kreditjét) minősítette, akkor a felderítési fájl csak egy számlázási sort fog tartalmazni. A **PriceAdjusmentDescription** oszlop a kedvezményre vagy a keresett kreditre hivatkozik.

3. Ha nincs olyan erőforrás egy adott mérőszámhoz, amely kedvezményre vagy partner által felhasználható kreditre van kiértékelve, akkor a felderítési fájl csak egy számlázási sort fog tartalmazni, és a hatályos egység ára a kiskereskedelmi díj (amely az egység díja).

4. Ha a mérő, vagy bármely olyan erőforrás, amely az adott mérőszámot kibocsátja, a partner által a hónap egy részében **kezelt szolgáltatásokra vonatkozó jóváírásra** jogosult, a Recon-fájl két számlázási sort fog tartalmazni. Az egyik sor azokat a napokat jelöli, amelyeknek a mérőszáma minősített, a második sor pedig azon napokat jelöli, amelyeknek a mérőszáma nem volt

## <a name="read-the-daily-usage-file"></a>A napi használati fájl elolvasása

- Az előfizetési mérőszámok az Azure-csomag keretében vannak értékelve, és naponta halmozódnak.

- A **felügyelt szolgáltatásokhoz tartozó partner által létrehozott kreditek** napi rendszerességgel vannak meghatározva és alkalmazva.

- Minden előfizetési fogyasztásmérőnek van egy sora a hónap minden napján, amelyben használatban volt.

- Az alábbi példában:

  - A 7/1-7/3-től **felügyelt szolgáltatások esetében a partner által szerzett kreditek** díja

  - A mérő nem felelt meg a partner által a 7/4-7/7-től **felügyelt szolgáltatásokra vonatkozó kreditért** (a tényleges egység ára a kiskereskedelmi díj).

  - A 7/8-7/31-től **felügyelt szolgáltatások esetében a partner által szerzett kreditek** díja (a tényleges egység ára a kiskereskedelmi ár, a partner által szerzett kredit).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Számla az ügyfél pénznemében

Az Azure-csomagokon keresztül az Azure-szolgáltatások díja USD lesz, és az ügyfél-országhoz rendelt pénznemben kell fizetni. Ha a számlázási pénznem nem USD, akkor a számla utolsó oldalán a használt deviza-(FX-) díj is megjelenik. Az FX díjszabását havonta határozzák meg, és a következő számlára kell alkalmazni. Az ország pénznemek teljes listájáért tekintse meg az [új kereskedelmi ajánlatok ország rendelkezésre állását és az ügyfél pénznemének mátrixát](https://go.microsoft.com/fwlink/?linkid=2112354).

A Microsoft a londoni tőzsdei árfolyamot követi az átalakításhoz. Az árfolyamot használjuk, amely a Londoni Értéktőzsdén a hónap utolsó munkanapján rögzített árfolyamot használja fel az utóbbi időben. Az FX díjszabása a hónap első előtti napján frissül és elérhető lesz.

## <a name="azure-reservations"></a>Azure Reserved Virtual Machine Instances


Az Azure- [foglalások](azure-reservations.md) Azure-csomagon keresztüli megvásárlásakor egyszeri vagy havi számlázást is választhat.


## <a name="azure-spending"></a>Azure-költség

A meglévő Azure-kiadások a partner Centerben új Azure-csomag számlázásának támogatásához frissülnek. Ez lehetővé teszi a partnerek számára a következőket:

- A költségvetési készletre vonatkozó riasztások megtekintése, kezelése és fogadása az ügyfél szintjén 

- Az Azure-csomag becsült összes kiadásának megtekintése (erőforrás-és mérési szint szerinti bontásban)

Mivel az Azure-szolgáltatások számlázási modellje az Azure-csomagon keresztüli fizetés utáni használatot jelent, hogy a vártnál nagyobb mennyiségű számla elkerülhető legyen, a partnerek havi költségvetést alkalmazhatnak, és nyomon követhetik a használat százalékos arányát. Egy költségvetést egyszerre csak egy vagy több ügyfélre lehet alkalmazni. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure-költség":::

## <a name="next-steps"></a>Következő lépések

- Megtudhatja, hogyan számítja ki a partner által létrehozott kreditet (PEC). Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/) , és keresse meg az elérhető árlista listáját.

- További információ [Az Azure-csomag megvásárlásáról](purchase-azure-plan.md)

- Tekintse meg a [CSP új kereskedelmi élményét ismertető árlistát](azure-plan-price-list.md)
