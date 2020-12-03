---
title: Microsoft Azure foglalás megvásárlása az ügyfelek számára
description: Megtudhatja, hogyan vásárolhat vagy vásárolhat Azure-foglalásokat az ügyfelek nevében a partner Centerben. Azokat a piacokat is felsorolja, amelyekben az Azure-foglalások nem érhetők el.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: 0e81a9561f3749aab281bb4ebd7cd0c38540ff31
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534607"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Microsoft Azure foglalások vásárlása az ügyfelek nevében a partner Centerben

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Globális rendszergazda
- Segélyszolgálat ügynöke
- Értékesítési ügynök
- Felhasználói felügyeleti rendszergazda

Ez a cikk azt ismerteti, hogyan vásárolhat vagy vásárolhat Azure-foglalásokat az ügyfelek nevében a partner Centerben. Azokat a piacokat is azonosítja, amelyekben az Azure-foglalások nem érhetők el.
 
> [!NOTE]
> Ez a cikk csak a Cloud Solution Provider (CSP) programban található partnerekre vonatkozik. A más típusú előfizetéseket (például az utólagos elszámolású, az egyéni, a Microsoft-ügyféli szerződést vagy a Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek Ehelyett olvasniuk kell [Az Azure foglalási dokumentációját](/azure/cost-management-billing/reservations).

## <a name="before-you-begin"></a>Előkészületek

Tekintse át az alábbi fontos információkat, mielőtt az ügyfelek nevében megvásárolja az Azure-foglalásokat. (Szeretné, hogy az ügyfelek megvásárolják saját Azure-foglalásait egy korábban megvásárolt Azure-előfizetésből? Tekintse [meg, hogy az ügyfelek jogosultak-e saját Azure-foglalások megvásárlására](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations).)

- Ha és amikor az ügyfél aláírja az új Microsoft ügyfél-szerződést (lásd: [a Microsoft ügyfél-szerződés elfogadásának megerősítése](confirm-customer-agreement.md)), az Azure-csomag keretében kell megvásárolnia az Azure-foglalásokat. További információért olvassa el az [Azure-csomag megvásárlása](purchase-azure-plan.md)című témakört.

- Az ügyfeleknek már aktív Azure-előfizetéssel kell rendelkezniük ahhoz, hogy a nevükben foglalásokat lehessen vásárolni
  
- A szoftveres előfizetések költségei, például az SQL Database vagy a SUSE Linux szoftver nem szerepelnek az Azure foglalási áraiban

- A Microsoft kereskedelmi díjszabása nem tartalmaz adókat, kivéve, ha a tartózkodási helye Brazília. Ha a tartózkodási helye Brazília, a kereskedelmi ár tartalmazza a megfelelő adókat

- Az értékesítési és ügyfélszolgálati ügynököknek explicit hozzáférésre van szükségük az Azure-előfizetéshez, így az ügyfél nevében megvásárolhatják vagy kezelhetik a Azure Portal és a fájlokra vonatkozó támogatási kéréseket, beleértve az adatcseréket és a visszatérítéseket is.  

- Ha Ön közvetett szolgáltató, és az Azure-foglalásokat a Azure Portal keresztül vásárolja meg, akkor a Record (közvetett viszonteladó) partner a kiválasztott Azure CSP-előfizetéstől örökölt.

- A Record for Azure-foglalások partnere nem módosítható a vásárlás után. Megszakíthatja a meglévő foglalást, és vásárolhat újat a rekord új partnerével.

- Ha egy ügyfél közvetlen vagy nagyvállalati szerződéssel rendelkező Azure-előfizetést szeretne átvinni a CSP-re, a foglalások nem vihetők át.

## <a name="azure-reservations-unavailable-markets"></a>Azure-foglalások nem elérhető piacai

> [!IMPORTANT]
> Az Azure-foglalások **nem** érhetők el az alábbi piacokon:  
>  
> **Nem elérhető piacok (ABC sorrendben)**
>
> |A – GI   | Gr – PAL  | Pap – Z |
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
> | Bouvet-sziget     | Jan Mayen     | São Tomé és Príncipe   |
> | Brit indiai-óceáni terület       | Jersey     | Seychelle-szigetek   |
> | Brit Virgin-szigetek     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Koszovó     | Sint Eustatius     |
> | Burundi     | Laosz     | Sint Maarten     |
> | Kambodzsa     | Lesotho     | Salamon-szigetek     |
> | Közép-afrikai Köztársaság     | Libéria     | Szomália     |
> | Csád     | Madagaszkár     | Déli-Georgia és Déli-Sandwich-szigetek     |
> | Kína     | Malawi     | Dél-Szudán     |
> | Karácsony-sziget     | Maldív-szigetek     | Szent Ilona, Ascension, Tristan da Cunha     |
> | Cocos (Keeling)-szigetek     | Mali     | Suriname     |
> | Comore-szigetek     | Marshall-szigetek     | Svalbard     |
> | Kongó     | Martinique     | Szváziföld     |
> | Kongó (KDK)     | Mauritánia     | Timor-Leste   |
> | Cook-szigetek     | Mayotte     | Togo   |
> | Dzsibuti     | Mikronézia     | Tokelau   |
> | Dominika     | Montserrat     | Tonga   |
> | Egyenlítői-Guinea     | Mozambik     | Turks- és Caicos-szigetek   |
> | Eritrea     | Mianmar     | Tuvalu   |
> | Falkland-szigetek     | Nauru     | Az Amerikai Egyesült Államok lakatlan külbirtokai   |
> | Francia Guyana     | Új-Kaledónia     | Vanuatu   |
> | Francia Polinézia     | Niger     | Vatikán   |
> | Francia Déli Területek     | Niue     | Wallis és Futuna   |
> | Gabon     | Norfolk-sziget     | Jemen   |
> | Gambia     | Északi Mariana-szigetek     |    |
> | Gibraltár     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Azure-foglalások vásárlása

Az alábbi lépéseket követve vásárolhatja meg Microsoft Azure foglalásait az ügyfelek nevében a partner Centerben. (Szeretné, hogy az ügyfelek megvásárolják saját Azure-foglalásait egy korábban megvásárolt Azure-előfizetésből? Tekintse [meg, hogy az ügyfelek jogosultak-e saját Azure-foglalások megvásárlására](give-customers-permission.md).)

1. Válassza ki az **ügyfelek** elemet a partner központ menüből.  

2. Az **ügyfelek** lapon keresse meg azt az ügyfelet, aki szeretné megvásárolni az Azure-foglalásokat, majd a lefelé mutató nyílra kattintva bontsa ki az ügyfél sorát.  

3. Válassza a **termékek hozzáadása** lehetőséget, majd válassza az **Azure** lehetőséget. 

    a. Válassza ki az ügyfél piaci szegmensét a **szegmens** listából.

    b. A **terméktípus listából válassza** a **foglalások** lehetőséget.

    c. Válassza ki, hogy az ügyfél milyen típusú foglalást szeretne a **foglalások típusa** listából.

4. Az Azure-foglalásokat aktív Azure-előfizetéssel kell társítani. Válassza ki azt az ügyfél-előfizetést, amelyhez Azure-foglalásokat kíván hozzáadni az **ügyfél-előfizetések** listájából. 

   >[!IMPORTANT]
   >Ha az ügyfél még nem rendelkezik aktív Azure-előfizetéssel, válassza az **Azure** lehetőséget a hozzáadáshoz. 

5. A szűrők használatával megkeresheti az ügyfél igényeinek megfelelő virtuális gépeken az Azure-foglalásokat.  

6. Ha megtalálta a megvásárolni kívánt foglalás (oka) t, adja meg a lefoglalt példányok számát **, majd válassza** a **Hozzáadás a kosárhoz** lehetőséget.  

7. Ismételje meg az 5. és a 6. lépést, amíg hozzá nem adta az összes szükséges elemet a rendeléshez. A megrendelés helyességének ellenőrzéséhez válassza az **Áttekintés** lehetőséget.  

8. A **megrendelések áttekintése** lapon a következőket teheti: 

    - Ellenőrizze vagy módosítsa a fenntartott példányok mennyiségét.

    - Válassza ki a foglalás hatókörét. A foglalás hatóköre egyetlen előfizetésre vagy több előfizetésre (megosztott hatókörre) is vonatkozhat. Ha a foglalás hatókörét egyetlen előfizetésre alkalmazza, a foglalási kedvezmény csak erre az előfizetésre lesz alkalmazva. Ha a megosztott lehetőséget választja, a foglalási kedvezményt az ügyfél számlázási környezetében lévő összes előfizetésre alkalmazza a rendszer. 

      >[!NOTE] 
      >Ha úgy dönt, hogy a foglalás hatókörét egyetlen Azure-előfizetésre korlátozza, akkor előfordulhat, hogy meg kell emelnie az előfizetés vCPU-kvótáját. Az előfizetés vCPU-kvótájának növeléséhez létre kell hoznia egy támogatási kérelmet a Azure Portal. A kérelem létrehozásához kövesse az [ebben a témakörben található](/azure/azure-supportability/resource-manager-core-quotas-request) utasításokat. 

      >[!NOTE]   
      >Ha az ügyfél az Azure-csomag alatt van, a **hatókör**  a **megosztott** értékre lesz állítva. 

    - Ha Ön szolgáltatói partner, válassza ki azt a viszonteladót, amelyet hozzá szeretne rendelni a termékhez.
    
    - Ha az Azure-foglalás támogatja a számlázási csomag lehetőséget, akkor a legördülő menüből kiválaszthatja a számlázási gyakoriságot. 
    - Ha az Azure-foglalás nem támogatja a számlázási csomag lehetőséget, akkor a számlázási gyakoriság alapértelmezés szerint egyszeres számlázást végez. 

9. Válassza a **vásárlás** lehetőséget a megrendelés megvásárlásához. A megrendelés részletei, beleértve a megrendelés számát is, a **megerősítés** lapon jelennek meg. A **kész** gombra kattintva lépjen a **rendelési előzmények** lapra. 

10. Ha az ügyfél foglalását a Azure Portalban szeretné kezelni, keresse meg az ügyfelet az **ügyfelek** lapon, majd a lefelé mutató nyílra kattintva bontsa ki az ügyfél sorát. Válassza a **a Microsoft Azure felügyeleti portálja** lehetőséget az ügyfél rekordjának megnyitásához a Azure Portal.

## <a name="next-steps"></a>További lépések

|**További információ**   |**Olvassa el ezt**    |
|:-----------------------------|:-----------------|
|Azure-foglalások a CSP-ben – áttekintés  | [Microsoft Azure fenntartott példányok eladása](azure-reservations.md) |
|Azure-foglalások kezelése a partner Centerben | [Azure-foglalások kezelése a partner Centerben](azure-reservations-manage.md)
|A virtuális gép megfelelő méretének meghatározása és az ügyfél virtuális gépek használatának ellenőrzése   |[Virtuális gép méretezése az Azure-foglalások maximális használatára](azure-usage.md)   |
|Azure-foglalások vásárlása a partner Center API használatával | [Vásárlás Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) a partner Center fejlesztői dokumentációjában   |
|Engedélyt ad a felhasználóknak a saját Azure-foglalások megvásárlására  | [Engedélyt ad az ügyfeleknek a saját Azure-foglalások megvásárlására](give-customers-permission.md)  |