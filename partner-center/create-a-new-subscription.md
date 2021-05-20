---
title: Ügyfél-előfizetések létrehozása a Partnerközpont
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan értékesítsen előfizetéseket az ügyfeleinek a Microsoft által közzétett termékekre, valamint a külső isv-k által közzétett SaaS-termékekre.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201408"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Ügyfél-előfizetések létrehozása, felfüggesztése vagy lemondása

**A következőkre vonatkozik:** Partnerközpont | Partnerközpont a Microsoft Cloud for US Government

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Globális rendszergazdai | Az | Értékesítési ügynök

Miután létrehozott egy rekordot az ügyfélről a Partnerközpont, előfizetéseket értékesíthet a katalógusban található termékekhez. Ide tartoznak a Microsoft által közzétett termékek és a külső független szoftverszállítók (ISV-k) által a kereskedelmi piactéren közzétett Szolgáltatott szoftver (SaaS) [termékek.](https://azuremarketplace.microsoft.com/marketplace)

Egyes ajánlatok ügyfelenként egy előfizetésre vannak korlátozva. A korlátozott ajánlatok listáját a Díjszabás és ajánlatok Partnerközpont oldalon láthatja.

>[!IMPORTANT]
> A CSP-programban partnerként licencalapú **vagy** forgalmi díjas SaaS-előfizetéseket vásárolhat a csv-közzétevőktől a Partnerközpont.  Ez azt jelenti, hogy bármilyen licencalapú vagy forgalmi díjas  SaaS-ajánlatot [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) megvásárolhat, amelyet az ISV közzétevő tett elérhetővé az Ön számára, beleértve az olyan kizárólagos ajánlatokat is, amelyekhez Hozzáféréssel rendelkezik.  A kereskedelmi piactéren elérhető egyéb ajánlatok (például Azure-alkalmazásokat, tárolókat vagy virtuális gépeket érintő használatalapú ajánlatok) megvásárlásához vagy kezeléséhez meg kell [Azure Portal.](https://portal.azure.com/)

>[!NOTE]
>A dátumok és időpontok Partnerközpont az egyezményes világidő (UTC) szerinti időszava szerint vannak megadva. Ez a helyi időtől legfeljebb 24 óráig térhet el.

## <a name="create-a-new-subscription"></a>Új előfizetés létrehozása

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard).

2. A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.

3. Válassza **az Előfizetés hozzáadása lehetőséget.** Az **Online szolgáltatások lapon** érhetők el az összes elérhető Marketplace SaaS-ajánlat.

4. Ha csak bizonyos típusú előfizetéseket kell látnia, az elérhető szűrők között tegye a következőt:
   - **Közzétevő:** Válassza a **Microsoft** lehetőséget, ha csak a Microsoft ajánlatai vagy a **Partner** ajánlatai közül kíváncsi az ISV-k által közzétett kereskedelmi piactéri termékekre.
   - **Számlázási típus:** Válassza ki a használni kívánt előfizetés-számlázás típusát: **Licenc vagy** **Használat.** A [havi és éves számlázási](license-based-billing.md) gyakoriság közötti döntéshez szükséges információkért tekintse meg a licencalapú számlázást.
   - **Kategória:** **Válassza a Vállalati,** **Kisvállalkozások vagy** Próbaverzió **lehetőséget.** További információ a próbaverziós előfizetésekkel kapcsolatban: Ajánlat az ügyfeleknek [a Microsoft-termékekkel kapcsolatos próbaverziókra.](offer-your-customers-trials-of-microsoft-products.md)

5. Válassza ki az ügyfél számára megvásárolni kívánt termék-előfizetéseket. A látható termékek az ügyfélszegmens típusától (oktatás, kormányzat stb.) és az alkalmazott szűrőktől függenek. Előfordulhat, hogy a Marketplace-en megjelenő egyes ajánlatok nem mindig érhetők el egy adott ügyfél vagy egy adott CSP-partner számára. Ennek oka a következő lehet:

   - Az ügyfél már rendelkezik előfizetéssel az adott termékre, és csak egy engedélyezett

   - Előfordulhat, hogy az ügyfél előfizetése fel lett függesztve (ebben az esetben újraaktiválhatja az előfizetést ahelyett, hogy újat vásárol.

   - IsV SaaS-ajánlatok esetén több oka is lehet annak, hogy az ajánlat nem vásárolható meg: Előfordulhat, hogy az ISV nem támogatja az ügyfél számlázási országát vagy régióját; lehetséges, hogy a szoftverszolgáltató úgy döntött, hogy nem teszi elérhetővé az ajánlatot a CSP-programon keresztül; vagy előfordulhat, hogy a isV kizárólag bizonyos CSP-partnerek számára tette kizárólagosként az ajánlatot. [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) Előfordulhat, hogy az ISV-ajánlat nem kezelhető a Partnerközpont (például tárolókon vagy használatalapú ajánlatokon) keresztül.  

6. Minden hozzáadni kívánt előfizetéshez adja meg a licencek számát (ha szükséges), majd válassza a **Hozzáadás a kosárhoz lehetőséget.**

7. Ha befejezte az előfizetések hozzáadását, válassza a **Megrendelés** áttekintése és áttekintése lehetőséget.

8. Miután áttekintte a rendeléseket, és készen áll az előfizetések megvásárlására, válassza a **Vásárlás lehetőséget.**

9. Miután előfizetést vásárol egy ügyfélnek, a következő történik:

    - Az előfizetés áttekintéséhez vagy szerkesztéséhez válassza ki az előfizetés nevét az ügyfél **Előfizetések oldalán.** Innen kiválaszthatja a bővítménylicenceket, ha vannak elérhetőek, módosíthatja a licencek mennyiségét, vagy felfüggesztheti az előfizetést.

    **ISV SaaS-előfizetések (licencalapú és forgalmi díjas) esetén:**
    - Egy hivatkozást fog kapni az ISV-közzétevő webhelyére. Ez a hivatkozás segíthet az ügyfél előfizetésének üzembe helyezésében vagy a fiók beállításában.
      
    >[!NOTE]
    > Sem Ön, sem az ügyfele nem kap e-mailt az ilyen típusú ISV-előfizetéshez beállított/kiépítési fiók befejezésére vonatkozó utasításokkal.)

    - Ha az előfizetése 30 napos ingyenes próbaverzióval rendelkezik, az ingyenes próbaidőszak automatikusan alkalmazva lesz. A CSP-programban partnerként nem hagyhatja ki az ügyfelek számára vásárolt ajánlatok ingyenes próbaidőszakát. Az ingyenes próbaidőszak végén megkezdődik az előfizetési időszak, és az előfizetés fizetős állapotra vált. Az előfizetés ekkor automatikusan megújul ugyanazon ütemezés szerint.
   
## <a name="update-subscriptions-with-add-ons"></a>Előfizetések frissítése bővítményekkel 

Bővítmény vásárlásához az ügyfélnek először aktív alap-előfizetéssel kell rendelkezik.  A katalóguson keresztül nem vásárolhat bővítményeket.

1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)

