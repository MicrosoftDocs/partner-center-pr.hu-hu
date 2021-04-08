---
title: A Bill & Recon-fájl beolvasása
ms.topic: article
ms.date: 06/05/2020
description: További információ a számla & egyeztetési fájlokról. A számlán az adott havi időszakra vonatkozó, a programon, a termékeken és az ügyfeleknek felszámított partneri költségek szerepelnek.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e93bc59d4ddb8ac2323807a716d7ba6404b00fce
ms.sourcegitcommit: 58432bbb7eb0aed123547da65642ca728cb9b32c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/07/2021
ms.locfileid: "106964357"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>A számla és a megbékélési fájl megismerése – Ismerje meg, hogyan keresheti meg őket a partner Centerben


**Megfelelő szerepkörök**

- Globális rendszergazda
- Számlázási adminisztrátor
- Felügyeleti ügynök


A **számla** az **összes partner Center-díj** (a program, az összes termék és minden ügyfél) összefoglalása. 

## <a name="find-your-bill-and-reconciliation-file"></a>A számla és a megbékélési fájl megkeresése 

A számla a partner Center irányítópultjának számlázási lapján található. Ezen a lapon megtekintheti a számlázási előzményeit, a kiadások trendjét és a fájlok egyeztetését. 

1. Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard/home). 

2. A bal oldali menüben válassza a **számlázás** lehetőséget. 

3. A számlázási állapot oldalán válassza ki a számlát vagy az egyeztetési fájlt a részletesebb információk megtekintéséhez. 

Az oldal tetején található utolsó számlára mutató hivatkozást a számla egyenlege a legutóbbi számlázási dátum alapján lehetőségre kattintva találja. 

A korábbi számlákat a számlázási előzmények szakaszban találja. Válassza ki a megfelelő évet, majd válassza a megfelelő számlázási időszak melletti legördülő nyilat. Válassza a számlák melletti hivatkozást (. pdf) az adott időszak számlájának letöltéséhez. 

## <a name="invoice-types"></a>Számlák típusai

A Microsoft egy számlát ad ki a licenc-alapú díjak (például az Office 365) és a használati díjak (például az Azure) számára, valamint egy külön számlát az egyszeri költségek (például az Azure RI, a piactér vagy az Azure-csomag) számára.

Példa:  

**1. forgatókönyv [egyetlen pénznem]**: a partner 145P-ajánlatokat és O365-licenceket vásárol,  

- A partner egy számla PDF és 2 egyeztetési fájlt kap, amely a O365 és az Azure (145p) díjait is tartalmazza.  

**2. forgatókönyv [egyetlen pénznem]**: a partner az Azure RI, a piactér és/vagy az Azure-csomag megvásárlásával, valamint a 145p-vásárlásokkal is rendelkezik.

- A partner egy számla PDF-fájlját és egy egyeztetési fájlt kap, amely az Azure (145p) díjait tartalmazza. 

- A partner egy másik számla PDF-fájlját és egy egyeztető fájlt fog kapni, amely az Azure RI, a piactér és az Azure-csomag díjaira vonatkozik. 

**3. forgatókönyv [többszörös pénznem]**: a partner az Azure ri-t a DKK-ben és az Azure-ban, a 145p-vásárlások esetében pedig euróban vásárolja meg.

- A partner egy számla PDF-fájlját és egy egyeztető fájlt fog kapni, amely a DKK-ban található Azure RI díját tartalmazza. 

- A partner egyetlen számla PDF-fájlját és egy egyeztető fájlt kap, amely az Azure-csomag díjait tartalmazza EUR-ban. 

- A partner egy másik számla PDF-fájlját és egy egyeztetési fájlt fog kapni, amely az 145p ajánlat díjait (vagy a partner számlázási pénznemét) tartalmazza. 


## <a name="understanding-invoice-pdf"></a>A számla PDF-fájljának ismertetése 

**Használati és licenc-alapú díjakra vonatkozó számlák**: az Office 365-es és Azure-szolgáltatások díjainak számlázása két (2) napon belül elérhető lesz a kiválasztott számlázási dátum [UTC] alapján.  

**Egyszeri és ismétlődő díjakkal kapcsolatos számlák**: az Azure RI, az Azure-csomag és a piactér díjainak számlázása minden hónap 8. után lesz elérhető.  

Az alábbiakban a számla PDF-dokumentumának legfontosabb mezői találhatók:

**Számla száma**: a megfelelő számlázási időszakra vonatkozóan generált számla dokumentum egyedi azonosítója. 

**Számlázási időszak**: ez az az időszak, amely alatt a használati és a licenc-alapú szolgáltatásokat használhatja. 

**Számla dátuma**: az a számlázási dátum vagy évfordulós dátum, amikor a számla generálása havonta történik. 

**Fizetési** határidő: az a dátum, ameddig a fizetést meg kell kapni. 

**Díjak**: a megfelelő számlázási időszakra vonatkozó számlázási pénznemben esedékes összeg. 

**Kreditek**: kreditek (SLA) vagy az előfizetések módosításaira vonatkozó módosítások (például a licenc növekedése vagy csökkentése). 

**Fizetési utasítások**: a számla fizetésének leírása a régió alapján. A számla számát mindig adja meg a fizetéskor. 

A számlázási fájlban lévő összes mező részletes ismertetését (beleértve az egyszeri költségekkel kapcsolatos mezőket is) lásd: [számlasorok mezői](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Az egyeztetési fájlok ismertetése

 Az egyeztetési fájlok, amelyek részletezik és részletezik a díjak részleteit, letölthetők a számla PDF-fájljával együtt. Az egyeztetési fájlok közé tartoznak az ügyfél-azonosítók és az előfizetés-azonosítók, amelyeket az ügyfél-számlák létrehozásához használhat. A felderítési fájlokkal kapcsolatos további részletekért tekintse meg az  [egyeztetési fájlok használatát ismertető](use-the-reconciliation-files.md) témakört. 

## <a name="next-steps"></a>Következő lépések

- [A megbékélési fájlok használata](use-the-reconciliation-files.md)