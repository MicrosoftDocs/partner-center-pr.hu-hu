---
title: Partner által létrehozott kredit a felügyelt szolgáltatásokhoz
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan számítják ki és fizetik ki a Microsoft partner által létrehozott kreditet (PEC) a felügyelt szolgáltatásokhoz, és hogy miként biztosítható a jogosultsága.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 010f74164b0428a5cd6ffcde5000b52ac6a6993f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624000"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="b03f3-103">A partneri jóváírás kiszámításának és kifizetésének részletei</span><span class="sxs-lookup"><span data-stu-id="b03f3-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="b03f3-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="b03f3-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b03f3-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="b03f3-105">Global admin</span></span>
- <span data-ttu-id="b03f3-106">Felhasználói rendszergazda</span><span class="sxs-lookup"><span data-stu-id="b03f3-106">User admin</span></span>
- <span data-ttu-id="b03f3-107">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="b03f3-107">Admin agent</span></span>
- <span data-ttu-id="b03f3-108">Számlázási adminisztrátor</span><span class="sxs-lookup"><span data-stu-id="b03f3-108">Billing admin</span></span>
- <span data-ttu-id="b03f3-109">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="b03f3-109">Sales agent</span></span>

<span data-ttu-id="b03f3-110">A felügyelt szolgáltatások (PEC) partner által létrehozott kreditje felismeri és jutalmazza a partnereket, akik a saját nonstop, illetve az ügyfelek teljes, Azure-környezetének felügyeletét és felügyeletét végzik.</span><span class="sxs-lookup"><span data-stu-id="b03f3-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="b03f3-111">A CSP-ben alapértelmezés szerint a partnerek megkapják a szükséges hozzáférési jogosultságokat az ügyfél előfizetéséhez, amely lehetővé teszi, hogy az előfizetéshez tartozó erőforrások 24 X 7 működési felügyeletét és felügyeletét végezzék el.</span><span class="sxs-lookup"><span data-stu-id="b03f3-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="b03f3-112">A következő szakasz ismerteti az ügyfelek által a transacting partnerhez való hozzáférés kiépítésének további módjait.</span><span class="sxs-lookup"><span data-stu-id="b03f3-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="b03f3-113">A havi számla összege a partneri jóváírás levonása utána érték.</span><span class="sxs-lookup"><span data-stu-id="b03f3-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="b03f3-114">A partnerek megtekinthetik a PEC részleteit a havi Recon-fájlon.</span><span class="sxs-lookup"><span data-stu-id="b03f3-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="b03f3-115">Az [Azure-csomag előfizetések és erőforrások kezelése](azure-plan-manage.md)című cikkből megtudhatja, hogy az ügyfél hogyan építhet ki hozzáférést a transacting partnerhez.</span><span class="sxs-lookup"><span data-stu-id="b03f3-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="b03f3-116">Olvassa el [a rendszergazdai jogosultságok visszaállítása az Azure CSP-előfizetésekhez](revoke-reinstate-csp.md) lehetőséget is.</span><span class="sxs-lookup"><span data-stu-id="b03f3-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="eligibility"></a><span data-ttu-id="b03f3-117">Támogathatósági</span><span class="sxs-lookup"><span data-stu-id="b03f3-117">Eligibility</span></span>

<span data-ttu-id="b03f3-118">A partner által létrehozott kredit (PEC) megszerzéséhez a következő követelmények érvényesek:</span><span class="sxs-lookup"><span data-stu-id="b03f3-118">In order to receive the partner earned credit (PEC), the following requirements apply:</span></span> 

- <span data-ttu-id="b03f3-119">Rendelkeznie kell egy aktív MPN-szerződéssel és egy érvényes szerepköralapú hozzáférés-vezérlési (RBAC) szerepkörrel, amely az Ön által kezelt Azure-eszközök számára szerzett kreditet kap.</span><span class="sxs-lookup"><span data-stu-id="b03f3-119">You must have an active MPN agreement and valid role-based access control (RBAC) role to receive earned credit for the Azure assets you manage.</span></span>

