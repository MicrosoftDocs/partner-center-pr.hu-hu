---
title: Analytics használata az előfizetési elemzésekhez
ms.topic: article
ms.date: 11/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan használhatja az elemzést a partner Centerben az üzleti tevékenység jobb megismeréséhez, valamint arról, hogy az ügyfelek hogyan használják a megvásárolt licenceket.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3aec8c8abe6184be48fd54e0f76bc7e0c08e4792
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441880"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a><span data-ttu-id="c5499-103">Az előfizetés bevételének megismerése az Analytics használatával</span><span class="sxs-lookup"><span data-stu-id="c5499-103">Use analytics to learn more about subscription revenue</span></span>

<span data-ttu-id="c5499-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="c5499-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c5499-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="c5499-105">Global admin</span></span>
- <span data-ttu-id="c5499-106">MPN-partner rendszergazdája</span><span class="sxs-lookup"><span data-stu-id="c5499-106">MPN partner admin</span></span>

<span data-ttu-id="c5499-107">Egy CSP-vállalkozás fejlesztésének megtervezéséhez fontos tudni, hogy az ügyfelek hogyan használják a Microsoft termékeit.</span><span class="sxs-lookup"><span data-stu-id="c5499-107">Planning ways to develop your CSP business includes understanding how your customers use their Microsoft products.</span></span> <span data-ttu-id="c5499-108">Több lehetőség is van az adatok összegyűjtésére a partner Centerben, és a vállalaton és az ügyfeleken is gyűjthet adatokat a megvásárolt licencek használatával.</span><span class="sxs-lookup"><span data-stu-id="c5499-108">You have several options for gathering data in Partner Center, and you can gather data on both your business and on if and how your customers are using the licenses they've purchased.</span></span> <span data-ttu-id="c5499-109">Ha a CSP Direct modellben van, lehetősége van arra is, hogy a Power BI a partner Center Analytics alkalmazást is telepítse és használja a további adatok összegyűjtéséhez.</span><span class="sxs-lookup"><span data-stu-id="c5499-109">If you are in the CSP direct model, you also have the opportunity to install and use the Partner Center Analytics app for Power BI to gather additional data.</span></span>

## <a name="access-to-the-subscription-analytics"></a><span data-ttu-id="c5499-110">Hozzáférés az előfizetés-elemzéshez</span><span class="sxs-lookup"><span data-stu-id="c5499-110">Access to the Subscription Analytics</span></span>

1. <span data-ttu-id="c5499-111">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/home).</span><span class="sxs-lookup"><span data-stu-id="c5499-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>
1. <span data-ttu-id="c5499-112">A partner Center menüjéből válassza az **elemzés**, majd az **előfizetés-elemzés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c5499-112">From CSP in the Partner Center menu, select **Analyze**, and then select **Subscription analytics**.</span></span>

1. <span data-ttu-id="c5499-113">A jelenleg tizenkét hónapos CSP-bevétel megjelenik az oldal tetején.</span><span class="sxs-lookup"><span data-stu-id="c5499-113">The trailing twelve-month CSP revenue will be displayed at the top of the page</span></span>

:::image type="content" source="images/analytics/subscription1.png" alt-text="Előfizetés képernyő":::

## <a name="trailing-twelve-month-ttm-csp-revenue"></a><span data-ttu-id="c5499-115">Záró Twelve-Month (TTM) CSP-bevétel</span><span class="sxs-lookup"><span data-stu-id="c5499-115">Trailing Twelve-Month (TTM) CSP Revenue</span></span>

<span data-ttu-id="c5499-116">A 12 hónapos CSP-bevétel nyomon követő befizetése a felhőalapú megoldás szolgáltatói programjának bevételét jelenti USD-ben a partner globális fiók szintjén.</span><span class="sxs-lookup"><span data-stu-id="c5499-116">Trailing 12-month CSP revenue represents the trailing Cloud Solution Provider program revenue in USD at a Partner Global Account level.</span></span> <span data-ttu-id="c5499-117">A rendszer minden hónap nyolcadik napján frissíti az adatmennyiséget, hogy az előző hónap végéig a tizenkét hónapos bevételt jelenítse meg.</span><span class="sxs-lookup"><span data-stu-id="c5499-117">The data is refreshed on the eighth of every month, to display the trailing twelve-month revenue until the prior month.</span></span> <span data-ttu-id="c5499-118">Például szeptember 9-én a 2020-es rögzített időszakra vonatkozóan láthatja az TTM-t az 2020 augusztus 2019-ig terjedő időszakban.</span><span class="sxs-lookup"><span data-stu-id="c5499-118">For example, on 9 September 2020, you should be able to see the TTM for the fixed period of September 2019 to August 2020.</span></span>

<span data-ttu-id="c5499-119">A partner Centerben megjelenő bevétel a 12 hónapos rögzített időtartamra van kiszámítva, és nem módosítható rövidebb időszakra.</span><span class="sxs-lookup"><span data-stu-id="c5499-119">The revenue displayed on Partner Center is calculated for a fixed time interval of 12 months, and cannot be modified to a shorter time frame.</span></span>