2. A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.

3. Válassza ki a kezelni kívánt előfizetést.

4. Az Állapot **szakasz** alatt az előfizetéshez elérhető bővítmények listája látható.  

5. Frissítse az egyes szükséges bővítmények licencmennyiségét. Küldje el a módosításokat a **Küldés** gombbal.

A bővítmények vásárlásának lehetősége Partnerközpont csak közvetlen számlázású és közvetett szolgáltatók számára érhető el.
Csak a jogosult bővítmények jelennek meg az alapkövetelmények és a regionális rendelkezésre állás alapján. A díjszabásról és az ajánlatokról a felhő viszonteladói ajánlat mátrixában található további információ. Az alapszintű előfizetés felfüggesztése a kapcsolódó bővítményeket is felfüggeszti.

A bővítmények kezdő dátuma az alapszintű előfizetéshez igazodik, és a díjakat a díj kezdő dátuma és a díj befejezési dátuma alapján számítjuk ki, az első számlán pedig arányosított díjak szerepelnek. További információ: [Licencalapú számlázás.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Előfizetés felfüggesztése vagy lemondása

A partnerek felfüggeszthetik vagy megszüntethetik az előfizetést, ha az ügyfél ezt kéri, illetve fizetés elmaradása vagy csalás esetén.

### <a name="suspend-a-subscription"></a>Előfizetés felfüggesztése

Ha egy előfizetés állapotát Felfüggesztve állapotra **módosítja,** a felhasználók nem tudnak bejelentkezni vagy hozzáférni a szolgáltatásokhoz.

1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)

2. A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.

3. Válassza ki a kezelni kívánt előfizetést.

4. Az **Állapot** szakaszban válassza a **Felfüggesztve** lehetőséget. Küldje el a módosításokat a **Küldés** gombbal.

