---
title: Partneri központ – áttekintés
description: Ismerje meg ezt a partneri központ egyesített jelentéskészítési irányítópultját. Ismerje meg, hogyan végezheti el a KPI-ket az értékesítéshez és üzembe helyezéshez, az ügyfelek fejlesztéséhez és egyebekhez.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: ba8389ff613b47b17b87a6769674e33948fdc37d
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086583"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a><span data-ttu-id="a0e24-104">Partner Center-elemzések – egy irányítópult, amely bemutatja, hogyan történik a Microsoft kereskedelmi partnere</span><span class="sxs-lookup"><span data-stu-id="a0e24-104">Partner Center Insights - a dashboard that shows how a Microsoft commercial partner is doing</span></span>

<span data-ttu-id="a0e24-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="a0e24-105">**Appropriate roles**</span></span>

- <span data-ttu-id="a0e24-106">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="a0e24-106">Global admin</span></span>
- <span data-ttu-id="a0e24-107">Fiókadminisztrátor</span><span class="sxs-lookup"><span data-stu-id="a0e24-107">Account admin</span></span>
- <span data-ttu-id="a0e24-108">Executive Report Viewer</span><span class="sxs-lookup"><span data-stu-id="a0e24-108">Executive report viewer</span></span>
- <span data-ttu-id="a0e24-109">Jelentés megjelenítője</span><span class="sxs-lookup"><span data-stu-id="a0e24-109">Report viewer</span></span>

## <a name="introduction"></a><span data-ttu-id="a0e24-110">Bevezetés</span><span class="sxs-lookup"><span data-stu-id="a0e24-110">Introduction</span></span>

<span data-ttu-id="a0e24-111">Az áttekintési irányítópult a Microsoft kereskedelmi partnereinek a Microsoft Partner Network-(MPN-) programban regisztrált partnereinek egyesített jelentési irányítópultja.</span><span class="sxs-lookup"><span data-stu-id="a0e24-111">The Insights dashboard is a unified reporting dashboard in Partner Center for Microsoft’s Commercial partners who are enrolled in the Microsoft Partner Network (MPN) program.</span></span> <span data-ttu-id="a0e24-112">Az áttekintések irányítópultja a főbb teljesítménymutatók (KPI) 360 fokos áttekintését biztosítja a felhőalapú termékek, például az Office, az Azure, a Dynamics és a licencelési modellek (például a CSP és az EA) között.</span><span class="sxs-lookup"><span data-stu-id="a0e24-112">The Insights dashboard provides 360-degree view of your key performance indicators (KPI) across Cloud products such as Office, Azure, Dynamics, and licensing models such as CSP and EA.</span></span> <span data-ttu-id="a0e24-113">Számos KPI-jelentést tesz elérhetővé, amelyek segíthetnek az adatvezérelt döntések meghozatalában a szervezet számára.</span><span class="sxs-lookup"><span data-stu-id="a0e24-113">It exposes a rich set of KPI reports that can help you make data driven decisions for your organization.</span></span> 

## <a name="role-based-access-control-to-the-insights-dashboard"></a><span data-ttu-id="a0e24-114">Szerepköralapú hozzáférés-vezérlés a bepillantást az irányítópultra</span><span class="sxs-lookup"><span data-stu-id="a0e24-114">Role-based access control to the Insights dashboard</span></span>

<span data-ttu-id="a0e24-115">A partner Centerben két új szerepkör van kialakítva, kifejezetten az információhoz való hozzáféréshez: a **jelentéskészítő** és a **Executive Report Viewer**.</span><span class="sxs-lookup"><span data-stu-id="a0e24-115">There are two new roles in Partner Center designed specifically for access to Insights: **Report Viewer** and **Executive Report Viewer**.</span></span> <span data-ttu-id="a0e24-116">A vezetői jelentés megjelenítője szerepkör felhasználói hozzáférhetnek az összes jelentéskészítési adatkészlethez, míg a jelentés-megjelenítőben lévő felhasználók nem férhetnek hozzá a bizalmas adatkészletekhez, például a bevételekhez és az ügyfél/alkalmazottak személyes adatokhoz.</span><span class="sxs-lookup"><span data-stu-id="a0e24-116">Users in the Executive Report Viewer role have access to all reporting data sets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span> 

