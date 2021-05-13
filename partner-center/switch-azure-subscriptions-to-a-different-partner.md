---
title: Azure-előfizetés átvitele másik partnernek
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan módosíthatja Felhőszolgáltató ügyfél Azure-előfizetéséhez társított partnerprogram-partnert.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 94f79762e7fabb377b8d7b559ff9ba2623b135fe
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856066"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a><span data-ttu-id="31352-103">Megtudhatja, hogyan adhatja át egy ügyfél Azure-előfizetéseit egy másik partnernek</span><span class="sxs-lookup"><span data-stu-id="31352-103">Learn how to transfer a customer's Azure subscriptions to another partner</span></span>

<span data-ttu-id="31352-104">**A következőkre vonatkozik:** Partnerközpont | Partnerközpont a Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="31352-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="31352-105">**Megfelelő szerepkörök:** Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="31352-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="31352-106">Ez a cikk azt ismerteti, hogy az ügyfelek hogyan válthatnak Microsoft Azure szolgáltatásaik között az Felhőszolgáltató (CSP) között.</span><span class="sxs-lookup"><span data-stu-id="31352-106">This article describes how a customer can switch their Microsoft Azure services from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="31352-107">Ha egy ügyfél Azure-szolgáltatásait vagy -előfizetéseit egy másik partnerre cseréli, kövesse az alábbi manuális lépéseket.</span><span class="sxs-lookup"><span data-stu-id="31352-107">To switch a customer's Azure services or subscriptions to a different partner, follow these manual steps.</span></span> <span data-ttu-id="31352-108">A lépéseket a partnernek és az ügyfélnek is el kell látnia.</span><span class="sxs-lookup"><span data-stu-id="31352-108">Both the partner and the customer need to complete the steps.</span></span>

>[!Note]  
><span data-ttu-id="31352-109">Jelenleg csak közvetlen vagy közvetett szolgáltatók továbbíthatók előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="31352-109">Currently, only Direct or Indirect Providers can transfer subscriptions.</span></span>
><span data-ttu-id="31352-110">Az Azure-csomaghoz Felhőszolgáltató Office 365-höz, Nagyvállalati mobilitási csomaghoz vagy Microsoft Dynamics CRM-előfizetésekhez társított előfizetések partnerét nem módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="31352-110">You can't change partners for Cloud Solution Provider subscriptions associated with Azure plan, Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

## <a name="switch-partners-for-azure-subscriptions"></a><span data-ttu-id="31352-111">Partnerek váltása Azure-előfizetések esetén</span><span class="sxs-lookup"><span data-stu-id="31352-111">Switch partners for Azure subscriptions</span></span>

1. <span data-ttu-id="31352-112">Az Azure-előfizetés új partnernek való átadásához az ügyfélnek el kell kezdenie a folyamatot, és írásban kapcsolatba kell lépnie jelenlegi partnerével.</span><span class="sxs-lookup"><span data-stu-id="31352-112">To transfer an Azure subscription to a new partner, the customer must start the process and contact their current partner of record in writing.</span></span>

   >[!Note]
   > <span data-ttu-id="31352-113">Az aktuális partner felelőssége, hogy létrehozza az átadási folyamatot elindítani szükséges szolgáltatásjegyet.</span><span class="sxs-lookup"><span data-stu-id="31352-113">It is the current partner's responsibility to create the service ticket that initiates the transfer process.</span></span> <span data-ttu-id="31352-114">A Microsoft nem avatkozhat be az ügyfél vagy az új partner nevében.</span><span class="sxs-lookup"><span data-stu-id="31352-114">Microsoft cannot intervene on behalf of the customer or the new partner.</span></span> <span data-ttu-id="31352-115">Az ügyfélnek szorosan együtt kell működnie az aktuális partnerrel, hogy zökkenőmentesen működjön az átállás.</span><span class="sxs-lookup"><span data-stu-id="31352-115">The customer should plan to work closely with the current partner to make the transition go smoothly.</span></span>

