---
title: Korlátozott közvetlen számlázási képességek
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg a csp közvetlen számlázási partnerekre vonatkozó követelményeit, és hogy mi a helyzet a képességek korlátozásának elkerüléséhez. Derítse ki, hogy korlátozva vannak-e a képességei.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b3b1f3e1593f7e35bd3b9ed6c56ea28683bff95a
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855488"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a><span data-ttu-id="dfbaa-104">Korlátozott közvetlen számlázási képességek és a közvetlen számlapartnerek CSP-hez szükséges követelményei</span><span class="sxs-lookup"><span data-stu-id="dfbaa-104">Restricted direct bill capabilities and the requirements needed for CSP direct bill partners</span></span>

<span data-ttu-id="dfbaa-105">**Megfelelő szerepkörök:** Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="dfbaa-105">**Appropriate roles**: Global admin</span></span>

## <a name="overview"></a><span data-ttu-id="dfbaa-106">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="dfbaa-106">Overview</span></span>

<span data-ttu-id="dfbaa-107">A közvetlen számlázási partnereknek meg kell felelnie az [új](direct-partner-new-requirements.md) követelményeknek ahhoz, hogy a CSP közvetlen számlázási partnerprogramjában maradjanak.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-107">Direct bill partners must meet the new [requirements](direct-partner-new-requirements.md) to remain in the CSP direct bill partner program.</span></span> <span data-ttu-id="dfbaa-108">Ellenkező esetben a közvetlen számlázási képességekhez való hozzáférésük idővel korlátozott lesz, és tovább végezhet bizonyos feladatokat, például új vásárlásokat az ügyfeleik számára.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-108">Otherwise, their access to direct bill capabilities will eventually be restricted and can longer perform specific tasks, such as making new purchases for their customers.</span></span>

> [!Note]
> <span data-ttu-id="dfbaa-109">A Közvetlen csp-partnerprogram követelményeinek nem megfelelő közvetlen számlázási partnereket a Microsoft értesíti, ha a közvetlen számlázási képességeik korlátozva lesznek.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-109">Direct bill partners who do not meet the new requirements for CSP direct bill partner program will be informed by Microsoft when their direct bill capabilities will be restricted.</span></span> <span data-ttu-id="dfbaa-110">Ez az összes közvetlen számlázási partnerre vonatkozik, függetlenül attól, hogy a közvetlen számlázási partnerről a közvetett viszonteladókra való áttérés mellett döntöttek-e. [](transition-direct-to-indirect.md)</span><span class="sxs-lookup"><span data-stu-id="dfbaa-110">This applies to all direct bill partners, whether they have opted for [transition from direct bill partner to indirect resellers](transition-direct-to-indirect.md) or not.</span></span>  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a><span data-ttu-id="dfbaa-111">Hogyan lehet tudni, hogy korlátozva vannak-e a közvetlen számlázási képességek?</span><span class="sxs-lookup"><span data-stu-id="dfbaa-111">How to tell if your direct bill capabilities has been restricted</span></span>

<span data-ttu-id="dfbaa-112">Annak megerősítéséhez, hogy a közvetlen számlázási partner bérlője hozzáférése a közvetlen számlázási képességekhez korlátozva van-e, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-112">To confirm whether access from the direct bill partner tenant to direct bill capabilities has been restricted, follow these steps.</span></span>

1. <span data-ttu-id="dfbaa-113">Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="dfbaa-113">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="dfbaa-114">Ugrás a **Fiókbeállítások**  ->  **Jogi profil elemre.**</span><span class="sxs-lookup"><span data-stu-id="dfbaa-114">Go to **Account settings** -> **Legal Profile**.</span></span>

3. <span data-ttu-id="dfbaa-115">A **Programadatok alatt** keresse meg **a Microsoft felhőszolgáltató állapotát.**</span><span class="sxs-lookup"><span data-stu-id="dfbaa-115">Under **Program info**, look for **Microsoft Cloud Solution Provider status**.</span></span>

