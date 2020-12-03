---
title: Az Azure Cost Management by Cloudyn CSP-k számára
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan regisztrálhat a Cloudyn-webalkalmazást, és hogyan használhat titkos kulcsot a partner Centerben, így az alkalmazással nyomon követheti az ügyfelek Azure-használati adatait és költségeit.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534989"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>A Customer Azure-beli használat és költségek nyomon követése a CSP-partnerek Azure Cost Management alkalmazásával  

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felügyeleti ügynök

[További információ a Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Előkészületek
A Azure Cost Management használata előtt győződjön meg arról, hogy megfelel a következő követelményeknek:

- Ön egy partner a Cloud Solution Provider programban.
- Lehetőség van a partner Center API-webalkalmazás létrehozására.

## <a name="overview"></a>Áttekintés

A Cloudyn egy webalkalmazás, amellyel nyomon követheti és kezelheti az Azure-t és a használat költségeit. A partner Center API-n keresztül használja.

## <a name="register-your-web-app-in-the-partner-center"></a>Webalkalmazás regisztrálása a partner Centerben
Ha Azure Active Directory webalkalmazást regisztrál a partner Centerben, engedélyezze a hozzáférést a partner Center API-hoz. 
1.  Jelentkezzen be a [partner Centerbe](https://partnercenter.microsoft.com/pcv/dashboard/overview) [globális rendszergazdai vagy rendszergazdai ügynök fiók](create-user-accounts-and-set-permissions.md)használatával.
2.  A **partner Center** lapon válassza a **Fiókbeállítások** &gt; **[alkalmazás-kezelés](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** lehetőséget.
3.  A **webalkalmazás** szakaszban kattintson az **Add New Web App (új webalkalmazás hozzáadása**) elemre.
<br> **Megjegyzés**: Ha korábban létrehozott egy webalkalmazást, kihagyhatja a 3. lépést.
4.  Másolja és mentse a **kereskedelmi azonosító** GUID azonosítóját és az **alkalmazás azonosítójának** GUID azonosítóját a webalkalmazáshoz. Az Azure Cost Management alkalmazás 30 napos ingyenes próbaverziójának használatához mindkét azonosítóra szüksége lesz.

## <a name="add-a-secret-key-to-your-app"></a>Titkos kulcs hozzáadása az alkalmazáshoz
1. A **Kulcs hozzáadása** gomb melletti legördülő listából válassza ki az 1 vagy 2 év időtartamát.
2. Kattintson a **Kulcs hozzáadása** lehetőségre. 
3. Másolja ki és mentse a titkos kulcs értékét. Erre szüksége lesz a 30 napos ingyenes próbaidőszakra.<br>
   > [!NOTE]  
   > Az alkalmazás titkos kulcsa a több lejárati dátummal rendelkező jelszavakhoz hasonló. Mentse a kulcs értékét egy biztonságos helyre későbbi használatra.

## <a name="next-steps"></a>További lépések
Kezdjen el egy [30 napos ingyenes próbaverziót](https://go.microsoft.com/fwlink/?linkid=857895).
A próbaverzió elindításához a következő adatokat kell megadnia:
- A partner Center bejelentkezési hitelesítő adatai
- Kereskedelmi azonosító GUID
- Alkalmazás azonosítója GUID
- Alkalmazás titkos kulcsának értéke
