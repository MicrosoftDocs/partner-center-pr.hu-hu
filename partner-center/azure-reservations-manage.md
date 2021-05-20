---
title: Azure Reservations kezelése ügyfelek számára
description: Megtudhatja, hogyan kezelheti egy ügyfél Azure-foglalását, beleértve a foglalás lemondását, a foglalás cseréjét vagy a visszatérítés kérelmezését.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 1184b199d6235dd1d16fe981000bae44b797f76a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149485"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Foglalások kezelése, lemondása, cseréje vagy visszatérítése Microsoft Azure ügyfelek számára

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Globális rendszergazdai | Az | Értékesítési ügynök | Felhasználókezelő rendszergazda

Ez a cikk azt ismerteti, hogyan kezelheti egy ügyfél Azure-foglalását, beleértve a foglalás lemondását, a foglalás cseréjét vagy a visszatérítés kérelmezését.

> [!NOTE]
> Ez a cikk csak a Felhőszolgáltató (CSP) program partnereire vonatkozik. A más típusú előfizetéseket (például használat alapján fizetett, egyéni, Microsoft Ügyfélszerződés- vagy Nagyvállalati Szerződés-előfizetéseket) használó ügyfeleknek érdemes elolvasni az [Azure Reservations dokumentációját.](/azure/cost-management-billing/reservations)

Az ügyfelek Azure Reservations-foglalásának vásárlás utáni kezeléséhez ki kell választania a Partnerközpont-ban kezelni kívánt ügyfelet és foglalást, majd a foglalást a Azure Portal.

1. Első lépésekként válassza az **Ügyfelek** Partnerközpont menüből, majd válassza ki azt az ügyfelet, akinek a foglalását kezelni szeretné. 

2. Az ügyfél részletek oldalmenüjében válassza az **Azure Reservations** lehetőséget, majd válassza ki a kezelni kívánt foglalást.  

3. A **Műveletek alatt** válassza a **Kezelés** lehetőséget az ügyfél foglalási rekordját a Azure Portal. A foglalás részletei lapon kövesse az alábbi lépéseket a feladatok végrehajtásához.  

    | **Kiválasztás**   | **Ide:**    |
    |:-----------------------------|:-----------------|
    | **Áttekintés**   | Megtekintheti az ügyfél foglalásának részleteit, beleértve a lejárati dátumot, a hatókört és a kihasználtsági adatokat. **MEGJEGYZÉS** Válassza **a Visszatérítés** lehetőséget, hogy támogatási kérést hozzon létre egy pro-rated visszatérítéshez. Válassza **az Exchange** lehetőséget, és hozzon létre egy támogatási kérést a foglalási időszak fel nem használt részének cseréjéhez.  
    | **Access Control (IAM)**   | Kezelheti az ügyfél foglalási információihoz való hozzáférést.|
    | **Konfigurálás**   | Módosítsa a foglalás hatókörét és/vagy azt az Azure-előfizetést, amelyhez a foglalás társítva van.    |
    | **Tulajdonságok**   | Tekintse meg a foglalás tulajdonságait, és másolja a vágólapra a foglalás azonosítóját és a foglalási rendelés azonosítóját. **MEGJEGYZÉS** A támogatás kérheti a foglalásazonosítót és a foglalásrendelés azonosítóját, amikor támogatást kér egy ügyfél nevében.    |
    | **Új támogatási kérelem**    | Kérjen segítséget a Microsoft ügyfélszolgálata.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Foglalás lemondása vagy cseréje

Ha az ügyfél üzleti igényei bármikor megváltoznak, előfordulhat, hogy le szeretné mondani a foglalást, és visszatérítést szeretne kapni, vagy le szeretné cserélni a foglalás időkorreált visszatérítési összegét, hogy az új foglalás árát ki tudják használni.

Mindkét esetben a Microsoft visszatérítést ad vissza Önnek, így Ön kezelheti az ügyfelekkel az eredményül kapott pénzügyi tranzakciókat. A Microsoft nem lép kapcsolatba közvetlenül az ügyfelekkel a számlázással, lemondásokkal vagy visszatérítésekkel kapcsolatban.

### <a name="how-cancellations-work"></a>A lemondások hogyan működnek

Az ügyfelek bármikor kérhetik a foglalás lemondását (a visszatérítés összege évente 50 000 dollár). A foglalás lemondása lehetővé teszi, hogy az ügyfél egy korai felmondási díjért visszatérjen az Azure-foglalás fennmaradó hónapjaiból. A fennmaradó, idő előtti felmondási díj nélkül fennmaradó időkorlátot a fiókba térítjük vissza, így Ön visszatérítést kérhet az ügyfél fiókjáért. 

