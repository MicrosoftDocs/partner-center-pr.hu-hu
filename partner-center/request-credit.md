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
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a><span data-ttu-id="f45e1-103">Szolgáltatói szerződési (SLA-) kredit igénylése a Microsofttól</span><span class="sxs-lookup"><span data-stu-id="f45e1-103">How and when to request a service-level agreement (SLA) credit from Microsoft</span></span>

<span data-ttu-id="f45e1-104">A Microsoft **szolgáltatói szerződési (SLA) kreditjét** is kérheti, ha az ügyfeleknek nyújtott szolgáltatás leállással rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="f45e1-104">You're able to request **service-level agreement (SLA) credits** from Microsoft if a service that you're providing for your customers has an outage.</span></span>

## <a name="sla-credit-calculation"></a><span data-ttu-id="f45e1-105">SLA-jóváírások kiszámítása</span><span class="sxs-lookup"><span data-stu-id="f45e1-105">SLA credit calculation</span></span>

<span data-ttu-id="f45e1-106">A Microsofttól származó SLA-kreditek az érintett szolgáltatás (ok) alapján vannak meghatározva.</span><span class="sxs-lookup"><span data-stu-id="f45e1-106">SLA credits from Microsoft are determined based on which service(s) were impacted.</span></span> <span data-ttu-id="f45e1-107">Ha például az ügyfél rendelkezik Office 365 Suite-csomaggal, de csak SharePoint-kimaradást észlelt, az SLA-kreditek csak a SharePoint rendszerre érvényesek, és nem az ügyfél teljes csomagját.</span><span class="sxs-lookup"><span data-stu-id="f45e1-107">For example, if your customer has an Office 365 suite but only experienced a SharePoint outage, the SLA credit is approved only for SharePoint and not the customer's entire plan.</span></span>

<span data-ttu-id="f45e1-108">*A kreditek az érintett szolgáltatás és a leállás időtartama alapján lesznek Pro-értékelve.*</span><span class="sxs-lookup"><span data-stu-id="f45e1-108">*Credits are pro-rated based on the service affected and the duration of the outage.*</span></span> <span data-ttu-id="f45e1-109">Az SLA-kreditekre jogosító forgatókönyvek típusait az [online szolgáltatások összevont SLA-dokumentumában](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)tekintheti meg.</span><span class="sxs-lookup"><span data-stu-id="f45e1-109">To see the types of scenarios that qualify for SLA credits, see the [Online Services Consolidated SLA document](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37).</span></span> <span data-ttu-id="f45e1-110">Ezek az információk a Cloud Solution Provider programon keresztül eladott szolgáltatásokra vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="f45e1-110">This information applies to services sold through the Cloud Solution Provider program, too.</span></span>

## <a name="request-an-sla-credit"></a><span data-ttu-id="f45e1-111">SLA-kredit igénylése</span><span class="sxs-lookup"><span data-stu-id="f45e1-111">Request an SLA credit</span></span>

<span data-ttu-id="f45e1-112">*A felhőalapú megoldás szolgáltatójának (CSP) partnerének a következő naptári hónap végéig kell elküldenie a jogcímet és az összes szükséges információt.*</span><span class="sxs-lookup"><span data-stu-id="f45e1-112">*The Cloud Solution Provider (CSP) partner must submit the claim and all required information by the end of the calendar month following the month in which the incident occurred.*</span></span> <span data-ttu-id="f45e1-113">Ha például az incidens február 15-én fordult elő, a Microsoftnak március 31-ig kell megkapnia a jogcímet és az összes szükséges információt.</span><span class="sxs-lookup"><span data-stu-id="f45e1-113">For example, if the incident occurred on February 15th, Microsoft must receive the claim and all required information by March 31st.</span></span> <span data-ttu-id="f45e1-114">A végfelhasználók és a közvetett viszonteladók nem nyújthatnak be SLA-jóváírási jogcímeket; vagy a közvetett szolgáltató vagy a közvetlen számla partnernek az Ön nevében kell benyújtania a jogcímeket.</span><span class="sxs-lookup"><span data-stu-id="f45e1-114">End customers and indirect resellers can't submit SLA credit claims; either the indirect provider or direct bill partner must submit claims on their behalf.</span></span>