4. <span data-ttu-id="dfbaa-116">Ha a program állapotának értéke **korlátozott,** az azt jelenti, hogy a közvetlen számlázási partner bérlője nem férhet hozzá a közvetlen számlázási képességekhez.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-116">If the program status has value **restricted**, it means that your direct bill partner tenant's access to direct bill capabilities has been restricted.</span></span>

## <a name="affected-direct-bill-capabilities"></a><span data-ttu-id="dfbaa-117">Az érintett közvetlen számlázási képességek</span><span class="sxs-lookup"><span data-stu-id="dfbaa-117">Affected direct bill capabilities</span></span>

<span data-ttu-id="dfbaa-118">Ha a közvetlen számlázási lehetőségek korlátozva vannak, nem vásárolhat új vásárlásokat az ügyfelek számára a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-118">If your direct bill capabilities have been restricted, you can no longer make new purchases for your customers in Partner Center.</span></span> <span data-ttu-id="dfbaa-119">Ez a korlátozás a következőket foglalja magában:</span><span class="sxs-lookup"><span data-stu-id="dfbaa-119">This restriction includes:</span></span>

- <span data-ttu-id="dfbaa-120">Azure-előfizetések</span><span class="sxs-lookup"><span data-stu-id="dfbaa-120">Azure subscriptions</span></span>

- <span data-ttu-id="dfbaa-121">Licencalapú előfizetések</span><span class="sxs-lookup"><span data-stu-id="dfbaa-121">License-based subscriptions</span></span>

- <span data-ttu-id="dfbaa-122">Új bővítmények hozzáadása meglévő licencalapú előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-122">Add new add-ons to existing license-based subscriptions.</span></span>

- <span data-ttu-id="dfbaa-123">Vásároljon szoftvereket és foglalási termékeket (például szoftver-előfizetéseket, folyamatos szoftvereket és Azure Reserved Virtual Machine-példányokat).</span><span class="sxs-lookup"><span data-stu-id="dfbaa-123">Make one-time purchases of software and reservation products (for example, software subscriptions, perpetual software, and Azure Reserved Virtual Machine instances).</span></span>

<span data-ttu-id="dfbaa-124">A CSP-program [keretében elérhető Azure-partnerek](shared-services.md) megosztott szolgáltatási ajánlatával nem vásárolhat saját használatra új Azure-előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-124">You also cannot use the [Azure partner shared services offer](shared-services.md) under the CSP program to purchase new Azure subscriptions for your own use.</span></span>

<span data-ttu-id="dfbaa-125">A meglévő közvetlen számlázási előfizetések nem érintettek.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-125">Existing direct bill subscriptions are not affected.</span></span> <span data-ttu-id="dfbaa-126">Ezek érvényesek maradnak, és automatikusan megújulnak.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-126">They remain valid and are auto-renewed.</span></span> <span data-ttu-id="dfbaa-127">A Microsoft a lemondásáig továbbra is közvetlenül önnek számláz.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-127">You will continue to be billed directly by Microsoft until they are canceled.</span></span> <span data-ttu-id="dfbaa-128">Továbbra is a következő módokon kezelheti a meglévő előfizetéseket:</span><span class="sxs-lookup"><span data-stu-id="dfbaa-128">You can still manage existing subscriptions in the following ways:</span></span>

- <span data-ttu-id="dfbaa-129">Meglévő előfizetések felfüggesztése</span><span class="sxs-lookup"><span data-stu-id="dfbaa-129">Suspend existing subscriptions</span></span>

- <span data-ttu-id="dfbaa-130">Meglévő licencalapú előfizetések licencszámának beállítása</span><span class="sxs-lookup"><span data-stu-id="dfbaa-130">Adjust license count of existing license-based subscriptions</span></span>

