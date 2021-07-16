---
title: Partnerközpont Elemzések Microsoft Learn elemzés
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Nyomon követheti vállalata tanulóit az egyéni betanításokkal, befejezett modulokkal, befejezett képzési programokkal és egyéb adatokkal.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d9f9ce631fe667030638e1a9167809e3dae69830
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114373864"
---
# <a name="use-microsoft-learn-analytics-reports"></a>Az Microsoft Learn-jelentések használata

**Megfelelő szerepkörök:** Globális rendszergazdai | MPN-partner rendszergazdája

A [Microsoft Learn](/learn/) jelentés információkat nyújt a vállalat tanulóiról, beleértve az eddig befejezett modulokat és a képzési útvonalakat. A jelentés megjeleníti az egyes tanulók állapotát. A vállalat globális rendszergazdái és MPN-rendszergazdái megtekinthetik az adatokat.

## <a name="how-to-read-the-report"></a>A jelentés olvasása

### <a name="summary-charts"></a>Összegző diagramok

Ezek a diagramok összegzi a szám- és havi kumulatív trendeket a betanított személyek, a modulok befejezései és a képzési útvonalak alapján.

**Betanított személyek száma:** Az összes olyan tanuló száma, aki legalább egy modult befejezett a kiválasztott dátumtartományban 

**Betanított személyek trend minidiagramja:** Az aktív tanulók havi összesített száma 

**Modul befejezési száma:** A partner vállalatának tanulói által a kiválasztott dátumtartományon belül végzett modul-befejezések száma.
Ha például az "1. modult" 15 személy, a "2. modult" pedig ugyanaz a 15 személy, akkor a modul befejezésének száma 30 lesz. A modul befejezési dátumának a kiválasztott dátumtartományba kell esni.

**Modul-befejezési trend minidiagram:** A modulok befejezésinek összesített száma havonta 

**Tanulás** elérésiút-kiegészítések száma: A Tanulás vállalat tanulói által a kiválasztott dátumtartományban végzett útvonal-befejezések száma.
Ha például az Tanulás Path 1 (1. út) útvonalat 20 személy, az Tanulás Path 2 útvonalat pedig ugyanaz a 20 személy haladta meg, akkor az Tanulás Path completion count (Az Tanulás elérési út befejezési száma) 40 lesz. A Tanulás elérési út befejezési dátumának a kiválasztott dátumtartományba kell esni.

**Tanulás útvonal kiegészítésének trendje minidiagram:** A képzési képzési útvonal befejezésének összesített száma hónapról hónapra 

### <a name="trained-individuals-monthly-trend"></a>Betanított személyek havi trendje

Ezek az adatok a vállalat felhasználóinak trendje, akik ebben a hónapban először fejezték be a modult. 

**Az X tengely a** kiválasztott időszűrő hónapja. 

**Az Y tengely** az aktív tanulók száma, akik az ebben a hónapban regisztráltak (egy modul első befejezésekor). Ez nem kumulatív.

### <a name="module-completions-monthly-trend"></a>Modul-befejezések havi trendje

Ezek az adatok a vállalat összes felhasználója által az ebben a hónapban befejezett modulok trendjét jelentik. (nem összesítve) 

**Az X tengely a** kiválasztott időszűrő hónapja. 

**Az Y tengely az** ebben a hónapban végzett modul-befejezéseket jelenti. Ez nem kumulatív.

### <a name="learning-path-completions-monthly-trend"></a>Tanulás útvonal kiegészítésének havi trendje

Ezek az adatok a vállalat felhasználói által az ebben a hónapban befejezett képzési útvonalak trendje. (nem összesítve) 

**Az X tengely a** kiválasztott időszűrő hónapja. 

**Az Y tengely az** abban a hónapban végzett modul-befejezések száma. Ez nem kumulatív.

### <a name="learning-path-completion-tabs"></a>Tanulás elérésiút-befejezési lapok használata

#### <a name="module-tab"></a>Modul lap

Ez a lap a vállalaton belül befejezett modulok lebontását tartalmazza az első öt modulnév alapján; az a termék, amelyhez a modul társítva van; és a modulra vonatkozó felhasználói szerepkör.  

- A modul befejezési fánkdiagramja: a modul befejezésének lebontása (az összefoglaló szakaszban látható szám) a modulok nevei alapján.

A diagram közepén megjelenő szám a befejezett modulok teljes számát mutatja

- Befejezések szerepkör szerint: a modul befejezésének lebontása a modul szerepköre szerint. Ha egy modul több szerepkörhöz is társítva van, akkor mindegyik szerepkör hozzá lesz adva a modul befejezésének számhoz.

A diagram közepén megjelenő szám a modul befejezéséhez szükséges különböző szerepkörök száma. 

