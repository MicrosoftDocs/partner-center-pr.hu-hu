---
title: Partnerközpont Elemzések
description: Fedezze fel ezt Partnerközpont jelentéskészítési irányítópultot. Tekintse meg, hogyan működik az értékesítéssel és üzembe helyezéssel, az ügyfélfejlesztéssel és más szolgáltatásokkal kapcsolatos KPI-kben.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: a16cca546142d3a8091643607534697e0403fff9
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114373726"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a><span data-ttu-id="7322e-104">Partnerközpont Elemzések – egy irányítópult, amely bemutatja, hogyan működik egy Microsoft kereskedelmi partner</span><span class="sxs-lookup"><span data-stu-id="7322e-104">Partner Center Insights - a dashboard that shows how a Microsoft commercial partner is doing</span></span>

<span data-ttu-id="7322e-105">**Megfelelő szerepkörök:** Globális rendszergazdai | Fiók-rendszergazdai | Vezetői jelentésmegjelenítő | Jelentésmegjelenítő</span><span class="sxs-lookup"><span data-stu-id="7322e-105">**Appropriate roles**: Global admin | Account admin | Executive report viewer | Report viewer</span></span>

## <a name="introduction"></a><span data-ttu-id="7322e-106">Bevezetés</span><span class="sxs-lookup"><span data-stu-id="7322e-106">Introduction</span></span>

<span data-ttu-id="7322e-107">Az Elemzések irányítópult egy egységes jelentéskészítési irányítópult a Partnerközpont-ban a Microsoft kereskedelmi partnerei számára, akik regisztrálva vannak a Microsoft Partner Network (MPN) programban.</span><span class="sxs-lookup"><span data-stu-id="7322e-107">The Insights dashboard is a unified reporting dashboard in Partner Center for Microsoft's Commercial partners who are enrolled in the Microsoft Partner Network (MPN) program.</span></span> <span data-ttu-id="7322e-108">Az Elemzések irányítópultján 360 fokban megtekintheti a fő teljesítménymutatókat (KPI-ket) a felhőalapú termékekben, például az Office-ban, az Azure-ban, a Dynamicsben és a licencelési modellekben, például a CSP-ben és az EA-ben.</span><span class="sxs-lookup"><span data-stu-id="7322e-108">The Insights dashboard provides 360-degree view of your key performance indicators (KPI) across Cloud products such as Office, Azure, Dynamics, and licensing models such as CSP and EA.</span></span> <span data-ttu-id="7322e-109">KpI-jelentések gazdag készletét teszi elérhetővé, amelyek segítségével adatvezérelt döntéseket hozhat a szervezet számára.</span><span class="sxs-lookup"><span data-stu-id="7322e-109">It exposes a rich set of KPI reports that can help you make data driven decisions for your organization.</span></span> 

## <a name="role-based-access-control-to-the-insights-dashboard"></a><span data-ttu-id="7322e-110">Szerepköralapú hozzáférés-vezérlés a Elemzések irányítópulthoz</span><span class="sxs-lookup"><span data-stu-id="7322e-110">Role-based access control to the Insights dashboard</span></span>

<span data-ttu-id="7322e-111">A jelentés két új szerepkört Partnerközpont kifejezetten a jelentések **Elemzések:** a Jelentésmegjelenítő és a Vezetői jelentésmegjelenítő. </span><span class="sxs-lookup"><span data-stu-id="7322e-111">There are two new roles in Partner Center designed specifically for access to Insights: **Report Viewer** and **Executive Report Viewer**.</span></span> <span data-ttu-id="7322e-112">A Vezetői jelentésmegjelenítő szerepkörben a felhasználók az összes jelentéskészítési adatkészlethez hozzáférhetnek, míg a Jelentésmegjelenítő szerepkör felhasználói nem férhetnek hozzá a bizalmas adatkészlethez, például a bevételhez és az ügyfél/alkalmazott személyes adataihoz.</span><span class="sxs-lookup"><span data-stu-id="7322e-112">Users in the Executive Report Viewer role have access to all reporting data sets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span> 

<span data-ttu-id="7322e-113">A globális rendszergazda vagy a fiók rendszergazdája hozzárendelheti ezeket a szerepköröket a felhasználókhoz, és a teljes vállalathoz vagy egy adott MPN-helyhez vannak hozzárendelve.</span><span class="sxs-lookup"><span data-stu-id="7322e-113">The Global admin or the Account admin can assign users these roles and are assigned either for the entire company or for a specific MPN location.</span></span>  

