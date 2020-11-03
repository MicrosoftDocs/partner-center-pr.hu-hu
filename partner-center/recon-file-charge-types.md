---
title: Egyeztetési felszámított fájlok típusai
ms.topic: article
ms.date: 06/05/2020
description: Fedezze fel a (például licenc-alapú, használati és egyszeri), kreditek és kedvezmények típusát a partner Center egyeztetési fájljaiban.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/31/2020
ms.locfileid: "92528061"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>A különböző díjszabási típusok ismertetése a partner Center egyeztetési fájljaiban

**A következőkre vonatkozik**

- Partnerközpont
- Az USA kormányzati szerveinek Microsoft Cloud a partneri központ

**Megfelelő szerepkörök**

- Felügyeleti ügynök
- Számlázási adminisztrátor
- Globális rendszergazda

Ez a témakör a számla szakasz és a társított díjszabási típusok közötti leképezéseket ismerteti, amelyek lehetnek a megbékélési fájlban. A számla a díjak összegzését tartalmazza. Az egyeztetési fájl részletesen részletezi a line-Item tranzakciókat, beleértve a díjszabási típusokat is. Az egyeztetési fájlokkal kapcsolatos további információkért lásd: [a megbékélési fájlok használata](use-the-reconciliation-files.md).

A [használaton alapuló egyeztetési fájlok](usage-based-recon-files.md) és a [licenc-alapú egyeztetési fájlok](license-based-recon-files.md) csak a használattal kapcsolatos tranzakciókat és díjakat (a felhasznált egységek és a kapcsolódó díjak) mutatják.

> [!NOTE]
> A számlán megjelenő egyszeri kreditek, kedvezmények vagy visszatérítések nem jelennek meg az egyeztetési fájlban. **Adjustments**

## <a name="map-charge-types-to-invoice-charges"></a>Vegyesköltség-típusok hozzárendelése a számlázáshoz

A számla és a megbékélési fájl közötti Összevetéshez használja a Microsoft Excelben a szűrési lehetőségeket. Az egyeztetési fájlban lévő vegyesköltség-típusok alapján szűkítse a számla díját a visszaegyeztetési fájlban lévő vegyesköltség-részletezési csoportba.

## <a name="license-based-charges"></a>Licenc-alapú díjak

Ha ezeket a licencfeltételeket szeretné feltérképezni a számlán, a licenc-alapú fájl **összeg** oszlopát adja meg.

| Díj leírása (ChargeType oszlop az egyeztetési fájlban) | Díj magyarázata |
| ------------------------------------------------------------- | ------------------ |
| Aktiválási díj | Az ügyfélnek a vásárlás után az előfizetés használatakor felszámított összeg. |
| Megszakított díj | A hozzárendelt licencek megváltozásakor a rendszer visszafizeti az előfizetést az ügyfélnek. |
| Példány-arány megszakítása | Az elszámolási díjak megszakadtak, ha a havi előfizetéssel rendelkező ügyfél felfüggesztette az előfizetést, és a társított licencek egy hónapon belül változnak |
| Ciklus díja | Egy előfizetés rendszeres díjai. |
| Ciklus példányának gyakorisága | Az ügyfél által a társított licencek megváltozásakor kiértékelt arányban elszámolt díjak. |
| A megszakítás díja | A szolgáltatás fel nem használt részének elszámolási aránya a lemondás után. |
| Az aktuális ajánlatból való áttéréskor felmerülő díjak | Arányos díjak az aktuális havi előfizetésből egy éves előfizetésre való áttérés után. |
| Az új ajánlatra való áttéréskor felmerülő díjak | A havi előfizetés új éves előfizetésre való konvertálása után eltelt díjak. |
| Díjszabási díjak a vásárláskor | Az előfizetés díja, ha havi vagy éves számlázást is használ. |
| A megújítás díjszabása | Az Előfizetés megújítása után elszámolt díjak. |
| Megújítás díja | Előfizetés megújításának díja |
| Díjszabási díjak aktiváláskor | Elszámolási díjak az aktiválástól egészen a számlázási időszak végéig. |

## <a name="one-time-charges"></a>Egyszeri díj

Ha ezeket az egyszeri díjakat szeretné leképezni a számlára, akkor a licenc-alapú fájl **összeg** oszlopát adja meg.

| Díj leírása (ChargeType oszlop az egyeztetési fájlban) | Díj magyarázata |
| ------------------------------------------------------------- | ------------------ |
| Új | Új vásárlás létrehozásakor használatos. |
| addQuantity | Az eredeti vásárlás és az új mennyiség visszatérítése után is használatos. |
| removeQuantity | Az eredeti vásárlás visszatérítésében és az új mennyiség csökkenése után is használatos. |
| Mégse | Előfizetés megszakadása esetén használatos. |
| Konvertálás | A licenc frissítésekor használatos, de a licencek száma változatlan marad. |

## <a name="usage-charges"></a>Használati díjak

A használati díjaknak a számlára való hozzárendeléséhez a **PretaxCharges** oszlopot a használaton alapuló fájlból kell összegezni.

| Díj leírása (ChargeType oszlop az egyeztetési fájlban) | Díj magyarázata |
| ------------------------------------------------------------- | ------------------ |
| Használati díj kiértékelése megszakításkor | Az aktuális számlázási időszakban a nem fizetett használat megszüntetésére vonatkozó hozzáférési díj. |
| A jelenlegi ciklus használati díjának felmérése | Az aktuális számlázási időszakhoz való hozzáférés használati díja. |

### <a name="credits"></a>Kreditek

A kreditek hozzárendelése a számlához:

- Adja meg a **TotalForCustomer** a licenc-alapú fájlból.
- A **PostTaxTotal** oszlop összege a használaton alapuló fájlból.

| Díj leírása (ChargeType oszlop az egyeztetési fájlban) | Díj magyarázata |
| ------------------------------------------------------------- | ------------------ |
| Egy tétel eltolása | Részleges vagy teljes visszatérítés egy sorra, beleértve az adókat is. |

### <a name="usage-based-discounts"></a>Használati alapú kedvezmények

A használati alapú kedvezmények a számlára való hozzárendeléséhez a **PretaxCharges** oszlopot a használaton alapuló fájlból kell összegezni.

| Díj leírása (ChargeType oszlop az egyeztetési fájlban) | Díj magyarázata |
| ------------------------------------------------------------- | ------------------ |
| Aktiválási kedvezmény | Az előfizetés aktiválása esetén érvényes kedvezmény. |
| Ciklus kedvezménye | Az időszakos költségekre alkalmazott kedvezmény. |
| Kedvezmény megújítása | Az előfizetés megújításakor alkalmazott kedvezmény. |
| Kedvezmény lemondása | A kedvezmények megszakításakor alkalmazott díjak. |

### <a name="license-based-discounts"></a>Licenc-alapú kedvezmények

A licenc-alapú kedvezmények a számlára való leképezéséhez adja a **TotalOtherDiscount** oszlopot a licenc-alapú fájlból.

*A licenc-alapú kedvezmények több feltöltési típusra is alkalmazhatók.*
