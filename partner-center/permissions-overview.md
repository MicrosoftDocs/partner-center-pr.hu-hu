---
title: Szerepkörök & jogosultságok kiosztása a felhasználók számára
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogy mely szerepkörök a legmegfelelőbbek a vállalat azon felhasználói számára, akik kereskedelmi tranzakciókat, hivatkozásokat, ösztönzőket vagy MPN-tagságokat kezelnek a partner Centerben.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 80aeb62ba875d4ecd7c11063663f7c2d29912bdf
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492704"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Felhasználói szerepkörök és engedélyek kiosztása a vállalat felhasználói számára, akik a partner Centerben szeretnének dolgozni

**Megfelelő szerepkörök**

- Globális rendszergazda
- Felhasználói rendszergazda
- MPN-partner rendszergazdája

Beállította a partneri profilt, beleértve a jogi nevet és a címeket, a támogatási adatokat, a fájlokra vonatkozó adómentességeket, a banki adatokat és a vállalat elsődleges kapcsolattartóját. Következő lépés: szerezze be a felhasználókat jelszavakkal és szerepkörökkel, hogy megkezdődjön a partneri központban való munka.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Az alkalmazottak beállítása a partner Centerben való működésre

Ön határozza meg, hogy a felhasználók milyen típusú hozzáférési jogosultságokkal rendelkeznek a partnerek számára a szerepkörök és engedélyek használatával. A szerepkörök a vállalata által érintett program (ok) hoz kapcsolódnak. Ha például a vállalata egy felhőalapú megoldás-szolgáltató (CSP) vállalat, akkor nem csak a szokásos Azure Active Directory bérlői felügyeleti szerepköröket, például a globális rendszergazdát kell használnia, de a CSP-programra vonatkozó szerepkörökre lesz szüksége. Minden programhoz tartozik Szerepkörök.

>[!Note]
> Azure Active Directory bérlői szerepkörök közé tartozik a globális rendszergazda, a felhasználói rendszergazda és a CSP-szerepkörök. Nem Azure-Active-Directory szerepkörök azok a szerepkörök, amelyek nem kezelik a bérlőt, és tartalmazzák az MPN-rendszergazda, az üzleti profil rendszergazdája, az Ajánlói rendszergazda, az ösztönző rendszergazda és az ösztönző felhasználó. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Kereskedelmi tranzakciók kezelése a partner Centerben (Azure AD-és CSP-szerepkörök)

|**Szerepkör**|**Mit tehetnek**|**További információ**|
|----------------------------------|---|:---------------------------------|
|Globális rendszergazda|* Minden Microsoft-fiók/szolgáltatáshoz teljes körű jogosultságokkal férhet hozzá|[Partnerközponti fiók kezelése](partner-center-account-setup.md)
|      |* Támogatási jegyek létrehozása a partner központhoz
||* A létrehozott partneri támogatási jegyek megtekintése
||* Szerződések, árlista és ajánlatok megtekintése
||* Partner felhasználók megtekintése, létrehozása és kezelése|
||  Számlázás, számlák és felderítési fájlok megtekintése, létrehozása és kezelése
|Felhasználói felügyeleti rendszergazda   | * Felhasználók megtekintése, létrehozása és kezelése|[A Microsoft Partner Network tagsági előnyeinek és ajánlatának kezelése a partner Centerben](manage-your-partner-network-benefits.md)
||* Az összes partner Profil megtekintése
||* Támogatási jegyek létrehozása a partner központhoz
||* A létrehozott partneri támogatási jegyek megtekintése
|Számlázási adminisztrátor | -Számlázás, számlák és felderítési fájlok megtekintése, létrehozása és kezelése|[A számla elolvasása](billing.md)
||* Díjszabás megtekintése
||* Támogatási jegyek létrehozása a partner központhoz
||* A létrehozott partneri támogatási jegyek megtekintése
|Alapértelmezett felhasználó|  Saját profil megtekintése   |[Új jelszó kérése](reset-my-pasword.md)
|Felügyeleti ügynök | * Ügyfél-felügyelet|[Az ügyfélkapcsolatok szorosabbra fűzése](connect-with-your-customers.md)
||* Eszközök listájának hozzáadása a partner központhoz
||* Profilok létrehozása és alkalmazása eszközökre
||* Előfizetés-kezelés
||* Szolgáltatás állapotára és szolgáltatásra vonatkozó kérelmek ügyfelek számára
||* Delegált rendszergazdai jogosultságok kérése
||* Díjszabás és ajánlatok megtekintése
||* Számlázás
||* Felügyelet az ügyfél nevében
||* A hozzáadott értékkel rendelkező viszonteladó regisztrálása
||* Támogatási jegyek létrehozása a partner központhoz
||* A létrehozott partneri támogatási jegyek megtekintése|
|Értékesítési ügynök | * Ügyfél-felügyelet|[Számlázási támogatás biztosítása az ügyfelek számára, és a számlázási kérdések megválaszolása](provide-billing-support.md)
||* Eszközök listájának hozzáadása a partner központhoz
||* Előfizetés-kezelés
||* Támogatási jegyek megtekintése
||* Kapcsolat kérése egy ügyféllel
||* Díjszabás és ajánlatok megtekintése
||* Ügyfél-érdeklődők kezelése
||* Az ügyfél-szerződés megtekintése
||* Értéknövelt viszonteladó regisztrálása
||* Támogatási jegyek létrehozása a partner központhoz
||* A létrehozott partneri támogatási jegyek megtekintése|
|Segélyszolgálat ügynöke| * Ügyfél keresése és megtekintése|[A Microsofttal kapcsolatos problémák megismerése és a Microsoft-eszkalációval kapcsolatos problémák ismertetése](escalate-problems-to-microsoft.md)
||* Ügyfél adatainak szerkesztése
||* A számlázással és az előfizetés-kezeléssel kapcsolatos ügyfelekkel kapcsolatos problémák megoldása
||* Támogatás kérése az ügyfelek nevében 
||* Az előfizetések és a számlázási problémák kezelése az ügyfelek nevében
||* Támogatási jegyek létrehozása a partner központhoz
||* A létrehozott partneri támogatási jegyek megtekintése| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Vezérlőpult-gyártó (CPV). (CSP-szerepkör és nem Azure AD-szerepkör)