- <span data-ttu-id="b03f3-120">Az ügyfél Azure-erőforrásainak nonstop operatív vezérléssel és felügyelettel kell rendelkeznie a CSP-ben.</span><span class="sxs-lookup"><span data-stu-id="b03f3-120">You must have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span> <span data-ttu-id="b03f3-121">Ez azt jelenti, hogy rendszergazdai jogosultságokkal kell rendelkeznie az ügyfél Azure-előfizetéséhez, az Azure-erőforráscsoport, az Azure-erőforráshoz.</span><span class="sxs-lookup"><span data-stu-id="b03f3-121">This means you must have admin privileges on the customer’s Azure subscription, Azure resource group, Azure resource.</span></span> <span data-ttu-id="b03f3-122">Közvetett szolgáltatók és a közvetett viszonteladóik esetében a közvetett szolgáltató jogosult lesz a PEC-re, ha a közvetett szolgáltató vagy a közvetett viszonteladó vagy mindkettő rendelkezik ezzel az operatív ellenőrzéssel.</span><span class="sxs-lookup"><span data-stu-id="b03f3-122">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider or the indirect reseller or both have this operational control.</span></span> <span data-ttu-id="b03f3-123">További információ: [rendszergazdai jogosultságok visszaállítása az Azure CSP-előfizetésekhez](./revoke-reinstate-csp.md).</span><span class="sxs-lookup"><span data-stu-id="b03f3-123">To learn more about this, see [Reinstate admin privileges for Azure CSP subscriptions](./revoke-reinstate-csp.md).</span></span>

