---
title: Munkahelyi fiók összekapcsolása a Partnerközpont
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hozzon létre egy munkahelyi fiókot, amely összeköti a vállalatát Partnerközpont fiókjával. Ez lehetővé teszi, hogy a vállalat alkalmazottai hozzáférjenek Partnerközpont.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: a06a38ef9d96b4c2a1e95328d510eb2fd71ff0e3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149842"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Hozzon létre egy munkahelyi fiókot, amely összeköti a vállalatot Partnerközpont fiókjával

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelő rendszergazda

## <a name="why-you-need-a-work-account"></a>Miért van szüksége munkahelyi fiókra?

A Microsoft megköveteli, hogy a vállalat munkahelyi fiókját az új munkahelyi Partnerközpont hozzá. A hivatkozással a fiók felhasználói bejelentkeznek Partnerközpont munkahelyi fiókjuk felhasználónevével és jelszavával.

## <a name="the-work-account-email-address"></a>A munkahelyi fiók e-mail-címe

Munkahelyi fiókja vagy munkahelyi e-mail-címe a vállalat által megadott e-mail-cím. A munkahelyi fiók e-mail-címe általában formátumban `you@yourcompany.com` van. Az olyan személyes e-mail-címek, mint a Hotmail, a Gmail vagy a Yahoo, nem munkahelyi e-mail-címek, és nem használhatók Partnerközpont fiókjához.

Ha több érvényes e-mail-címmel is dolgozik, használja azt, amely a regionális részleg helyett a vállalati főközponthoz van társítva, például használja az e-mail-címét a `contoso.com` cím `contoso.uk` helyett.

> [!NOTE]  
> Mielőtt úgy dönt, hogy meglévő munkahelyi fiókot használ, gondolja át, hány felhasználónak kell a fiókban dolgoznia a Partnerközpont. Ha vannak olyan felhasználói a fiókban, akiknek nem kell a Partnerközpont-ban dolgoznia, fontolja meg egy új fiók létrehozását csak azok számára, akiknek a Partnerközpont.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nem tudja, hogy a vállalata rendelkezik-e már munkahelyi fiókkal?

Ha nem biztos abban, hogy a vállalata rendelkezik-e munkahelyi fiókkal, kövesse az alábbi lépéseket az ellenőrzéshez. Ha aktív előfizetéssel rendelkezik egy Microsoft Azure Office 365-előfizetéssel, már rendelkezik munkahelyi fiókkal.

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com).

2. Válassza Azure Active Directory a menüből, majd válassza a Tartománynevek lehetőséget.

3. Ha már rendelkezik munkahelyi fiókkal, a tartománynév megjelenik a listában.

Ha a vállalat még nem rendelkezik munkahelyi fiókkal, létrehozhat egyet a regisztrációs folyamat során.

Az alábbi ábra számos tipikus forgatókönyv lépéseit mutatja be:

- állapítsa meg, hogy van-e munkahelyi fiókja
- a munkahelyi fiókba való bejelentkezés mikéntjének meghatározása
- annak meghatározása, hogy létre kell-e hoznia egy új munkahelyi fiókot

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Van munkahelyi fiókja, vagy létre kell hoznia egyet?":::

További információ tartományok hozzáadásáról az Azure AD-ban: Tartomány hozzáadása vagy társítása az [Azure AD-ban.](/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>A Microsoft Azure

Microsoft Azure egy nyilvános felhőplatform, amely segítségével a vállalatok alkalmazásokat építenek ki, helyezhetnek üzembe és kezelnek a Microsoft által felügyelt adatközpontok globális hálózatán. A vállalatok az Azure-ral fizikai gépek helyett virtuális függvényekkel vagy szolgáltatásokkal működő virtuális it-infrastruktúrát építenek ki.

Amikor Azure-előfizetést vásárol, lényegében egy dedikált, biztonságos helyet bérel az Azure nyilvános felhőben, nem olyan különbözik attól, mintha egy irodaépületben bérel egy padlót a vállalat fizikai üzlete számára. Az irodaépület tulajdonosa számára a vállalat bérlő.

Az Azure-beli munkahelyi fiók a vállalat dedikált és elkülönített virtuális reprezentációja az Azure nyilvános felhőben, amely akkor jön létre, amikor előfizet egy Microsoft-felhőszolgáltatásra, például az Azure-ra, az Microsoft Intune-re vagy az Office 365-re.

A munkahelyi fiókjában vannak az Azure AD-felhasználók, valamint a rájuk vonatkozó információk – a jelszavaik, profiladatok, engedélyek stb. A munkahelyi fiók csoportokat, alkalmazásokat és a vállalat biztonságával kapcsolatos egyéb információkat is tartalmaz.

## <a name="next-steps"></a>Következő lépések

- [Partnerközponti fiók kezelése](partner-center-account-setup.md)
- [Ellenőrzési állapot nyomon követése](verification-responses.md)