---
title: Annak megerősítése, hogy az ügyfél elfogadta a Microsoft Ügyfélszerződést
description: Megtudhatja, hogyan erősítheti meg a Microsoft-ügyfél szerződését. Erre szükség lehet a Microsoft termékeinek és szolgáltatásainak megrendeléséhez az ügyfelek számára.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/02/2021
ms.openlocfilehash: ab2f5be77f6480b4a8b47bef0e0fd5096f7c1776
ms.sourcegitcommit: a7897284b79abb1ceeee79deb3a87b72d59900dc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "102029916"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="b565e-104">Annak megerősítése, hogy az ügyfél elfogadta a Microsoft-ügyfélszerződést</span><span class="sxs-lookup"><span data-stu-id="b565e-104">Confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="b565e-105">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="b565e-105">**Appropriate roles**</span></span>

- <span data-ttu-id="b565e-106">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="b565e-106">Admin agent</span></span>
- <span data-ttu-id="b565e-107">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="b565e-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="b565e-108">A partner Center jelenleg csak a Microsoft nyilvános felhőben támogatja a szerződési erőforrást.</span><span class="sxs-lookup"><span data-stu-id="b565e-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="b565e-109">Nem alkalmazható a következőre:</span><span class="sxs-lookup"><span data-stu-id="b565e-109">It is not applicable to:</span></span>
> * <span data-ttu-id="b565e-110">A 21Vianet által üzemeltetett partneri központ</span><span class="sxs-lookup"><span data-stu-id="b565e-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="b565e-111">A Microsoft Cloud Germany Partnerközpontja</span><span class="sxs-lookup"><span data-stu-id="b565e-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="b565e-112">A Microsoft Cloud for US Government Partnerközpontja</span><span class="sxs-lookup"><span data-stu-id="b565e-112">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="b565e-113">Partnerként be kell szereznie a Microsoft-ügyfél szerződését, mielőtt a Microsoft termékeit és szolgáltatásait megrendeli az adott ügyfélhez.</span><span class="sxs-lookup"><span data-stu-id="b565e-113">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="b565e-114">A partnereknek a megfelelőségi követelményeknek való megfelelés érdekében a Microsoft felkéri a partnereket, hogy erősítse meg az elfogadást a szerződést elfogadó személyre vonatkozó alábbi részletek megadásával:</span><span class="sxs-lookup"><span data-stu-id="b565e-114">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="b565e-115">Utónév</span><span class="sxs-lookup"><span data-stu-id="b565e-115">First name</span></span>

- <span data-ttu-id="b565e-116">Vezetéknév</span><span class="sxs-lookup"><span data-stu-id="b565e-116">Last name</span></span>

- <span data-ttu-id="b565e-117">E-mail-cím</span><span class="sxs-lookup"><span data-stu-id="b565e-117">Email address</span></span>

- <span data-ttu-id="b565e-118">Telefonszám (nem kötelező)</span><span class="sxs-lookup"><span data-stu-id="b565e-118">Phone number (optional)</span></span>

- <span data-ttu-id="b565e-119">Elfogadás dátuma</span><span class="sxs-lookup"><span data-stu-id="b565e-119">Date of acceptance</span></span>

<span data-ttu-id="b565e-120">A közvetlen számlás partnereknek és a közvetett szolgáltatóknak meg kell erősíteniük a Microsoft-ügyfél szerződését a partner Center vagy a partner Center API-n keresztül történő átadáskor.</span><span class="sxs-lookup"><span data-stu-id="b565e-120">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="b565e-121">A megerősítés *kötelező*.</span><span class="sxs-lookup"><span data-stu-id="b565e-121">Confirmation is *mandatory*.</span></span>

