---
title: Ügyféltársítás létrehozása
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Ügyfél-társítások létrehozása a igénylő regisztrált partner (CPOR) modellel. Segít a Dynamics 365-ügyfelek értékesítésének, használatának és Microsoft 365 & kezelésében.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9526a47d0b6d734bde48f403c11fa84d734511c1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856100"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a>Ügyféltársítások az igényelt rekordpartner (CPOR) modellen keresztül a Microsoft 365 Dynamics 365-höz


**Megfelelő szerepkörök:** Ösztönzők rendszergazdája

2019. október 1-től a Microsoft az igénylő regisztrált partner (CPOR) modellt kezdte használni az Microsoft 365- és Dynamics 365-ügyfelekkel való társítások kezelésére az Online Services Tanácsadás (OSA) Értékesítés, Online Services Usage (OSU)-Microsoft 365 és OSU-Business Application ösztönzők tekintetében.

>[!Important]
> Az ügyfél-társítási (CPOR) igények csak az Online Services Advisor (OSA) értékesítésre, az online szolgáltatások használatára (OSU) vonatkozó Microsoft 365 és az OSU-Business alkalmazásösztönző programokra vonatkoznak. Ha együttműködési igényt nyújt be egy másik programhoz, például a Felhőszolgáltató, Managed Reseller, Hosting vagy Surface programhoz, tekintse meg az itt ismertetett együttműködési igényfolyamatot. <br><br>Az igénylés elküldésekor a Microsoft érvényesíti azt. Ezen a ponton további információkat kérhetünk Öntől. A társítási kérelemről is értesítjük az ügyfelet. Az ügyfeleknek öt munkanapjuk van a lemondásra. Ha nem fogják kikapcsolni a regisztrációt, az Adott bérlővel és számítási feladattal való társítása hivatalos lesz. Ezen a ponton hozzáférhet az ügyfél használati adataihoz. 

A jogcímek igénylésének befejezéséhez a következő információkra lesz szüksége:

- A jogcímet igénylést igénylő entitás **MPN-azonosítója**

- Ügyfél **tartományneve** [Keresse meg ezt](find-ids-and-domain-names.md)

- Az ügyfél **címtár-azonosítója** vagy **bérlőazonosítója** [Keresse meg ezt](find-ids-and-domain-names.md)

- A **Megoldás terület,** például Business Applications vagy Microsoft 365

- Az **elvégzett** tevékenység és a kívánt jogcím típusa, például értékesítés előtti, használati vagy bevételi társítás

- Az ügyfél Kapcsolattartó **neve,** címe és e-mail-címe

- A Dynamics 365 esetén az ügyfél műszaki  kapcsolattartója nevét, címét és e-mail-címét is meg kell adnia

- Saját vállalata **kapcsolattartójának neve és** e-mail-címe

- Létre fog hozni egy **Nevet** a jogcímhez

- Az **igényelt termék(nek)** vagy számítási feladat(nak)

- **A végrehajtás igazolása (PoE),** például az ügyfél által aláírt munkakivonat. A használathoz letöltheti a PoE-sablont is.

- Csak bevételi társítást igénylő partnerek esetén: **Dynamics-megoldás** értékesítője neve, Ügyfél **neve** és **ISV-termék/megoldás neve.** 

A következő pontokat is érdemes megértenie:

- Ha már vannak Microsoft 365 ügyfelek, akkor a folyamat használatával újra társíthatja azokat, akik továbbra is OSU-ösztönzőket keresnek.

- Ha már rendelkezik Dynamics 365- vagy Power BI-ügyfelekkel, ezek a társítások az előfizetésük lejáratáig érvényesek maradnak.

- Egy ügyfél több partnerrel is rendelkezik, de minden számítási feladat (OSU-Microsoft 365 esetében) vagy előfizetés (OSA-Sell és OSU-Business-alkalmazások esetén) csak egy partnerhez társítható.

## <a name="create-a-customer-association"></a>Ügyféltársítás létrehozása

1. Jelentkezzen be a [Partnerközpont irányítópultjába](https://partner.microsoft.com/dashboard/).

2. Válassza az **Ösztönzők lapot,** válassza az **Áttekintés,** majd az Ügyfél-társítások **lehetőséget.**

3. Az Ügyfél-társítások lap tetején válassza a + Ügyfél **társítása lehetőséget.**

4. Válassza ki az ügyfélhez társítani kívánt partnerhely **MPN-azonosítóját**, majd adja hozzá az ügyfél tartománynevét és címtár-azonosítóját. [Keresse meg ezt a](find-ids-and-domain-names.md)

5. Válassza a **Folytatás** lehetőséget.

6. Válassza ki **a Megoldás területet és** a **Tevékenységet.** 

   >[!Note]
   >
   >Ha a Business Applications, válassza a **Használat és/vagy** az Értékesítés előtti , vagy a Bevétel társítása **lehetőséget,** majd válassza a Folytatás **lehetőséget.** 
   <br><br>Ha a bevétel társítását választja, a rendszer az alább felsorolttól némileg eltérő adatokat kér.

7. Adja meg a megfelelő adatokat a **Associate customer (Ügyfél** társítása) lapon, majd válassza a Create claim (Jogcím **létrehozása) lehetőséget.**

8. Válassza ki az ügyfél-társításhoz társított termék(eket), majd válassza a **Continue (Folytatás) lehetőséget.**

9. Töltse ki az ügyfél és a vállalat kapcsolattartási adatait. Minden mezőt ki kell tölteni. 

   >[!NOTE]
   >Ha a termék a Dynamics 365, és a választott termék több előfizetéssel rendelkezik ehhez az ügyfélhez, meg kell adnia az előfizetés azonosítóját is.

10. A végrehajtási igazolást (PoE) is meg kell adni. Húzza a mezőbe, tallózással keresse meg a saját támogató dokumentációját, vagy válassza a **Sablon letöltése** lehetőséget, és használjon egy sablont. 

11. Tetszés szerint adja hozzá és mentse a megjegyzéseket, majd válassza az **Igénylés beküldése** elemet. Egy e-mailt küldünk az Ön ügyféltársítását elfogadását kérő ügyfélnek.

   >[!NOTE]
   >Miután beküldi az ügyfél-társítást, nem szerkesztheti.

Az ügyféltársítás állapota az **Állapot** mezőben jelenik meg.

Válassza az **Előzmények** lehetőséget az ügyféltársítás előzményeinek megtekintéséhez.

## <a name="next-steps"></a>Következő lépések

- [Ügyféltársítások kezelése](incentives-manage-customer-associations.md)