---
title: A számla olvasása & recon fájlban
ms.topic: article
ms.date: 06/05/2020
description: Ismerje meg a számla- és & fájlokat. A számla a Partnerközpont, termékek és ügyfelek teljes havi díjait jeleníti meg.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f16b619aba838da1d1da0c5eb13648ebb107c802
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855913"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>A számla és az egyeztetési fájl megismertetése – megtudhatja, hogyan találhatja meg őket a Partnerközpont


**Megfelelő szerepkörök:** Globális rendszergazdai | Számlázási rendszergazdai | Rendszergazdai ügynök


A **számla** a teljes számlázási **Partnerközpont** összegző (a programban, az összes termékben és az összes ügyfélben). 

## <a name="find-your-bill-and-reconciliation-file"></a>Keresse meg a számla- és egyeztetési fájlt 

A számlát az irányítópult Számlázás lapján találja a Partnerközpont. Ezen az oldalon a számlázási előzményeket, a költési trendeket és az egyeztetési fájlokat is megtalálja. 

1. Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard/home) 

2. A bal oldali menüben válassza a Számlázás **lehetőséget.** 

3. A számlázási állapot oldalán válassza ki a számlát vagy az egyeztetési fájlt a részletesebb információk megtekintéséhez. 

A legutóbbi számlára mutató hivatkozást az oldal tetején, a Számlaegyenleg az utolsó számla dátuma alatt találja. 

A korábbi számlákat a Számlázási előzmények szakaszban találja. Válassza ki a megfelelő évet, majd kattintson a megfelelő számlázási időszak melletti legördülő nyílra. Válassza a Számlák (.pdf) melletti hivatkozást az időszakhoz tartozó számla letöltéséhez. 

## <a name="invoice-types"></a>Számlatípusok

A Microsoft egy számlát ad ki az esetleges licencalapú díjakról (például az Office 365-ről) és a használatalapú díjakról (például az Azure-ról), valamint egy külön számlát az egyszeres díjakról (például Azure RI, Marketplace vagy Azure-csomag).

Példa:  

**1. forgatókönyv [Egyetlen pénznem]**: A partner 145P-ajánlathoz és O365-licenchez rendelkezik vásárlásokkal,  

- A partner egy pdf formátumú számlát és 2 egyeztetési fájlt kap, amelyek az O365 és az Azure díjának (145p) költségeit fedezik.  

**2. forgatókönyv [Egyetlen pénznem]**: A partner 145p vásárlással együtt vásárol az Azure-beli RI-hez, a Marketplace-hez és/vagy az Azure-csomaghoz.

- A partner kap egy PDF-formátumú számlát és egy egyeztetési fájlt, amely az Azure költségeit fedezi (145p). 

- A partner egy másik számla PDF-fájlt és egy egyeztetési fájlt kap, amely az Azure RI, Marketplace, Azure-csomag díjára vonatkozó költségeket fedezi. 

**3. forgatókönyv :A** partner megvásárolta az Azure RI-t DKK-ban és az Azure-csomaghoz EUR-ban, valamint 145p vásárlást EUR-ban.

- A partner kap egy PDF formátumú számlát és egy egyeztetési fájlt, amely az Azure RI DKK-ban való költségeit fedezi. 

- A partner kap egy PDF formátumú számlát és egy egyeztetési fájlt, amely az Azure-csomag díjának összegét (EUR) fedezi. 

- A partner kap egy másik számla PDF-fájlt és egy egyeztetési fájlt, amely a 145p-es ajánlat díját fedezi EUR-ben (vagy a partner számlázási pénznemében). 


## <a name="understanding-invoice-pdf"></a>A számla PDF-fájlja 

**Használati és** licencalapú díjak számlái: Az olyan szolgáltatások díjára vonatkozó számlák, mint az Office 365 és az Azure, a kiválasztott számlázási dátumtól számított két (2) napon belül lesznek elérhetők [UTC].  

**Egyszeri és ismétlődő** díjak számlái: Az olyan szolgáltatások díjára vonatkozó számlák, mint az Azure RI, az Azure-csomag és a Marketplace, legkésőbb minden hónap 8. napján lesznek elérhetők.  

Az alábbiakban a számla PDF-dokumentumának néhány fő mezőjét olvashatja–

**Számlaszám:** A megfelelő számlázási időszakhoz létrehozott számladokumentum egyedi azonosítója. 

**Számlázási időszak:** Ez az az időszak, amelyben használat és licencalapú szolgáltatások vannak. 

**Számla dátuma:** Az a számlázási dátum vagy évforduló, amelyen a számla minden hónapban létrejön. 

**Fizetési határidő:** Az a dátum, amely szerint a kifizetést át kell fizetni. 

**Díjak:** Az adott számlázási időszak számlázási pénznemében esedékes összeg. 

**Kreditek:** Kreditek (például SLA) vagy az előfizetések módosításainak (például a licenc növekedésével vagy csökkenésével) kapcsolatos módosítások. 

**Fizetési utasítások:** A számla kifizetésének leírása a régiója alapján. A fizetéskor mindig foglalja bele a számlaszámot. 

A számlafájl összes mezőjének részletes leírását (az egyszeres díjak mezőit is beleértve) lásd: [Számlafájlmezők.](invoice-file.md) 

## <a name="understand-reconciliation-files"></a>Egyeztetési fájlok

 Az egyeztetési fájlok, amelyek részletes információkat érhetők el a díjakról, letölthetők a számla PDF-fájljával együtt. Az egyeztetési fájlok között ügyfél-azonosítók és előfizetés-azonosítók is vannak, amelyek segítségével ügyfélszámlákat hozhat létre. A felderítési  [fájlokkal kapcsolatos](use-the-reconciliation-files.md) további részletekért tekintse meg az egyeztetési fájlok használatát. 

## <a name="next-steps"></a>Következő lépések

- [Az egyeztetési fájlok használata](use-the-reconciliation-files.md)