- Befejezés termék szerint: a modul befejezésének lebontása az alapján a termék szerint, amelybe a modul le van leképezve. Ha egy modul több termékhez van társítva, akkor mindegyik termék hozzá lesz adva a modul befejezésének számhoz.    

A diagram közepén megjelenő szám a modul befejezéséhez szükséges különálló termékek száma.  

#### <a name="learning-path-tab"></a>Tanulás elérési út lap

Ez a lap a vállalatnál befejezett képzési útvonalakat tartalmazza az első öt modulnév alapján; az a termék, amelyhez a képzési útvonal le van leképezve; és az ehhez a képzési útvonalhoz megfelelő szerepkör.  

- Tanulás elérésiút-kiegészítések fánkdiagramja: a Tanulás (az összefoglaló szakaszban látható darabszám) lebontása név szerint.

- Befejezések szerepkör szerint: a képzési útvonalak befejezésinek lebontása szerepkör szerint. Ha egy modul több szerepkörhöz is társítva van, akkor mindegyik szerepkör hozzá lesz adva a modul befejezésének számhoz.

- Befejezés termék szerint: a képzési útvonalak befejezésének lebontása a termék szerint, amelyre a képzési útvonal le van leképezve. Ha egy modul több termékhez van társítva, akkor mindegyik termék hozzá lesz adva a modul befejezésének számhoz.

### <a name="completions-by-learning-individuals"></a>Képzések egyes személyektől

Ez felsorolja a vállalat betanított felhasználóit, valamint a befejezett moduljaik és képzési útjaik részleteit.

Microsoft Learn felhasználói objektumazonosítóval azonosítja a tanulókat. A **Modulok lapon minden** tanuló a befejezett modulok szerint van rendezve. A felhasználónevük, Microsoft Learn objektumazonosítójuk és a modulok száma alapján jelennek meg. A kereséshez használja a felhasználónevet. 

A **Tanulás** képzési útvonalak lapon minden tanuló a befejezett képzési útvonalak szerint rendezve jelenik meg a tanuló megjelenített nevével, objektumazonosítójával és modulszámával.

A tanuló részleteinek lekért adatai a felhasználói objektum azonosítójával: 

1. Jelentkezzen be a [Graph Explorerbe.](https://developer.microsoft.com/graph/graph-explorer ) (Önnek kell a vállalata Azure AD-bérlője globális rendszergazdának lennie.)

2. Másolja a felhasználói objektum azonosítóját az [Explorerben](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) kiemelt Graph területre. 

## <a name="frequently-asked-questions-faq"></a>Gyakori kérdések (GYIK)

1. Nem látom a cégEm Learn-adatait.

   Ez a jelentés olyan partnerek számára érhető el, akik fiókkal Partnerközpont. Ha még mindig a Partner Membership Center van, nem fogja látni ezt a jelentést.

2. Who cégen belül a cégen belül meg tudja tekinteni ezt a jelentést? 

   A globális rendszergazda és az MPN-rendszergazda megtekintheti a jelentést.

3. Hogyan győződhet meg arról, hogy minden felhasználó a saját Microsoft Learn a saját Partnerközpont fiókjához?

   *Miután* a globális rendszergazda hozzáadta az új felhasználót, a felhasználónak az [Microsoft Learn-hoz](/learn/) kell mennie, hogy a Azure Active Directory(AD) vállalati fiókját vagy munkahelyi fiókját a Learn-fiókjához csatolja. Ez biztosítja, hogy Elemzések Tanulás lapon a megfelelő kurzusok és készségek mutassanak.
   
   A felhasználónak a következőt kell:
   
   1. Jelentkezzen be a [Microsoft Learn.](/learn/)
   2. Válassza ki a profilképüket, majd válassza a **Saját profil** lehetőséget.
   3. Válassza a **Beállítások** lehetőséget.
   4. A **Fiókkezelés alatt** adja hozzá a munkahelyi fiókját a Csatolt **fiókok alatt.**

4. Láthatom a jelentésben az összes olyan felhasználót, aki MSA-Microsoft Learn jelentkezik be az alkalmazásba?

   Jelenleg ezt úgy lehet a legjobban megtenni, ha hozzáadja ezeket a felhasználókat az Azure AD-bérlőhöz, majd hozzáadja őket az Partnerközpont-hoz, hogy Microsoft Learn-fiókjukat a Saját profil-ban Partnerközpont.  

   Azok a felhasználók, akik a közeljövőben csak MSA-fiókjukat használják képzésre, a Microsoft Learn csapata lehetővé teszi, hogy a munkahelyi e-mail-címüket a saját Microsoft Learn társítsa. 

## <a name="next-steps"></a>Következő lépések

További jelentések: [Partnerközpont Elemzések.](partner-center-insights.md)

>[!NOTE] 
> A jelentést az irányítópult Jelentések letöltése szakaszában töltheti le a Elemzések nyers adatokkal. [További információ](insights-download-reports.md) 
