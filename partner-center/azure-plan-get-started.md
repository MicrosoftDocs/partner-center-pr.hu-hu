---
title: Az Azure-csomagra való áthelyezés megkezdése
description: Megtudhatja, hogy Önnek és ügyfeleinek mit kell tudniuk a használat alapú fizetéses Azure-csomag használatával kapcsolatban, beleértve az első lépéseket, a biztonsági óvintézkedéseket és az első lépéseket.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 58feabdefb02660559c69f61190070310768b947
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149655"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Használat alapján fizetett díjak használatának megkezdése az Azure-csomaggal

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Értékesítési ügynök


A Microsoft új kereskedelmi élményt vezetett be a Partnerközpont.  Ezzel az új kereskedelmi megoldással a partnerek használat alapján, használat alapján férhetnek hozzá az Azure-szolgáltatásokhoz a Microsoft Ügyfélszerződés.

Ez a csomag leegyszerűsíti a vásárlási élményt – egy Azure-csomag több Azure-előfizetéssel is rendelkezik. Azure-előfizetésenként már nem kell külön rendelést beküldődni. Az Azure új kereskedelmi élményében pedig egyetlen globális díjszabási alapelvhez igazodtunk, amely lehetővé teszi a CSP-partnerek számára, hogy a közzétett árakon kínálják az Azure-t.

Ügyfeleink digitális átalakulási igényeihez új partneri készségekre van szükség. Számos ügyfél keres partnereket, hogy a tranzakción felül és azon kívül is szolgáltatásokat nyújtson, hogy zökkenőmentesebb legyen a felhőre való utazásuk, és hatékonyan használjuk fel az Azure-szolgáltatásokat. A Microsoft partnerei az ügyfél életciklusának minden szakaszában kritikus szerepet játszanak. Az ilyen típusú partnerszolgáltatások folyamatos jellegűek, és magukban foglalják az Azure-tulajdon monitorozását, a szabályzat- és cégirányítási felügyeletet, a finomhangolás beállítását és konfigurálást, a műszaki támogatást és számos más szolgáltatást. Egy partnernek szorosan ismernie kell az ügyfél Azure-környezetét, és folyamatos és megfelelő irányítással és irányítással kell rendelkezik a mögöttes erőforrások kezeléséhez. Azok **a** számlázási partnerek, akik ezt a 24 x 7 felhőművelet-felügyeleti műveletet biztosítják, jogosultak lesznek az erre a munkára felügyelt szolgáltatásokért kapott partneri jóváírásra.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Ellenőrizze, hogy az ügyfelek aláírták-e a Microsoft Ügyfélszerződés

2019. október 1-től elérhető a Microsoft Ügyfélszerződés, amely egy teljes mértékben digitális folyamattal egyszerűsíti és egyszerűsíti az ügyfelek vásárlási élményét. Minden ügyfélnek, aki ki szeretné használni a CSP for Azure új kereskedelmi élményét, alá kell írnia a Microsoft Ügyfélszerződés.

Az új Azure-csomag keretében tranzakciót és új rendelést tenni kívánó partnereknek meg kell erősíteniük az ügyfél által elfogadott Microsoft Ügyfélszerződés az Partnerközpont és API használatával éles környezetben.

2020. február 1-től a meglévő Microsoft Cloud szerződés el lesz távolítva a CSP-programból. Ettől az időponttól a partnernek meg kell erősítenie (igazolása) az új Microsoft Ügyfélszerződés ügyfél általi elfogadását az összes többi ajánlathoz, beleértve a Microsoft 365, a Dynamics 365 és a meglévő Azure-t is. A CSP-partnerek nem tudnak új rendelést tenni az ügyfélnek a szolgáltató igazolása Microsoft Ügyfélszerződés.

Részletes információkért olvassa el a Következőt: A feltételek [ügyfél általi elfogadásának Microsoft Ügyfélszerződés](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Biztonsági és hozzáférés-vezérlési eljárások

A partnerek és az ügyfelek védelme érdekében kötelező biztonsági követelményeket vezetünk be az Vezérlőpult programban részt vevő tanácsadók, Felhőszolgáltató partnerek számára.

Azok a partnerek, akik nem valósítják meg a kötelező biztonsági követelményeket, nem hajtanak végre tranzakciót a Felhőszolgáltató-programban, és nem kezelhetik az ügyfélbérlőket a delegált rendszergazdai jogosultságok érvénybe lépése után. Folyamatban van egy technikai kényszerítési dátum létrehozása a követelményekhez, és részletes információkkal értesítjük a partnereket a dátumról.

## <a name="actions-to-take-to-implement-mfa"></a>Az MFA megvalósításához szükséges műveletek

Mivel a partnerek rendkívül emelt szintű jogosultságokkal rendelkezik, minden egyes hitelesítésnél meg kell győződnünk arról, hogy minden felhasználónak MFA-kihívása van. Ez a következő módszerek egyikével valósítható meg:

- A prémium szintű Azure AD és a többtényezős hitelesítés (MFA) kényszerítésének biztosítása minden felhasználó számára
- Az [Azure AD biztonsági alapértelmezések megvalósítása](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Harmadik féltől származó megoldás megvalósítása és az MFA kényszerítésének biztosítása minden felhasználó számára

2019. augusztus 1-től minden partnernek kötelező többtényezős hitelesítést kikényszerítenie a partnerbérlő összes felhasználója számára, beleértve a szolgáltatásfiókokat is. A biztonsági követelményekkel kapcsolatos részletes információkat a [Partnerbiztonsági követelmények oldalon talál.](partner-security-requirements.md)

A Microsoft azt javasolja, hogy a partnerek gondosan használják az RBAC-t, a következő forrásokkal [engedélyezett ajánlott Azure Active Directory Privileged Identity Management használatával:](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="read-more-about-the-azure-plan"></a>További információ az Azure-csomagról

- [Az Azure-csomag megvásárlása](purchase-azure-plan.md)

- [Azure-ajánlatok összehasonlítása](compare-azure-offers.md)

- [Partneri jóváírás – áttekintés](partner-earned-credit.md)

- A partneri jóváírás (PEC) számításai, valamint a partneri jóváírásra jogosult szerepkörök és engedélyek a Partnerközpont Irányítópult árlistából érhetők el (bejelentkezés szükséges).

## <a name="next-steps"></a>Következő lépések 

- [A partneri jóváírás meghatározása – részletek](partner-earned-credit-explanation.md)
- [Az Azure-csomag árlistának magyarázata](azure-plan-price-list.md)
- [Az ügyfél áttérése az Azure-csomagra](azure-plan-transition.md)
- [Az Azure-csomagban foglalt előfizetések és erőforrások kezelése](azure-plan-manage.md)
- [Azon országok/régiók teljes listája, ahol elérhető az Azure-csomag](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)