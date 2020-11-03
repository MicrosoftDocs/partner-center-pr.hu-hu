---
title: Ügyfél-hozzárendelés létrehozása
ms.topic: article
ms.date: 09/11/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Hozzon létre ügyfél-hozzárendeléseket a Recording (CPOR) modell igénylési partnerével. Segíti az értékesítések, a használat és a Microsoft 365 & Dynamics 365-ügyfelek által nyújtott ösztönzők kezelését.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e34698b51a159445f4354e366f79f510533e6f30
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/19/2020
ms.locfileid: "92530469"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a>Ügyfél-hozzárendelések a Microsoft 365 és a Dynamics 365-es rekord (CPOR) modellje révén

**A következőkre vonatkozik**

- Partnerközpont

**Megfelelő szerepkörök:**

- Ösztönzők rendszergazdája

2019. október 1-jén a Microsoft megkezdte a CPOR-modell igénylési partnerének használatát a Microsoft 365 és a Dynamics 365-ügyfelekkel folytatott társítások kezeléséhez az online szolgáltatások tanácsadó (OSA) értékesítés, online szolgáltatások használata (OSU) Microsoft 365 és OSU-Business alkalmazási ösztönzők tekintetében.

>[!Important]
> Az ügyfél-hozzárendelési (CPOR) jogcímek csak az online szolgáltatások tanácsadó (OSA) értékesítésére, az online szolgáltatások használatára (OSU) vonatkoznak, és a OSU-Business alkalmazás Microsoft 365-ösztönző programokra. Ha egy másik programhoz (például a felhőalapú megoldás-szolgáltatóhoz, a felügyelt viszonteladóhoz, az üzemeltetéshez vagy a felszínhez) tartozó együttes op-jogcímet küld, tekintse meg az itt ismertetett együttes op-jogcímek folyamatát. <br><br>A jogcímek beküldésekor a Microsoft érvényesíti azt. Ezen a ponton további információkat kérhetünk. A társulási kérelem ügyfelét is értesíteni fogjuk. Az ügyfeleknek öt munkanapon belül kell kijelentkezniük. Ha nem, akkor az adott Bérlővel és munkaterheléssel való társítása hivatalos lesz. Ezen a ponton elérheti az ügyfél használati adatait. 

A jogcímek elvégzéséhez a következő információkra lesz szüksége:

- Az entitáshoz tartozó **MPN-azonosító** , amely a jogcímet végrehajtja

- Az ügyfél **tartománynevének** [megkeresése](find-domain-name.md)

- Az ügyfél **címtár-azonosítójának** vagy **bérlői azonosítójának** [megkeresése](find-domain-name.md)

- A **megoldási területen** , például Business Applications vagy Microsoft 365

- A végrehajtott **tevékenység** és a kívánt jogcím típusa, például értékesítés előtti, használati vagy bevételi társítás

- Az ügyfél **kapcsolattartási neve** , címe és e-mail-címe

- A Dynamics 365 esetében meg kell adnia az ügyfél **technikai kapcsolattartójának** nevét, címét és e-mail-címét is.

- Saját vállalata **kapcsolattartójának neve** és e-mail-címe

- Létre kell hoznia egy **nevet** a jogcím számára

- Az Ön által igényelt **termék (ek)** vagy számítási feladat (ok)

- A **végrehajtás igazolása (PoE)** , például az ügyfél által aláírt munkavégzési utasítás. Le is töltheti a használni kívánt PoE-sablont.

- Csak a bevételi társulást igénylő partnerek esetén: a **Dynamics-megoldás eladójának neve** , az **ügyfél neve** és **az ISV termék/megoldás neve** . 

A következő szempontokat is ismernie kell:

- Ha már rendelkezik Microsoft 365 ügyfelekkel, újra hozzá kell rendelnie azokat, akikkel továbbra is OSU-ösztönzőket szeretne keresni a folyamat használatával.

- Ha meglévő, Dynamics 365-as vagy Power BI ügyfelekkel rendelkező társításokkal rendelkezik, ezek a társítások érvényesek maradnak az előfizetésük lejárta után.

- Egy ügyfél több partnerrel is rendelkezhet, de a munkaterhelések (OSU-Microsoft 365) vagy az előfizetés (OSA-Sell és OSU-Business alkalmazások esetében) csak egyetlen partnerhez társíthatók.

## <a name="create-a-customer-association"></a>Ügyfél-hozzárendelés létrehozása

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).

2. Válassza az **ösztönzők** lapot, válassza az **Áttekintés** lehetőséget, majd válassza az **ügyfelek társítások** lehetőséget.

3. Az ügyfél-hozzárendelések lap tetején válassza a **+ Ügyfél-hozzárendelés** lehetőséget.

4. Válassza ki az ügyfélhez társítani kívánt partnerhely **MPN-azonosítóját** , majd adja hozzá az ügyfél tartománynevét és címtár-azonosítóját. [Keresés](find-domain-name.md)

5. Válassza a **Folytatás** lehetőséget.

6. Válassza ki a **megoldási területeket** és **tevékenységeket** . 

   >[!Note]
   >
   >Ha a Business Applications lehetőséget választja, válassza a **használat és/vagy az értékesítés előtti** vagy a **bevételi társítás** lehetőséget, majd válassza a **Folytatás** lehetőséget. 
   <br><br>Ha a bevétel társítását választja, a rendszer az alább felsorolttól némileg eltérő adatokat kér.

7. Adja meg a megfelelő adatokat az **Ügyfél hozzárendelése** lapon, majd válassza a **jogcím létrehozása** lehetőséget.

8. Válassza ki az ügyfél-hozzárendeléshez társított terméket (ka) t, majd válassza a **Folytatás** lehetőséget.

9. Töltse ki az ügyfél és a vállalat kapcsolattartási adatait. Minden mezőt ki kell tölteni. 

   >[!NOTE]
   >Ha a termék a Dynamics 365, és a kiválasztott termék több előfizetéssel rendelkezik ehhez az adott ügyfélhez, meg kell adnia az előfizetés-azonosítót is.

10. Adja meg a végrehajtás igazolását (PoE). Húzza a mezőbe, tallózással keresse meg a saját támogató dokumentációját, vagy válassza a **Sablon letöltése** lehetőséget, és használjon egy sablont. 

11. Tetszés szerint adja hozzá és mentse a megjegyzéseket, majd válassza az **Igénylés beküldése** elemet. Egy e-mailt küldünk az Ön ügyféltársítását elfogadását kérő ügyfélnek.

   >[!NOTE]
   >Miután elküldte az ügyfél-hozzárendelést, nem szerkesztheti.

Az ügyféltársítás állapota az **Állapot** mezőben jelenik meg.

Válassza az **Előzmények** lehetőséget az ügyféltársítás előzményeinek megtekintéséhez.

## <a name="next-steps"></a>Következő lépések

- [Ügyféltársítások kezelése](incentives-manage-customer-associations.md)