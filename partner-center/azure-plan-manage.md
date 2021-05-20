---
title: Azure-csomag – Előfizetések és & kezelése
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan használhatnak a partnerek különböző szerepköralapú hozzáférés-vezérlési (RBAC) lehetőségeket az ügyfelek Azure-erőforrásainak üzemeltetési vezérléséhez és felügyeletéhez.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 18cc5c62beaa76f6e3ade79f2f2069e0f2bd3c7e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149604"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Az Azure-csomagban foglalt előfizetések és erőforrások kezelése

**Megfelelő szerepkörök:** Rendszergazdai ügynök


Ez a cikk azt ismerteti, hogy a CSP-partnerek hogyan használhatnak különböző szerepköralapú hozzáférés-vezérlési (RBAC) lehetőségeket az ügyfelek Azure-erőforrásainak üzemeltetési vezérléséhez és felügyeletéhez. Amikor átvált egy ügyfelet az Azure-csomagra, alapértelmezés szerint kiemelt rendszergazdai jogosultságokkal rendelkezik az Azure-ban (előfizetés-tulajdonosi jogosultságok rendszergazdai nevében).

 > [!NOTE]
 > Az Azure-előfizetés rendszergazdai jogosultságát az ügyfél előfizetési, erőforráscsoport- vagy számítási feladatszinten távolíthatja el. 

 A partnerek a szerepköralapú hozzáférés-vezérlési funkció (RBAC) által biztosított különböző lehetőségek használatával a felhőszolgáltatóban kaphatják meg az ügyfelek Azure-erőforrásainak 24 órás operatív vezérlését és felügyeletét. 

- **Rendszergazda nevében (AOBO)** – Az [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)használatával a partnerbérlőben rendszergazdai ügynök szerepkörrel rendelkezik RBAC-tulajdonosi hozzáféréssel a CSP-programon keresztül létrehozott Azure-előfizetésekhez.

- **Azure Lighthouse:** Az AOBO nem teszi lehetővé a különböző ügyfelekkel rendelkező különálló csoportok, illetve a különböző szerepkörök csoportok vagy felhasználók számára való engedélyezésének rugalmasságát. A Azure Lighthouse különböző csoportokat rendelhet hozzá különböző ügyfelekhez vagy szerepkörökhöz. Mivel a felhasználók megfelelő szintű hozzáféréssel fognak hozzáférni az Azure által delegált erőforrás-kezelésen keresztül, csökkentheti a rendszergazdai ügynök szerepkörű (és így teljes AOBO-hozzáféréssel) felhasználóinak számát. Ez hozzájárul a biztonság javításához azáltal, hogy korlátozza az ügyfelek erőforrásaihoz való szükségtelen hozzáférést. Emellett nagyobb rugalmasságot biztosít több ügyfél nagy léptékű kezeléséhez. További információkért olvassa el a [Azure Lighthouse és a Felhőszolgáltató programot.](/azure/lighthouse/concepts/cloud-solution-provider)

- **Címtár- vagy [](/azure/active-directory/develop/app-objects-and-service-principals)vendégfelhasználók vagy** szolgáltatásnév: A CSP-előfizetések részletes hozzáférésének delegálható felhasználók hozzáadásával az ügyfél címtárában, vendégfelhasználók hozzáadásával és meghatározott RBAC-szerepkörök hozzárendelésével.

