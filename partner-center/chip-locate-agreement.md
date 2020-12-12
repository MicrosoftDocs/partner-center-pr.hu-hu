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
ms.openlocfilehash: 032ad30c17136dcf102af9134153a3921e29c38a
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354440"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Megállapodáshoz tartozó munkaállomásszám és díjszabás megkeresése

**Megfelelő szerepkörök**

- Elsődleges kapcsolattartó vagy program rendszergazdája

Letöltheti az Excel programba, egy olyan fájlt, amely az asztal darabszámára és a díj szintjére vonatkozó szerződési adatokat biztosít.

## <a name="how-to-locate-the-information"></a>Az információk megkeresése

1. Jelentkezzen be a CHIPre, és válassza az LSP-ösztönzők lehetőséget.

2. A **partneri fizetés összegzése** lapon válassza ki a megtekinteni kívánt jelentési hónapot, majd a legördülő listából válassza ki a **számítás részleteit** az Exportálás Excelbe gombra:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Program részleteinek megkeresése":::

3. Az Exportálás elindul, és megnyithatja a fájlt, vagy mentheti/mentheti a célhelyet.

4. A jelentés megnyitása után navigáljon a **DetailReport-FlatFile** lapra a bal alsó sarokban:

:::image type="content" source="images/chip/flatfile.png" alt-text="Lapos fájl letöltése":::

Most megkeresheti a J oszlopban keresett szerződés számát, és megtalálhatja a hozzárendelt asztalokat az R oszlopban, a Agreement_DesktopCount címkével. A jelen Szerződés díjait a "AI" címkével ellátott szinten is megerősítheti.

## <a name="next-steps"></a>Következő lépések

- [A CHIPek elérésével kapcsolatos problémák elhárítása](chip-access-trouble.md)
