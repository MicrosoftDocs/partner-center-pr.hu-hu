---
title: SaaS-ajánlat vásárlása Azure Portal
description: Megtudhatja, hogyan találhat meg és vásárolhat SaaS-ajánlatot a Azure Portal.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/29/2021
ms.openlocfilehash: a124e4c5bb31a1fbb744bf2c5e1ea65a356bdd54
ms.sourcegitcommit: 1d09ccaaa54f167b0c63e99761172ebe84e89f2e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/02/2021
ms.locfileid: "113221440"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>SaaS-ajánlat vásárlása Azure Portal

Ez a cikk a szolgáltatott szoftverre (SaaS) vonatkozó ajánlatok keresésének, kipróbálásának és megvásárlásának különböző lehetőségeit és követelményeit ismerteti a Azure Portal.

## <a name="create-a-saas-subscription"></a>SaaS-előfizetés létrehozása

SaaS-előfizetés vásárlásához szüksége lesz egy Azure-beli felhasználói fiókra, amely hozzáféréssel rendelkezik egy megfelelő Azure-előfizetéshez. Ezt az előfizetést a számlázáshoz, valamint a megvásárolt felhőerőforrások részleteinek felszűkítéséhez fogjuk használni. Az Azure-előfizetésekkel kapcsolatos további információkért lásd: [További Azure-előfizetés létrehozása.](/azure/cost-management-billing/manage/create-subscription)

A Azure Portal válassza ki a kívánt SaaS-ajánlatot a **Marketplace szakaszban.**

A szolgáltatásként megadott szoftveres előfizetések egy adott időtartamra online előfizetésen keresztül biztosítják a szolgáltatás használatát ahelyett, hogy helyi telepítést telepítenének az egyes számítógépekre. Az előfizetés egy vagy több felhőplatform vagy -szolgáltatás használatára vonatkozó szerződés, amelynek díja a felhasználónkénti licencdíj vagy a felhőalapú erőforrás-használat alapján fizetendő. Egy szervezet több SaaS-előfizetéssel is rendelkezik.

Az SaaS-előfizetések korlátozásai a következők:

- Nincsenek tanulói előfizetések.
- Nincs Visual Studio Enterprise-előfizetés.
- Nincs ingyenes kredit-előfizetés.
- Fizetős ajánlatokhoz fizetési eszközre van szükség.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS-ajánlatok felderítése a Azure Portal

Miután a Azure Portal, több módon is leszűkítheti a keresést, hogy az SaaS-ajánlatokra összpontosítson.

### <a name="narrowing-your-search"></a>A keresés szűkítése

A kezdőlapOn, az **Azure-szolgáltatások alatt válassza** **az + Erőforrás létrehozása vagy a** Marketplace **lehetőséget.** Vagy használja a **G + N parancsikont** bárhol a platformon.

- Szűkítse le az eredményeket SaaS-ajánlatokra az Ajánlattípus **szűrővel,** majd válassza az **SaaS lehetőséget.**
- Egy adott SaaS globális keresés használhatja a felső navigációs terület felső sávján található felső sávot.

Keresse meg a [privát SaaS-ajánlatot](/marketplace/private-offers) a Marketplace kezdőlapján található **szalagcím kiválasztásával.** Nem minden ajánlat vagy csomag érhető el minden földrajzi helyen, és előfordulhat, hogy néhány csak bizonyos bérlők számára jelenik meg.

A szűrt nézetben minden elérhető SaaS-ajánlat címként jelenik meg. Válassza ki az egyiket a termékadatok oldalának kiválasztásához. A következő szakaszokból áll:

- Áttekintés – a szolgáltatás, a marketing és a tananyagok részletei
- Csomagok és díjszabás – minden ajánlat tartalmazni fog legalább egy, eltérő számlázási feltételekkel és árakkal
- Használati adatok + támogatás – tartalmazza Publisher azonosítót, az ajánlat azonosítóját és a csomagazonosítót
- Az adott SaaS-ajánlat értékelése és értékelése

## <a name="available-billing-models-plansskus-for-saas-offers"></a>SaaS-ajánlatokhoz elérhető számlázási modellek (csomagok/termékkódok)

Minden Egyes SaaS-ajánlat egy vagy több csomaggal fog bejelentkezni. Minden ajánlathoz tartozik egy díjszabási modell: egyendíjas vagy felhasználónkénti. Minden csomag ára ismétlődő díj, amely nulla dollár lehet (a felsorolt árak csak példaként szolgálnak, és nem a tényleges költségeket hivatottak tükrözni). Ez a díj lehet egyendíjas, vagy felhasználónkénti ár. Elérhető csomagok típusai:

