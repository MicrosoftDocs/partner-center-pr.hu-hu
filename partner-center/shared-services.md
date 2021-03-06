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
ms.openlocfilehash: a59cf0b271a0ccf5fd5a1d8e3e85ff43818a3801
ms.sourcegitcommit: fe867be44de3479607be3309940b904d7ea9fc6e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/06/2021
ms.locfileid: "102247707"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a><span data-ttu-id="9512c-103">Azure partner megosztott szolgáltatások hozzáadása, hogy a partnerek saját használatra tudják megvásárolni az Azure-előfizetéseket</span><span class="sxs-lookup"><span data-stu-id="9512c-103">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>

 
<span data-ttu-id="9512c-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="9512c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9512c-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="9512c-105">Global admin</span></span>
- <span data-ttu-id="9512c-106">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="9512c-106">Admin agent</span></span>
- <span data-ttu-id="9512c-107">Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="9512c-107">Sales agent</span></span>

<span data-ttu-id="9512c-108">Az Azure partner Shared Services egy új ajánlat típusa a CSP programban lévő partnereknek, amely lehetővé teszi, hogy a partnerek saját használatra vásárolják meg az Azure-előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="9512c-108">Azure Partner Shared Services is a new offer type for partners in the CSP program enabling partners to purchase Azure subscriptions for their own use.</span></span><span data-ttu-id="9512c-109">Lehetőséget teremt arra, hogy a partnerek egységes módszert használjanak az Azure megvásárlására, nyomon követésére és felügyeletére, valamint az Azure-licencek konszolidálása és a szerződések a Microsofttal való viszonteladásának lehetősége mellett.</span><span class="sxs-lookup"><span data-stu-id="9512c-109">  It creates the opportunity for partners to use a uniform method for purchasing, tracking, and managing Azure in addition to the ability to consolidate their Azure licensing and reselling agreements with Microsoft.</span></span> <span data-ttu-id="9512c-110">Az Azure partner megosztott szolgáltatásainak köszönhetően a partnerek mostantól ugyanolyan rugalmasan használhatják az Azure-előfizetéseket a CSP-ben, mint a Microsoft Nagyvállalati Szerződés és a webes Direct programokban, olyan forgatókönyveket nyitnak meg, mint például a fejlesztési és tesztelési környezetek létrehozása, a belső számítási feladatok üzembe helyezése és a megosztott szolgáltatások vagy több-bérlős alkalmazások</span><span class="sxs-lookup"><span data-stu-id="9512c-110">With Azure Partner Shared Services, partners now have the same flexibility to use Azure subscriptions in CSP as they do in the Microsoft Enterprise Agreement and Web Direct programs, opening up scenarios such as:  build development and test environments, deploy internal workloads, and host shared services or multi-tenant applications.</span></span>  

## <a name="create-the-shared-services-tenant"></a><span data-ttu-id="9512c-111">A megosztott szolgáltatások bérlő létrehozása</span><span class="sxs-lookup"><span data-stu-id="9512c-111">Create the shared services tenant</span></span>

1. <span data-ttu-id="9512c-112">Lépjen a **Beállítások**  >  **fiók beállításai**  >  **megosztott szolgáltatások** menüpontra.</span><span class="sxs-lookup"><span data-stu-id="9512c-112">Go to **Settings** > **Account settings** > **Shared services**.</span></span>

   :::image type="content" source="images/sharedservices2.png" alt-text="Fiókbeállítások > megosztott szolgáltatások":::

2. <span data-ttu-id="9512c-114">Ha még nem rendelkezik megosztott szolgáltatások Bérlővel, kattintson a **megosztott szolgáltatások létrehozása** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="9512c-114">If you don't already have a shared services tenant, click **Create shared services**.</span></span>

   :::image type="content" source="images/sharedservices3.png" alt-text="Megosztott szolgáltatások létrehozása":::

3. <span data-ttu-id="9512c-116">Ez létrehoz egy megosztott szolgáltatások bérlőt, és megvásárolja az Azure CSP megosztott szolgáltatásainak előfizetését, amelyet a megosztott erőforrásokhoz és a belső számítási feladatokhoz használhat.</span><span class="sxs-lookup"><span data-stu-id="9512c-116">This creates a shared services tenant and purchases the Azure CSP Shared Services subscription, to be used for shared resources and internal workload.</span></span>

   :::image type="content" source="images/sharedservices5.png" alt-text="A bérlő létrehozása és az előfizetés megvásárlása":::

## <a name="about-the-azure--internalshared-services-offer"></a><span data-ttu-id="9512c-118">Az Azure-Internal/Shared Services ajánlat</span><span class="sxs-lookup"><span data-stu-id="9512c-118">About the Azure- Internal/Shared Services offer</span></span>

