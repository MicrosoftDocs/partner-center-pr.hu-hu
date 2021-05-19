---
title: Elemzés használata az előfizetési elemzésekhez
ms.topic: article
ms.date: 11/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan használhatja a Partnerközpont, hogy jobban megértse vállalkozását, és hogy az ügyfelek hogyan használják a megvásárolt licenceket.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7dab3469b885f693ba8498e8a07eb120b8f07021
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147207"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a><span data-ttu-id="e1c01-103">Elemzések használata az előfizetés bevételével kapcsolatos további információkért</span><span class="sxs-lookup"><span data-stu-id="e1c01-103">Use analytics to learn more about subscription revenue</span></span>

<span data-ttu-id="e1c01-104">**Megfelelő szerepkörök:** Globális rendszergazdai | MPN-partneri rendszergazda</span><span class="sxs-lookup"><span data-stu-id="e1c01-104">**Appropriate roles**: Global admin | MPN partner admin</span></span>

<span data-ttu-id="e1c01-105">Egy CSP-vállalkozás fejlesztésének megtervezéséhez fontos tudni, hogy az ügyfelek hogyan használják a Microsoft termékeit.</span><span class="sxs-lookup"><span data-stu-id="e1c01-105">Planning ways to develop your CSP business includes understanding how your customers use their Microsoft products.</span></span> <span data-ttu-id="e1c01-106">Számos lehetőség áll rendelkezésre az adatok gyűjtésére a Partnerközpont, és adatokat gyűjthet a vállalatról, valamint arról, hogy az ügyfelek hogyan és hogyan használják a megvásárolt licenceket.</span><span class="sxs-lookup"><span data-stu-id="e1c01-106">You have several options for gathering data in Partner Center, and you can gather data on both your business and on if and how your customers are using the licenses they've purchased.</span></span> <span data-ttu-id="e1c01-107">Ha Ön a közvetlen CSP-modellben van, lehetősége van telepíteni és használni a Partnerközpont adatelemzési alkalmazás a Power BI-hoz további adatok gyűjtése érdekében.</span><span class="sxs-lookup"><span data-stu-id="e1c01-107">If you are in the CSP direct model, you also have the opportunity to install and use the Partner Center Analytics app for Power BI to gather additional data.</span></span>

## <a name="access-to-the-subscription-analytics"></a><span data-ttu-id="e1c01-108">Hozzáférés az Előfizetési elemzéshez</span><span class="sxs-lookup"><span data-stu-id="e1c01-108">Access to the Subscription Analytics</span></span>

1. <span data-ttu-id="e1c01-109">Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="e1c01-109">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>
1. <span data-ttu-id="e1c01-110">A csp-Partnerközpont válassza az **Elemzés,** majd az **Előfizetés-elemzés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e1c01-110">From CSP in the Partner Center menu, select **Analyze**, and then select **Subscription analytics**.</span></span>

1. <span data-ttu-id="e1c01-111">A záró 12 hónapos CSP-bevétel az oldal tetején jelenik meg</span><span class="sxs-lookup"><span data-stu-id="e1c01-111">The trailing twelve-month CSP revenue will be displayed at the top of the page</span></span>

:::image type="content" source="images/analytics/subscription1.png" alt-text="Előfizetés képernyő":::

## <a name="trailing-twelve-month-ttm-csp-revenue"></a><span data-ttu-id="e1c01-113">Záró Twelve-Month (TTM) CSP-bevétel</span><span class="sxs-lookup"><span data-stu-id="e1c01-113">Trailing Twelve-Month (TTM) CSP Revenue</span></span>

<span data-ttu-id="e1c01-114">A 12 hónapos CSP-bevétel záródása a program Felhőszolgáltató bevételét jelzi USD-ben a partner globális fiókja szintjén.</span><span class="sxs-lookup"><span data-stu-id="e1c01-114">Trailing 12-month CSP revenue represents the trailing Cloud Solution Provider program revenue in USD at a Partner Global Account level.</span></span> <span data-ttu-id="e1c01-115">Az adatok minden hónap első napján frissülnek, így az előző hónap utolsó tizenkettő havi bevételét jelenítik meg.</span><span class="sxs-lookup"><span data-stu-id="e1c01-115">The data is refreshed on the eighth of every month, to display the trailing twelve-month revenue until the prior month.</span></span> <span data-ttu-id="e1c01-116">2020. szeptember 9-én például látnia kell a 2019. szeptember és 2020. augusztus között rögzített időtartamra vonatkozó TTM-et.</span><span class="sxs-lookup"><span data-stu-id="e1c01-116">For example, on 9 September 2020, you should be able to see the TTM for the fixed period of September 2019 to August 2020.</span></span>

<span data-ttu-id="e1c01-117">A rendszer a Partnerközpont rögzített, 12 hónapos időszakra számítja ki a bevételt, és nem módosítható rövidebb időszakra.</span><span class="sxs-lookup"><span data-stu-id="e1c01-117">The revenue displayed on Partner Center is calculated for a fixed time interval of 12 months, and cannot be modified to a shorter time frame.</span></span>

