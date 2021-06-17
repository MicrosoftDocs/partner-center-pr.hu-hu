---
title: Annak ellenőrzése, hogy az ügyfél elfogadta-e Microsoft Ügyfélszerződés CSP-programhoz
description: Felhőszolgáltató (CSP) partnereknek meg kell erősítenie az ügyfél általi Microsoft Ügyfélszerződés, mielőtt Microsoft-szolgáltatások az ügyfeleknek.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277011"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Annak ellenőrzése, hogy az ügyfél elfogadta-e Microsoft Ügyfélszerződés CSP-programhoz

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Értékesítési ügynök


Az ügyfelek két lehetőség közül választhatnak, hogy hogyan fogadják el a Microsoft Ügyfélszerződés.

**1. lehetőség:** Az ügyfél-elfogadás partneri igazolása – A partner az API/SDK használatával Partnerközpont ügyfél-elfogadást Partnerközpont meg.

**2. lehetőség:** Az ügyfél közvetlen elfogadása – A partner meghívhatja az ügyfelet egy URL-címen keresztül, hogy áttekintse és elfogadja a Microsoft 365 Felügyeleti központban.

## <a name="access-microsoft-customer-agreement-template"></a>Hozzáférés Microsoft Ügyfélszerződés sablonhoz

A sablon legújabb verzióját manuálisan letöltheti innen Microsoft Ügyfélszerződés [sablont.](https://aka.ms/customeragreement) A Microsoft Ügyfélszerződés országspecifikus. A sablon Microsoft Ügyfélszerződés mindenképpen a megfelelő országot válassza ki az ügyfél helye alapján.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>1. lehetőség: Az ügyfél elfogadásának megerősítése a Partnerközpont

A közvetlen számlázási partnerek megerősíthetik, hogy az ügyfelek elfogadják Microsoft Ügyfélszerződés-Partnerközpont új és meglévő ügyfelek számára. A közvetett viszonteladók nem igazolhatóak az ügyfeleik nevében, és a közvetett szolgáltatójukkal kell dolgozniuk az igazolás elvégzéséhez.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Az ügyfelek új ügyfelek általi elfogadásának megerősítése

Amikor új ügyfélbérlőt hoz létre a Partnerközpont, a következő lépésekkel erősítse meg, hogy az ügyfél elfogadta a Microsoft Ügyfélszerződés. A lépések végrehajtásához rendszergazdai vagy értékesítési ügynöknek kell lennie.

1. Válassza **az Ügyfelek,** majd az **Új ügyfél lehetőséget.**

2. A **Fiókadatok alatt** adja meg a vállalat és az elsődleges kapcsolattartó adatait.

3. A **Microsoft-szerződés** alatt jelölje be a jelölőnégyzetet annak ellenőrzésére, hogy az ügyfél elfogadta-e a Microsoft Ügyfélszerződés.

4. A **Szerződés elfogadásának dátuma alatt** adja meg a megfelelő dátumot. Ezt nem állíthatja be jövőbeli dátumra.

5. Győződjön meg arról, hogy az elsődleges felhasználó megjelenített kapcsolattartási adatai helyesek. Ha helytelen, válassza a **Frissítés** lehetőséget, és adja meg a szerződést elfogadó személy pontos adatait.

6. Az **ügyfélbérlő** létrehozásának folytatásához válassza a Tovább lehetőséget.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Új ügyfél.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Az ügyfelek meglévő ügyfelek általi elfogadásának megerősítése

Ehhez rendszergazdai vagy értékesítési ügynöknek kell lennie:

1. Válassza az **Ügyfelek** lehetőséget. Keresse meg és válassza ki az ügyfelet.

2. Válassza a **Fiókadatok lehetőséget.**

3. A **Microsoft Ügyfélszerződés** válassza a **Frissítés lehetőséget.**

4. Adja meg **a** szerződést elfogadó személy vezetéknevét, vezetéknevét, e-mail-címét és telefonszámát **(nem** kötelező).  A **Szerződés elfogadásának dátuma alatt** adja meg a megfelelő dátumot. Ezt nem állíthatja be jövőbeli dátumra.

5. Válassza **a Mentés és** folytatás lehetőséget.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Meglévő ügyfél.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Ügyfél-elfogadás megerősítésének lekérése

Ha megerősítést kér le arról, hogy egy meglévő ügyfél elfogadta a Microsoft Ügyfélszerződés, kövesse az alábbi lépéseket. Ehhez rendszergazdai vagy értékesítési ügynöknek kell lennie.

1. Válassza **az Ügyfelek** lehetőséget, majd keresse meg és válassza ki a látni kívánt ügyfelet.

2. Válassza a **Fiókadatok lehetőséget.**

3. A **Microsoft-ügyfélszerződés alatt** megtekintheti, hogy az ügyfél nem adott-e meg megerősítést.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Ügyfél-elfogadás megerősítése Partnerközpont API/SDK használatával

A Partnerközpont API/SDK használatával megerősítheti, hogy az ügyfelek elfogadják a Microsoft Ügyfélszerződés. Az API/SDK részleteiért tekintse meg a következőt:

- [A Microsoft Ügyfélszerződés szerződési metaadatainak lekérése](/partner-center/develop/get-customer-agreement-metadata)

- [Annak megerősítése, hogy az ügyfél elfogadta a Microsoft Ügyfélszerződést](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [A Microsoft Ügyfélszerződés ügyfél általi elfogadási megerősítésének lekérése](/partner-center/develop/get-confirmation-of-customer-agreement)

- [A sablon letöltési hivatkozásának Microsoft Ügyfélszerződés letöltése](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>2. lehetőség: Ügyfél-elfogadás Microsoft 365 Felügyeleti központban

A partnerek meghívhatják az új és meglévő ügyfeleket egy URL-címen keresztül, hogy áttekintik és elfogadják a Microsoft 365 Felügyeleti központban. A következő néhány szakasz a következőt mutatja be:

- Hozzon létre egy új ügyfelet, és hívja meg az ügyfelet, hogy tekintse át és fogadja el a szerződést.

- Hívjon meg egy új ügyfelet, hogy tekintse át és fogadja el a viszonteladói kapcsolatot és szerződést.

- Meghívhat egy meglévő ügyfelet, hogy tekintse át és fogadja el a szerződést.

>[!NOTE]
> A Partnerközpont [API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) használatával lekértheti az ügyfél közvetlen elfogadásának Microsoft Ügyfélszerződés.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Hozzon létre egy új ügyfelet, és hívja meg az ügyfelet, hogy tekintse át és fogadja el a szerződést

Az alábbi lépésekkel hozzon létre egy új ügyfelet a Partnerközpont, majd hívja meg őket, hogy fogadják el Microsoft Ügyfélszerződés felügyeleti Microsoft 365 felügyeleti központban.

1. A lap **Ügyfelek lapján** válassza Partnerközpont Ügyfél **hozzáadása lehetőséget.**

2. A **Fiókadatok területen** adja meg az új ügyfél adatait az összes kötelező mezőben, beleértve az ügyfél vállalatnevét és elsődleges kapcsolattartóját.

3. Az **Ügyfélszerződés alatt** válassza az Ügyfél lehetőséget, és fogadja el Microsoft Ügyfélszerződés felügyeleti **Microsoft 365 központban.** Töltse ki az oldalon található összes többi kötelező mezőt.

4. Válassza **a Tovább: Áttekintés lehetőséget,** majd folytassa az ügyfélbérlő létrehozásához szükséges lépéseket. 

>[!NOTE] 
>Az új ügyfelek csak akkor vásárolhatnak, ha elfogadják a Microsoft Ügyfélszerződés.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Új ügyfél létrehozása.":::

5. Amikor eléri a **Megerősítés képernyőt** az új ügyfél-munkafolyamatban, mentse az ügyfél hitelesítő adatait. Ezeket a hitelesítő adatokat később meg kell adnia az ügyfélnek.

6. A Partnerközpont hozzon létre és küldjön egy e-mailt, amely meghívja az ügyfelet, hogy fogadja Microsoft Ügyfélszerződés felügyeleti Microsoft 365 felügyeleti központban. Ügyeljen arra, hogy az alábbi elemeket is tartalmazza az e-mailben:

   - Az URL-címre mutató [hivatkozás](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (bejelentkezés szükséges)

   - Az ügyfél 5. lépésben mentett hitelesítő adatai.

7. Az ügyfél ezután megkapja a partnertől kapott e-mailes meghívót, és kiválasztja a [URL-címet.](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)

8. Az ügyfél bejelentkezik Microsoft 365 Felügyeleti központba az Ön által megadott ügyfél-hitelesítő adatokkal.

9. Az ügyfél a Microsoft-ügyfélszerződés elfogadásához ellenőrzi a jelölőnégyzetet.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Hívjon meg egy új ügyfelet, hogy tekintse át és fogadja el a viszonteladói kapcsolatot és Microsoft Ügyfélszerződés 

Az alábbi lépésekkel meghívhat egy új ügyfelet, hogy tekintse át és fogadja el a viszonteladói kapcsolatot és a Microsoft Ügyfélszerződés. 

1. Az **ügyfelek lapon** a Partnerközpont válassza **a Viszonteladói kapcsolat kérése hivatkozást.** 

2. A rendszer létrehoz egy automatikus e-mail-sablont, amely szöveget és egy paraméteres URL-címet tartalmaz, amely az ügyfelet a felügyeleti Microsoft 365 irányítja.

3. Testre szabhatja az automatikusan létrehozott e-mail-sablont, majd kiválaszthatja a Másolás a **vágólapra** vagy **a Megnyitás e-mailben lehetőséget.**

4. Ezzel az e-mail-sablonnal meghívhatja az ügyfelet, hogy fogadja el a **viszonteladói** kapcsolatkérést és a **Microsoft Ügyfélszerződés.** (Megjegyzés: Az e-mailes meghívóban győződjön meg arról, hogy a partner tartalmazza az automatikusan megadott URL-címet, valamint a közelmúltban létrehozott ügyfél-hitelesítő adatokat.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="hozzon létre egy kapcsolatot.":::

5. Az ügyfél e-mailben kap meghívót, és a paraméteres URL-címre kattint. 

6. Az ügyfél az e-mailben megadott hitelesítő adatokat használja a felügyeleti Microsoft 365 való bejelentkezéshez.

7. Az ügyfél ellenőrzi a jelölőnégyzetet a **viszonteladói kapcsolat elfogadásához,** és **Microsoft Ügyfélszerződés.** 

8. Ugyanazon az URL-címen belül az ügyfél láthatja azon partnerek összesített listáját, akiknél dolgozik. Kiválaszthat egy partnert, hogy lássa a részleteket.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Fogadja el a szerződést.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Meglévő ügyfél meghívása a szerződés felülvizsgálatára és elfogadására

Az alábbi lépésekkel meghívhat egy meglévő ügyfelet, hogy tekintse át és fogadja el Microsoft Ügyfélszerződés. 

1. Hozza létre az ügyfél e-mail-címét a beágyazott URL-címmel, amely meghívja az ügyfelet, hogy fogadja Microsoft Ügyfélszerződés.

2. Az ügyfél e-mailben megkapja a meghívót, és a URL-címre [kattint.](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 

3. Az ügyfél a Felügyeleti központban adja meg Microsoft 365 hitelesítő adatait.

4. Az ügyfél a jelölőnégyzet be- és elfogadásával fogadja Microsoft Ügyfélszerződés. 

5. Ugyanazon az URL-címen belül az ügyfél láthatja azon partnerek összesített listáját, akiknél dolgozik. Kiválaszthat egy partnert, hogy lássa a részleteket.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Ügyfél.":::

>[!NOTE]
>Bizonyos esetekben előfordulhat, hogy az ügyfelek nem tudják közvetlenül elfogadni a Microsoft Ügyfélszerződés. Az ilyen helyzetekkel kapcsolatos további információkért olvassa el az alábbi két forgatókönyvet, ahol az ügyfél nevében kell igazolnia.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Két forgatókönyv, ahol az ügyfél nevében kell igazolnia

Két esetben előfordulhat, hogy az ügyfelek nem tudják közvetlenül elfogadni a Microsoft Ügyfélszerződés felügyeleti Microsoft 365 belül.

**1.** forgatókönyv: Egy meglévő ügyfél a következők bármelyikét megvásárolta egy meglévő partnerkapcsolaton keresztül: ajánlatok, szoftver- vagy szoftver-előfizetések, fenntartott példányok vagy Azure-csomag. Az ügyfél most új vásárlást kísérel meg (kivéve az automatikus megújítást). Amikor az ügyfél az URL-címre kattint, a következő üzenet jelenik meg: "Kérjük, forduljon a partneréhez, hogy erősítse meg a Microsoft Ügyfélszerződés."  

**A megoldáshoz:** Az ügyfél nevében kell igazolnia.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Képernyőkép Microsoft 365 Felügyeleti központ oldalról, amely arra kéri, hogy a partnerrel való megerősítést kérve erősítse meg a Microsoft Ügyfélszerződés.":::

**2. forgatókönyv:** Egy meglévő ügyfél megvásárolta az alábbi ajánlatok, szoftver- és szoftver-előfizetések, fenntartott példányok és Azure-csomag bármelyikét. Az ügyfél most új vásárlást kísérel meg egy új partnernél.

Amikor az ügyfél az Microsoft 365 Felügyeleti központ URL-címére kattint az új partnerkapcsolat és a szerződés elfogadásához, a következő üzenetet kapja: "Kérjük, forduljon a partneréhez, hogy erősítse meg az ügyfél Microsoft Ügyfélszerződés."  

**A megoldáshoz:** Az ügyfél nevében kell igazolnia.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Annak ellenőrzése, hogy az ügyfél elfogadta-e a szerződést

Ha egy olyan meglévő ügyfélnek próbál új rendelést létrehozni, akit korábban nem erősítette meg, a rendszer felkéri a megerősítés befejezésére. Ehhez a következő eljárást használhatja.

1. Adja meg **a** szerződést elfogadó felhasználó vezetéknevét, vezetéknevét, e-mail-címét és telefonszámát **(nem** kötelező). 

2. A **Szerződés elfogadásának dátuma alatt** adja meg a megfelelő dátumot. Ezt nem állíthatja be jövőbeli dátumra.

3. Válassza a **Mentés és folytatás** lehetőséget. 

## <a name="next-steps"></a>Következő lépések

- [A vállalati profil információinak ellenőrzése vagy frissítése](update-your-partner-profile.md)
- [Microsoft Ügyfélszerződés (régió és nyelv szerint)](Agreements.md)
