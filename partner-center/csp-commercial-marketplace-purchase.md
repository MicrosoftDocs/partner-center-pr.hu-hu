---
title: Kereskedelmi piactéri ajánlatok vásárlása
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan vásárolhatnak SaaS-ajánlatokat független szoftverszállítóktól (ISV-ktől) a Partnerközpont piactéren a CSP-programpartnerek.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147853"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a><span data-ttu-id="aa58b-103">Kereskedelmi piactéri termékek vásárlása az ügyfelek számára Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="aa58b-103">Purchase commercial marketplace products for your customers in Partner Center</span></span>


<span data-ttu-id="aa58b-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Rendszergazdai ügynök</span><span class="sxs-lookup"><span data-stu-id="aa58b-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="aa58b-105">A Felhőszolgáltató (CSP) program egyik partnereként a kereskedelmi piactéren vásárolhat előfizetéseket az ügyfelei számára a független szoftverszállítók (ISV-k) által kínált bizonyos Szolgáltatott szoftver (SaaS) termékekhez.</span><span class="sxs-lookup"><span data-stu-id="aa58b-105">As a partner in the Cloud Solution Provider (CSP) program, you can use the commercial marketplace to purchase subscriptions for your customers to certain Software as a Service (SaaS) products offered by Independent Software Vendors (ISVs).</span></span>

<span data-ttu-id="aa58b-106">Ha ISV SaaS-előfizetéseket kínál ügyfeleinek, megkülönböztetheti vállalkozását.</span><span class="sxs-lookup"><span data-stu-id="aa58b-106">By offering ISV SaaS subscriptions to your customers, you can help differentiate your business.</span></span> <span data-ttu-id="aa58b-107">Emellett hozzáférést adhat az ügyfeleknek az adott üzleti igényeiknek megfelelő szoftvercsomaghoz.</span><span class="sxs-lookup"><span data-stu-id="aa58b-107">You can also give customers access to software bundles that address their specific business needs.</span></span> <span data-ttu-id="aa58b-108">Ezeknek a piactéri SaaS-termékeknek a licencét és előfizetését is az ISV-közzétevőktől kezelheti, ahogyan a Microsoft-termékek licencét és előfizetését.</span><span class="sxs-lookup"><span data-stu-id="aa58b-108">You manage licenses and subscriptions for these marketplace SaaS products from ISV publishers just as you manage licenses and subscriptions for Microsoft products.</span></span>

<span data-ttu-id="aa58b-109">Vásárolhat licencalapú **SaaS-előfizetéseket** vagy **használatalapú előfizetéseket.**</span><span class="sxs-lookup"><span data-stu-id="aa58b-109">You can purchase either **license-based** SaaS subscriptions or **usage-based** subscriptions.</span></span> <span data-ttu-id="aa58b-110">A licencalapú és a használatalapú számlázás közötti különbségekkel kapcsolatos további információkért lásd a [számlázás alapjait.](billing-basics.md)</span><span class="sxs-lookup"><span data-stu-id="aa58b-110">To learn more about the difference between license-based and usage-based billing, see [Billing basics](billing-basics.md).</span></span>

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a><span data-ttu-id="aa58b-111">Licencalapú és forgalmi díjas SaaS-előfizetések vásárlása a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="aa58b-111">Purchase license-based and metered SaaS subscriptions in Partner Center</span></span>

<span data-ttu-id="aa58b-112">Az ISV-közzétevők által kínált licencalapú vagy forgalmi díjas SaaS-termékek előfizetését ugyanazokkal a folyamatokkal vásárolhatja meg, mint a Microsoft-termékekhez.</span><span class="sxs-lookup"><span data-stu-id="aa58b-112">You purchase subscriptions for license-based or metered SaaS products offered by ISV publishers using the same process you use to purchase subscriptions for Microsoft products.</span></span>

