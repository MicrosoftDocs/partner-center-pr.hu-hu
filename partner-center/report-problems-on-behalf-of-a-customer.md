---
title: Problémabejelentés ügyfél nevében
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, mikor kell eszkalálni egy ügyfélszolgálati problémát a Microsoftnak, és hogyan lehet támogatási jegyet be Microsoft-szolgáltatások.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f67a3b6a403f09cb773a5ca663d6cf6db1b03e2e
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018118"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Szolgáltatási probléma jelentése egy ügyfél nevében – beleértve azt is, hogy mikor és hogyan kell ezt megtenni

**A következőre érvényes:**

- A Microsoft Cloud for US Government Partnerközpontja

**Megfelelő szerepkörök**

- Globális rendszergazda

Ha az ügyfél olyan szolgáltatásproblémát tapasztal, amely nem oldható meg, és amely megfelel a Problémák eszkalációja a [Microsoftnak](escalate-problems-to-microsoft.md)feltételeinek, a közvetett szolgáltató támogatási jegyet tud bejegyzni számukra. Ez a folyamat a számlázási problémák vagy vitatások eszkalálására, valamint csalással kapcsolatos problémák esetén is hasznos.

## <a name="submit-a-service-request-for-a-customer"></a>Szolgáltatáskérés elküldése egy ügyfélnek

1. A CSP Partnerközpont menüjében válassza az Ügyfelek **lehetőséget.**

2. Az Ügyfelek lapon válassza ki a kívánt ügyfelet, vagy keressen rá rá
    
3. Az ügyfél menüjében válassza a **Szolgáltatáskérések elemet**

4. Az Új **kérés legördülő** menüben válassza az **Azure** vagy az **Office 365, Dynamics 365, Nagyvállalati mobilitási csomag lehetőséget.** A rendszer átirányítja a Microsoft Azure Portal Office 365 felügyeleti központjába.

>[!NOTE]
>A Dynamics 365-öt CSP-ben tranzakciós támogatási műveleti partnereknek fenn kell tartaniuk a partneri (ASfP) csomagra vagy annál magasabb szintű támogatási szerződésre vonatkozó támogatási szerződést. Ez a támogatási szerződés szükséges a Dynamics 365-incidensek CSP-ügyfél nevében történő elküldéhez. [További információ](https://partner.microsoft.com/support/partnersupport) a támogatási szerződés lehetőségeiről.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Ha szolgáltatáskérést kell létrehoznia az ügyfél számára az Azure-ban, vegye figyelembe a következőket:
>
>- Ahhoz, hogy Ön, mint közvetett viszonteladó szolgáltatási kéréseket hoz létre az Azure-beli ügyfél számára, a közvetett szolgáltatónak hozzáférést kell rendelnie Az ügyfél Azure-fiókjához. Ez eltér az Office 365-ügyfelek nevében történő felügyelettől.
>
>- Bár az Partnerközpont ügyfélszolgálati rendszergazdája nem tud szolgáltatáskéréseket létrehozni az Azure szolgáltatásportálon, létrehozhatnak egy támogatási csoportot az Azure szolgáltatási portálon, és engedélyt adhatnak a csoportnak a támogatási kérelmek naplózására.

1. Válassza az **Új támogatási kérelem** lehetőséget.

2. Adja meg a megfelelő információkat a támogatási kérésben, majd válassza a **Létrehozás lehetőséget:**

   - A támogatási kérelem Alapvető **beállítások** szakaszában válassza  az Felhőszolgáltató **mezőben.**

   - A támogatási **kérelem Kapcsolattartási** adatok szakaszában adja meg az adatait, ne az ügyfél adatait.

3. Később tekintse át az ügyfél szolgáltatási kérését a Microsoft Azure Portal **a Támogatási kérelmek kezelése lehetőség kiválasztásával.**

Előfordulhat, hogy támogatási kérést kell létrehoznia egy ügyfélhez, ha nem rendelkezik rendszergazdai engedélyekkel az adott ügyfélhez. Ez két forgatókönyv egyikében fordulhat elő:

- Nem kért rendszergazdai jogosultságokat a kapcsolat első létrejöttekor.
- Ön csak az ügyfél Azure-előfizetését kezeli, így nem rendelkezik rendszergazdai engedélyekkel.
 
Ezekben az esetekben az alábbi eljárással hozhat létre támogatási kérést. 

1. Másolja ki az ügyfél tartománynevét a fiókoldalról a Partnerközpont.

2. Ugrás https://portal.azure.com/ a[customerdomainname] elemre. 

3. Válassza ki a támogatást igénylő Azure-előfizetést.

4. Válassza **az Új támogatási kérelem** lehetőséget, majd kövesse az utasításokat a kérés létrehozásához. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Nagyvállalati mobilitási csomag

1. A **Szolgáltatáskérés létrehozása szakaszban** válassza ki a megfelelő támogatási kategóriát. Előfordulhat, hogy további cikkek **megtekintéséhez a További...** lehetőséget kell választania.

2. Töltse ki a szolgáltatáskérési űrlapot, majd válassza a **Küldés lehetőséget.**

   > [!TIP]
   > Ügyeljen arra, hogy a kapcsolattartási adatait tartalmazza, ne az ügyfélét.

3. Később tekintse át az ügyfél szolgáltatáskéréseit az Office 365 Felügyeleti központban, és válassza az **Összes támogatási jegy áttekintése et.**

### <a name="support-for-commercial-marketplace-products"></a>A kereskedelmi piactéren elérhető termékek támogatása

A Microsoft nem nyújt terméktámogatást a kereskedelmi piactéren elérhető termékekhez. A támogatáshoz a független szoftverszállítóhoz (ISV) kell kapcsolatba lépnie, aki közzétette a terméket.

Az ISV kapcsolattartási adatait a következővel találhatja meg:

1.  A **Marketplace lapon** válassza ki azt a terméket, amelyhez segítségre van szüksége.

2.  A termék oldalán támogatási kapcsolattartási adatokat talál. Ez a következő lehetőségek közül egy vagy több lehet:

    - Az ISV webhelyén található támogatási belépési pontra mutató hivatkozás
    - Támogatási e-mail
    - Támogatási kapcsolattartó telefonszáma

## <a name="faq"></a>GYIK

Tekintse meg az alábbi gyakori kérdéseket az ügyfelek nevében beküldhető szolgáltatáskérésekkel kapcsolatban. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>Mit tartalmaz a támogatási jogosultság?

A szolgáltatáskéréseket a szolgáltatáson keresztül kell Partnerközpont. Elérhetők az Azure, a Microsoft Office 365, a Microsoft Dynamics CRM Online és a Nagyvállalati mobilitási csomag számára. A Felhőszolgáltató programban részt vevő partnerként számíthat a nagyobb problémákra adott prioritású válaszidőre.

A saját partnerbérlő támogatása nem része a CSP támogatási juttatásnak. Az Office 365, Microsoft Dynamics CRM Online és a Nagyvállalati mobilitási csomag azonban nem számít fel külön támogatási előfizetési díjat a partnerek vagy ügyfelek számára. Az Azure díjat számít fel, de ha ön jogosult Signature Felhőtámogatás vagy más Microsoft Partner Network(MPN) előnyeire, akkor ezeket az előnyöket használhatja a díj fizetésére.

Ez az előny a Felhőszolgáltató programban részt vevő összes partnerre vonatkozik, akár fizetős, akár próbaidőszakban. A csomag ingyenes összetevője a számlázási és előfizetés-kezelési támogatás is.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Milyen gyorsan kapok kezdeti választ?

A kezdeti válaszidő a beküldött incidens súlyosságától függ. A probléma súlyosságát a szolgáltatáskérés elküldésekor az üzletre gyakorolt hatásra utaló jelzés határozza meg.

A műszaki **hibajavítási incidensek kezdeti válaszideje:**

- Kritikus hatás (A súlyosság): Két óra (a szolgáltatások jelentős elvesztése vagy csökkenése. Az éles szolgáltatások leálltak.)
- Közepes hatás (B súlyosság): Négy óra (a szolgáltatások közepes mértékű elvesztése vagy csökkenése). Az éles szolgáltatások részben érintettek.)
- Minimális hatás (C súlyosság): Nyolc óra (a szolgáltatások minimális elvesztése vagy romlása. A továbbra is elérhető vagy nem éles szolgáltatások érintettek.)

