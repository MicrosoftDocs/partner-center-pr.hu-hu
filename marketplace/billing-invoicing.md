---
title: Számlázás és számlázás Azure Marketplace ügyfelek számára
description: Ez a cikk az ügyfelek számlázására és számlázására vonatkozó gyakori Azure Marketplace ismerteti.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 05/04/2021
ms.openlocfilehash: 6fdbbf9ad2b31e2b61eec20193717f60dd8e199a
ms.sourcegitcommit: b6959846c30d062d05028c9b4ba14c07e903e61a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/25/2021
ms.locfileid: "112970191"
---
# <a name="azure-marketplace-billing-and-invoicing"></a>Azure Marketplace számlázás és számlázás

Ez a cikk az ügyfelek számlázási és számlázási Azure Marketplace ismerteti.

## <a name="microsoft-supports-multiple-currencies"></a>A Microsoft több pénznemet is támogat

Azure Marketplace ajánlatok ára és számlázása az alábbi 17 pénznemben történt:

- Ausztrál dollár (AUD)
- Brazíliai real (BRL)
- Angol font (GBP)
- Kanadai dollár (CAD)
- Kínai yuan (CNY)
- Dán nyelv (DKK)
- Euro (EUR)
- Indiai rúpia (INR)
- Japán yen (JPY)
- Koreai won (KRW)
- Új-zélandi dollár (NZD)
- Norvég norvég (NOK)
- Orosz nyelv (FOG)
- Svéd nyelv (SEK)
- Német francia (CHF)
- Tajvani dollár (TWD)
- Amerikai dollár (USD)

## <a name="billing"></a>Számlázás

Az ismétlődő vásárlások után abban az időszakban kell fizetni, amelyben megvásárolta. Ezek a díjak az adott naptári hónap számláján jelennek meg. A következő időszakban az eredeti vásárlás napján automatikusan újra meg fognak újodni.

[![Példa a havi és éves rendszeres vásárlások számlázásának ütemterve.](media/billing/billing-charges-recurring.png)](media/billing/billing-charges-recurring.png#lightbox)

>[!NOTE]
> A szolgáltatási időszak az az időszak, amelyért a szolgáltatás használatára fizetett. A rendszer automatikusan megújítja a szolgáltatást a és a időszakban, kivéve, ha korábban megszakítja a műveletet.

> [!NOTE]
> Módosítjuk a számlázási adatokat (vagy a számlázási hónap utolsó napját), ha a megújítási hónap dátuma nem egyenlő a vásárlás hónap dátumával. Ez azt jelenti, hogy ha valaki 1/31-én fizet elő, a számlázási záró dátum 2/27-re módosul, a megújítási dátum pedig 2/28 (2/28, illetve 2/29, ha egy ugróévben kezdődik).

## <a name="invoices"></a>Számlák

Minden naptári hónap elején kap egy e-mailt, amikor a számla elérhető a Azure Portal. A számla a naptári hónap során megvásárolt és/vagy felhasznált összes ingyenes és fizetős ajánlatot mutatja. Ha csak ingyenes ajánlata van, csak 0 dollár sorelemeket lát, és nem kell semmilyen fizetési műveletet eltennünk. **Nagyvállalati Szerződés ügyfelek** összevont számlát kapnak, amely az Azure- és Azure Marketplace-díjakat is tartalmazza (kivéve az ausztráliában, Japánban és Szingapúrban található ügyfeleket). **A közvetlenül a Azure Marketplace** ügyfelek csak a vásárlásokért Azure Marketplace számlát kapnak. Részletekért lásd: [MosP-fiókok számlái.](/azure/cost-management-billing/understand/download-azure-invoice#invoices-for-mosp-billing-accounts)

Amikor megkapja a számlát, az változó:

- Ha a fizetési eszköz hitelkártyás, a foglalás megvásárlása után azonnal ki lesz számlázva. Ez a számla elkülönül a havi számlájától.
- Ha a fizetési eszköz csekkes/átutalásos, a vásárlás szerepelni fog a havi Marketplace-számlán.

Ez lehet a Microsoft Online Services Program (MOSP), Microsoft-ügyfélszerződés (MCA) vagy Microsoft-partnerszerződés (MPA) számlázási fiókja. A számlák a számlázási fiók típusa alapján generálnak. Azure Marketplace a számlázási időszak vége után néhány nappal számlás. A virtuális Azure Marketplace, foglalások és spot virtuális gépek számlái a hónap [9.](/azure/cost-management-billing/understand/download-azure-invoice#invoices-for-mosp-billing-accounts)napján jönnek létre. Az előző hónap vonatkozó díjait jeleníti meg. Ha például egy felhasználó március 1-jén vásárolt foglalást, és március 30-án vásárolt egy másik foglalást, egyetlen áprilisi számla tartalmazza mindkét foglalást.

A számlákkal kapcsolatos további információkért lásd az [Azure külső szolgáltatási díjának az azure-beli külső szolgáltatásokra vonatkozó díjszabását.](/azure/cost-management-billing/understand/understand-azure-marketplace-charges)

## <a name="next-steps"></a>Következő lépések

- [Mi az Azure Marketplace?](azure-marketplace-overview.md)
- [Azure Marketplace vásárlás](azure-purchasing-invoicing.md)
