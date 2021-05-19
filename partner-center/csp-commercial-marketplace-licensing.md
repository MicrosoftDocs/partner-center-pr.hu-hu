---
title: Licencelés kezelése a Marketplace-ajánlatokban
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan állíthatja be és kezelheti az ISV kereskedelmi piactéri ajánlatok licencelését.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147955"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Licencelés kezelése a Marketplace-ajánlatokban

**Megfelelő szerepkörök:** Globális rendszergazdai | Fiók rendszergazdája

Ez a cikk végigvezeti egy ajánlat Partnerközpont- és Microsoft AppSource- és licenckezelésének folyamatán.  

>[!IMPORTANT]
>A cikkben lévő képességek jelenleg nyilvános előzetes verzióban állnak rendelkezésre.

## <a name="before-you-begin"></a>Előkészületek

### <a name="commercial-marketplace-basics"></a>A kereskedelmi piactér alapjai

A folyamat megkezdése előtt ismerkedjen meg a kereskedelmi piactér alapjaival. Az alábbi táblázatban található cikkek segítenek az első lépésekben. 

| Témakör  | Cikk  |
|-------|--------|
|Kereskedelmi piactéri csomagok | [A kereskedelmi piactéri ajánlatok csomagja és díjszabása](/azure/marketplace/plans-pricing)    |
|Kereskedelmi piactéri ajánlatok  | [Termékoldal-típusok](/azure/marketplace/determine-your-listing-type)    |
|Kereskedelmi piactéri fiókok |  [Kereskedelmi piactéri fiók létrehozása a Partnerközpont](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Az ajánlatazonosító meghatározása

Az alábbi eljárásokban meg kell adnia egy ajánlatazonosítót. Most egy kis idő alatt meg kell szereznie egy megfelelő ajánlatazonosítót, és vegye figyelembe a következő pontokat:

- Ez az azonosító látható az ügyfelek számára a Marketplace-ajánlat webcímén, és Azure Resource Manager sablonokat, ha van ilyen.
- Az ajánlatazonosítónak és a közzétevő azonosítójának 40 karakternél nem hosszabbnak kell lennie.
- Csak kisbetűket és számokat használjon. Az ajánlatazonosító tartalmazhat kötőjeleket és aláhúzásjeleket, szóközök nélkül. Ha például a közzétevő azonosítója , és beírja a címet, az ajánlat `testpublisherid` `test-offer-1` webcíme `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` lesz.
- Ez az azonosító a Létrehozás lehetőséget választva nem **módosítható.**

### <a name="determine-your-offer-alias"></a>Az ajánlat aliasának meghatározása

Az Offer alias az ajánlathoz használt név a Partnerközpont. Szüksége lesz egy megfelelő Offer aliasra is, amely az alábbi irányelveket követi:

- Ez a név nem használatos a piactéren, és eltér az ajánlat nevétől és az ügyfelek számára megjelenő egyéb értékektől.
- Ez a név a Létrehozás kiválasztása után már nem módosítható.

## <a name="create-your-offer"></a>Az ajánlat létrehozása

A licencelési folyamat első lépése a kereskedelmi piactéri ajánlat létrehozása. 

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).
2. A bal oldali navigációs menüben válassza a **Kereskedelmi piactér/Áttekintés lehetőséget.**
3. Az Áttekintés oldal tetején válassza az Új ajánlat lehetőséget, majd a **Dynamics 365 for Customer Engagement & PowerApps lehetőséget.**
4. Adja meg a korábban létrehozott **ajánlatazonosítót** és ajánlat aliast. 
5. Válassza **a Létrehozás** lehetőséget az ajánlat létrehozásához és a folytatáshoz.
6. Válassza ki a licencelési beállításokat.

    - Ha engedélyezni szeretné az ajánlat licenckezelését, válassza az **Alkalmazáslicenc-kezelés engedélyezése a Microsofton keresztül** lehetőséget. Ez egy egyszeres beállítás, és nem módosíthatja az ajánlat közzététele után.

    - Azt is engedélyezheti, hogy az ügyfelek licenc nélkül futtatják az alkalmazás alapfunkcióit, és prémium szintű funkciókat futtassanak a licenc vásárlása után. Ehhez jelölje be Az alkalmazás telepítésének engedélyezése az ügyfelek számára akkor is, ha nincs **licenc hozzárendelve jelölőnégyzetet.**

    - Ha nem szeretné, hogy az ajánlatában engedélyezve legyen a licenckezelés, válassza a **Get it now (Free) (Szerezze be az ingyenes)** lehetőséget, az **Ingyenes** próbaverziót, vagy a Contact **me (Kapcsolatfelvétel) lehetőséget.**

