---
title: Migrálás a PMC-ből a partneri központba
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan telepítheti át vállalatát a partner Membership Center (PMC) szolgáltatásból a partner Centerbe, beleértve a követendő lépéseket.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 8b6646ff943ff219c41c975d60e66a46d1e0f595
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530535"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Útmutató PMC-ből a Partnerközpontba történő áttelepítéshez

**Megfelelő szerepkörök**

- Globális rendszergazda

A Microsoft partner webhelye a partner.microsoft.com-ben egységes digitális felhasználói élményt nyújt a partnerek számára. A partner webhelyről megismerheti a lehetőségeit, és olyan interaktív tapasztalatokat vehet igénybe, amelyek segítségével a vállalata alkalmazásokat és szolgáltatásokat hozhat létre a Microsofttal. A partner webhelyén elérhető irányítópult-hivatkozás használatával a Microsoft Partner Network tagjai bejelentkezhetnek a partneri központba, ahol kezelheti a kapcsolatot a Microsofttal, regisztrálhat a programokba, és regisztrálhat az ajánlatokra.

Folyamatban van a Partner tagsági központ (PMC) leszerelése. A vállalat meghívást kapott, hogy áttérjen a Microsoft Partner Network tagságának felügyeletéről a partneri központba. Ez az útmutató arra készül, hogy mire számíthat, ahogy a PMC-ról a partneri központba való áttérést végzi.

>[!NOTE]
>Még ha a vállalatnál több fiók vagy hely is van, akkor a partner Centerbe való áttérés egy (az első) fióknak a fiókpartner-központba való áthelyezésével kezdődik.

## <a name="get-started"></a>Bevezetés

Az áthelyezés a PMC-ban kezdődik. A globális rendszergazda meghívót kap az áthelyezés megkezdéséhez.

### <a name="prepare-in-pmc"></a>Felkészülés a PMC-ban

- A vállalat adatainak ellenőrzése
- Elsődleges program kapcsolatának ellenőrzése
- Üzleti helyszínek ellenőrzése
- A jóváhagyott felhasználók frissítése

### <a name="when-youre-ready"></a>Ha elkészült

Válassza az első **lépések** lehetőséget a meghívóban. Ekkor megnyílik a partner központ bejelentkezési lapja.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Első lépések":::

## <a name="start-with-your-work-email"></a>A munkahelyi e-mail-cím megkezdése

Ha a vállalat nem rendelkezik munkahelyi e-mail-címmel és HRE-Bérlővel, akkor a partner központ bejelentkezési folyamata során is segítünk. Ha olyan e-mail-fiókkal próbál bejelentkezni, amely nem munkahelyi e-mail-cím, például személyes fiókja, a rendszer arra irányítja át a vállalat adatait, hogy HRE-bérlőt és munkahelyi e-mail-címet is beállíthat. A rendszer ezeket a vállalati adatokat fogja használni a partner Centerben lévő fiók véglegesítéséhez, ezért ügyeljen arra, hogy pontosak legyenek.

>[!NOTE]
>Ha Ön Kínában található partner, és a Microsoft Partner Network és a Cloud Solution Provider (CSP) programban is regisztrálva lesz, minden egyes fiókhoz külön bérlő fog rendelkezni. A felhőalapú megoldás-szolgáltatói programmal rendelkező fiókját a rendszer felügyeli a nemzeti felhőben, és a Microsoft Partner Network-fiókját a globális felhő kezeli. A két fiók nem csatolható.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Első lépések":::

Miután ellenőrizte vagy frissítette az adatokat, válassza az **elfogadás és folytatás** lehetőséget.
Az oldalon megjelenő feltételek és kikötések **pontosan ugyanazok** , mint a vállalat által a PMC-ban már aláírt szerződés.  
Ez a lépés kezdeményezi az Azure AD-bérlő létrehozását, és biztosítja a munkahelyi fiókot.

Az **elfogadás és folytatás** lehetőséget választva a következő műveleteket is elvégezheti:

- Áttelepíti a fiókját és az összes helyét a partner központba

- Áttelepíti az esetlegesen a PMC-ban vásárolt kompetenciákat vagy térképeket.

- Áttelepíti a PMC-ban található összes marketing-erőforrást, ajánlatot és programot (MAPs, Silver, Gold).

## <a name="invite-employees-to-join-you"></a>Munkatársak meghívása a csatlakozáshoz

