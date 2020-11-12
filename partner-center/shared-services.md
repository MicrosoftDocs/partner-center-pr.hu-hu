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
ms.date: 11/11/2020
ms.openlocfilehash: 93ee3e142bf11c3b329fd27ec7320b93aea780b8
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/12/2020
ms.locfileid: "94532038"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a><span data-ttu-id="5d395-103">Azure partner megosztott szolgáltatások hozzáadása, hogy a partnerek saját használatra tudják megvásárolni az Azure-előfizetéseket</span><span class="sxs-lookup"><span data-stu-id="5d395-103">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>

 
<span data-ttu-id="5d395-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="5d395-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5d395-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="5d395-105">Global admin</span></span>
- <span data-ttu-id="5d395-106">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="5d395-106">Admin agent</span></span>
- <span data-ttu-id="5d395-107">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="5d395-107">Sales agent</span></span>

<span data-ttu-id="5d395-108">Az Azure partner Shared Services egy új ajánlat típusa a CSP programban lévő partnereknek, amely lehetővé teszi, hogy a partnerek saját használatra vásárolják meg az Azure-előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="5d395-108">Azure Partner Shared Services is a new offer type for partners in the CSP program enabling partners to purchase Azure subscriptions for their own use.</span></span><span data-ttu-id="5d395-109">Lehetőséget teremt arra, hogy a partnerek egységes módszert használjanak az Azure megvásárlására, nyomon követésére és felügyeletére, valamint az Azure-licencek konszolidálása és a szerződések a Microsofttal való viszonteladásának lehetősége mellett.</span><span class="sxs-lookup"><span data-stu-id="5d395-109">  It creates the opportunity for partners to use a uniform method for purchasing, tracking, and managing Azure in addition to the ability to consolidate their Azure licensing and reselling agreements with Microsoft.</span></span> <span data-ttu-id="5d395-110">Az Azure partner megosztott szolgáltatásainak köszönhetően a partnerek mostantól ugyanolyan rugalmasan használhatják az Azure-előfizetéseket a CSP-ben, mint a Microsoft Nagyvállalati Szerződés és a webes Direct programokban, olyan forgatókönyveket nyitnak meg, mint például a fejlesztési és tesztelési környezetek létrehozása, a belső számítási feladatok üzembe helyezése és a megosztott szolgáltatások vagy több-bérlős alkalmazások</span><span class="sxs-lookup"><span data-stu-id="5d395-110">With Azure Partner Shared Services, partners now have the same flexibility to use Azure subscriptions in CSP as they do in the Microsoft Enterprise Agreement and Web Direct programs, opening up scenarios such as:  build development and test environments, deploy internal workloads, and host shared services or multi-tenant applications.</span></span>  

## <a name="create-the-shared-services-tenant"></a><span data-ttu-id="5d395-111">A megosztott szolgáltatások bérlő létrehozása</span><span class="sxs-lookup"><span data-stu-id="5d395-111">Create the shared services tenant</span></span>

1. <span data-ttu-id="5d395-112">Lépjen a **Beállítások**  >  **fiók beállításai**  >  **megosztott szolgáltatások** menüpontra.</span><span class="sxs-lookup"><span data-stu-id="5d395-112">Go to **Settings** > **Account settings** > **Shared services**.</span></span>

   :::image type="content" source="images/sharedservices2.png" alt-text="Fiókbeállítások > megosztott szolgáltatások":::

2. <span data-ttu-id="5d395-114">Ha még nem rendelkezik megosztott szolgáltatások Bérlővel, kattintson a **megosztott szolgáltatások létrehozása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="5d395-114">If you don't already have a shared services tenant, click **Create shared services**.</span></span>

   :::image type="content" source="images/sharedservices3.png" alt-text="Megosztott szolgáltatások létrehozása":::

3. <span data-ttu-id="5d395-116">Ez létrehoz egy megosztott szolgáltatások bérlőt, és megvásárolja az Azure CSP megosztott szolgáltatásainak előfizetését, amelyet a megosztott erőforrásokhoz és a belső számítási feladatokhoz használhat.</span><span class="sxs-lookup"><span data-stu-id="5d395-116">This creates a shared services tenant and purchases the Azure CSP Shared Services subscription, to be used for shared resources and internal workload.</span></span>

   :::image type="content" source="images/sharedservices5.png" alt-text="A bérlő létrehozása és az előfizetés megvásárlása":::

## <a name="about-the-azure--internalshared-services-offer"></a><span data-ttu-id="5d395-118">Az Azure-Internal/Shared Services ajánlat</span><span class="sxs-lookup"><span data-stu-id="5d395-118">About the Azure- Internal/Shared Services offer</span></span>

- <span data-ttu-id="5d395-119">A Azure-Internal/Shared Services-előfizetés egy olyan új Azure-ajánlat típusa, amely a partner centeren keresztül érhető el, és a partnerek az Azure-t használják.</span><span class="sxs-lookup"><span data-stu-id="5d395-119">The Azure - Internal/Shared Services subscription is a new Azure offer type in CSP accessed through Partner Center that partners get for their own use of Azure.</span></span>

