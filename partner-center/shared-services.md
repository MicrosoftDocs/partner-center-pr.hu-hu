---
title: Azure partner megosztott szolgáltatások hozzáadása
description: Az Azure partner megosztott szolgáltatásaival saját használatra vásárolhat Azure-előfizetéseket, és egységes módszert használhat az Azure megvásárlásához, nyomon követéséhez és kezeléséhez.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 49b5bd1c9a7cd4c56f2fac28a45cc8a4b922b9b0
ms.sourcegitcommit: 2d11dbdcc2b1e64ad16d29182824984517470a63
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/24/2020
ms.locfileid: "92530103"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a><span data-ttu-id="ff363-103">Azure partner megosztott szolgáltatások hozzáadása, hogy a partnerek saját használatra tudják megvásárolni az Azure-előfizetéseket</span><span class="sxs-lookup"><span data-stu-id="ff363-103">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>

<span data-ttu-id="ff363-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="ff363-104">**Applies to**</span></span>

- <span data-ttu-id="ff363-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="ff363-105">Partner Center</span></span>
 
<span data-ttu-id="ff363-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="ff363-106">**Appropriate roles**</span></span>

- <span data-ttu-id="ff363-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="ff363-107">Global admin</span></span>
- <span data-ttu-id="ff363-108">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="ff363-108">Admin agent</span></span>
- <span data-ttu-id="ff363-109">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="ff363-109">Sales agent</span></span>

<span data-ttu-id="ff363-110">Az Azure partner Shared Services egy új ajánlat típusa a CSP programban lévő partnereknek, amely lehetővé teszi, hogy a partnerek saját használatra vásárolják meg az Azure-előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="ff363-110">Azure Partner Shared Services is a new offer type for partners in the CSP program enabling partners to purchase Azure subscriptions for their own use.</span></span><span data-ttu-id="ff363-111">Lehetőséget teremt arra, hogy a partnerek egységes módszert használjanak az Azure megvásárlására, nyomon követésére és felügyeletére, valamint az Azure-licencek konszolidálása és a szerződések a Microsofttal való viszonteladásának lehetősége mellett.</span><span class="sxs-lookup"><span data-stu-id="ff363-111">  It creates the opportunity for partners to use a uniform method for purchasing, tracking, and managing Azure in addition to the ability to consolidate their Azure licensing and reselling agreements with Microsoft.</span></span> <span data-ttu-id="ff363-112">Az Azure partner megosztott szolgáltatásainak köszönhetően a partnerek mostantól ugyanolyan rugalmasan használhatják az Azure-előfizetéseket a CSP-ben, mint a Microsoft Nagyvállalati Szerződés és a webes Direct programokban, olyan forgatókönyveket nyitnak meg, mint például a fejlesztési és tesztelési környezetek létrehozása, a belső számítási feladatok üzembe helyezése és a megosztott szolgáltatások vagy több-bérlős alkalmazások</span><span class="sxs-lookup"><span data-stu-id="ff363-112">With Azure Partner Shared Services, partners now have the same flexibility to use Azure subscriptions in CSP as they do in the Microsoft Enterprise Agreement and Web Direct programs, opening up scenarios such as:  build development and test environments, deploy internal workloads, and host shared services or multi-tenant applications.</span></span>  

## <a name="create-the-shared-services-tenant"></a><span data-ttu-id="ff363-113">A megosztott szolgáltatások bérlő létrehozása</span><span class="sxs-lookup"><span data-stu-id="ff363-113">Create the shared services tenant</span></span>

1. <span data-ttu-id="ff363-114">Lépjen a **Beállítások**  >  **fiók beállításai**  >  **megosztott szolgáltatások** menüpontra.</span><span class="sxs-lookup"><span data-stu-id="ff363-114">Go to **Settings** > **Account settings** > **Shared services** .</span></span>

   :::image type="content" source="images/sharedservices2.png" alt-text="Fiókbeállítások > megosztott szolgáltatások":::

2. <span data-ttu-id="ff363-116">Ha még nem rendelkezik megosztott szolgáltatások Bérlővel, kattintson a **megosztott szolgáltatások létrehozása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="ff363-116">If you don't already have a shared services tenant, click **Create shared services** .</span></span>

   :::image type="content" source="images/sharedservices3.png" alt-text="Megosztott szolgáltatások létrehozása":::

3. <span data-ttu-id="ff363-118">Ez létrehoz egy megosztott szolgáltatások bérlőt, és megvásárolja az Azure CSP megosztott szolgáltatásainak előfizetését, amelyet a megosztott erőforrásokhoz és a belső számítási feladatokhoz használhat.</span><span class="sxs-lookup"><span data-stu-id="ff363-118">This creates a shared services tenant and purchases the Azure CSP Shared Services subscription, to be used for shared resources and internal workload.</span></span>

   :::image type="content" source="images/sharedservices5.png" alt-text="A bérlő létrehozása és az előfizetés megvásárlása":::

