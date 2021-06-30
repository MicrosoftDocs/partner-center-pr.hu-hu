---
title: Megállapodások regisztrálása
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ha egy olyan ajánlatot regisztrál, amely a Partnerközpont, az segít a Microsoftnak, hogy a jövőben több lehetőséget nyújtson Önnek.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: eaa9bb6f8e57033669ef584e7c52c0d050a532e0
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080663"
---
# <a name="register-deals-youve-won-in-partner-center"></a>A következőben megnyert ügyletek regisztrálása Partnerközpont

**Megfelelő szerepkörök:** Ajánlói rendszergazda

A szerződéssel kapcsolatos további információkkal a Partnerközpont is regisztrálhatja az ön által megnyert ügyleteket. Ezek az információk további lehetőségeket biztosítanak a jövőben.

Az üzletregisztrációhoz két útvonal vezet:

- Létrehozott egy új ajánlatot  az Együttműködési lehetőségek szakaszban, és az üzlet megfelel az üzletregisztráció feltételeinek.
- Lezárt ISV Connect-ajánlatot szeretne jelenteni, amelyet nem adtak el együtt a Microsofttal.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Közös eladási lehetőségből származó üzlet regisztrálása

Ha egy közös értékesítésből származó ajánlatot regisztrál, az üzletnek az alábbi jogosultsági követelményeknek kell megfelelnie:

- Az ajánlat típusa lehet közös értékesítés vagy partner által vezetett (Ön úgy döntött, hogy engedélyezi a Microsoft-értékesítőknek, hogy megtekintsék ezt az ajánlatot).
- Az ajánlatban legalább egy ösztönzőnek megfelelő megoldás van. A megoldások akkor jogosultak az ösztönzőkre, ha a következő címkék közül legalább egyet tartalmaznak:
  - Azure IP-alapú közös értékesítés
  - Business Applications Premium
  - Business Applications Standard
- Az üzlet állapota "Won" (Megnyerve).
- Ha az ajánlat típusa közös értékesítés, akkor a Microsoftnak el kell fogadnia a meghívót, vagy az ajánlatot megnyertként kell megjelölnie. A Microsoft állapotát az üzlet részletei alatti Microsoft-kártyán láthatja.

Ha megfelel a jogosultsági követelményeknek, a rendszer automatikusan kérni fogja, hogy regisztrálja az ajánlatot az ajánlat folyamatjelző sávjában látható **Regisztráció** most gombbal:

:::image type="content" source="images/register-deals.png" alt-text="Képernyőkép az üzlet folyamatjelző sávról.":::

> [!NOTE]
> Ha **az Ajánlatregisztráció** elem nem jelent meg az ajánlat folyamatjelző sávjában, akkor az ajánlat nem felel meg az üzlet regisztrációja összes követelményének.

Miután rákattintott a **Regisztráció most** elemre, a rendszer átirányítja az Ajánlatregisztráció oldalra, és felkéri, hogy töltsön ki egy űrlapot, amely tartalmazza az ügyfél és a megoldás előre kitöltött adatait. Töltse ki az űrlapot az alábbi utasítások szerint, majd kattintson a **Register (Regisztrálás) gombra.**

Regisztrációkor a megoldástól függően egy vagy két üzletregisztrációs rekord jön létre.

- Ha a megoldás jogosult az ISV Connectre, létrejön egy ISV Connect-ajánlat regisztrációs rekordja. Ez az üzletregisztrációs rekord lesz használva a számlázáshoz.
- Ha a megoldás jogosult az IP-alapú közös értékesítéshez szükséges ösztönzőkre, akkor létrejön egy IP-cím az értékesítéssel kapcsolatos ajánlat regisztrációs rekordja. Ezt az üzletregisztrációs rekordot az értékesítést felülvizsgáló csapat fogja áttekinteni, jóváhagyni vagy elutasítani.

## <a name="report-a-closed-isv-connect-deal"></a>Lezárt ISV Connect-ajánlat jelentése

Lezárt ISV Connect-ajánlat jelentéséhez  lépjen az Ajánlatregisztráció lapra, és kattintson a **+ Lezárt jelentés ISV Connect-ajánlat elemre.** Töltse ki a kötelező mezőket, és kattintson a **Register (Regisztrálás) gombra.** Ez az üzletregisztrációs rekord lesz használva a számlázáshoz.

## <a name="fill-out-the-deal-registration-form"></a>Töltse ki az ajánlat regisztrációs űrlapját

> [!NOTE]
> Az ügyleteket szűrheti az ügyfél neve, állapota és ügylettípusa alapján. Kattintson az Ajánlatregisztráció oldal tetején található Szűrő gombra. 

