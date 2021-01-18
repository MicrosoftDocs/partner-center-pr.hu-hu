---
title: Regisztráció Vezérlőpult-gyártóként
description: Ismerje meg, hogyan regisztrálhat a felügyeleti panel Gyártójába (CPV) a partner Centerben, hogy jobban integrálja a CSP-partneri rendszereket a partner Center API-kkal.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: 5fd2267d53641fe4a0b6181217a35f0470e5bbe5
ms.sourcegitcommit: 7681c6fc51e78cba106c46a52f6bb27e1a5c1c6b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "98560510"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="174e0-103">Regisztráció a felügyeleti panel gyártójával, amely segít a CSP-partneri rendszerek integrálásában a partner Center API-kkal</span><span class="sxs-lookup"><span data-stu-id="174e0-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="174e0-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="174e0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="174e0-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="174e0-105">Global admin</span></span>

<span data-ttu-id="174e0-106">A Vezérlőpult gyártója (CPV) egy független szoftvergyártó, amely a Cloud Solution Provider (CSP) partnerei által használt alkalmazásokat fejleszti, és lehetővé teszi, hogy a rendszereket a partner Center API-kkal integrálják.</span><span class="sxs-lookup"><span data-stu-id="174e0-106">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="174e0-107">A Vezérlőpult gyártója nem egy olyan CSP-partner, amelynek közvetlen hozzáférése van a partner Center irányítópulthoz vagy a partner Center API-khoz.</span><span class="sxs-lookup"><span data-stu-id="174e0-107">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="174e0-108">Akár egy aktuális Vezérlőpult-gyártó (CPV), akár egy új, a Microsoft-partnerekkel együttműködni kívánó CPV, a Microsoft most regisztrálnia kell a partner Centerben, hogy regisztrálja az alkalmazásait és támogassa a felhőalapú megoldások szolgáltatói partnereit.</span><span class="sxs-lookup"><span data-stu-id="174e0-108">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="174e0-109">Fiók létrehozásához a CPV-partner használhat meglévő CSP-partneri bérlőt vagy meglévő CPV-bérlőt, vagy létrehozhat egy új bérlőt a bevezetési folyamat részeként.</span><span class="sxs-lookup"><span data-stu-id="174e0-109">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="174e0-110">Ha a CPV-partner úgy dönt, hogy a meglévő CSP bérlőt használja, külön több-bérlős alkalmazásokat kell létrehoznia, és regisztrálnia kell őket a fiókpartner-tevékenységekhez.</span><span class="sxs-lookup"><span data-stu-id="174e0-110">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="174e0-111">Egy alkalmazás nem regisztrálható CSP-ként és CPV-alkalmazásként.</span><span class="sxs-lookup"><span data-stu-id="174e0-111">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="174e0-112">Miután regisztrált a partner Centerben, és regisztrálta az alkalmazásait, hozzáférhet a partner Center API-khoz.</span><span class="sxs-lookup"><span data-stu-id="174e0-112">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="174e0-113">Ha sandbox-fiókra van szüksége, vegye fel a kapcsolatot a Microsofttal Microsoft ügyfélszolgálata kéréssel.</span><span class="sxs-lookup"><span data-stu-id="174e0-113">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="174e0-114">Ha már rendelkezik egy sandbox-fiókkal, folytassa a használatát.</span><span class="sxs-lookup"><span data-stu-id="174e0-114">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="174e0-115">Nem lesz szüksége új homokozóra</span><span class="sxs-lookup"><span data-stu-id="174e0-115">You won't need a new sandbox</span></span>

<span data-ttu-id="174e0-116">A [Microsoft Vezérlőpult gyártói szerződésének](https://go.microsoft.com/fwlink/?linkid=2055198) áttekintése</span><span class="sxs-lookup"><span data-stu-id="174e0-116">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="174e0-117">A partner Center használata</span><span class="sxs-lookup"><span data-stu-id="174e0-117">Working in Partner Center</span></span>

<span data-ttu-id="174e0-118">Miután regisztrált a partner Center-beli CPV-felületre, és elfogadta a CPV-szerződést, a következőket teheti:</span><span class="sxs-lookup"><span data-stu-id="174e0-118">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="174e0-119">Több-bérlős alkalmazások kezelése (alkalmazások hozzáadása a partner Centerben lévő alkalmazások Azure Portalához, regisztrálásához és regisztrációjának megszüntetéséhez).</span><span class="sxs-lookup"><span data-stu-id="174e0-119">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="174e0-120">A CPVs regisztrálnia kell az alkalmazásaikat a partner Centerben ahhoz, hogy engedélyt kapjon a partner Center API-k számára.</span><span class="sxs-lookup"><span data-stu-id="174e0-120">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="174e0-121">Az alkalmazások csak a Azure Portalhez való hozzáadása nem engedélyezi a CPV-alkalmazások számára a partner Center API-kat.</span><span class="sxs-lookup"><span data-stu-id="174e0-121">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="174e0-122">A CPV-Profil megtekintése és kezelése</span><span class="sxs-lookup"><span data-stu-id="174e0-122">View and manage your CPV profile</span></span> 

- <span data-ttu-id="174e0-123">Megtekintheti és kezelheti azokat a felhasználókat, akiknek hozzáférésre van szükségük a CPV-képességekhez.</span><span class="sxs-lookup"><span data-stu-id="174e0-123">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="174e0-124">A globális rendszergazda a CPV egyetlen szerepköre.</span><span class="sxs-lookup"><span data-stu-id="174e0-124">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="174e0-125">További lépések</span><span class="sxs-lookup"><span data-stu-id="174e0-125">Next steps</span></span>

<span data-ttu-id="174e0-126">-[További bérlők hozzáadása a partner Center-fiókhoz](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="174e0-126">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>