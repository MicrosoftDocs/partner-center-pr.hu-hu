---
title: Szerepkörök hozzárendelése & engedélyek hozzárendelése felhasználókhoz
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, mely szerepkörök a legmegfelelőbbek a vállalat kereskedelmi tranzakciókat, terjesztéseket, ösztönzőket vagy MPN-tagságokat Partnerközpont.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: b1ac34bbb92d600805465ca5f6d1b28af54cd5e1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855131"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Felhasználói szerepkörök és engedélyek hozzárendelése olyan vállalati felhasználókhoz, akik a vállalaton belül Partnerközpont

**Megfelelő szerepkörök:** Globális rendszergazdai | Felhasználókezelési rendszergazdai | MPN-partner rendszergazdája

Beállította partnerprofilját, amely tartalmazza a jogi nevet és címet, a támogatási adatokat, a fájl-adómentességet, a banki adatokat és a vállalat elsődleges kapcsolattartóját. Következő lépés: Állítsa be a felhasználók számára a jelszavakat és a szerepköröket, hogy megkezdjék Partnerközpont munkát.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Az alkalmazottak beállítása a Partnerközpont

Ön határozza meg, hogy a felhasználók milyen típusú hozzáféréseket Partnerközpont az Ön által adott szerepkörök és engedélyek alapján. A szerepkörök ahhoz a programhoz vagy programokhoz kapcsolódnak, amelyekben a vállalat részt vesz. Ha például a vállalata egy Felhőszolgáltató- (CSP-) vállalat, nem csupán a szabványos Azure Active Directory-bérlői felügyeleti szerepkörökkel, például a globális rendszergazdával rendelkezik, hanem a CSP-programra jellemző szerepkörökre is szüksége lesz. Minden program saját szerepkörökkel rendelkezik.

>[!Note]
> Azure Active Directory a globális rendszergazdai, felhasználói rendszergazdai és CSP-szerepkörök. A nem Azure-Active-Directory szerepkörök azok a szerepkörök, amelyek nem kezelik a bérlőt, és mpN-rendszergazdai, üzletiprofil-rendszergazdai, ajánlói rendszergazdai, ösztönzőrendszergazdát és ösztönzőfelhasználót tartalmaznak. 

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
|Értékesítési ügynök | * Ügyfélkezelés|[Számlázási támogatás biztosítanak az ügyfelek számára, és segítenek megválaszolni a számlázási kérdéseket](provide-billing-support.md)
||* Eszközlista hozzáadása a Partnerközpont
||* Előfizetés-kezelés
||* Támogatási jegyek megtekintése
||* Kapcsolat kérése egy ügyféllel
||* Díjszabás és ajánlatok megtekintése
||* Ügyfelek érdeklődők kezelése
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

A CPV-k az Felhőszolgáltató (CSP) partnerek által használt alkalmazásokat fejlesztnek, amelyek lehetővé teszik számukra, hogy rendszereiket integrálják Partnerközpont API-okkal. 

|**Szerepkör**   |**Miket végezhet el?**|**További információ**|
|------------------------------|:----------------------------|----|
|Globális rendszergazda| CPV-profil megtekintése és kezelése|[Regisztrálás Vezérlőpult a CSP-partnerrendszerek és az Partnerközpont API-k integrálásához](enroll-as-cpv.md)
||A CPV-képességekhez hozzáféréssel bíró felhasználók megtekintése és kezelése|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a>Vendégfelhasználó (hozzá kell adni a Azure Active Directory bérlőhöz)

|**Vendégfelhasználó**   | **Szerepkörök**|
|---------------------------|:--------------------|
||MPN-partner rendszergazdája|
||Üzletiprofil-rendszergazda|
||Ajánlói rendszergazda|


## <a name="manage-mpn-membership-and-your-company"></a>MPN-tagság és a vállalat kezelése 

Ezek a szerepkörök nem Azure Active Directory szerepkörök. Ezek a szerepkörök nem a bérlőt, hanem a vállalat vállalatát kezelik.

|**Szerepkör** | **Miket végezhet el?**|**További információ**|
|----------------------------|:----------------------------|-----|
|MPN-partneri rendszergazda|* Partnerszolgáltatás-kérelmek megtekintése, létrehozása és kezelése|[Microsoft Action Pack-előfizetés, illetve Silver és Gold kompetencia vásárlása vagy megújítása](mpn-get-action-pack.md)
||* Jogi, vállalati, üzleti és MPN-profilok megtekintése
||* Felhasználói adatok és képzettségi adatok megtekintése
||* Kompetenciák megtekintése
||* Előnyök megtekintése és kezelése
||* MPN-ajánlatok megtekintése és vásárlása
||* Az MPN-ajánlatok rendelési előzményeinek és számláinak megtekintése
||* Partneri hozzájárulási mutatók adatainak megtekintése
||* Használható a érvényesítési eszközben|
||* Ügyféladatok elemzésének megtekintése
||* Megtekintheti a vállalaton belüli más felhasználói szerepköröket, de nem rendelhet hozzájuk szerepköröket
||* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése
|Fiókadminisztrátor| Helyek hozzáadása|[Helyek kezelése](manage-locations.md)
|| A rendszergazdai fiókokkal kapcsolatos profilok kezelése 
||* Szerepkörök hozzárendelése a bérlőn lévő felhasználókhoz nem Azure-Active-Directory-szerepkörökhöz 
||* Helyek regisztrálása programokba
||* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése

## <a name="manage-referrals"></a>Hivatkozások kezelése

|**Szerepkör** | **Miket végezhet el?**|**További információ**
|------------------------------|:-------------------------|---|
|Ajánlói rendszergazda|Hozzon létre és kezeljen mindent az Partnerközpont|[Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)
||    Megtekintheti és szerkesztheti az összes közös értékesítési lehetőséget és érdeklődőt
||    Csapattagokat rendelhet hozzá egy ajánlathoz
||    Megtekintheti és szerkesztheti az üzleti profilokat
||    Megtekintheti és regisztrálhatja az ügyleteket az olyan lehetőségekhez, amelyek megnyertként vannak megjelölve, és jogosultak az ügylet regisztrációra
||    Létrehozhat és megtekinthet támogatási jegyeket
|Ajánlói felhasználó|Az közös értékesítés lehetőségeinek létrehozása és kezelése csak akkor, ha tagjai a csapatnak |[Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)
||    Közös értékesítési lehetőségeket hozhat létre azokkal a helyekkel, amelyekhez hozzá vannak rendelve a szerepkör.
||    Megtekintheti és regisztrálhatja az ügyleteket az olyan lehetőségekhez, amelyek megnyertként vannak megjelölve, és jogosultak az ügylet regisztrációra, ha csapattagok.
||    Létrehozhat és megtekinthet támogatási jegyeket
|Üzletiprofil-rendszergazda|Üzleti profilok létrehozása és kezelése | [Üzleti profilok kezelése](create-a-marketing-profile.md)
||    Létrehozhat és megtekinthet támogatási jegyeket

Az új javaslati felhasználói szerepkör mellett bemutatjuk az ügyletek helyének hatókörét is. Az alábbi táblázat a hely alapján mutatja be az ügyletekhez való hozzáférést.

|**Hatókör** | **Miket végezhet el?** |
|------------------------------|:-------------------------|
|Az egész vállalat | A rendszergazdák és a felhasználók is hozzáférhetnek a vállalatuk bármely helyével kötött ügyletek létrehozásához|
|| A ajánló rendszergazda hozzáfér az összes ügylet megtekintéséhez és szerkesztéséhez |
|| A ajánló felhasználók csak akkor férhetnek hozzá az összes ügylet megtekintéséhez és szerkesztéséhez, ha tagjai a csapatnak |
|Egy vagy több hely | A rendszergazdák és a felhasználók egyaránt hozzáférhetnek a vállalatukhoz rendelt helyre vonatkozó ügyletek létrehozásához|
|| A ajánló rendszergazdának hozzáférése van a hozzárendelt helyekhez tartozó összes ügylet megtekintéséhez és szerkesztéséhez|
|| A ajánló felhasználók megtekinthetik és szerkeszthetik a hozzárendelt helyekhez tartozó összes ügyletet, ha tagjai a csapatnak|

## <a name="manage-incentives"></a>Ösztönzők kezelése

|**Szerepkör** | **Miket végezhet el?**|**További információ**
|------------------------------|:-------------------------|---|
|Ösztönzők rendszergazdája|* Ösztönzőket kezdeményez és kezel |[Ezekkel az erőforrásokkal elkezdeni az ösztönzők használatát](incentives-get-started-intro.md)
||* Megtekintheti és szerkesztheti az ösztönzőprogramok összes aspektusát
||* Megtekintheti és szerkesztheti a banki és adóadatokat
||* Az együttműködési bevételek megtekintése
||* Hozzáférés-támogatás
||* Vitatáson áteső ösztönzők kifizetései|
|Ösztönzők felhasználója|* Megtekintheti az ösztönzőprogramokat
||* Megtekintheti és kezdeményezheti az ösztönzőkre vonatkozó igényeket
||* Az együttműködési bevételek megtekintése
||* Támogatási jegyek létrehozása a Partnerközpont
||* A létrehozott partnertámogatási jegyek megtekintése

## <a name="view-partner-center-insights-data"></a>Az Partnerközpont Insights-adatok megtekintése

|**Szerepkör** | **Miket végezhet el?**|**További információ**|
|------------------------------|:-------------------------|---|
|Vezetői jelentésmegjelenítő|Hozzáférés az összes jelentéskészítési adatkészlethez, partnertámogatási jegyek létrehozása, a létrehozott partnertámogatási jegyek megtekintése|[A Partnerközpont Insightsban elérhető Partnerközpont irányítópult-jelentések](pci-overview-report.md)
|Jelentésmegjelenítő|Hozzáférés az adatjelentésekhez a bevétel és az ügyfél és az alkalmazott személyes adatai kivételével, partnertámogatási jegyek létrehozása, a létrehozott partnertámogatási jegyek megtekintése|

## <a name="next-steps"></a>Következő lépések

- [Felhasználói fiókok létrehozása, illetve szerepkörök és engedélyek hozzárendelése](create-user-accounts-and-set-permissions.md)
- [Fiókinformációk ellenőrzése egy új Partnerközpont regisztrálva](verification-responses.md)
