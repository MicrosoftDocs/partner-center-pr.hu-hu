---
title: Partnerközpont Insights szerepköralapú hozzáférése
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megismeri az Insights-jelentések Partnerközpont szerepköröket. Ezek közé tartozik a Vezetői jelentésmegjelenítő és a Jelentésmegjelenítő szerepkör.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6af9c7d674d1956332a564628b6b2ea0b1796f6
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120783"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Szerepköralapú hozzáférés-vezérlés a Partnerközpont Insights irányítópulthoz

**Megfelelő szerepkörök**

- Globális rendszergazda
- Rendszergazdai ügynök
- Jelentésmegjelenítő
- Vezetői jelentésmegjelenítő

Az Elemzések irányítópult két új szerepkört használ a Partnerközpont a jelentésekhez való alkalmazotti hozzáférés kezeléséhez : a Vezetői jelentésmegjelenítőt és a Jelentésmegjelenítőt.  A Vezetői jelentésmegjelenítő szerepkörben a felhasználók az összes jelentési adathalmazhoz hozzáférhetnek, míg a Jelentésmegjelenítő szerepkör felhasználói nem férhetnek hozzá olyan bizalmas adatkészlethez, mint a bevétel és az ügyfél/alkalmazott személyes adatai.  

Ahogy a többi Partnerközpont, a globális rendszergazda vagy a fiók rendszergazdája is hozzárendelhet felhasználókat ezekhez a szerepkörökhöz a Felhasználókezelés lapon. A szerepkörök a teljes vállalatra vagy adott MPN-helyre alkalmazhatók. Az adott MPN-hely(ék) számára hozzárendelt szerepkörök korlátozzák, hogy a felhasználó csak a kiválasztott MPN-hely(ekkel) társított jelentésadatokat megtekintsen. A partner az alábbi nézetben kiválaszthat egy vagy több helyet.

:::image type="content" source="images/pci/roles.png" alt-text="A Jelentésmegjelenítő és Partnerközpont jelentésmegjelenítő Insights-szerepkör-beállításainak helyspecifikus adatait jeleníti meg.":::

>[!Note]
> Azok a felhasználók, akik 2020. január 20-án MPN-rendszergazdák, automatikusan hozzáadódnak a vállalati Szintű Vezetői jelentésmegjelenítő szerepkörhöz az adott bérlő összes helyéhez.  Ezek a felhasználók így a globális rendszergazda vagy a fiók-rendszergazda kifejezett beavatkozása nélkül is hozzáférhetnek a jelentésekhez vezetői jelentés megtekintőjeként. A globális rendszergazdák és a fiókgazdák felülbírálhatják ezen felhasználók automatikusan hozzárendelt szerepköreit a képességeik további növelése vagy korlátozása érdekében.

## <a name="next-steps"></a>Következő lépések

- További információ az [Partnerközpont elemzésekről](partner-center-insights.md) és a különböző jelentésekről.
