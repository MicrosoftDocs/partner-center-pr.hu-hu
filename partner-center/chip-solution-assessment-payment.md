---
title: Megoldásértékelés fizetési állapota
ms.topic: how-to
ms.date: 11/09/2020
description: A Channel Incentives Platform (CHIP) használatával információkat találhat a megoldásértékelési lehetőségekről, azok számításáról és fizetési állapotáról.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4184d155ceff22a34e1a85d2909f4e1b17a46daa
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148873"
---
# <a name="solution-assessment-payment-status-and-calculation-info"></a>Megoldásértékelés fizetési állapota és számítási adatai

**Megfelelő szerepkörök:** Elsődleges kapcsolattartó vagy program-rendszergazda

A Megoldásértékelési lehetőség fizetési állapotát a CHIP-ban tudja áttekintni.

## <a name="how-to-review-your-payment-status"></a>A fizetési állapot áttekintése

1. Nyissa meg a CHIP-et, és jelentkezzen be Microsoft-fiókjával (az előző Live ID-val).
2. A **Lehetőségazonosító mezőbe** írja vagy illessze be a lehetőség azonosítószámát.
3. Kattintson a **Keresés** gombra.
4. Válassza ki a lehetőség nevét a lehetőség részleteinek megtekintéséhez.
5. Ellenőrizze **a Fizetési kérelmek szakaszban,** hogy létrejött-e a fizetési kérelem.
6. Tekintse át a lehetőség állapotát.

    - Ha a fizetési kérelem nem jön létre, győződjön meg arról, hogy a lehetőség megfelel a Megoldásértékelési ösztönző bevételére vonatkozó feltételeknek. A jogosultsági feltételek ellenőrzésével kapcsolatos további információkat a [Solution Assessment (Megoldásértékelés) oldalon talál.](chip-solution-assessment.md)
    - Ha a fizetési kérelem létrejött, folytassa a 7. lépéssel.
7. Ellenőrizze a fizetési kérelem állapotát.

    - Fizetés felülvizsgálata függőben: További vizsgálatért lépjen kapcsolatba a csatornaösztönzők csapatával – az alább felsorolt kapcsolattartási adatok alapján.
    - Kifizetés jóváhagyva: A Microsoft a hónap végén 35 napon belül rendereli a kifizetést, miután az EM tanúsítja a kötelezettségvállalás teljességét a CHIP-ben, amelyben a fizetési kérelem létrejött
    -  Elküldött fizetés: Kattintson az állapothivatkozásra a fizetési kiadás részleteinek megtekintéséhez.
    - Fizetés lemondva: Kattintson az állapothivatkozásra az elutasítás okának megtekintéséhez. További részletekért forduljon a Csatornaösztönzők csapathoz.

## <a name="calculations-for-solutions-assessment"></a>Megoldások felmérésének számításai

A megadott díjütemezők használatával a Microsoft regionális műveleti központjai kiszámítják és feldolgozják a kapcsolódó ösztönződíjakat, havi kifizetésekkel.

Ahhoz, hogy a lehetőségek megjelenjenek ebben a fizetési jóváhagyási jelentésben, az alábbi attribútumokkal kell, hogy legyen:

1. A Megoldásértékelési ösztönzőt jóvá kell hagyni.

1. Solution Assessment Engagement Level local attribute Rate level is set for the engagement at the incentive is approved in MSX (A Solution Assessment Engagement-szint helyi attribútumának sebességszintje az ösztönző MSX-beli jóváhagyásakor).
 
1. Az EM-nek be kell jelölve és be kell nyújtania az EM által a CHIP-be beküldött "EM Review" (EM-felülvizsgálat) jelölőnégyzetet.

## <a name="next-steps"></a>Következő lépések

- [Problémák a CHIP elérésekor](chip-access-trouble.md) 
