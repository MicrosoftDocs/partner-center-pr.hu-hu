---
title: Partnerközpont Insights
description: Fedezze fel ezt Partnerközpont jelentéskészítési irányítópultot. Tekintse meg, hogyan működik az értékesítéssel és üzembe helyezéssel, az ügyfélfejlesztéssel és egyéb szolgáltatásokkal kapcsolatos KPI-kben.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: 05fad9c7eecbc8b7f639faa24b654fb0474245ca
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277623"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>Partnerközpont Insights – egy irányítópult, amely bemutatja, hogyan működik egy Microsoft kereskedelmi partner

**Megfelelő szerepkörök:** Globális rendszergazdai | Fiók-rendszergazdai | Vezetői jelentésmegjelenítő | Jelentésmegjelenítő

## <a name="introduction"></a>Bevezetés

Az Insights irányítópult egy egységes jelentéskészítési irányítópult a Partnerközpont microsoftos kereskedelmi partnerek számára, akik regisztrálva vannak a Microsoft Partner Network (MPN) programban. Az Insights irányítópult 360 fokos áttekintést nyújt a fő teljesítménymutatókról (KPI-kről) az olyan felhőalapú termékekben, mint az Office, az Azure, a Dynamics és az olyan licencelési modellek, mint a CSP és az EA. KPI-jelentések gazdag készletét teszi elérhetővé, amelyek segítségével adatvezérelt döntéseket hozhat a szervezete számára. 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>Szerepköralapú hozzáférés-vezérlés az Insights-irányítópulthoz

A jelentés két új szerepkört Partnerközpont kifejezetten az  Elemzések elérésére terveztek: a Jelentésmegjelenítőt és a Vezetői jelentésmegjelenítőt.  A Vezetői jelentésmegjelenítő szerepkörben a felhasználók az összes jelentéskészítési adatkészlethez hozzáférhetnek, míg a Jelentésmegjelenítő szerepkör felhasználói nem férhetnek hozzá olyan bizalmas adatkészlethez, mint a bevétel és az ügyfél/alkalmazott személyes adatai. 

A globális rendszergazda vagy a fiók rendszergazdája hozzárendelheti ezeket a szerepköröket a felhasználókhoz, és a teljes vállalathoz vagy egy adott MPN-helyhez vannak hozzárendelve.  

>[!Note] 
>Azok a felhasználók, akik 2020. január 20-án MPN-rendszergazdák voltak, automatikusan bekerültek a vállalati szintű jelentésmegjelenítői szerepkörbe. A jelentéseket a globális rendszergazda vagy a fiók rendszergazdai beavatkozása nélkül is elérhetik jelentésmegjelenítőként. A globális rendszergazdák vagy a fiók rendszergazdái szükség esetén felülbírálhatják ezeket a hozzárendeléseket. 

## <a name="reports-available"></a>Elérhető jelentések

Az alábbi jelentések az Insights irányítópult részeként érhetők el.

**Áttekintés:** Az Áttekintő jelentés pillanatkép-nézetben mutatja be az Ön számára érdekes KPI-ket, például az ügyfelek számát, az aktív előfizetések számát, az Azure Consumption Revenue-t, az aktív licenceket stb.

**Ügyfél:** Az Ügyféljelentés elemzéseket készít az ügyfelekről, például ügyfélszerzési adatokat, aktív ügyfeleket stb.

**Termék – Előfizetések:** Az Előfizetések jelentés a felhőalapú előfizetések beszerzési és használati elemzését mutatja be (például O365, Azure, Dynamics stb.)

**Termék – Licencek:** A Licencek irányítópult licencelemzést biztosít olyan licencalapú felhőalapú termékekhez, mint az O365, a Dynamics, Power BI stb.

**Termék – Azure-használat:** Az Azure használati jelentése az ügyfelek Azure-előfizetéséhez kapcsolódó metrikákat mutatja be, beleértve az Azure-használati bevételt és a fogyasztásmérők kategóriái szerint meghatározott használatot.