- <span data-ttu-id="9512c-119">A Azure-Internal/Shared Services-előfizetés egy olyan új Azure-ajánlat típusa, amely a partner centeren keresztül érhető el, és a partnerek az Azure-t használják.</span><span class="sxs-lookup"><span data-stu-id="9512c-119">The Azure - Internal/Shared Services subscription is a new Azure offer type in CSP accessed through Partner Center that partners get for their own use of Azure.</span></span>

- <span data-ttu-id="9512c-120">Az Azure partner Shared Services-előfizetések jogosultak, és a RIs megvásárlására is használhatók.</span><span class="sxs-lookup"><span data-stu-id="9512c-120">Azure Partner Shared Services subscriptions are eligible and can be used to purchase RIs.</span></span>

- <span data-ttu-id="9512c-121">Az Azure-Internal/Shared Services ajánlat csak a megosztott szolgáltatások bérlőre alkalmazható.</span><span class="sxs-lookup"><span data-stu-id="9512c-121">The Azure - Internal/Shared Services offer can only be applied to the shared services tenant.</span></span>

- <span data-ttu-id="9512c-122">Az Azure-Internal/Shared Services-előfizetés elsődleges használata, hogy az Azure-t saját fejlesztési célokra használhatja.</span><span class="sxs-lookup"><span data-stu-id="9512c-122">The primary use for the Azure - Internal/Shared Services subscription is so that you can use Azure for your own development purposes.</span></span> <span data-ttu-id="9512c-123">Az ajánlat kiépítéséhez használt megosztott bérlő nem használható más szolgáltatásokhoz, például az Office 365-hez vagy a Dynamics-licencekhez.</span><span class="sxs-lookup"><span data-stu-id="9512c-123">The shared tenant you use to provision this offer cannot be used for other services such as Office 365 or Dynamics licenses.</span></span>

- <span data-ttu-id="9512c-124">Megszakíthatja az előfizetést, mint bármely más előfizetést.</span><span class="sxs-lookup"><span data-stu-id="9512c-124">You can cancel the subscription like any other subscription.</span></span> <span data-ttu-id="9512c-125">Lépjen a **Beállítások**  >  **nézet minden beállítás**  >  **megosztott szolgáltatások** menüpontra.</span><span class="sxs-lookup"><span data-stu-id="9512c-125">Go to the **settings** > **View all settings** > **Shared services**.</span></span> <span data-ttu-id="9512c-126">Válassza ki a Azure-Internal/Shared Services-előfizetést, és szakítsa meg.</span><span class="sxs-lookup"><span data-stu-id="9512c-126">Select the Azure - Internal/Shared Services subscription and cancel it.</span></span>

## <a name="accessing-azure-partner-shared-services-consumption-details"></a><span data-ttu-id="9512c-127">Az Azure partner megosztott szolgáltatások használati adatainak elérése</span><span class="sxs-lookup"><span data-stu-id="9512c-127">Accessing Azure Partner Shared Services consumption details</span></span>

<span data-ttu-id="9512c-128">Az Azure-beli felhasználást a CSP-számlán és a megbékélési fájlban találja.</span><span class="sxs-lookup"><span data-stu-id="9512c-128">You will find the Azure consumption on your CSP invoice and the reconciliation file.</span></span> <span data-ttu-id="9512c-129">Ez a számla Microsoft Azure tételének részeként fog szerepelni.</span><span class="sxs-lookup"><span data-stu-id="9512c-129">It will be included as part of Microsoft Azure line item in the invoice.</span></span> <span data-ttu-id="9512c-130">A részletes használati adatok az ajánlathoz létrehozott Bérlővel naplózott egyeztetési fájlban lesznek elérhetők.</span><span class="sxs-lookup"><span data-stu-id="9512c-130">The detailed consumption information will be available in the reconciliation file logged against the tenant that was created for this offer.</span></span>

## <a name="azure-partner-shared-services-pricing"></a><span data-ttu-id="9512c-131">Az Azure partner megosztott szolgáltatásainak díjszabása</span><span class="sxs-lookup"><span data-stu-id="9512c-131">Azure Partner Shared Services pricing</span></span>

<span data-ttu-id="9512c-132">Ha szeretné megtekinteni az Azure partner megosztott szolgáltatásainak új díjszabási fájlját, válassza a   >  **díjszabás és ajánlatok** eladása lehetőséget, és válassza ki az aktuális hónap árlista listáját.</span><span class="sxs-lookup"><span data-stu-id="9512c-132">To see the new pricing file for Azure Partner Shared Services go to **Sell** > **Pricing and offers** and select the current month's price list.</span></span> <span data-ttu-id="9512c-133">Az elkövetkező hetekben egy adott díj kártya API-t is kiadunk.</span><span class="sxs-lookup"><span data-stu-id="9512c-133">In the coming weeks, a specific rate card api will also be released.</span></span>

