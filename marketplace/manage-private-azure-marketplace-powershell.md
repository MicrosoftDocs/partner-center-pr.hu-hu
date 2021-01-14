---
title: 'Rövid útmutató: privát Azure piactér kezelése a PowerShell használatával'
description: Ez a rövid útmutató bemutatja, hogyan kezelheti az ajánlatokat egy privát Azure piactéren a Azure PowerShell használatával.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d0021be17ab12b6e549b0e5263772a4a1e42f8a3
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182341"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="4232b-103">Rövid útmutató: privát Azure piactér kezelése a PowerShell használatával</span><span class="sxs-lookup"><span data-stu-id="4232b-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="4232b-104">Ez a cikk azt ismerteti, hogyan kezelheti az ajánlatokat egy privát Azure piactéren az az [. Marketplace](/powershell/module/az.marketplace) PowerShell-modul használatával.</span><span class="sxs-lookup"><span data-stu-id="4232b-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4232b-105">A privát Azure piactér jelenleg nyilvános előzetes verzióban érhető el.</span><span class="sxs-lookup"><span data-stu-id="4232b-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="4232b-106">Erre az előzetes verzióra nem vonatkozik szolgáltatói szerződés.</span><span class="sxs-lookup"><span data-stu-id="4232b-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="4232b-107">Az előzetes verzió használata NEM javasolt éles számítási feladatok esetén.</span><span class="sxs-lookup"><span data-stu-id="4232b-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="4232b-108">Előfordulhat, hogy egyes funkciók nem támogatottak, vagy korlátozott képességekkel rendelkeznek.</span><span class="sxs-lookup"><span data-stu-id="4232b-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="4232b-109">További információ: [Kiegészítő használati feltételek a Microsoft Azure előzetes verziójú termékeihez](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="4232b-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="4232b-110">Követelmények</span><span class="sxs-lookup"><span data-stu-id="4232b-110">Requirements</span></span>

* <span data-ttu-id="4232b-111">Ha nem rendelkezik Azure-előfizetéssel, első lépésként mindössze néhány perc alatt létrehozhat egy [ingyenes](https://azure.microsoft.com/free/) fiókot.</span><span class="sxs-lookup"><span data-stu-id="4232b-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="4232b-112">Ha a Azure PowerShell helyi használatát választja:</span><span class="sxs-lookup"><span data-stu-id="4232b-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="4232b-113">[Telepítse az az PowerShell-modult](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="4232b-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="4232b-114">Kapcsolódjon az Azure-fiókjához a [AzAccount](/powershell/module/az.accounts/connect-azaccount) parancsmag használatával.</span><span class="sxs-lookup"><span data-stu-id="4232b-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="4232b-115">Ha a Azure Cloud Shell használatát választja:</span><span class="sxs-lookup"><span data-stu-id="4232b-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="4232b-116">További információ: [Azure Cloud Shell áttekintése](/azure/cloud-shell/overview) .</span><span class="sxs-lookup"><span data-stu-id="4232b-116">See [Overview of Azure Cloud Shell](/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="4232b-117">Noha az az **. Marketplace** PowerShell-modul előzetes verzióban érhető el, a parancsmaggal külön kell telepítenie `Install-Module` .</span><span class="sxs-lookup"><span data-stu-id="4232b-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="4232b-118">Miután ez a PowerShell-modul általánosan elérhetővé válik, a jövőbeli Az PowerShell modulkiadások részévé válik, és natívan elérhető lesz az Azure Cloud Shellből.</span><span class="sxs-lookup"><span data-stu-id="4232b-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="4232b-119">Ha több Azure-előfizetéssel rendelkezik, válassza ki a megfelelő előfizetést, amelyben az erőforrásokat számlázni kell.</span><span class="sxs-lookup"><span data-stu-id="4232b-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="4232b-120">Válasszon ki egy adott előfizetést a [set-AzContext](/powershell/module/az.accounts/set-azcontext) parancsmag használatával.</span><span class="sxs-lookup"><span data-stu-id="4232b-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="4232b-121">Privát tárolók listázása</span><span class="sxs-lookup"><span data-stu-id="4232b-121">List private stores</span></span>

<span data-ttu-id="4232b-122">A privát áruházak listájának lekéréséhez használja a [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) parancsmagot.</span><span class="sxs-lookup"><span data-stu-id="4232b-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="4232b-123">Az alábbi példa felsorolja a bérlői hatókörben létrehozott privát tárolókat.</span><span class="sxs-lookup"><span data-stu-id="4232b-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="4232b-124">Ajánlat hozzáadása privát piactérhez</span><span class="sxs-lookup"><span data-stu-id="4232b-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="4232b-125">Ha ajánlatot szeretne adni egy privát áruházhoz, használja a [set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) parancsmagot.</span><span class="sxs-lookup"><span data-stu-id="4232b-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="4232b-126">A következő példa hozzáadja a megadott ajánlatot egy privát piactérhez a bérlői hatókörben létrehozott privát áruházhoz.</span><span class="sxs-lookup"><span data-stu-id="4232b-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="4232b-127">Privát áruházbeli ajánlatok beszerzése</span><span class="sxs-lookup"><span data-stu-id="4232b-127">Get private store offers</span></span>

<span data-ttu-id="4232b-128">Egy vagy több privát áruházi ajánlat beszerzéséhez használja a [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) parancsmagot.</span><span class="sxs-lookup"><span data-stu-id="4232b-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="4232b-129">Az alábbi példa olyan ajánlatokat kap, amelyek a bérlői hatókörben hozzáadott, a megadott privát áruházhoz vannak társítva.</span><span class="sxs-lookup"><span data-stu-id="4232b-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="4232b-130">Ajánlat eltávolítása</span><span class="sxs-lookup"><span data-stu-id="4232b-130">Remove an offer</span></span>

<span data-ttu-id="4232b-131">Ha el szeretne távolítani egy ajánlatot egy privát áruházból, használja a [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) parancsmagot.</span><span class="sxs-lookup"><span data-stu-id="4232b-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="4232b-132">A következő példa egy olyan privát áruházból származó ajánlatot távolít el, amely a bérlői hatókörben lett létrehozva.</span><span class="sxs-lookup"><span data-stu-id="4232b-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="4232b-133">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="4232b-133">Next steps</span></span>

<span data-ttu-id="4232b-134">[Privát Azure Marketplace létrehozása és kezelése](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="4232b-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>