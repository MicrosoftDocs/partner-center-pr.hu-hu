---
title: Privát ajánlatok a Azure Marketplace
description: További információ a privát ajánlatokról a Azure Marketplace.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 06/03/2021
ms.openlocfilehash: 55d0716b183e9e8905e631447e547396d6f55404
ms.sourcegitcommit: 9cb6bc9df20540f812b7932f88e520976c1aa85a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/06/2021
ms.locfileid: "111534180"
---
# <a name="private-plans-in-azure-marketplace"></a><span data-ttu-id="96094-103">Privát csomagok a Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="96094-103">Private plans in Azure Marketplace</span></span>

<span data-ttu-id="96094-104">A közzétevők a privát csomagok alapján nyújtanak egyéni csomagokat adott ügyfeleknek.</span><span class="sxs-lookup"><span data-stu-id="96094-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="96094-105">A privát csomagok csak fizetős ajánlatokhoz érhetők el, amelyek megvásárolhatók és közvetlenül telepíthetők a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="96094-105">Private plans are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="96094-106">A közzétevők nem hozhatnak létre  privát csomagokat tanácsadási szolgáltatásokhoz, olyan szolgáltatásokhoz, amelyekhez a Kapcsolatfelvétel műveletként vagy bármely ingyenes szolgáltatással rendelkezik, függetlenül attól, hogy telepíthetők-e a portálról vagy sem.</span><span class="sxs-lookup"><span data-stu-id="96094-106">Publishers cannot create private plans for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-plans-in-the-azure-portal"></a><span data-ttu-id="96094-107">Privát csomagok megkeresi a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="96094-107">Find private plans in the Azure portal</span></span>

<span data-ttu-id="96094-108">Amikor egy partner közzétesz egy privát tervet, az  csak a jogosult felhasználók számára látható a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="96094-108">When a partner publishes a private plan, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="96094-109">Ezek a felhasználók az ajánlat típusától függően előfizetés-azonosító vagy bérlőazonosító alapján vannak meghatározva.</span><span class="sxs-lookup"><span data-stu-id="96094-109">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="96094-110">Ha jogosult privát csomagokra, kétféleképpen találhatja meg őket a portálon.</span><span class="sxs-lookup"><span data-stu-id="96094-110">If you are eligible for private plans, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="96094-111">A privát csomagok kereshetők, de nem szűrhetők (kategóriák szerint) a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="96094-111">Private plans are searchable but not filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="96094-112">A Azure Portal válassza az **+ Erőforrás** létrehozása lehetőséget, vagy keressen a "marketplace" kifejezésre a **Marketplace oldalának kiválasztásához.**</span><span class="sxs-lookup"><span data-stu-id="96094-112">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="96094-113">Ha jogosult privát csomagokra, az  oldal tetején megjelenik a Privát csomagok érhetőek el szalagcím.</span><span class="sxs-lookup"><span data-stu-id="96094-113">If you are eligible for private plans, you will see the **You have private plans available** banner on the top of the page.</span></span> <span data-ttu-id="96094-114">Válassza **a Privát ajánlatok és csomagok megtekintése lehetőséget** a privát csomagok oldalának megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="96094-114">Select **View private offers + plans** to go to your private plans page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="A szalagcím, amely akkor jelenik meg, ha vannak elérhető privát csomagok.":::

## <a name="review-private-plans"></a><span data-ttu-id="96094-116">Privát csomagok áttekintése</span><span class="sxs-lookup"><span data-stu-id="96094-116">Review private plans</span></span>

<span data-ttu-id="96094-117">A privát csomag egy ajánlat több csomagja részét képezi.</span><span class="sxs-lookup"><span data-stu-id="96094-117">A private plan is part of several plans in an offer.</span></span> <span data-ttu-id="96094-118">Minden ajánlat több, nyilvános és privát csomagtal is lehet, de a privát csomagok a nyilvános csomagoktól külön listában jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="96094-118">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="96094-119">Az elérhető privát csomagokat a **Plans** (Csomagok) lapon láthatja, és egy privát jelvény **jelöli:**</span><span class="sxs-lookup"><span data-stu-id="96094-119">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Privátként megjelölt csomagok oldala.":::

<span data-ttu-id="96094-121">Ha egynél több előfizetéssel rendelkezik, az összes előfizetéséhez elérhető privát csomagok érhetők el.</span><span class="sxs-lookup"><span data-stu-id="96094-121">If you have more than one subscription, you will see all private plans available for all your subscriptions.</span></span> <span data-ttu-id="96094-122">Ha a **Létrehozás lehetőséget választja,** a rendszer az erőforrás-létrehozási oldalra irányítva elkezdi konfigurálni az erőforrást.</span><span class="sxs-lookup"><span data-stu-id="96094-122">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="96094-123">Ha a **Létrehozás lehetőséget** választja, és több előfizetéssel rendelkezik, de nem mindegyiket adja hozzá a privát csomaghoz, előfordulhat, hogy az alapértelmezett előfizetés nem jogosult erre a privát csomagra.</span><span class="sxs-lookup"><span data-stu-id="96094-123">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private plan.</span></span> <span data-ttu-id="96094-124">Ebben az esetben válassza ki a megfelelő előfizetést.</span><span class="sxs-lookup"><span data-stu-id="96094-124">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="A további privát csomagokra mutató hivatkozás.":::

## <a name="next-steps"></a><span data-ttu-id="96094-126">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="96094-126">Next steps</span></span>

- [<span data-ttu-id="96094-127">Mi az Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="96094-127">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