- <span data-ttu-id="dfbaa-131">Módosíthatja az előfizetés meglévő bővítményei licencszámát.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-131">Adjust license count of existing add-ons to a subscription.</span></span> 

    >[!Note]
    ><span data-ttu-id="dfbaa-132">A meglévő előfizetések nem adhatnak hozzá új bővítményeket, mivel a rendszer új vásárlásként kezeli őket.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-132">You cannot add new add-ons to existing subscriptions as it is treated as new purchase.</span></span>

- <span data-ttu-id="dfbaa-133">Új Azure-erőforrások üzembe helyezése és meglévő Azure-erőforrások kezelése meglévő Azure-előfizetések alatt.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-133">Deploy new Azure resources and manage existing Azure resources under existing Azure subscriptions.</span></span> <span data-ttu-id="dfbaa-134">Ide tartoznak az előfizetések és előfizetések Azure Marketplace Visual Studio elérhető erőforrások is.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-134">This includes resources, which are available through Azure Marketplace and Visual Studio subscriptions.</span></span>

<span data-ttu-id="dfbaa-135">Az új vásárlások mellett a következő közvetlen számlázási funkciók nem biztosítanak hozzáférést a Partnerközpont:</span><span class="sxs-lookup"><span data-stu-id="dfbaa-135">In addition to new purchases, you cannot access the following direct bill capabilities in Partner Center:</span></span>

- <span data-ttu-id="dfbaa-136">Nem hozhat létre új ügyfélbérlőket.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-136">You cannot create new customer tenants.</span></span> <span data-ttu-id="dfbaa-137">Az **Ügyfél létrehozása lehetőség** nem lesz **Partnerközpont** ügyfelek oldalán.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-137">The **Create customer** option under **Customers** page in Partner Center will not be available.</span></span>

- <span data-ttu-id="dfbaa-138">Nem hozhat létre közvetlen viszonteladói kapcsolatot kérő meghívót az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-138">You cannot generate invitation to customer requesting for direct reseller relationship.</span></span> <span data-ttu-id="dfbaa-139">A  **Viszonteladói kapcsolat kérése** lehetőség nem érhető el az Ügyfelek Partnerközpont lapon.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-139">The **Request a reseller relationship** option under **Customers** page in Partner Center will not be available.</span></span>

    >[!NOTE]
    ><span data-ttu-id="dfbaa-140">A közvetlen számlázási partnerről a közvetett viszonteladóra való áttérés részeként, ha már regisztrálta közvetett viszonteladóként a közvetlen számlázási partnerbérlőt, meghívót hozhat létre a közvetett viszonteladói kapcsolatot kérő ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-140">As part of transitioning from direct bill partner to indirect reseller, if you have already enrolled your direct bill partner tenant as indirect reseller, you can generate invitation to customer requesting for indirect reseller relationship instead.</span></span>

- <span data-ttu-id="dfbaa-141">Nem hozhat létre új sandbox-bérlőt.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-141">You cannot create new sandbox tenant.</span></span> <span data-ttu-id="dfbaa-142">Minden közvetlen számlázási partnerbérlő létrehozhat egy sandbox-bérlőt a közvetlen számlázási API-integrációhoz.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-142">Each direct bill partner tenant can create one sandbox tenant for direct bill API integration.</span></span> <span data-ttu-id="dfbaa-143">Ha még nem hozott létre egyet, a közvetlen számlázási partner képességeinek korlátozását követően erre nincs jogosultsága.</span><span class="sxs-lookup"><span data-stu-id="dfbaa-143">If you haven't created one previously, you are not allowed to do so after your direct bill partner capability has been restricted.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="dfbaa-144">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="dfbaa-144">Next steps</span></span>

- [<span data-ttu-id="dfbaa-145">További információ a közvetett viszonteladóvá válásról</span><span class="sxs-lookup"><span data-stu-id="dfbaa-145">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [<span data-ttu-id="dfbaa-146">A közvetlen CSP-partnerre vonatkozó új követelmények</span><span class="sxs-lookup"><span data-stu-id="dfbaa-146">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
