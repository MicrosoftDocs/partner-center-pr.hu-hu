---
title: Azure-csomag – előfizetések kezelése & erőforrásokkal
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy a partnerek hogyan használhatják a különböző szerepköralapú hozzáférés-vezérlési (RBAC) lehetőségeket az ügyfelek Azure-erőforrásainak operatív vezérléséhez és kezeléséhez.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 4bbeb417fdc5964d66f754a789873c1dbc8b1d25
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92530048"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Az Azure-csomagban foglalt előfizetések és erőforrások kezelése

Amikor átvált egy ügyfelet az Azure-csomagra, a jogosultsági szintű rendszergazdai jogosultságokat az Azure-ban rendeli hozzá (az előfizetés tulajdonosi jogosultságai a rendszergazda nevében) alapértelmezés szerint.

 > [!NOTE]
 > Az ügyfél az Azure-előfizetéshez tartozó rendszergazdai jogosultságokat az előfizetés, az erőforráscsoport vagy a munkaterhelés szintjén távolíthatja el. 

 A partnerek a szerepköralapú hozzáférés-vezérlési funkció (RBAC) által biztosított különböző beállítások használatával nonstop az ügyfél Azure-erőforrásainak működési irányítását és felügyeletét a CSP-ben. 

- **Rendszergazda a (z) (Aobo) nevében** – az [Aobo](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)szolgáltatásban a partner bérlőn lévő rendszergazdai ügynök szerepkörrel rendelkező felhasználók a CSP program keretében létrehozott Azure-előfizetésekhez RBAC tulajdonosi hozzáféréssel.

- Az **Azure Lighthouse** : a AOBO nem teszi lehetővé a rugalmasságot olyan különálló csoportok létrehozására, amelyek különböző ügyfelekkel működnek, vagy különböző szerepköröket engedélyeznek a csoportoknak vagy a felhasználóknak. Az Azure Lighthouse használatával különböző csoportokat rendelhet hozzá különböző ügyfelekhez vagy szerepkörökhöz. Mivel a felhasználók a megfelelő szintű hozzáféréssel rendelkeznek az Azure-beli delegált erőforrás-kezelésen keresztül, csökkentheti a rendszergazdai ügynök szerepkörrel rendelkező felhasználók számát (és így teljes AOBO-hozzáféréssel rendelkezik). Ez segít a biztonság javításában azáltal, hogy korlátozza az ügyfelek erőforrásainak szükségtelen hozzáférését. Emellett nagyobb rugalmasságot biztosít több ügyfél felügyeletéhez. További információért olvassa el [Az Azure Lighthouse és a Cloud Solution Provider programot](/azure/lighthouse/concepts/cloud-solution-provider).

-  **Címtár vagy vendég felhasználók vagy [egyszerű szolgáltatások](/azure/active-directory/develop/app-objects-and-service-principals)** : a CSP-előfizetésekre vonatkozó részletes hozzáférést delegálhat, ha felhasználókat ad hozzá az ügyfél-címtárban, illetve vendég felhasználókat ad hozzá, és hozzárendel egy adott RBAC-szerepkört.