## <a name="create-your-plan"></a>Csomag létrehozása

Ezekben a lépésekben meghatározhatja az ajánlathoz engedélyezni kívánt tervet vagy csomagokat.

1. A bal oldali navigációs menüben válassza a **Csomag áttekintése,** majd az **Új csomag létrehozása lehetőséget.**
2. Adja meg a **csomagazonosítót** és a **csomag nevét,** majd válassza a **Létrehozás lehetőséget.**
3. A **Csomaglista lapon** adja meg a csomag **leírását.**
4. A leírás mentéshez és a későbbi befejezéshez válassza a **Piszkozat mentése lehetőséget.**

5. Ha elkészült, válassza az Áttekintés **és közzététel lehetőséget.** A csomaginformációk most már megjelennek a appsource.microsoft.com ajánlatlistában (csomagok szakaszban) jelennek meg.

6. Miután létrehozta az ajánlat összes csomagját, ki kell másolnia az egyes csomagok szolgáltatásazonosítóját. Válassza **a Plan overview (Csomag** áttekintése) lehetőséget a Plan listing (Csomaglista) lap tetején. Másolja az egyes tervek szolgáltatásazonosítóját egy biztonságos helyre.

## <a name="add-service-ids-to-your-solution"></a>Szolgáltatás-idok hozzáadása a megoldáshoz

A következő lépés a megoldás frissítése úgy, hogy hozzáadja a szolgáltatás-értékeket minden másolt csomaghoz. Ezzel kapcsolatos útmutatásért lásd: [AppSource-csomag létrehozása a megoldáshoz.](/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>A csomag feltöltése és az ajánlat közzététele

1. A bal oldali navigációs panelen válassza a **Kereskedelmi piactér** lehetőséget, majd a **Technikai konfiguráció lehetőséget.**
2. Az **Alaplicenc-modell alatt válassza** a Felhasználó **lehetőséget.**
3. A **CRM-csomag alatt** adja meg a csomag helyének URL-címét.
4. A bal oldali navigációs panel többi lapjával adja meg az egyéb szükséges adatokat. Ha végzett, válassza az Áttekintés **és közzététel lehetőséget.**

Az ajánlat közzététele után áttekintjük és ellenőrizzük az adatait. Ha bármilyen probléma van a folyamattal, értesítjük Önt. Ha minden probléma megoldódott, értesítést kap arról, hogy az ajánlata elérhető az AppSource-ban. Ezen a ponton élő adásra lehet képes.

## <a name="make-your-offer-live-in-partner-center"></a>Az ajánlat élő adásban Partnerközpont

Az alábbi eljárás végigvezeti az ajánlat AppSource-ban való élő készítésének folyamatán. A folyamattal kapcsolatos további információkért lásd: [Bevezetés a termékoldali lehetőségekbe.](/azure/marketplace/determine-your-listing-type)

>[!NOTE]
>Az ajánlat közzététele után az élő adás 4–6 órát fog igénybe venni.

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).
2. A bal oldali navigációs menüben válassza a **Kereskedelmi piactér/Áttekintés lehetőséget.**
3. Az Áttekintés **lapon** keresse meg a keresett ajánlatot. A közzétételre kész ajánlatok előzetes verziójúak **lesznek.** Válassza ki az ajánlatot.
4. Az Ajánlat **áttekintése lapon** válassza az Élő **adásba lehetőséget.**
Az ajánlat 4-6 óra múlva lesz élő.
5. Az ajánlatoldalt az AppSource-on az Ajánlat áttekintő oldalának alján található **AppSource** hivatkozásra **kattintva láthatja.**

    - **Licenccel rendelkező ajánlatok** esetén: Ha az ajánlatához licencellenőrzés szükséges, a felhasználók csak a Kapcsolatfelvétel elemre kattintva léphetnek be az érdeklődőbe, hogy kommunikáljanak velük.

    - **Ingyenes telepítési lehetőséggel** rendelkező licenccel rendelkező ajánlatok esetén: Ha az ajánlathoz nincs szükség licencellenőrzésre, **a** rendszergazdai felhasználók a Kapcsolatfelvétel lehetőség mellett egy Azonnali lekért gombot is **láthatnak.** Azok a felhasználók, akik ki szeretnék próbálni az ingyenes telepítési lehetőséget, a **Get It Now**(Szerezze be most) gombra kattintva telepítik az ajánlatot a felügyeleti Power Platform központban. A felhasználók továbbra is használhatjak a **Kapcsolatfelvétel a velem** kapcsolatot, ha kérdéseik vannak, vagy ha fizetős csomagra szeretnék frissíteni.