## <a name="about-the-azure--internalshared-services-offer"></a><span data-ttu-id="ff363-120">Az Azure-Internal/Shared Services ajánlat</span><span class="sxs-lookup"><span data-stu-id="ff363-120">About the Azure- Internal/Shared Services offer</span></span>

- <span data-ttu-id="ff363-121">A Azure-Internal/Shared Services-előfizetés egy olyan új Azure-ajánlat típusa, amely a partner centeren keresztül érhető el, és a partnerek az Azure-t használják.</span><span class="sxs-lookup"><span data-stu-id="ff363-121">The Azure - Internal/Shared Services subscription is a new Azure offer type in CSP accessed through Partner Center that partners get for their own use of Azure.</span></span>

- <span data-ttu-id="ff363-122">Azure-Internal/Shared Services ajánlat nem jogosult kedvezmények és ösztönzők használatára.</span><span class="sxs-lookup"><span data-stu-id="ff363-122">Azure - Internal/Shared Services offer is not eligible for discounts and incentives.</span></span>

- <span data-ttu-id="ff363-123">Az Azure-Internal/Shared Services ajánlat csak a megosztott szolgáltatások bérlőre alkalmazható.</span><span class="sxs-lookup"><span data-stu-id="ff363-123">The Azure - Internal/Shared Services offer can only be applied to the shared services tenant.</span></span>

- <span data-ttu-id="ff363-124">Az Azure-Internal/Shared Services-előfizetés elsődleges használata, hogy az Azure-t saját fejlesztési célokra használhatja.</span><span class="sxs-lookup"><span data-stu-id="ff363-124">The primary use for the Azure - Internal/Shared Services subscription is so that you can use Azure for your own development purposes.</span></span> <span data-ttu-id="ff363-125">Az ajánlat kiépítéséhez használt megosztott bérlő nem használható más szolgáltatásokhoz, például az Office 365-hez vagy a Dynamics-licencekhez.</span><span class="sxs-lookup"><span data-stu-id="ff363-125">The shared tenant you use to provision this offer cannot be used for other services such as Office 365 or Dynamics licenses.</span></span>

- <span data-ttu-id="ff363-126">Megszakíthatja az előfizetést, mint bármely más előfizetést.</span><span class="sxs-lookup"><span data-stu-id="ff363-126">You can cancel the subscription like any other subscription.</span></span> <span data-ttu-id="ff363-127">Lépjen a **Beállítások**  >  **nézet minden beállítás**  >  **megosztott szolgáltatások** menüpontra.</span><span class="sxs-lookup"><span data-stu-id="ff363-127">Go to the **settings** > **View all settings** > **Shared services** .</span></span> <span data-ttu-id="ff363-128">Válassza ki a Azure-Internal/Shared Services-előfizetést, és szakítsa meg.</span><span class="sxs-lookup"><span data-stu-id="ff363-128">Select the Azure - Internal/Shared Services subscription and cancel it.</span></span>

## <a name="accessing-azure-partner-shared-services-consumption-details"></a><span data-ttu-id="ff363-129">Az Azure partner megosztott szolgáltatások használati adatainak elérése</span><span class="sxs-lookup"><span data-stu-id="ff363-129">Accessing Azure Partner Shared Services consumption details</span></span>

<span data-ttu-id="ff363-130">Az Azure-beli felhasználást a CSP-számlán és a megbékélési fájlban találja.</span><span class="sxs-lookup"><span data-stu-id="ff363-130">You will find the Azure consumption on your CSP invoice and the reconciliation file.</span></span> <span data-ttu-id="ff363-131">Ez a számla Microsoft Azure tételének részeként fog szerepelni.</span><span class="sxs-lookup"><span data-stu-id="ff363-131">It will be included as part of Microsoft Azure line item in the invoice.</span></span> <span data-ttu-id="ff363-132">A részletes használati adatok az ajánlathoz létrehozott Bérlővel naplózott egyeztetési fájlban lesznek elérhetők.</span><span class="sxs-lookup"><span data-stu-id="ff363-132">The detailed consumption information will be available in the reconciliation file logged against the tenant that was created for this offer.</span></span>

## <a name="azure-partner-shared-services-pricing"></a><span data-ttu-id="ff363-133">Az Azure partner megosztott szolgáltatásainak díjszabása</span><span class="sxs-lookup"><span data-stu-id="ff363-133">Azure Partner Shared Services pricing</span></span>

<span data-ttu-id="ff363-134">Ha szeretné megtekinteni az Azure partner megosztott szolgáltatásainak új díjszabási fájlját, válassza a **Sell**  >  **díjszabás és ajánlatok** eladása lehetőséget, és válassza ki az aktuális hónap árlista listáját.</span><span class="sxs-lookup"><span data-stu-id="ff363-134">To see the new pricing file for Azure Partner Shared Services go to **Sell** > **Pricing and offers** and select the current month's price list.</span></span> <span data-ttu-id="ff363-135">Az elkövetkező hetekben egy adott díj kártya API-t is kiadunk.</span><span class="sxs-lookup"><span data-stu-id="ff363-135">In the coming weeks, a specific rate card api will also be released.</span></span>

