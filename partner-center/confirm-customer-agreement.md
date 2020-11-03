---
title: Annak megerősítése, hogy az ügyfél elfogadta a Microsoft-ügyfélszerződést
description: Megtudhatja, hogyan erősítheti meg a Microsoft-ügyfél szerződését. A Cloud Solution Provider (CSP) program résztvevői számára a Microsoft termékeinek és szolgáltatásainak megrendeléséhez szükséges.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 05/05/2020
ms.openlocfilehash: 45a34473ff63875af8bd07962ea836661bc948ee
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530637"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a>Erősítse meg a Microsoft Customer szerződés ügyfél általi elfogadását a CSP-partner programban

**A következőkre vonatkozik**

- Partnerközpont
- Microsoft 365 felügyeleti központ

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Értékesítési ügynök

2019. október 1-jén a Microsoft bevezette a **Microsoft ügyfél-szerződést** a CSP programba, hogy lecserélje a Microsoft Cloud szerződést. További [útmutatást](indirect-reseller-tasks-in-partner-center.md) a közvetett viszonteladók számára című témakörben talál. A partnereknek az új szerződésre való áttelepítésének megkönnyítése érdekében mindkét szerződés a CSP-programban a 2020. január 31-ig is létezett. 2020. február 1-től a Microsoft Customer szerződése lecserélte a Microsoft Cloud szerződést.

Az ügyfelek két lehetőség közül választhatnak a Microsoft ügyfél-szerződés elfogadásához. 

**1. lehetőség** : az ügyfél-hitelesítés partneri igazolása – a partner megerősítheti az ügyfelek elfogadását a partner Center API/SDK használatával vagy a partner Center irányítópultján.

**2. lehetőség** : közvetlen ügyfél-elfogadás – a partner meghívhatja az ügyfelet egy URL-címen keresztül, hogy áttekintse és elfogadja a szerződést a Microsoft 365 felügyeleti központban.

## <a name="access-microsoft-customer-agreement-template"></a>Hozzáférés a Microsoft ügyfél-szerződési sablonhoz

