---
title: Privát csomagok a Microsoft AppSource
description: Privát csomagok beállítása a Microsoft AppSource (Azure Marketplace).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008582"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="7bc33-103">Privát csomagok a Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="7bc33-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="7bc33-104">A közzétevők a privát csomagokkal biztosítanak egyéni csomagokat adott ügyfeleknek.</span><span class="sxs-lookup"><span data-stu-id="7bc33-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="7bc33-105">Ez a lehetőség mostantól elérhető a Microsoft AppSource.</span><span class="sxs-lookup"><span data-stu-id="7bc33-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="7bc33-106">A Get it now call-to-action (Get **it now** call-to-action) segítségével privát csomagokat lehet értékesíteni az AppSource-ban szolgáltatott szoftver (SaaS) ajánlatokhoz.</span><span class="sxs-lookup"><span data-stu-id="7bc33-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="7bc33-107">Privát csomag lekérte az ISV-t</span><span class="sxs-lookup"><span data-stu-id="7bc33-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="7bc33-108">Ahhoz, hogy egy privát csomag elérhető legyen az AppSource-ban, közvetlenül az ISV-vel kell kapcsolatba lépnie, és egyeztetni kell egy egyéni árat és műszaki specifikációkat.</span><span class="sxs-lookup"><span data-stu-id="7bc33-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="7bc33-109">Amint a magánhálózati csomag feltételeit elfogadta, a isV létrehoz Önnek egy tervet, és hozzárendeli azt a szervezet bérlőazonosítójának, amelyet meg kell adnia.</span><span class="sxs-lookup"><span data-stu-id="7bc33-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="7bc33-110">A bérlőazonosító megkeresása</span><span class="sxs-lookup"><span data-stu-id="7bc33-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="7bc33-111">Az AppSource jobb felső sarkában válassza a fiókprofil ikonját, majd a **Bérlő megtekintése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7bc33-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="7bc33-112">Másolja ki a bérlőazonosítót, és adja meg az ISV-nek.</span><span class="sxs-lookup"><span data-stu-id="7bc33-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Bemutatja, hogyan találhatja meg a bérlőazonosítót.":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="7bc33-114">Privát csomag megkeresi az AppSource-ban</span><span class="sxs-lookup"><span data-stu-id="7bc33-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="7bc33-115">Akár 48 órát is igénybe vehet, miután az ISV közzétette az új privát tervet, mielőtt az megjelent volna az AppSource-ban.</span><span class="sxs-lookup"><span data-stu-id="7bc33-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="7bc33-116">A bérlőazonosítóhoz társított privát csomagok kereséséhez válassza a Privát csomagok **(Zárolás** ikon) lehetőséget az AppSource jobb felső sarkában.</span><span class="sxs-lookup"><span data-stu-id="7bc33-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="A felső eszköztár zárolás ikonját (lakat ikonját) jeleníti meg.":::

<span data-ttu-id="7bc33-118">Ha nincs bejelentkezve, egy üzenet fogja kérni erre.</span><span class="sxs-lookup"><span data-stu-id="7bc33-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="7bc33-119">Ezután a Csomagok + díjszabás lapon vásárolhatja meg a bérlőazonosítóhoz társított privát **csomagokat.**</span><span class="sxs-lookup"><span data-stu-id="7bc33-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Megjeleníti a privát ajánlatokat a csomag és a díjszabás lapon.":::

<span data-ttu-id="7bc33-121">Ha a privát csomagok nem érhetők el a bérlő számára, egy üzenet jelenik meg, amely szerint nem rendelkezik privát csomagokkal vagy ajánlatokkal.</span><span class="sxs-lookup"><span data-stu-id="7bc33-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="7bc33-122">Privát csomag vásárlása</span><span class="sxs-lookup"><span data-stu-id="7bc33-122">Purchase a private plan</span></span>

<span data-ttu-id="7bc33-123">A isV-k egy vagy több privát csomagból is tartalmazhatnak egy ajánlatot.</span><span class="sxs-lookup"><span data-stu-id="7bc33-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="7bc33-124">Minden ajánlat nyilvános és privát csomagokkal is lehet, de a privát csomagok egy külön ajánlatlista-oldalon jelennek meg, amely az oldal jobb felső sarkában található Privát ajánlatok ikonról (lakat) érhető el.</span><span class="sxs-lookup"><span data-stu-id="7bc33-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="7bc33-125">Az elérhető privát csomagok a Csomagok **+ díjszabás lapon jelennek** meg. A privát csomagoknak van egy kék jelvényük.</span><span class="sxs-lookup"><span data-stu-id="7bc33-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="A privát ajánlatok melletti kék privát ajánlat jelvényt jeleníti meg.":::

<span data-ttu-id="7bc33-127">Egy kiválasztott csomag megvásárlásához válassza a **Beszerzés most lehetőséget,** és kövesse a megadott lépéseket.</span><span class="sxs-lookup"><span data-stu-id="7bc33-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7bc33-128">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="7bc33-128">Next steps</span></span>

- [<span data-ttu-id="7bc33-129">Mi az a Microsoft AppSource?</span><span class="sxs-lookup"><span data-stu-id="7bc33-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