<span data-ttu-id="a0e24-117">A globális rendszergazda vagy a fiók rendszergazdája hozzárendelheti a felhasználókat ezekhez a szerepkörökhöz, és a teljes vállalathoz vagy egy adott MPN-helyhez hozzá lehet rendelni.</span><span class="sxs-lookup"><span data-stu-id="a0e24-117">The Global admin or the Account admin can assign users these roles and are assigned either for the entire company or for a specific MPN location.</span></span>  

>[!Note] 
><span data-ttu-id="a0e24-118">Azok a felhasználók, akik január 20-án, a 2020-as és az MPN-rendszergazdák voltak, automatikusan hozzáadódnak a vállalati szintű jelentéskészítő szerepkörhöz.</span><span class="sxs-lookup"><span data-stu-id="a0e24-118">Users who were MPN admins as of Jan 20th, 2020 were automatically added to the company-wide report viewer role.</span></span> <span data-ttu-id="a0e24-119">A jelentéseket jelentés-megjelenítőként érhetik el anélkül, hogy a globális rendszergazda vagy a fiók rendszergazdája nem igényel explicit műveletet. Ha szükséges, a globális rendszergazdák vagy a fiók rendszergazdája felülbírálhatja ezeket a hozzárendeléseket.</span><span class="sxs-lookup"><span data-stu-id="a0e24-119">They are able to access the reports as a report viewer without any explicit action required by Global admin or Account admin. The Global admins or account admin can override these assignments if necessary.</span></span> 

## <a name="reports-available"></a><span data-ttu-id="a0e24-120">Elérhető jelentések</span><span class="sxs-lookup"><span data-stu-id="a0e24-120">Reports available</span></span>

<span data-ttu-id="a0e24-121">Az alábbi jelentések az áttekintések irányítópultjának részeként érhetők el.</span><span class="sxs-lookup"><span data-stu-id="a0e24-121">The following reports are available as part of the Insights dashboard.</span></span>

<span data-ttu-id="a0e24-122">**Áttekintés**: az áttekintő jelentés a különféle KPI-k, például az ügyfelek száma, az aktív előfizetések száma, az Azure-beli használati bevétel, az aktív licencek stb. pillanatkép-nézetét jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="a0e24-122">**Overview**: The Overview report presents a snapshot view of various KPIs of interest to you such as Customer count, Active Subscriptions count, Azure Consumption Revenue, Active licenses etc.</span></span>

<span data-ttu-id="a0e24-123">**Ügyfél**: az ügyfél-jelentés az ügyfelek körét, például az ügyfelek beszerzési adatait, az aktív ügyfeleket stb.</span><span class="sxs-lookup"><span data-stu-id="a0e24-123">**Customer**: The Customer report presents analytics around your customers such as Customer acquisition data, Active customers, etc.</span></span>

<span data-ttu-id="a0e24-124">**Termék-** előfizetések: az előfizetések jelentés a felhőalapú előfizetések (például a O365, az Azure, a Dynamics stb.) beszerzési és használati elemzéseit mutatja be.</span><span class="sxs-lookup"><span data-stu-id="a0e24-124">**Product - Subscriptions**: The Subscriptions report presents acquisition and usage analytics for your Cloud subscriptions (such as O365, Azure, Dynamics etc.)</span></span>

<span data-ttu-id="a0e24-125">**Termék-licencek**: a licencek irányítópultja a licenc-alapú felhőalapú termékek, például a O365, a Dynamics, a Power bi stb. licenc-elemzési szolgáltatásait mutatja be.</span><span class="sxs-lookup"><span data-stu-id="a0e24-125">**Product- Licenses**: The Licenses dashboard presents license analytics for license-based Cloud products such as O365, Dynamics, Power BI etc.</span></span>

<span data-ttu-id="a0e24-126">**Termék – Azure-használat**: az Azure-használati jelentés az ügyfelek Azure-előfizetéséhez kapcsolódó mérőszámokat jelenít meg, beleértve az Azure-beli felhasználás bevételét és a mérési kategóriák alapján történő használatot.</span><span class="sxs-lookup"><span data-stu-id="a0e24-126">**Product - Azure usage**: The Azure Usage report presents metrics related to your customers’ Azure subscriptions including Azure consumption revenue and usage by meter categories.</span></span>

<span data-ttu-id="a0e24-127">**Kompetenciák**: a kompetenciák jelentés mérőszámokat jelenít meg az aktív, minősített és veszélyeztetett kompetenciákkal kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="a0e24-127">**Competencies**: The Competencies report presents metrics on your Active, Qualified, and At-risk competencies.</span></span>