A Microsoft Customer Agreement sablon legújabb verzióját manuálisan is letöltheti [innen.](https://aka.ms/customeragreement) A Microsoft Customer szerződés országspecifikus. A Microsoft ügyfél-szerződési sablon kérésekor a megfelelő országot válassza ki az ügyfél helye alapján.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>1. lehetőség: az ügyfelek elfogadásának megerősítése a partner Centerben

A partnerek megerősítik a Microsoft ügyfél-szerződését a partner Centerben az új és a meglévő ügyfelek számára. A viszonteladók nem tanúsítják az ügyfeleik nevében, és nem kell együttműködni a közvetett szolgáltatóval az igazolás befejezéséhez.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Az ügyfelek elfogadásának megerősítése új ügyfelek esetén

Amikor új ügyfél-bérlőt hoz létre a partner Centerben, kövesse az alábbi lépéseket a Microsoft ügyfél-szerződés elfogadásának megerősítéséhez. A lépések végrehajtásához rendszergazdai vagy értékesítési ügynöknek kell tartoznia.

1. Válassza az **ügyfelek** , majd az **új ügyfél** lehetőséget.

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

4. Adja meg a szerződést elfogadó személy **utónevét** , **vezetéknevét** , **e-mail-címét** és **telefonszámát** (nem kötelező). A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot. Ez nem állítható be jövőbeli dátumra.

5. Válassza a **Mentés** és Folytatás lehetőséget.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Új ügyfél":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Az ügyfél-elfogadás megerősítésének beolvasása

A következő lépésekkel kérheti le, hogy egy meglévő ügyfél elfogadta a Microsoft ügyfél-szerződést. Ehhez rendszergazdai ügynöknek vagy értékesítési ügynöknek kell lennie.

1. Válassza ki az **ügyfelek** lehetőséget, majd keresse meg és válassza ki a megtekinteni kívánt ügyfelet.

2. Válassza a **fiókadatok** lehetőséget.

3. A **Microsoft ügyfél-szerződés** alatt tekintse meg, hogy az ügyfél nem adta-e meg a megerősítést.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Az ügyfelek elfogadásának megerősítése a partner Center API/SDK használatával

A partner Center API/SDK használatával megerősítheti a Microsoft-ügyfél szerződését. Az API-val/SDK-val kapcsolatos részletekért tekintse meg a következőt:

- [Szerződési metaadatok beszerzése a Microsoft ügyfél-szerződéshez](/partner-center/develop/get-customer-agreement-metadata)

- [A Microsoft ügyfél-szerződés elfogadásának megerősítése](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [A Microsoft ügyfél-szerződés elfogadásának megerősítése](/partner-center/develop/get-confirmation-of-customer-agreement)

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

3. Az **ügyfél szerződése** területen válassza az első lehetőséget, a **rendszer felkéri az ügyfelet, hogy fogadja el a Microsoft Customer szerződést Microsoft 365 felügyeleti központban** . Hajtsa végre az oldalon található egyéb kötelező mezőket.

4. Válassza a Next (tovább) lehetőséget **: Tekintse át** , majd folytassa az ügyfél-bérlő létrehozásához szükséges lépéseket. 

>[!NOTE] 
>Az új ügyfelek nem tudnak új vásárlást végezni, amíg el nem fogadják a Microsoft Customer szerződést.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Új ügyfél":::

5. Amikor eléri a **megerősítő** képernyőt az új ügyfél munkafolyamatban, mentse az ügyfél hitelesítő adatait. Ezeket a hitelesítő adatokat később kell megadnia az ügyfélnek.

6. A partner centeren kívül hozzon létre és küldjön egy e-mailt, amely meghívja az ügyfelet, hogy fogadja el a Microsoft Customer szerződést Microsoft 365 felügyeleti központban. Ügyeljen rá, hogy ezeket az elemeket az e-mailben adja meg:

   - Hivatkozás erre az [URL-címre](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (bejelentkezés szükséges)

   - Az ügyfél az 5. lépésben mentett hitelesítő adatai.

7. Az ügyfél ezután megkapja az e-mailes meghívót a partnertől, és kiválasztja az [URL-címet](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Az ügyfél a partnertől kapott ügyfél-hitelesítő adatokkal jelentkezik be Microsoft 365 felügyeleti központba.

9. Az ügyfél ezután megkeresi a mezőt, hogy fogadja el a Microsoft ügyfél-szerződést.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Új ügyfél meghívása a viszonteladói kapcsolat és a Microsoft ügyfél-szerződés áttekintéséhez és elfogadásához 

A következő lépésekkel meghívhat egy új ügyfelet a viszonteladói kapcsolat és a Microsoft ügyfél-szerződés áttekintésére és elfogadására. 

1. A partner Center **ügyfelek** lapján válassza a **viszonteladói kapcsolat kérése** hivatkozást. 

2. Létrejön egy automatikus e-mail sablon, amely tartalmazza a szöveget és egy paraméteres URL-címet, amely a Microsoft 365 felügyeleti központba irányítja az ügyfelet.

3. Testreszabhatja az automatikusan létrehozott e-mail-sablont, majd kiválaszthatja a **Másolás a vágólapra** vagy **a Megnyitás e-mailben** lehetőséget.

4. Ezzel az e-mail sablonnal meghívhatja az ügyfelet, hogy fogadja el a **viszonteladói kapcsolatra** vonatkozó kérelmet és a **Microsoft Customer szerződést** . (Megjegyzés: a meghívó e-mailben ellenőrizze, hogy a partner tartalmazza-e az automatikusan megadott URL-címet, valamint a nemrégiben létrehozott ügyfél-hitelesítő adatokat is.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Új ügyfél":::

5. Az ügyfél e-mailben fogadja a meghívót, és rákattint a paraméteres URL-címre. 

6. Az ügyfél a partner e-mailben megadott hitelesítő adatait használja a Microsoft 365 felügyeleti központba való bejelentkezéshez.

7. Az ügyfél ellenőrzi a mezőt, hogy elfogadja a **viszonteladói kapcsolatot** és a **Microsoft ügyfél-szerződést** . 

8. Ugyanazon az URL-címen belül az ügyfél megtekintheti a különböző partnerek összevont listáját, amelyekkel dolgozik. Kijelölhetnek egy partnert a részletek megtekintéséhez.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Új ügyfél":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Meglévő ügyfél meghívása a szerződés áttekintéséhez és elfogadásához

A következő lépésekkel meghívhat egy meglévő ügyfelet a Microsoft Customer szerződés áttekintéséhez és elfogadásához. 

1. Hozza létre az ügyfél e-mail-címét a beágyazott URL-címmel, amelyben meghívja ügyfeleit, hogy fogadja el a Microsoft Customer szerződést.

2. Az ügyfél e-mailben fogadja a meghívót, és rákattint az [URL-címre](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Az ügyfél a hitelesítő adataikat Microsoft 365 felügyeleti központba írja be.

4. Az ügyfél ellenőrzi a mezőt, hogy fogadja el a Microsoft ügyfél-szerződést. 

5. Ugyanezen az URL-címen az ügyfél láthatja a különböző partnerek összevont listáját, amelyekkel dolgozik. Kijelölhetnek egy partnert a részletek megtekintéséhez.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Új ügyfél":::

>[!NOTE]
>Bizonyos esetekben előfordulhat, hogy az ügyfelek nem tudják közvetlenül elfogadni a Microsoft ügyfél-szerződést. Ha többet szeretne megtudni ezekről a helyzetekről, tekintse meg az alábbi [két forgatókönyvet, ahol igazolnia kell az ügyfél nevében](attest-acceptance-customer-agreement.md).

### <a name="historical-timeline-details"></a>Korábbi idővonal részletei

| Dátum | Mérföldkő | Részletek |
|------------|------------|--------------------------------|
|Augusztus 01., 2019| Az UX előzetes verziója elérhető a homokozóban| A partnerek megerősítik a Microsoft ügyfél-szerződését a CSP homokozó környezetében található partner Center irányítópult használatával. Partnerek, akik hozzáférnek a CSP homokozó környezethez – előzetes verzió a felhasználói élmény változásairól. A sandbox-hozzáférés nélküli partnerek megismerhetik a jelen témakör változásait.|
|Szeptember 03., 2019|Az API előzetes verziója elérhető a homokozóban.|A partner megerősítheti a Microsoft-ügyfél szerződését a Customer Center API használatával a CSP homokozó környezetében. Az API-partnerek ezzel a lehetőséggel megtekinthetik az API-módosításokat, és megkezdhetik a munkát az API-integrációban az új szerződés támogatásához.|
|Szeptember 20., 2019|A .NET SDK előzetes verziója elérhető a homokozóban.|A partner megerősítheti a Microsoft-ügyfél szerződését a partner Center .NET SDK-val a CSP homokozó környezetében. Az API-partnerek ezt a lehetőséget használhatják a .NET SDK változásainak megtekintésére és az API-integráció használatának megkezdésére az új szerződés támogatásához.|
|Október 01, 2019|A Microsoft ügyfél-szerződése az éles környezetben érhető el|A Microsoft bevezeti a Microsoft ügyfél-szerződést a CSP programba, hogy lecserélje a Microsoft Cloud szerződést. A partnerek megerősítik a Microsoft ügyfél-szerződését a partner Center irányítópultjának és az éles környezetben futó API-nak a használatával. A Microsoft Cloud szerződés továbbra is támogatott a CSP-partner programon belül. A partnerek azonban azt tanácsolják, hogy kezdjen el migrálni a Microsoft ügyfél-szerződésbe. A meglévő előfizetésekhez tartozó új vásárlások és licencek száma a Microsoft ügyfél-szerződéssel vagy a Microsoft Cloud Szerződéssel való partneri megerősítést igényel. Bizonyos új ajánlatok (például az új Azure-csomag) megerősítést igényelnek a Microsoft ügyfél-szerződéshez.|
|2020. január 31.|Microsoft Cloud a szerződés el lett távolítva az éles környezetből|A Microsoft Cloud szerződés már nem fogadható el a CSP-partner programon belül. A meglévő előfizetésekhez tartozó új vásárlások és licencek számának változása esetén a partnernek meg kell erősítenie a Microsoft ügyfél-szerződést. Ez a követelmény olyan új ügyfelekre és meglévő ügyfelekre vonatkozik, akik korábban elfogadták a Microsoft Cloud szerződést.|
|Február 3., 2020|A partnernek lehetősége van arra, hogy meghívja az ügyfelet egy URL-címen keresztül, hogy áttekintse és elfogadja a megállapodást a hitelesített Microsoft 365 felügyeleti központban. | Az ügyfél elfogadhatja a Microsoft Customer szerződést Microsoft 365 felügyeleti központban. Az ügyfél Microsoft 365 felügyeleti központban lévő szerződésének közvetlen elfogadása megerősíti a feltételek jóváhagyását. 