- <span data-ttu-id="5d395-120">Azure-Internal/Shared Services ajánlat kedvezményeket és ösztönzőket vehet igénybe.</span><span class="sxs-lookup"><span data-stu-id="5d395-120">Azure - Internal/Shared Services offer is eligible for discounts and incentives.</span></span>  <span data-ttu-id="5d395-121">Az Azure partner Shared Services-előfizetések jogosultak, és a RIs megvásárlására is használhatók.</span><span class="sxs-lookup"><span data-stu-id="5d395-121">Azure Partner Shared Services subscriptions are eligible and can be used to purchase RIs.</span></span>

- <span data-ttu-id="5d395-122">Az Azure-Internal/Shared Services ajánlat csak a megosztott szolgáltatások bérlőre alkalmazható.</span><span class="sxs-lookup"><span data-stu-id="5d395-122">The Azure - Internal/Shared Services offer can only be applied to the shared services tenant.</span></span>

- <span data-ttu-id="5d395-123">Az Azure-Internal/Shared Services-előfizetés elsődleges használata, hogy az Azure-t saját fejlesztési célokra használhatja.</span><span class="sxs-lookup"><span data-stu-id="5d395-123">The primary use for the Azure - Internal/Shared Services subscription is so that you can use Azure for your own development purposes.</span></span> <span data-ttu-id="5d395-124">Az ajánlat kiépítéséhez használt megosztott bérlő nem használható más szolgáltatásokhoz, például az Office 365-hez vagy a Dynamics-licencekhez.</span><span class="sxs-lookup"><span data-stu-id="5d395-124">The shared tenant you use to provision this offer cannot be used for other services such as Office 365 or Dynamics licenses.</span></span>

- <span data-ttu-id="5d395-125">Megszakíthatja az előfizetést, mint bármely más előfizetést.</span><span class="sxs-lookup"><span data-stu-id="5d395-125">You can cancel the subscription like any other subscription.</span></span> <span data-ttu-id="5d395-126">Lépjen a **Beállítások**  >  **nézet minden beállítás**  >  **megosztott szolgáltatások** menüpontra.</span><span class="sxs-lookup"><span data-stu-id="5d395-126">Go to the **settings** > **View all settings** > **Shared services**.</span></span> <span data-ttu-id="5d395-127">Válassza ki a Azure-Internal/Shared Services-előfizetést, és szakítsa meg.</span><span class="sxs-lookup"><span data-stu-id="5d395-127">Select the Azure - Internal/Shared Services subscription and cancel it.</span></span>

## <a name="accessing-azure-partner-shared-services-consumption-details"></a><span data-ttu-id="5d395-128">Az Azure partner megosztott szolgáltatások használati adatainak elérése</span><span class="sxs-lookup"><span data-stu-id="5d395-128">Accessing Azure Partner Shared Services consumption details</span></span>

<span data-ttu-id="5d395-129">Az Azure-beli felhasználást a CSP-számlán és a megbékélési fájlban találja.</span><span class="sxs-lookup"><span data-stu-id="5d395-129">You will find the Azure consumption on your CSP invoice and the reconciliation file.</span></span> <span data-ttu-id="5d395-130">Ez a számla Microsoft Azure tételének részeként fog szerepelni.</span><span class="sxs-lookup"><span data-stu-id="5d395-130">It will be included as part of Microsoft Azure line item in the invoice.</span></span> <span data-ttu-id="5d395-131">A részletes használati adatok az ajánlathoz létrehozott Bérlővel naplózott egyeztetési fájlban lesznek elérhetők.</span><span class="sxs-lookup"><span data-stu-id="5d395-131">The detailed consumption information will be available in the reconciliation file logged against the tenant that was created for this offer.</span></span>

## <a name="azure-partner-shared-services-pricing"></a><span data-ttu-id="5d395-132">Az Azure partner megosztott szolgáltatásainak díjszabása</span><span class="sxs-lookup"><span data-stu-id="5d395-132">Azure Partner Shared Services pricing</span></span>

<span data-ttu-id="5d395-133">Ha szeretné megtekinteni az Azure partner megosztott szolgáltatásainak új díjszabási fájlját, válassza a **Sell**  >  **díjszabás és ajánlatok** eladása lehetőséget, és válassza ki az aktuális hónap árlista listáját.</span><span class="sxs-lookup"><span data-stu-id="5d395-133">To see the new pricing file for Azure Partner Shared Services go to **Sell** > **Pricing and offers** and select the current month's price list.</span></span> <span data-ttu-id="5d395-134">Az elkövetkező hetekben egy adott díj kártya API-t is kiadunk.</span><span class="sxs-lookup"><span data-stu-id="5d395-134">In the coming weeks, a specific rate card api will also be released.</span></span>

