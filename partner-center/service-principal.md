---
title: Azure AD-szolgáltatásnév
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan adhat hozzá szolgáltatásnévt az Azure AD-bérlőhöz. Ez egy Azure AD-alkalmazás (szolgáltatásnév) hozzáadását jelenti a Partnerközpont.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551554"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Azure AD-alkalmazás (szolgáltatásnév) hozzáadása a Partnerközpont

**Megfelelő szerepkörök:** Globális rendszergazda

A Partnerközpont kereskedelmi piactéri programjában most már hozzáadhat egy Microsoft Azure Active Directory-alkalmazást (Azure AD)-alkalmazást (szolgáltatásnév) az Partnerközpont fiókjában. (Ezt korábban már meg tudta tenni a Cloud Partner Portal (CPP) fiókjában. Most, hogy migrált a Partnerközpont, a CPP-fiók csak olvasható.)
 
>[!Note] 
>A szolgáltatásnév az Azure AD-alkalmazás szinonimája.

## <a name="add-an-azure-ad-application-service-principal"></a>Azure AD-alkalmazás hozzáadása (szolgáltatásnév)

1. A Partnerközpont válassza a **Beállítások,** majd a Fejlesztői **beállítások lehetőséget.**

2. Válassza **a Felhasználók,** majd az **Azure AD-alkalmazások hozzáadása lehetőséget.**

3. Válasszon ki egy meglévő Azure AD-alkalmazást, vagy hozzon létre egy újat.

4. Ha új Azure AD-alkalmazást hoz létre, a következő információkat kell tartalmaznia:  

   - **Válasz URL-cím:** Az AZ URL-cím, ahová a felhasználók bejelentkeznek az Azure AD-alkalmazás használata érdekében.

   - **Alkalmazásazonosító URI:** Az Azure AD-alkalmazás logikai azonosítója, amely akkor lesz bemutatva, amikor egyszeri bejelentkezési kérelmet küld az Azure AD-nek.

   - **Biztonsági szerepkörök:**  A szerepkörkezelő (ugyanaz, mint a CPP tulajdonosi szerepköre) és a fejlesztő **(ugyanaz,** mint a CPP közreműködői szerepköre) a Partnerközpont kereskedelmi piactéri programjában érvényesek, és társíthatóak ehhez az Azure AD-alkalmazáshoz.  

## <a name="next-steps"></a>Következő lépések

- [A kereskedelmi piactér áttekintése a Partnerközpont](csp-commercial-marketplace-overview.md)