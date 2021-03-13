---
title: 'Rövid útmutató: privát Azure piactér kezelése a PowerShell használatával'
description: Ez a rövid útmutató bemutatja, hogyan kezelheti az ajánlatokat egy privát Azure piactéren a Azure PowerShell használatával.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412454"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>Rövid útmutató: privát Azure piactér kezelése a PowerShell használatával

Ez a cikk azt ismerteti, hogyan kezelheti az ajánlatokat egy privát Azure piactéren az az [. Marketplace](/powershell/module/az.marketplace) PowerShell-modul használatával.

> [!IMPORTANT]
> A privát Azure piactér jelenleg nyilvános előzetes verzióban érhető el. Erre az előzetes verzióra nem vonatkozik szolgáltatói szerződés. Az előzetes verzió használata NEM javasolt éles számítási feladatok esetén. Előfordulhat, hogy egyes funkciók nem támogatottak, vagy korlátozott képességekkel rendelkeznek. További információ: [Kiegészítő használati feltételek a Microsoft Azure előzetes verziójú termékeihez](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).

## <a name="requirements"></a>Követelmények

* Ha nem rendelkezik Azure-előfizetéssel, első lépésként mindössze néhány perc alatt létrehozhat egy [ingyenes](https://azure.microsoft.com/free/) fiókot.

* Ha a Azure PowerShell helyi használatát választja:
  * [Telepítse az az PowerShell-modult](/powershell/azure/install-az-ps).
  * Kapcsolódjon az Azure-fiókjához a [AzAccount](/powershell/module/az.accounts/connect-azaccount) parancsmag használatával.
* Ha a Azure Cloud Shell használatát választja:
  * További információ: [Azure Cloud Shell áttekintése](/azure/cloud-shell/overview) .

  > [!IMPORTANT]
  > Noha az az **. Marketplace** PowerShell-modul előzetes verzióban érhető el, a parancsmaggal külön kell telepítenie `Install-Module` . Miután ez a PowerShell-modul általánosan elérhetővé válik, a jövőbeli Az PowerShell modulkiadások részévé válik, és natívan elérhető lesz az Azure Cloud Shellből.

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* Ha több Azure-előfizetéssel rendelkezik, válassza ki a megfelelő előfizetést, amelyben az erőforrásokat számlázni kell. Válasszon ki egy adott előfizetést a [set-AzContext](/powershell/module/az.accounts/set-azcontext) parancsmag használatával.

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>Privát tárolók listázása

A privát áruházak listájának lekéréséhez használja a [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) parancsmagot. Az alábbi példa felsorolja a bérlői hatókörben létrehozott privát tárolókat.

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

## <a name="add-an-offer-to-a-private-marketplace"></a>Ajánlat hozzáadása privát piactérhez

Ha ajánlatot szeretne adni egy privát áruházhoz, használja a [set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) parancsmagot. A következő példa hozzáadja a megadott ajánlatot egy privát piactérhez a bérlői hatókörben létrehozott privát áruházhoz.

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

## <a name="get-private-store-offers"></a>Privát áruházbeli ajánlatok beszerzése

Egy vagy több privát áruházi ajánlat beszerzéséhez használja a [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) parancsmagot. Az alábbi példa olyan ajánlatokat kap, amelyek a bérlői hatókörben hozzáadott, a megadott privát áruházhoz vannak társítva.

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

## <a name="remove-an-offer"></a>Ajánlat eltávolítása

Ha el szeretne távolítani egy ajánlatot egy privát áruházból, használja a [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) parancsmagot. A következő példa egy olyan privát áruházból származó ajánlatot távolít el, amely a bérlői hatókörben lett létrehozva.

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>Következő lépések

[Privát Azure Marketplace létrehozása és kezelése](create-manage-private-azure-marketplace.md).