>[!Note] 
><span data-ttu-id="7322e-114">Azok a felhasználók, akik 2020. január 20-án MPN-rendszergazdák voltak, automatikusan bekerültek a vállalati szintű jelentésmegjelenítő szerepkörbe.</span><span class="sxs-lookup"><span data-stu-id="7322e-114">Users who were MPN admins as of Jan 20th, 2020 were automatically added to the company-wide report viewer role.</span></span> <span data-ttu-id="7322e-115">A jelentéseket a globális rendszergazda vagy a fiók-rendszergazda kifejezett beavatkozása nélkül is elérhetik jelentésmegjelenítőként. A globális rendszergazdák vagy a fiók rendszergazdái szükség esetén felülbírálhatják ezeket a hozzárendeléseket.</span><span class="sxs-lookup"><span data-stu-id="7322e-115">They are able to access the reports as a report viewer without any explicit action required by Global admin or Account admin. The Global admins or account admin can override these assignments if necessary.</span></span> 

## <a name="reports-available"></a><span data-ttu-id="7322e-116">Elérhető jelentések</span><span class="sxs-lookup"><span data-stu-id="7322e-116">Reports available</span></span>

<span data-ttu-id="7322e-117">A következő jelentések érhetők el az irányítópult Elemzések részeként.</span><span class="sxs-lookup"><span data-stu-id="7322e-117">The following reports are available as part of the Insights dashboard.</span></span>

<span data-ttu-id="7322e-118">**Áttekintés:** Az Áttekintés jelentés pillanatkép-nézetben mutatja be az Ön számára érdekes KPI-ket, például az ügyfelek számát, az aktív előfizetések számát, az Azure Consumption Revenue-t, az aktív licenceket stb.</span><span class="sxs-lookup"><span data-stu-id="7322e-118">**Overview**: The Overview report presents a snapshot view of various KPIs of interest to you such as Customer count, Active Subscriptions count, Azure Consumption Revenue, Active licenses etc.</span></span>

<span data-ttu-id="7322e-119">**Ügyfél:** Az Ügyféljelentés elemzéseket készít az ügyfelekről, például ügyfélszerzési adatokat, aktív ügyfeleket stb.</span><span class="sxs-lookup"><span data-stu-id="7322e-119">**Customer**: The Customer report presents analytics around your customers such as Customer acquisition data, Active customers, etc.</span></span>

<span data-ttu-id="7322e-120">**Termék – Előfizetések:** Az Előfizetések jelentés bemutatja a felhőalapú előfizetések beszerzési és használati elemzését (például O365, Azure, Dynamics stb.)</span><span class="sxs-lookup"><span data-stu-id="7322e-120">**Product - Subscriptions**: The Subscriptions report presents acquisition and usage analytics for your Cloud subscriptions (such as O365, Azure, Dynamics etc.)</span></span>

<span data-ttu-id="7322e-121">**Termék – Licencek:** A Licencek irányítópult licencelemzést biztosít olyan licencalapú felhőalapú termékekhez, mint az O365, a Dynamics, Power BI stb.</span><span class="sxs-lookup"><span data-stu-id="7322e-121">**Product- Licenses**: The Licenses dashboard presents license analytics for license-based Cloud products such as O365, Dynamics, Power BI etc.</span></span>

<span data-ttu-id="7322e-122">**Termék – Azure-használat:** Az Azure használati jelentése az ügyfelek Azure-előfizetéséhez kapcsolódó metrikákat mutatja be, beleértve az Azure-beli használati bevételt és a fogyasztásmérők kategóriánkénti használatát.</span><span class="sxs-lookup"><span data-stu-id="7322e-122">**Product - Azure usage**: The Azure Usage report presents metrics related to your customers' Azure subscriptions including Azure consumption revenue and usage by meter categories.</span></span>

<span data-ttu-id="7322e-123">**Kompetenciák:** A Kompetenciák jelentés az Aktív, Minősített és At-Risk kompetenciák metrikait mutatja be.</span><span class="sxs-lookup"><span data-stu-id="7322e-123">**Competencies**: The Competencies report presents metrics on your Active, Qualified, and At-risk competencies.</span></span>