<span data-ttu-id="a0e24-128">**Előnyök**: az előnyökről szóló jelentés az elemzést nyújtja a partneri előnyökkel kapcsolatban, amelyet a keresett és felhasznált</span><span class="sxs-lookup"><span data-stu-id="a0e24-128">**Benefits**: The Benefits report presents analytics on partner benefits you have earned vs consumed.</span></span>

## <a name="navigating-the-insights-reports"></a><span data-ttu-id="a0e24-129">Navigálás az áttekintési jelentésekben</span><span class="sxs-lookup"><span data-stu-id="a0e24-129">Navigating the Insights reports</span></span>

<span data-ttu-id="a0e24-130">**Dátumtartomány-szűrők**: az egyes lapok jobb felső sarkában található dátumtartomány-kijelölést is megtalálhatja.</span><span class="sxs-lookup"><span data-stu-id="a0e24-130">**Date range filters**: You can find a date range selection at the top-right corner of each page.</span></span> <span data-ttu-id="a0e24-131">Az áttekintő oldal diagramjainak kimenete testreszabható úgy, hogy kijelöl egy dátumtartományt az elmúlt 3, 6 vagy 12 hónap alapján, vagy egy egyéni dátumtartományt választ.</span><span class="sxs-lookup"><span data-stu-id="a0e24-131">The output of the overview page graphs can be customized by selecting a date range based on the past 3, 6, or 12 months, or by selecting a custom date range.</span></span> <span data-ttu-id="a0e24-132">A dátumtartomány alapértelmezett kiválasztása 12 hónap.</span><span class="sxs-lookup"><span data-stu-id="a0e24-132">The default date range selection is 12 months.</span></span> 

:::image type="content" source="images/pci/intro1.png" alt-text="Bevezetési Térkép":::

<span data-ttu-id="a0e24-134">**Visszajelzés gomb**: az összes betekintési jelentés minden diagramja/vezérlése egy visszajelzési gombbal van beépítve, amely lehetővé teszi a példányok visszajelzésének megadását egy jelentési szolgáltatásban.</span><span class="sxs-lookup"><span data-stu-id="a0e24-134">**Feedback button**: Each chart/control in all the Insights reports is incorporated with a feedback button to let you provide instance feedback on a report feature.</span></span> 

 
<span data-ttu-id="a0e24-135">**Oldal szintű szűrők**: az Áttekintés, az előnyök és a kompetenciák jelentéseinek kivételével az összes betekintési jelentés lehetővé teszi az oldal szintű szűrők alkalmazását.</span><span class="sxs-lookup"><span data-stu-id="a0e24-135">**Page level filters**: Except for the Overview, Benefits, and Competencies reports, all Insights reports enable you to apply page level filters.</span></span> 

- <span data-ttu-id="a0e24-136">A kiválasztott szűrők a lapon lévő összes diagramra és metrikára érvényesek lesznek, beleértve az összefoglalás szakaszt is.</span><span class="sxs-lookup"><span data-stu-id="a0e24-136">The filters selected will be applicable for all charts and metrics on a page, including the summary section.</span></span> <span data-ttu-id="a0e24-137">A szűrő elem akkor lesz elérhető, ha az adott szűrési feltételben lévő bármilyen adattal rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="a0e24-137">A filter item will be available if you have any data within that filter criteria.</span></span> 

- <span data-ttu-id="a0e24-138">Az egyes szűrőlisták alapértelmezett kiválasztása az **összes**.</span><span class="sxs-lookup"><span data-stu-id="a0e24-138">Default selection of each filter list is **all**.</span></span> <span data-ttu-id="a0e24-139">Ha például nem jelölt ki egy terméket a Products (termékek) szűrőben, a rendszer alapértelmezés szerint az összes terméket kijelöli.</span><span class="sxs-lookup"><span data-stu-id="a0e24-139">For example, if you have not selected a specific product in products filter, default selection will be all products.</span></span>

- <span data-ttu-id="a0e24-140">A kiválasztott szűrők a lap tetején jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="a0e24-140">Filters selected will be displayed at the top of the page.</span></span> 

:::image type="content" source="images/pci/filters.png" alt-text="Részleges képernyőkép az alkalmazott szűrők sávjáról a termékek, az ügyfelek piacai, a partnerek és az értékesítési csatornák szűrési kiválasztásával.":::

### <a name="filters-definitions"></a><span data-ttu-id="a0e24-142">Szűrők definíciói:</span><span class="sxs-lookup"><span data-stu-id="a0e24-142">Filters definitions:</span></span>