5. Az összes adat törlődik, kivéve, ha az előfizetést 90 napon belül újraaktiválják, vagy a fiók megnyitása és az első számlázási időszak (legfeljebb 120 nap) közötti napok számán túl.

Ha felfüggeszt egy előfizetést, a  Felfüggesztve gomb alatt látható dátum jelzi, hogy mikor jár le automatikusan az előfizetés, ha nem aktiválja újra. 

>[!NOTE]
>A CSP-előfizetések nem lejártak (ahogyan a webes előfizetések is), amely alatt a szolgáltatások továbbra is működnek, de az előfizetés nem hoz létre számlázási díjakat. A CSP-előfizetések aktívak vagy fel vannak függesztve (vagy teljesen törölve vannak).

### <a name="cancel-a-subscription"></a>Előfizetés lemondása

A licencalapú SaaS-előfizetéseket a kereskedelmi piactéren található külső isV-közzétevőktől Partnerközpont [le.](csp-commercial-marketplace-overview.md) Ha a lemondási időszakon belül mondja le, teljes visszatérítést kap.

IsV-ajánlatok havi számlázása:

- Ha a rendelést követően kevesebb mint 24 órával lemondja a lemondást, a következő számlán teljes jóváírást fog kapni.

- Ha a rendelést követően 24 óránál később lemond, a lemondás a megújításkor lesz ütemezve.

Az évente számlázható ajánlatokhoz:

- Ha kevesebb mint 14 nappal a rendelés leírása után mondja le, a következő számlán teljes jóváírást fog kapni.

- Ha a lemondást a rendelést követően 14 napnál később mondja le, a lemondás a megújításkor lesz ütemezve.

Miután ezek az időszakok véget érnek, többé nem lesz lehetősége megszüntetni az előfizetést.

> [!NOTE]
> A használatalapú és forgalmi díjas, külső isV-szolgáltatások (amelyek például virtuális gépeket vagy tárolókat használnak) nem jogosultak a visszaküldésre. A használatalapú szolgáltatások kiépítve megszakítási módszerként is fel lehet szabad használni. Mivel a díjakat használat után számlázjuk, ezek a szolgáltatások nem jogosultak visszatérítésre.

Ha törölni szeretne egy licencalapú SaaS-előfizetést egy ISV-kiadóból, tegye a következőket:

1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)

2. A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.

3. Keresse meg a megszüntetni kívánt előfizetést.

4. Az Állapot **oszlopban** válassza a **Mégse lehetőséget.** Küldje el a módosításokat a **Küldés** gombbal.

5. Ha megjelenik egy párbeszédpanel, adja meg a vonatkozó adatokat, majd válassza a **Küldés lehetőséget.**

6. A lemondás megerősítéséhez válassza az **Igen, megszakítás lehetőséget.**

> [!NOTE]
> Dönthet úgy is, hogy API-Azure Marketplace lemondja a Azure Marketplace előfizetést. A műveletet lásd: [Előfizetés lemondása Azure Marketplace.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Annak kiválasztása, hogy a rendszer automatikusan megújítsa-e a kereskedelmi piactéri előfizetést

Alapértelmezés szerint az aktív előfizetések úgy vannak beállítva, hogy az előfizetési időszak lejáratakor automatikusan megújuljanak. A [kereskedelmi piactéri termékekre való előfizetések esetében](csp-commercial-marketplace-overview.md)dönthet úgy, hogy nem újítja meg automatikusan az előfizetést.

Az aktív kereskedelmi piactér-előfizetés automatikus megújításának megállítása:

1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)

2. A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.

3. Válassza az **Előfizetések** lehetőséget. Ez felsorolja az ügyfél számára megvásárolt licencalapú előfizetéseket.

4. Az Előfizetés **oszlopban** válassza ki a módosítani kívánt előfizetést.

5. Az előfizetés részleteit tartalmazó lapon keresse meg az **Állapot szakaszt,** és törölje a jelölést az **Automatikus megújítás jelölőnégyzetből.**

6. Válassza a **Küldés** lehetőséget.

## <a name="next-steps"></a>Következő lépések

- [Kereskedelmi piactéri termékek vásárlása az ügyfelek számára](csp-commercial-marketplace-purchase.md)

- [Kereskedelmi piactéri termékek kezelése az ügyfelek számára](csp-commercial-marketplace-manage.md)

- [Kereskedelmi piactér áttekintése](csp-commercial-marketplace-overview.md)