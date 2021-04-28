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
ms.openlocfilehash: a6af9c7d674d1956332a564628b6b2ea0b1796f6
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120783"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="5c04c-104">Szerepköralapú hozzáférés-vezérlés a Partnerközpont Insights irányítópulthoz</span><span class="sxs-lookup"><span data-stu-id="5c04c-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="5c04c-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="5c04c-105">**Appropriate roles**</span></span>

- <span data-ttu-id="5c04c-106">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="5c04c-106">Global admin</span></span>
- <span data-ttu-id="5c04c-107">Rendszergazdai ügynök</span><span class="sxs-lookup"><span data-stu-id="5c04c-107">Admin agent</span></span>
- <span data-ttu-id="5c04c-108">Jelentésmegjelenítő</span><span class="sxs-lookup"><span data-stu-id="5c04c-108">Report viewer</span></span>
- <span data-ttu-id="5c04c-109">Vezetői jelentésmegjelenítő</span><span class="sxs-lookup"><span data-stu-id="5c04c-109">Executive report viewer</span></span>

<span data-ttu-id="5c04c-110">Az Elemzések irányítópult két új szerepkört használ a Partnerközpont a jelentésekhez való alkalmazotti hozzáférés kezeléséhez : a Vezetői jelentésmegjelenítőt és a Jelentésmegjelenítőt.</span><span class="sxs-lookup"><span data-stu-id="5c04c-110">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="5c04c-111">A Vezetői jelentésmegjelenítő szerepkörben a felhasználók az összes jelentési adathalmazhoz hozzáférhetnek, míg a Jelentésmegjelenítő szerepkör felhasználói nem férhetnek hozzá olyan bizalmas adatkészlethez, mint a bevétel és az ügyfél/alkalmazott személyes adatai.</span><span class="sxs-lookup"><span data-stu-id="5c04c-111">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="5c04c-112">Ahogy a többi Partnerközpont, a globális rendszergazda vagy a fiók rendszergazdája is hozzárendelhet felhasználókat ezekhez a szerepkörökhöz a Felhasználókezelés lapon.</span><span class="sxs-lookup"><span data-stu-id="5c04c-112">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="5c04c-113">A szerepkörök a teljes vállalatra vagy adott MPN-helyre alkalmazhatók.</span><span class="sxs-lookup"><span data-stu-id="5c04c-113">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="5c04c-114">Az adott MPN-hely(ék) számára hozzárendelt szerepkörök korlátozzák, hogy a felhasználó csak a kiválasztott MPN-hely(ekkel) társított jelentésadatokat megtekintsen.</span><span class="sxs-lookup"><span data-stu-id="5c04c-114">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="5c04c-115">A partner az alábbi nézetben kiválaszthat egy vagy több helyet.</span><span class="sxs-lookup"><span data-stu-id="5c04c-115">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="A Jelentésmegjelenítő és Partnerközpont jelentésmegjelenítő Insights-szerepkör-beállításainak helyspecifikus adatait jeleníti meg.":::

>[!Note]
> <span data-ttu-id="5c04c-117">Azok a felhasználók, akik 2020. január 20-án MPN-rendszergazdák, automatikusan hozzáadódnak a vállalati Szintű Vezetői jelentésmegjelenítő szerepkörhöz az adott bérlő összes helyéhez. </span><span class="sxs-lookup"><span data-stu-id="5c04c-117">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="5c04c-118">Ezek a felhasználók így a globális rendszergazda vagy a fiók-rendszergazda kifejezett beavatkozása nélkül is hozzáférhetnek a jelentésekhez vezetői jelentés megtekintőjeként. A globális rendszergazdák és a fiókgazdák felülbírálhatják ezen felhasználók automatikusan hozzárendelt szerepköreit a képességeik további növelése vagy korlátozása érdekében.</span><span class="sxs-lookup"><span data-stu-id="5c04c-118">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5c04c-119">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="5c04c-119">Next steps</span></span>

- <span data-ttu-id="5c04c-120">További információ az [Partnerközpont elemzésekről](partner-center-insights.md) és a különböző jelentésekről.</span><span class="sxs-lookup"><span data-stu-id="5c04c-120">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