2. <span data-ttu-id="31352-116">Az előfizetés partnerének a következő feladatokat kell elvégeznie:</span><span class="sxs-lookup"><span data-stu-id="31352-116">The partner for the subscription needs to do the following tasks:</span></span>

   <span data-ttu-id="31352-117">Hozzon létre egy Azure-szolgáltatásjegyet Partnerközpont előfizetés átvitelének igényléséhez:</span><span class="sxs-lookup"><span data-stu-id="31352-117">Create an Azure service ticket from Partner Center to request a subscription transfer:</span></span>

   1. <span data-ttu-id="31352-118">A Partnerközpont válassza az **Ügyfelek** lehetőséget, válassza ki az ügyfelet a listából, majd válassza a **Szolgáltatáskezelés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="31352-118">From the Partner Center menu, select **Customers**, select your customer from the list, and then select **Service management**.</span></span>

   2. <span data-ttu-id="31352-119">A Támogatási **jegyek szakaszban** válassza az Új **jegy** legördülő menüt, majd a **Microsoft Azure.**</span><span class="sxs-lookup"><span data-stu-id="31352-119">Under the **Support tickets** section, select the **New ticket** dropdown and choose **Microsoft Azure**.</span></span>
   
   3. <span data-ttu-id="31352-120">A [Azure Portal](https://portal.azure.com)válassza az **Új támogatási kérelem lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="31352-120">From the [Azure portal](https://portal.azure.com), select **New support request**.</span></span>
   
   4. <span data-ttu-id="31352-121">Az 1.  lépésben válassza az Előfizetés-kezelés problématípust, adja meg az átvitni kívánt előfizetés-azonosítót, és válassza Felhőszolgáltató **előfizetést** támogatási csomagként.</span><span class="sxs-lookup"><span data-stu-id="31352-121">In Step 1, choose **Subscription management** as the issue type, specify the Subscription ID you want transferred, and choose **Cloud Solution Provider** as the support plan.</span></span>
   
   5. <span data-ttu-id="31352-122">A 2. lépésben válassza a **C–Minimális hatás lehetőséget,** és válassza az **Egyéb általános kérdések** lehetőséget a probléma típusaként.</span><span class="sxs-lookup"><span data-stu-id="31352-122">In Step 2, select **C-Minimal impact** and choose **Other General Questions** as the problem type.</span></span>
   
   6. <span data-ttu-id="31352-123">Töltse le a [CSP-előfizetés átvitele űrlapot.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)</span><span class="sxs-lookup"><span data-stu-id="31352-123">Download the [CSP Subscription Transfer form](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC).</span></span>

3. <span data-ttu-id="31352-124">Az előfizetés partnere: Töltse ki a [CSP-előfizetés](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)átviteli űrlapját, írja alá, majd küldje el az ügyfélnek.</span><span class="sxs-lookup"><span data-stu-id="31352-124">The partner for the subscription: Fill in the [CSP Subscription Transfer form](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC), sign it, and then send it to the customer.</span></span> 

   <span data-ttu-id="31352-125">Az űrlap kitöltéshez a következő információkra lesz szüksége:</span><span class="sxs-lookup"><span data-stu-id="31352-125">To fill in the form, you'll need the following information:</span></span>

   - <span data-ttu-id="31352-126">Az aktuális partner kapcsolattartási adatai és Microsoft-azonosítója.</span><span class="sxs-lookup"><span data-stu-id="31352-126">The current partner's contact information and Microsoft ID.</span></span> <span data-ttu-id="31352-127">A Partnerközpont válassza a Fiókbeállítások  Szervezeti profil lehetőséget, és használja az itt felsorolt &gt;  **Microsoft-azonosítót,** Szervezetnevet és **Címet.** </span><span class="sxs-lookup"><span data-stu-id="31352-127">In the Partner Center menu, select **Account settings** &gt; **Organization profile**, and use the **Microsoft ID**, **Organization name**, and **Address** listed there.</span></span>

   - <span data-ttu-id="31352-128">Az ügyfél Microsoft-azonosítója.</span><span class="sxs-lookup"><span data-stu-id="31352-128">The customer's Microsoft ID.</span></span> <span data-ttu-id="31352-129">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd bontsa ki az ügyfél termékoldalát a **Microsoft-azonosítójukhoz.**</span><span class="sxs-lookup"><span data-stu-id="31352-129">In the Partner Center menu, select **Customers**, then expand the customer's listing to see their **Microsoft ID**.</span></span>

   - <span data-ttu-id="31352-130">Az átvitelhez szükséges előfizetés-azonosító.</span><span class="sxs-lookup"><span data-stu-id="31352-130">The subscription ID to transfer.</span></span> <span data-ttu-id="31352-131">A bővített ügyféllistában válassza az Előfizetések megtekintése lehetőséget, majd **bontsa** ki a kiválasztott előfizetést az előfizetés **azonosítójának megtekintéséhez.**</span><span class="sxs-lookup"><span data-stu-id="31352-131">In the expanded customer listing, select **View Subscriptions**, then expand the chosen subscription to see the **Subscription ID**.</span></span>

   >[!Note]
   ><span data-ttu-id="31352-132">Az előfizetés átvitele két előfizetés-azonosítót ad vissza, amelyek az átvitt előfizetés Előfizetés szerkesztése lapján fognak látni: **1**– Az Partnerközpont-előfizetés azonosítóját számlázási célokra használjuk. </span><span class="sxs-lookup"><span data-stu-id="31352-132">Transferring a subscription results in two subscription IDs which you will see on the **Edit Subscription** page of the transferred subscription: **1**- The Partner Center Subscription ID is used for billing purposes.</span></span> <span data-ttu-id="31352-133">**2**– A rendszer megőrzi az eredeti Azure-előfizetés azonosítóját, és Partnerközpont az Azure felügyeleti portálján is.</span><span class="sxs-lookup"><span data-stu-id="31352-133">**2**-  The original Azure Subscription ID is retained and will appear in Partner Center as well as in the Azure Management portal.</span></span> <span data-ttu-id="31352-134">Ez az azonosító megjelenik a recon fájlban.</span><span class="sxs-lookup"><span data-stu-id="31352-134">This ID will appear in your recon file.</span></span>  <span data-ttu-id="31352-135">**Támogatási jegyek naplózásakor mindkét bérletet használnia kell.**</span><span class="sxs-lookup"><span data-stu-id="31352-135">**When logging support tickets, you need to use both IDs.**</span></span>

4. <span data-ttu-id="31352-136">Az előfizetéshez az ügyfél és az új partner:</span><span class="sxs-lookup"><span data-stu-id="31352-136">The customer and new partner for the subscription:</span></span>

   <span data-ttu-id="31352-137">Tekintse át az űrlapot, adja meg az új partner adatait, és írja alá.</span><span class="sxs-lookup"><span data-stu-id="31352-137">Review the form, fill in information about the new partner, and sign it.</span></span> <span data-ttu-id="31352-138">Ellenőrizze, hogy az új ügyfél rendelkezik-e szerződéssel.</span><span class="sxs-lookup"><span data-stu-id="31352-138">Confirm that the new customer has a contract agreement in place.</span></span> <span data-ttu-id="31352-139">Küldje vissza az űrlapot az aktuális rekordpartnernek.</span><span class="sxs-lookup"><span data-stu-id="31352-139">Send the form back to the current partner of record.</span></span>

   <span data-ttu-id="31352-140">*Fontos:* Ha az új CSP-partner nem rendelkezik viszonteladói kapcsolattal az ügyféllel, az előfizetés átadása előtt létre kell hoznia egyet.</span><span class="sxs-lookup"><span data-stu-id="31352-140">*Important*: If the new CSP Partner doesn't have a reseller relationship with the customer, they must establish one before the subscription is transferred.</span></span> <span data-ttu-id="31352-141">[Ennek mikéntjről itt talál információt:](request-a-relationship-with-a-customer.md).</span><span class="sxs-lookup"><span data-stu-id="31352-141">[You can find information on how to do this here](request-a-relationship-with-a-customer.md).</span></span>

   >[!Note]
   ><span data-ttu-id="31352-142">Az új CSP-partnernek és az ügyfélbérlőnek ugyanabban az országban kell lennie.</span><span class="sxs-lookup"><span data-stu-id="31352-142">The new CSP partner and the customer tenant must be in the same country.</span></span> 

5. <span data-ttu-id="31352-143">Aktuális partner:</span><span class="sxs-lookup"><span data-stu-id="31352-143">Current partner:</span></span>

   <span data-ttu-id="31352-144">Győződjön meg arról, hogy az űrlap mindkét partner-rendszergazda kapcsolattartási adatait tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="31352-144">Make sure the form includes contact information for both partner admins.</span></span> <span data-ttu-id="31352-145">Microsoft ügyfélszolgálata mindkét rendszergazdával kapcsolatba lép az átvitel ellenőrzéséhez.</span><span class="sxs-lookup"><span data-stu-id="31352-145">Microsoft Support will contact both admins to verify the transfer.</span></span> <span data-ttu-id="31352-146">Győződjön meg arról, hogy mindhárom aláírással van.</span><span class="sxs-lookup"><span data-stu-id="31352-146">Make sure you have all three signatures.</span></span> <span data-ttu-id="31352-147">Ezután a **Fájlfeltöltés lehetőséggel** csatolja a kitöltött űrlapot a meglévő szolgáltatáskéréshez.</span><span class="sxs-lookup"><span data-stu-id="31352-147">Then use the **File Upload** option to attach the completed form to your existing service request.</span></span> <span data-ttu-id="31352-148">A Microsoft támogatási szakembere nyolc órán belül visszatér Önhez, hogy ellenőrizze a nyugtát és a befejezést.</span><span class="sxs-lookup"><span data-stu-id="31352-148">A Microsoft support engineer will get back to you within eight business hours to validate receipt and completion.</span></span>

6. <span data-ttu-id="31352-149">Új partner:</span><span class="sxs-lookup"><span data-stu-id="31352-149">New partner:</span></span>

   <span data-ttu-id="31352-150">Frissítse az Azure-előfizetés beállításait, hogy eltávolítsa a régi partnert a fiókból.</span><span class="sxs-lookup"><span data-stu-id="31352-150">Update the Azure subscription settings to remove the old partner from the account.</span></span> <span data-ttu-id="31352-151">Két PowerShell-parancsmag futtatásával láthatja, hogy mely szerepkör-hozzárendelések vannak kiépítve.</span><span class="sxs-lookup"><span data-stu-id="31352-151">To see which role assignments are provisioned, run two PowerShell Commandlets.</span></span>

   - <span data-ttu-id="31352-152">Adja hozzá az új partnert viszonteladóként a fiókhoz:</span><span class="sxs-lookup"><span data-stu-id="31352-152">Add the new partner as the reseller on the account:</span></span>

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > <span data-ttu-id="31352-153">Az ügyfél **bérlőazonosítója** megjelenik a Partnerközpont az ügyfél **Microsoft-azonosítójaként.**</span><span class="sxs-lookup"><span data-stu-id="31352-153">The customer's **Tenant ID** appears in Partner Center as the customer's **Microsoft ID**.</span></span> <span data-ttu-id="31352-154">Egy adott ügyfél Microsoft-azonosítójának (bérlőazonosítójának) megkereséhez jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="31352-154">To find the Microsoft ID (Tenant ID) for a specific customer, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span> <span data-ttu-id="31352-155">Ezután válassza **az Ügyfelek** lehetőséget a menüből.</span><span class="sxs-lookup"><span data-stu-id="31352-155">Then select **Customers** from the menu.</span></span> <span data-ttu-id="31352-156">Keresse meg az ügyfelet a listában.</span><span class="sxs-lookup"><span data-stu-id="31352-156">Locate the customer on the list.</span></span> <span data-ttu-id="31352-157">A lefelé mutató nyílra kattintva bontsa ki az ügyfél termékoldalát.</span><span class="sxs-lookup"><span data-stu-id="31352-157">Select the down-arrow to expand the customer's listing.</span></span> <span data-ttu-id="31352-158">Az ügyfél tartománynevére és  Microsoft-azonosítójára vonatkozó adatokat **fog látni.**</span><span class="sxs-lookup"><span data-stu-id="31352-158">You will see information about the customer's *Domain name* and the customer's **Microsoft ID**.</span></span> <span data-ttu-id="31352-159">Használja a 16 jegyű **Microsoft-azonosítót** a PowerShell-parancsmagban.</span><span class="sxs-lookup"><span data-stu-id="31352-159">Use the 16-digit **Microsoft ID** in the PowerShell commandlet.</span></span>

   - <span data-ttu-id="31352-160">Megtekintheti a fiók szerepköreit, beleértve a korábbi CSP-partnereket is:</span><span class="sxs-lookup"><span data-stu-id="31352-160">View roles on the account, including previous CSP partners:</span></span>

     ```powershell
     Get-AzRoleAssignment
     ```

7. <span data-ttu-id="31352-161">Távolítsa el az elavult hozzáférési engedélyeket:</span><span class="sxs-lookup"><span data-stu-id="31352-161">Remove outdated access permissions:</span></span>

   - <span data-ttu-id="31352-162">A Partnerközpont válassza az Ügyfelek **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="31352-162">In the Partner Center menu, select **Customers**.</span></span>
   - <span data-ttu-id="31352-163">Keresse meg az ügyfelet a listában.</span><span class="sxs-lookup"><span data-stu-id="31352-163">Locate the customer on the list.</span></span> <span data-ttu-id="31352-164">Válassza ki (kattintson duplán) a vállalata nevére.</span><span class="sxs-lookup"><span data-stu-id="31352-164">Select (double-click) their company name.</span></span> <span data-ttu-id="31352-165">Ez a művelet megnyitja az ügyfél **Előfizetések oldalát.**</span><span class="sxs-lookup"><span data-stu-id="31352-165">This action opens the customer **Subscriptions** page.</span></span>
   - <span data-ttu-id="31352-166">Az ügyféladatok menüben válassza a **Szolgáltatáskezelés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="31352-166">In the customer detail menu, select **Service management**.</span></span>
   - <span data-ttu-id="31352-167">A **Microsoft Azure** alatt kattintson a hivatkozásra, hogy a következőre **a Microsoft Azure felügyeleti portálja.**</span><span class="sxs-lookup"><span data-stu-id="31352-167">Under **Microsoft Azure**, select the link to go to the **Microsoft Azure Management Portal**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="31352-168">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="31352-168">Next steps</span></span>

- <span data-ttu-id="31352-169">Töltse le a [CSP-előfizetés átvitele űrlapot.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA)</span><span class="sxs-lookup"><span data-stu-id="31352-169">Download the [CSP Subscription Transfer form](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).</span></span>

- <span data-ttu-id="31352-170">További információ [a többpartneres támogatásról.](multipartner.md)</span><span class="sxs-lookup"><span data-stu-id="31352-170">Learn about [multi-partner support](multipartner.md).</span></span>

- <span data-ttu-id="31352-171">[többpartneres támogatás.](multipartner.md)</span><span class="sxs-lookup"><span data-stu-id="31352-171">[multi-partner support](multipartner.md).</span></span>
- <span data-ttu-id="31352-172">[többcsatornás támogatás.](multichannel.md)</span><span class="sxs-lookup"><span data-stu-id="31352-172">[multi-channel support](multichannel.md).</span></span>
- [<span data-ttu-id="31352-173">Azure-előfizetések átvitele</span><span class="sxs-lookup"><span data-stu-id="31352-173">Transfer Azure subscriptions</span></span>](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)