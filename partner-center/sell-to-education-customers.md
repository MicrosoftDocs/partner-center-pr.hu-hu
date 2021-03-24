---
title: Ajánlatok eladása az oktatási ügyfeleknek
description: Ismerje meg, hogyan hozhat létre oktatási ügyfelet, és hogyan adhat hozzájuk ajánlatokat a partner Centerben. Magában foglalja az oktatási ügyfél ellenőrzési állapotának megerősítését.
ms.topic: how-to
ms.date: 12/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e0c8812683a038ce1f869cb3cb6750424d49ec05
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028367"
---
# <a name="how-to-sell-offers-to-education-customers-and-how-to-create-an-education-customer-in-partner-center"></a>Ajánlatok értékesítése az oktatási ügyfeleknek és oktatási ügyfelek létrehozása a partner Centerben

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felügyeleti ügynök
- Értékesítési ügynök

## <a name="create-an-education-customer"></a>Oktatási ügyfél létrehozása

Ez a cikk bemutatja, hogyan hozhat létre oktatási ügyfelet a partner Centerben, és hogyan adhat hozzájuk oktatási termékeket. Azt is ismerteti, hogyan tekintheti meg az ellenőrzési állapotot, és szükség esetén küldje el újra az ellenőrzési kérelmet. Az oktatási ajánlatok jelenleg **csak olyan licencelési szolgáltatásokhoz érhetők el** , mint a Microsoft 365, a Dynamics, az Intune stb. Más típusú (szoftver-előfizetések, örökös szoftverek vagy Azure-termékek) esetén nem érhető el.

> [!IMPORTANT]
> A Microsoft ellenőrzi, hogy az újonnan létrehozott oktatási ügyfelek bérlői jogosultak-e az oktatási ajánlatokra.  Ügyeljen arra, hogy a szükséges információkat a lehető legpontosabban és teljes mértékben adja meg az ellenőrzési folyamat késésének elkerülése érdekében.

1. Jelentkezzen be a Partnerközpontba.

2. Válassza az **ügyfelek** lehetőséget, majd kattintson **az ügyfél hozzáadása** lehetőségre. Válassza az **oktatás** lehetőséget a **speciális képesítések** legördülő menüből.  Adja meg a fiók további adatait a szükséges módon.  Az ellenőrzési folyamatot segítő legfontosabb mezők a következők:

   - **Cég neve**: írja be a jogi entitás nevét – az ellenőrzéshez szükséges
   - **Ország/régió és címterület**: írja be a teljes entitás levelezési címe – az ellenőrzéshez szükséges
   - **E-mail cím**: adja meg az entitás tulajdonosának e-mail-címét – nem ingyenes vagy on.microsoft.com e-mailt – az ellenőrzéshez szükséges
   - **Ügyfél elérhetőségi adatai**: ezeket a részleteket az ellenőrzési folyamat részeként fogjuk használni
   - **Elsődleges tartománynév**: az ügyfél fiókjának és e-mail-címeinek létrehozásához használatos.  Válasszon egy, a vállalat nevéhez hasonló nevet a szóközök és a speciális karakterek nélkül.  Ez a név később nem módosítható.

3. Ha elkészült, válassza az **Áttekintés** lehetőséget.

   :::image type="content" source="images/eduaccountinfo.png" alt-text="Oktatási ügyfél fiókja":::

4. A **felülvizsgálat** megerősítése után a rendszer **visszatekintő** állapotot kap, ha a megadott információ érvényes. 

    :::image type="content" source="images/edu/create-review.png" alt-text="Oktatási Customer-fiók a felülvizsgálati oldalon"lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>Az oktatási ügyfél ellenőrzési állapotának megerősítése

Az ügyfél **fiókja** oldalon tekintse meg a **speciális minősítési állapotot**.
Példák az állapotra:

- Ha az ügyfél ellenőrzést kapott: oktatás

   :::image type="content" source="images/edupassedvetting.png" alt-text="Az oktatási ellenőrzés sikeres volt":::

- Ha az ügyfél nem adta át az ellenőrzést: nem oktatási ügyfél

   :::image type="content" source="images/edu/fail-reason.png" alt-text="Az oktatás ellenőrzése nem sikerült" lightbox="images/edu/fail-reason-expanded.png":::

- Ha az ügyfél nem oktatási ügyfélként van megjelölve: nincs

   :::image type="content" source="images/edu/account-one.png" alt-text="az oktatási ügyfél nincs megjelölve" lightbox="images/edu/account-one-expanded.png":::

- Ha az ügyfél oktatási ügyfélként van áttekintve, tekintse át a következőket:

    :::image type="content" source="images/edu/in-review.png" alt-text="az oktatási ügyfél áttekintése" lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>Adja meg az ügyfél fiókjának adatait, és küldje el újra az ellenőrzéshez

Ha az ügyfél a kezdeti ellenőrzést elmulasztja, megadhatja az adatokat, és újból elküldheti azt.

### <a name="correct-the-customer-account-information"></a>Ügyfélfiók adatainak javítása

Az ügyfél adatainak frissítéséhez globális rendszergazdai jogosultságokkal kell rendelkeznie. Frissíti az Office 365-portál adatait, mivel ezek az adatok nem frissíthetők a partner Center portálról.

1. A **fiók** oldalon láthatja, hogy az ügyfél minősítése "nem oktatási ügyfél".

2. Frissítse a böngészőt az oldal alaphelyzetbe állításához. A **frissítés** gomb és a **speciális képzettségi állapot** értéke **none**.

3. Válassza a **Frissítés** lehetőséget. A **Service Management** lapon válassza az **Office 365** lehetőséget.

4. A böngésző új lapján a rendszer átirányítja az Office 365 felügyeleti központba. Előfordulhat, hogy a rendszer kéri, hogy jelentkezzen be a hitelesítő adataival.

5. Válassza a **Beállítások** lehetőséget.

6. A képernyő tetején válassza a **szervezeti profil** fület, majd a **szervezet adatai** elemet. Most már frissítheti az ügyfél adatait.

7. Válassza a **módosítások mentése** elemet az oldalsáv alján.  

### <a name="resubmit-for-verification"></a>Ellenőrzés újraküldése

1. Navigáljon a partner **Center lapra és a Vevőkód lapra** . Frissítse a böngészőt, és ellenőrizze, hogy a vállalat oldal frissítve lett-e az új adatokkal. Kattintson a **frissítés** gombra az oktatási ismételt ellenőrzés kéréséhez.

2. Ha a frissített vásárlói adatok oktatási ajánlatokra jogosultak, a **speciális képesítések** az **oktatásban** is megjelennek. Ha továbbra **sem oktatási felhasználó**, forduljon az ügyfélszolgálathoz a manuális ellenőrzéshez.

## <a name="next-steps"></a>Következő lépések

- [Értékesítés különleges ágazatoknak](get-special-pricing-for-offers.md)

- [Új ügyfél hozzáadása](add-a-new-customer.md)

- [Értékesítési Minecraft: Education Edition-előfizetés az oktatási ügyfeleknek](minecraft-subscriptions.md)
