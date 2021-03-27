---
title: Annak ellenőrzése, hogy az ügyfél elfogadta-e a Microsoft ügyfél-szerződést a CSP programhoz
description: A Microsoft-szolgáltatások ügyfeleknek való megrendelése előtt a Cloud Solution Provider (CSP) partnereinek meg kell erősíteniük a Microsoft ügyfél-szerződését.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633778"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Annak ellenőrzése, hogy az ügyfél elfogadta-e a Microsoft ügyfél-szerződést a CSP programhoz

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Értékesítési ügynök


Az ügyfelek két lehetőség közül választhatnak, hogy elfogadják a Microsoft ügyfél-szerződését.

**1. lehetőség**: az ügyfél-hitelesítés partneri igazolása – a partner megerősítheti az ügyfelek elfogadását a partner Center API/SDK használatával vagy a partner Center irányítópultján.

**2. lehetőség**: közvetlen ügyfél-elfogadás – a partner meghívhatja az ügyfelet egy URL-címen keresztül, hogy áttekintse és elfogadja a szerződést a Microsoft 365 felügyeleti központban.

## <a name="access-microsoft-customer-agreement-template"></a>Hozzáférés a Microsoft ügyfél-szerződési sablonhoz

A Microsoft Customer Agreement sablon legújabb verzióját manuálisan is letöltheti [innen.](https://aka.ms/customeragreement) A Microsoft Customer szerződés országspecifikus. A Microsoft ügyfél-szerződési sablon kérésekor a megfelelő országot válassza ki az ügyfél helye alapján.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>1. lehetőség: az ügyfelek elfogadásának megerősítése a partner Centerben

A közvetlen számla partnerei megerősítik a Microsoft ügyfél-szerződését a partner Centerben az új és a meglévő ügyfelek számára. A közvetett viszonteladók nem tanúsítják az ügyfeleik nevében, és nem kell együttműködni a közvetett szolgáltatóval az igazolás befejezéséhez.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Az ügyfelek elfogadásának megerősítése új ügyfelek esetén

Amikor új ügyfél-bérlőt hoz létre a partner Centerben, kövesse az alábbi lépéseket a Microsoft ügyfél-szerződés elfogadásának megerősítéséhez. A lépések végrehajtásához rendszergazdai vagy értékesítési ügynöknek kell tartoznia.

1. Válassza az **ügyfelek**, majd az **új ügyfél** lehetőséget.

2. A **fiók adatai** területen adja meg a vállalat és az elsődleges kapcsolattartó adatait.

3. A **Microsoft-szerződés** területen jelölje be a jelölőnégyzetet annak igazolására, hogy az ügyfél elfogadta a Microsoft ügyfél-szerződést.

4. A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot. Ez nem állítható be jövőbeli dátumra.

5. Győződjön meg arról, hogy az elsődleges felhasználói kapcsolattartási adatok helyesek. Ha nem megfelelő, válassza a **frissítés** lehetőséget, és adja meg a szerződést elfogadó személy pontos információit.

6. A **tovább** gombra kattintva folytathatja az ügyfél-bérlő létrehozását.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Új ügyfél":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Ügyfelek elfogadásának megerősítése meglévő ügyfelek esetén

Ennek elvégzéséhez rendszergazdai vagy értékesítési ügynöknek kell lennie:

1. Válassza az **Ügyfelek** lehetőséget. Keresse meg és válassza ki az ügyfelet.

2. Válassza a **fiókadatok** lehetőséget.

3. A **Microsoft ügyfél-szerződés** területen válassza a **frissítés** lehetőséget.

4. Adja meg a szerződést elfogadó személy **utónevét**, **vezetéknevét**, **e-mail-címét** és **telefonszámát** (nem kötelező). A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot. Ez nem állítható be jövőbeli dátumra.

5. Válassza a **Mentés** és Folytatás lehetőséget.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Meglévő ügyfél":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Az ügyfél-elfogadás megerősítésének beolvasása

A következő lépések végrehajtásával kérheti le, hogy egy meglévő ügyfél elfogadta a Microsoft ügyfél-szerződést. Ehhez rendszergazdai ügynöknek vagy értékesítési ügynöknek kell lennie.

1. Válassza ki az **ügyfelek** lehetőséget, majd keresse meg és válassza ki a megtekinteni kívánt ügyfelet.

2. Válassza a **fiókadatok** lehetőséget.

3. A **Microsoft ügyfél-szerződés** alatt tekintse meg, hogy az ügyfél nem adta-e meg a megerősítést.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Az ügyfelek elfogadásának megerősítése a partner Center API/SDK használatával

A partner Center API/SDK használatával megerősítheti a Microsoft-ügyfél szerződését. Az API-val/SDK-val kapcsolatos részletekért tekintse meg a következőt:

- [A Microsoft Ügyfélszerződés szerződési metaadatainak lekérése](/partner-center/develop/get-customer-agreement-metadata)

- [Annak megerősítése, hogy az ügyfél elfogadta a Microsoft Ügyfélszerződést](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [A Microsoft Ügyfélszerződés ügyfél általi elfogadási megerősítésének lekérése](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Letöltési hivatkozás letöltése a Microsoft ügyfél-szerződési sablonhoz](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>2. lehetőség: az ügyfél elfogadottsága Microsoft 365 felügyeleti központban

A partnerek meghívhatnak új és meglévő ügyfeleket egy URL-címen keresztül, hogy áttekintsék és elfogadják a szerződést a Microsoft 365 felügyeleti központban. A következő néhány szakaszban bemutatjuk, hogyan végezheti el a következőket:

- Hozzon létre egy új ügyfelet, és kérje meg az ügyféltől a szerződés áttekintését és elfogadását.

- Kérje meg az új ügyfelet, hogy tekintse át és fogadja el a viszonteladói kapcsolatot és szerződést.

- Kérje meg a meglévő ügyfelet, hogy tekintse át és fogadja el a szerződést.

>[!NOTE]
> A [partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) használatával lekérheti a Microsoft ügyfél-szerződés közvetlen elfogadásának állapotát.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Hozzon létre egy új ügyfelet, és kérje meg az ügyfelet a szerződés áttekintésére és elfogadására

A következő lépésekkel hozzon létre egy új ügyfelet a partner Centerben, majd hívja meg őket, hogy tekintsék át és fogadják el a Microsoft Customer szerződést Microsoft 365 felügyeleti központban.

1. A partner Center **ügyfelek** lapján válassza az **ügyfél hozzáadása** lehetőséget.

2. A **fiókadatok** területen adja meg az új ügyfél adatait az összes kötelező mezőben, beleértve az ügyfél vállalatának nevét és az elsődleges kapcsolattartót is.

3. Az **ügyfél szerződése** területen válassza **az ügyfél lehetőséget, hogy fogadja el a Microsoft Customer szerződést Microsoft 365 felügyeleti központban**. Hajtsa végre az oldalon található egyéb kötelező mezőket.

4. Válassza a Next (tovább) lehetőséget **: Tekintse át** , majd folytassa az ügyfél-bérlő létrehozásához szükséges lépéseket. 

>[!NOTE] 
>Az új ügyfelek nem vásárolhatják meg a vásárlást, amíg el nem fogadják a Microsoft Customer szerződést.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Új ügyfél létrehozása":::

5. Amikor eléri a **megerősítő** képernyőt az új ügyfél munkafolyamatban, mentse az ügyfél hitelesítő adatait. Ezeket a hitelesítő adatokat később kell megadnia az ügyfélnek.

6. A partner centeren kívül hozzon létre és küldjön egy e-mailt, amely meghívja az ügyfelet, hogy fogadja el a Microsoft Customer szerződést Microsoft 365 felügyeleti központban. Ügyeljen rá, hogy ezeket az elemeket az e-mailben adja meg:

   - Hivatkozás erre az [URL-címre](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (bejelentkezés szükséges)

   - Az ügyfél az 5. lépésben mentett hitelesítő adatai.

7. Az ügyfél ezután megkapja az e-mailes meghívót a partnertől, és kiválasztja az [URL-címet](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Az ügyfél a megadott felhasználói hitelesítő adatokkal jelentkezik be Microsoft 365 felügyeleti központba.

9. Az ügyfél ellenőrzi a mezőt, hogy fogadja el a Microsoft ügyfél-szerződést.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Új ügyfél meghívása a viszonteladói kapcsolat és a Microsoft ügyfél-szerződés áttekintéséhez és elfogadásához 

A következő lépésekkel meghívhat egy új ügyfelet a viszonteladói kapcsolat és a Microsoft ügyfél-szerződés áttekintésére és elfogadására. 

1. A partner Center **ügyfelek** lapján válassza a **viszonteladói kapcsolat kérése** hivatkozást. 

2. Létrejön egy automatikus e-mail sablon, amely tartalmazza a szöveget és egy paraméteres URL-címet, amely a Microsoft 365 felügyeleti központba irányítja az ügyfelet.

3. Testreszabhatja az automatikusan létrehozott e-mail-sablont, majd kiválaszthatja a **Másolás a vágólapra** vagy **a Megnyitás e-mailben** lehetőséget.

4. Ezzel az e-mail sablonnal meghívhatja az ügyfelet, hogy fogadja el a **viszonteladói kapcsolatra** vonatkozó kérelmet és a **Microsoft Customer szerződést**. (Megjegyzés: a meghívó e-mailben ellenőrizze, hogy a partner tartalmazza-e az automatikusan megadott URL-címet, valamint a nemrégiben létrehozott ügyfél-hitelesítő adatokat is.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="kapcsolat létrehozása":::

5. Az ügyfél e-mailben fogadja a meghívót, és rákattint a paraméteres URL-címre. 

6. Az ügyfél az e-mailben megadott hitelesítő adatokat használja a Microsoft 365 felügyeleti központba való bejelentkezéshez.

7. Az ügyfél ellenőrzi a mezőt, hogy elfogadja a **viszonteladói kapcsolatot** és a **Microsoft ügyfél-szerződést**. 

8. Ugyanazon az URL-címen belül az ügyfél megtekintheti a különböző partnerek összevont listáját, amelyekkel dolgozik. Kijelölhetnek egy partnert a részletek megtekintéséhez.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Szerződés elfogadása":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Meglévő ügyfél meghívása a szerződés áttekintéséhez és elfogadásához

A következő lépésekkel meghívhat egy meglévő ügyfelet a Microsoft Customer szerződés áttekintéséhez és elfogadásához. 

1. Hozza létre az ügyfél e-mail-címét a beágyazott URL-címmel, amelyben meghívja ügyfeleit, hogy fogadja el a Microsoft Customer szerződést.

2. Az ügyfél e-mailben fogadja a meghívót, és rákattint az [URL-címre](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Az ügyfél a hitelesítő adataikat Microsoft 365 felügyeleti központba írja be.

4. Az ügyfél ellenőrzi a mezőt, hogy fogadja el a Microsoft ügyfél-szerződést. 

5. Ugyanezen az URL-címen az ügyfél láthatja a különböző partnerek összevont listáját, amelyekkel dolgozik. Kijelölhetnek egy partnert a részletek megtekintéséhez.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="ügyfél":::

>[!NOTE]
>Bizonyos esetekben előfordulhat, hogy az ügyfelek nem tudják közvetlenül elfogadni a Microsoft ügyfél-szerződést. Ha többet szeretne megtudni ezekről a helyzetekről, olvassa el a következő két forgatókönyvet, ahol az ügyfél nevében kell tanúsítani az alábbi lépéseket.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Két forgatókönyv, ahol az ügyfél nevében kell tanúsítani

Két forgatókönyv esetén előfordulhat, hogy az ügyfelek nem tudják közvetlenül elfogadni a Microsoft ügyfél-szerződést a Microsoft 365 felügyeleti központban.

**1. eset**: egy meglévő ügyfél a következők bármelyikét vásárolta egy meglévő partneri kapcsolaton keresztül: ajánlatok, szoftver-vagy szoftver-előfizetések, fenntartott példányok vagy Azure-csomag. Az ügyfél most megpróbál új vásárlást végezni (az automatikus megújítás kivételével). Amikor az ügyfél az URL-címre kattint, a "Kérjük, forduljon a partneréhez, hogy erősítse meg a Microsoft-ügyfél szerződését."  

**Megoldás**: az ügyfél nevében kell tanúsítani.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Képernyőkép a Microsoft 365 felügyeleti központ oldaláról, amely arra kéri, hogy forduljon a partnerhez a Microsoft ügyfél-szerződés elfogadásának megerősítéséhez.":::

**2. forgatókönyv**: egy meglévő ügyfél megvásárolta a következő ajánlatok bármelyikét, a szoftver-és szoftver-előfizetéseket, a fenntartott példányokat és az Azure-csomagot. Az ügyfél most megpróbál új partnert vásárolni.

Amikor az ügyfél az új partneri kapcsolat és a szerződés elfogadásához rákattint az Microsoft 365 felügyeleti központ URL-címére, a következő üzenet jelenik meg: "Kérjük, forduljon a partneréhez, hogy erősítse meg a Microsoft-ügyfél szerződését."  

**Megoldás**: az ügyfél nevében kell tanúsítani.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Erősítse meg, hogy az ügyfél elfogadta a szerződést

Ha olyan meglévő ügyfélhez próbál új rendelést létrehozni, akit még nem erősített meg, a megerősítés befejezésére vonatkozó kérést kap. Ezt a következő eljárással végezheti el.

1. Adja meg a szerződést elfogadó felhasználó **utónevét**, **vezetéknevét**, **e-mail címét** és **telefonszámát** (nem kötelező).

2. A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot. Ez nem állítható be jövőbeli dátumra.

3. Válassza a **Mentés és folytatás** lehetőséget. 

## <a name="next-steps"></a>Következő lépések

- [A vállalati profil adatainak ellenőrzése vagy frissítése](update-your-partner-profile.md)
- [Microsoft Ügyfélszerződés (régió és nyelv szerint)](Agreements.md)