A lemondási adatokat és a díjakat lásd alább.


|**Lemondás dátuma**<br> (nap)   |**Használat**    |**Kredit**  |**Korai felmondás**<br> Díj    |**Visszatérítési felső összeg** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 vagy kevesebb                         | No          | 100%       | No                              | 50 000 USD   |
|5 vagy kevesebb                         | Yes         | Pro-rated (Pro-rated)  | No                              | 50 000 USD   |
|Több mint 5                        | No          | Pro-rated (Pro-rated)  | 12%                             | 50 000 USD   |
|Több mint 5                        | Yes         | Pro-rated (Pro-rated)  | 12%                             | 50 000 USD   |

### <a name="how-exchanges-work"></a>A cserék a munka során 

Ha egy ügyfél más foglalást szeretne vásárolni, mint amelyet eredetileg vásárolt Öntől, cserét kérhet. A foglalás cseréje vonzó alternatíva lehet a foglalás lemondása ellenében, mivel lehetővé teszi az ügyfél számára, hogy a visszatérítések összegét az új foglalás árában használja fel. 

Az időkorreklált visszatérítési összeg az Ön fiókjához lesz jóvá keretve, így cserét kínálhat fel az ügyfélnek.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Visszatérítés vagy csere kérése az ügyfél nevében

Ha visszatérítésre vagy cserére vonatkozó támogatási kérést kell bejelítenie az ügyfelek nevében, ki kell választania az ügyfelet és a foglalást az Partnerközpont-ban, majd létre kell hoznia a támogatási kérést a Azure Portal. 

>[!NOTE]
>Microsoft ügyfélszolgálata ügynök megkérheti, hogy adja meg a foglalás azonosítóját és a foglalási rendelés azonosítóját. Ezt az információt a foglalás  Tulajdonságok oldalán találja a Azure Portal.

1. Első lépésekként válassza **az** Ügyfelek lehetőséget Partnerközpont menüből, majd válassza ki azt az ügyfelet, aki visszatérítést szeretne. 

2. Az ügyfél részletek lapján válassza az **Azure Reservations** lehetőséget, majd válassza ki azt a foglalást, amelyért az ügyfél visszatérítést szeretne igényelni.  

3. Az **Actions (Műveletek)** alatt válassza a **Refund** (Visszatérítés) lehetőséget, hogy az ügyfél foglalási rekordját a Azure Portal kezdeményezze a támogatási kérést.  

4. Az Új **támogatási kérelem oldalon** kövesse az alábbi lépéseket a visszatérítés igénylése érdekében. Minden **lépés után** válassza a Tovább lehetőséget. 

   |**Lépés**                    |**Kiválasztás**    |
   |:---------------------------|:-----------------|
   |**1. Alapok**                |Probléma típusa: Számlázás.  |
   |**2. Probléma**               |Probléma típusa: Foglaláskezelés. Kategória: Cserék és visszatérítések. |
   |**3 Kapcsolattartási adatok**   |Válassza ki a beállításokat, és adja meg a szükséges adatokat. 

5. Ha **végzett,** válassza a Létrehozás lehetőséget.

## <a name="azure-reservations-resources"></a>Azure Reservations-erőforrások

|**További információ:**   |**Olvassa el ezt**    |
|:-----------------------------|:-----------------|
|Azure Reservations a CSP-ban – áttekintés  | [Fenntartott Microsoft Azure értékesítés](azure-reservations.md) |
|Azure-foglalások vásárlása az ügyfelek számára Partnerközpont   | [Azure Reservations vásárlása](azure-reservations-buying.md) |
|A megfelelő virtuálisgép-méret meghatározása és az ügyfél virtuálisgép-használatának ellenőrzése   | [Virtuális gép méretezése az Azure-beli foglalások maximális kihasználtságában](azure-usage.md)   |
|Azure-foglalások vásárlása a Partnerközpont API-val | [Vásárlási Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) az Partnerközpont fejlesztői dokumentációjában   |
|Engedélyt ad az ügyfeleknek arra, hogy megvásárolják saját Azure-foglalásukat egy számukra megvásárolt előfizetésből. | [Engedélyt adhat az ügyfeleknek a saját Azure-foglalásaik vásárlásra](give-customers-permission.md)   |