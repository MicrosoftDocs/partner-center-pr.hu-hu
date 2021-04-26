---
title: Azure-előfizetés átvitele másik partnernek
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan módosíthatja Felhőszolgáltató ügyfél Azure-előfizetéséhez társított programpartnert.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: b21bfcae4472763c19481ad506ae1c72d238e8f0
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002901"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a><span data-ttu-id="4d6a5-103">Megtudhatja, hogyan adhatja át egy ügyfél Azure-előfizetéseit egy másik partnernek</span><span class="sxs-lookup"><span data-stu-id="4d6a5-103">Learn how to transfer a customer's Azure subscriptions to another partner</span></span>

<span data-ttu-id="4d6a5-104">**A következőre érvényes:**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-104">**Applies to**</span></span>

- <span data-ttu-id="4d6a5-105">A Microsoft Cloud for US Government Partnerközpontja</span><span class="sxs-lookup"><span data-stu-id="4d6a5-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="4d6a5-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-106">**Appropriate roles**</span></span>

- <span data-ttu-id="4d6a5-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="4d6a5-107">Global admin</span></span>

<span data-ttu-id="4d6a5-108">Ez a cikk azt ismerteti, hogyan válthatnak az ügyfelek Microsoft Azure szolgáltatásaik között az Felhőszolgáltató (CSP) között.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-108">This article describes how a customer can switch their Microsoft Azure services from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="4d6a5-109">Ha egy ügyfél Azure-szolgáltatásait vagy -előfizetéseit egy másik partnerre cseréli, kövesse az alábbi manuális lépéseket.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-109">To switch a customer's Azure services or subscriptions to a different partner, follow these manual steps.</span></span> <span data-ttu-id="4d6a5-110">A lépéseket a partnernek és az ügyfélnek is el kell végrehajtania.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-110">Both the partner and the customer need to complete the steps.</span></span>

>[!Note]  
><span data-ttu-id="4d6a5-111">Jelenleg csak közvetlen vagy közvetett szolgáltatók továbbíthatók előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-111">Currently, only Direct or Indirect Providers can transfer subscriptions.</span></span>
><span data-ttu-id="4d6a5-112">Az Azure-csomaghoz Felhőszolgáltató Office 365-höz, Nagyvállalati mobilitási csomaghoz vagy Microsoft Dynamics CRM-előfizetésekhez társított előfizetések partnerét nem módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-112">You can't change partners for Cloud Solution Provider subscriptions associated with Azure plan, Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

## <a name="switch-partners-for-azure-subscriptions"></a><span data-ttu-id="4d6a5-113">Partnerek váltása Azure-előfizetések esetén</span><span class="sxs-lookup"><span data-stu-id="4d6a5-113">Switch partners for Azure subscriptions</span></span>

1. <span data-ttu-id="4d6a5-114">Azure-előfizetés új partnernek való átadásához az ügyfélnek el kell kezdenie a folyamatot, és írásban kapcsolatba kell lépnie jelenlegi partnerével.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-114">To transfer an Azure subscription to a new partner, the customer must start the process and contact their current partner of record in writing.</span></span>

   >[!Note]
   > <span data-ttu-id="4d6a5-115">A jelenlegi partner felelőssége, hogy létrehozza az átadási folyamatot elindítani szükséges szolgáltatásjegyet.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-115">It is the current partner's responsibility to create the service ticket that initiates the transfer process.</span></span> <span data-ttu-id="4d6a5-116">A Microsoft nem avatkozhat be az ügyfél vagy az új partner nevében.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-116">Microsoft cannot intervene on behalf of the customer or the new partner.</span></span> <span data-ttu-id="4d6a5-117">Az ügyfélnek szorosan együtt kell működnie az aktuális partnerrel, hogy zökkenőmentes legyen az átállás.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-117">The customer should plan to work closely with the current partner to make the transition go smoothly.</span></span>