## <a name="marketplace-offers-and-azure-partner-shared-services"></a><span data-ttu-id="ff363-136">Piactéri ajánlatok és az Azure partner megosztott szolgáltatásai</span><span class="sxs-lookup"><span data-stu-id="ff363-136">Marketplace offers and Azure Partner Shared Services</span></span>

<span data-ttu-id="ff363-137">2019. március 1-től az Azure partner Shared Services (APSS) már nem támogatja a Piactéri ajánlatokat.</span><span class="sxs-lookup"><span data-stu-id="ff363-137">As of March 1, 2019, Azure Partner Shared Services (APSS) no longer supports Marketplace offers.</span></span>

|<span data-ttu-id="ff363-138">**Marketplace-támogatás**</span><span class="sxs-lookup"><span data-stu-id="ff363-138">**Marketplace support**</span></span>   |<span data-ttu-id="ff363-139">**A APSS a 2019. március 1. előtt támogatott**</span><span class="sxs-lookup"><span data-stu-id="ff363-139">**APSS supported before March 1, 2019**</span></span>|<span data-ttu-id="ff363-140">**2019. március 1-től**</span><span class="sxs-lookup"><span data-stu-id="ff363-140">**After March 1, 2019**</span></span>|
|---------------------------|:----------------------------|:-------------------|
|<span data-ttu-id="ff363-141">Saját licenc használata (BYOL) és ingyenes szolgáltatások</span><span class="sxs-lookup"><span data-stu-id="ff363-141">Bring your own license (BYOL) and free services</span></span>   | <span data-ttu-id="ff363-142">Igen</span><span class="sxs-lookup"><span data-stu-id="ff363-142">Yes</span></span>   | <span data-ttu-id="ff363-143">Nem</span><span class="sxs-lookup"><span data-stu-id="ff363-143">No</span></span>|
|<span data-ttu-id="ff363-144">Egyéb harmadik féltől származó Piactéri ajánlatok</span><span class="sxs-lookup"><span data-stu-id="ff363-144">Other third-party marketplace offers</span></span>   | <span data-ttu-id="ff363-145">Nem</span><span class="sxs-lookup"><span data-stu-id="ff363-145">No</span></span>   |<span data-ttu-id="ff363-146">Nem</span><span class="sxs-lookup"><span data-stu-id="ff363-146">No</span></span>|

<span data-ttu-id="ff363-147">A APSS használatával üzembe helyezett BYOL-vagy ingyenes szolgáltatásokkal kapcsolatos partnereinket nem érinti a rendszer. 2019. március 1-től azonban nem vásárolhat új BYOL vagy ingyenes szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="ff363-147">Partners who have BYOL or free services deployed using APSS will not be impacted; however after March 1, 2019 they will not be able to purchase new BYOL or free services.</span></span>

<span data-ttu-id="ff363-148">A piactéren elérhető ajánlatok teljes katalógusának kihasználásához (nem csak BYOL és ingyenes szolgáltatásokhoz) javasoljuk, hogy a CSP-partnerek a web Direct Azure-előfizetések használatával közös szolgáltatásokat telepítsenek.</span><span class="sxs-lookup"><span data-stu-id="ff363-148">To take advantage of the full catalog of Marketplace offers available (not just BYOL and free services), we recommend CSP partners deploy shared services using web direct Azure subscriptions.</span></span>  <span data-ttu-id="ff363-149">Azok a CSP-partnerek, akik korábban üzembe helyeztek harmadik féltől származó BYOL és ingyenes szolgáltatási erőforrásokat a piactéren, és továbbra is szeretnék használni őket, és több harmadik féltől származó ajánlatot is üzembe helyezhetnek, javasoljuk, hogy a APSS-előfizetés áttelepítését a [meglévő Azure-előfizetések áttelepítéséhez](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="ff363-149">CSP partners who have deployed third-party BYOL and free service resources from the Marketplace previously and wish to continue using them and deploy more third-party offerings are encouraged to migrate the APSS subscription to web direct [Migrating Existing Azure Subscriptions](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span></span>

<span data-ttu-id="ff363-150">Azok a partnerek, akik a APSS-előfizetés 2019. március 1. után való használatának folytatását tervezik, és új, harmadik féltől származó [BYOL-szolgáltatásokat](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) vagy ingyenes szolgáltatásokat kívánnak telepíteni, a független gyártóktól származó utasításokat követve telepíthetik ezeket a APSS-előfizetésekre.</span><span class="sxs-lookup"><span data-stu-id="ff363-150">Partners, who plan to continue using APSS subscription after the March 1, 2019 and wish to deploy new third-party [BYOL services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) or free services, can follow the instructions from ISVs to deploy these to their APSS subscriptions.</span></span>