- <span data-ttu-id="a0e24-143">Termékek: a szervezet által eladott/kezelt Microsoft Cloud termékek listája, például O365, Azure, D365, EMS, Power BI stb.</span><span class="sxs-lookup"><span data-stu-id="a0e24-143">Products: List of all Microsoft Cloud products sold/managed by your organization, for example,  O365, Azure, D365, EMS, Power BI, etc.</span></span>
- <span data-ttu-id="a0e24-144">Ügyfelek piacai: az ügyfél-országok listája</span><span class="sxs-lookup"><span data-stu-id="a0e24-144">Customer markets: List of customer countries</span></span>
- <span data-ttu-id="a0e24-145">Partneri hozzárendelések: a társítás típusa az ügyfelek előfizetésével együtt, például a digitális Partner of Record (DPOR), a delegált rendszergazdai jogosultság (DAP) és a partner rendszergazdai hivatkozása (PAL).</span><span class="sxs-lookup"><span data-stu-id="a0e24-145">Partner attributions: Your association type with your customers' subscriptions, for example, Digital partner of record (DPOR), Delegated admin privilege (DAP), and Partner Admin link (PAL).</span></span> 
- <span data-ttu-id="a0e24-146">Partneri helyszínek: az összes szervezet MPN-helyeinek listája.</span><span class="sxs-lookup"><span data-stu-id="a0e24-146">Partner locations: List of all your organization’s MPN locations.</span></span>
- <span data-ttu-id="a0e24-147">Értékesítési csatornák: minden értékesítési csatorna/díjszabás, amelyen keresztül vásárolja meg/kiépíti a termékeket és szolgáltatásokat, azaz CSP, EA, CSP indirekt, Direct, Advisor, Open, Others</span><span class="sxs-lookup"><span data-stu-id="a0e24-147">Sales channels: All sales channel/pricing through which you are purchasing/provisioning products and services namely CSP, EA, CSP indirect, Direct, Advisor, Open, others</span></span>
- <span data-ttu-id="a0e24-148">Felhasználói szegmensek: az ügyfél-szegmensek listája a partnerek ügyfélkörén keresztül.</span><span class="sxs-lookup"><span data-stu-id="a0e24-148">Customer segments: List of customer segments across the partners customer base.</span></span>

## <a name="read-about-each-of-the-dashboards-and-reports"></a><span data-ttu-id="a0e24-149">További információ az irányítópultokról és jelentésekről:</span><span class="sxs-lookup"><span data-stu-id="a0e24-149">Read about each of the dashboards and reports:</span></span>

- [<span data-ttu-id="a0e24-150">A partner Center-információk áttekintése – irányítópult</span><span class="sxs-lookup"><span data-stu-id="a0e24-150">Partner Center Insights - Overview dashboard</span></span>](pci-overview-report.md)

- [<span data-ttu-id="a0e24-151">Partneri központ – áttekintés – ügyfél-irányítópult</span><span class="sxs-lookup"><span data-stu-id="a0e24-151">Partner Center Insights - Customer dashboard</span></span>](pci-customer-report.md)

- [<span data-ttu-id="a0e24-152">Partneri központ – bejelentések – előfizetések jelentése</span><span class="sxs-lookup"><span data-stu-id="a0e24-152">Partner Center Insights - Subscriptions report</span></span>](pci-product-subscriptions-report.md)

- [<span data-ttu-id="a0e24-153">A partneri központ által észlelt jelentések – licencek jelentése</span><span class="sxs-lookup"><span data-stu-id="a0e24-153">Partner Center Insights - Licenses report</span></span>](pci-product-licenses-report.md)

- [<span data-ttu-id="a0e24-154">Partner Center-adatok – Azure-használati jelentés</span><span class="sxs-lookup"><span data-stu-id="a0e24-154">Partner Center Insights - Azure usage report</span></span>](pci-azure-usage-report.md)

- [<span data-ttu-id="a0e24-155">A partner Center-ismeretek – kompetenciák jelentése</span><span class="sxs-lookup"><span data-stu-id="a0e24-155">Partner Center Insights - Competencies report</span></span>](pci-competencies-report.md)

- [<span data-ttu-id="a0e24-156">A partner Center által nyújtott ismeretek – előnyök jelentés</span><span class="sxs-lookup"><span data-stu-id="a0e24-156">Partner Center Insights - Benefits report</span></span>](pci-benefits-report.md)