<span data-ttu-id="c5499-120">A partner helyének fiókja szintjén megjelenő bevétel részletezésének megtekintéséhez:</span><span class="sxs-lookup"><span data-stu-id="c5499-120">To see a breakdown of the revenue at your Partner Location Account level:</span></span>

- <span data-ttu-id="c5499-121">Válassza ki a "részletek letöltése" hivatkozást, és töltsön le egy. TSV fájlt, amely megjeleníti a TTM bevételét az összes helyen.</span><span class="sxs-lookup"><span data-stu-id="c5499-121">Select the ‘Download Details’ link and download a .tsv file that displays the TTM revenue across all your locations.</span></span>

>[!NOTE] 
><span data-ttu-id="c5499-122">Előfordulhat, hogy a. TSV fájlban lévő MPN-azonosítók között az egyes TTM-bevételi számok összegzése nagyobb, mint a TTM megjelenő teljes bevétel.</span><span class="sxs-lookup"><span data-stu-id="c5499-122">Summing up the individual TTM Revenue numbers across MPN IDs in the .tsv file may appear to be greater than the overall TTM revenue you see displayed on Partner Center.</span></span> <span data-ttu-id="c5499-123">Ennek az az oka, hogy a bevételt a letöltött fájlban több partneri kapcsolattal rendelkező előfizetések esetében kétszer is megszámoljuk.</span><span class="sxs-lookup"><span data-stu-id="c5499-123">This is because the revenue may be double counted for subscriptions with multiple partner attributions in the downloaded file.</span></span>

## <a name="subscription-summary"></a><span data-ttu-id="c5499-124">Előfizetés összefoglalása</span><span class="sxs-lookup"><span data-stu-id="c5499-124">Subscription Summary</span></span>

<span data-ttu-id="c5499-125">A képernyő alsó fele az előfizetések összegzését jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="c5499-125">The lower half of the screen displays a summary of the subscriptions.</span></span> <span data-ttu-id="c5499-126">Használja a következő szűrőket a szükséges előfizetés részleteinek megtekintéséhez:</span><span class="sxs-lookup"><span data-stu-id="c5499-126">Use the following filters to see the necessary subscription details:</span></span>  

1. <span data-ttu-id="c5499-127">**Időtartam**: dönthet úgy, hogy megtekinti az előfizetés összegzését</span><span class="sxs-lookup"><span data-stu-id="c5499-127">**Duration**: You may opt to see the subscription summary for</span></span> 

- <span data-ttu-id="c5499-128">30D – elmúlt 30 nap</span><span class="sxs-lookup"><span data-stu-id="c5499-128">30D – Last 30 days</span></span>
- <span data-ttu-id="c5499-129">3M – elmúlt 3 hónap</span><span class="sxs-lookup"><span data-stu-id="c5499-129">3M – Last 3 months</span></span>
- <span data-ttu-id="c5499-130">6M – elmúlt 6 hónap</span><span class="sxs-lookup"><span data-stu-id="c5499-130">6M – Last 6 months</span></span>
- <span data-ttu-id="c5499-131">12M – elmúlt 12 hónap</span><span class="sxs-lookup"><span data-stu-id="c5499-131">12M – Last 12 months</span></span>

2. <span data-ttu-id="c5499-132">**Terméktípus**:</span><span class="sxs-lookup"><span data-stu-id="c5499-132">**Product Type**:</span></span>
 
- <span data-ttu-id="c5499-133">Office 365</span><span class="sxs-lookup"><span data-stu-id="c5499-133">Office 365</span></span>
- <span data-ttu-id="c5499-134">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c5499-134">Microsoft 365</span></span>
- <span data-ttu-id="c5499-135">Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="c5499-135">Dynamics 365</span></span>
- <span data-ttu-id="c5499-136">EMS</span><span class="sxs-lookup"><span data-stu-id="c5499-136">EMS</span></span>

<span data-ttu-id="c5499-137">Ezen szűrők alkalmazása nem befolyásolja a jelentés elején található TTM bevételi mérőszámot.</span><span class="sxs-lookup"><span data-stu-id="c5499-137">Applying these filters will not impact the TTM revenue metric at the top of this report.</span></span>


 
## <a name="next-steps"></a><span data-ttu-id="c5499-138">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="c5499-138">Next steps</span></span>

- [<span data-ttu-id="c5499-139">Elemezze, hogy az ügyfelek hogyan használják a megvásárolt licenceket</span><span class="sxs-lookup"><span data-stu-id="c5499-139">Analyze how your customers are using the licenses they purchased</span></span>](increasing-adoption-and-satisfaction.md)  
- [<span data-ttu-id="c5499-140">Az ügyféltevékenységi naplók megtekintése</span><span class="sxs-lookup"><span data-stu-id="c5499-140">View customer activity logs</span></span>](activity-logs.md)
- [<span data-ttu-id="c5499-141">A Power BIhez készült partner Center Analytics-alkalmazás</span><span class="sxs-lookup"><span data-stu-id="c5499-141">Partner Center Analytics app for Power BI</span></span>](power-bi-app-for-direct-partners.md)






