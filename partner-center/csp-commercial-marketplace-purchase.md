---
title: Kereskedelmi Piactéri ajánlatok vásárlása
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy a CSP-program partnerei hogyan használhatják a partner Center Marketplace-t a független szoftvergyártók (ISV-ket) által kínált SaaS-ajánlatok vásárlásához.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 841308d535d4071ee0a8eabf3e70325edea5777c
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979716"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a><span data-ttu-id="50914-103">Kereskedelmi piactéren vásárolt termékek vásárlása a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="50914-103">Purchase commercial marketplace products for your customers in Partner Center</span></span>


<span data-ttu-id="50914-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="50914-104">**Appropriate roles**</span></span>

- <span data-ttu-id="50914-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="50914-105">Global admin</span></span>
- <span data-ttu-id="50914-106">Felügyeleti ügynök</span><span class="sxs-lookup"><span data-stu-id="50914-106">Admin agent</span></span>

<span data-ttu-id="50914-107">A Cloud Solution Provider (CSP) programban partnerként a kereskedelmi piactéren vásárolhat előfizetéseket ügyfelei számára a független szoftvergyártók (ISV-EK) által kínált, szolgáltatásként nyújtott szoftverként (SaaS).</span><span class="sxs-lookup"><span data-stu-id="50914-107">As a partner in the Cloud Solution Provider (CSP) program, you can use the commercial marketplace to purchase subscriptions for your customers to certain Software as a Service (SaaS) products offered by Independent Software Vendors (ISVs).</span></span>

<span data-ttu-id="50914-108">Az ISV SaaS-előfizetések ügyfelei számára történő biztosításával megkönnyítheti a vállalatok megkülönböztetését.</span><span class="sxs-lookup"><span data-stu-id="50914-108">By offering ISV SaaS subscriptions to your customers, you can help differentiate your business.</span></span> <span data-ttu-id="50914-109">Az ügyfelek számára hozzáférést biztosíthat az adott üzleti igényeknek megfelelő szoftver-kötegekhez is.</span><span class="sxs-lookup"><span data-stu-id="50914-109">You can also give customers access to software bundles that address their specific business needs.</span></span> <span data-ttu-id="50914-110">A piactéren elérhető SaaS-termékek licenceit és előfizetéseit a Microsoft-termékekhez tartozó licencek és előfizetések kezelése során kezelheti.</span><span class="sxs-lookup"><span data-stu-id="50914-110">You manage licenses and subscriptions for these marketplace SaaS products from ISV publishers just as you manage licenses and subscriptions for Microsoft products.</span></span>

