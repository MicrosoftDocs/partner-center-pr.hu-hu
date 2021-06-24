---
title: Szerepkörök hozzárendelése & engedélyek felhasználókhoz
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, mely szerepkörök a legmegfelelőbbek a vállalat kereskedelmi tranzakciókat, terjesztéseket, ösztönzőket vagy MPN-tagságokat Partnerközpont.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 582fdc98617be7d82c0bc61a0bf46ceb662954d3
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565083"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Felhasználói szerepkörök és engedélyek hozzárendelése olyan vállalati felhasználókhoz, akik a vállalaton belül Partnerközpont

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | MPN-partner rendszergazdája

Beállította partnerprofilját, amely tartalmazza a jogi nevet és címet, a támogatási adatokat, a fájl-adómentességet, a banki adatokat és a vállalat elsődleges kapcsolattartóját. Következő lépés: Állítsa be a felhasználók számára a jelszavakat és a szerepköröket, hogy megkezdjék Partnerközpont munkát.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Az alkalmazottak beállítása a Partnerközpont

Ön határozza meg, hogy a felhasználók milyen típusú hozzáféréseket Partnerközpont az Ön által adott szerepkörök és engedélyek alapján. A szerepkörök ahhoz a programhoz vagy programokhoz kapcsolódnak, amelyekben a vállalat részt vesz. Ha például a vállalata egy Felhőszolgáltató- (CSP-) vállalkozás, nem csak a szabványos Azure Active Directory- (Azure AD-) bérlőkezelési szerepkörökkel, például globális rendszergazdai szerepkörökkel rendelkezik, hanem a CSP-programra jellemző szerepkörökre is szüksége lesz. Minden program saját szerepkörökkel rendelkezik.

>[!Note]
> Az Azure AD-bérlői szerepkörök közé tartoznak a globális rendszergazdai, a felhasználói rendszergazdai és a CSP-szerepkörök. A nem Azure AD-szerepkörök azok a szerepkörök, amelyek nem kezelik a bérlőt, és tartalmazzák az MPN (Microsoft Partner Network) partnerrendszergazdát, az üzleti profil rendszergazdáját, a ajánlói rendszergazdát, az ösztönző rendszergazdáját és az ösztönző felhasználót. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Üzleti tranzakciók kezelése a Partnerközpont (Azure AD- és CSP-szerepkörök)

|**Szerepkör**|**Mire valók**|**További információ**|
|----------------------------------|---|:---------------------------------|
|Globális rendszergazda|* Az összes Microsoft-fiók/szolgáltatáshoz teljes körű jogosultsággal fér hozzá|[Partnerközponti fiók kezelése](partner-center-account-setup.md)
|      |* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése
||* Szerződések, árlisták és ajánlatok megtekintése
||* Partnerfelhasználók megtekintése, létrehozása és kezelése|
||  A számlázás, a számlák és a felderítési fájlok megtekintése, létrehozása és kezelése
|Felhasználókezelő rendszergazda   | * Felhasználók megtekintése, létrehozása és kezelése|[Kezelheti a Microsoft Partner Network előnyeit és ajánlatát a Partnerközpont](manage-your-partner-network-benefits.md)
||* Az összes megtekintése partnerprofilok létrehozása
||* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése
|Számlázási adminisztrátor | – A számlázás, a számlák és a felderítési fájlok megtekintése, létrehozása és kezelése|[A számla elolvasása](billing.md)
||* Díjszabás megtekintése
||* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése
|Alapértelmezett felhasználó|  Nézet Saját profil   |[Új jelszó kérése](reset-my-pasword.md)
|Rendszergazdai ügynök | * Ügyfélkezelés|[Az ügyfélkapcsolatok szorosabbra fűzése](connect-with-your-customers.md)
||* Eszközlista hozzáadása a Partnerközpont
||* Profilok létrehozása és alkalmazása az eszközökre
||* Előfizetés-kezelés
||* Szolgáltatás állapot- és szolgáltatáskérései ügyfelek számára
||* Delegált rendszergazdai jogosultságok kérése
||* Díjszabás és ajánlatok megtekintése
||* Számlázás
||* Felügyelet ügyfél nevében
||* Értékkel hozzáadott viszonteladó regisztrálása
||* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése|
|Értékesítési ügynök | * Ügyfélkezelés|[Számlázási támogatás biztosítanak az ügyfelek számára, és segítenek megválaszolni a számlázással kapcsolatos kérdéseket](provide-billing-support.md)
||* Eszközlista hozzáadása a Partnerközpont
||* Előfizetés-kezelés
||* Támogatási jegyek megtekintése
||* Kapcsolat kérése egy ügyféllel
||* Díjszabás és ajánlatok megtekintése
||* Érdeklődők kezelése
||* Az ügyfélszerződés megtekintése
||* Értékkel hozzáadott viszonteladó regisztrálása
||* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése|
|Helpdesk agent| * Ügyfél keresése és megtekintése|[Problémák eszkalálása a Microsoftnak, és a Microsoft eszkalálásának leginkább megfelelő problémák megismerása](escalate-problems-to-microsoft.md)
||* Ügyféladatok szerkesztése
||* Segítség az ügyfelek számlázással vagy előfizetés-kezeléssel kapcsolatos problémáinak megoldásához
||* Támogatás kérése az ügyfelek nevében 
||* Előfizetések és számlázási problémák kezelése az ügyfelek nevében
||* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Vezérlőpult Szállító (CPV). (CSP-szerepkör és nem Azure AD-szerepkör)

