---
title: Azure AD egyszerű szolgáltatás
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan adhat hozzá egy egyszerű szolgáltatást az Azure AD-bérlőhöz. Ez azt jelenti, hogy hozzáad egy Azure AD-alkalmazást (egyszerű szolgáltatásnév) a partner Centerben.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2020
ms.locfileid: "92528154"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Azure AD-alkalmazás (egyszerű szolgáltatásnév) hozzáadása a partner Centerben

**A következőkre vonatkozik**

- Partnerközpont

**Megfelelő szerepkörök**

- Globális rendszergazda

A partner Center kereskedelmi piactér programjában mostantól hozzáadhat egy Azure AD-alkalmazást (egyszerű szolgáltatásnév) a partner Center-fiókjában. (Korábban már megtehette a Cloud Partner Portalban, vagy a CPP-ben, a fiókban. Most, hogy áttelepítette a partner központba, a CPP-fiók írásvédett.)
 
>[!Note] 
>Az egyszerű szolgáltatásnév az Azure AD-alkalmazás szinonimája.

## <a name="add-an-azure-ad-application-service-principal"></a>Azure AD-alkalmazás hozzáadása (egyszerű szolgáltatásnév)

1. A partner Center irányítópultján válassza a **Beállítások** , majd a **fejlesztői beállítások** elemet.

2. Válassza a **felhasználók** , majd az **Azure ad-alkalmazások hozzáadása** lehetőséget.

3. Válasszon ki egy meglévő Azure AD-alkalmazást, vagy hozzon létre egy újat.

4. Ha új Azure AD-alkalmazást hoz létre, a következő információkat kell tartalmaznia:  

   - **Válasz URL-címe** : az az URL-cím, amelyben a felhasználók bejelentkezhetnek az Azure ad-alkalmazás használatára.

   - **Alkalmazás-azonosító URI** : az Azure ad-alkalmazáshoz tartozó logikai azonosító, amely akkor jelenik meg, amikor egyszeri bejelentkezésre vonatkozó kérést küld az Azure ad-nek.

   - **Biztonsági szerepkörök** : a szerepkörök **kezelője** (ugyanaz, mint a "tulajdonos" szerepkör a CPP-ben) és a **fejlesztő** (ugyanaz, mint a "közreműködői" szerepkör a CPP-ben) a partner Center kereskedelmi piactér programjára vonatkozik, és társítható ehhez az Azure ad-alkalmazáshoz.  

## <a name="next-steps"></a>Következő lépések

- [A partneri központ kereskedelmi piactérének áttekintése](csp-commercial-marketplace-overview.md)