<span data-ttu-id="e1c01-118">A bevétel részletezése a partnerhelyi fiók szintjén:</span><span class="sxs-lookup"><span data-stu-id="e1c01-118">To see a breakdown of the revenue at your Partner Location Account level:</span></span>

- <span data-ttu-id="e1c01-119">Válassza a Részletek letöltése hivatkozást, és töltsön le egy .tsv fájlt, amely megjeleníti a TTM-bevételt az összes helyen.</span><span class="sxs-lookup"><span data-stu-id="e1c01-119">Select the ‘Download Details’ link and download a .tsv file that displays the TTM revenue across all your locations.</span></span>

>[!NOTE] 
><span data-ttu-id="e1c01-120">Úgy tűnik, hogy a .tsv fájlban az egyes TTM-bevételi számok összege több MPN-azonosítóban nagyobb, mint a jelen fájlban látható teljes TTM-Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="e1c01-120">Summing up the individual TTM Revenue numbers across MPN IDs in the .tsv file may appear to be greater than the overall TTM revenue you see displayed on Partner Center.</span></span> <span data-ttu-id="e1c01-121">Ennek az az oka, hogy a letöltött fájlban található több partneri forrásmegjelöléssel rendelkező előfizetések bevétele kétszer is beleszámolhat.</span><span class="sxs-lookup"><span data-stu-id="e1c01-121">This is because the revenue may be double counted for subscriptions with multiple partner attributions in the downloaded file.</span></span>

## <a name="subscription-summary"></a><span data-ttu-id="e1c01-122">Előfizetés összegzése</span><span class="sxs-lookup"><span data-stu-id="e1c01-122">Subscription Summary</span></span>

<span data-ttu-id="e1c01-123">A képernyő alsó felében megjelenik az előfizetések összegzése.</span><span class="sxs-lookup"><span data-stu-id="e1c01-123">The lower half of the screen displays a summary of the subscriptions.</span></span> <span data-ttu-id="e1c01-124">A következő szűrőkkel tekintse meg a szükséges előfizetési adatokat:</span><span class="sxs-lookup"><span data-stu-id="e1c01-124">Use the following filters to see the necessary subscription details:</span></span>  

1. <span data-ttu-id="e1c01-125">**Időtartam:** Dönthet úgy, hogy a következő előfizetési összefoglalást látja:</span><span class="sxs-lookup"><span data-stu-id="e1c01-125">**Duration**: You may opt to see the subscription summary for</span></span> 

- <span data-ttu-id="e1c01-126">30D – Az elmúlt 30 nap</span><span class="sxs-lookup"><span data-stu-id="e1c01-126">30D – Last 30 days</span></span>
- <span data-ttu-id="e1c01-127">3M – Az elmúlt 3 hónap</span><span class="sxs-lookup"><span data-stu-id="e1c01-127">3M – Last 3 months</span></span>
- <span data-ttu-id="e1c01-128">6M – Az elmúlt 6 hónap</span><span class="sxs-lookup"><span data-stu-id="e1c01-128">6M – Last 6 months</span></span>
- <span data-ttu-id="e1c01-129">12 M – Az elmúlt 12 hónap</span><span class="sxs-lookup"><span data-stu-id="e1c01-129">12M – Last 12 months</span></span>

2. <span data-ttu-id="e1c01-130">**Terméktípus:**</span><span class="sxs-lookup"><span data-stu-id="e1c01-130">**Product Type**:</span></span>
 
- <span data-ttu-id="e1c01-131">Office 365</span><span class="sxs-lookup"><span data-stu-id="e1c01-131">Office 365</span></span>
- <span data-ttu-id="e1c01-132">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e1c01-132">Microsoft 365</span></span>
- <span data-ttu-id="e1c01-133">Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="e1c01-133">Dynamics 365</span></span>
- <span data-ttu-id="e1c01-134">EMS</span><span class="sxs-lookup"><span data-stu-id="e1c01-134">EMS</span></span>

<span data-ttu-id="e1c01-135">A szűrők alkalmazása nem befolyásolja a jelentés tetején található TTM bevételi metrikát.</span><span class="sxs-lookup"><span data-stu-id="e1c01-135">Applying these filters will not impact the TTM revenue metric at the top of this report.</span></span>


 
## <a name="next-steps"></a><span data-ttu-id="e1c01-136">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="e1c01-136">Next steps</span></span>

- [<span data-ttu-id="e1c01-137">Annak elemzése, hogy az ügyfelek hogyan használják a megvásárolt licenceket</span><span class="sxs-lookup"><span data-stu-id="e1c01-137">Analyze how your customers are using the licenses they purchased</span></span>](increasing-adoption-and-satisfaction.md)  
- [<span data-ttu-id="e1c01-138">Az ügyféltevékenységi naplók megtekintése</span><span class="sxs-lookup"><span data-stu-id="e1c01-138">View customer activity logs</span></span>](activity-logs.md)
- [<span data-ttu-id="e1c01-139">Partnerközpont adatelemzési alkalmazás a Power BI-hoz</span><span class="sxs-lookup"><span data-stu-id="e1c01-139">Partner Center Analytics app for Power BI</span></span>](power-bi-app-for-direct-partners.md)






