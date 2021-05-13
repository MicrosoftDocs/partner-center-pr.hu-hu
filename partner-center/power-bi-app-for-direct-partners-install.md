---
title: A Partnerközpont Analytics for Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A cikk lépéseit követve telepítheti és megtekintheti az Partnerközpont adatelemzési alkalmazás a Power BI-hoz (a CSP közvetlen partnerei számára).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 15ee391d6b748b6499700aee321ff4abd85e75d2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854485"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>A Partnerközpont adatelemzési alkalmazás a Microsoft Power BI-hoz telepítése és előzetes verziója


**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | Értékesítési ügynök | Rendszergazdai ügynök

## <a name="before-you-begin"></a>Előkészületek

Válassza ki a vállalat számára legfontosabb alkalmazást az elérhető alkalmazások Power BI listájából:

- [Közvetlen szolgáltató](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Közvetett szolgáltató](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Közvetett viszonteladó](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

A Partnerközpont Analytics alkalmazás előzetes verziójának telepítése előtt győződjön meg arról, hogy megfelel az alábbi követelményeknek.

- Válassza ki a Power BI megfelelő alkalmazást.

- Pro-licenccel Power BI rendelkezik.

- Rendelkezik a sablonalkalmazások bérlőn való telepítéséhez szükséges engedélyekkel.

- Bejelentkezhet a Power BI.

- Bejelentkezhet globális rendszergazdaként, rendszergazdai ügynökként vagy számlázási rendszergazdaként a vállalat Azure Active Directory [(Azure AD) bérlőjébe.](azure-active-directory-tenants-and-partner-center.md)

## <a name="to-install-the-app"></a>Az alkalmazás telepítése

1. Válassza ki a fenti szakaszban megadott alkalmazásforrás-hivatkozást (közvetlen szolgáltató/közvetett szolgáltató/közvetett viszonteladó).

2. Válassza **a GET IT NOW (SZEREZZE BE MOST) lehetőséget.** 

3. A Folytatás lehetőség kiválasztásával elfogadja a feltételeket és **a feltételeket.**

4. A Már van fiókja alatt? válassza **a Bejelentkezés lehetőséget.**

5. A következő lapon adja meg a Power BI felhasználónevét és jelszavát, majd válassza a **Bejelentkezés lehetőséget.**

6. Telepítse a munkaterületet a munkaterület nevének meg megszava.

7. A telepített sablonalkalmazásokat az Alkalmazások szakaszban találja.

8. Válassza **az Alkalmazások lehetőséget,** és válassza ki a telepített alkalmazásokat.

9. Megnyílik az Új alkalmazás első lépések képernyője.

10. Az adatokhoz való csatlakozáshoz válassza a Csatlakozás **lehetőséget.**

11. A **Csatlakozás az Partnerközpont Analyticshez** előugró ablakban  ellenőrizze, hogy a Hitelesítési módszer **beállítása oAuth2,** vagy ha nem, válassza az **oAuth2** lehetőséget a listából. 

> [!NOTE]  
>  Az ablak megjelenése eltarthat néhány percig.

12. A **Partnerközpont Analytics-összekötő** lapon jelentkezzen be a vállalati Azure AD-bérlő globális rendszergazdai, rendszergazdai vagy számlázási rendszergazdai hitelesítő adataival, majd válassza a **Bejelentkezés lehetőséget.**
 
13. Amikor a rendszer hozzáférést kér, válassza az **Elfogadás lehetőséget.** 

Miután az Partnerközpont Analytics szolgáltatás csatlakozott a Power BI, megkezdődik az adatok betöltése. Az adatok mennyiségétől függően ez akár 10 percig is eltarthat. 

Az adatok betöltését követően elkezdheti használni a Partnerközpont Analytics-alkalmazás irányítópultját és jelentéseit a Power BI.

## <a name="next-steps"></a>Következő lépések

[Üzleti adatok megtekintése a Microsoft Partnerközpont Analytics alkalmazással Power BI](power-bi-app-for-direct-partners-use.md)
