---
title: Foglalások Microsoft Azure vásárlása ügyfelek számára
description: Megtudhatja, hogyan vásárolhat Azure-foglalásokat az ügyfelei nevében a Partnerközpont. Azokat a piacokat is felsorolja, ahol az Azure-foglalások nem érhetők el.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: cd8a78edab25b94e678aafd61ca96e61a625fb07
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149536"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Vásároljon Microsoft Azure foglalásokat az ügyfelek nevében a Partnerközpont

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Globális rendszergazdai | Az | Értékesítési ügynök | Felhasználókezelő rendszergazda

Ez a cikk azt ismerteti, hogyan vásárolhat Azure-foglalásokat az ügyfelek nevében a Partnerközpont. Azokat a piacokat is azonosítja, ahol az Azure-foglalások nem érhetők el.
 
> [!NOTE]
> Ez a cikk csak a Felhőszolgáltató (CSP) program partnereire vonatkozik. A más típusú előfizetéseket (például használat alapján fizetett, egyéni, Microsoft Ügyfélszerződés- vagy Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek érdemes elolvasni az [Azure Reservations dokumentációját.](/azure/cost-management-billing/reservations)

## <a name="before-you-begin"></a>Előkészületek

Tekintse át az alábbi fontos információkat, mielőtt megvásárolja az Azure Reservationst az ügyfelek nevében. (Azt szeretné, hogy az ügyfelek megvásárolják saját Azure-foglalásukat a számukra megvásárolt korábbi Azure-előfizetésből? Lásd: Adjon engedélyt az ügyfeleknek a [saját Azure-foglalásaik vásárlásra.)](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations)

- Ha és amikor az ügyfél aláírja az új Microsoft Ügyfélszerződés (lásd: [Ügyfél](confirm-customer-agreement.md)általi elfogadás megerősítése a Microsoft Ügyfélszerződés ), Azure-foglalásokat kell vásárolnia az Azure-csomag alatt. További információ: [Azure-csomag vásárlása.](purchase-azure-plan.md)

- Az ügyfeleknek már aktív Azure-előfizetéssel kell rendelkezikuk, mielőtt megvásárolni tudja a foglalásokat a nevükben
  
- Az Azure-foglalások díjszabása nem SQL Database a szoftver-előfizetési költségeket, például a SQL Database vagy a SUSE Linux szoftverét

- A Microsoft kereskedelmi díjszabása nem tartalmazza az adókat, kivéve, ha a tartózkodási helye Brazília. Ha a tartózkodási helye Brazília, az Önnek megfelelő kereskedelmi ár tartalmazza a megfelelő adókat

- Az értékesítési és ügyfélszolgálati ügynököknek explicit hozzáférésre van szükségük az Azure-előfizetéshez, hogy megvásárolni vagy kezelni tudják az Azure Portal-ban és a fájltámogatási kérelmekben, beleértve a cserét és a visszatérítést az ügyfél nevében  

- Ha Ön közvetett szolgáltató, és az Azure Portal-ban vásárol Azure-foglalásokat, a rekordpartner (közvetett viszonteladó) a kiválasztott Azure CSP örökli.

- Az Azure Reservations rekordpartnere nem módosítható a vásárlás után. Megszüntetheti a meglévő foglalást, és megvásárolhat egy újat az új Rekord partnerrel.

- Ha egy ügyfél Egy Azure-előfizetést szeretne átvini a Közvetlen előfizetésből vagy a Nagyvállalati Szerződésből a CSP-be, a foglalások átadása nem történik meg.

## <a name="azure-reservations-unavailable-markets"></a>Az Azure Reservations nem elérhető piacai

> [!IMPORTANT]
> Az **Azure-foglalások a** következő piacokon nem érhetők el:  
>  
> **Nem elérhető piacok (betűrendben)**
>
> |A–Gi   | Gr –Pal  | Pap–Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Åland-szigetek     | Grönland     | Pápua Új-Guinea     |
> | Amerikai Szamoa     | Grenada     | Pitcairn-szigetek     |
> | Andorra     | Guadeloupe     | Réunion     |
> | Anguilla     | Guam     | Saba   |
> | Antarktisz     | Guernsey     | Saint Barthélemy   |
> | Antigua és Barbuda       | Guinea     | Saint Lucia   |
> | Aruba       | Bissau-Guinea     | Saint Martin   |
> | Azerbajdzsán       | Guyana     | Saint-Pierre és Miquelon   |
> | Benin     | Haiti       | Saint Vincent és Grenadine-szigetek     |
> | Bhután     | Heard-sziget és McDonald-szigetek       | Szamoa     |
> | Bonaire     | Man-sziget     | San Marino     |
> | Bouvet-sziget     | Jan Mayen     | Sémo Tomé és Príncipe   |
> | Brit indiai-óceáni terület       | Jersey     | Seychelle-szigetek   |
> | Brit Virgin-szigetek     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Koszovó     | Sint Eustatius     |
> | Burundi     | Laosz     | Sint Maarten     |
> | Kambodzsa     | Lesotho     | Salamon-szigetek     |
> | Közép-afrikai Köztársaság     | Libéria     | Szomália     |
> | Csád     | Madagaszkár     | Dél-Georgia és Déli-Sandwich-szigetek     |
> | Kína     | Malawi     | Dél-Szudán     |
> | Karácsony-sziget     | Maldív-szigetek     | St Majda, Ascension, Tristan da Canha     |
> | Cocos (Keeling)-szigetek     | Mali     | Suriname     |
> | Comore-szigetek     | Marshall-szigetek     | Svalbard     |
> | Kongó     | Martinique     | Szváziföld     |
> | Kongó (KDK)     | Mauritánia     | Timor-Leste   |
> | Cook-szigetek     | Mayotte     | Togo   |
> | Dzsibuti     | Mikronézia     | Tokelau   |
> | Dominika     | Montserrat     | Tonga   |
> | Egyenlítői-Guinea     | Mozambik     | Turks- és Caicos-szigetek   |
> | Eritrea     | Mianmar     | Tuvalu   |
> | Falkland-szigetek     | Nauru     | Az Usa-beli, outlying-szigetek   |
> | Francia Guyana     | Új-Kaledónia     | Vanuatu   |
> | Francia Polinézia     | Niger     | Vatikán   |
> | Francia Déli Területek     | Niue     | Wallis és Futuna   |
> | Gabon     | Norfolk-sziget     | Jemen   |
> | Gambia     | Északi Mariana-szigetek     |    |
> | Gibraltár     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Azure-foglalások megvásárlása

Kövesse az alábbi lépéseket a Microsoft Azure vásárláshoz az ügyfelek nevében a Partnerközpont. (Azt szeretné, hogy az ügyfelek megvásárolják saját Azure-foglalásukat egy korábbi Azure-előfizetésből, amit megvásárolt nekik? Lásd: Give customers permission to buy their own Azure reservations (Engedélyeket adhat az ügyfeleknek [saját Azure-foglalások vásárláshoz).)](give-customers-permission.md)

1. Válassza **az Ügyfelek** lehetőséget Partnerközpont menüből.  

2. Az Ügyfelek **lapon** keresse meg az Azure Reservationst megvásárolni kívánó ügyfelet, majd a lefelé mutató nyílra kattintva bontsa ki az ügyfél sorát.  

3. Válassza a **Termékek hozzáadása,** majd az **Azure lehetőséget.** 

    a. Válassza ki az ügyfél piaci szegmensét a **Szegmens listából.**

    b. Válassza a **Foglalások** lehetőséget a **terméktípus listából.**

    c. A Foglalások típusa listából válassza ki, hogy az ügyfél milyen **típusú foglalást szeretne.**

4. Az Azure Reservationst aktív Azure-előfizetéssel kell társítva lennie. Válassza ki annak az ügyfélnek az előfizetését, akihez Azure-foglalásokat szeretne hozzáadni az **Ügyfél-előfizetések listájából.** 

   >[!IMPORTANT]
   >Ha az ügyfél még nem rendelkezik aktív Azure-előfizetéssel, válassza az **Azure** lehetőséget egy új hozzáadásához. 

5. A szűrőkkel megkeresheti az Azure Reservationst az ügyfél igényeinek megfelelő virtuális gépeken.  

6. Miután megkeresi a megvásárolni kívánt foglalás(ak)t, adja meg, hogy az ügyfélnek hány fenntartott példányra lesz szüksége a **Quantity** (Mennyiség) mezőben, majd válassza a Add to cart (Hozzáadás a **kosárhoz) lehetőséget.**  

7. Ismételje meg az 5. és a 6. lépést, amíg hozzá nem adott minden szükséges elemet a rendeléshez. Válassza **az Áttekintés** lehetőséget a rendelés helyességének ellenőrzéséhez.  

8. A Rendelések **áttekintése lapon** a következőt használhatja: 

    - Ellenőrizze vagy módosítsa a fenntartott példányok mennyiségét.

    - Válassza ki a foglalás hatókörét. A foglalás hatóköre egy vagy több előfizetésre (megosztott hatókör) vonatkozhat. Ha a foglalás hatóköre egyetlen előfizetésre terjed ki, a rendszer csak erre az előfizetésre alkalmazza a foglalási kedvezményt. Ha a megosztott lehetőséget választja, a rendszer a foglalási kedvezményt az ügyfél számlázási környezetében található összes előfizetésre alkalmazza. 

      >[!NOTE] 
      >Ha úgy dönt, hogy a foglalás hatókörét egyetlen Azure-előfizetésre korlátozza, előfordulhat, hogy növelnie kell az előfizetés vCPU-kvótáját. Az előfizetés vCPU-kvótája növeléséhez létre kell hoznia egy támogatási kérést a Azure Portal. A kérelem [létrehozásához kövesse az](/azure/azure-supportability/resource-manager-core-quotas-request) ebben a témakörben található utasításokat. 

      >[!NOTE]   
      >Ha az ügyfél az Azure-csomag alá van beállítva, **a Hatókör**  beállítása **Megosztott** lesz. 

    - Ha Ön szolgáltatói partner, válassza ki a termékhez társítani kívánt viszonteladót.
    
    - Ha az Azure-foglalása támogatja a Számlázási csomag lehetőséget, kiválaszthatja a számlázási gyakoriságot havi szinten a legördülő menüből. 
    - Ha az Azure-foglalás nem támogatja a Számlázási csomag lehetőséget, a számlázási gyakoriság alapértelmezés szerint csak egyszer lesz kiszámlázás. 

9. A **rendelés megvásárlásához** válassza a Vásárlás lehetőséget. A rendelés részletei, beleértve a rendelés számát is, a Megerősítés **lapon jelennek** meg. A **Rendelési** előzmények oldalra **való ugráshoz** válassza a Kész lehetőséget. 

10. Az ügyfél foglalásának kezeléséhez a Azure Portal keresse meg az ügyfelet az **Ügyfelek** oldalon, majd a lefelé mutató nyílra kattintva bontsa ki az ügyfél sorát. Válassza **a Microsoft Azure felügyeleti portálja** az ügyfél rekordját a Azure Portal.

## <a name="next-steps"></a>Következő lépések

|**További információ:**   |**Olvassa el ezt**    |
|:-----------------------------|:-----------------|
|Azure Reservations a CSP-ban – áttekintés  | [Fenntartott Microsoft Azure értékesítés](azure-reservations.md) |
|Azure Reservations kezelése a Partnerközpont | [Azure Reservations kezelése a Partnerközpont](azure-reservations-manage.md)
|A megfelelő virtuálisgép-méret meghatározása és az ügyfél virtuálisgép-használatának ellenőrzése   |[Virtuális gép méretezése az Azure-beli foglalások maximális kihasználtságában](azure-usage.md)   |
|Azure-foglalások vásárlása a Partnerközpont API-val | [Vásárlás Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) a Partnerközpont fejlesztői dokumentációjában   |
|Engedély adva az ügyfeleknek a saját Azure-foglalásaik vásárláshoz  | [Engedélyt adhat az ügyfeleknek a saját Azure-foglalásaik vásárlásra](give-customers-permission.md)  |