<span data-ttu-id="7322e-124">**Előnyök:** Az előnyökről szóló jelentés elemzéseket biztosít a megszerzett és a felhasznált partneri előnyökről.</span><span class="sxs-lookup"><span data-stu-id="7322e-124">**Benefits**: The Benefits report presents analytics on partner benefits you have earned vs consumed.</span></span>

## <a name="navigating-the-insights-reports"></a><span data-ttu-id="7322e-125">Navigálás a Elemzések jelentésekben</span><span class="sxs-lookup"><span data-stu-id="7322e-125">Navigating the Insights reports</span></span>

<span data-ttu-id="7322e-126">**Dátumtartomány-szűrők:** Az egyes oldalak jobb felső sarkában talál egy dátumtartomány-kijelölést.</span><span class="sxs-lookup"><span data-stu-id="7322e-126">**Date range filters**: You can find a date range selection at the top-right corner of each page.</span></span> <span data-ttu-id="7322e-127">Az áttekintő oldalgráfok kimenete az elmúlt 3, 6 vagy 12 hónap alapján dátumtartomány kiválasztásával, vagy egy egyéni dátumtartomány kiválasztásával szabható testre.</span><span class="sxs-lookup"><span data-stu-id="7322e-127">The output of the overview page graphs can be customized by selecting a date range based on the past 3, 6, or 12 months, or by selecting a custom date range.</span></span> <span data-ttu-id="7322e-128">Az alapértelmezett dátumtartomány-beállítás 12 hónap.</span><span class="sxs-lookup"><span data-stu-id="7322e-128">The default date range selection is 12 months.</span></span> 

:::image type="content" source="images/insights/introduction.png" alt-text="Bevezetési térkép.":::

<span data-ttu-id="7322e-130">**Visszajelzés gomb:** Az összes Elemzések-jelentés minden diagramja/vezérlői egy visszajelzési gombbal vannak beépítve, így példányokkal kapcsolatos visszajelzést adhat a jelentés funkciójával kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="7322e-130">**Feedback button**: Each chart/control in all the Insights reports is incorporated with a feedback button to let you provide instance feedback on a report feature.</span></span> 

 
<span data-ttu-id="7322e-131">**Oldalszintű szűrők:** Az Áttekintés, Előnyök és Kompetenciák jelentések kivételével minden Elemzések jelentés lehetővé teszi oldalszintű szűrők alkalmazását.</span><span class="sxs-lookup"><span data-stu-id="7322e-131">**Page level filters**: Except for the Overview, Benefits, and Competencies reports, all Insights reports enable you to apply page level filters.</span></span> 

- <span data-ttu-id="7322e-132">A kiválasztott szűrők az egy oldalon található összes diagramra és metrikára vonatkoznak, beleértve az összefoglaló szakaszt is.</span><span class="sxs-lookup"><span data-stu-id="7322e-132">The filters selected will be applicable for all charts and metrics on a page, including the summary section.</span></span> <span data-ttu-id="7322e-133">A szűrőelem akkor lesz elérhető, ha a szűrési feltételekben vannak adatok.</span><span class="sxs-lookup"><span data-stu-id="7322e-133">A filter item will be available if you have any data within that filter criteria.</span></span> 

- <span data-ttu-id="7322e-134">Az összes szűrőlista alapértelmezett **kijelölése.**</span><span class="sxs-lookup"><span data-stu-id="7322e-134">Default selection of each filter list is **all**.</span></span> <span data-ttu-id="7322e-135">Ha például nem választott ki egy adott terméket a termékek szűrőben, az alapértelmezett kijelölés az összes termék lesz.</span><span class="sxs-lookup"><span data-stu-id="7322e-135">For example, if you have not selected a specific product in products filter, default selection will be all products.</span></span>

- <span data-ttu-id="7322e-136">A kiválasztott szűrők az oldal tetején jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="7322e-136">Filters selected will be displayed at the top of the page.</span></span> 

:::image type="content" source="images/insights/filters.png" alt-text="Részleges képernyőkép az Alkalmazott szűrők sávról a Termékek, az Ügyfélpiacok, a Partnerek forrásmegjelölése és az Értékesítés csatornák szűrőkijelölésével.":::

### <a name="filters-definitions"></a><span data-ttu-id="7322e-138">Szűrődefiníciók:</span><span class="sxs-lookup"><span data-stu-id="7322e-138">Filters definitions:</span></span>