### <a name="required-information"></a><span data-ttu-id="f45e1-115">Szükséges információk</span><span class="sxs-lookup"><span data-stu-id="f45e1-115">Required information</span></span>

<span data-ttu-id="f45e1-116">Mielőtt [elküld egy SLA-jóváírási kérést](#submit-sla-credit-request) a Microsoftnak, össze kell gyűjtenie az alábbi információkat a támogatási jegybe való felvételhez:</span><span class="sxs-lookup"><span data-stu-id="f45e1-116">Before you [submit an SLA credit request](#submit-sla-credit-request) to Microsoft, you must gather the following information to include in your support ticket:</span></span>

- <span data-ttu-id="f45e1-117">Az ügyfél bérlője GUID azonosítója</span><span class="sxs-lookup"><span data-stu-id="f45e1-117">The customer tenant's GUID</span></span>
- <span data-ttu-id="f45e1-118">A [leállás incidensének azonosítója](#outage-incident-identifier)?</span><span class="sxs-lookup"><span data-stu-id="f45e1-118">The [outage incident identifier](#outage-incident-identifier)?</span></span>
- <span data-ttu-id="f45e1-119">A CSP-n keresztül vásároltak-e érintett előfizetéseket?</span><span class="sxs-lookup"><span data-stu-id="f45e1-119">Were the impacted subscriptions purchased through CSP?</span></span> <span data-ttu-id="f45e1-120">( *Igen* vagy *nem* )</span><span class="sxs-lookup"><span data-stu-id="f45e1-120">( *yes* or *no* )</span></span>

#### <a name="outage-incident-identifier"></a><span data-ttu-id="f45e1-121">Kimaradási incidens azonosítója</span><span class="sxs-lookup"><span data-stu-id="f45e1-121">Outage incident identifier</span></span>

<span data-ttu-id="f45e1-122">A leállás incidens azonosítóját a Microsoft 365 felügyeleti központban található **Service Health** lapon találja.</span><span class="sxs-lookup"><span data-stu-id="f45e1-122">You can find the identifier for the outage incident on the **Service Health** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="f45e1-123">Az **kimaradási incidens azonosítója** az érintett szolgáltatást (például az Exchange Online-kimaradás *EX25194* ) jelző kétbetűs rövidítéssel megelőzően megadott szám.</span><span class="sxs-lookup"><span data-stu-id="f45e1-123">The **Outage Incident ID** is a number preceded by a two-letter abbreviation that indicates the affected service (for example, *EX25194* for an Exchange Online outage).</span></span> <span data-ttu-id="f45e1-124">A következő táblázat a gyakori szolgáltatások rövidítéseit ismerteti:</span><span class="sxs-lookup"><span data-stu-id="f45e1-124">The follow table describes common service abbreviations:</span></span>

| <span data-ttu-id="f45e1-125">Kétbetűs rövidítés</span><span class="sxs-lookup"><span data-stu-id="f45e1-125">Two-letter abbreviation</span></span> | <span data-ttu-id="f45e1-126">Microsoft-szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="f45e1-126">Microsoft service</span></span> |
| ----------------------- | ----------------- |
| <span data-ttu-id="f45e1-127">PÉLDÁUL</span><span class="sxs-lookup"><span data-stu-id="f45e1-127">EX</span></span> | <span data-ttu-id="f45e1-128">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="f45e1-128">Exchange Online</span></span> |
| <span data-ttu-id="f45e1-129">UTCÁN</span><span class="sxs-lookup"><span data-stu-id="f45e1-129">FO</span></span> | <span data-ttu-id="f45e1-130">Exchange Online-védelem</span><span class="sxs-lookup"><span data-stu-id="f45e1-130">Exchange Online Protection</span></span> |
| <span data-ttu-id="f45e1-131">SB</span><span class="sxs-lookup"><span data-stu-id="f45e1-131">SB</span></span> | <span data-ttu-id="f45e1-132">Skype vállalati online verzió (korábban Lync Online)</span><span class="sxs-lookup"><span data-stu-id="f45e1-132">Skype for Business Online (formerly Lync Online)</span></span> |
| <span data-ttu-id="f45e1-133">Operációs rendszer</span><span class="sxs-lookup"><span data-stu-id="f45e1-133">OS</span></span> | <span data-ttu-id="f45e1-134">Office-előfizetés</span><span class="sxs-lookup"><span data-stu-id="f45e1-134">Office Subscription</span></span> |
| <span data-ttu-id="f45e1-135">PB</span><span class="sxs-lookup"><span data-stu-id="f45e1-135">PB</span></span> | <span data-ttu-id="f45e1-136">Office 365-höz készült Power BI</span><span class="sxs-lookup"><span data-stu-id="f45e1-136">Power BI for Office 365</span></span> |
| <span data-ttu-id="f45e1-137">SP</span><span class="sxs-lookup"><span data-stu-id="f45e1-137">SP</span></span> | <span data-ttu-id="f45e1-138">SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f45e1-138">SharePoint Online</span></span> |
| <span data-ttu-id="f45e1-139">YA</span><span class="sxs-lookup"><span data-stu-id="f45e1-139">YA</span></span> | <span data-ttu-id="f45e1-140">Yammer Enterprise</span><span class="sxs-lookup"><span data-stu-id="f45e1-140">Yammer Enterprise</span></span> |
| <span data-ttu-id="f45e1-141">MO</span><span class="sxs-lookup"><span data-stu-id="f45e1-141">MO</span></span> | <span data-ttu-id="f45e1-142">Portál-hiba</span><span class="sxs-lookup"><span data-stu-id="f45e1-142">Portal error</span></span> |

### <a name="submit-sla-credit-request"></a><span data-ttu-id="f45e1-143">SLA-jóváírási kérelem beküldése</span><span class="sxs-lookup"><span data-stu-id="f45e1-143">Submit SLA credit request</span></span>

<span data-ttu-id="f45e1-144">Az SLA-jóváírási kérelem küldése a Microsoftnak a partner Center irányítópultján:</span><span class="sxs-lookup"><span data-stu-id="f45e1-144">To submit your SLA credit request to Microsoft through the Partner Center dashboard:</span></span>

1. <span data-ttu-id="f45e1-145">Jelentkezzen be a partner Center irányítópultra.</span><span class="sxs-lookup"><span data-stu-id="f45e1-145">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="f45e1-146">A bal oldali menüben válassza a **szolgáltatáskérelmek** lehetőséget, majd válassza a **partneri támogatási kérelmek** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f45e1-146">In the left-hand menu, choose **Service requests** , then select **Partner support requests** .</span></span>
3. <span data-ttu-id="f45e1-147">A **partneri kérelem** lapon válassza az **új kérelem** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f45e1-147">On the **Partner request** page, choose **New request** .</span></span>
4. <span data-ttu-id="f45e1-148">A **kérelem indítása** lapon keresse meg a **CSP-ügyfelek, megrendelések és előfizetések** szakaszt.</span><span class="sxs-lookup"><span data-stu-id="f45e1-148">On the **Start the request** page, find the section **CSP - customers, orders and subscriptions** .</span></span> <span data-ttu-id="f45e1-149">Ebben a szakaszban válassza a **probléma típusának kiválasztása** , majd az **ügyfél-szolgáltatási jóváírások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f45e1-149">In this section, choose **Select an issue type** , then select **Customer services credit requests** .</span></span>
5. <span data-ttu-id="f45e1-150">Az **ajánlott megoldások** lapon a **további segítségre van szüksége?** területen válassza az **Igen** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f45e1-150">On the **Recommended solutions** page, under **Do you need more help?** , choose **Yes** .</span></span>
6. <span data-ttu-id="f45e1-151">A **részletek** lapon töltse ki a **probléma részletei** szakaszt.</span><span class="sxs-lookup"><span data-stu-id="f45e1-151">On the **Details** page, fill out the **Issue details** section.</span></span> <span data-ttu-id="f45e1-152">A **részletek** szövegmezőben ügyeljen arra, hogy a korábban összegyűjtött [szükséges adatokat](#required-information) adja meg.</span><span class="sxs-lookup"><span data-stu-id="f45e1-152">In the **Details** text box, be sure to enter the [required information](#required-information) that you gathered earlier.</span></span>
7. <span data-ttu-id="f45e1-153">Válassza a **Submit (Küldés** ) lehetőséget az SLA-jóváírási kérelem küldéséhez.</span><span class="sxs-lookup"><span data-stu-id="f45e1-153">Choose **Submit** to send in your SLA credit request.</span></span>