A Microsoft azt javasolja, hogy a felhasználók biztonsági gyakorlatként a munkájuk elvégzéséhez szükséges minimális engedélyekkel rendelkezniük kell. Lásd: [Azure Active Directory Privileged Identity Management erőforrások.](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="link-your-partner-id-mpn-id-to-your-credentials-for-managing-customers-azure-resources"></a>A partnerazonosító (MPN-azonosító) csatolása az ügyfél Azure-erőforrásainak kezeléséhez használt hitelesítő adataihoz

Az alábbi táblázat a partnerazonosító különböző RBAC-hozzáférési beállításokkal való társításának módszereit mutatja be.

|**Kategória**   |**Forgatókönyv**   |**MPN-azonosító társítása**|
|-----------------|:------------------------|:------------------|
|Aobo   |A KÖZVETLEN CSP-partner vagy közvetett szolgáltató az AOBO használatával hozza létre az előfizetést a közvetlen CSP-partnert vagy közvetett szolgáltatót alapértelmezett tulajdonosként adó ügyfél számára. A KÖZVETLEN CSP-partner vagy közvetett szolgáltató közvetett viszonteladói hozzáférést ad az előfizetéshez az AOBO használatával.|Automatikus (nincs szükség partneri munkára)|
|Azure Lighthouse|A partner létrehoz egy új [felügyelt szolgáltatási ajánlatot a Marketplace-en.](/azure/lighthouse/concepts/managed-services-offers) Ez az ajánlat a CSP-előfizetésben lesz elfogadva, és a partner hozzáférést kap a CSP-előfizetéshez.|Automatikus (nincs szükség partneri munkára)|
|Azure Lighthouse|A partner üzembe helyez [egy ARM-sablont](/azure/lighthouse/how-to/onboard-customer) az Azure-előfizetésben|A partnernek társítania kell az MPN-azonosítót a partnerbérlőben a felhasználóhoz vagy szolgáltatásnévhez. További információ: [Hivatkozás Partnerazonosító.](/azure/billing/billing-partner-admin-link-started)|
|Címtár- vagy vendégfelhasználó|A partner létrehoz egy új felhasználót vagy szolgáltatásnévt az ügyfél címtárában, és hozzáférést biztosít a CSP-előfizetéshez a felhasználónak. A partner létrehoz egy új felhasználót vagy szolgáltatásnévt az ügyfél címtárában. A partner hozzáadja a felhasználót egy csoporthoz, és hozzáférést biztosít a CSP-előfizetéshez a csoporthoz.|A partnernek társítania kell az MPN-azonosítót az ügyfélbérlőben a felhasználóhoz vagy szolgáltatásnévhez. További információ: [Hivatkozás Partnerazonosító.](/azure/billing/billing-partner-admin-link-started)|

## <a name="confirm-that-you-have-admin-access"></a>Győződjön meg arról, hogy rendszergazdai hozzáféréssel rendelkezik

Rendszergazdai hozzáférésre van szüksége az ügyfél szolgáltatásainak kezeléséhez és a megszerzett jóváíráshoz. A [jóváírásokkal kapcsolatos](partner-earned-credit.md) részletes információkért olvassa el a partneri jóváírásokat. Kétféleképpen győződhet meg arról, hogy rendszergazdai hozzáféréssel rendelkezik.

- A napi használati adatokat ismertető fájl áttekintése – Ez az egységár és a tényleges egységár áttekintését a napi használati adatokat ismertető fájlban, valamint annak megerősítésével határozható meg, hogy alkalmaznak-e kedvezményt. Ha Ön megkapja a kedvezményt, Ön a rendszergazda.

- Azure Monitor-riasztás létrehozása – Létrehozhat egy Azure Monitor-tevékenységnapló-riasztást, amely értesítést küld, ha az RBAC-hozzáférést eltávolítják a CSP-előfizetésből. [](/azure/azure-monitor/platform/alerts-activity-log)

### <a name="create-an-azure-monitor-alert"></a>Azure Monitor-riasztás létrehozása

1. Riasztás létrehozása.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="azure-riasztás":::

2. Válassza ki a riasztáshoz kívánt művelettípust. Ha például azt adja meg, hogy e-mailt szeretne kapni, egy e-mailt fog kapni, amely értesíti Önt, ha szerepkör-hozzárendelést törölnek.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="riasztás konfigurálása":::

### <a name="aobo-removal"></a>AOBO-eltávolítás

Az ügyfelek úgy kezelhetik az előfizetéseikhez való hozzáférést, hogy Access Control **a** Azure Portal. A **Szerepkör-hozzárendelések lapon** kiválasztják a **Hozzáférés eltávolítása lehetőséget.** Ilyen esetben a következőt használhatja:

- Beszéljen az ügyféllel, és nézze meg, visszaállítható-e a rendszergazdai hozzáférés.

- Használja a szerepköralapú [hozzáférés-vezérlésen (RBAC) keresztül](/azure/role-based-access-control/overview)biztosított hozzáférést.

- Használja a [Azure Lighthouse.](https://azure.microsoft.com/services/azure-lighthouse/)

A szerepköralapú hozzáférés eltér a rendszergazdai hozzáféréstől. A szerepkörök pontosan azt határják el, hogy mit lehet és mit nem. A rendszergazdai hozzáférés szélesebb körű.

A PEC-jóváírásra jogosult szerepköröket a Partneri jóváírás szerepkörei és engedélyei [dokumentumban láthatja.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)

## <a name="next-steps"></a>Következő lépések

- [Rendszergazdai jogosultságok lemondása és Azure CSP előfizetések esetén](revoke-reinstate-csp.md)

- [Partneri jóváírás – áttekintés](partner-earned-credit.md)

- [Partneri jóváírás felügyelt szolgáltatásokhoz](partner-earned-credit-explanation.md)