A CPVs a Cloud Solution Provider (CSP) partnerei által használható alkalmazások fejlesztésével lehetővé teszik a rendszerek integrálását a partner Center API-kkal. 

|**Szerepkör**   |**Miket végezhet el?**|**További információ**|
|------------------------------|:----------------------------|----|
|Globális rendszergazda| A CPV-Profil megtekintése és kezelése|[Regisztráció a felügyeleti panel gyártójával, amely segít a CSP-partneri rendszerek integrálásában a partner Center API-kkal](enroll-as-cpv.md)
||A CPV-képességekhez hozzáférést igénylő felhasználók megtekintése és kezelése|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a>Vendég felhasználó (hozzá kell adni a Azure Active Directory bérlőhöz)

|**Vendég felhasználó**   | **Szerepkörök**|
|---------------------------|:--------------------|
||MPN-partner rendszergazdája|
||Üzleti profil rendszergazdája|
||Ajánlói rendszergazda|


## <a name="manage-mpn-membership-and-your-company"></a>MPN-tagság és a vállalat kezelése 

Ezek a szerepkörök nem Azure Active Directory szerepkörök. Ezek a szerepkörök nem a bérlők, hanem a vállalat üzleti tevékenységét kezelik.

|**Szerepkör** | **Miket végezhet el?**|**További információ**|
|----------------------------|:----------------------------|-----|
|MPN-partner rendszergazdája|* Partner Service-kérelmek megtekintése, létrehozása és kezelése|[Microsoft Action Pack-előfizetés, illetve Silver és Gold kompetencia vásárlása vagy megújítása](mpn-get-action-pack.md)
||* Jogi, vállalati, üzleti és MPN-profilok megtekintése
||* A felhasználói adatok és a képzettségi adatok megtekintése
||* Kompetenciák megtekintése
||* Előnyök megtekintése és kezelése
||* MPN-ajánlatok megtekintése és vásárlása
||* Az MPN megtekintése a rendelési előzményeket és a számlákat
||* Partneri hozzájárulást jelző adatértékek megtekintése
||* Működhet a bizonylat-ellenőrzési eszközben|
||* Az ügyfél-adatelemzés megtekintése
||* Más felhasználói szerepkörök megtekintése a vállalaton belül, de nem rendelhet hozzá szerepköröket
||* Támogatási jegyek létrehozása a partner központhoz
||* A létrehozott partneri támogatási jegyek megtekintése
|Fiókadminisztrátor| Webhelyek hozzáadása|[Helyek kezelése](manage-locations.md)
|| A rendszergazda által használt fiókokhoz kapcsolódó profilok kezelése 
||* Szerepkörök kiosztása a bérlő felhasználói számára nem Azure-Active-Directory-szerepkörökhöz 
||* Webhelyek beléptetése programokba
||* Támogatási jegyek létrehozása a partner központhoz
||* A létrehozott partneri támogatási jegyek megtekintése

## <a name="manage-referrals"></a>Hivatkozások kezelése

> [!Note]
>Az új hivatkozói felhasználói szerepkör 2020. november 18-án kezdődik. A meglévő hivatkozó rendszergazdák megőrzik a teljes vállalatra kiterjedő hivatkozó rendszergazdai szerepkört.