Akár egy közös értékesítésből származó regisztrációval foglalkozik, akár egy zárt ISV Connect-ajánlatot jelent, amely nem volt együtt értékesítve a Microsofttal, a rendszer kérni fogja, hogy töltse ki az alábbi mezőket az ajánlatregisztrációs űrlapon.

- **Ügyfél adatai:** Adja **meg** az ügyfél cégnevét, és válassza ki az **országát/régióját.** Ezután adja meg a **városukat** és **államukat/tartományukat.**
- **Megoldás:** Válassza ki az üzlethez használni kívánt megoldást. Ha nem látja a megfelelő megoldást a listában, forduljon az ügyfélszolgálathoz.
- **Szerződés típusa:** Adja meg,  hogy az ajánlat új szerződés vagy egy **korábbi** szerződés megújítása.
- **Teljes szerződésérték:** A kötelezettségvállalás várt teljes értéke. Ennek az értéknek tartalmaznia kell az összes szoftver- és szolgáltatásdíjat, a hardverköltségeket azonban nem. Győződjön meg arról, hogy a megfelelő pénznemet választja ki.
- **Megoldás értéke:** Az üzlethez használt felhőalapú megoldás teljes értéke. Mindenképpen foglalja bele a szoftver- és karbantartási díjakkal kapcsolatos összes költséget, de ne foglalja bele a fizetendő tételeket, a nem ismétlődő testreszabási díjakat és a Microsoft által fizetett, közvetlenül kapcsolódó CSP-licencdíjakat.
- Üzembe lesz helyezni a megoldást **az Azure-ban? Ha nem, válassza az Egyéb:** Válassza az **Azure** vagy az **Egyéb lehetőséget.**
- **A megoldás a partnerbérlőn** vagy az ügyfélbérlőn  fog futni? : Válassza ki az ügyfélbérlőt vagy a **partnerbérlőt.**
- **Szerződés kezdő dátuma:** A szerződés kezdési dátuma. Használat alapján fizetett (PAYG) ügyletekhez használja az első számla dátumát. A tervezés Partnerközpont nem fogja lehetővé, hogy a szerződés aláírási dátumnál korábbi kezdő dátumot adjon meg. Ez hatással lehet néhány ügyletre, például az aláírási dátum előtti IP-telepítésre. Ezeknek az ajánlatoknak a sikeres megkötéséhez  használja a szerződés aláírási dátumát az aláírási dátum és a kezdő dátum mezőben is a beküldéskor. (A szerződésnek explicit módon meg kell határoznia az ajánlat időtartamát, hogy az ACV megfelelően kiszámítható legyen.)
- **Szerződés záró dátuma:** Ha a szerződés egy adott dátumon fog véget érni, válassza a **Záró dátummal** rendelkezik lehetőséget, és adja meg a dátumot. Ha a szerződésnek nincs meghatározott záró dátuma, válassza a **Folyamatos lehetőséget.** A használat alapján fizetett (PAYG) ügyletekhez használja a legutóbbi vagy a legutóbbi számla dátumát.
- **Szerződés aláírt dátuma:** Az a dátum, amikor a végleges szerződést a szervezet és az ügyfél aláírta. Használat alapján fizetett (PAYG) ügyletekhez használja az első számla dátumát.
- **Regisztrációs kapcsolattartó:** **A** szervezet egy olyan személyének vezetékneve, vezetékneve, telefonszáma és e-mail-címe, akivel kapcsolatba léphetünk, ha további információra van szükségünk az itt megadott adatokkal kapcsolatban. 

Ha az oldal összes szakaszát befejezte, kattintson a **Regisztráció elemre.**

- Ha az üzlet ISV Connect-ajánlat, észreveheti, hogy az ajánlat állapota "Beküldött, Befejezve". Ehhez az üzletregisztrációs rekordhoz nem szükséges további művelet. Ezt a rekordot fogja használni a számlázáshoz.
- Ha az ajánlat egy IP-cím alapú közös értékesítés, észreveheti, hogy az ajánlat állapota "Elküldve". A Microsoft közös értékesítéseket áttekintő csapata áttekinti az ezen az ajánlat regisztrációs rekordon megadott adatokat. A felülvizsgálati csapat további lépéseket fog kérni Öntől, ha szükséges, vagy közvetlenül jóváhagyja/elutasítja az ajánlatot.
- Ha olyan ajánlatot regisztrál, amely egy közös értékesítésből származik, és azt látja, hogy két ajánlatregisztrációs rekord jött létre, az azt jelenti, hogy az adott ajánlat megoldása jogosult mind az ISV Connect, mind az IP-cím alapú közös értékesítésre. Az ISV Connect-rekord a számlázáshoz lesz használva. Az IP co-sell rekordot az értékesítést ellenőrző csapat fogja áttekinteni.