## <a name="marketplace-offers-and-azure-partner-shared-services"></a><span data-ttu-id="9512c-134">Piactéri ajánlatok és az Azure partner megosztott szolgáltatásai</span><span class="sxs-lookup"><span data-stu-id="9512c-134">Marketplace offers and Azure Partner Shared Services</span></span>

<span data-ttu-id="9512c-135">2019. március 1-től az Azure partner Shared Services (APSS) már nem támogatja a Piactéri ajánlatokat.</span><span class="sxs-lookup"><span data-stu-id="9512c-135">As of March 1, 2019, Azure Partner Shared Services (APSS) no longer supports Marketplace offers.</span></span>

|<span data-ttu-id="9512c-136">**Marketplace-támogatás**</span><span class="sxs-lookup"><span data-stu-id="9512c-136">**Marketplace support**</span></span>   |<span data-ttu-id="9512c-137">**A APSS a 2019. március 1. előtt támogatott**</span><span class="sxs-lookup"><span data-stu-id="9512c-137">**APSS supported before March 1, 2019**</span></span>|<span data-ttu-id="9512c-138">**2019. március 1-től**</span><span class="sxs-lookup"><span data-stu-id="9512c-138">**After March 1, 2019**</span></span>|
|---------------------------|:----------------------------|:-------------------|
|<span data-ttu-id="9512c-139">Saját licenc használata (BYOL) és ingyenes szolgáltatások</span><span class="sxs-lookup"><span data-stu-id="9512c-139">Bring your own license (BYOL) and free services</span></span>   | <span data-ttu-id="9512c-140">Igen</span><span class="sxs-lookup"><span data-stu-id="9512c-140">Yes</span></span>   | <span data-ttu-id="9512c-141">Nem</span><span class="sxs-lookup"><span data-stu-id="9512c-141">No</span></span>|
|<span data-ttu-id="9512c-142">Egyéb harmadik féltől származó Piactéri ajánlatok</span><span class="sxs-lookup"><span data-stu-id="9512c-142">Other third-party marketplace offers</span></span>   | <span data-ttu-id="9512c-143">Nem</span><span class="sxs-lookup"><span data-stu-id="9512c-143">No</span></span>   |<span data-ttu-id="9512c-144">Nem</span><span class="sxs-lookup"><span data-stu-id="9512c-144">No</span></span>|

<span data-ttu-id="9512c-145">A APSS használatával üzembe helyezett BYOL-vagy ingyenes szolgáltatásokkal kapcsolatos partnereinket nem érinti a rendszer. 2019. március 1-től azonban nem vásárolhat új BYOL vagy ingyenes szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="9512c-145">Partners who have BYOL or free services deployed using APSS will not be impacted; however after March 1, 2019 they will not be able to purchase new BYOL or free services.</span></span>

<span data-ttu-id="9512c-146">A piactéren elérhető ajánlatok teljes katalógusának kihasználásához (nem csak BYOL és ingyenes szolgáltatásokhoz) javasoljuk, hogy a CSP-partnerek a web Direct Azure-előfizetések használatával közös szolgáltatásokat telepítsenek.</span><span class="sxs-lookup"><span data-stu-id="9512c-146">To take advantage of the full catalog of Marketplace offers available (not just BYOL and free services), we recommend CSP partners deploy shared services using web direct Azure subscriptions.</span></span>  <span data-ttu-id="9512c-147">Azok a CSP-partnerek, akik korábban üzembe helyeztek harmadik féltől származó BYOL és ingyenes szolgáltatási erőforrásokat a piactéren, és továbbra is szeretnék használni őket, és több harmadik féltől származó ajánlatot is üzembe helyezhetnek, javasoljuk, hogy a APSS-előfizetés áttelepítését a [meglévő Azure-előfizetések áttelepítéséhez](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="9512c-147">CSP partners who have deployed third-party BYOL and free service resources from the Marketplace previously and wish to continue using them and deploy more third-party offerings are encouraged to migrate the APSS subscription to web direct [Migrating Existing Azure Subscriptions](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span></span>

<span data-ttu-id="9512c-148">Azok a partnerek, akik a APSS-előfizetés 2019. március 1. után való használatának folytatását tervezik, és új, harmadik féltől származó [BYOL-szolgáltatásokat](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) vagy ingyenes szolgáltatásokat kívánnak telepíteni, a független gyártóktól származó utasításokat követve telepíthetik ezeket a APSS-előfizetésekre.</span><span class="sxs-lookup"><span data-stu-id="9512c-148">Partners, who plan to continue using APSS subscription after the March 1, 2019 and wish to deploy new third-party [BYOL services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) or free services, can follow the instructions from ISVs to deploy these to their APSS subscriptions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9512c-149">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="9512c-149">Next steps</span></span>

- [<span data-ttu-id="9512c-150">Szoftver-előfizetések értékesítése felhőszolgáltatón keresztül</span><span class="sxs-lookup"><span data-stu-id="9512c-150">Sell software subscriptions through CSP</span></span>](csp-software-subscriptions.md)