## <a name="register-isv-connect-deal-in-deal-registration"></a>ISV Connect-ajánlat regisztrálása az ajánlatregisztrációban

Mielőtt licenceket rendelhet egy ügyfélhez, minden értékesítést regisztrálni kell a Partnerközpont. Ehhez lásd: [Az ügylet regisztrálása.](register-deals.md)

## <a name="invite-the-customer"></a>Az ügyfél meghívása

Az alábbi eljárással hívatja meg az ügyfelet az ajánlatban való részvételre.  

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).
2. A bal oldali navigációs menüben válassza a **Kereskedelmi piactér/Áttekintés lehetőséget.**
3. A bal oldali navigációs menüben válassza a **Hivatkozások,** majd az **Ajánlatregisztráció lehetőséget.**
4. Szűrjön **az Elküldött ügyletekre,** válassza a **Folyamatban lapot,** majd válassza ki a kívánt ügyletet.
5. Az ajánlat áttekintő oldalán válassza a **Licencek kezelése lehetőséget.**
6. A **Licencek kezelése ablakban** válassza ki az ügyfelet az Ügyfél **adatai** legördülő listából. Ha az ügyfélkapcsolat még nem létezik, válassza a +Új ügyfél **meghívása a jóváhagyáshoz lehetőséget.**
7. Másolja ki a megjelenő hivatkozást.
8. Küldje el e-mailben ezt a hivatkozást az ügyfél számlázási rendszergazdája vagy globális rendszergazdája számára, és használja ezt a hivatkozást a admin.microsoft.com eléréséhez és az Ön által létesítetet kapcsolat elfogadásához és elfogadásához.

    >[!NOTE]
    >A kapcsolat addig nem lesz létrejön, amíg az ügyfél el nem végzi ezt a lépést.

## <a name="activate-manage-and-remove-your-licenses"></a>Licencek aktiválása, kezelése és eltávolítása

Miután az ügyfél engedélyezte a kapcsolatot, elkezdheti csomagokat hozzáadni az ajánlatból, és licenceket rendelni az egyes csomagokhoz.

1. Az ajánlat Licencek kezelése ablakában válassza a **+Csomag hozzáadása lehetőséget.**
2. Töltse ki **a Csomag ehhez a megoldáshoz és** a **Licencek száma** mezőket, majd válassza a **Licencek frissítése lehetőséget.** A licencek a következő admin.microsoft.com az ügyfelek kezelhetik és rendelhetik hozzá az alkalmazottakhoz.

    - Egy meglévő csomag licencszámának módosításához írja be az új számot a **Licencek** száma mezőbe, majd válassza a **Licencek frissítése lehetőséget.**

    - Egy üzlet licencének inaktiválásához vagy eltávolításához válassza a Kuka ikont a **Műveletek** mezőben, majd válassza a **Licencek frissítése lehetőséget.**

## <a name="next-steps"></a>Következő lépések

[Licencelési erőforrások](support-resources-licensing.md)