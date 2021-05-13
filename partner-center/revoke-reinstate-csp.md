---
title: Rendszergazdai jogosultságok újbóli Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan segítheti az ügyfeleket a partner rendszergazdai jogosultságai visszaállításában, hogy a partner segítséget tudjon kérni az ügyfelek Azure CSP előfizetései kezeléséhez.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855420"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Rendszergazdai jogosultságok visszahelyezése egy ügyfél Azure CSP előfizetéséhez  

**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök

CSP-partnerként az ügyfelek gyakran elvárják, hogy Ön kezelje az Azure-használatot és azok rendszereit számukra. Ehhez rendszergazdai jogosultság szükséges. Bizonyos jogosultságok akkor kapnak, ha a viszonteladói kapcsolat létrejött az ügyféllel. Az ügyfél másokat is ad Önnek.

## <a name="admin-privileges-for-azure-in-csp"></a>Rendszergazdai jogosultságok a Azure in CSP

A rendszergazdai jogosultságoknak két szintje van a Azure in CSP.

**Bérlői szintű rendszergazdai jogosultságok** (**Delegált** rendszergazdai jogosultságok ) – A CSP-partnerek a CSP-viszonteladói kapcsolat létrehozása közben kapják meg ezeket a jogosultságokat az ügyfelekkel. A delegált rendszergazdai jogosultságok hozzáférést adnak a CSP-partnereknek az ügyfeleik bérlőihez, ami lehetővé teszi számukra olyan rendszergazdai funkciók elvégzését, mint a felhasználók hozzáadása/kezelése, a jelszavak visszaállítása és a felhasználói licencek kezelése.

**Előfizetési szintű rendszergazdai jogosultságok** – A CSP-partnerek ezeket a jogosultságokat az Azure CSP létrehozásakor kapják meg az ügyfeleik számára. Ezek a jogosultságok teljes hozzáférést számukra biztosít a CSP-partnerek számára ezekhez az előfizetésekhez, ami lehetővé teszi számukra az Azure-erőforrások építését és kezelését.

## <a name="reinstate-csp-partners-admin-privileges"></a>CSP-partnerek rendszergazdai jogosultságának újbóli state

Az ügyfél újra létrehozhatja a CSP szerepkör-hozzárendelést, ha Ön az AdminAgents csoport objektumazonosítóját adja meg az ügyfélnek. A delegált rendszergazdai jogosultságok visszaszerzése előtt az ügyféllel kell dolgoznia.

1. Jelentkezzen be a Partnerközpont irányítópultra, és a Partnerközpont menüjében válassza az Ügyfelek **lehetőséget.**

2. Válassza ki azt az ügyfelet, akinél dolgozik, és **kérjen viszonteladói kapcsolatot.** Ez a művelet létrehoz egy hivatkozást arra az ügyfélre, aki bérlői rendszergazdai jogosultságokkal rendelkezik.

3. Az ügyfélnek ki kell választania a hivatkozást, és jóvá kell hagynia a viszonteladói kapcsolatkérést.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Példa e-mailben viszonteladói kapcsolat létrehozására":::

4. Önnek, a partnernek csatlakoznia kell a partnerbérlőhöz, hogy le tudja szerezni az AdminAgents csoport objektumazonosítóját.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Az ügyfél, aki  tulajdonosi vagy felhasználói hozzáférés-rendszergazdai szerepkört tölt be, és jogosultsággal rendelkezik szerepkör-hozzárendelés létrehozására az előfizetés szintjén, a következőket teszi:


    1. Csatlakozik ahhoz a bérlőhöz, ahol a CSP-előfizetés létezik.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Csatlakozik az előfizetéshez (csak akkor alkalmazható, ha a felhasználó több előfizetésre vonatkozó szerepkör-hozzárendelési engedélyekkel rendelkezik a bérlőben).
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"


    3. Létrehozza a szerepkör-hozzárendelést
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Ha az előfizetés hatóköre helyett erőforráscsoport- vagy erőforrásszinten szeretne tulajdonosi szerepköri engedélyt ad, a következő parancsok működnek:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Következő lépések

- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)
