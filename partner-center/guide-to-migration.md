---
title: Áttelepítés PMC-ről Partnerközpont
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan miképpen miképpen migelheti vállalatát Partner Membership Center (PMC) Partnerközpont, beleértve a szükséges lépéseket is.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 511612042f7da5e43d045d2991fa7d5251612726
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150743"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Útmutató PMC-ből a Partnerközpontba történő áttelepítéshez

**Megfelelő szerepkörök:** Globális rendszergazda

A Microsoft partner webhelye partner.microsoft.com egységes digitális felhasználói élményt nyújt a partnerek számára. A partner webhelyén megismerheti a lehetőségeket, és interaktív élményeket végezhet, amelyek segítenek a vállalatnak az alkalmazások és szolgáltatások Microsofttal való felépítésében és értékesítésében. A partner webhelyén elérhető Irányítópult hivatkozással az Microsoft Partner Network tagjai bejelentkeznek a partnerközpontba, ahol Ön kezeli a Microsofttal való kapcsolatot, programokat regisztrálhat, és feliratkozhat az ajánlatokra.

Partner Membership Center (PMC) leszerelés alatt áll. A vállalatot arra hívták meg, hogy a vállalat Microsoft Partner Network át a Partnerközpont. Ez az útmutató felkészíti a PMC-ről a Partnerközpont.

>[!NOTE]
>Még ha a vállalata több fiókkal vagy helyről is rendelkezik, a Partnerközpont való áthelyezés első lépése egy (az első) fiók áthelyezése a Partnerközpont.

## <a name="get-started"></a>Bevezetés

Az áthelyezés a PMC-ről kezdődik. A globális rendszergazda meghívót kap az áthelyezés megkezdésére.

### <a name="prepare-in-pmc"></a>Előkészítés a PMC-ban

- A céges adatok ellenőrzése
- Az elsődleges program kapcsolattartójának ellenőrzése
- Üzleti helyek ellenőrzése
- Jóváhagyott felhasználók frissítése

### <a name="when-youre-ready"></a>Ha készen áll

Válassza **az Első lépések lehetőséget** a meghívóban. Meg fog jelenni az Partnerközpont bejelentkezési oldalára.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Első lépések":::

## <a name="start-with-your-work-email"></a>Kezdje a munkahelyi e-mail-címmel

Ha a vállalata nem rendelkezik munkahelyi e-mail-címmel és AAD-bérlővel, segíthetünk beállítani egyet a Partnerközpont során. Amikor olyan e-mail-fiókkal próbál bejelentkezni, amely nem munkahelyi e-mail-cím, például a személyes fiókja, a rendszer arra fogja irányítani, hogy adja meg a vállalat adatait, hogy beállítsunk egy AAD-bérlőt és egy munkahelyi e-mailt. Ezeket a vállalati adatokat fogja használni a fiók végleges Partnerközpont, ezért győződjön meg arról, hogy azok pontosak.

>[!NOTE]
>Ha Ön Kínában található partner, és az Microsoft Partner Network és Felhőszolgáltató (CSP) programban is regisztrált, minden fiókhoz külön bérlővel fog rendelkezik. Az Felhőszolgáltató Program programhoz Microsoft Partner Network az Ön fiókja az országos felhőben, a Microsoft Partner Network pedig a globális felhőben. A két fiók nem kapcsolható össze.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Mondja el nekünk a cégét":::

Miután ellenőrizte vagy frissítette az adatokat, válassza az **Elfogadás lehetőséget, és folytassa a következőt:**.
Az oldalon található használati  feltételek pontosan ugyanazok, mint a PMC-be már bejelentkezett szerződés.  
Ez a lépés kezdeményezi az Azure AD-bérlő létrehozását, és biztosítja a munkahelyi fiókot.

Az **Elfogadás és folytatás lehetőség kiválasztása** a következőket is lehetővé teszi:

- A fiók és az összes hely migrálta az Partnerközpont

- Áttelepíti a PMC-ban vásárolt kompetenciákat vagy MAP-ket

- Áttelepíti a PMC-hez rendelkezésre álló marketinges erőforrásokat, ajánlatokat és programokat (MAPs, Silver, Gold)

## <a name="invite-employees-to-join-you"></a>Alkalmazottak meghívása, hogy csatlakozzanak Önhez

Az új Azure AD-bérlő létrehozásakor meghívhatja az alkalmazottakat, hogy jelentkezzenek be Partnerközpont.

