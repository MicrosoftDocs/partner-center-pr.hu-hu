---
title: Rendszergazdai jogosultságok újbóli Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan segítheti az ügyfeleket a partner rendszergazdai jogosultságai visszaállításában, hogy a partner segítséget tudjon kérni az ügyfelek Azure CSP kezeléséhez.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 90c8f413398fcb9f65f7fef402a1cdcd092abbc4
ms.sourcegitcommit: 212471150efc8fd2c30023bc6a981a7e052e79ef
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/11/2021
ms.locfileid: "112025955"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Rendszergazdai jogosultságok visszahelyezése egy ügyfél Azure CSP előfizetéséhez  

**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök

CSP-partnerként az ügyfelek gyakran elvárják, hogy Ön kezelje az Azure-használatot és azok rendszereit a számukra. Erre rendszergazdai jogosultsággal kell rendelkezik. Bizonyos jogosultságok akkor kapnak, ha a viszonteladói kapcsolat létrejött az ügyféllel. Az ügyfél másokat is ad Önnek.

## <a name="admin-privileges-for-azure-in-csp"></a>Rendszergazdai jogosultságok a Azure in CSP

A rendszergazdai jogosultságoknak két szintje van a Azure in CSP.

- **Bérlői szintű rendszergazdai jogosultságok (Delegált** rendszergazdai jogosultságok): A CSP-partnerek ezeket a jogosultságokat kapják meg, amikor CSP-viszonteladói kapcsolatot hoznak létre az ügyfelekkel. A delegált rendszergazdai jogosultságok hozzáférést adnak a CSP-partnereknek az ügyfeleik bérlőihez. Ez a hozzáférés lehetővé teszi, hogy olyan rendszergazdai feladatokat is el tudjanak látni, mint a felhasználók hozzáadása/kezelése, a jelszavak visszaállítása és a felhasználói licencek kezelése.
- **Előfizetési szintű rendszergazdai jogosultságok:** A CSP-partnerek ezeket a jogosultságokat a Azure CSP létrehozásakor kapják meg az ügyfeleik számára. Ezen jogosultságok révén a CSP-partnerek teljes hozzáférést számukra az előfizetésekhez, így ők is kiépítik és kezelhetik az Azure-erőforrásokat.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>A CSP-k visszaállításához a partner rendszergazdai jogosultságai

Az ügyfél újra létrehozhatja a CSP szerepkör-hozzárendelést, ha az AdminAgents csoport tagjait adja `object ID` meg az ügyfélnek. A delegált rendszergazdai jogosultságok visszaszerzése érdekében az alábbi lépésekkel együtt kell működnie az ügyféllel.

1. Jelentkezzen be a Partnerközpont irányítópultjára.

2. A Partnerközpont válassza az Ügyfelek **lehetőséget.**

3. Válassza ki azt az ügyfelet, akinél dolgozik, és **igényeljön viszonteladói kapcsolatot.** Ez a művelet létrehoz egy hivatkozást arra az ügyfélre, aki bérlői rendszergazdai jogosultságokkal rendelkezik.

4. Az ügyfélnek ki kell választania a hivatkozást, és jóvá kell hagynia a viszonteladói kapcsolatkérést.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Példa e-mailben viszonteladói kapcsolat létrehozására":::

5. Önnek, a partnernek csatlakoznia kell a partnerbérlőhöz, hogy le tudja szerezni az AdminAgents csoport objektumazonosítóját.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Az ügyfélnek ezután a következő lépéseket kell megtennie a PowerShell vagy az Azure CLI használatával. Az ügyfélnek a következővel kell lennie:

- A tulajdonosi **vagy felhasználói** **hozzáférés rendszergazdájának szerepköre** 
- Szerepkör-hozzárendelések előfizetési szinten való létrehozására vonatkozó engedélyek

   a. Csak PowerShell esetén az ügyfélnek frissítenie kell a `Az.Resources` modult.
   ```powershell
   Update-Module Az.Resources
   ```

   b. Az ügyfél ahhoz a bérlőhöz csatlakozik, ahol a CSP-előfizetés található.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. Az ügyfél csatlakozik az előfizetéshez. Ez csak *akkor érvényes,* ha a felhasználó több előfizetésre vonatkozó szerepkör-hozzárendelési engedélyekkel rendelkezik a bérlőben.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. Az ügyfél ezután létrehozza a szerepkör-hozzárendelést.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

Ahelyett, hogy tulajdonosi engedélyeket ad meg az előfizetés hatókörében, az erőforráscsoport vagy az erőforrás szintjén is adhat. 

- Az erőforráscsoport szintjén

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Az erőforrás szintjén

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Ha a fenti lépések nem működnek, vagy hibaüzenetet kap a kísérlet során, próbálkozzon a következő "catch-all" eljárással az ügyfél rendszergazdai jogosultságának visszaállításához.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Hibaelhárítás

Ha az ügyfél nem tudja végrehajtani a fenti 6. lépést, próbálja ki a következő parancsot:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

További elemzés céljából adja meg az eredményül kapott fájlt `newRoleAssignment.log` a Microsoftnak.

Ha a "catch-all" eljárás sikertelen a (összes művelet) művelet `Import-Module` során, próbálkozzon a következő lépésekkel:
- Ha az importálás meghiúsul, mert a modul használatban van, indítsa újra a PowerShell-munkamenetet az összes ablak bezárásával és újbóli megnyitásával.
- Ellenőrizze a verzióját az `Az.Resources` `Get-Module Az.Resources -ListAvailable` -hez.
- Ha a 4.1.1-es verzió nem szerepel az elérhető listában, a következőt kell használnia: `Update-Module Az.Resources -Force` .
- Ha a hiba azt állítja, hogy egy adott verziónak kell lennie, frissítse a modult is, és cserélje le a et `Az.Accounts` a `Az.Resources` `Az.Accounts` következőre: . Ezután újra kell indítania a PowerShell-munkamenetet.


## <a name="next-steps"></a>Következő lépések

- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)
