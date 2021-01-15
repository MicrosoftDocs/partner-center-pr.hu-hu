---
title: A Power BI a partner Center Analytics telepítése
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A cikk lépéseit követve telepítse és tekintse meg a partner Center Analytics alkalmazást a Power BIhoz (közvetlen partnerek számára a CSP-ben).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 754b3310918df9b38129cf1374ae3731d9d8062e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215849"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>A Partnerközpont adatelemzési alkalmazás a Microsoft Power BI-hoz telepítése és előzetes verziója


**Megfelelő szerepkörök**
-   Globális rendszergazda
-   Felhasználói rendszergazda
-   Értékesítési ügynök
-   Felügyeleti ügynök

## <a name="before-you-begin"></a>Előkészületek

Válassza ki a vállalata számára leginkább megfelelő alkalmazást az elérhető Power BI alkalmazások alábbi listájából:
- [Közvetlen szolgáltató](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Közvetett szolgáltató](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Közvetett viszonteladó](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

A partner Center Analytics-alkalmazás előzetes verziójának telepítése előtt győződjön meg arról, hogy megfelel az alábbi követelményeknek.

- Kiválaszthatja a vállalata számára megfelelő Power BI alkalmazást.

- Power BI Pro-licenccel rendelkezik.

- Rendelkezik a sablon alkalmazásainak a bérlőre való telepítéséhez szükséges engedélyekkel.

- Bejelentkezhet Power BIba.

- A [vállalat Azure Active Directory (Azure ad) bérlője](azure-active-directory-tenants-and-partner-center.md)globális rendszergazdaként, rendszergazdai ügynökként vagy számlázási rendszergazdaként is bejelentkezhet.

## <a name="to-install-the-app"></a>Az alkalmazás telepítése

1. Kattintson az adott alkalmazás forrás hivatkozására (közvetlen szolgáltató/közvetett szolgáltató/közvetett viszonteladó) a fenti szakaszban.

2. Kattintson a **Letöltés most** lehetőségre. 

3. A **Folytatás** gombra kattintva fogadja el a feltételeket és a kikötéseket.

4. Már van fiókja? válassza **a bejelentkezés** lehetőséget.

5. A következő lapon adja meg Power BI felhasználónevét és jelszavát, majd válassza a bejelentkezés lehetőséget.

6. A munkaterület nevének megadásával telepítse a munkaterületet.

7. Megtalálhatja az alkalmazások szakaszban telepített sablonok alkalmazásait.

8. Kattintson az alkalmazások elemre, és válassza ki a telepített alkalmazásokat.

9. Megnyílik az új alkalmazás képernyője.

10. Az adatkapcsolathoz kattintson a **Kapcsolódás** gombra.

11. A **Kapcsolódás a partneri központ Analytics** előugró ablakhoz lapon ellenőrizze, hogy a **hitelesítési módszer** a **oAuth2** értékre van-e állítva, vagy válassza a **oAuth2** lehetőséget a listából, ha nem. 

> [!NOTE]  
>  Ez az ablak néhány percig is eltarthat.

12. A **partner Center Analytics-összekötő** lapon jelentkezzen be a vállalati Azure ad-bérlőhöz a globális rendszergazda, a rendszergazdai ügynök vagy a számlázási rendszergazdai hitelesítő adatokkal, majd válassza a **Bejelentkezés** lehetőséget.
 
13. Amikor a rendszer kéri a hozzáférést, válassza az **elfogadás** lehetőséget. 

Miután a partner Center Analytics szolgáltatás csatlakozott a Power BIhoz, a rendszer betölti az adatgyűjtést. Az adatmennyiségtől függően ez akár 10 percet is igénybe vehet. 

Az adatbetöltések befejezése után elkezdheti a partner Center Analytics alkalmazás irányítópultjának és jelentéseinek használatát Power BI.

## <a name="next-steps"></a>Következő lépések

[Üzleti adatai megtekinthetők a Microsoft Power BI partner Center Analytics alkalmazásával](power-bi-app-for-direct-partners-use.md)
