---
title: Asztali darabszám, díj szintje a CHIPben
ms.topic: how-to
ms.date: 11/09/2020
description: Megtudhatja, hogyan használhatja a Channel ösztönzők platformot (CHIP) a szerződések asztalának darabszámára és díjszabására vonatkozó információk megkereséséhez.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 51307be51de3c41aca9fb9d39ab623f4dac318a7
ms.sourcegitcommit: 6b03ff400d1350db9696f9b457fcfe710310c5d3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/03/2020
ms.locfileid: "96570552"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Megállapodáshoz tartozó munkaállomásszám és díjszabás megkeresése

Letöltheti az Excel programba, egy olyan fájlt, amely az asztal darabszámára és a díj szintjére vonatkozó szerződési adatokat biztosít.

## <a name="how-to-locate-the-information"></a>Az információk megkeresése

1. Jelentkezzen be a CHIPre, és válassza az LSP-ösztönzők lehetőséget.

2. A **partneri fizetés összegzése** lapon válassza ki a megtekinteni kívánt jelentési hónapot, majd a legördülő listából válassza ki a **számítás részleteit** az Exportálás Excelbe gombra:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Program részleteinek megkeresése":::

3. Az Exportálás elindul, és megnyithatja a fájlt, vagy mentheti/mentheti a célhelyet.

4. A jelentés megnyitása után navigáljon a **DetailReport-FlatFile** lapra a bal alsó sarokban:

:::image type="content" source="images/chip/flatfile.png" alt-text="Lapos fájl letöltése":::

Most megkeresheti a J oszlopban keresett szerződés számát, és megtalálhatja a hozzárendelt asztalokat az R oszlopban, a Agreement_DesktopCount címkével. A jelen Szerződés díjait a "AI" címkével ellátott szinten is megerősítheti.

## <a name="next-steps"></a>További lépések

- [A CHIPek elérésével kapcsolatos problémák elhárítása](chip-access-trouble.md)
