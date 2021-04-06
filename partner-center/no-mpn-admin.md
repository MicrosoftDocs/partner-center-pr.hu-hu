---
title: Mi a teendő, ha az MPN-program egyetlen rendszergazdája elhagyta a vállalatot?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, mi a teendő, ha új MPN-rendszergazdát keres, vagy segítséget szeretne kapni a vállalat globális rendszergazdájától. Azt is megtudhatja, hogyan adhat hozzá új partner Center globális rendszergazdát.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3702ebd5a9421036a053a9a142a2f40d3e488137
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441999"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Mi a teendő, ha az MPN-program egyetlen rendszergazdája elhagyta a vállalatot?

**Megfelelő szerepkörök**

- MPN-partner rendszergazdája
- Fiókadminisztrátor
- Globális rendszergazda

A következő cikk bemutatja, hogy mi a teendő, ha az MPN rendszergazdája elhagyta a vállalatot.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>1. forgatókönyv: az MPN-partner rendszergazdája/fiók rendszergazdája elhagyta a vállalatot, de a fiókban még mindig vannak globális rendszergazdák

Ebben az esetben a vállalat egy másik személye is hozzárendelheti az MPN partner-rendszergazda szerepkört. Adott MPN-partner rendszergazda/fiók rendszergazdai szerepkör szerepkörének hozzárendeléséhez:

1. Jelentkezzen be a partner Center-fiókjába a munkahelyi fiókjával (például: tom@contoso.com ).
1. A globális rendszergazda **felhasználó-felügyeleti** oldalának szűrésével megtekintheti, hogy kik a vállalat globális rendszergazdái. 
1. Lépjen kapcsolatba az egyik globális rendszergazdával, és kérje meg őket, hogy rendelje hozzá a szükséges MPN-specifikus szerepkört. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>2. forgatókönyv: az MPN-partner rendszergazdája/fiók rendszergazdája elhagyta a vállalatot, és nincsenek globális rendszergazdák a fiókban. 

Ha a **felhasználó-felügyeleti** lapra lép, és a globális rendszergazda szűrője, de úgy találja, hogy nincs olyan globális rendszergazda a cégnél, aki segítségére lehet az MPN-specifikus szerepkör megszerzésében, kövesse az alábbi lépéseket:

1. Lépjen a [Portal.Azure.com](https://ms.portal.azure.com/), és jelentkezzen be a munkahelyi fiókjával (például: tom@contoso.com ). 
1. Kattintson a **Súgó + támogatás** lehetőségre a bal oldali menüben a navigációs sávon.
1. A következő lapon válassza a legördülő menü **új support Request** és **technikai probléma** típusa elemét, szúrja be a további részleteket, és kattintson a **Tovább gombra: megoldások.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Rendszergazda keresése a Azure Portalban":::

4. Miután megtekintette a javasolt megoldásokat a következő lapon, válassza a **Next (tovább) gombot: részletek** és a szükséges mezők elvégzése.
1. Tekintse át és hozza létre a támogatási kérelmet.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>3. forgatókönyv: MPN-partner rendszergazdája/fiók rendszergazdája/globális rendszergazda elhagyta a vállalatot, és nincsenek más felhasználók, akik hozzáférhetnek a vállalat Azure AD-hez. Ez a hozzáférés teljes elvesztése.

A felügyelet nélküli címtár Azure Active Directory-rendszergazdaként való átvételéhez kövesse a [rendszergazda általi átvétel](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) lépéseit.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nem biztos abban, hogy a vállalata már rendelkezik munkahelyi fiókkal?

Ha nem biztos abban, hogy munkahelyi fiókja van-e, kövesse az alábbi lépéseket az ellenőrzéshez.

1. Jelentkezzen be az [Azure felügyeleti portálra](https://ms.portal.azure.com).
2. A bal oldali menüben válassza a **Azure Active Directory** lehetőséget, majd válassza a **tartománynevek** lehetőséget.
Ha már rendelkezik munkahelyi fiókkal, a rendszer a tartománynevet fogja listázni.

>[!Note]
>Ha rendelkezik aktív előfizetéssel Microsoft Azure vagy Office 365-re, akkor már rendelkezik munkahelyi fiókkal, és a bejelentkezési hitelesítő adatainak meg kell egyezniük a szolgáltatások eléréséhez használt adatokkal.