<span data-ttu-id="aa58b-113">Licencalapú vagy forgalmi díjas SaaS-előfizetés Partnerközpont ügyfél-előfizetések létrehozása, felfüggesztése vagy [lemondása.](create-a-new-subscription.md#create-a-new-subscription)</span><span class="sxs-lookup"><span data-stu-id="aa58b-113">To purchase a license-based or metered SaaS subscription in Partner Center, see [Create, suspend, or cancel customer subscriptions](create-a-new-subscription.md#create-a-new-subscription).</span></span>

<span data-ttu-id="aa58b-114">A kereskedelmi [piactéri előfizetések Partnerközpont API-kat](/partner-center/develop/) is használhatja az ügyfelek számára.</span><span class="sxs-lookup"><span data-stu-id="aa58b-114">You can also use [Partner Center APIs](/partner-center/develop/) to create commercial marketplace subscriptions for your customers.</span></span> <span data-ttu-id="aa58b-115">(Az API-k használatával kapcsolatos Partnerközpont lásd: [Előfizetés létrehozása kereskedelmi piactéri termékekhez.)](/partner-center/develop/create-subscription-azure-marketplace-products)</span><span class="sxs-lookup"><span data-stu-id="aa58b-115">(For more info on using Partner Center APIs, see [Create a subscription for commercial marketplace products](/partner-center/develop/create-subscription-azure-marketplace-products).)</span></span>

>[!IMPORTANT]
> <span data-ttu-id="aa58b-116">A CSP-programban partnerként licencalapú **vagy** forgalmi díjas SaaS-előfizetéseket vásárolhat a csv-közzétevőktől a Partnerközpont. </span><span class="sxs-lookup"><span data-stu-id="aa58b-116">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="aa58b-117">Ez azt jelenti, hogy bármilyen licencalapú vagy forgalmi díjas  SaaS-ajánlatot [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) megvásárolhat, amelyet az ISV közzétevő tett elérhetővé az Ön számára, beleértve azokat az ajánlatokat is, amelyekhez Hozzáféréssel rendelkezik. </span><span class="sxs-lookup"><span data-stu-id="aa58b-117">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="aa58b-118">Az ISV-k (például Azure-alkalmazásokat, tárolókat vagy virtuális gépeket érintő használatalapú ajánlatok) kereskedelmi piactéri ajánlatának megvásárlásához vagy kezeléséhez meg kell [Azure Portal.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="aa58b-118">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a><span data-ttu-id="aa58b-119">Használatalapú előfizetések vásárlása a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="aa58b-119">Purchase usage-based subscriptions in the Azure portal</span></span>

<span data-ttu-id="aa58b-120">A külső ISV-közzétevőktől származó licencalapú SaaS-előfizetésekkel ellentétben a használatalapú előfizetések esetében az ügyfélnek először Azure-előfizetésre van szüksége.</span><span class="sxs-lookup"><span data-stu-id="aa58b-120">In contrast to license-based SaaS subscriptions from third-party ISV publishers, usage-based subscriptions first require a customer to have an Azure subscription.</span></span> <span data-ttu-id="aa58b-121">A kereskedelmi piactér számlázása, a használatalapú erőforrások az ügyfél Azure-előfizetése alá esnek.</span><span class="sxs-lookup"><span data-stu-id="aa58b-121">Billing for commercial marketplace, usage-based resources falls under the customer's Azure subscription.</span></span> <span data-ttu-id="aa58b-122">Ha az ügyfél már rendelkezik Azure-előfizetéssel, a CSP-program egyik partnere az alábbi lépéseket követve vásárolhat számukra kereskedelmi piactér-előfizetést:</span><span class="sxs-lookup"><span data-stu-id="aa58b-122">Once your customer has an Azure subscription, a partner in the CSP program can follow these steps to purchase a commercial marketplace subscription for them:</span></span>

1. <span data-ttu-id="aa58b-123">Jelentkezzen be a Partnerközpont [irányítópultra,](https://partner.microsoft.com/dashboard)majd válassza az **Ügyfelek** lehetőséget a bal oldali menüben.</span><span class="sxs-lookup"><span data-stu-id="aa58b-123">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **Customers** from the left-hand menu.</span></span>

2. <span data-ttu-id="aa58b-124">Válassza ki az adott ügyfelet, majd válassza az **Előfizetések lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="aa58b-124">Select the specific customer, then select **Subscriptions**.</span></span>  

3. <span data-ttu-id="aa58b-125">A **Használatalapú előfizetések alatt válassza a** **Minden erőforrás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="aa58b-125">Under the **Usage-based subscriptions**, select **All resources**.</span></span> <span data-ttu-id="aa58b-126">Ezzel az Azure felügyeleti portálra kerül.</span><span class="sxs-lookup"><span data-stu-id="aa58b-126">This takes you to the Azure Management portal.</span></span>

4. <span data-ttu-id="aa58b-127">Az Azure felügyeleti portál bal oldali menüjében válassza **az Erőforrás** létrehozása lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="aa58b-127">In the Azure Management portal, select **Create a resource** from the left-hand menu.</span></span>

5. <span data-ttu-id="aa58b-128">A **lista tetején** válassza az Összes Azure Marketplace lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="aa58b-128">Select **See all** at the top of the Azure Marketplace list.</span></span>

6. <span data-ttu-id="aa58b-129">A lista szűkítéshez használjon szűrőket a Marketplace-lista tetején.</span><span class="sxs-lookup"><span data-stu-id="aa58b-129">To narrow your list, use filters at the top of the Marketplace list.</span></span> <span data-ttu-id="aa58b-130">Kiválaszthatja például a **Microsoft** vagy  a **Partner** lehetőséget a Közzétevő legördülő listából, hogy csak a Microsoft vagy egy ISV-közzétevő ajánlatát tekintse meg.</span><span class="sxs-lookup"><span data-stu-id="aa58b-130">For example, you can select **Microsoft** or **Partner** from the **Publisher** dropdown list to view only offers from Microsoft or those from an ISV publisher.</span></span>

7. <span data-ttu-id="aa58b-131">Válasszon ki egy adott ajánlatot, majd válassza a **Létrehozás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="aa58b-131">Choose a specific offer, then select **Create**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="aa58b-132">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="aa58b-132">Next steps</span></span>

- [<span data-ttu-id="aa58b-133">Kereskedelmi piactéri ajánlatok kezelése</span><span class="sxs-lookup"><span data-stu-id="aa58b-133">Manage commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)