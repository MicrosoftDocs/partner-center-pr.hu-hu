---
title: A megbékélési fájlok használata
ms.topic: article
ms.date: 03/26/2021
description: Ismerje meg a fiókpartner egyeztetési fájljait, valamint azt, hogy miként értelmezhető az adott számlázási időszakra vonatkozó díjak részletes, sorokra vonatkozó nézetei.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730082"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Megtudhatja, hogyan olvashatja el a partner Center-egyeztetési fájlok sorát

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

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Ha a fájl túllépi az Excelben megadott korlátot

Ha le tudja tölteni az egyeztetési fájlt, de nem nyitja meg a Microsoft Excelben, valószínűleg azt jelenti, hogy a fájl több sort is tartalmaz, mint amennyit az Excel engedélyez. Ha ez történik, a fájl megnyitásához használhatja az alábbi eljárások egyikét.

### <a name="open-a-recon-file-in-power-bi"></a>Felderítési fájl megnyitása Power BI

1. Töltse le az egyeztetési fájlt a szokásos módon.
2. Power BI-példány letöltése, telepítése és megnyitása.
3. A Power BI **Kezdőlap** lapon válassza az **adatlekérdezés** lehetőséget.
4. A **gyakori adatforrások** listájában válassza a **text/CSV** lehetőséget.
5. Ha a rendszer kéri, nyissa meg a Recon-fájlt.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Egy Recon-fájl megnyitása egy Excel-pivot táblában

1. Töltse le az egyeztetési fájlt a szokásos módon.
2. Nyisson meg egy új fájlt a Microsoft Excelben.
3. Az **adatok** lapon válassza az **adatok lekérése** elemet, válassza a **fájlból** lehetőséget, majd válassza a **text/CSV** lehetőséget.
4. Ha a rendszer kéri, nyissa meg a Recon-fájlt. Ekkor megjelennek az adatai.
5. A **Betöltés** legördülő menüben válassza a **Betöltés a** következőhöz lehetőséget, majd **az OK gombot**.
6. Az **adatimportálás** párbeszédpanelen válassza a **kimutatás jelentést** a fájl megnyitásához.

## <a name="negative-amount-displayed"></a>Megjelenített negatív mennyiség

Az egyeztetési fájlban negatív összeg jelenhet meg. Ezt valószínűleg az alábbi dolgok okozzák:

- A közelmúltban megszakította vagy csökkentette a licencek számát
- A szolgáltatás licencszerződése (SLA) vagy az Azure-beli felhasználás esetében kreditet kapott

Ha további információt szeretne kapni erről a tranzakcióról, tekintse át a reegyeztető fájlban lévő Charge Type attribútumát.

## <a name="map-taxes-or-vat"></a>Adók vagy ÁFA leképezése

Adók vagy hozzáadottérték-adó (ÁFA) hozzárendelése a számlához:

- Adja meg az **adó** oszlopot a licenc-alapú fájlból.
- A **TaxAmount** oszlop összege a használaton alapuló fájlból.

## <a name="itemize-reconciliation-files-by-partner"></a>Itemize-egyeztetési fájlok partner szerint

A **közvetett modellben** lévő partnerek ezeket a további mezőket használhatják a licenc-és a használati alapú egyeztetési fájlokban is, hogy itemize a fájlokat a viszonteladók által.

| MPN-azonosító | Description |
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