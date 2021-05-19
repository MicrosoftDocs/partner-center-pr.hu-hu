---
title: Regisztráció Vezérlőpult szállítóként
description: Megtudhatja, hogyan regisztrálhat Vezérlőpult (CPV) a Partnerközpont, hogy jobban integrálni tudja a CSP-partnerrendszereket az Partnerközpont API-jával.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147139"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="99f60-103">Regisztrálás egy Vezérlőpult szállítóként a CSP-partnerrendszerek és az Partnerközpont API-k integrálásához</span><span class="sxs-lookup"><span data-stu-id="99f60-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="99f60-104">**Megfelelő szerepkörök:** Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="99f60-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="99f60-105">A Vezérlőpult Vendor (CPV) egy független szoftverszállító, amely alkalmazásokat fejleszt az Felhőszolgáltató- (CSP-) partnerek számára, hogy lehetővé tegye számukra a rendszereik integrálását Partnerközpont API-okkal.</span><span class="sxs-lookup"><span data-stu-id="99f60-105">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="99f60-106">A Vezérlőpult szállító nem CSP-partner, aki közvetlen hozzáféréssel rendelkezik a Partnerközpont irányítópultjához vagy Partnerközpont API-khoz.</span><span class="sxs-lookup"><span data-stu-id="99f60-106">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="99f60-107">Függetlenül attól, hogy Ön aktuális Vezérlőpult-szállító (CPV) vagy egy új CPV, aki Microsoft-partnerekkel szeretne dolgozni, a Microsoft megköveteli, hogy regisztráljon az Partnerközpont-ban az alkalmazások regisztrálásához és a Felhőszolgáltató támogatásához.</span><span class="sxs-lookup"><span data-stu-id="99f60-107">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="99f60-108">A fiókok létrehozásához a CPV-partnerek használhatnak egy meglévő CSP-partnerbérlőt vagy meglévő CPV-bérlőt, vagy létrehozhatnak egy új bérlőt az előfizetési folyamat részeként.</span><span class="sxs-lookup"><span data-stu-id="99f60-108">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="99f60-109">Ha a CPV-partner úgy dönt, hogy a meglévő CSP-bérlőt használja, akkor különálló több-bérlős alkalmazásokat kell létrehoznia, és regisztrálnia Partnerközpont CPV-tevékenységekhez.</span><span class="sxs-lookup"><span data-stu-id="99f60-109">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="99f60-110">Egy alkalmazás nem regisztrálható CSP- és CPV-alkalmazásként.</span><span class="sxs-lookup"><span data-stu-id="99f60-110">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="99f60-111">Miután regisztrált a Partnerközpont és regisztrálta az alkalmazásokat, hozzáférhet a Partnerközpont API-khoz.</span><span class="sxs-lookup"><span data-stu-id="99f60-111">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="99f60-112">Ha egy sandbox-fiókra van szüksége Microsoft ügyfélszolgálata forduljon a Microsofthoz egy Microsoft ügyfélszolgálata kérésen keresztül.</span><span class="sxs-lookup"><span data-stu-id="99f60-112">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="99f60-113">Ha már rendelkezik egy sandbox-fiókkal, folytassa a használatot.</span><span class="sxs-lookup"><span data-stu-id="99f60-113">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="99f60-114">Nem lesz szüksége új védőfalra</span><span class="sxs-lookup"><span data-stu-id="99f60-114">You won't need a new sandbox</span></span>

<span data-ttu-id="99f60-115">A [Microsoft Vezérlőpult szállítói szerződésének áttekintése](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="99f60-115">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="99f60-116">Munka a Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="99f60-116">Working in Partner Center</span></span>

<span data-ttu-id="99f60-117">Miután regisztrált a cpv Partnerközpont be, és elfogadta a CPV-szerződést, a következőt használhatja:</span><span class="sxs-lookup"><span data-stu-id="99f60-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="99f60-118">Több-bérlős alkalmazások kezelése (alkalmazások hozzáadása a Azure Portal alkalmazások regisztrálása és regisztrációjának Partnerközpont).</span><span class="sxs-lookup"><span data-stu-id="99f60-118">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="99f60-119">A CPV-knek regisztrálniuk kell az Partnerközpont, hogy engedélyt kapnak Partnerközpont API-kra.</span><span class="sxs-lookup"><span data-stu-id="99f60-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="99f60-120">Az alkalmazásoknak a Azure Portal való hozzáadása önmagában nem engedélyezi a CPV-alkalmazásokat Partnerközpont API-k számára.</span><span class="sxs-lookup"><span data-stu-id="99f60-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="99f60-121">CPV-profil megtekintése és kezelése</span><span class="sxs-lookup"><span data-stu-id="99f60-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="99f60-122">Megtekintheti és kezelheti a CPV-képességekhez hozzáféréssel bíró felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="99f60-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="99f60-123">A globális rendszergazda az egyetlen szerepkör, amely egy CPV-vel lehet.</span><span class="sxs-lookup"><span data-stu-id="99f60-123">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="99f60-124">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="99f60-124">Next steps</span></span>

<span data-ttu-id="99f60-125">-[További bérlők hozzáadása a Partnerközpont fiókjához](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="99f60-125">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>