- <span data-ttu-id="b03f3-124">A fenti követelményeken felül a PEC csak az Azure-csomag fogyasztási díjszabásában felsorolt szolgáltatásokra vonatkozik, amelyeket az [Azure-csomag díjszabási](https://partner.microsoft.com/commerce/sales) lapjáról exportálhat.</span><span class="sxs-lookup"><span data-stu-id="b03f3-124">In addition to the requirements above, PEC is only applicable to services listed in the Azure plan consumption pricing, which you can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span>

- <span data-ttu-id="b03f3-125">A PEC **nem** alkalmazható a következő szolgáltatásokra:</span><span class="sxs-lookup"><span data-stu-id="b03f3-125">PEC is **not** applicable to the following services:</span></span>
    - <span data-ttu-id="b03f3-126">Azure-csomag – foglalások</span><span class="sxs-lookup"><span data-stu-id="b03f3-126">Azure Plan reservations</span></span>
    - <span data-ttu-id="b03f3-127">Harmadik féltől származó termékek, amelyek az Azure-csomag használati árát a címkék oszlopban vannak azonosítva</span><span class="sxs-lookup"><span data-stu-id="b03f3-127">Third-party products identified as Third Party in the Tags column of the Azure plan consumption price</span></span>
    - <span data-ttu-id="b03f3-128">A piactér árlista termékei</span><span class="sxs-lookup"><span data-stu-id="b03f3-128">Products in the Marketplace price list</span></span>
    - [<span data-ttu-id="b03f3-129">Azure spot Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="b03f3-129">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="b03f3-130">A PEC-t az Azure-erőforrás szintjén szerezték le.</span><span class="sxs-lookup"><span data-stu-id="b03f3-130">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="b03f3-131">Ha az előfizetés vagy az erőforráscsoport szintjén érvényes hozzáférése van, akkor minden olyan erőforrás, amely a magasabb entitást összesíti, a PEC-t fogja keresni.</span><span class="sxs-lookup"><span data-stu-id="b03f3-131">If you have valid access at either the subscription or resource group level, each resource that rolls up to the higher entity will earn PEC.</span></span>

- <span data-ttu-id="b03f3-132">A PEC részletei az [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) oldalán is elérhetők.</span><span class="sxs-lookup"><span data-stu-id="b03f3-132">Details on PEC are also available on the [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners) page.</span></span>

### <a name="calculation"></a><span data-ttu-id="b03f3-133">Számítás</span><span class="sxs-lookup"><span data-stu-id="b03f3-133">Calculation</span></span>

<span data-ttu-id="b03f3-134">A PEC napi rendszerességgel van kiszámítva, és a napi használati fájlban és a havi számlaengedmény-fájlban is megtekinthető.</span><span class="sxs-lookup"><span data-stu-id="b03f3-134">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="b03f3-135">Egy partnernek (közvetett szolgáltató vagy közvetett viszonteladó) hozzáféréssel kell rendelkeznie a teljes naphoz (nonstop) annak biztosításához, hogy a PEC-t keresnek.</span><span class="sxs-lookup"><span data-stu-id="b03f3-135">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="b03f3-136">A PEC kiszámítása napi rendszerességgel történik a felügyelt Azure-eszközökön.</span><span class="sxs-lookup"><span data-stu-id="b03f3-136">PEC is calculated on a daily basis on the managed Azure assets.</span></span> <span data-ttu-id="b03f3-137">Az állandó jogosultsági szintű hozzáférés a hónapban (a hozzáférés hatóköre) és az összes jogosult erőforrás (a hozzáférés hatóköre) megőrzi a teljes PEC-t.</span><span class="sxs-lookup"><span data-stu-id="b03f3-137">Partners retaining persistent privileged access through the month (span of access) and for all the eligible resources (scope of access) will earn full PEC.</span></span> <span data-ttu-id="b03f3-138">A hatókör-és a sávszélesség-csökkentés az adott hónapban alacsonyabb PEC-arányt eredményez.</span><span class="sxs-lookup"><span data-stu-id="b03f3-138">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="b03f3-139">A napi névleges használati fájl napi rendszerességgel jelenik meg egy Azure-eszközön, függetlenül attól, hogy a PEC van-e alkalmazva.</span><span class="sxs-lookup"><span data-stu-id="b03f3-139">Daily rated usage file shows on a daily basis on an Azure asset, whether PEC is applied or not.</span></span> <span data-ttu-id="b03f3-140">A partnerek riasztásokat is regisztrálhatnak az állandó jogosultsági szintű hozzáférés változásainak figyelésére.</span><span class="sxs-lookup"><span data-stu-id="b03f3-140">Partners can also enroll in alerts to monitor changes to persistent privileged access.</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="b03f3-141">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="b03f3-141">Azure Cost Management</span></span>

<span data-ttu-id="b03f3-142">A Cost Analysis Azure Cost Management (ACM) lehetővé teszi, hogy partnereként megtekintse a PEC előnyeit megillető költségeket.</span><span class="sxs-lookup"><span data-stu-id="b03f3-142">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="b03f3-143">A [Azure Portal](https://portal.azure.com)jelentkezzen be a partner bérlőbe, és válassza a **Cost Management + számlázás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b03f3-143">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="b03f3-144">**Cost Management** kiválasztása</span><span class="sxs-lookup"><span data-stu-id="b03f3-144">Select **Cost management**</span></span>

3. <span data-ttu-id="b03f3-145">**Cost Analysis** kiválasztása</span><span class="sxs-lookup"><span data-stu-id="b03f3-145">Select **Cost Analysis**</span></span>

   <span data-ttu-id="b03f3-146">A Cost Analysis View (költség elemzése) nézetben megjelennek a Számlázási fiók költségei, a Microsoft által megvásárolt és felhasznált összes szolgáltatás esetében.</span><span class="sxs-lookup"><span data-stu-id="b03f3-146">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="b03f3-147">Válassza a **PartnerEarnedCreditApplied** lehetőséget a kimutatás legördülő listájában a PEC-t alkalmazó költségek megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="b03f3-147">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="b03f3-148">Ha a **PartnerEarnedCreditApplied** tulajdonság értéke TRUE (igaz), a kapcsolódó díj a partner által létrehozott kredit előnye.</span><span class="sxs-lookup"><span data-stu-id="b03f3-148">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

   <span data-ttu-id="b03f3-149">Ha a PartnerEarnedCreditApplied tulajdonság értéke false (hamis), akkor a kapcsolódó költség nem teljesült a kredithez szükséges jogosultsággal, vagy a megvásárolt szolgáltatás nem jogosult a partner által szerzett kreditre.</span><span class="sxs-lookup"><span data-stu-id="b03f3-149">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

   >[!NOTE] 
   ><span data-ttu-id="b03f3-150">A szolgáltatások használata általában 8-24 órát vesz igénybe **Cost Managementban** , és a PEC-kreditek 48 órán belül megjelennek a Azure Cost Managementban való hozzáférés időpontjában.</span><span class="sxs-lookup"><span data-stu-id="b03f3-150">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="b03f3-151">A Group By, a Group By, a **PartnerEarnedCreditApplied** tulajdonság és a szűrési funkció alapján is szűrheti **a szűrési** funkciókat a PEC-t használó költségek és a PEC-t nem alkalmazó költségek részletezése céljából.</span><span class="sxs-lookup"><span data-stu-id="b03f3-151">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b03f3-152">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="b03f3-152">Next steps</span></span>

- [<span data-ttu-id="b03f3-153">Partner által létrehozott kredit – áttekintés</span><span class="sxs-lookup"><span data-stu-id="b03f3-153">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="b03f3-154">A partneri kreditek kiszámítására vonatkozó részletes példákat az árlista tartalmazza, amely a partner Center irányítópultján érhető el (bejelentkezés szükséges).</span><span class="sxs-lookup"><span data-stu-id="b03f3-154">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="b03f3-155">Áttérés az Azure planre – első lépések</span><span class="sxs-lookup"><span data-stu-id="b03f3-155">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="b03f3-156">Az Azure-csomagban foglalt előfizetések és erőforrások kezelése</span><span class="sxs-lookup"><span data-stu-id="b03f3-156">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="b03f3-157">Rendszergazdai jogosultságok visszavonása vagy újraindítása az Azure CSP-előfizetésekhez</span><span class="sxs-lookup"><span data-stu-id="b03f3-157">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
