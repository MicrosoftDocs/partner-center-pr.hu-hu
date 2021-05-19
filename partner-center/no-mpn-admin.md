---
title: Mi a legjobb, ha az MPN-program egyetlen rendszergazdája távozott a vállalattól?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan találhat új MPN-rendszergazdát, vagy hogyan találhat segítséget a vállalat globális rendszergazdája. Emellett megtudhatja, hogyan adhat hozzá új Partnerközpont globális rendszergazdához.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5efd157078acd72ca47418aaa9559a678fc5b129
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151168"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Mi a legjobb, ha az MPN-program egyetlen rendszergazdája távozott a vállalattól?

**Megfelelő szerepkörök:** MPN-partner | Fiók-rendszergazdai | Globális rendszergazda

A következő cikk három tipikus forgatókönyvet is végigvezet arra vonatkozóan, hogy mi a helyzet, ha az MPN-rendszergazda elhagyta a vállalatot.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>1. forgatókönyv: Az MPN-partner/fiók adminisztrátora elhagyta a vállalatot, de a fiókban továbbra is vannak globális rendszergazdák

Ebben az esetben a vállalat egy másik személye is hozzárendelhető MPN-partneri rendszergazdai szerepkörhöz. Adott MPN-partner-rendszergazdai/fiók-rendszergazdai szerepkör szerepkör hozzárendelése:

1. Jelentkezzen be Partnerközpont fiókjába a munkahelyi fiókjával tom@contoso.com (például: ).
1. A **Felhasználókezelés lapon** szűrje a Globális rendszergazda szűrőt, hogy lássa, kik a vállalat globális rendszergazdái. 
1. Lépjen kapcsolatba az egyik globális rendszergazdával, és kérje meg, hogy rendelje hozzá a szükséges MPN-specifikus szerepkört. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>2. forgatókönyv: Az MPN-partner/fiók adminisztrátora elhagyta a vállalatot, és a fiókban nincsenek globális rendszergazdák 

Ha a Felhasználókezelés oldalra lép, és szűr a globális rendszergazdai szűrésre, de azt találja, hogy a vállalatában nincs olyan globális rendszergazda, aki segíthetne az MPN-specifikus szerepkör elnyerésében, kövesse az alábbi lépéseket: 

1. A [portal.azure.com,](https://ms.portal.azure.com/)jelentkezzen be a munkahelyi fiókjával tom@contoso.com (például: ). 
1. Válassza a **Súgó és támogatás** lehetőséget a bal oldali menü navigációs sávjában.
1. A következő oldalon válassza az **Új**  Support request és a Technikai probléma típusa lehetőséget a legördülő menüben, szúrja be a további részleteket, majd kattintson a **Tovább: Megoldások elemre.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Keresse meg a rendszergazdai Azure Portal":::

4. Miután a következő oldalon áttekinti az ajánlott megoldásokat, válassza a **Tovább: Részletek** lehetőséget, és töltse ki a szükséges mezőket.
1. Tekintse át és hozza létre a támogatási kérést.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>3. forgatókönyv: Az MPN-partner rendszergazdája/fiók rendszergazdája/globális rendszergazda elhagyta a vállalatot, és nincsenek más felhasználók, akik hozzáférhetnek a vállalat Azure AD-hez. Ez a hozzáférés teljes elvesztése.

A [rendszergazdai feladatátvétel lépéseit](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) követve vegye át a nem Azure Active Directory címtárat.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nem tudja, hogy a vállalata rendelkezik-e már munkahelyi fiókkal?

Ha nem biztos abban, hogy a vállalata rendelkezik-e munkahelyi fiókkal, kövesse az alábbi lépéseket az ellenőrzéshez.

1. Jelentkezzen be az [Azure felügyeleti portálra.](https://ms.portal.azure.com)
2. Válassza **Azure Active Directory** bal oldali menüben a Tartománynevek, majd a **Tartománynevek lehetőséget.**
Ha már rendelkezik munkahelyi fiókkal, a tartománynév megjelenik a listában.

>[!Note]
>Ha aktív előfizetéssel rendelkezik a Microsoft Azure vagy az Office 365 szolgáltatásra, már rendelkezik munkahelyi fiókkal, és a bejelentkezési hitelesítő adatoknak meg kell egyednek lennie az ezen szolgáltatások eléréséhez használt hitelesítő adatokkal.