:::image type="content" source="images/migration/invite.png" alt-text="Alkalmazottak meghívása":::

Ha egy meglévő AAD-bérlővel jelentkezett be, az alkalmazottakat áthelyezték. Ebben az esetben rendelje hozzá az alkalmazottak szerepköreit, hogy felügyelni tudják, milyen feladatokat Partnerközpont. 

>[!NOTE] 
>A szerepkörök Partnerközpont különböznek a PMC szerepköreitől. További információ: [Áthelyezés PMC-ről Partnerközpont.](move-pmc-pc-map.md)

## <a name="verify-your-domain-and-become-a-global-admin"></a>Ellenőrizze a tartományt, és legyen globális rendszergazda  

Ha az AAD-bérlője új, senki sem kap globális rendszergazdai szerepkört. Ahhoz, hogy ön legyen a globális rendszergazda, ellenőriznie kell a tartomány tulajdonjogát. Előfordulhat, hogy ehhez a tartományi rendszergazdára van szüksége.

Bár használhatja a már megvásárolt ajánlatokat, addig nem vásárolhat új ajánlatokat, amíg el nem fogja tudni látni a globális rendszergazda hozzárendelésének lépését.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Irányítás vezérlése":::

Az első lépések kiválasztásakor a következő képernyő jelenik meg:

:::image type="content" source="images/migration/verifytxt.png" alt-text="A tartomány tulajdonjogának igazolása":::

A tartományregisztráló már ki lesz töltve. Csak a tartomány tulajdonosa frissítheti a DNS-fájlt, így a szövegfájlnak a DNS-rekordba való másolásával és hozzáadásával ellenőrizheti, hogy Ön-e a tulajdonos. A frissítés eltarthat néhány percig. Ki kell jelentkeznie a Partnerközpont majd újra be kell jelentkeznie. A szerepköre globális rendszergazdai szerepkörre módosul.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Ismerkedjen meg az irányítópult és a Partnerközpont

Az irányítópult bemutatója. Itt kezelheti a tagságot, hozzáadhat üzleti profilt a hivatkozásokhoz, regisztrálhat a Felhőszolgáltató-programban, és bármikor láthatja a vállalkozására vonatkozó értesítéseket és ajánlatokat az Irányítópult lehetőség **kiválasztásával.** Emellett ösztönzőket is kezelhet, a piactéren vásárolhat, regisztrálhat a piacra lépő szolgáltatásokra, és egyéb szolgáltatásokat is regisztrálhat.  

:::image type="content" source="images/migration/fre.png" alt-text="Bemutató":::

## <a name="sign-the-microsoft-partner-agreement"></a>A Microsoft Partnerszerződés

Ha Ön közvetett viszonteladó, a saját Partnerközpont beállítása után is hivatalosan regisztrálnia kell a Felhőszolgáltató programba. A tagság állapotának ellenőrzéshez a Jogi profilban [erősítse](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) meg a fiók típusát. Ezután regisztráljon a CSP-be [közvetett viszonteladóként.](enrolling-in-the-csp-program.md)

 Miután regisztrált közvetett viszonteladóként, fogadja el a közvetett szolgáltatóval való [CSP-kapcsolatkérést.](indirect-reseller-tasks-in-partner-center.md)

Ezután fogadja el Microsoft Partnerszerződés irányítópult áttekintésének Partnerközpont [a](https://partner.microsoft.com/pvc/dashboard) globális rendszergazdai hitelesítő adatok használatával. Győződjön meg arról, hogy Microsoft Partnerszerződés partnerprofil Program info szakaszában. A CSP áttekintési oldalán egy megerősítő szalagcím-értesítés is megjelenik. 

## <a name="next-steps"></a>Következő lépések

- [Keresse meg a globális rendszergazdát](become-global-admin.md)

- [Microsoft-partnerszerződés](microsoft-partner-agreement.md)

- [Felhasználói fiókok létrehozása](create-user-accounts-and-set-permissions.md)

- [Felhasználói szerepkörök és engedélyek hozzárendelése](permissions-overview.md)

- [Tagsági programok kezelése](renew-mpn-offers.md)

- [A vállalat üzleti profiljának létrehozása](create-a-marketing-profile.md)

- [Kapcsolat az ügyfelekkel hivatkozásokon keresztül](manage-leads.md)

- [Útmutató több vállalat PMC-ről Partnerközpont](move-multiple-companies.md)
