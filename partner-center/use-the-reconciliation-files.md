---
title: A megbékélési fájlok használata
ms.topic: article
ms.date: 06/08/2020
description: Ismerje meg a fiókpartner egyeztetési fájljait, valamint azt, hogy miként értelmezhető az adott számlázási időszakra vonatkozó díjak részletes, sorokra vonatkozó nézetei.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d927b138c32b3e5f6f5d906db898e17f89a85aae
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "101755784"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Megtudhatja, hogyan olvashatja el a partner Center-egyeztetési fájlok sorát

A következőkre vonatkozik:

- Partnerközpont
- A Microsoft Cloud for US Government Partnerközpontja

**Megfelelő szerepkörök**

- Számlázási adminisztrátor
- Globális rendszergazda

A partner Centerről letöltheti a megbékélési fájlokat a számlázási ciklusban minden egyes díj részletes, sorban álló nézetéhez. A sor részletei közé tartoznak az egyes ügyfelek előfizetései, valamint a részletes események (például a licencek félidős hozzáadása az előfizetéshez).

A **számla** beolvasásával kapcsolatos információkért lásd: [a számla olvasása](read-your-bill.md).

## <a name="understand-reconciliation-file-fields"></a>Az egyeztetési fájl mezőinek megismerése

- [Licencalapú egyeztetési fájl mezői](license-based-recon-files.md)
- [Használatalapú egyeztetési fájl mezői](usage-based-recon-files.md)
- [Napi névleges használatú egyeztetési fájl mezői](daily-rated-usage-recon-files.md)
- [Egyszeri beszerzési CSP-egyeztetési fájl mezői](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>A díjszabási típusok megértése az egyeztetési fájlokban

Ha meg szeretné ismerni az egyeztetési fájlok (a **ChargeType** oszlop) használati feltételeit, tekintse meg a következőt: [egyeztetési](recon-file-charge-types.md)feltételek.

## <a name="fix-formatting-issues"></a>Formázási problémák javítása

Esetenként előfordulhat, hogy egy egyeztető fájl formázási problémákat tartalmaz. Ez a probléma például akkor fordulhat elő, ha az en-US területi beállítás nincs használatban.

A következő lépések végrehajtásával javítsa ki az egyeztetési fájlok formázási problémáit:

1. Nyissa meg az egyeztetési fájlt (. csv formátumban) a Microsoft Excelben.
2. Válassza ki a fájl első oszlopát.
3. Nyissa meg a **szöveg konvertálása oszlopokra varázslót**. A menüszalagon válassza az adatelemet, majd válassza a **szöveg oszlopokra** **lehetőséget.**
4. A varázslóban válassza a **tagolt fájl típusa** lehetőséget. Ezután válassza a **tovább** lehetőséget.
5. A **határolójelek** mezőben válassza a **vessző** lehetőséget. (Ha a **Tab** már be van jelölve, akkor ezt a lehetőséget kiválasztva hagyhatja.) Ezután válassza a **tovább** lehetőséget.
6. Az **oszlop adatformátuma** mezőben válassza a **Date: MDY** lehetőséget. Ezután válassza a **tovább** lehetőséget.
7. Az **oszlop adatformátuma** mezőben válassza a **szöveg** lehetőséget az összes oszlop értéknél. Ezután válassza a **Befejezés** gombot.

## <a name="download-reconciliation-files-programmatically"></a>Az egyeztetési fájlok programozott módon tölthetők le

Az egyeztetési fájlok nagyon nagy méretűek lehetnek, és időnként nehéz letölteni. Ha programozott módon szeretné letölteni az egyeztetési fájlokat, tekintse meg a [Számlázási sorok beolvasása című cikket](/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Adók vagy ÁFA leképezése

Adók vagy hozzáadottérték-adó (ÁFA) hozzárendelése a számlához:

- Adja meg az **adó** oszlopot a licenc-alapú fájlból.
- A **TaxAmount** oszlop összege a használaton alapuló fájlból.

## <a name="itemize-reconciliation-files-by-partner"></a>Itemize-egyeztetési fájlok partner szerint

A **közvetett modellben** lévő partnerek ezeket a további mezőket használhatják a licenc-és a használati alapú egyeztetési fájlokban is, hogy itemize a fájlokat a viszonteladók által.

| MPN-azonosító | Leírás |
| ------ | ----------- |
| MPN-azonosító | A Cloud Solution Provider (CSP) partner (közvetlen vagy közvetett) Microsoft Partner Network (MPN) azonosítója. |
| [Viszonteladói MPN-azonosító](#reseller-mpn-id) | Az [előfizetéshez tartozó rekord viszonteladójának MPN-azonosítója](#reseller-mpn-id). Ez a mező az adott előfizetéshez tartozó, a partner Centerben megadott viszonteladói AZONOSÍTÓnak felel meg. Csak a közvetett modellben lévő partnereknek szóló egyeztető fájlokban jelenik meg. |

### <a name="reseller-mpn-id"></a>Viszonteladói MPN-azonosító

Ha egy CSP-partner közvetlenül az ügyfélnek adta el az előfizetést, az **MPN-azonosítójuk** kétszer jelenik meg, mint az **MPN-azonosító** és a **viszonteladói MPN-azonosító**.

Ha a CSP-partner rendelkezik **MPN-azonosító** nélküli viszonteladóval, akkor ez az érték a partner **MPN-azonosítóját** adja meg helyette.

Ha a CSP-partner eltávolít egy **viszonteladói MPN-azonosítót**, az érték *-1* lesz.

A **viszonteladói MPN-azonosító** megtekintése vagy frissítése:

1. Jelentkezzen be a Partnerközpontba.
2. A partner Center menüben válassza az **ügyfelek** lehetőséget.
3. Válassza ki az ügyfelet a listából.
4. Az ügyfél menüben válassza az **előfizetések** lehetőséget.
5. Válassza ki az előfizetést a listából.
6. Válassza a **frissítés** lehetőséget a **viszonteladó (MPN-azonosító)** módosításához.

## <a name="next-steps"></a>Következő lépések

- [A Bill & Recon-fájl beolvasása](read-your-bill.md) 