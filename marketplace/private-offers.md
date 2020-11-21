---
title: Privát ajánlatok az Azure Marketplace-en
description: Ismerje meg az Azure piactéren elérhető privát ajánlatokat.
ms.prod: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 055151f0420d642d591554a829dc21b69df84ebd
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007555"
---
# <a name="private-offers-in-azure-marketplace"></a><span data-ttu-id="50151-103">Privát ajánlatok az Azure Marketplace-en</span><span class="sxs-lookup"><span data-stu-id="50151-103">Private offers in Azure Marketplace</span></span>

<span data-ttu-id="50151-104">A privát ajánlatok szerint a kiadók egyéni csomagokat biztosítanak bizonyos ügyfeleknek.</span><span class="sxs-lookup"><span data-stu-id="50151-104">Private offers are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="50151-105">Ez a beállítás jelenleg csak az Azure Marketplace-en érhető el a Azure Portalban.</span><span class="sxs-lookup"><span data-stu-id="50151-105">This option is currently supported only in the Azure Marketplace experience in the Azure portal.</span></span> <span data-ttu-id="50151-106">A privát ajánlatok csak olyan fizetős ajánlatok esetén érhetők el, amelyek a Azure Portal vásárolhatók meg, és közvetlenül is telepíthetők.</span><span class="sxs-lookup"><span data-stu-id="50151-106">Private offers are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="50151-107">A kiadó nem tud privát ajánlatokat létrehozni a tanácsadási szolgáltatásokhoz, bármely olyan szolgáltatáshoz, amely hívási műveletként vagy ingyenes szolgáltatásként **kapcsolatba lép** , függetlenül attól, hogy telepíthető-e a portálról vagy sem.</span><span class="sxs-lookup"><span data-stu-id="50151-107">Publisher cannot create private offers for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-offers-in-the-azure-portal"></a><span data-ttu-id="50151-108">Privát ajánlatok keresése a Azure Portalban</span><span class="sxs-lookup"><span data-stu-id="50151-108">Find private offers in the Azure portal</span></span>

<span data-ttu-id="50151-109">Ha egy partner privát ajánlatot tesz közzé, a Azure Portal **piactér** szakaszában csak a jogosult felhasználók láthatók.</span><span class="sxs-lookup"><span data-stu-id="50151-109">When a partner publishes a private offer, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="50151-110">Ezeket a felhasználókat az előfizetés azonosítója vagy a bérlő azonosítója határozza meg az ajánlat típusától függően.</span><span class="sxs-lookup"><span data-stu-id="50151-110">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="50151-111">Ha Ön jogosult a privát ajánlatokra, kétféleképpen is megtalálhatja őket a portálon.</span><span class="sxs-lookup"><span data-stu-id="50151-111">If you are eligible for  private offers, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="50151-112">A privát ajánlatok jelenleg nem kereshetők vagy szűrhetők (kategóriánként) a Azure Portalban.</span><span class="sxs-lookup"><span data-stu-id="50151-112">Private offers are currently not searchable or filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="50151-113">A Azure Portal kattintson az **+ erőforrás létrehozása** vagy a "piactér" kifejezésre a **piactér** lapon való ugráshoz.</span><span class="sxs-lookup"><span data-stu-id="50151-113">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="50151-114">Ha privát ajánlatokra jogosult, látni fogja, hogy az oldal tetején elérhető-e az **Ön privát ajánlata** .</span><span class="sxs-lookup"><span data-stu-id="50151-114">If you are eligible for private offers, you will see the **You have private offers available** banner on the top of the page.</span></span> <span data-ttu-id="50151-115">Válassza a **privát ajánlatok megtekintése** lehetőséget a privát ajánlatok oldalának megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="50151-115">Select **View private offers** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Az a szalagcím, amely akkor jelenik meg, ha elérhetők a privát ajánlatok.":::

<span data-ttu-id="50151-117">Ha a privát ajánlatok szalagcímét látja, akkor a Product Gallery oldal aljára is görgetheti, és megtekintheti a privát ajánlatok egy részhalmazát.</span><span class="sxs-lookup"><span data-stu-id="50151-117">Alternately, if you see the private offers banner, you can also scroll to the bottom of the product gallery page and you will see a subset of your private offers.</span></span> <span data-ttu-id="50151-118">Válassza ki a hivatkozást, és **tekintse** meg a privát ajánlatok oldalát.</span><span class="sxs-lookup"><span data-stu-id="50151-118">Select the link to **See More** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/see-more-link.png" alt-text="A képernyő alján található privát ajánlatokat mutatja be, a továbbiak hivatkozással együtt.":::

## <a name="review-private-plans"></a><span data-ttu-id="50151-120">Privát csomagok áttekintése</span><span class="sxs-lookup"><span data-stu-id="50151-120">Review private plans</span></span>

<span data-ttu-id="50151-121">Egy privát ajánlat tulajdonképpen egy privát csomag egy ajánlaton belül.</span><span class="sxs-lookup"><span data-stu-id="50151-121">A private offer is actually a private plan within an offer.</span></span> <span data-ttu-id="50151-122">Minden ajánlat több, nyilvános és privát csomaggal is rendelkezhet, de a privát csomagok a nyilvános csomagokból származó külön listában jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="50151-122">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="50151-123">A rendelkezésre álló privát csomagokat a **csomagok** lapon tekintheti meg, amely a megkülönböztető **privát** jelvénysel van megjelölve:</span><span class="sxs-lookup"><span data-stu-id="50151-123">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Privátként megjelölt csomagok lapja.":::

<span data-ttu-id="50151-125">Ha egynél több előfizetéssel rendelkezik, az összes előfizetéséhez elérhető privát ajánlatokat fogja látni.</span><span class="sxs-lookup"><span data-stu-id="50151-125">If you have more than one subscription, you will see all private offers available for all your subscriptions.</span></span> <span data-ttu-id="50151-126">Ha a **Létrehozás** lehetőséget választja, a rendszer az erőforrás-létrehozási lapra irányítja az erőforrás konfigurálásának megkezdéséhez.</span><span class="sxs-lookup"><span data-stu-id="50151-126">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="50151-127">Ha a **Létrehozás** lehetőséget választja, és több előfizetéssel rendelkezik, de nem mindegyiket adja hozzá a privát csomaghoz, akkor az alapértelmezett előfizetés nem lehet a privát ajánlatra jogosult előfizetés.</span><span class="sxs-lookup"><span data-stu-id="50151-127">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private offer.</span></span> <span data-ttu-id="50151-128">Ebben az esetben válassza ki a megfelelő előfizetést.</span><span class="sxs-lookup"><span data-stu-id="50151-128">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="A hivatkozás azt mutatja, hogy több privát ajánlat áll rendelkezésre.":::

## <a name="next-steps"></a><span data-ttu-id="50151-130">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="50151-130">Next steps</span></span>

- [<span data-ttu-id="50151-131">Mi az Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="50151-131">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