## <a name="marketplace-offers-and-azure-partner-shared-services"></a><span data-ttu-id="5d395-135">Piactéri ajánlatok és az Azure partner megosztott szolgáltatásai</span><span class="sxs-lookup"><span data-stu-id="5d395-135">Marketplace offers and Azure Partner Shared Services</span></span>

<span data-ttu-id="5d395-136">2019. március 1-től az Azure partner Shared Services (APSS) már nem támogatja a Piactéri ajánlatokat.</span><span class="sxs-lookup"><span data-stu-id="5d395-136">As of March 1, 2019, Azure Partner Shared Services (APSS) no longer supports Marketplace offers.</span></span>

|<span data-ttu-id="5d395-137">**Marketplace-támogatás**</span><span class="sxs-lookup"><span data-stu-id="5d395-137">**Marketplace support**</span></span>   |<span data-ttu-id="5d395-138">**A APSS a 2019. március 1. előtt támogatott**</span><span class="sxs-lookup"><span data-stu-id="5d395-138">**APSS supported before March 1, 2019**</span></span>|<span data-ttu-id="5d395-139">**2019. március 1-től**</span><span class="sxs-lookup"><span data-stu-id="5d395-139">**After March 1, 2019**</span></span>|
|---------------------------|:----------------------------|:-------------------|
|<span data-ttu-id="5d395-140">Saját licenc használata (BYOL) és ingyenes szolgáltatások</span><span class="sxs-lookup"><span data-stu-id="5d395-140">Bring your own license (BYOL) and free services</span></span>   | <span data-ttu-id="5d395-141">Igen</span><span class="sxs-lookup"><span data-stu-id="5d395-141">Yes</span></span>   | <span data-ttu-id="5d395-142">Nem</span><span class="sxs-lookup"><span data-stu-id="5d395-142">No</span></span>|
|<span data-ttu-id="5d395-143">Egyéb harmadik féltől származó Piactéri ajánlatok</span><span class="sxs-lookup"><span data-stu-id="5d395-143">Other third-party marketplace offers</span></span>   | <span data-ttu-id="5d395-144">Nem</span><span class="sxs-lookup"><span data-stu-id="5d395-144">No</span></span>   |<span data-ttu-id="5d395-145">Nem</span><span class="sxs-lookup"><span data-stu-id="5d395-145">No</span></span>|

<span data-ttu-id="5d395-146">A APSS használatával üzembe helyezett BYOL-vagy ingyenes szolgáltatásokkal kapcsolatos partnereinket nem érinti a rendszer. 2019. március 1-től azonban nem vásárolhat új BYOL vagy ingyenes szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="5d395-146">Partners who have BYOL or free services deployed using APSS will not be impacted; however after March 1, 2019 they will not be able to purchase new BYOL or free services.</span></span>

<span data-ttu-id="5d395-147">A piactéren elérhető ajánlatok teljes katalógusának kihasználásához (nem csak BYOL és ingyenes szolgáltatásokhoz) javasoljuk, hogy a CSP-partnerek a web Direct Azure-előfizetések használatával közös szolgáltatásokat telepítsenek.</span><span class="sxs-lookup"><span data-stu-id="5d395-147">To take advantage of the full catalog of Marketplace offers available (not just BYOL and free services), we recommend CSP partners deploy shared services using web direct Azure subscriptions.</span></span>  <span data-ttu-id="5d395-148">Azok a CSP-partnerek, akik korábban üzembe helyeztek harmadik féltől származó BYOL és ingyenes szolgáltatási erőforrásokat a piactéren, és továbbra is szeretnék használni őket, és több harmadik féltől származó ajánlatot is üzembe helyezhetnek, javasoljuk, hogy a APSS-előfizetés áttelepítését a [meglévő Azure-előfizetések áttelepítéséhez](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="5d395-148">CSP partners who have deployed third-party BYOL and free service resources from the Marketplace previously and wish to continue using them and deploy more third-party offerings are encouraged to migrate the APSS subscription to web direct [Migrating Existing Azure Subscriptions](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span></span>

<span data-ttu-id="5d395-149">Azok a partnerek, akik a APSS-előfizetés 2019. március 1. után való használatának folytatását tervezik, és új, harmadik féltől származó [BYOL-szolgáltatásokat](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) vagy ingyenes szolgáltatásokat kívánnak telepíteni, a független gyártóktól származó utasításokat követve telepíthetik ezeket a APSS-előfizetésekre.</span><span class="sxs-lookup"><span data-stu-id="5d395-149">Partners, who plan to continue using APSS subscription after the March 1, 2019 and wish to deploy new third-party [BYOL services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) or free services, can follow the instructions from ISVs to deploy these to their APSS subscriptions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5d395-150">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="5d395-150">Next steps</span></span>

- [<span data-ttu-id="5d395-151">Szoftver-előfizetések értékesítése felhőszolgáltatón keresztül</span><span class="sxs-lookup"><span data-stu-id="5d395-151">Sell software subscriptions through CSP</span></span>](csp-software-subscriptions.md)