<span data-ttu-id="50914-111">Vásárolhat **licenc-alapú** SaaS-előfizetéseket vagy **használati alapú** előfizetéseket.</span><span class="sxs-lookup"><span data-stu-id="50914-111">You can purchase either **license-based** SaaS subscriptions or **usage-based** subscriptions.</span></span> <span data-ttu-id="50914-112">Ha többet szeretne megtudni a licenc-alapú és a használati alapú számlázás közötti különbségekről, tekintse meg a [számlázás alapjai](billing-basics.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="50914-112">To learn more about the difference between license-based and usage-based billing, see [Billing basics](billing-basics.md).</span></span>

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a><span data-ttu-id="50914-113">Licenc-alapú és mért SaaS-Előfizetések vásárlása a partner Centerben</span><span class="sxs-lookup"><span data-stu-id="50914-113">Purchase license-based and metered SaaS subscriptions in Partner Center</span></span>

<span data-ttu-id="50914-114">Az ISV-gyártók által kínált licenc-alapú vagy mért SaaS-termékek előfizetéseit a Microsoft-termékek előfizetésének megvásárlására használt eljárással vásárolhatja meg.</span><span class="sxs-lookup"><span data-stu-id="50914-114">You purchase subscriptions for license-based or metered SaaS products offered by ISV publishers using the same process you use to purchase subscriptions for Microsoft products.</span></span>

<span data-ttu-id="50914-115">Ha licenc-alapú vagy mért SaaS-előfizetést szeretne vásárolni a partner Centerben, tekintse meg az [ügyfél-előfizetések létrehozása, felfüggesztése vagy megszakítása](create-a-new-subscription.md#create-a-new-subscription)című témakört.</span><span class="sxs-lookup"><span data-stu-id="50914-115">To purchase a license-based or metered SaaS subscription in Partner Center, see [Create, suspend, or cancel customer subscriptions](create-a-new-subscription.md#create-a-new-subscription).</span></span>

<span data-ttu-id="50914-116">A [partner Center API](/partner-center/develop/) -k használatával kereskedelmi piactér-előfizetéseket hozhat létre ügyfelei számára.</span><span class="sxs-lookup"><span data-stu-id="50914-116">You can also use [Partner Center APIs](/partner-center/develop/) to create commercial marketplace subscriptions for your customers.</span></span> <span data-ttu-id="50914-117">(A partner Center API-k használatával kapcsolatos további információkért lásd: [előfizetés létrehozása kereskedelmi Piactéri termékekhez](/partner-center/develop/create-subscription-azure-marketplace-products).)</span><span class="sxs-lookup"><span data-stu-id="50914-117">(For more info on using Partner Center APIs, see [Create a subscription for commercial marketplace products](/partner-center/develop/create-subscription-azure-marketplace-products).)</span></span>

>[!IMPORTANT]
> <span data-ttu-id="50914-118">A CSP programban partnerként vásárolhat **licenc-alapú** vagy **mért** SaaS-előfizetéseket a partner centeren belüli ISV-közzétevők közül.</span><span class="sxs-lookup"><span data-stu-id="50914-118">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="50914-119">Ez azt jelenti, hogy vásárolhat bármilyen **licenccel** vagy **mért** SaaS-ajánlatot, amelyet az ISV közzétevő elérhetővé tett, beleértve az [exkluzív ajánlatokat](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) is, amelyekhez hozzáféréssel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="50914-119">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="50914-120">Ha más, kereskedelmi Piactéri ajánlatokat szeretne megvásárolni vagy kezelni (például Azure-alkalmazásokat,-tárolókat vagy virtuális gépeket érintő használaton alapuló ajánlatokat), akkor a [Azure Portalra](https://portal.azure.com/)kell lépnie.</span><span class="sxs-lookup"><span data-stu-id="50914-120">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a><span data-ttu-id="50914-121">Használati alapú Előfizetések vásárlása a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="50914-121">Purchase usage-based subscriptions in the Azure portal</span></span>

<span data-ttu-id="50914-122">A külső gyártótól származó ISV-közzétevők licenc-alapú SaaS-előfizetésével ellentétben a használati előfizetésekhez először az ügyfélnek Azure-előfizetésre van szüksége.</span><span class="sxs-lookup"><span data-stu-id="50914-122">In contrast to license-based SaaS subscriptions from third-party ISV publishers, usage-based subscriptions first require a customer to have an Azure subscription.</span></span> <span data-ttu-id="50914-123">A kereskedelmi piactéren a használaton alapuló erőforrások számlázása az ügyfél Azure-előfizetése alá tartozik.</span><span class="sxs-lookup"><span data-stu-id="50914-123">Billing for commercial marketplace, usage-based resources falls under the customer's Azure subscription.</span></span> <span data-ttu-id="50914-124">Ha az ügyfél Azure-előfizetéssel rendelkezik, a CSP programban található partner a következő lépésekkel vásárolhatja meg a kereskedelmi piactér-előfizetéseket:</span><span class="sxs-lookup"><span data-stu-id="50914-124">Once your customer has an Azure subscription, a partner in the CSP program can follow these steps to purchase a commercial marketplace subscription for them:</span></span>

1. <span data-ttu-id="50914-125">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard), majd válassza az **ügyfelek** lehetőséget a bal oldali menüben.</span><span class="sxs-lookup"><span data-stu-id="50914-125">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **Customers** from the left-hand menu.</span></span>

2. <span data-ttu-id="50914-126">Válassza ki az adott ügyfelet, majd válassza az **előfizetések** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="50914-126">Select the specific customer, then select **Subscriptions**.</span></span>  

3. <span data-ttu-id="50914-127">A **használat alapú előfizetések** területen válassza az **összes erőforrás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="50914-127">Under the **Usage-based subscriptions**, select **All resources**.</span></span> <span data-ttu-id="50914-128">Ezzel az Azure felügyeleti portálra kerül.</span><span class="sxs-lookup"><span data-stu-id="50914-128">This takes you to the Azure Management portal.</span></span>

4. <span data-ttu-id="50914-129">Az Azure felügyeleti portálján válassza az **erőforrás létrehozása** lehetőséget a bal oldali menüben.</span><span class="sxs-lookup"><span data-stu-id="50914-129">In the Azure Management portal, select **Create a resource** from the left-hand menu.</span></span>

5. <span data-ttu-id="50914-130">Az Azure Marketplace-lista tetején kattintson az **összes** megjelenítése lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="50914-130">Select **See all** at the top of the Azure Marketplace list.</span></span>

6. <span data-ttu-id="50914-131">A lista szűkítéséhez használjon szűrőket a piactér lista tetején.</span><span class="sxs-lookup"><span data-stu-id="50914-131">To narrow your list, use filters at the top of the Marketplace list.</span></span> <span data-ttu-id="50914-132">Kiválaszthatja például a **Microsoft** vagy a **partner** elemet a **közzétevő** legördülő listából, hogy csak a Microsoft vagy az ISV közzétevő által készített ajánlatokat tekintse meg.</span><span class="sxs-lookup"><span data-stu-id="50914-132">For example, you can select **Microsoft** or **Partner** from the **Publisher** dropdown list to view only offers from Microsoft or those from an ISV publisher.</span></span>

7. <span data-ttu-id="50914-133">Válasszon egy adott ajánlatot, majd válassza a **Létrehozás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="50914-133">Choose a specific offer, then select **Create**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="50914-134">További lépések</span><span class="sxs-lookup"><span data-stu-id="50914-134">Next steps</span></span>

- [<span data-ttu-id="50914-135">Kereskedelmi Piactéri ajánlatok kezelése</span><span class="sxs-lookup"><span data-stu-id="50914-135">Manage commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)