A CPV-k CSP-partnerek által használható alkalmazásokat fejlesztnek, hogy integrálják a rendszereiket az Partnerközpont API-okkal. 

|**Szerepkör**   |**Miket végezhet el?**|**További információ**|
|------------------------------|:----------------------------|----|
|Globális rendszergazda| A cpv Vezérlőpult profil megtekintése és kezelése|[Regisztrálás Vezérlőpult a CSP-partnerrendszerek és az Partnerközpont API-k integrálásához](enroll-as-cpv.md)
||A CPV-képességekhez hozzáféréssel bíró felhasználók megtekintése és kezelése|

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Vendégfelhasználó (hozzá kell adni az Azure AD-bérlőhöz)

|**Vendégfelhasználó**   | **Szerepkörök**|
|---------------------------|:--------------------|
||MPN-partner rendszergazdája|
||Üzletiprofil-rendszergazda|
||Ajánlói rendszergazda|


## <a name="manage-mpn-membership-and-your-company"></a>MPN-tagság és a vállalat kezelése 

Ezek a szerepkörök nem Azure AD-szerepkörök. Ezek a szerepkörök nem a bérlőt, hanem a vállalat vállalkozását kezelik.

|**Szerepkör** | **Miket végezhet el?**|**További információ**|
|----------------------------|:----------------------------|-----|
|MPN-partner rendszergazdája|* Partnerszolgáltatás-kérelmek megtekintése, létrehozása és kezelése|[Microsoft Action Pack-előfizetés, illetve Silver és Gold kompetencia vásárlása vagy megújítása](mpn-get-action-pack.md)
||* Jogi, vállalati, üzleti és MPN-profilok megtekintése
||* A felhasználói adatok és a készségeik adatainak megtekintése
||* Kompetenciák megtekintése
||* Előnyök megtekintése és kezelése
||* MPN-ajánlatok megtekintése és vásárlása
||* Az MPN-ajánlatok rendelési előzményeinek és számláinak megtekintése
||* Partneri hozzájárulás jelzői adatainak megtekintése
||* Használható a érvényesítési eszközben|
||* Ügyféladatok elemzésének megtekintése
||* A vállalaton belüli egyéb felhasználói szerepkörök megtekintése, de nem lehet szerepköröket hozzárendelni
||* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése
|Fiókadminisztrátor| Helyek hozzáadása|[Helyek kezelése](manage-locations.md)
|| A rendszergazdai fiókokkal kapcsolatos profilok kezelése 
||* Szerepkörök hozzárendelése bérlőbeli felhasználókhoz nem Azure-AD-szerepkörökhöz 
||* Helyek regisztrálása programokba
||* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése

## <a name="manage-referrals"></a>Hivatkozások kezelése

