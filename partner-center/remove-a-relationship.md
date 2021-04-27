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
ms.openlocfilehash: d6ff07d2c54d006478b290ad53c024a55dea4e18
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018101"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="e888b-103">Viszonteladói kapcsolat eltávolítása egy ügyfélről a Partnerközpontban</span><span class="sxs-lookup"><span data-stu-id="e888b-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="e888b-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="e888b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e888b-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="e888b-105">Global admin</span></span>

<span data-ttu-id="e888b-106">Ez a cikk azt ismerteti, hogyan távolítható el egy viszonteladói kapcsolat egy ügyféllel a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="e888b-106">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="e888b-107">Közvetlen partnerek vagy közvetett szolgáltatók: ha már nem történik tranzakció egy ügyféllel, eltávolíthatja a kapcsolatot a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="e888b-107">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="e888b-108">Egy kapcsolat eltávolítása az alábbi következményekkel jár:</span><span class="sxs-lookup"><span data-stu-id="e888b-108">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="e888b-109">Eltávolítja az ügyfelet a Partnerközpontban lévő ügyféllistáról</span><span class="sxs-lookup"><span data-stu-id="e888b-109">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="e888b-110">Eltávolítja Az ügyfél [elérhető támogatási kapcsolattartói](assign-support-contacts.md) listájáról</span><span class="sxs-lookup"><span data-stu-id="e888b-110">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="e888b-111">Eltávolítja az ügyfél számára delegált rendszergazdai jogosultságait</span><span class="sxs-lookup"><span data-stu-id="e888b-111">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="e888b-112">A jövőben nem vásárolhat az ügyfél nevében</span><span class="sxs-lookup"><span data-stu-id="e888b-112">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="e888b-113">Kapcsolat eltávolítása</span><span class="sxs-lookup"><span data-stu-id="e888b-113">How to remove a relationship</span></span>

<span data-ttu-id="e888b-114">A kapcsolat eltávolításához először le kell mondania az Azure RI-foglalásokat, le kell mondania a szoftvervásárlásokat, és fel kell függesztenie a fennmaradó aktív előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="e888b-114">To remove the relationship, you'll need to cancel Azure RI reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="e888b-115">**Függessze fel az aktív előfizetéseket.**</span><span class="sxs-lookup"><span data-stu-id="e888b-115">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="e888b-116">A Partnerközpont válassza az **Ügyfelek lehetőséget,** és válasszon ki egy ügyfelet</span><span class="sxs-lookup"><span data-stu-id="e888b-116">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="e888b-117">Az **Előfizetések alatt** válasszon ki egy előfizetést.</span><span class="sxs-lookup"><span data-stu-id="e888b-117">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="e888b-118">Válassza a **Felfüggesztve lehetőséget**</span><span class="sxs-lookup"><span data-stu-id="e888b-118">Select **Suspended**</span></span>

   4. <span data-ttu-id="e888b-119">Ismételje meg ezeket a lépéseket minden aktív előfizetésnél.</span><span class="sxs-lookup"><span data-stu-id="e888b-119">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="e888b-120">**Távolítsa el a kapcsolatot a Partnerközpont:**</span><span class="sxs-lookup"><span data-stu-id="e888b-120">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="e888b-121">a.</span><span class="sxs-lookup"><span data-stu-id="e888b-121">a.</span></span> <span data-ttu-id="e888b-122">A Partnerközpont válassza az **Ügyfelek** lehetőséget, és válasszon ki egy ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="e888b-122">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="e888b-123">b.</span><span class="sxs-lookup"><span data-stu-id="e888b-123">b.</span></span> <span data-ttu-id="e888b-124">Válassza ki a **Account (Fiók) lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e888b-124">Select the **Account**.</span></span>

   <span data-ttu-id="e888b-125">c.</span><span class="sxs-lookup"><span data-stu-id="e888b-125">c.</span></span> <span data-ttu-id="e888b-126">Válassza **a Viszonteladói kapcsolat eltávolítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e888b-126">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="e888b-127">Ha bármelyik előfizetés még aktív, a **Viszonteladó** eltávolítása kapcsolat hivatkozás inaktív lesz.</span><span class="sxs-lookup"><span data-stu-id="e888b-127">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e888b-128">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="e888b-128">Next steps</span></span>

- [<span data-ttu-id="e888b-129">Ügyfélkapcsolat kérése vagy újra létrehozása</span><span class="sxs-lookup"><span data-stu-id="e888b-129">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