- <span data-ttu-id="7322e-139">Termékek: A szervezet által értékesített/kezelt Microsoft Cloud-termékek listája, például O365, Azure, D365, EMS, Power BI stb.</span><span class="sxs-lookup"><span data-stu-id="7322e-139">Products: List of all Microsoft Cloud products sold/managed by your organization, for example,  O365, Azure, D365, EMS, Power BI, etc.</span></span>
- <span data-ttu-id="7322e-140">Ügyfélpiacok: Az ügyfél országok listája</span><span class="sxs-lookup"><span data-stu-id="7322e-140">Customer markets: List of customer countries</span></span>
- <span data-ttu-id="7322e-141">Partnerek forrásmegjelölése: Az Ön társítástípusa az ügyfelek előfizetésével, például a digitális rekordpartner (DPOR), a meghatalmazott rendszergazdai jogosultság (DAP) és a Partneradminisztrátor hivatkozás (PAL).</span><span class="sxs-lookup"><span data-stu-id="7322e-141">Partner attributions: Your association type with your customers' subscriptions, for example, Digital partner of record (DPOR), Delegated admin privilege (DAP), and Partner Admin link (PAL).</span></span> 
- <span data-ttu-id="7322e-142">Partnerhelyek: A szervezet összes MPN-helyének listája.</span><span class="sxs-lookup"><span data-stu-id="7322e-142">Partner locations: List of all your organization's MPN locations.</span></span>
- <span data-ttu-id="7322e-143">Értékesítési csatornák: Minden értékesítési csatorna/díjszabás, amelyen keresztül termékeket és szolgáltatásokat vásárol/létesít, azaz CSP, EA, közvetett CSP, Közvetlen, Advisor, Open stb.</span><span class="sxs-lookup"><span data-stu-id="7322e-143">Sales channels: All sales channel/pricing through which you are purchasing/provisioning products and services namely CSP, EA, CSP indirect, Direct, Advisor, Open, others</span></span>
- <span data-ttu-id="7322e-144">Ügyfélszegmensek: A partnerek ügyfélkörében lévő ügyfélszegmensek listája.</span><span class="sxs-lookup"><span data-stu-id="7322e-144">Customer segments: List of customer segments across the partners customer base.</span></span>

## <a name="read-about-each-of-the-dashboards-and-reports"></a><span data-ttu-id="7322e-145">Olvassa el az egyes irányítópultokat és jelentéseket:</span><span class="sxs-lookup"><span data-stu-id="7322e-145">Read about each of the dashboards and reports:</span></span>

- [<span data-ttu-id="7322e-146">Partnerközpont Elemzések – Áttekintő irányítópult</span><span class="sxs-lookup"><span data-stu-id="7322e-146">Partner Center Insights - Overview dashboard</span></span>](insights-overview-report.md)

- [<span data-ttu-id="7322e-147">Partnerközpont Elemzések – Ügyfél irányítópultja</span><span class="sxs-lookup"><span data-stu-id="7322e-147">Partner Center Insights - Customer dashboard</span></span>](insights-customer-report.md)

- [<span data-ttu-id="7322e-148">Partnerközpont Elemzések – Előfizetések jelentés</span><span class="sxs-lookup"><span data-stu-id="7322e-148">Partner Center Insights - Subscriptions report</span></span>](insights-product-subscriptions-report.md)

- [<span data-ttu-id="7322e-149">Partnerközpont Elemzések – Licencjelentés</span><span class="sxs-lookup"><span data-stu-id="7322e-149">Partner Center Insights - Licenses report</span></span>](insights-product-licenses-report.md)

- [<span data-ttu-id="7322e-150">Partnerközpont Elemzések – Azure-használati jelentés</span><span class="sxs-lookup"><span data-stu-id="7322e-150">Partner Center Insights - Azure usage report</span></span>](insights-azure-usage-report.md)

- [<span data-ttu-id="7322e-151">Partnerközpont Elemzések – Kompetenciajelentés</span><span class="sxs-lookup"><span data-stu-id="7322e-151">Partner Center Insights - Competencies report</span></span>](insights-competencies-report.md)

- [<span data-ttu-id="7322e-152">Partnerközpont Elemzések – Előnyök jelentés</span><span class="sxs-lookup"><span data-stu-id="7322e-152">Partner Center Insights - Benefits report</span></span>](insights-benefits-report.md)
