---
title: Szerepköralapú hozzáférés a partneri központban
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerkedjen meg a partneri központ által jelentett információk megtekintéséhez szükséges szerepkörökkel. Ezek közé tartoznak a Executive Report Viewer és a Report Viewer szerepkörei.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 980c086a2ab1ee0a21592ceb1e2e018c0e1159ae
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2020
ms.locfileid: "92528331"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="24042-104">Szerepköralapú hozzáférés-vezérlés a partner Center-alapú adatellenőrzési irányítópulthoz</span><span class="sxs-lookup"><span data-stu-id="24042-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="24042-105">Az áttekintési irányítópult két új szerepkört használ a partner Centerben, hogy az alkalmazottak hozzáférjenek a jelentésekhez – az Executive Report Viewer és a Report Viewer.</span><span class="sxs-lookup"><span data-stu-id="24042-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="24042-106">A vezetői jelentés megjelenítője szerepkör felhasználói hozzáférhetnek az összes jelentési adatkészlethez, míg a jelentés-megjelenítőben lévő felhasználók nem férhetnek hozzá a bizalmas adatkészletekhez, például a bevételekhez és az ügyfélhez vagy alkalmazottakhoz tartozó személyes adatokhoz.</span><span class="sxs-lookup"><span data-stu-id="24042-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="24042-107">A többi partner Center-szerepkörhöz hasonlóan a globális rendszergazda vagy a fiók rendszergazdája is hozzárendelheti a felhasználókat a szerepkörökhöz a felhasználói kezelés lapon.</span><span class="sxs-lookup"><span data-stu-id="24042-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="24042-108">A szerepkörök a teljes vállalaton belül, illetve adott MPN-hely (ek) esetében alkalmazhatók.</span><span class="sxs-lookup"><span data-stu-id="24042-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="24042-109">A megadott MPN-hely (ek) hez rendelt szerepkörök korlátozzák a felhasználót a csak a kiválasztott MPN-hely (ek) hez társított jelentési adat megtekintésére.</span><span class="sxs-lookup"><span data-stu-id="24042-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="24042-110">A partner az alábbi nézetből választhat ki egy vagy több helyet.</span><span class="sxs-lookup"><span data-stu-id="24042-110">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Az adott helyhez kapcsolódó partneri központ-keresési szerepkörök beállításainak megjelenítése a jelentéskészítő és a Executive Report Viewer számára.":::

>[!Note]
> <span data-ttu-id="24042-112">Azok a felhasználók, akik az MPN-rendszergazdák, január 20., 2020 automatikusan hozzáadódnak a vállalati szintű **Executive Report Viewer** szerepkörhöz az adott bérlő összes helyéhez.</span><span class="sxs-lookup"><span data-stu-id="24042-112">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="24042-113">Ezek a felhasználók így a jelentéseket ügyvezető jelentés megjelenítőként férhetnek hozzá a globális rendszergazda vagy a fiók rendszergazdája által igényelt kifejezett beavatkozás nélkül. A globális rendszergazdák és a rendszergazdák felülbírálják ezen felhasználók automatikusan hozzárendelt szerepköreit a képességek további növeléséhez vagy korlátozásához.</span><span class="sxs-lookup"><span data-stu-id="24042-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="24042-114">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="24042-114">Next steps</span></span>

- <span data-ttu-id="24042-115">További információ a [partner Center](partner-center-insights.md) -információkról és a különböző jelentésekről.</span><span class="sxs-lookup"><span data-stu-id="24042-115">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
