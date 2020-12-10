---
title: Rendszergazdai jogosultságok visszaállítása az Azure CSP-hez
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy az ügyfelek hogyan állíthatják vissza a partner rendszergazdai jogosultságait, hogy a partner segítsen kezelni az ügyfelek Azure CSP-előfizetéseit.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 13fdeb01ecd73dc1a63d174a4ad5cb8e1bdc813a
ms.sourcegitcommit: 455894365fa488368f7572ac72312e84a267ef5e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/10/2020
ms.locfileid: "97011502"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Rendszergazdai jogosultságok visszaállítása az ügyfél Azure CSP-előfizetései esetében  

**Alkalmazható szerepkörök**

- Globális rendszergazda
- Felügyeleti ügynök

CSP-partnerként az ügyfelek gyakran elvárják, hogy az Azure-használatot és azok rendszereit is kezelni tudják. Ehhez rendszergazdai jogosultságokkal kell rendelkeznie. Ezeket a jogosultságokat akkor kell megadnia, amikor a viszonteladói kapcsolat létrejött az ügyféllel. Másokat az ügyfél biztosít Önnek.

## <a name="admin-privileges-for-azure-in-csp"></a>Rendszergazdai jogosultságok az Azure-ban a CSP-ben

Az Azure-ban a CSP-ben két rendszergazdai jogosultsági szint van.

**Bérlői szintű rendszergazdai jogosultságok** (**delegált rendszergazdai jogosultságok**) – a CSP-partnerek megkapják ezeket a jogosultságokat a CSP viszonteladói kapcsolat ügyfelekkel való létrehozásakor. Ez lehetővé teszi, hogy a CSP-partnerek hozzáférhessenek az ügyfelek bérlői számára, így olyan rendszergazdai feladatokat végezhetnek, mint például a felhasználók hozzáadása vagy kezelése, a jelszavak alaphelyzetbe állítása és a felhasználói licencek kezelése.

**Előfizetés szintű rendszergazdai jogosultságok** – a CSP-partnerek megkapják ezeket a jogosultságokat az Azure CSP-előfizetések létrehozásakor az ügyfelek számára. Ezek a jogosultságok lehetővé teszik a CSP-partnerek számára az Azure-erőforrások kiépítését és kezelését.

## <a name="reinstate-csp-partners-admin-privileges"></a>A CSP-partnerek rendszergazdai jogosultságának visszaállítása

A delegált rendszergazdai jogosultságok visszaszerzéséhez az ügyfelet kell használnia.

1. Jelentkezzen be a partner Center irányítópultra, és válassza a partner Center menü **ügyfelek** elemét.

2. Válassza ki azt az ügyfelet, aki dolgozik, és **kérjen egy viszonteladói kapcsolatot.** Ez létrehoz egy hivatkozást arra a felhasználóra, aki bérlői rendszergazdai jogosultságokkal rendelkezik.

3. A felhasználónak ki kell választania a hivatkozást, és jóvá kell hagynia a viszonteladói kapcsolat kérését.

   :::image type="content" source="images/azure/revoke4.png" alt-text="viszonteladói kapcsolat":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>A felügyeleti ügynökök csoport hozzáadása az Azure CSP-előfizetés tulajdonosaként

Az ügyfélnek hozzá kell adnia a felügyeleti ügynök csoportját az Azure CSP-előfizetés, egy erőforráscsoport vagy egy erőforrás tulajdonosaként. 

1. A PowerShell-konzol vagy a PowerShell integrált parancsfájlkezelési környezet (ISE) használata. Győződjön meg arról, hogy a AzureAD modulok telepítve vannak.

2. Kapcsolódjon az Azure AD-bérlőhöz.

   ```powershell
   Connect-AzureAD
   ```

3. A felügyeleti ügynökök csoportjai ObjectId beolvasása.

   ```powershell
   Get-AzureADGroup
   ```
   A következő lépéseket az ügyfél azon vállalata végzi, aki tulajdonosi hozzáféréssel rendelkezik az Azure CSP-előfizetéshez.

4. Az Azure CSP-előfizetéshez tulajdonosi hozzáféréssel rendelkező felhasználó hitelesítő adataival bejelentkezik az Azure-ba.

   ```powershell
   Connect-AzureRmAccount
   ```

5. Ezután hozzáadhatja a felügyeleti ügynök csoportját tulajdonosként a CSP Azure-előfizetéshez, az erőforráscsoporthoz vagy az erőforráshoz egy megfelelő erőforrás-URI alkalmazásával a hatókör-paraméterben. 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a>Következő lépések

[Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)