>[!NOTE]
><span data-ttu-id="b565e-122">2020. január 31-ig az összes meglévő és új ügyfélnek alá kell írnia az új Microsoft Customer szerződést.</span><span class="sxs-lookup"><span data-stu-id="b565e-122">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="b565e-123">További információért olvassa el [a Microsoft ügyfél-szerződés megerősítő ügyfeleinek jóváhagyása](confirm-customer-agreement.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="b565e-123">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="b565e-124">Ha nincs megadva visszaigazolás az adott ügyfélhez:</span><span class="sxs-lookup"><span data-stu-id="b565e-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="b565e-125">Ehhez az ügyfélhez nem fog tudni új rendeléseket létrehozni.</span><span class="sxs-lookup"><span data-stu-id="b565e-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="b565e-126">Az ügyfélhez már meglévő licenccel rendelkező előfizetések licencének száma nem módosítható.</span><span class="sxs-lookup"><span data-stu-id="b565e-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="b565e-127">Az ügyfelek elfogadásának megerősítése a partner Center vagy a partner Center API használatával végezhető el.</span><span class="sxs-lookup"><span data-stu-id="b565e-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="b565e-128">Ha ezt a partner Center API-val szeretné elvégezni, tekintse meg a következő témaköröket:</span><span class="sxs-lookup"><span data-stu-id="b565e-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="b565e-129">Az ügyfél jóváhagyásának megerősítése</span><span class="sxs-lookup"><span data-stu-id="b565e-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="b565e-130">Szerződés metaadatainak beolvasása</span><span class="sxs-lookup"><span data-stu-id="b565e-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="b565e-131">Az ügyfél jóváhagyásának megerősítése</span><span class="sxs-lookup"><span data-stu-id="b565e-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="b565e-132">Ez a termelési és a homokozó környezetekre is vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="b565e-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="b565e-133">Ügyfél-elfogadás megerősítése új ügyfél számára</span><span class="sxs-lookup"><span data-stu-id="b565e-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="b565e-134">A következő eljárással ellenőrizheti az ügyfelek elfogadását, miközben új ügyfél-bérlőt hoz létre a partner Centerben.</span><span class="sxs-lookup"><span data-stu-id="b565e-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="b565e-135">Ehhez rendszergazdai ügynöknek vagy értékesítési ügynöknek kell lennie.</span><span class="sxs-lookup"><span data-stu-id="b565e-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="b565e-136">Válassza az **ügyfelek**, majd az **új ügyfél** lehetőséget, majd válassza a **fiókadatok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b565e-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="b565e-137">Adja meg a **vállalat** és az **elsődleges kapcsolat** adatait.</span><span class="sxs-lookup"><span data-stu-id="b565e-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Vállalati adatok":::

3. <span data-ttu-id="b565e-139">A **Microsoft ügyfél-szerződés** területen válassza ki **az ügyfelet a Microsoft legújabb ügyfél-szerződésének elfogadásával**.</span><span class="sxs-lookup"><span data-stu-id="b565e-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="b565e-140">A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot.</span><span class="sxs-lookup"><span data-stu-id="b565e-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="b565e-141">Ez nem állítható be jövőbeli dátumra.</span><span class="sxs-lookup"><span data-stu-id="b565e-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="b565e-142">Adja meg az elfogadást elfogadó felhasználó részleteit.</span><span class="sxs-lookup"><span data-stu-id="b565e-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Elfogadás dátumának hozzáadása":::

   <span data-ttu-id="b565e-144">Alapértelmezés szerint az elsődleges kapcsolattartási felhasználói adatok jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="b565e-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="b565e-145">Ha ez nem megfelelő, válassza a **frissítés** lehetőséget, majd adja meg a szerződést elfogadó személy **utónevét**, **vezetéknevét**, **e-mail-címét** és \**telefonszámát* (nem kötelező).</span><span class="sxs-lookup"><span data-stu-id="b565e-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="b565e-146">A **Tovább gombra kattintva** folytassa az ügyfél bérlő létrehozásához szükséges további lépéseket.</span><span class="sxs-lookup"><span data-stu-id="b565e-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="b565e-147">Ügyfél-elfogadás megerősítése egy meglévő ügyfélnél</span><span class="sxs-lookup"><span data-stu-id="b565e-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="b565e-148">Ehhez rendszergazdai ügynöknek vagy értékesítési ügynöknek kell lennie.</span><span class="sxs-lookup"><span data-stu-id="b565e-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="b565e-149">Válassza ki az **ügyfelek** lehetőséget, majd keresse meg és válassza ki a megtekinteni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="b565e-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="b565e-150">Válassza a **fiókadatok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b565e-150">Select **Account info**.</span></span>

3. <span data-ttu-id="b565e-151">A **Microsoft ügyfél-szerződés** területen válassza a **frissítés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b565e-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Frissítés":::

4. <span data-ttu-id="b565e-153">Adja meg a szerződést elfogadó felhasználó **utónevét**, **vezetéknevét**, **e-mail címét** és **telefonszámát** (nem kötelező).</span><span class="sxs-lookup"><span data-stu-id="b565e-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="b565e-154">A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot.</span><span class="sxs-lookup"><span data-stu-id="b565e-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="b565e-155">Ez nem állítható be jövőbeli dátumra.</span><span class="sxs-lookup"><span data-stu-id="b565e-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="b565e-156">Válassza a **Mentés és folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b565e-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="b565e-157">Az ügyfelek elfogadásának megerősítése egy meglévő ügyfél új sorrendjének létrehozásakor</span><span class="sxs-lookup"><span data-stu-id="b565e-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="b565e-158">Ha olyan meglévő ügyfélhez próbál új rendelést létrehozni, akit még nem erősített meg, a megerősítés befejezésére vonatkozó kérést kap.</span><span class="sxs-lookup"><span data-stu-id="b565e-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="b565e-159">Ezt a következő eljárással végezheti el.</span><span class="sxs-lookup"><span data-stu-id="b565e-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="b565e-160">Adja meg a szerződést elfogadó felhasználó **utónevét**, **vezetéknevét**, **e-mail címét** és **telefonszámát** (nem kötelező).</span><span class="sxs-lookup"><span data-stu-id="b565e-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="b565e-161">A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot.</span><span class="sxs-lookup"><span data-stu-id="b565e-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="b565e-162">Ez nem állítható be jövőbeli dátumra.</span><span class="sxs-lookup"><span data-stu-id="b565e-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="b565e-163">Válassza a **Mentés és folytatás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b565e-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="b565e-164">Ügyfél-elfogadás megerősítésének beolvasása egy meglévő ügyfélnél</span><span class="sxs-lookup"><span data-stu-id="b565e-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="b565e-165">Lekérheti az ügyfél elfogadásának megerősítését egy meglévő ügyfél számára, amelyet korábban az alábbi eljárással adott meg.</span><span class="sxs-lookup"><span data-stu-id="b565e-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="b565e-166">Ehhez rendszergazdai ügynöknek vagy értékesítési ügynöknek kell lennie.</span><span class="sxs-lookup"><span data-stu-id="b565e-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="b565e-167">Válassza ki az **ügyfelek** lehetőséget, majd keresse meg és válassza ki a megtekinteni kívánt ügyfelet.</span><span class="sxs-lookup"><span data-stu-id="b565e-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="b565e-168">Válassza a **fiókadatok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b565e-168">Select **Account info**.</span></span>

3. <span data-ttu-id="b565e-169">A **Microsoft ügyfél-szerződés** alatt láthatja, hogy az ügyfél megkapta-e a megerősítést.</span><span class="sxs-lookup"><span data-stu-id="b565e-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b565e-170">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="b565e-170">Next steps</span></span>

- [<span data-ttu-id="b565e-171">Erősítse meg a Microsoft Customer szerződés ügyfél általi elfogadását a CSP-partner programban</span><span class="sxs-lookup"><span data-stu-id="b565e-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="b565e-172">A Microsoft ügyfél-szerződés elfogadásának igazolása az ügyfél nevében</span><span class="sxs-lookup"><span data-stu-id="b565e-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)