---
title: Partnerközpont Elemzések hozzáférés
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg az egyes jelentések Partnerközpont Elemzések szerepköröket. Ezek közé tartozik a Vezetői jelentésmegjelenítő és a Jelentésmegjelenítő szerepkör.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 836ae2ab193437fca501dc5c5713a4fe09b49ef4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376611"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="20461-104">Szerepköralapú hozzáférés-vezérlés a Partnerközpont Elemzések irányítópulthoz</span><span class="sxs-lookup"><span data-stu-id="20461-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="20461-105">**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök | Jelentésmegjelenítő | Vezetői jelentésmegjelenítő</span><span class="sxs-lookup"><span data-stu-id="20461-105">**Appropriate roles**: Global admin | Admin agent | Report viewer | Executive report viewer</span></span>

<span data-ttu-id="20461-106">A Elemzések irányítópult két új szerepkört használ a Partnerközpont az alkalmazottak jelentésekhez való hozzáférésének kezeléséhez : a Vezetői jelentésmegjelenítőt és a Jelentésmegjelenítőt.</span><span class="sxs-lookup"><span data-stu-id="20461-106">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="20461-107">A Vezetői jelentésmegjelenítő szerepkörben a felhasználók az összes jelentéskészítési adathalmazhoz hozzáférhetnek, míg a Jelentésmegjelenítő szerepkör felhasználói nem férhetnek hozzá olyan bizalmas adatkészlethez, mint a bevétel és az ügyfél/alkalmazott személyes adatai.</span><span class="sxs-lookup"><span data-stu-id="20461-107">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="20461-108">Mint minden Partnerközpont, a globális rendszergazda vagy a fiók rendszergazdája is hozzárendelhet felhasználókat ezekhez a szerepkörökhöz a Felhasználókezelés lapon.</span><span class="sxs-lookup"><span data-stu-id="20461-108">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="20461-109">A szerepkörök a teljes vállalatra vagy adott Microsoft Partner Network (MPN) alkalmazhatók.</span><span class="sxs-lookup"><span data-stu-id="20461-109">The roles can be applicable across the entire company or for specific Microsoft Partner Network (MPN) location(s).</span></span> <span data-ttu-id="20461-110">Az adott MPN-hely(ék) számára hozzárendelt szerepkörök korlátozzák a felhasználót a csak a kiválasztott MPN-hely(ekkel) társított jelentésadatok megtekintésére.</span><span class="sxs-lookup"><span data-stu-id="20461-110">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="20461-111">A partner az alábbi nézetben kiválaszthat egy vagy több helyet.</span><span class="sxs-lookup"><span data-stu-id="20461-111">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/insights/roles.png" alt-text="A Jelentésmegjelenítő és Partnerközpont Elemzések jelentésmegjelenítő szerepkör-beállításainak helyspecifikus beállításait jeleníti meg.":::

>[!Note]
> <span data-ttu-id="20461-113">Azok a felhasználók, akik 2020. január 20-án MPN-partneri  rendszergazdák, automatikusan hozzáadódnak a vállalati szintű Vezetői jelentésmegjelenítő szerepkörhöz az adott bérlő összes helyéhez.</span><span class="sxs-lookup"><span data-stu-id="20461-113">Users who are MPN partner admins as of January 20, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="20461-114">Ezek a felhasználók így a globális rendszergazda vagy a fiók-rendszergazda kifejezett beavatkozása nélkül is hozzáférhetnek a jelentésekhez vezetői jelentésmegjelenítőként. A globális rendszergazdák és a fiókgazdák felülbírálhatják ezen felhasználók automatikusan hozzárendelt szerepköreit a képességeik további növelése vagy korlátozása érdekében.</span><span class="sxs-lookup"><span data-stu-id="20461-114">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="20461-115">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="20461-115">Next steps</span></span>

- <span data-ttu-id="20461-116">További információ a [Partnerközpont Elemzések](partner-center-insights.md) és a különböző jelentésekről.</span><span class="sxs-lookup"><span data-stu-id="20461-116">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
