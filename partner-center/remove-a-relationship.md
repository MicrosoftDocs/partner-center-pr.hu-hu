---
title: Viszonteladói kapcsolat eltávolítása egy ügyféllel
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan távolíthatja el a Microsoft közvetlen partnerei az ügyfeleket a listából, hogyan távolíthatja el a delegált rendszergazdai jogosultságokat, és hogyan állíthatja le az ügyfelek támogatását vagy vásárlását.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 735a8b2c2436df61216ceb476be4a55b18785325
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855692"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="acb89-103">Viszonteladói kapcsolat eltávolítása egy ügyfélről a Partnerközpontban</span><span class="sxs-lookup"><span data-stu-id="acb89-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="acb89-104">**Megfelelő szerepkörök:** Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="acb89-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="acb89-105">Ez a cikk azt ismerteti, hogyan távolítható el egy viszonteladói kapcsolat egy ügyféllel a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="acb89-105">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="acb89-106">Közvetlen partnerek vagy közvetett szolgáltatók: ha már nem történik tranzakció egy ügyféllel, eltávolíthatja a kapcsolatot a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="acb89-106">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="acb89-107">Egy kapcsolat eltávolítása az alábbi következményekkel jár:</span><span class="sxs-lookup"><span data-stu-id="acb89-107">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="acb89-108">Eltávolítja az ügyfelet a Partnerközpontban lévő ügyféllistáról</span><span class="sxs-lookup"><span data-stu-id="acb89-108">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="acb89-109">Eltávolítja Az ügyfél [elérhető támogatási kapcsolattartói](assign-support-contacts.md) listájáról</span><span class="sxs-lookup"><span data-stu-id="acb89-109">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="acb89-110">Eltávolítja az ügyfél számára delegált rendszergazdai jogosultságait</span><span class="sxs-lookup"><span data-stu-id="acb89-110">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="acb89-111">A jövőben nem vásárolhat az ügyfél nevében</span><span class="sxs-lookup"><span data-stu-id="acb89-111">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="acb89-112">Kapcsolat eltávolítása</span><span class="sxs-lookup"><span data-stu-id="acb89-112">How to remove a relationship</span></span>

<span data-ttu-id="acb89-113">A kapcsolat eltávolításához először le kell mondania az Azure RI-foglalásokat, le kell mondania a szoftvervásárlásokat, és fel kell függesztenie a fennmaradó aktív előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="acb89-113">To remove the relationship, you'll need to cancel Azure RI reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="acb89-114">**Függessze fel az aktív előfizetéseket.**</span><span class="sxs-lookup"><span data-stu-id="acb89-114">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="acb89-115">A Partnerközpont válassza az **Ügyfelek lehetőséget,** és válasszon ki egy ügyfelet</span><span class="sxs-lookup"><span data-stu-id="acb89-115">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="acb89-116">Az **Előfizetések alatt** válasszon ki egy előfizetést.</span><span class="sxs-lookup"><span data-stu-id="acb89-116">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="acb89-117">Válassza a **Felfüggesztve lehetőséget**</span><span class="sxs-lookup"><span data-stu-id="acb89-117">Select **Suspended**</span></span>

   4. <span data-ttu-id="acb89-118">Ismételje meg ezeket a lépéseket minden aktív előfizetésnél.</span><span class="sxs-lookup"><span data-stu-id="acb89-118">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="acb89-119">**Távolítsa el a kapcsolatot a Partnerközpont:**</span><span class="sxs-lookup"><span data-stu-id="acb89-119">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="acb89-120">a.</span><span class="sxs-lookup"><span data-stu-id="acb89-120">a.</span></span> <span data-ttu-id="acb89-121">A Partnerközpont válassza az **Ügyfelek** lehetőséget, és válasszon ki egy ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="acb89-121">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="acb89-122">b.</span><span class="sxs-lookup"><span data-stu-id="acb89-122">b.</span></span> <span data-ttu-id="acb89-123">Válassza ki a **Account (Fiók) lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="acb89-123">Select the **Account**.</span></span>

   <span data-ttu-id="acb89-124">c.</span><span class="sxs-lookup"><span data-stu-id="acb89-124">c.</span></span> <span data-ttu-id="acb89-125">Válassza **a Viszonteladói kapcsolat eltávolítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="acb89-125">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="acb89-126">Ha bármelyik előfizetés még aktív, a **Viszonteladó** eltávolítása kapcsolat hivatkozás inaktív lesz.</span><span class="sxs-lookup"><span data-stu-id="acb89-126">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="acb89-127">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="acb89-127">Next steps</span></span>

- [<span data-ttu-id="acb89-128">Ügyfélkapcsolat kérése vagy újra létrehozása</span><span class="sxs-lookup"><span data-stu-id="acb89-128">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