2. <span data-ttu-id="4d6a5-118">Az előfizetés partnerének a következő feladatokat kell elvégeznie:</span><span class="sxs-lookup"><span data-stu-id="4d6a5-118">The partner for the subscription needs to do the following tasks:</span></span>

   <span data-ttu-id="4d6a5-119">Hozzon létre egy Azure-szolgáltatásjegyet a Partnerközpont előfizetés átvitelének igényléséhez:</span><span class="sxs-lookup"><span data-stu-id="4d6a5-119">Create an Azure service ticket from Partner Center to request a subscription transfer:</span></span>

   1. <span data-ttu-id="4d6a5-120">A Partnerközpont válassza az **Ügyfelek** lehetőséget, válassza ki az ügyfelet a listából, majd válassza a **Szolgáltatáskezelés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-120">From the Partner Center menu, select **Customers**, select your customer from the list, and then select **Service management**.</span></span>

   2. <span data-ttu-id="4d6a5-121">A Támogatási **jegyek szakaszban** válassza az Új **jegy** legördülő menüt, majd **a** Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-121">Under the **Support tickets** section, select the **New ticket** dropdown and choose **Microsoft Azure**.</span></span>
   
   3. <span data-ttu-id="4d6a5-122">A [Azure Portal](https://portal.azure.com)válassza az **Új támogatási kérelem lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-122">From the [Azure portal](https://portal.azure.com), select **New support request**.</span></span>
   
   4. <span data-ttu-id="4d6a5-123">Az 1.  lépésben válassza az Előfizetés-kezelés problématípust, adja meg az átvitni kívánt előfizetés-azonosítót, és Felhőszolgáltató **támogatási** csomagként.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-123">In Step 1, choose **Subscription management** as the issue type, specify the Subscription ID you want transferred, and choose **Cloud Solution Provider** as the support plan.</span></span>
   
   5. <span data-ttu-id="4d6a5-124">A 2. lépésben válassza a **C–Minimális hatás lehetőséget,** és válassza az **Egyéb általános kérdések** lehetőséget a probléma típusaként.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-124">In Step 2, select **C-Minimal impact** and choose **Other General Questions** as the problem type.</span></span>
   
   6. <span data-ttu-id="4d6a5-125">Töltse le a [CSP-előfizetés átviteli űrlapját.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)</span><span class="sxs-lookup"><span data-stu-id="4d6a5-125">Download the [CSP Subscription Transfer form](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC).</span></span>

3. <span data-ttu-id="4d6a5-126">Az előfizetés partnere: Töltse ki a [CSP-előfizetés](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)átviteli űrlapját, írja alá, majd küldje el az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-126">The partner for the subscription: Fill in the [CSP Subscription Transfer form](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC), sign it, and then send it to the customer.</span></span> 

   <span data-ttu-id="4d6a5-127">Az űrlap kitöltéshez a következő információkra lesz szüksége:</span><span class="sxs-lookup"><span data-stu-id="4d6a5-127">To fill in the form, you'll need the following information:</span></span>

   - <span data-ttu-id="4d6a5-128">Az aktuális partner kapcsolattartási adatai és Microsoft-azonosítója.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-128">The current partner's contact information and Microsoft ID.</span></span> <span data-ttu-id="4d6a5-129">A Partnerközpont válassza a Fiókbeállítások Szervezeti profil lehetőséget, és használja az itt felsorolt  &gt;  **Microsoft-azonosítót,** Szervezetnevet és  **Címet.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-129">In the Partner Center menu, select **Account settings** &gt; **Organization profile**, and use the **Microsoft ID**, **Organization name**, and **Address** listed there.</span></span>

   - <span data-ttu-id="4d6a5-130">Az ügyfél Microsoft-azonosítója.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-130">The customer's Microsoft ID.</span></span> <span data-ttu-id="4d6a5-131">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd bontsa ki az ügyfél termékoldalát a **Microsoft-azonosítójukhoz.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-131">In the Partner Center menu, select **Customers**, then expand the customer's listing to see their **Microsoft ID**.</span></span>

   - <span data-ttu-id="4d6a5-132">Az áthelyezni szükséges előfizetés-azonosító.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-132">The subscription ID to transfer.</span></span> <span data-ttu-id="4d6a5-133">A bővített ügyféllistában válassza az Előfizetések megtekintése lehetőséget, majd **bontsa** ki a kiválasztott előfizetést az előfizetés **azonosítójának megtekintéséhez.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-133">In the expanded customer listing, select **View Subscriptions**, then expand the chosen subscription to see the **Subscription ID**.</span></span>

   >[!Note]
   ><span data-ttu-id="4d6a5-134">Az előfizetések átvitele két előfizetés-azonosítót  ad eredményként, amelyek az átvitt előfizetés Előfizetés szerkesztése oldalán fognak látni: **1**– A Partnerközpont-előfizetés azonosítóját számlázási célokra használjuk.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-134">Transferring a subscription results in two subscription IDs which you will see on the **Edit Subscription** page of the transferred subscription: **1**- The Partner Center Subscription ID is used for billing purposes.</span></span> <span data-ttu-id="4d6a5-135">**2**– A rendszer megőrzi az eredeti Azure-előfizetés azonosítóját, és Partnerközpont az Azure felügyeleti portálján is.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-135">**2**-  The original Azure Subscription ID is retained and will appear in Partner Center as well as in the Azure Management portal.</span></span> <span data-ttu-id="4d6a5-136">Ez az azonosító megjelenik a recon fájlban.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-136">This ID will appear in your recon file.</span></span>  <span data-ttu-id="4d6a5-137">**A támogatási jegyek naplózásakor mindkét adatbázist használnia kell.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-137">**When logging support tickets, you need to use both IDs.**</span></span>

4. <span data-ttu-id="4d6a5-138">Az előfizetéshez az ügyfél és az új partner:</span><span class="sxs-lookup"><span data-stu-id="4d6a5-138">The customer and new partner for the subscription:</span></span>

   <span data-ttu-id="4d6a5-139">Tekintse át az űrlapot, adja meg az új partner adatait, majd írja alá.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-139">Review the form, fill in information about the new partner, and sign it.</span></span> <span data-ttu-id="4d6a5-140">Ellenőrizze, hogy az új ügyfél rendelkezik-e szerződéssel.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-140">Confirm that the new customer has a contract agreement in place.</span></span> <span data-ttu-id="4d6a5-141">Küldje vissza az űrlapot az aktuális rekordpartnernek.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-141">Send the form back to the current partner of record.</span></span>

   <span data-ttu-id="4d6a5-142">*Fontos:* Ha az új CSP-partner nem rendelkezik viszonteladói kapcsolattal az ügyféllel, az előfizetés átadása előtt létre kell hoznia egyet.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-142">*Important*: If the new CSP Partner doesn't have a reseller relationship with the customer, they must establish one before the subscription is transferred.</span></span> <span data-ttu-id="4d6a5-143">[Ennek a mikéntjről itt talál információt.](request-a-relationship-with-a-customer.md)</span><span class="sxs-lookup"><span data-stu-id="4d6a5-143">[You can find information on how to do this here](request-a-relationship-with-a-customer.md).</span></span>

   >[!Note]
   ><span data-ttu-id="4d6a5-144">Az új CSP-partnernek és az ügyfélbérlőnek ugyanabban az országban kell lennie.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-144">The new CSP partner and the customer tenant must be in the same country.</span></span> 

5. <span data-ttu-id="4d6a5-145">Aktuális partner:</span><span class="sxs-lookup"><span data-stu-id="4d6a5-145">Current partner:</span></span>

   <span data-ttu-id="4d6a5-146">Győződjön meg arról, hogy az űrlap mindkét partner-rendszergazda kapcsolattartási adatait tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-146">Make sure the form includes contact information for both partner admins.</span></span> <span data-ttu-id="4d6a5-147">Microsoft ügyfélszolgálata mindkét rendszergazdával kapcsolatba lép az átvitel ellenőrzéséhez.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-147">Microsoft Support will contact both admins to verify the transfer.</span></span> <span data-ttu-id="4d6a5-148">Győződjön meg arról, hogy mindhárom aláírással van.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-148">Make sure you have all three signatures.</span></span> <span data-ttu-id="4d6a5-149">Ezután a **Fájlfeltöltés lehetőséggel** csatolja a kitöltött űrlapot a meglévő szolgáltatáskéréshez.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-149">Then use the **File Upload** option to attach the completed form to your existing service request.</span></span> <span data-ttu-id="4d6a5-150">A Microsoft támogatási szakembere nyolc órán belül visszatér Önhez a nyugta és a befejezés ellenőrzéséhez.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-150">A Microsoft support engineer will get back to you within eight business hours to validate receipt and completion.</span></span>

6. <span data-ttu-id="4d6a5-151">Új partner:</span><span class="sxs-lookup"><span data-stu-id="4d6a5-151">New partner:</span></span>

   <span data-ttu-id="4d6a5-152">Frissítse az Azure-előfizetés beállításait, hogy eltávolítsa a régi partnert a fiókból.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-152">Update the Azure subscription settings to remove the old partner from the account.</span></span> <span data-ttu-id="4d6a5-153">Két PowerShell-parancsmag futtatásával láthatja, hogy mely szerepkör-hozzárendelések vannak kiépítve.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-153">To see which role assignments are provisioned, run two PowerShell Commandlets.</span></span>

   - <span data-ttu-id="4d6a5-154">Adja hozzá az új partnert viszonteladóként a fiókhoz:</span><span class="sxs-lookup"><span data-stu-id="4d6a5-154">Add the new partner as the reseller on the account:</span></span>

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > <span data-ttu-id="4d6a5-155">Az ügyfél **bérlőazonosítója** megjelenik a Partnerközpont az ügyfél **Microsoft-azonosítójaként.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-155">The customer's **Tenant ID** appears in Partner Center as the customer's **Microsoft ID**.</span></span> <span data-ttu-id="4d6a5-156">Egy adott ügyfél Microsoft-azonosítójának (bérlőazonosítójának) megkereséhez jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="4d6a5-156">To find the Microsoft ID (Tenant ID) for a specific customer, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span> <span data-ttu-id="4d6a5-157">Ezután válassza **az Ügyfelek** lehetőséget a menüből.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-157">Then select **Customers** from the menu.</span></span> <span data-ttu-id="4d6a5-158">Keresse meg az ügyfelet a listában.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-158">Locate the customer on the list.</span></span> <span data-ttu-id="4d6a5-159">A lefelé mutató nyílra kattintva bontsa ki az ügyfél termékoldalát.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-159">Select the down-arrow to expand the customer's listing.</span></span> <span data-ttu-id="4d6a5-160">Az ügyfél tartománynevére és  Microsoft-azonosítójára vonatkozó információkat fog **látni.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-160">You will see information about the customer's *Domain name* and the customer's **Microsoft ID**.</span></span> <span data-ttu-id="4d6a5-161">Használja a 16 számjegyű **Microsoft-azonosítót** a PowerShell-parancsmagban.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-161">Use the 16-digit **Microsoft ID** in the PowerShell commandlet.</span></span>

   - <span data-ttu-id="4d6a5-162">Tekintse meg a fiók szerepköreit, beleértve a korábbi CSP-partnereket is:</span><span class="sxs-lookup"><span data-stu-id="4d6a5-162">View roles on the account, including previous CSP partners:</span></span>

     ```powershell
     Get-AzRoleAssignment
     ```

7. <span data-ttu-id="4d6a5-163">Elavult hozzáférési engedélyek eltávolítása:</span><span class="sxs-lookup"><span data-stu-id="4d6a5-163">Remove outdated access permissions:</span></span>

   - <span data-ttu-id="4d6a5-164">A Partnerközpont válassza az Ügyfelek **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-164">In the Partner Center menu, select **Customers**.</span></span>
   - <span data-ttu-id="4d6a5-165">Keresse meg az ügyfelet a listában.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-165">Locate the customer on the list.</span></span> <span data-ttu-id="4d6a5-166">Válassza ki (kattintson duplán) a vállalata nevére.</span><span class="sxs-lookup"><span data-stu-id="4d6a5-166">Select (double-click) their company name.</span></span> <span data-ttu-id="4d6a5-167">Ez a művelet megnyitja az ügyfél **Előfizetések oldalát.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-167">This action opens the customer **Subscriptions** page.</span></span>
   - <span data-ttu-id="4d6a5-168">Az ügyféladatok menüben válassza a **Szolgáltatáskezelés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-168">In the customer detail menu, select **Service management**.</span></span>
   - <span data-ttu-id="4d6a5-169">A **Microsoft Azure** alatt kattintson a hivatkozásra, hogy a következőre **a Microsoft Azure felügyeleti portálja.**</span><span class="sxs-lookup"><span data-stu-id="4d6a5-169">Under **Microsoft Azure**, select the link to go to the **Microsoft Azure Management Portal**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4d6a5-170">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="4d6a5-170">Next steps</span></span>

- <span data-ttu-id="4d6a5-171">Töltse le a [CSP-előfizetés átviteli űrlapját.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA)</span><span class="sxs-lookup"><span data-stu-id="4d6a5-171">Download the [CSP Subscription Transfer form](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).</span></span>

- <span data-ttu-id="4d6a5-172">További információ [a többpartneres támogatásról.](multipartner.md)</span><span class="sxs-lookup"><span data-stu-id="4d6a5-172">Learn about [multi-partner support](multipartner.md).</span></span>

- <span data-ttu-id="4d6a5-173">[többpartneres támogatás.](multipartner.md)</span><span class="sxs-lookup"><span data-stu-id="4d6a5-173">[multi-partner support](multipartner.md).</span></span>
- <span data-ttu-id="4d6a5-174">[többcsatornás támogatás.](multichannel.md)</span><span class="sxs-lookup"><span data-stu-id="4d6a5-174">[multi-channel support](multichannel.md).</span></span>
- [<span data-ttu-id="4d6a5-175">Azure-előfizetések átvitele</span><span class="sxs-lookup"><span data-stu-id="4d6a5-175">Transfer Azure subscriptions</span></span>](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)