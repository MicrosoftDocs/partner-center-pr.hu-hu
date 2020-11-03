---
title: SLA-jóváírás kérése a Microsofttól
ms.topic: article
ms.date: 04/28/2020
description: Megtudhatja, milyen előnyökkel, korlátozásokkal és eljárásokkal igényelhet szolgáltatói szerződést (SLA) a Microsofttól, ha az ügyfelek szolgáltatás-kimaradást tapasztalnak.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: cb8f6b2280318427b2015403b528fc288ef64d97
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/14/2020
ms.locfileid: "92527981"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Szolgáltatói szerződési (SLA-) kredit igénylése a Microsofttól

A Microsoft **szolgáltatói szerződési (SLA) kreditjét** is kérheti, ha az ügyfeleknek nyújtott szolgáltatás leállással rendelkezik.

## <a name="sla-credit-calculation"></a>SLA-jóváírások kiszámítása

A Microsofttól származó SLA-kreditek az érintett szolgáltatás (ok) alapján vannak meghatározva. Ha például az ügyfél rendelkezik Office 365 Suite-csomaggal, de csak SharePoint-kimaradást észlelt, az SLA-kreditek csak a SharePoint rendszerre érvényesek, és nem az ügyfél teljes csomagját.

*A kreditek az érintett szolgáltatás és a leállás időtartama alapján lesznek Pro-értékelve.* Az SLA-kreditekre jogosító forgatókönyvek típusait az [online szolgáltatások összevont SLA-dokumentumában](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)tekintheti meg. Ezek az információk a Cloud Solution Provider programon keresztül eladott szolgáltatásokra vonatkoznak.

## <a name="request-an-sla-credit"></a>SLA-kredit igénylése

*A felhőalapú megoldás szolgáltatójának (CSP) partnerének a következő naptári hónap végéig kell elküldenie a jogcímet és az összes szükséges információt.* Ha például az incidens február 15-én fordult elő, a Microsoftnak március 31-ig kell megkapnia a jogcímet és az összes szükséges információt. A végfelhasználók és a közvetett viszonteladók nem nyújthatnak be SLA-jóváírási jogcímeket; vagy a közvetett szolgáltató vagy a közvetlen számla partnernek az Ön nevében kell benyújtania a jogcímeket.

### <a name="required-information"></a>Szükséges információk

Mielőtt [elküld egy SLA-jóváírási kérést](#submit-sla-credit-request) a Microsoftnak, össze kell gyűjtenie az alábbi információkat a támogatási jegybe való felvételhez:

- Az ügyfél bérlője GUID azonosítója
- A [leállás incidensének azonosítója](#outage-incident-identifier)?
- A CSP-n keresztül vásároltak-e érintett előfizetéseket? ( *Igen* vagy *nem* )

#### <a name="outage-incident-identifier"></a>Kimaradási incidens azonosítója

A leállás incidens azonosítóját a Microsoft 365 felügyeleti központban található **Service Health** lapon találja. Az **kimaradási incidens azonosítója** az érintett szolgáltatást (például az Exchange Online-kimaradás *EX25194* ) jelző kétbetűs rövidítéssel megelőzően megadott szám. A következő táblázat a gyakori szolgáltatások rövidítéseit ismerteti:

| Kétbetűs rövidítés | Microsoft-szolgáltatás |
| ----------------------- | ----------------- |
| PÉLDÁUL | Exchange Online |
| UTCÁN | Exchange Online-védelem |
| SB | Skype vállalati online verzió (korábban Lync Online) |
| Operációs rendszer | Office-előfizetés |
| PB | Office 365-höz készült Power BI |
| SP | SharePoint Online |
| YA | Yammer Enterprise |
| MO | Portál-hiba |

### <a name="submit-sla-credit-request"></a>SLA-jóváírási kérelem beküldése

Az SLA-jóváírási kérelem küldése a Microsoftnak a partner Center irányítópultján:

1. Jelentkezzen be a partner Center irányítópultra.
2. A bal oldali menüben válassza a **szolgáltatáskérelmek** lehetőséget, majd válassza a **partneri támogatási kérelmek** lehetőséget.
3. A **partneri kérelem** lapon válassza az **új kérelem** lehetőséget.
4. A **kérelem indítása** lapon keresse meg a **CSP-ügyfelek, megrendelések és előfizetések** szakaszt. Ebben a szakaszban válassza a **probléma típusának kiválasztása** , majd az **ügyfél-szolgáltatási jóváírások** lehetőséget.
5. Az **ajánlott megoldások** lapon a **további segítségre van szüksége?** területen válassza az **Igen** lehetőséget.
6. A **részletek** lapon töltse ki a **probléma részletei** szakaszt. A **részletek** szövegmezőben ügyeljen arra, hogy a korábban összegyűjtött [szükséges adatokat](#required-information) adja meg.
7. Válassza a **Submit (Küldés** ) lehetőséget az SLA-jóváírási kérelem küldéséhez.
