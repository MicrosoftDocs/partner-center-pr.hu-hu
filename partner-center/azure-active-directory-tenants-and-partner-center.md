---
title: Munkahelyi fiók összekapcsolása a partner Center eléréséhez
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Hozzon létre egy munkahelyi fiókot, amely összeköti a vállalatot a partner Center-fiókjával. Ez lehetővé teszi a vállalat alkalmazottai számára a partneri központ elérését.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: 2cc30c3681f0310f738ed937c15e0142b20cdc4c
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528495"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Munkahelyi fiók létrehozása, amely összeköti a vállalatot a partner Center-fiókkal

**A következőkre vonatkozik**

- Partnerközpont

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói felügyeleti rendszergazda

## <a name="why-you-need-a-work-account"></a>Miért van szüksége munkahelyi fiókra

A Microsoft megköveteli, hogy a vállalati munkahelyi fiókot az új partner Center-fiókhoz kapcsolja. A hivatkozás lehetővé teszi, hogy a fiók felhasználói bejelentkezzenek a partner központba a munkahelyi fiók felhasználónevével és jelszavával.

## <a name="the-work-account-email-address"></a>A munkahelyi fiók e-mail-címe

Munkahelyi fiókja vagy munkahelyi e-mail-címe a vállalata által megadott e-mail-cím. A munkahelyi fiókhoz tartozó e-mailek formátuma általában `you@yourcompany.com` . A személyes e-mail-címek, például a Hotmail, a Gmail vagy a Yahoo nem működnek e-mailben, és nem használhatók a partner Center-fiókhoz.

Ha egynél több érvényes munkahelyi e-mail-címmel rendelkezik, használja a céges központhoz társított, nem pedig a regionális részleget, hanem a `contoso.com` cím helyett használja az e-mail-címét `contoso.uk` .

> [!NOTE]  
> Mielőtt meglévő munkahelyi fiókot szeretne használni, gondolja át, hogy a fiók hány felhasználójának kell működnie a partner Centerben. Ha olyan fiókkal rendelkező felhasználókkal rendelkezik, akiknek nem kell a partner Centerben dolgoznia, érdemes lehet új fiókot létrehozni csak azokhoz a felhasználókhoz, akiknek a partner Centerben kell működniük.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nem biztos abban, hogy a vállalata már rendelkezik munkahelyi fiókkal?

Ha nem biztos abban, hogy munkahelyi fiókja van-e, kövesse az alábbi lépéseket az ellenőrzéshez. Ha Microsoft Azure vagy Office 365-es aktív előfizetéssel rendelkezik, már van munkahelyi fiókja.

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com).

2. Válassza a menü Azure Active Directory elemét, majd válassza a tartománynevek lehetőséget.

3. Ha már rendelkezik munkahelyi fiókkal, a rendszer a tartománynevet fogja listázni.

Ha a vállalat még nem rendelkezik munkahelyi fiókkal, létrehozhat egyet a beléptetési folyamat során.

Az alábbi ábra számos jellemző forgatókönyvhöz biztosít lépéseket:

- annak megállapítása, hogy van-e munkahelyi fiókja
- a munkahelyi fiókba való bejelentkezés módjának meghatározása
- annak megállapítása, hogy létre kell-e hoznia egy új munkahelyi fiókot

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Van munkahelyi fiókja, vagy létre kell hoznia egyet?":::

További információ tartományok hozzáadásáról az Azure AD-ben: [tartomány hozzáadása vagy hozzárendelése az Azure ad](/azure/active-directory/active-directory-add-domain) -ben

## <a name="about-microsoft-azure"></a>Tudnivalók Microsoft Azure

A Microsoft Azure egy nyilvános felhőalapú platform, amellyel a vállalatok a Microsoft által felügyelt adatközpontok globális hálózatán hozhatnak létre, helyezhetnek üzembe és kezelhetnek alkalmazásokat. A vállalatok az Azure-t használják virtuális informatikai infrastruktúra létrehozásához virtuális funkciókkal vagy szolgáltatásokkal fizikai gépek helyett.

Ha Azure-előfizetést vásárol, lényegében egy dedikált, biztonságos területet bérel az Azure nyilvános felhőben, nem egészen más, mint a vállalat fizikai üzleti tevékenységének elsajátításához. Az irodaház tulajdonosának a vállalata bérlő.

Az Azure-beli munkahelyi fiók a vállalat dedikált és elszigetelt virtuális ábrázolása az Azure nyilvános felhőben, amely akkor jön létre, amikor előfizet egy Microsoft Cloud Service-re (például Azure, Microsoft Intune vagy Office 365).

Munkahelyi fiókja az Azure AD-felhasználókat és a rájuk vonatkozó információkat – a jelszavukat, a profil adatait, az engedélyeket stb. – tárolja. A munkahelyi fiók a vállalatra és annak biztonságára vonatkozó csoportokat, alkalmazásokat és egyéb információkat is tartalmaz.