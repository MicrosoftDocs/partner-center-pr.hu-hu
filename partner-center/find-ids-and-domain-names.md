---
title: Bérlőazonosító, tartománynév, felhasználói objektumazonosító megkeresása
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan találhat azonosítókat a Azure Portal a szervezet Azure AD-bérlőazonosítóját, tartománynevét vagy adott felhasználói objektumazonosítóját. Néhány feladatnak szüksége van erre az információra.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150862"
---
# <a name="locate-important-ids-for-a-user"></a>Felhasználó fontos azonosítóinak megkereste

**Megfelelő szerepkörök:** Globális rendszergazda

Ez a cikk bemutatja, hogyan keresheti meg [Azure Portal](https://portal.azure.com/) felhasználóra vonatkozó alábbi információkat a jelen témakörben:

- A Microsoft Azure Active Directory szervezet vagy vállalat Microsoft Azure Active Directory (Azure AD) bérlőazonosítója

- Az Azure AD-bérlőhöz társított szervezet vagy vállalat elsődleges tartományneve

- A felhasználói objektum azonosítója

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Keresse meg Microsoft Azure AD bérlőazonosítóját és elsődleges tartománynevét

Az alábbi lépésekkel keresheti meg az Azure AD-bérlőazonosítót vagy az elsődleges tartománynevet a Azure Portal. (Ha programozott módon szeretné megtalálni a bérlőazonosítót, tekintse meg a bérlőazonosító PowerShell vagy parancssori felület használatával [történő megkeresését.)](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)

> [!NOTE]
> A bérlőazonosító más néven is hívható a különböző alkalmazásokban vagy erőforrásokban. A bérlőazonosítóra hivatkozhat például címtár-azonosítónak, Azure Active Directory-bérlőnek (Azure AD-bérlőnek), Microsoft-azonosítónak, vagy bizonyos jelentéseknek, még a *tenantguid-nak is.*

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).

2. Válassza **Azure Active Directory** lehetőséget a menüből.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Megjeleníti Azure Portal menüben Azure Active Directory lehetőség kiválasztását.":::

3. Megjelenik Azure Active Directory **Áttekintés** lap. Az Azure AD-bérlőazonosító vagy az elsődleges  tartománynév megkereséhez keresse meg a Bérlőazonosító mezőt és az **Elsődleges tartomány** mezőt. Ezek a mezők a Bérlő adatai szakaszban jelennek meg.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Az Áttekintés oldalt jeleníti meg két kiemelt mezővel, a bérlőazonosítóval és az elsődleges tartománynévvel.":::

4. A bérlőazonosítót a Azure Portal más módokon is megkeresheti. Válassza **Azure Active Directory** lehetőséget a menüből. Ezután keresse meg a **Kezelés szakaszt** a menüben, és válassza a **Tulajdonságok lehetőséget.**

   A Tulajdonságok lapon a felhasználóhoz társított bérlőazonosító is megjelenik.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Megjeleníti a Tulajdonságok lapot a kiemelt Bérlőazonosító mezővel.":::

## <a name="find-the-user-object-id"></a>A felhasználói objektum azonosítójának megkeresása

Előfordulhat, hogy a tartománynév és a bérlőazonosító megkeresása nem mindig elég. Előfordulhat, hogy meg kell találnia a felhasználóhoz rendelt adott objektumazonosítót is. Kövesse az alábbi lépéseket, hogy megtalálja a felhasználó objektumazonosítóját a Azure Portal:

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).

2. Válassza **Azure Active Directory** lehetőséget a menüből.

3. Keresse meg **a Kezelés** szakaszt a menüben, majd válassza a **Felhasználók lehetőséget.**

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Megjeleníti Azure Active Directory menüt a Kiemelt Felhasználók lehetőséggel.":::

4. A Felhasználók lapon írja be a felhasználó nevét a keresőmezőbe.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Megjeleníti a Felhasználók lapot egy adott felhasználó keresésére vonatkozó keresőmezővel.":::

5. Válassza ki a felhasználó nevét, ahol az megjelenik a listában.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Megjeleníti a Felhasználó lapot, amely megjelenít egy sort a keresett felhasználó számára.":::

6. Keresse meg az Identitás szakaszt a felhasználó Profil lapján. Itt megjelenik az Objektumazonosító mező a felhasználó egyedi objektumazonosítójával.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Megjeleníti a Felhasználói profil oldalt az Identitás szakaszsal, valamint egy kiemelt mezőt az objektumazonosítóhoz.":::

## <a name="next-steps"></a>Következő lépések

- [A bérlőazonosító programozott módon történő megkeresés a PowerShell vagy a parancssori felület használatával](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [További információ a felhasználói profilokról a Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Ismerje meg, hogyan láthatják vagy exportálják a partnerek az ügyfelek adatait a Partnerközpont](see-your-customer-list.md)