**Kompetenciák:** A Kompetenciák jelentés az Aktív, a Minősített és a Veszélyeztetett kompetencia metrikait mutatja be.

**Előnyök:** Az előnyökről szóló jelentés elemzéseket biztosít a megszerzett és a felhasznált partneri előnyökről.

## <a name="navigating-the-insights-reports"></a>Navigálás az Insights-jelentésekben

**Dátumtartomány-szűrők:** Az egyes oldalak jobb felső sarkában talál egy dátumtartomány-kijelölést. Az áttekintő oldalgráfok kimenete az elmúlt 3, 6 vagy 12 hónap alapján egy dátumtartomány kiválasztásával vagy egy egyéni dátumtartomány kiválasztásával szabható testre. Az alapértelmezett dátumtartomány kiválasztása 12 hónap. 

:::image type="content" source="images/pci/intro1.png" alt-text="Bevezetési térkép.":::

**Visszajelzés gomb:** Az összes Insights-jelentés minden diagramja/vezérlőjéhez be van építve egy visszajelzési gomb, amely lehetővé teszi a példányok visszajelzését egy jelentési funkcióval kapcsolatban. 

 
**Oldalszintű szűrők:** Az Áttekintés, Előnyök és Kompetenciák jelentések kivételével minden Insights-jelentés lehetővé teszi oldalszintű szűrők alkalmazását. 

- A kiválasztott szűrők az egy oldalon található összes diagramra és metrikára vonatkoznak, beleértve az összefoglaló szakaszt is. A szűrőelem akkor lesz elérhető, ha a szűrési feltételekben vannak adatok. 

- Az összes szűrőlista alapértelmezett **kijelölése.** Ha például nem választott ki egy adott terméket a termékek szűrőben, az alapértelmezett kijelölés az összes termék lesz.

- A kiválasztott szűrők az oldal tetején jelennek meg. 

:::image type="content" source="images/pci/filters.png" alt-text="Részleges képernyőkép az Alkalmazott szűrők sávról a Termékek, az Ügyfélpiacok, a Partnerek forrásmegjelölése és az Értékesítés csatornák szűrőkijelölésével.":::

### <a name="filters-definitions"></a>Szűrődefiníciók:

- Termékek: A szervezet által értékesített/kezelt Microsoft Cloud-termékek listája, például O365, Azure, D365, EMS, Power BI stb.
- Ügyfélpiacok: Az ügyfél országok listája
- Partnerek forrásmegjelölése: Az Ön társítástípusa az ügyfelek előfizetésével, például Digitális partner a rekordhoz (DPOR), Delegált rendszergazdai jogosultság (DAP) és Partneradminisztrátor hivatkozás (PAL). 
- Partnerhelyek: A szervezet összes MPN-helyének listája.
- Értékesítési csatornák: Minden értékesítési csatorna/díjszabás, amelyen keresztül termékeket és szolgáltatásokat vásárol vagy kiépít, nevezetesen CSP, EA, KÖZVETETT CSP, Közvetlen, Advisor, Open stb.
- Ügyfélszegmensek: A partnerek ügyfélkörében lévő ügyfélszegmensek listája.

## <a name="read-about-each-of-the-dashboards-and-reports"></a>Olvassa el az egyes irányítópultokat és jelentéseket:

- [Partnerközpont Insights – Áttekintő irányítópult](pci-overview-report.md)

- [Partnerközpont Insights – Ügyfél irányítópultja](pci-customer-report.md)

- [Partnerközpont Insights – Előfizetések jelentés](pci-product-subscriptions-report.md)

- [Partnerközpont Insights – Licencjelentés](pci-product-licenses-report.md)

- [Partnerközpont Insights – Azure használati jelentés](pci-azure-usage-report.md)

- [Partnerközpont Insights – Kompetenciák jelentés](pci-competencies-report.md)

- [Partnerközpont Insights – Előnyök jelentés](pci-benefits-report.md)