- **Havi csomagok** – ismétlődő havi díj; havi rendszerességgel fizetendő, felhasználónkénti havi díj. A kifejezés végén a terv automatikusan megújul.
- **Éves csomagok** – ismétlődő éves díj; egy éves ismétlődésben fizetendő, felhasználónkénti éves díj. A kifejezés végén a terv automatikusan megújul.
- **Egyéni fogyasztásmérők** – az ismétlődő díjak mellett az egydíjas csomag opcionális egyéni forgalmi díjas dimenziókat is tartalmazhat a túlhasználatért, amely nem része az egyszerű díjnak. Minden dimenzió egy számlázható egységet képvisel. Ez egy változó költség, amely a forgalmi díjas egységek (például a sávszélesség, a jegyek vagy a feldolgozott e-mailek) használata alapján változik. Ezeknek a dimenzióknak a havi használatának megfelelően kell fizetnie. Vegye figyelembe, hogy a túlóra-használat csak akkor kezdődik, ha az összes forgalmi díjas egységet felhasználta, amely az egyszerű díjban szerepel.
- **Ingyenes próbaverzió** – Bizonyos esetekben a csomag egy hónapos próbaidőszakot tartalmaz, amelynek során ingyenesen használhatja a szoftvert.  Ha a próbaidőszak véget ért, a díj fel lesz számolva a csomagnak megfelelően. A próbaverziós ajánlatok nem kompatibilisek az egyéni mérőműveletekkel.

Ezek a díjszabási modellek nyilvános és privát csomagokhoz is elérhetők.

## <a name="saas-purchase-experience"></a>SaaS vásárlási élmény

1. A termékoldalon válasszon ki egy, az igényeinek megfelelő tervet, és folytassa a **beállítását és előfizetését**
2. A vásárlási folyamat részeként a rendszer átirányítja  az Alapvető beállítások lapra, és a következőt kell megadnia:
    1. Határozza *meg, hogy melyik* előfizetést szeretné használni a számlázáshoz. A használt Azure-előfizetéshez meg kell határozni egy érvényes vásárlási módszert. Rendelkeznie kell a megfelelő szintű engedélyekkel, vagy rendelkeznie kell egy erőforráscsoporttal az előfizetés alatt a megfelelő szintű engedélyekkel. A számlázási országnak az az országnak kell lennie, ahol az ajánlat megvásárolható. Érvényes fizetési mód nélküli Azure-előfizetések (például MSDN-előfizetések) csak ingyenes csomagok vásárlására használhatók
    1. Válasszon ki vagy hozzon létre egy **erőforráscsoportot,* amelyhez az SaaS-erőforrás tartozni fog.
    1. Írja *be* az SaaS-előfizetés nevét, hogy később könnyen azonosíthatja. A vásárlás után a nevet nem módosíthatja.
    1. A **Csomag** alatt láthatja a kiválasztott tervet a termék részletes oldalán (PDP). Ha nem tett aktív kijelölést a PDP-ben, az alapértelmezett csomag látható. A kijelölést a Terv módosítása hivatkozásra **kattintva módosíthatja.** Válassza ki a megfelelő számlázási időszak, majd válasszon egy másik csomag. Ha a közzétevő támogatja a vásárlást, módosíthatja a csomagját. A kifejezést azonban nem módosíthatja haviról évesre, illetve évesről havira.
    1. Abban az esetben, ha a díjszabási modell *felhasználónkénti,* előfordulhat, hogy meg kell adnia a Felhasználók *számát.* A látható ár a kiválasztott előfizetés, csomag és időszak alapján változik.
3. Lépjen a **Címkék lapra** – *A* címkék felhasználó által definiált kulcs/érték párok, amelyek közvetlenül elhelyezhetőek egy erőforráson vagy erőforráscsoporton. A címkékkel később könnyen megkeresheti az SaaS-erőforrást. Az Azure jelenleg erőforrásonként és erőforráscsoportonként legfeljebb 50 címkét támogat. A címkék elhelyezhetőek az erőforrásokon a létrehozáskor, vagy hozzáadhatóak egy meglévő erőforráshoz.
4. Folytassa az **Áttekintés + Előfizetés gombra** az ajánlat és a csomag részleteinek áttekintésével.
    1. Tekintse *Használati feltételek* közzétevő és  a közzétevő adatvédelmi szabályzatának, módosításainak és adatvédelmi szabályzatának Azure Marketplace 
    1. Előfordulhat, hogy meg kell adni a kapcsolattartási adatait
    1. Az *alapok és a* címkék *részleteinek* áttekintése
5. Megerősítés után válassza a **Feliratkozás lehetőséget.**

## <a name="saas-subscription-and-configuration"></a>SaaS-előfizetés és -konfiguráció

Ha a feliratkozás lehetőséget választja, a következő üzenet jelenik meg: "Az SaaS-előfizetés folyamatban van". Ez a folyamat eltarthat néhány percig, és ne zárja be az ablakot, amíg be nem fejeződik.

