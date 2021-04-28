---
title: Bérlőazonosító, tartománynév, felhasználói objektumazonosító megkeresása
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan találhat azonosítókat a Azure Portal – a szervezet Azure AD-bérlőazonosítóját, tartománynevét vagy adott felhasználói objektumazonosítóját. Egyes feladatoknak szüksége van erre az információra.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 17b0100bf5e45e931a765a73fb98afddf6dba656
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172251"
---
# <a name="locate-important-ids-for-a-user"></a>Felhasználó fontos azonosítóinak megkeresve

**Megfelelő szerepkörök**

- Globális rendszergazda

Ez a cikk azt ismerteti, hogyan használhatja [Azure Portal](https://portal.azure.com/) segítségével a következő információkat keresheti meg egy felhasználó számára:

- A Microsoft Azure Active Directory szervezet vagy vállalat Microsoft Azure Active Directory (Azure AD) bérlőazonosítója

- Az Azure AD-bérlőhöz társított szervezet vagy vállalat elsődleges tartományneve

- A felhasználói objektum azonosítója

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Keresse meg Microsoft Azure AD bérlőazonosítót és az elsődleges tartománynevet

Az alábbi lépéseket követve keresse meg az Azure AD-bérlőazonosítót vagy az elsődleges tartománynevet a Azure Portal. (Ha programozott módon szeretné megtalálni a bérlőazonosítót, tekintse meg a bérlőazonosító PowerShell vagy parancssori felület használatával [történő keresését.)](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)

> [!NOTE]
> A bérlőazonosító más neveket is nevezhet a különböző alkalmazásokban vagy erőforrásokban. A bérlőazonosítóra hivatkozhat például címtár-azonosítónak, Azure Active Directory-bérlőnek (Azure AD-bérlőnek), Microsoft-azonosítónak, vagy bizonyos jelentéseknek, még a *tenantguid-nek is.*

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).

2. Válassza **Azure Active Directory** lehetőséget a menüből.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Megjeleníti Azure Portal menü Azure Active Directory lehetőség kiválasztását.":::

3. Megjelenik Azure Active Directory **Áttekintés** lap. Az Azure AD-bérlőazonosító vagy az elsődleges  tartománynév kereséséhez keresse meg a Bérlőazonosító mezőt és az **Elsődleges tartomány** mezőt. Ezek a mezők a Bérlő adatai szakaszban jelennek meg.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Az Áttekintés oldalt jeleníti meg két kiemelt mezővel, a bérlőazonosítóval és az elsődleges tartománynévvel.":::

4. A bérlőazonosítót a Azure Portal más módokon is megkeresheti. Válassza **Azure Active Directory** lehetőséget a menüből. Ezután keresse meg a **Kezelés szakaszt** a menüben, és válassza a **Tulajdonságok lehetőséget.**

   A Tulajdonságok lapon a felhasználóhoz társított bérlőazonosító is megjelenik.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Megjeleníti a Tulajdonságok lapot a kiemelt Bérlőazonosító mezővel.":::

## <a name="find-the-user-object-id"></a>A felhasználói objektum azonosítójának megkeresása

Előfordulhat, hogy a tartománynév és a bérlőazonosító megkeresása nem mindig elég. Előfordulhat, hogy meg kell találnia a felhasználóhoz rendelt objektumazonosítót is. Kövesse az alábbi lépéseket, hogy megtalálja a felhasználó objektumazonosítóját a Azure Portal:

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).

2. Válassza **Azure Active Directory** lehetőséget a menüből.

3. Keresse meg **a Kezelés** szakaszt a menüben, majd válassza a **Felhasználók lehetőséget.**

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Megjeleníti Azure Active Directory menüt, kiemelt Felhasználók lehetőséggel.":::

4. A Felhasználók lapon írja be a felhasználó nevét a keresőmezőbe.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Megjeleníti a Felhasználók lapot egy keresőmezővel, amely egy adott felhasználót keres.":::

5. Válassza ki a felhasználó nevét, ahol az megjelenik a listában.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="A Keresett felhasználóhoz egy sort megjelenítő Felhasználó oldalt jelenít meg.":::

6. Keresse meg az Identitás szakaszt a felhasználó Profil lapján. Az Objektumazonosító mező itt jelenik meg a felhasználó egyedi objektumazonosítójával.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Megjeleníti a Felhasználói profil oldalt az Identitás szakaszsal és az objektumazonosító egy kiemelt mezőjével.":::

## <a name="next-steps"></a>Következő lépések

- [A bérlőazonosító programozott módon történő megkeresés a PowerShell vagy a parancssori felület használatával](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [További információ a felhasználói profilokról a Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Ismerje meg, hogyan láthatják vagy exportálják a partnerek az ügyféladatokat a Partnerközpont](see-your-customer-list.md)

