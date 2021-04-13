---
title: Rendszergazdai jogosultságok visszaállítása az Azure CSP-hez
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy az ügyfelek hogyan állíthatják vissza a partner rendszergazdai jogosultságait, hogy a partner segítsen kezelni az ügyfelek Azure CSP-előfizetéseit.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315847"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Rendszergazdai jogosultságok visszaállítása az ügyfél Azure CSP-előfizetései esetében  

**Alkalmazható szerepkörök**

- Globális rendszergazda
- Felügyeleti ügynök

CSP-partnerként az ügyfelek gyakran elvárják, hogy az Azure-használatot és azok rendszereit is kezelni tudják. Ehhez rendszergazdai jogosultságokkal kell rendelkeznie. Bizonyos jogosultságokat akkor kell megadni, ha a viszonteladói kapcsolat létrejött az ügyféllel. Másokat az ügyfél biztosít Önnek.

## <a name="admin-privileges-for-azure-in-csp"></a>Rendszergazdai jogosultságok az Azure-ban a CSP-ben

Az Azure-ban a CSP-ben két rendszergazdai jogosultsági szint van.

**Bérlői szintű rendszergazdai jogosultságok** (**delegált rendszergazdai jogosultságok**) – a CSP-partnerek megkapják ezeket a jogosultságokat a CSP viszonteladói kapcsolat ügyfelekkel való létrehozásakor. A delegált rendszergazdai jogosultságok lehetővé teszik a CSP-partnerek számára, hogy hozzáférjenek az ügyfelek bérlői számára, így olyan rendszergazdai feladatokat hajthatnak végre, mint például felhasználók hozzáadása/kezelése, jelszavak alaphelyzetbe állítása és felhasználói licencek kezelése.

**Előfizetés szintű rendszergazdai jogosultságok** – a CSP-partnerek megkapják ezeket a jogosultságokat az Azure CSP-előfizetések létrehozásakor az ügyfelek számára. Ezek a jogosultságok lehetővé teszik a CSP-partnerek számára az Azure-erőforrások kiépítését és kezelését.

## <a name="reinstate-csp-partners-admin-privileges"></a>A CSP-partnerek rendszergazdai jogosultságának visszaállítása

Az ügyfél újra létrehozhatja a CSP szerepkör-hozzárendelést, ha megadja az ügyfélnek az AdminAgents-csoport objektumazonosítót. A delegált rendszergazdai jogosultságok visszaszerzéséhez az ügyfelet kell használnia.

1. Jelentkezzen be a partner Center irányítópultra, és válassza a partner Center menü **ügyfelek** elemét.

2. Válassza ki azt az ügyfelet, aki dolgozik, és **kérjen egy viszonteladói kapcsolatot.** Ez létrehoz egy hivatkozást arra a felhasználóra, aki bérlői rendszergazdai jogosultságokkal rendelkezik.

3. Az ügyfélnek ki kell választania a hivatkozást, és jóvá kell hagynia a viszonteladói kapcsolat kérését.

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-mail-példa viszonteladói kapcsolat létrehozására":::

4. Önnek, a partnernek csatlakoznia kell a partner bérlőhöz a AdminAgents-csoport objektumazonosító beszerzéséhez.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Az a felhasználó, aki rendelkezik a **tulajdonosi vagy a felhasználói hozzáférés-adminisztrátor** szerepkörrel, és jogosult szerepkör-hozzárendelés létrehozására az előfizetési szinten, a következő műveleteket végzi el:


    1. Csatlakozik ahhoz a bérlőhöz, ahol a CSP-előfizetés létezik.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Csatlakozás az előfizetéshez (csak akkor alkalmazható, ha a felhasználó szerepkör-hozzárendelési engedéllyel rendelkezik több előfizetéshez a bérlőn).
   
         PS CWindowsSystem32> Set-AzContext-SubscriptionID "CSP előfizetés azonosítója" "


    3. Létrehozza a szerepkör-hozzárendelést.
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Ha azt szeretné, hogy az erőforrás-csoport szintjén vagy az erőforrás szintjén adja meg a tulajdonosi szerepkör engedélyt az előfizetés hatóköre helyett, a következő parancsok működhetnek:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Következő lépések

- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)