Az új Azure AD-bérlő létrehozásakor meghívhatja alkalmazottaikat, hogy jelentkezzenek be a fiókpartner központjába.

:::image type="content" source="images/migration/invite.png" alt-text="Első lépések":::

Ha már bejelentkezett egy meglévő HRE-Bérlővel, az alkalmazottak átkerülnek Önnel. Ebben az esetben rendelje hozzá az alkalmazottak szerepköreit, amelyek meghatározzák, hogy mit tehetnek a partner Centerben. 

>[!NOTE] 
>A partner Center szerepkörei eltérnek a PMC szerepköreitől. További információ: [áttérés a PMC-ról a partneri központba](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Ellenőrizze a tartományt, és legyen globális rendszergazda  

Ha a HRE-bérlő új, a globális rendszergazda szerepkört senki nem rendeli hozzá. Ahhoz, hogy a globális rendszergazda legyen, ellenőriznie kell a tartomány tulajdonjogát. Ehhez szükség lehet a tartományi rendszergazda segítségére.

Habár használhatja a már megvásárolt ajánlatokat, nem vásárolhat új ajánlatokat, amíg el nem végzi a globális rendszergazda hozzárendelésének lépését.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Első lépések":::

Az első lépések lehetőség kiválasztásakor a következő képernyő jelenik meg:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Első lépések":::

A tartományregisztráló már ki lesz töltve Önnek. Csak a tartomány tulajdonosa tudja frissíteni a DNS-fájlt, így a szövegfájlnak a DNS-rekordba való másolásával és hozzáadásával ellenőrizheti, hogy Ön a tulajdonos. A frissítés elvégzése néhány percet is igénybe vehet. Ki kell jelentkeznie a partneri központból, majd újra be kell jelentkeznie. A szerepkör a globális rendszergazda értékre módosult.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Ismerje meg az irányítópultot és a partneri központot

Az irányítópult bemutatójának megtekintése. Itt kezelheti a tagságát, hozzáadhat egy üzleti profilt az átirányítási feltételekhez, regisztrálhat a Cloud Solution Provider programba, és az **irányítópult** kiválasztásával bármikor megtekintheti a vállalata számára releváns értesítéseket és ajánlatokat. Emellett kezelheti az ösztönzőket, megvásárolhatja a piactéren, regisztrálhat a piacra jutási szolgáltatásokra, és így tovább.  

:::image type="content" source="images/migration/fre.png" alt-text="Első lépések":::

## <a name="sign-the-microsoft-partner-agreement"></a>A Microsoft partneri szerződés aláírása

Ha Ön közvetett viszonteladó, akkor a partner Center-fiók beállítása után is hivatalosan regisztrálnia kell a Cloud Solution Provider programban. A tagsági állapot ellenőrzéséhez lépjen a [partner profiljába](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) , és erősítse meg a fiók típusát. Ezután regisztrálja magát a CSP-ben [közvetett viszonteladóként](enrolling-in-the-csp-program.md).

 Miután regisztrálta magát a közvetett viszonteladóként, fogadja el a [CSP-kapcsolat kérését a közvetett szolgáltatónál](indirect-reseller-tasks-in-partner-center.md).

Ezután fogadja el a Microsoft partneri szerződést a partner Center [irányítópultjának](https://partner.microsoft.com/pvc/dashboard) áttekintésében a globális rendszergazdai hitelesítő adatok használatával. Ellenőrizze, hogy aláírta-e a Microsoft partneri szerződést a partner profil program információi szakaszában. Emellett a rendszer megerősítő szalagcím-értesítést is tartalmaz a CSP Áttekintés oldalán. 

## <a name="next-steps"></a>Következő lépések

- [A globális rendszergazda megkeresése](become-global-admin.md)

- [Microsoft-partnerszerződés](microsoft-partner-agreement.md)

- [Felhasználói fiókok létrehozása](create-user-accounts-and-set-permissions.md)

- [Felhasználói szerepkörök és engedélyek hozzárendelése](permissions-overview.md)

- [A tagsági programok kezelése](renew-mpn-offers.md)

- [A vállalat üzleti profiljának létrehozása](create-a-marketing-profile.md)

- [Ügyfelekkel való kapcsolat az átirányítási szolgáltatásokkal](manage-leads.md)

- [Útmutató több vállalat a PMC-ből a partneri központba való áttelepítéséhez](move-multiple-companies.md)