A kezdeti válaszidők csak angol nyelvű támogatáshoz vannak megszabadulva. A helyi nyelvi támogatás munkaidőben biztosított.
Az olyan incidensek esetén, amelyek a támogatási jogosultság határain belülre esnek, de nem minősülnek javításra képes incidensnek, a kezdeti válaszidő akár egy nap is lehet.

### <a name="can-i-submit-a-service-request-by-phone"></a>Küldhetek szolgáltatáskérést telefonon?

Nem, ehhez a programhoz nem áll rendelkezésre telefonos támogatás.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Mi történik, ha bejelentkezek a Azure Portal és kihagyom a Partnerközpont?

Ha közvetlenül jelentkezik be a Microsoft Azure Portal, akkor a központot a saját környezetében, nem pedig az ügyfél környezetében nézi meg. Ezért csak akkor jelentkezzen be közvetlenül a Microsoft Azure Portal amikor saját előfizetéséhez hoz létre szolgáltatáskérést.

A CSP-program támogatási jogosultsága nem biztosít támogatást a saját Partner-előfizetésében. Emiatt érvényes támogatási csomagja jogosultságát kell adnia, amikor olyan szolgáltatáskérést hoz létre, amely a saját partner-előfizetésére vonatkozik. Ilyen például az MPN-szerződés azonosítója, a Premier vagy Azure-támogatás csomag. További információt a gyakori kérdések [Azure ügyfélszolgálata talál.](https://go.microsoft.com/fwlink/?LinkId=717532)

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Mi történik, ha bejelentkezek az Office 365 Felügyeleti központ portálra, és kihagyom a Partnerközpont?

Ha közvetlenül az Office 365 felügyeleti központjába jelentkezik be, a központot a saját környezetében, nem pedig az ügyfél környezetében nézi meg. Ezért csak akkor jelentkezzen be közvetlenül az Office 365 Felügyeleti központba, amikor saját előfizetéséhez hoz létre szolgáltatáskérést.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Hogyan Dynamics 365 további támogatását?

Ha a következő problémákat tapasztalja: Dynamics 365-csomag előfizetései, Licencelés, Számlázás, Finance & Operations, Dynamics 365-terméklicencek, vagy további technikai támogatásra van szüksége:
 
Kapcsolatfelvétel a [Dynamics ügyfélszolgálatával](/dynamics365/customer-engagement/admin/contact-technical-support)

## <a name="next-steps"></a>Következő lépések

- [Támogatás biztosítása az ügyfeleknek](customer-support.md)
- [A szolgáltatás állapotának ellenőrzése](check-service-health.md)
