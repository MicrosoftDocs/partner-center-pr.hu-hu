---
title: Egyeztetési fájlok díjtípusai
ms.topic: article
ms.date: 06/05/2020
description: Megismerheti a díjtípusokat (például licencalapú, használatalapú és egyszeres), krediteket és kedvezményeket az egyeztetési Partnerközpont fájlokban.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855879"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Az egyeztetési fájlokban található különböző Partnerközpont típusainak

**A következőkre vonatkozik:** Partnerközpont | Partnerközpont a Microsoft Cloud for US Government

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Globális rendszergazda

Ez a cikk a számlaszakaszok és a társított díjtípusok közötti leképezéseket ismerteti, amelyek az egyeztetési fájlban lehetnek. A számla a díjak összegzését biztosítja. Az egyeztetési fájl részletesen részletezi a sortétel-tranzakciókat, beleértve a díjtípusokat is. Az egyeztetési fájlokkal kapcsolatos további információkért lásd az egyeztetési [fájlok használatát.](use-the-reconciliation-files.md)

Mind [a használatalapú egyeztetési](usage-based-recon-files.md) fájlok, mind a licencalapú egyeztetési fájlok [csak](license-based-recon-files.md) a használattal kapcsolatos tranzakciókat és díjakat (felhasznált egységeket és kapcsolódó díjakat) mutatják.

> [!NOTE]
> A számlán a Helyesbítésekként megjelenő egyszeres jóváírások, kedvezmények vagy visszatérítések nem jelennek meg az egyeztetési fájlban. 

## <a name="map-charge-types-to-invoice-charges"></a>Díjtípusok leképezés a számlás díjakra

A díj összegeinek a számla és az egyeztetési fájl közötti kereszthivatkozáshoz használja a Microsoft Excel szűrési lehetőségeit. Szűrhet díjtípusok szerint az egyeztetési fájlban, hogy a számlázási díjakat leképezheti az egyeztetési fájlban található költséglebontások készletére.

## <a name="license-based-charges"></a>Licencalapú díjak

Ezeknek a licencalapú díjaknak a számlán való leképezésén a **licencalapú** fájl Amount oszlopát összegezve kell összeadni.

| Díj leírása (ChargeType oszlop az egyeztetési fájlban) | Díj magyarázata |
| ------------------------------------------------------------- | ------------------ |
| Aktiválási díj | Az ügyfélnek a vásárlást követően az előfizetés használata után felszámított összeg. |
| Lemondási díj | Az ügyfélnek a társított licencek módosult díjának megfelelő visszatérítésekért. |
| Példány-prorate megszakítása | A havi előfizetéssel rendelkező ügyfél előfizetésének felfüggesztése és a társított licencek ugyanabban a hónapban való módosult időszakában az időszakra vonatkozó, az időszakra vonatkozó díjakat az időszakban megszüntetjük. |
| Ciklus díja | Az előfizetések rendszeres díjai. |
| Ciklikus példány-prorate | Az ügyféltől származó, a társított licencek módosulásával kapcsolatos, az igényeknek megfelelő díjakat kell megállapítani. |
| Díjfizetési díjak lemondáskor | A szolgáltatás fel nem használt részének időkorrekét visszatérítése lemondáskor. |
| Az aktuális ajánlatról való átváltás díjai | Az aktuális havi előfizetésről egy éves előfizetésre való átváltás után az időkorreklott díjak. |
| Az új ajánlatra való átváltás díjai | A havi előfizetés új éves előfizetésre való átváltása után fizetendő díjak. |
| Díjfizetés vásárláskor | Az előfizetés díjtípusa havi vagy éves számlázás esetén is. |
| Megújítás után fizetendő díj | Az előfizetés megújítása után fizetendő díjak. |
| Díj megújítása | Előfizetés megújításának díj |
| Az aktiválás díjai | Az aktiválástól a számlázási időszak végéig fizetendő díjak. |

## <a name="one-time-charges"></a>Egyszer fizetendő díjak

Ha ezeket az egyszeres díjakat le kell leképezni a számlájára, összegezve a licencalapú fájl **Amount** (Összeg) oszlopát.

| Díj leírása (ChargeType oszlop az egyeztetési fájlban) | Díj magyarázata |
| ------------------------------------------------------------- | ------------------ |
| Új | Új vásárlás létrehozásakor használatos. |
| addQuantity (Hozzáadásquantitás) | Az eredeti vásárlás visszatérítésében és az új mennyiségben is felhasználható a növekedés után. |
| removeQuantity (Quantity eltávolítása) | Az eredeti vásárlás visszatérítésében és az új mennyiségben is felhasználható a csökkenést követően. |
| Mégse | Az előfizetés lemondása esetén használatos. |
| Konvertálás | Akkor használatos, ha a licenc frissítve van, de a licencek száma változatlan marad. |

## <a name="usage-charges"></a>Használati díjak

Ezeknek a használati díjaknak a számlán való leképezésén a Használatalapú fájl **PretaxCharges** oszlopát összegezve kell összeadni.

| Díj leírása (ChargeType oszlop az egyeztetési fájlban) | Díj magyarázata |
| ------------------------------------------------------------- | ------------------ |
| Használati díj értékelése lemondáskor | A ki nem fizetett használat lemondása után a jelenlegi számlázási időszakra vonatkozó használati díj elérése. |
| A jelenlegi ciklus használati díjának felmérése | Az aktuális számlázási időszak használati díjának elérése. |

### <a name="credits"></a>Kreditek

A kreditek a számlán való leképezésén a következőt kell látni:

- Összegezve **a TotalForCustomer a** licencalapú fájlból.
- Összegezve **a PostTaxTotal** oszlopot a használatalapú fájlból.

| Díj leírása (ChargeType oszlop az egyeztetési fájlban) | Díj magyarázata |
| ------------------------------------------------------------- | ------------------ |
| Sorelem eltolása | Részleges vagy teljes visszatérítés egy sortételre, az adókkal együtt. |

### <a name="usage-based-discounts"></a>Használatalapú kedvezmények

Ezeknek a használatalapú kedvezményeknek a számlán való leképezésén a Használatalapú fájl **PretaxCharges** oszlopát összegezve adatokat kaphat.

| Díj leírása (ChargeType oszlop az egyeztetési fájlban) | Díj magyarázata |
| ------------------------------------------------------------- | ------------------ |
| Aktiválási kedvezmény | Az előfizetés aktiválásakor alkalmazott kedvezmény. |
| Ciklusra kedvezményes | Az időszakos díjakra alkalmazott kedvezmény. |
| Kedvezmény megújítása | Az előfizetés megújításakor alkalmazott kedvezmény. |
| Kedvezmény lemondása | A kedvezmények törlésekor alkalmazott díjak. |

### <a name="license-based-discounts"></a>Licencalapú kedvezmények

Ha licencalapú kedvezményeket kell leképezni a számlára, összesítenünk kell a **TotalOtherDiscount** oszlopot a licencalapú fájlból.

*A licencalapú kedvezmények több díjtípusra is alkalmazhatók.*