A Microsoft azt javasolja, hogy a felhasználóknak olyan minimális engedélyekkel rendelkezzenek, amelyekre szükségük van a munkájuk biztonsági gyakorlatként való elvégzéséhez. Lásd: [Azure Active Directory Privileged Identity Management erőforrások](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>A partner-azonosító (MPN-azonosító) összekapcsolása a hitelesítő adatokkal az ügyfél Azure-erőforrásainak kezeléséhez

A következő táblázat a partner-azonosító különböző RBAC-hozzáférési lehetőségekkel való hozzárendeléséhez használt módszereket mutatja be.

|**Kategória**   |**Forgatókönyv**   |**MPN-azonosító társítása**|
|-----------------|:------------------------|:------------------|
|AOBO   |A CSP Direct partner vagy közvetett szolgáltató létrehoz egy előfizetést az ügyfél számára, amely a CSP közvetlen partnere vagy a közvetett szolgáltató alapértelmezett tulajdonosa az előfizetéshez az AOBO használatával.; A CSP közvetlen partnere vagy közvetett szolgáltatója közvetett viszonteladói hozzáférést biztosít az előfizetéshez a AOBO használatával.|Automatikus (nincs szükség partneri munkára)|
|Azure Lighthouse|A partner létrehoz egy új [, felügyelt szolgáltatási ajánlatot a piactéren](/azure/lighthouse/concepts/managed-services-offers). Ezt az ajánlatot a CSP-előfizetés fogadja el, és a partner hozzáférést kap a CSP-előfizetéshez.|Automatikus (nincs szükség partneri munkára)|
|Azure Lighthouse|Partner üzembe helyezése [ARM-sablon](/azure/lighthouse/how-to/onboard-customer) az Azure-előfizetésben|A partnernek hozzá kell rendelnie az MPN-azonosítót a felhasználóhoz vagy az egyszerű szolgáltatáshoz a partner bérlőn. További információ: [kapcsolati partner azonosítója](/azure/billing/billing-partner-admin-link-started).|
|Címtár vagy vendég felhasználó|A partner létrehoz egy új felhasználót vagy szolgáltatásnevet az ügyfél címtárában, és hozzáférést biztosít a felhasználó számára a CSP-előfizetéshez. A partner új felhasználót vagy szolgáltatásnevet hoz létre az ügyfél címtárában. A partner hozzáadja a felhasználót egy csoporthoz, és hozzáférést biztosít a CSP-előfizetéshez a csoport számára.|A partnernek az MPN-azonosítót hozzá kell rendelnie a felhasználóhoz vagy az egyszerű szolgáltatáshoz az ügyfél bérlője számára. További információ: [kapcsolati partner azonosítója](/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Ellenőrizze, hogy rendelkezik-e rendszergazdai hozzáféréssel

Rendszergazdai hozzáféréssel kell rendelkeznie az ügyfél szolgáltatásainak kezeléséhez és a szerzett kreditek fogadásához. A keresett kreditekkel kapcsolatos részletes információkért olvassa el a [partner által szerzett krediteket](partner-earned-credit.md) . Kétféleképpen lehet meggyőződni arról, hogy rendszergazdai hozzáférése van.

- Tekintse át a napi használati fájlt – ez az egységár és a tényleges egység árának áttekintésével határozható meg a napi használati fájlban, és megerősíti, hogy van-e kedvezmény alkalmazva. Ha a kedvezményt kapja, Ön a rendszergazda.

- Azure monitor-riasztás létrehozása – létrehozhat egy Azure Monitor műveletnapló [riasztást](/azure/azure-monitor/platform/alerts-activity-log) arról, hogy értesítést kapjon, ha a RBAC hozzáférése el lett távolítva a CSP-előfizetésből.

### <a name="create-an-azure-monitor-alert"></a>Azure monitor-riasztás létrehozása

1. Riasztás létrehozása.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="Azure-riasztás":::

2. Válassza ki, hogy milyen típusú műveletet szeretne végrehajtani a riasztásban. Ha például azt szeretné, hogy egy e-mailt küldjön, a rendszer értesítést küld arról, hogy a szerepkör-hozzárendelés törlése megtörténik-e.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="Azure-riasztás":::

### <a name="aobo-removal"></a>AOBO eltávolítása

Az ügyfelek az előfizetésekhez való hozzáférést a Azure Portal **Access Control** is kezelhetik. A **szerepkör-hozzárendelések** lapon válassza a **hozzáférés eltávolítása** lehetőséget. Ha ez történik, a következőket teheti:

- Beszéljen az ügyféllel, és ellenőrizze, hogy a rendszergazdai hozzáférés visszaállítható-e.

- Használja a [szerepköralapú hozzáférés-vezérlés (RBAC)](/azure/role-based-access-control/overview)által biztosított hozzáférést.

- Az [Azure világítótoronyon](https://azure.microsoft.com/services/azure-lighthouse/)keresztül biztosított hozzáférés használata.

A szerepköralapú hozzáférés különbözik a rendszergazdai hozzáféréstől. A szerepkörök leszűkítik pontosan, hogy mit tehet és mit nem. A rendszergazdai hozzáférés szélesebb körű.

Ha meg szeretné tekinteni a PEC-t kereső szerepköröket, olvassa el [a partner által létrehozott kreditek szerepköreit és engedélyeit](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).

## <a name="next-steps"></a>Következő lépések

- [Az Azure CSP-előfizetések rendszergazdai jogosultságának visszavonása és visszaállítja](revoke-reinstate-csp.md)

- [Partner által létrehozott kredit – áttekintés](partner-earned-credit.md)

- [Partner által létrehozott kredit a felügyelt szolgáltatásokhoz](partner-earned-credit-explanation.md)