---
title: Az ügyfelek listájának kezelése
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A vásárlói rekordok a legfontosabb információs eszközök közé tartoznak. Megtudhatja, hogyan tekintheti meg, keresheti meg, frissítheti, & exportálhatja a partneri központ ügyfelének listájára vonatkozó információkat.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 40df034e88a1bba7829d6f73e0fb970795a2a0dd
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2020
ms.locfileid: "92528159"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Az ügyfelek listájának kezelése – ügyfelek keresése, frissítése vagy exportálása a partner Centerben

**A következőkre vonatkozik**

- Partnerközpont
- Az USA kormányzati szerveinek Microsoft Cloud a partneri központ

Az ügyfelek rekordjai a partner Center legfontosabb információs eszközei közé tartoznak. Megkeresheti a felhasználói fiókok adatbázisát, exportálhatja a teljes ügyfél-adatbázist, vagy exportálhat egy részhalmazt egy Excel-kompatibilis, vesszővel tagolt formátumú fájlformátumba (. csv). Az ügyfél előfizetési adatait egy. csv-fájlba is exportálhatja.

A tevékenységi naplók exportálható, a tranzakciókkal és a felügyeleti műveletekkel kapcsolatos műveleteket is biztosítanak az ügyfelek számára. További információ: ügyfél- [tevékenységi naplók megtekintése](activity-logs.md).

## <a name="search-for-a-customer"></a>Ügyfél keresése

1.  A **partner Center** menüben válassza az **ügyfelek** lehetőséget.
2.  Ha meg szeretne keresni egy ügyfelet, adja meg az ügyfél nevét vagy a tartománynevet a keresőmezőbe.
3.  Válassza ki az ügyfél sor végén lévő **lefelé mutató nyilat** a Microsoft-azonosítójuk, valamint a hozzájuk tartozó előfizetések és szolgáltatások rövid hivatkozásai megtekintéséhez.

## <a name="update-a-customers-company-name"></a>Ügyfél vállalata nevének frissítése

A **partner Center** menüben válassza az **ügyfelek** lehetőséget.
2.  Ha meg szeretne keresni egy ügyfelet, adja meg az ügyfél nevét vagy a tartománynevet a keresőmezőbe.
3.  Válassza ki az ügyfél sor végén lévő **lefelé mutató nyilat** a Microsoft-azonosítójuk, valamint a hozzájuk tartozó előfizetések és szolgáltatások rövid hivatkozásai megtekintéséhez.
4.  Az ügyfél **Számlázási** adatai alatt frissítse a vállalat nevét. Az új érték mentésekor a rendszer megjeleníti az ügyfelek listáját. Ez csak a számla és a vállalat nevét, valamint az ügyfél-lista értékét fogja módosítani. Nem fog megjelenni máshol.

## <a name="export-your-customer-list"></a>Az ügyfelek listájának exportálása

1. A **partner Center** menüben válassza az **ügyfelek** lehetőséget.
2. Válassza az **ügyfelek exportálása** lehetőséget.

   A partner Center átalakítja a teljes ügyfelet egy. csv-fájlba, és feltölti a számítógép alapértelmezett letöltési mappájába. Az ügyféladatok részhalmazait is exportálhatja. Az adatoszlopok például a következők:

   - **Microsoft ID** ;
   - **Cég neve** ;
   - **Elsődleges tartománynév** ;
   - **Kapcsolat** – a partner üzleti kapcsolata a felsorolt ügyfelekkel.

    Alapértelmezés szerint a partneri központ a teljes ügyfél listát exportálja, a hossztól függetlenül. Az ügyfelek listáját a vállalat neve vagy tartománya alapján is megkeresheti, és exportálhatja az adathalmazt.

3. Ha Ön közvetett szolgáltató, akkor közvetett viszonteladóként szűrheti az ügyfelek listáját. Válassza a **szűrés közvetett viszonteladó** alapján lehetőséget a listából, majd válasszon egy viszonteladót.


## <a name="export-customer-subscription-information"></a>Ügyfél-előfizetés adatainak exportálása

1. A **partner Center** menüben válassza az **ügyfelek** lehetőséget.

2. Válassza ki a **vállalat nevét** bármelyik ügyfélnél. Megnyílik az ügyfél **előfizetések** lapja, amely a termék-előfizetések teljes listáját jeleníti meg.

3. Válassza az **előfizetések exportálása** lehetőséget. A partner Center átalakítja az ügyfél előfizetési adatait egy. csv-fájlba, és feltölti a számítógép alapértelmezett letöltési mappájába. Az adatoszlopok például a következők:
   - **Előfizetés-azonosító** ;
   - **Előfizetés** – az előfizetés terméknév;
   - **Mennyiség** – a megvásárolt licencek száma;
   - **Állapot** ;
   - **Viszonteladó** – az előfizetést birtokló és kezelő viszonteladó azonosítója.

> [!NOTE]  
> Az előfizetés-kezeléssel kapcsolatos további információkért lásd: [ügyfél-előfizetések](customer-subscriptions.md).