Az előfizetés befejezése után egy üzenet jelenik meg, amely szerint az SaaS-előfizetés befejeződött, és úgy kell konfigurálnia a fiókot, hogy elkezdi élvezni a vásárlást. Egy e-mailt is kap, amely arra kéri, hogy aktiválja az új előfizetést. Ha nem Ön az, aki konfigurálja az SaaS-fiókot, továbbk továbbította ezt az e-mailt a megfelelő személynek.

A folyamat befejezéséhez és az SaaS használatának elkezdéséhez el kell kezdenie az előfizetés konfigurálását. A Fiók **konfigurálása gombra** kattintva a rendszer átirányítja a közzétevő webhelyére.

Az előfizetés állapotát a fejléc jobb felső sarkában található "harang" ikon kiválasztásával is ellenőrizheti.

Ha *30* napon belül nem fejeződik be a konfigurációs folyamat, a rendszer automatikusan törli ezt az SaaS-előfizetést.  A számlázás azután kezdődik, hogy a fiók konfigurálva van a közzétevő webhelyén.

Hibaüzenetek jelenhetnek meg a folyamat során:

- A kiválasztott *csomag neve* nem vásárolható meg ingyenes előfizetésben
  - Frissítse a fiókját. https://aka.ms/UpgradeFreeSub További részletekért lásd: .

- A vásárlás meghiúsult, mert nem található érvényes hitelkártya vagy az Azure-előfizetéséhez társított fizetési mód.
  - Használjon másik Azure-előfizetést, vagy adja hozzá az aktuális hitelkártyát vagy fizetési módot, és próbálja meg újra.

- A *kiválasztott ajánlat neve*  az ajánlat  közzétevőnkénti közzétevője szerint csomagnév nem vásárolható meg a rendszergazda által meghatározott szabályok szerint.
  - Lépjen kapcsolatba a rendszergazdával.

- Az *ajánlat közzétevője* által  kiválasztott csomag csomagneve nem érhető el a bérlő rendszergazdája által megadott privát Marketplace-beállítások miatt. 
  - Kapcsolatfelvétel a rendszergazdával

- A vásárlás meghiúsult, mert a kért számlázási időszak üres vagy érvénytelen.
  - Próbáljon meg másik tervet vagy számlázási távon vásárolni.

- A vásárlás meghiúsult, mert nem sikerült ellenőrizni a jogi megállapodásra való bejelentkezést.
  - Újra. Ha a hiba továbbra is fennáll, próbálkozzon a vásárlással egy másik Azure-előfizetéssel, vagy forduljon az ügyfélszolgálathoz.

- Az ajánlat *ajánlatazonosítójának közzétevői* *közzétevő-azonosító alapján való* megvásárlása meghiúsult. Ez az ajánlat jelenleg nem érhető el vásárláshoz.
  - Próbálkozzon újra később. Ha egy óra múlva is megjelenik ez a hibaüzenet, forduljon az ügyfélszolgálathoz.  

- Az *offerID* csomag *csomagazonosítójának* közzétevő-közzétevő-azonosító alapján való megvásárlása meghiúsult.  Ez a csomag jelenleg nem érhető el vásárláshoz.
  - Próbálkozzon újra később. Ha egy óra múlva is megjelenik ez a hibaüzenet, forduljon az ügyfélszolgálathoz. 

- Az *ObjectID* objektumazonosítóval megadott ügyfél-e-mail-cím nem rendelkezik engedéllyel a *DeploymentValidationAction* művelet végrehajtásához a  *ResourceGroup hatókörben; DeploymentScope* vagy a hatókör érvénytelen.  
  - Ez az üzenet akkor jelenik meg, ha nem rendelkezik a megfelelő engedélyekkel az Azure-előfizetéshez/erőforráscsoporthoz.  
    Ha nemrég kapott hozzáférést, frissítse hitelesítő adatait.  
    Az erőforrások erőforráscsoportban való üzembe helyezéséhez legalább Közreműködői hozzáféréssel kell lennie. Ellenőrizze a hozzáférési állapotát az **Erőforráscsoportok alatt,** majd kattintson **a Access Control.** Itt látható, hogy ki a "Tulajdonos", és megkérheti, hogy közreműködőként rendeljen hozzá.

- Az ehhez a vásárláshoz használt előfizetés nem engedélyezi a Marketplace-vásárlásokat.  
  - Használjon másik előfizetést, vagy kérje meg a rendszergazdát, hogy módosítsa az előfizetés definícióját, és próbálja meg újra.

## <a name="next-steps"></a>Következő lépések

- Ha már vásárolt egy ajánlatot a piactéren, akkor a Számlázás és [számlázás lehetőséget kell látnia.](/marketplace/billing-invoicing)
- További információ a privát csomagok [beállításairól.](/marketplace/private-offers)
