---
title: Partnerközpont Insights szerepköralapú hozzáférése
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megismeri az Insights-jelentések Partnerközpont szerepköröket. Ezek közé tartozik a Vezetői jelentésmegjelenítő és a Jelentésmegjelenítő szerepkör.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 803c299311f129c4842a92a27abd9b9addb49f17
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854434"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="dec51-104">Szerepköralapú hozzáférés-vezérlés a Partnerközpont Insights irányítópulthoz</span><span class="sxs-lookup"><span data-stu-id="dec51-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="dec51-105">**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök | Jelentésmegjelenítő | Vezetői jelentésmegjelenítő</span><span class="sxs-lookup"><span data-stu-id="dec51-105">**Appropriate roles**: Global admin | Admin agent | Report viewer | Executive report viewer</span></span>

<span data-ttu-id="dec51-106">Az Elemzések irányítópult két új szerepkört használ a Partnerközpont a jelentésekhez való alkalmazotti hozzáférés kezeléséhez – a Vezetői jelentésmegjelenítőt és a Jelentésmegjelenítőt.</span><span class="sxs-lookup"><span data-stu-id="dec51-106">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="dec51-107">A Vezetői jelentésmegjelenítő szerepkörben a felhasználók az összes jelentéskészítési adathalmazhoz hozzáférhetnek, míg a Jelentésmegjelenítő szerepkör felhasználói nem férhetnek hozzá a bizalmas adatkészletekhez, például a bevételhez és az ügyfelek/alkalmazottak személyes adataihoz.</span><span class="sxs-lookup"><span data-stu-id="dec51-107">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="dec51-108">Mint minden Partnerközpont, a globális rendszergazda vagy a fiók rendszergazdája is hozzárendelhet felhasználókat ezekhez a szerepkörökhöz a Felhasználókezelés lapon.</span><span class="sxs-lookup"><span data-stu-id="dec51-108">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="dec51-109">A szerepkörök a teljes vállalatra vagy adott MPN-helyre alkalmazhatók.</span><span class="sxs-lookup"><span data-stu-id="dec51-109">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="dec51-110">Az adott MPN-hely(ék) számára hozzárendelt szerepkörök korlátozzák a felhasználót a csak a kiválasztott MPN-hely(ekkel) társított jelentésadatok megtekintésére.</span><span class="sxs-lookup"><span data-stu-id="dec51-110">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="dec51-111">A partner az alábbi nézetben kiválaszthat egy vagy több helyet.</span><span class="sxs-lookup"><span data-stu-id="dec51-111">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Megjeleníti a jelentésmegjelenítő és Partnerközpont Insights szerepkör-beállításainak helyspecifikus beállításait.":::

>[!Note]
> <span data-ttu-id="dec51-113">Azok a felhasználók, akik 2020. január 20-án MPN-rendszergazdák, automatikusan hozzáadódnak a vállalati Szintű Vezetői jelentésmegjelenítő szerepkörhöz az adott bérlő összes helyéhez. </span><span class="sxs-lookup"><span data-stu-id="dec51-113">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="dec51-114">Ezek a felhasználók így a globális rendszergazda vagy a fiók-rendszergazda kifejezett beavatkozása nélkül is hozzáférhetnek a jelentésekhez vezetői jelentés megtekintőjeként. A globális rendszergazdák és a fiókgazdák felülbírálhatják ezen felhasználók automatikusan hozzárendelt szerepköreit a képességeik további növelése vagy korlátozása érdekében.</span><span class="sxs-lookup"><span data-stu-id="dec51-114">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="dec51-115">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="dec51-115">Next steps</span></span>

- <span data-ttu-id="dec51-116">További információ az [Partnerközpont elemzésekről](partner-center-insights.md) és a különböző jelentésekről.</span><span class="sxs-lookup"><span data-stu-id="dec51-116">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
