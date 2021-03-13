---
title: Átruházási jogosultság – az előfizetés számlázási fiókok közötti továbbítására vonatkozó irányelvek, Azure Marketplace
description: A kereskedelmi ellenőrzésekre vonatkozó irányelvek a Azure Portalban lévő számlázási fiókok közötti előfizetés átadása előtt.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412556"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="84abe-103">Az előfizetés számlázási fiókok közötti átvitelének jogosultsága</span><span class="sxs-lookup"><span data-stu-id="84abe-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="84abe-104">Az [előfizetést átviheti](/azure/cost-management-billing/understand/subscription-transfer) az egyik számlázási fiókból a másikba a Azure Portal számlázási szakaszában.</span><span class="sxs-lookup"><span data-stu-id="84abe-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="84abe-105">Az átvitel előtt a rendszer az előfizetést a harmadik féltől származó termékek esetében ellenőrzi.</span><span class="sxs-lookup"><span data-stu-id="84abe-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="84abe-106">Az átvitel csak akkor engedélyezett, ha az *összes* termék el van távolítva az átvitelre (lásd az alábbi [feltételeket](#criteria-for-transfer-approval-or-denial) ).</span><span class="sxs-lookup"><span data-stu-id="84abe-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="84abe-107">A rendszer a következő lépések elvégzése érdekében a megfelelő hibaüzeneteket fogja létrehozni a nem egyértelmű alkalmazások számára.</span><span class="sxs-lookup"><span data-stu-id="84abe-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="84abe-108">Ez a cikk nem vonatkozik az SaaS-ajánlatokra, mert az SaaS-erőforrások egy bérlőhöz, nem pedig előfizetéshez vannak csatolva.</span><span class="sxs-lookup"><span data-stu-id="84abe-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="84abe-109">Az SaaS-erőforrások az egyik számlázási fiókból a másikba vihetők át, de az erőforrás és az Azure-támogatás támogatási kérelemként történik.</span><span class="sxs-lookup"><span data-stu-id="84abe-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="84abe-110">Az átvitel jóváhagyásának vagy elutasításának feltételei</span><span class="sxs-lookup"><span data-stu-id="84abe-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="84abe-111">Az előfizetés nem vihető át, ha a harmadik féltől származó alkalmazásai megfelelnek a következő feltételeknek:</span><span class="sxs-lookup"><span data-stu-id="84abe-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="84abe-112">A célként megadott fiók kereskedelmi jellegű, és az alkalmazás leválasztása partnereken keresztül történik.</span><span class="sxs-lookup"><span data-stu-id="84abe-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="84abe-113">Az alkalmazás a kiválasztott partnerek számára választható, és a cél fiók nem szerepel az engedélyezési listán.</span><span class="sxs-lookup"><span data-stu-id="84abe-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="84abe-114">Az ajánlat előzetes ajánlat volt a múltban a kiválasztott előfizetésekhez, vagy egy privát ajánlat volt, és az előfizetés már nem szerepel az engedélyezési listán.</span><span class="sxs-lookup"><span data-stu-id="84abe-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="84abe-115">Az új számlázási fiók olyan régióban található, amely eltér az ajánlat eladásának helyétől, és az ajánlat nem értékesíthető ebben a régióban.</span><span class="sxs-lookup"><span data-stu-id="84abe-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="84abe-116">A letiltott átvitel mindaddig érvényben marad, amíg el nem távolítja az erőforrást az előfizetésből, amely után újra próbálkozhat az átvitelsel.</span><span class="sxs-lookup"><span data-stu-id="84abe-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="84abe-117">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="84abe-117">Next steps</span></span>

[<span data-ttu-id="84abe-118">Támogatás kérése Microsoft AppSource és az Azure Marketplace-en</span><span class="sxs-lookup"><span data-stu-id="84abe-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

