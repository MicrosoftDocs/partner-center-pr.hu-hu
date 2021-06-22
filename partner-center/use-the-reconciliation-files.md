---
title: Az egyeztetési fájlok használata
ms.topic: article
ms.date: 03/26/2021
description: Megismerheti az egyeztetési fájlokat Partnerközpont és az adott számlázási ciklus díjtételek részletes, sortételes nézeteinek értelmezését.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431572"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Ismerje meg, hogyan olvashatja be az egyeztetési fájlokban Partnerközpont sorelemeket

**Megfelelő szerepkörök:** Számlázási rendszergazdai | Globális rendszergazda

Az egyeztetési fájlokat letöltheti a Partnerközpont a számlázási ciklusban lévő egyes díjtételek részletes, sorelemnézetéhez. A sortételek részletei tartalmazzák az egyes ügyfelek előfizetéseiért fizetendő díjakat és a részletes eseményeket (például a licencek előfizetéshez való rövid távú kiegészítését).

A számla beolvassa a (Számla olvasása) [adatokat.](read-your-bill.md) 

## <a name="understand-reconciliation-file-fields"></a>Az egyeztetési fájlmezők

- [Licencalapú egyeztetési fájl mezői](license-based-recon-files.md)
- [Használatalapú egyeztetési fájl mezői](usage-based-recon-files.md)
- [Napi névleges használatú egyeztetési fájl mezői](daily-rated-usage-recon-files.md)
- [Egy alkalommal vásárolt CSP egyeztetési fájl mezői](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Díjtípusok az egyeztetési fájlokban

Az egyeztetési fájlokban (a **ChargeType** oszlopban) található díjtípusokról az Egyeztetési fájl [díjtípusa tartalmaz további adatokat.](recon-file-charge-types.md)

## <a name="fix-formatting-issues"></a>Formázási problémák megoldása

Az egyeztetési fájlok esetenként formázási problémákat is tartalmazhatnak. Ez a probléma például akkor fordulhat elő, ha az en-US területi et nem használja.

Az egyeztetési fájlok formázási problémáinak megoldásához kövesse az alábbi lépéseket:

1. Nyissa meg az egyeztetési fájlt (.csv formátumban) a Microsoft Excelben.
2. Válassza ki a fájl első oszlopát.
3. Nyissa meg **a Szöveg átalakítása oszlopokká varázslót.** A menüszalagon válassza az **Adatok** lehetőséget, majd a **Szövegből oszlopokba lehetőséget.**
4. A varázslóban válassza a **Tagolt fájltípus lehetőséget.** Ezután válassza a **Tovább lehetőséget.**
5. Az **Elválasztó mezőkben** válassza a **Vessző lehetőséget.** (Ha **a Tab** már ki van jelölve, ezt a beállítást hagyja bejelölve.) Ezután válassza a **Tovább lehetőséget.**
6. Az Oszlop **adatformátuma mezőben** válassza a **Date:MDY lehetőséget.** Ezután válassza a **Tovább lehetőséget.**
7. Az Oszlop **adatformátuma mezőben** válassza a **Szöveg lehetőséget** minden összegoszlophoz. Ezután válassza a **Befejezés** gombot.

## <a name="download-reconciliation-files-programmatically"></a>Egyeztetési fájlok letöltése programozott módon

Az egyeztetési fájlok nagyon nagy méretűek, és néha nehezen tölthetők le. Az egyeztetési fájlok programozott letöltéséhez lásd: [Számlasorelemek betöltése.](/partner-center/develop/get-invoiceline-items)

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Ha a fájl túllépi a sorkorlátot az Excelben

Ha le tud tölteni egy egyeztetési fájlt, de nem nyitja meg a Microsoft Excelben, az valószínűleg azt jelenti, hogy a fájl több sort tartalmaz, mint amennyit az Excel engedélyez. Ebben az esetben az alábbi eljárások bármelyikével megnyithatja a fájlt.

### <a name="open-a-recon-file-in-power-bi"></a>Nyisson meg egy recon fájlt a Power BI

1. Töltse le az egyeztetési fájlt a szokásos módon.
2. Töltse le, telepítse és nyissa meg a Microsoft Power BI.
3. A Power BI **lapon** válassza az Adatok **lekérte lehetőséget.**
4. A Gyakori adatforrások **listájában válassza** a **Szöveg/CSV lehetőséget.**
5. Amikor a rendszer kéri, nyissa meg a recon fájlt.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Felderítési fájl megnyitása Excel-kimutatástáblában

1. Töltse le az egyeztetési fájlt a szokásos módon.
2. Nyisson meg egy új fájlt a Microsoft Excelben.
3. Az Adatok **lapon** válassza az Adatok **lekérte** lehetőséget, válassza a **Fájlból,** majd a **Szöveg/CSV lehetőséget.**
4. Amikor a rendszer kéri, nyissa meg a recon fájlt. Megjelennek az adatok.
5. A **Betöltés legördülő** menüben válassza **a** Betöltés ide, majd az **OK gombot.**
6. Az Adatok **importálása párbeszédpanelen** válassza a **Kimutatás jelentés lehetőséget** a fájl megnyitásához.

## <a name="negative-amount-displayed"></a>Megjelenített negatív összeg

Előfordulhat, hogy negatív összeget lát az egyeztetési fájlban. Ezt valószínűleg az alábbiak valamelyike okozza:

- Nemrég lemondta vagy csökkentette a licencek számát
- Jóváírást kapott egy szolgáltatáslicenc-szerződés (SLA) vagy az Azure-használat alapján

Ha további információt szeretne kapni erről a tranzakcióról, tekintse meg a díjtípus attribútumát az egyeztetési fájlban.

## <a name="map-taxes-or-vat"></a>Adó- vagy áfaleképés térképe

Adó- vagy értékadó (ÁFA) leképezése a számlára:

- Összegezve **a licencalapú** fájl Adó oszlopát.
- Összegezve **a TaxAmount oszlopot** a használatalapú fájlból.

## <a name="itemize-reconciliation-files-by-partner"></a>Egyeztetési fájlok elemet ad meg partner szerint

A közvetett **modellben lévő partnerek** ezeket a további mezőket licencalapú és használatalapú egyeztetési fájlokban is felhasználhatjak a fájlok viszonteladó szerint való elemztetéséhez.

| MPN-azonosító | Leírás |
| ------ | ----------- |
| MPN-azonosító | A Microsoft Partner Network (közvetlen vagy közvetett) partner Felhőszolgáltató (MPN) azonosítója. |
| [Viszonteladói MPN-azonosító](#reseller-mpn-id) | Az [előfizetés rekordjának viszonteladójának MPN-azonosítója.](#reseller-mpn-id) Ez a mező az adott előfizetéshez felsorolt viszonteladói azonosítónak felel meg a Partnerközpont. Csak a közvetett modellben lévő partnerek egyeztetési fájljaiban jelenik meg. |

### <a name="reseller-mpn-id"></a>Viszonteladói MPN-azonosító

Ha egy CSP-partner közvetlenül az ügyfélnek adta el az előfizetést, az **MPN-azonosítója** kétszer lesz listázva, mind **MPN-azonosítóként,** mind **viszonteladói MPN-azonosítóként.**

Ha egy CSP-partner egy **MPN-azonosítóval** nem rendelkezik viszonteladóval, akkor ez az érték a partner **MPN-azonosítójára van beállítva.**

Ha a CSP-partner eltávolít egy **viszonteladói MPN-azonosítót,** ez az érték *-1* lesz.

A Viszonteladói **MPN-azonosító megtekintése** vagy frissítése:

1. Jelentkezzen be a Partnerközpontba.
2. A Partnerközpont válassza az Ügyfelek **lehetőséget.**
3. Válassza ki az ügyfelet a listából.
4. Az ügyfélmenüben válassza az **Előfizetések lehetőséget.**
5. Válassza ki az előfizetést a listából.
6. Válassza **a Frissítés** lehetőséget a viszonteladó **(MPN-azonosító) módosításhoz.**

## <a name="next-steps"></a>Következő lépések

- [A számla olvasása & recon fájlban](read-your-bill.md) 