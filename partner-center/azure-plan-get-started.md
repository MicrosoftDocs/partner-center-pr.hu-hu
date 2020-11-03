---
title: Az Azure-csomagra való áttérés megkezdése
description: Ismerje meg, hogy az Azure utólagos elszámolású csomagjának használatával milyen információkat és ügyfeleket kell megismernie, beleértve az első lépéseket, a biztonsági óvintézkedéseket és a kezdéshez szükséges tudnivalókat.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 5ad7bd7c99d7caa044877c98aac6dc5e3ce69420
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "92530049"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Az utólagos elszámolású díjak használatának megkezdése az Azure-csomaggal

A Microsoft új kereskedelmi tapasztalatot vezetett be a partner Centerben.  Ezzel az új kereskedelmi tapasztalattal a partnerek a Microsoft ügyfél-szerződés keretében igénybe vehetik az Azure-szolgáltatásokat az utólagos elszámolású díjszabásban.

Ez a csomag leegyszerűsíti a vásárlási élményt – több Azure-előfizetéssel is rendelkezhet az Azure-csomagokban. Az Azure-előfizetések esetében már nem kell külön megrendelést elküldenie. Ebben az Azure-beli új kereskedelmi tapasztalattal összhangban vagyunk egy globális díjszabási elvvel, amely lehetővé teszi, hogy a CSP-partnerek az Azure-t a közzétett árakon nyújtsanak.

Ügyfeleink digitális átalakítási igényeihez új szaktudásra van szükség partnereinktől. Sok ügyfél olyan partnereket keres, akik a tranzakciót túlmutatva biztosítanak, hogy a Felhőbeli utazás zökkenőmentes legyen, és hatékonyan használják az Azure-szolgáltatásokat. A Microsoft partnerei kritikus szerepet játszanak az ügyfél életciklusának minden szakaszában. Az ilyen típusú partneri szolgáltatások a természetben jelennek meg, beleértve az Azure Estate monitoringot, a házirend-és irányítási felügyeletet, az üzembe helyezést és a konfiguráció finomhangolását, valamint a technikai támogatást és számos más szolgáltatást. Szükségük van egy partnerre, hogy az ügyfél Azure-környezetének megfelelően Ismerkedjen meg, és folyamatosan és megfelelő irányítással és felügyelettel rendelkezzen az általuk felügyelt erőforrások mögött. A 24 X 7 felhő-Operations Management szolgáltatást nyújtó számlázási partnereink jogosultak lesznek arra, hogy az adott munkához **felügyelt szolgáltatásokhoz kapcsolódó partneri kreditet** kapjanak.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Győződjön meg arról, hogy az ügyfelek aláírták a Microsoft Customer szerződést

2019. október 1. óta a Microsoft Customer szerződése egy olyan örökös megállapodást mutat be, amely leegyszerűsíti és egyszerűsíti az ügyfelek vásárlási élményét egy teljesen digitális folyamattal, elérhető. Minden olyan ügyfélnek, aki szeretné kihasználni az új kereskedelmi élményt az Azure-beli CSP-ben, alá kell írnia a Microsoft ügyfél-szerződést.

Azok a partnerek, akik az új Azure-csomag keretében szeretnének tranzakciókat használni, és új rendelést szeretne készíteni, meg kell erősíteniük a Microsoft ügyfél-szerződését a partner Center irányítópultján és az API-ban éles környezetben.

2020. február 1-től kezdődően a meglévő Microsoft Cloud szerződés el lesz távolítva a CSP programból. Ettől az időponttól kezdve az új Microsoft ügyfél-szerződéshez tartozó ügyfél-visszaigazolást (igazolást) minden egyéb ajánlathoz meg kell követelni, beleértve a Microsoft 365, a Dynamics 365 és a meglévő Azure-t is. A CSP-partnerek nem tudnak új rendelést készíteni az ügyfélnek a Microsoft-ügyfél szerződésének igazolása nélkül.

A részletekért olvassa el [a Microsoft ügyfél-szerződés megerősítő ügyfeleinek jóváhagyása](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Biztonsági és hozzáférés-vezérlési eljárások

A partnerek és az ügyfelek védelme érdekében az Advisors, a Vezérlőpult-szállítók és a felhőalapú megoldás-szolgáltatói programban részt vevő partnerek számára kötelező biztonsági követelményeket vezetünk be.

Azok a partnerek, akik nem alkalmazzák a kötelező biztonsági követelményeket, nem tudnak tranzakciót végezni a felhőalapú megoldás-szolgáltató programban, vagy a rendszergazdai jogosultságok kihasználása után felügyelik az ügyfél-bérlőket, ha ezek a követelmények érvénybe lép. Folyamatban van a követelmények technikai végrehajtási dátumának létrehozása, és részletes információkkal értesítjük a partnereket a dátumról.

## <a name="actions-to-take-to-implement-mfa"></a>Az MFA megvalósításához szükséges műveletek

Tekintettel arra, hogy a partner magas jogosultsági szinttel rendelkezik, gondoskodni kell arról, hogy minden egyes felhasználónak legyen MFA-kihívása minden egyes hitelesítéshez. Ez a következő módszerek egyikével valósítható meg:

- A prémium szintű Azure AD megvalósítása és a többtényezős hitelesítés (MFA) betartatása minden felhasználó esetében
- Az [Azure ad biztonsági Alapértelmezések](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) implementálása
- Harmadik féltől származó megoldás megvalósítása és az MFA biztosítása minden felhasználó számára

2019. augusztus 1-től minden partnernek ki kell kényszeríteni a többtényezős hitelesítést a partner bérlője minden felhasználója, beleértve a szolgáltatásfiókok szolgáltatást is. Az ezekkel a biztonsági követelményekkel kapcsolatos részletes információkat a [partneri biztonsági követelmények](partner-security-requirements.md)című témakörben találhat.

A Microsoft azt javasolja, hogy a partnerek szorgalmasan használják a RBAC, [Azure Active Directory Privileged Identity Management erőforrásokon](/azure/active-directory/privileged-identity-management/pim-configure)keresztül engedélyezett ajánlott eljárásokat követve.

## <a name="read-more-about-the-azure-plan"></a>További információ az Azure-csomagról

- [Az Azure-csomag megvásárlása](purchase-azure-plan.md)

- [Azure-ajánlatok összehasonlítása](compare-azure-offers.md)

- [Partner által létrehozott kredit – áttekintés](partner-earned-credit.md)

- A partner által létrehozott kredit (PEC) számítások, valamint a partner által szerzett kreditek beszerzésére jogosult szerepkörök és engedélyek elérhetők a partner Center irányítópult-árlista (bejelentkezés szükséges) lehetőséggel.

## <a name="next-steps"></a>Következő lépések 

- [A partner által létrehozott kreditek meghatározása – részletek](partner-earned-credit-explanation.md)
- [Az Azure-csomag árlista magyarázata](azure-plan-price-list.md)
- [Az ügyfél áttérése az Azure-csomagra](azure-plan-transition.md)
- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)
- [Azon országok/régiók teljes listája, ahol az Azure-csomag elérhető](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)