|**Szerepkör** | **Miket végezhet el?**|**További információ**
|------------------------------|:-------------------------|---|
|Ajánlói rendszergazda|Mindent hozhat létre és kezelhet a partner Center átirányítási lapján|[Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)
||    Megtekintheti és szerkesztheti az összes közös értékesítési lehetőséget és érdeklődőt
||    Oszthatja ki a csoporttagokat egy üzlethez
||    Megtekintheti és szerkesztheti az üzleti profilokat
||    Megtekintheti és regisztrálhatja a megnyert és a Deal-regisztrációra jogosult lehetőségek ajánlatait
||    Támogatási jegyeket hozhat létre és tekinthet meg
|Hivatkozó felhasználók|Közös értékesítési lehetőségek létrehozása és kezelése csak akkor, ha a csoport részét képezik |[Együttes értékesítési lehetőségek kezelése](manage-co-sell-opportunities.md)
||    Közös értékesítési lehetőségeket hozhat létre azon helyekhez, amelyekhez hozzá van rendelve a szerepkör.
||    Megtekintheti és regisztrálhatja azokat a lehetőségeket, amelyek megnyertként vannak megjelölve, és jogosultak arra, hogy a csoport tagjai legyenek regisztrálva.
||    Támogatási jegyeket hozhat létre és tekinthet meg
|Üzleti profil rendszergazdája|Üzleti profilok létrehozása és kezelése | [Üzleti profilok kezelése](create-a-marketing-profile.md)
||    Támogatási jegyeket hozhat létre és tekinthet meg

Az új hivatkozói felhasználói szerepkörrel együtt a telephelyek hatókörét is bevezetjük a szolgáltatáshoz. Az alábbi táblázat az ajánlatok elérését mutatja be a hely alapján.

|**Hatókör** | **Miket végezhet el?** |
|------------------------------|:-------------------------|
|Teljes vállalat | A rendszergazdák és a felhasználók is hozzáférhetnek a vállalat bármely pontjához tartozó ajánlatok létrehozásához|
|| Az Ajánlói rendszergazda hozzáférhet az összes ajánlat megtekintéséhez és szerkesztéséhez |
|| Az átirányítási felhasználók csak akkor tekinthetik meg és szerkeszthetik az összes ügyletet, ha a csoport részét képezik. |
|Egy vagy több helyszín | A rendszergazdák és a felhasználók is hozzáférhetnek a vállalathoz rendelt helyhez kapcsolódó ajánlatok létrehozásához|
|| Az Ajánlói rendszergazda hozzáférhet a hozzárendelt helyszínekhez tartozó összes ajánlat megtekintéséhez és szerkesztéséhez|
|| A hivatkozó felhasználók hozzáférhetnek a hozzárendelt helyszínekhez tartozó összes ajánlat megtekintéséhez és szerkesztéséhez, ha azok a csapat részei.|

## <a name="manage-incentives"></a>Ösztönzők kezelése

|**Szerepkör** | **Miket végezhet el?**|**További információ**
|------------------------------|:-------------------------|---|
|Ösztönzők rendszergazdája|* Ösztönzők kezdeményezése és kezelése |[Az alábbi források segítséget nyújtanak az ösztönzők megkezdéséhez](incentives-get-started-intro.md)
||* Megtekintheti és szerkesztheti az ösztönző programok összes aspektusát
||* Megtekintheti és szerkesztheti a bank és az adó adatait
||* Az árengedmény és a Co-op bevételek megtekintése
||* Hozzáférés-támogatás
||* A vitatott ösztönzők kifizetése|
|Ösztönzők felhasználója|* Megtekintheti az ösztönző programokat
||* Megtekintheti és kezdeményezheti az ösztönző jogcímeket
||* Az árengedmény és a Co-op bevételek megtekintése
||* Támogatási jegyek létrehozása a partner központhoz
||* A létrehozott partneri támogatási jegyek megtekintése

## <a name="view-partner-center-insights-data"></a>A partneri központ adatelemzési szolgáltatásának megtekintése

|**Szerepkör** | **Miket végezhet el?**|**További információ**|
|------------------------------|:-------------------------|---|
|Executive Report Viewer|Hozzáférés az összes jelentési adatkészlethez, partneri támogatási jegyek létrehozásához, a létrehozott partneri támogatási jegyek megtekintése|[A partner Center-információk áttekintésében elérhető irányítópult-jelentések](pci-overview-report.md)
|Jelentés megjelenítője|Hozzáférés az adatjelentésekhez, a bevétel és az ügyfél és az alkalmazottak személyes adatkezelése kivételével, partneri támogatási jegyek létrehozása, partneri támogatási jegyek megtekintése|

## <a name="next-steps"></a>Következő lépések

- [Felhasználói fiókok létrehozása, illetve szerepkörök és engedélyek hozzárendelése](create-user-accounts-and-set-permissions.md)
- [Fiók adatainak ellenőrzése új partner Center-programban való regisztráláskor](verification-responses.md)