|**Szerepkör** | **Miket végezhet el?**|**További információ**
|------------------------------|:-------------------------|---|
|Ajánlói rendszergazda|Hozzon létre és kezeljen mindent a Partnerközpont|[Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)
||    Megtekintheti és szerkesztheti az összes közös értékesítési lehetőséget és érdeklődőt
||    Csapattagokat rendelhet hozzá egy ajánlathoz
||    Megtekintheti és szerkesztheti az üzleti profilokat
||    Megtekintheti és regisztrálhatja az ügyleteket az olyan lehetőségekhez, amelyek megnyertként vannak megjelölve, és jogosultak az ügylet regisztrációra
||    Létrehozhat és megtekinthet támogatási jegyeket
|Ajánlói felhasználó|Az közös értékesítés lehetőségeinek létrehozása és kezelése csak akkor, ha tagjai a csapatnak |[Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)
||    Közös értékesítési lehetőségeket hozhat létre azokkal a helyekkel, amelyekhez hozzá vannak rendelve a szerepkör.
||    Megtekintheti és regisztrálhatja az olyan lehetőségek ajánlatait, amelyek megnyertként vannak megjelölve, és jogosultak az ügylet regisztrációra, ha csapattagok.
||    Létrehozhat és megtekinthet támogatási jegyeket
|Üzletiprofil-rendszergazda|Üzleti profilok létrehozása és kezelése | [Üzleti profilok kezelése](create-a-marketing-profile.md)
||    Létrehozhat és megtekinthet támogatási jegyeket

Az új javaslati felhasználói szerepkör mellett bemutatjuk az ügyletek helyének hatókörét is. Az alábbi táblázat a hely alapján mutatja be az ügyletekhez való hozzáférést.

|**Hatókör** | **Miket végezhet el?** |
|------------------------------|:-------------------------|
|Az egész vállalat | A rendszergazdák és a felhasználók is hozzáférhetnek a vállalatuk bármely helyére vonatkozó ügyletek létrehozásához|
|| A ajánló rendszergazdának hozzáférése van az összes ügylet megtekintéséhez és szerkesztéséhez |
|| A ajánló felhasználók csak akkor férhetnek hozzá az összes ügylet megtekintéséhez és szerkesztéséhez, ha tagjai a csapatnak |
|Egy vagy több hely | A rendszergazdák és a felhasználók is hozzáférhetnek a vállalatukhoz rendelt helyhez való ügylet létrehozásához|
|| A ajánlói rendszergazda hozzáférhet a hozzárendelt helyekhez tartozó összes ügylet megtekintéséhez és szerkesztéséhez|
|| A ajánló felhasználók akkor férhetnek hozzá a hozzárendelt helyekhez tartozó összes ügylet megtekintéséhez és szerkesztéséhez, ha tagjai a csapatnak|

## <a name="manage-incentives"></a>Ösztönzők kezelése

|**Szerepkör** | **Miket végezhet el?**|**További információ**
|------------------------------|:-------------------------|---|
|Ösztönzők rendszergazdája|* Ösztönzők kezdeményezése és kezelése |[Ezekkel az erőforrásokkal segíthet az ösztönzők használatának első lépésekben](incentives-get-started-intro.md)
||* Megtekintheti és szerkesztheti az ösztönzőprogramok összes aspektusát
||* Megtekintheti és szerkesztheti a banki és adóadatokat
||* Az együttműködési bevételek megtekintése
||* Hozzáférés támogatása
||* A vitatás ösztönzőinek kifizetései|
|Ösztönzők felhasználója|* Megtekintheti az ösztönzőprogramokat
||* Megtekintheti és kezdeményezheti az ösztönzőkre vonatkozó igényeket
||* Az együttműködési bevételek megtekintése
||* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése

## <a name="view-partner-center-insights-data"></a>Az Partnerközpont Insights-adatok megtekintése

|**Szerepkör** | **Miket végezhet el?**|**További információ**|
|------------------------------|:-------------------------|---|
|Vezetői jelentésmegjelenítő|Hozzáférés az összes jelentéskészítési adatkészlethez, partnertámogatási jegyek létrehozása, a létrehozott partnertámogatási jegyek megtekintése|[A Partnerközpont Insightsban elérhető Partnerközpont irányítópult-jelentések](pci-overview-report.md)
|Jelentésmegjelenítő|Hozzáférés az adatjelentéshez a bevétel és az ügyfél és az alkalmazott személyes adatai kivételével, partnertámogatási jegyek létrehozása, a létrehozott partnertámogatási jegyek megtekintése|

## <a name="next-steps"></a>Következő lépések

- [Felhasználói fiókok létrehozása, illetve szerepkörök és engedélyek hozzárendelése](create-user-accounts-and-set-permissions.md)
- [Fiókinformációk ellenőrzése egy új Partnerközpont regisztrálva](verification-responses.md)
