---
title: Azure-foglalások kezelése ügyfelek számára
description: Megtudhatja, hogyan kezelheti az ügyfelek Azure-foglalásait, beleértve a foglalások megszüntetését, a foglalások cseréjét vagy a visszatérítés igénylését.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: c377fca3e38161258c836d14202ac4db21484526
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534760"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Ügyfelek Microsoft Azure foglalásának kezelése, megszakítása, cseréje vagy visszatérítése

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Globális rendszergazda
- Segélyszolgálat ügynöke
- Értékesítési ügynök
- Felhasználói felügyeleti rendszergazda

Ez a cikk bemutatja, hogyan kezelheti az ügyfelek Azure-foglalásait, beleértve a foglalások megszüntetését, a foglalások cseréjét vagy a visszatérítés igénylését.

> [!NOTE]
> Ez a cikk csak a Cloud Solution Provider (CSP) programban található partnerekre vonatkozik. A más típusú előfizetéseket (például az utólagos elszámolású, az egyéni, a Microsoft-ügyféli szerződést vagy a Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek Ehelyett olvasniuk kell [Az Azure foglalási dokumentációját](/azure/cost-management-billing/reservations).

A vásárlás utáni Azure-foglalások kezeléséhez ki kell választania a partner Centerben felügyelni kívánt ügyfelet és foglalást, majd módosítania kell a foglalást a Azure Portalban.

1. Első lépésként válassza ki az **ügyfelek** lehetőséget a partner Center menüben, majd válassza ki azt az ügyfelet, amelynek a fenntartásait szeretné kezelni. 

2. Az ügyfél részletes oldalának menüjében válassza az **Azure-foglalások** lehetőséget, majd válassza ki a kezelni kívánt foglalást.  

3. A **műveletek** területen válassza a **kezelés** lehetőséget, hogy az ügyfél foglalási rekordjára lépjen a Azure Portal. A foglalás részletei lapon kövesse az alábbi lépéseket a feladatok elvégzéséhez.  

    | **Kiválasztás**   | **Hogy**    |
    |:-----------------------------|:-----------------|
    | **Áttekintés**   | Megtekintheti az ügyfél foglalásának részleteit, beleértve a lejárati dátumot, a hatókört és a kihasználtsági adatokat. **Megjegyzés** Válassza a **visszatérítés** lehetőséget, ha támogatási kérést szeretne létrehozni egy Pro minősítéssel rendelkező visszatérítéshez. Válassza az **Exchange** lehetőséget, ha támogatási kérést szeretne létrehozni a foglalási időszak fel nem használt részének cseréjéhez.  
    | **Access Control (IAM)**   | Az ügyfél foglalási adataihoz való hozzáférés kezelése.|
    | **Konfigurálás**   | Módosítsa a foglalás hatókörét és/vagy az Azure-előfizetést, amelyhez a foglalás társítva van.    |
    | **Tulajdonságok**   | Tekintse meg a foglalás tulajdonságait, és másolja a vágólapra a foglalási azonosító és a foglalási rendelés AZONOSÍTÓját. **Megjegyzés** A támogatás kérheti a foglalási azonosító és a foglalási sorrend AZONOSÍTÓjának megadását, ha az ügyfél nevében támogatást kér.    |
    | **Új támogatási kérelem**    | Segítség kérése Microsoft ügyfélszolgálataról.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Foglalás megszakítása vagy cseréje

Ha az ügyfél üzleti szükségleteit bármikor megváltoztatják, érdemes lehet lemondani egy foglalást, és visszatérítést vagy Exchange-foglalást kell fizetnie, amely az új foglalás díja alapján lesz felhasználva.

Mindkét forgatókönyv esetében a Microsoft visszafizeti az összeget Önnek, így kezelheti az így létrejövő pénzügyi tranzakciókat az ügyfelekkel. A Microsoft nem közvetlen kapcsolatba lép az ügyfelekkel a számlázással, a lemondással vagy a visszatérítéssel kapcsolatban.

### <a name="how-cancellations-work"></a>A lemondások működése

Az ügyfelek bármikor kérhetik a foglalások lemondását (a visszatérítés mértéke évente $50 000). A foglalás megszakítása lehetővé teszi, hogy az ügyfél egy korai lemondási díj után visszaállítsa egy Azure-foglalás hátralévő hónapjának összegét. A fennmaradó arányban elszámolt egyenleg, amely mínusz a korai lemondási díj, visszakerül a fiókjába, így visszatéríthető az ügyfél fiókja. 

A lemondási részletekért és a díjakért lásd alább.


|**Lemondási dátum**<br> nap   |**Használat**    |**Kredit**  |**Korai befejezés**<br> díj    |**Visszatérítési korlát** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 vagy kevesebb                         | Nem          | 100%       | Nem                              | $50 000 USD   |
|5 vagy kevesebb                         | Igen         | Pro-rated  | Nem                              | $50 000 USD   |
|Több mint 5                        | Nem          | Pro-rated  | 12%                             | $50 000 USD   |
|Több mint 5                        | Igen         | Pro-rated  | 12%                             | $50 000 USD   |

### <a name="how-exchanges-work"></a>A cserék működése 

Ha az ügyfél az eredetileg vásárolttól eltérő foglalást szeretne vásárolni, kérheti az Exchange-t. A foglalások cseréje vonzó alternatíva lehet a foglalás megszakítására, mivel lehetővé teszi az ügyfél számára, hogy az új foglalás díja felé az arányosan megadott visszatérítést használja. 

Az arányos visszatérítés összegét a rendszer jóváírja a fiókjához, így az ügyfélnek Exchange-et is biztosíthat.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Visszatérítés vagy Exchange kérése az ügyfél nevében

Ha támogatási kérést szeretne benyújtani az ügyfelek nevében a visszatérítéshez vagy az Exchange-hez, válassza ki az ügyfelet és a foglalást a partner Centerben, majd hozza létre a támogatási kérelmet a Azure Portal. 

>[!NOTE]
>Microsoft ügyfélszolgálata ügynökök kérhetik a foglalási azonosító és a foglalási sorrend AZONOSÍTÓjának megadását. Ezeket az információkat a Azure Portal a foglalás **tulajdonságlapján** találja.

1. Első lépésként válassza ki az **ügyfelek** lehetőséget a partner Center menüben, majd válassza ki azt az ügyfelet, aki visszatérítést szeretne kapni. 

2. Az ügyfél részletei lapon válassza az Azure- **foglalások** lehetőséget, majd válassza ki azt az adott foglalást, amelyet az ügyfél szeretne visszatéríteni.  

3. A **műveletek** területen válassza a **visszatérítés** lehetőséget, hogy az ügyfél foglalási rekordjára lépjen a Azure Portal és kezdeményezzen egy támogatási kérést.  

4. Az **új támogatási kérelem** oldalon hajtsa végre az alábbi lépéseket a visszatérítés igényléséhez. Az egyes lépések után válassza a **tovább** lehetőséget. 

   |**Lépés**                    |**Kijelölések**    |
   |:---------------------------|:-----------------|
   |**1 alapismeretek**                |Probléma típusa: számlázás.  |
   |**2 probléma**               |Probléma típusa: fenntartások kezelése. Kategória: cserék és visszatérítések. |
   |**3 kapcsolattartási adatok**   |Válassza ki a beállításokat, és adja meg a szükséges adatokat. 

5. Ha elkészült, válassza a **Létrehozás** lehetőséget.

## <a name="azure-reservations-resources"></a>Azure-foglalások erőforrásai

|**További információ**   |**Olvassa el ezt**    |
|:-----------------------------|:-----------------|
|Azure-foglalások a CSP-ben – áttekintés  | [Microsoft Azure fenntartott példányok eladása](azure-reservations.md) |
|Azure-foglalások vásárlása az ügyfelek számára a partner Centerben   | [Azure-foglalások vásárlása](azure-reservations-buying.md) |
|A virtuális gép megfelelő méretének meghatározása és az ügyfél virtuális gépek használatának ellenőrzése   | [Virtuális gép méretezése az Azure-foglalások maximális használatára](azure-usage.md)   |
|Azure-foglalások vásárlása a partner Center API használatával | [Vásárlás Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) a partner Center fejlesztői dokumentációjában   |
|Lehetővé teszi, hogy az ügyfelek megvásárolják saját Azure-foglalásait a számukra megvásárolt előfizetésből. | [Engedélyt ad az ügyfeleknek a saját Azure-foglalások megvásárlására](give-customers-permission.md)   |