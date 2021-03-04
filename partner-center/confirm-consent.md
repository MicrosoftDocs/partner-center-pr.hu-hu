---
title: Annak megerősítése, hogy az ügyfél elfogadta a Microsoft Ügyfélszerződést
description: Megtudhatja, hogyan erősítheti meg a Microsoft-ügyfél szerződését. Erre szükség lehet a Microsoft termékeinek és szolgáltatásainak megrendeléséhez az ügyfelek számára.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/02/2021
ms.openlocfilehash: ab2f5be77f6480b4a8b47bef0e0fd5096f7c1776
ms.sourcegitcommit: a7897284b79abb1ceeee79deb3a87b72d59900dc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "102029916"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Annak megerősítése, hogy az ügyfél elfogadta a Microsoft-ügyfélszerződést


**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Értékesítési ügynök

> [!NOTE]
> A partner Center jelenleg csak a Microsoft nyilvános felhőben támogatja a szerződési erőforrást. Nem alkalmazható a következőre:
> * A 21Vianet által üzemeltetett partneri központ
> * A Microsoft Cloud Germany Partnerközpontja
> * A Microsoft Cloud for US Government Partnerközpontja


Partnerként be kell szereznie a Microsoft-ügyfél szerződését, mielőtt a Microsoft termékeit és szolgáltatásait megrendeli az adott ügyfélhez. A partnereknek a megfelelőségi követelményeknek való megfelelés érdekében a Microsoft felkéri a partnereket, hogy erősítse meg az elfogadást a szerződést elfogadó személyre vonatkozó alábbi részletek megadásával:

- Utónév

- Vezetéknév

- E-mail-cím

- Telefonszám (nem kötelező)

- Elfogadás dátuma

A közvetlen számlás partnereknek és a közvetett szolgáltatóknak meg kell erősíteniük a Microsoft-ügyfél szerződését a partner Center vagy a partner Center API-n keresztül történő átadáskor. A megerősítés *kötelező*.

>[!NOTE]
>2020. január 31-ig az összes meglévő és új ügyfélnek alá kell írnia az új Microsoft Customer szerződést. További információért olvassa el [a Microsoft ügyfél-szerződés megerősítő ügyfeleinek jóváhagyása](confirm-customer-agreement.md)című témakört.

Ha nincs megadva visszaigazolás az adott ügyfélhez:

- Ehhez az ügyfélhez nem fog tudni új rendeléseket létrehozni.

- Az ügyfélhez már meglévő licenccel rendelkező előfizetések licencének száma nem módosítható.

Az ügyfelek elfogadásának megerősítése a partner Center vagy a partner Center API használatával végezhető el. Ha ezt a partner Center API-val szeretné elvégezni, tekintse meg a következő témaköröket:

- [Az ügyfél jóváhagyásának megerősítése](/partner-center/develop/get-confirmation-of-customer-consent)

- [Szerződés metaadatainak beolvasása](/partner-center/develop/get-agreement-metadata)

- [Az ügyfél jóváhagyásának megerősítése](/partner-center/develop/confirm-customer-consent)

Ez a termelési és a homokozó környezetekre is vonatkozik.

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>Ügyfél-elfogadás megerősítése új ügyfél számára

A következő eljárással ellenőrizheti az ügyfelek elfogadását, miközben új ügyfél-bérlőt hoz létre a partner Centerben. Ehhez rendszergazdai ügynöknek vagy értékesítési ügynöknek kell lennie.

1. Válassza az **ügyfelek**, majd az **új ügyfél** lehetőséget, majd válassza a **fiókadatok** lehetőséget.

2. Adja meg a **vállalat** és az **elsődleges kapcsolat** adatait.

   :::image type="content" source="images/mca/mca1.png" alt-text="Vállalati adatok":::

3. A **Microsoft ügyfél-szerződés** területen válassza ki **az ügyfelet a Microsoft legújabb ügyfél-szerződésének elfogadásával**.

4. A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot. Ez nem állítható be jövőbeli dátumra.

5. Adja meg az elfogadást elfogadó felhasználó részleteit.

   :::image type="content" source="images/mca/MCA3.png" alt-text="Elfogadás dátumának hozzáadása":::

   Alapértelmezés szerint az elsődleges kapcsolattartási felhasználói adatok jelennek meg. Ha ez nem megfelelő, válassza a **frissítés** lehetőséget, majd adja meg a szerződést elfogadó személy **utónevét**, **vezetéknevét**, **e-mail-címét** és **telefonszámát* (nem kötelező).

6. A **Tovább gombra kattintva** folytassa az ügyfél bérlő létrehozásához szükséges további lépéseket.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Ügyfél-elfogadás megerősítése egy meglévő ügyfélnél

Ehhez rendszergazdai ügynöknek vagy értékesítési ügynöknek kell lennie.

1. Válassza ki az **ügyfelek** lehetőséget, majd keresse meg és válassza ki a megtekinteni kívánt ügyfelet.

2. Válassza a **fiókadatok** lehetőséget.

3. A **Microsoft ügyfél-szerződés** területen válassza a **frissítés** lehetőséget.

   :::image type="content" source="images/mca/mca4.png" alt-text="Frissítés":::

4. Adja meg a szerződést elfogadó felhasználó **utónevét**, **vezetéknevét**, **e-mail címét** és **telefonszámát** (nem kötelező).

5. A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot. Ez nem állítható be jövőbeli dátumra.

6. Válassza a **Mentés és folytatás** lehetőséget.

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Az ügyfelek elfogadásának megerősítése egy meglévő ügyfél új sorrendjének létrehozásakor

Ha olyan meglévő ügyfélhez próbál új rendelést létrehozni, akit még nem erősített meg, a megerősítés befejezésére vonatkozó kérést kap. Ezt a következő eljárással végezheti el.

1. Adja meg a szerződést elfogadó felhasználó **utónevét**, **vezetéknevét**, **e-mail címét** és **telefonszámát** (nem kötelező).

2. A **Szerződés elfogadásának dátuma** mezőben adja meg a megfelelő dátumot. Ez nem állítható be jövőbeli dátumra.

3. Válassza a **Mentés és folytatás** lehetőséget.

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Ügyfél-elfogadás megerősítésének beolvasása egy meglévő ügyfélnél

Lekérheti az ügyfél elfogadásának megerősítését egy meglévő ügyfél számára, amelyet korábban az alábbi eljárással adott meg. Ehhez rendszergazdai ügynöknek vagy értékesítési ügynöknek kell lennie.

1. Válassza ki az **ügyfelek** lehetőséget, majd keresse meg és válassza ki a megtekinteni kívánt ügyfelet.

2. Válassza a **fiókadatok** lehetőséget.

3. A **Microsoft ügyfél-szerződés** alatt láthatja, hogy az ügyfél megkapta-e a megerősítést.

## <a name="next-steps"></a>Következő lépések

- [Erősítse meg a Microsoft Customer szerződés ügyfél általi elfogadását a CSP-partner programban](confirm-customer-agreement.md)

- [A Microsoft ügyfél-szerződés elfogadásának igazolása az ügyfél nevében](attest-acceptance-customer-agreement.md)