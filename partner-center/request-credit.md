---
title: SLA-jóváírás kérése a Microsofttól
ms.topic: article
ms.date: 03/31/2021
description: Megtudhatja, milyen előnyökkel, korlátozásokkal és eljárásokkal kérhet szolgáltatói szerződési (SLA-) jóváírást a Microsofttól, ha az ügyfelek szolgáltatáskimaradást tapasztalnak.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 4a8e785de051aa6f722a1bfddc4ad83d6502bbb3
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551656"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Hogyan és mikor kell szolgáltatásiszint-szerződési (SLA-) jóváírást igényelni a Microsofttól

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Globális rendszergazda

**Szolgáltatásiszint-szerződési (SLA-)** jóváírást kérhet a Microsofttól, ha egy Ön által az ügyfelek számára nyújtott szolgáltatás szolgáltatáskimaradást igényel.

## <a name="sla-credit-calculation"></a>SLA-jóváírás kiszámítása

A Microsoft SLA-jóváírásai az alapján vannak meghatározva, hogy melyik szolgáltatás(ak)t érintették. Ha például az ügyfél rendelkezik Office 365-csomagtal, de csak SharePoint-kimaradást tapasztalt, az SLA-jóváírás csak a SharePointhoz lesz jóváhagyva, az ügyfél teljes csomagja nem.

*A kreditek minősítése az érintett szolgáltatástól és a szolgáltatáskimaradás időtartamától függ.* Az SLA-jóváírásra jogosult forgatókönyvek típusait az Online Szolgáltatások összevont [SLA-dokumentumában láthatja.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Ezek az információk a Felhőszolgáltató (CSP) programon keresztül értékesített szolgáltatásokra is vonatkoznak.


## <a name="request-an-sla-credit"></a>SLA-jóváírás igénylése

*A CSP-partnernek be kell nyújtania az igényt és az összes szükséges információt az incidens beeseményének hónapját követő naptári hónap végéig.* Ha például az incidens február 15-én történt, a Microsoftnak március 31-ig meg kell kapnia az igényt és az összes szükséges információt. A végfelhasználók és a közvetett viszonteladók nem küldhetnek be SLA-jóváírási igényeket; A közvetett szolgáltatónak vagy a közvetlen számlázási partnernek be kell nyújtania a jogcímeket a nevükben.

>[!NOTE]
>A tanácsadási incidensek (A Microsoft 365[állapotának ellenőrzése)](/microsoft-365/enterprise/view-service-health#incidents-and-advisories)nem jogosultak SLA-jóváírásra.

### <a name="required-information"></a>Szükséges információk

Az ügyfélnév, a bérlőazonosító, a partnerjegy# és a jegy által létrehozott dátum-/időbélyeg nem elegendő a jogcím feldolgozásához.

Mielőtt [SLA-jóváírási](#submit-sla-credit-request) kérelmet küld a  Microsoftnak, össze kell gyűjtenie az összes alábbi információt, hogy szerepeljen a támogatási jegyben:

- Az ügyfélbérlő GUID-ja
- A [kimaradási incidens azonosítója?](#outage-incident-identifier)
- Annak bizonyítéka, hogy az ügyfelet a kimaradás érintette, és SLA-jóváírást kért.
- Az érintett előfizetéseket CSP-ről vásároltak? (*igen vagy* *nem*)

#### <a name="evidence-that-proves-customer-impact"></a>Az ügyfélre gyakorolt hatást bizonyító bizonyítékok

- Az állásidő időtartamával és időtartamával kapcsolatos információk
- Az érintett felhasználók száma és helye (ha van)
- Az incidens megoldására tett kísérletek leírása az előforduláskor
- Az érintett ügyféltől származó e-mail, amely támogatást kér, majd jóváírást kér
- A támogatási jegy száma és az ügyfélkapcsolat adatai a szolgáltatásra gyakorolt hatás megoldása kapcsán


#### <a name="outage-incident-identifier"></a>Kimaradás incidensazonosítója

A kimaradás esetének azonosítóját a Service Health **oldalán** találja Microsoft 365 Felügyeleti központ. A **szolgáltatáskimaradási** incidens azonosítója egy olyan szám, amelyet kétbetűs rövidítés előz meg, amely az érintett szolgáltatást jelzi (például *EX25194* Exchange Online-szolgáltatáskimaradás esetén). A következő táblázat a szolgáltatások gyakori rövidítését ismerteti:

| Kétbetűs rövidítés | Microsoft-szolgáltatás |
| ----------------------- | ----------------- |
| Ex | Exchange Online |
| FO | Exchange Online Protection |
| Sb | Skype Vállalati online verzió (korábban Lync Online) |
| Operációs rendszer | Office-előfizetés |
| PB | Office 365-höz készült Power BI |
| Sp | SharePoint Online |
| Ya | Yammer Enterprise |
| MO | Portálhiba |

### <a name="submit-sla-credit-request"></a>SLA-jóváírási kérelem elküldése

Az SLA-jóváírási kérés elküldése a Microsoftnak az Partnerközpont irányítópulton:

1. Jelentkezzen be a Partnerközpont irányítópultjába.
2. A bal oldali menüben válassza a **Szolgáltatáskérések** elemet, majd a **Partnertámogatási kérelmek elemet.**
3. A **Partnerkérés lapon** válassza az Új **kérelem lehetőséget.**
4. A **Kérés kezdete lapon** keresse meg a CSP szakaszt **: ügyfelek, megrendelések és előfizetések.** Ebben a szakaszban válassza a Válasszon ki **egy problématípust** lehetőséget, majd válassza az **Ügyfélszolgálati jóváírási kérések lehetőséget.**
5. Az Ajánlott **megoldások oldalon** a További segítségre van **szüksége?** alatt válassza az **Igen lehetőséget.**
6. A Részletek **lapon** töltse ki a **Probléma részletei szakaszt.** A **Részletek szövegmezőben** adja meg a korábban összegyűjtött [szükséges](#required-information) adatokat.
7. Válassza **a Küldés** lehetőséget az SLA-jóváírási kérelemben való küldéshez.

## <a name="next-steps"></a>Következő lépések

- [Problémák jelentése az ügyfél nevében](report-problems-on-behalf-of-a-customer.md)
