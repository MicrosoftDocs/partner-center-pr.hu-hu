---
title: Bérlő AZONOSÍTÓjának, tartománynevének, felhasználói objektum AZONOSÍTÓjának megkeresése
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan kereshet azonosítókat a Azure Portalban – egy szervezet Azure AD-bérlői AZONOSÍTÓjának, tartománynevének vagy adott felhasználói objektumának AZONOSÍTÓját. Néhány feladatnak szüksége van ezekre az adatokra.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: cb0325aae30fe57a4be2be3e37bca1ee6aa1eab8
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439232"
---
# <a name="locate-important-ids-for-a-user"></a>Felhasználók fontos azonosítóinak megkeresése

Ez a cikk azt ismerteti, hogyan használható a [Azure Portal](https://portal.azure.com/) az alábbi információk megkereséséhez a felhasználó számára:

- A felhasználó szervezetének vagy vállalatának Microsoft Azure Active Directory (Azure AD) bérlői azonosítója

- Az Azure AD-bérlőhöz társított szervezet vagy vállalat elsődleges tartományneve

- A felhasználói objektum azonosítója

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>A Microsoft Azure AD bérlő AZONOSÍTÓjának és elsődleges tartománynevének megkeresése

Az alábbi lépéseket követve megkeresheti az Azure AD-bérlő AZONOSÍTÓját vagy elsődleges tartománynevét a Azure Portalon belül. (Ha a bérlői azonosítót programozottan szeretné megtalálni, tekintse meg a [bérlői azonosító keresése a PowerShell vagy a CLI használatával](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)című témakört.)

> [!NOTE]
> A bérlői azonosító neve eltérő lehet különböző alkalmazásokban vagy erőforrásokban. Előfordulhat például, hogy a bérlő azonosítója a címtár-azonosító, a Azure Active Directory (Azure AD) bérlő, a Microsoft-azonosító, vagy bizonyos jelentések esetében még a *tenantguid* is hivatkozik.

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).

2. A menüből válassza a **Azure Active Directory** lehetőséget.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Megjeleníti Azure Portal a menüből válassza a Azure Active Directory lehetőséget.":::

3. Megjelenik egy Azure Active Directory **áttekintő** oldal. Az Azure AD-bérlő AZONOSÍTÓjának vagy elsődleges tartománynevének megkereséséhez keresse meg a **bérlői azonosító** mezőt és az **elsődleges tartomány** mezőt. Ezek a mezők a bérlői adatok szakaszban jelennek meg.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="A két Kiemelt mezőt, a bérlői azonosítót és az elsődleges tartománynevet tartalmazó áttekintő oldalt jeleníti meg.":::

4. A bérlői azonosítót többféleképpen is megtalálhatja a Azure Portal. A menüből válassza a **Azure Active Directory** lehetőséget. Ezután keresse meg a **kezelés** szakaszt a menüben, majd válassza a **Tulajdonságok** lehetőséget.

   A Tulajdonságok lap a felhasználó társított bérlői AZONOSÍTÓját is megjeleníti.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Megjeleníti a tulajdonságok lapot a Kiemelt bérlői azonosító mezővel.":::

## <a name="find-the-user-object-id"></a>A felhasználói objektum AZONOSÍTÓjának megkeresése

Ha csak a tartománynevet és a bérlő AZONOSÍTÓját találja, nem mindig lehet elég. Előfordulhat, hogy meg kell keresnie egy felhasználóhoz rendelt objektumazonosító-azonosítót is. Az alábbi lépéseket követve megkeresheti a felhasználó objektumazonosítót a Azure Portalban:

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).

2. A menüből válassza a **Azure Active Directory** lehetőséget.

3. Keresse meg a **kezelés** szakaszt a menüben, majd válassza a **felhasználók** lehetőséget.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Megjeleníti Azure Active Directory menüt a Kiemelt felhasználók lehetőséggel.":::

4. A felhasználók lapon írja be a felhasználó nevét a keresőmezőbe.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Megjeleníti a felhasználók lap keresési mezőjét egy adott felhasználó kereséséhez.":::

5. Válassza ki a felhasználó nevét, ahol megjelenik a listában.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Megjeleníti a felhasználó oldalát, amely a keresett felhasználó sorát jeleníti meg.":::

6. Keresse meg az identitás szakaszt a felhasználó profilja oldalon. Az objektumazonosító mező itt jelenik meg a felhasználó egyedi objektumazonosító-azonosítójával.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Megjeleníti a felhasználói profil oldalt az identitás szakaszban, valamint egy kiemelt mezőt az objektumazonosító számára.":::

## <a name="next-steps"></a>További lépések

- [A bérlői azonosító megkeresése programozott módon a PowerShell vagy a parancssori felület használatával](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [További információ a Azure Active Directory felhasználói profiljairól](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Megtudhatja, hogyan láthatják vagy exportálják a partnereink a partneri központban lévő vásárlói adatokat](see-your-customer-list.md)

