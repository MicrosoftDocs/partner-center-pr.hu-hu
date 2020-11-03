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
ms.date: 05/20/2020
ms.openlocfilehash: 1bfcb4de27233283b6188903b3e1f6bbdf67698c
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/14/2020
ms.locfileid: "92530385"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="a6760-103">Regisztráció a felügyeleti panel gyártójával, amely segít a CSP-partneri rendszerek integrálásában a partner Center API-kkal</span><span class="sxs-lookup"><span data-stu-id="a6760-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="a6760-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="a6760-104">**Applies to**</span></span>

- <span data-ttu-id="a6760-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="a6760-105">Partner Center</span></span>

<span data-ttu-id="a6760-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="a6760-106">**Appropriate roles**</span></span>

- <span data-ttu-id="a6760-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="a6760-107">Global admin</span></span>

<span data-ttu-id="a6760-108">A Vezérlőpult gyártója (CPV) egy független szoftvergyártó, amely a Cloud Solution Provider (CSP) partnerei által használt alkalmazásokat fejleszti, és lehetővé teszi, hogy a rendszereket a partner Center API-kkal integrálják.</span><span class="sxs-lookup"><span data-stu-id="a6760-108">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="a6760-109">A Vezérlőpult gyártója nem egy olyan CSP-partner, amelynek közvetlen hozzáférése van a partner Center irányítópulthoz vagy a partner Center API-khoz.</span><span class="sxs-lookup"><span data-stu-id="a6760-109">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="a6760-110">Akár egy aktuális Vezérlőpult-gyártó (CPV), akár egy új, a Microsoft-partnerekkel együttműködni kívánó CPV, a Microsoft most regisztrálnia kell a partner Centerben, hogy regisztrálja az alkalmazásait és támogassa a felhőalapú megoldások szolgáltatói partnereit.</span><span class="sxs-lookup"><span data-stu-id="a6760-110">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="a6760-111">Fiók létrehozásához a CPV-partner használhat meglévő CSP-partneri bérlőt vagy meglévő CPV-bérlőt, vagy létrehozhat egy új bérlőt a bevezetési folyamat részeként.</span><span class="sxs-lookup"><span data-stu-id="a6760-111">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="a6760-112">Ha a CPV-partner úgy dönt, hogy a meglévő CSP bérlőt használja, külön több-bérlős alkalmazásokat kell létrehoznia, és regisztrálnia kell őket a fiókpartner-tevékenységekhez.</span><span class="sxs-lookup"><span data-stu-id="a6760-112">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="a6760-113">Egy alkalmazás nem regisztrálható CSP-ként és CPV-alkalmazásként.</span><span class="sxs-lookup"><span data-stu-id="a6760-113">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="a6760-114">Miután regisztrált a partner Centerben, és regisztrálta az alkalmazásait, hozzáférhet a partner Center API-khoz.</span><span class="sxs-lookup"><span data-stu-id="a6760-114">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="a6760-115">A Microsoft felveszi Önnel a kapcsolatot a partner Center-értesítésen keresztül a sandbox adataival.</span><span class="sxs-lookup"><span data-stu-id="a6760-115">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="a6760-116">Ha már rendelkezik egy sandbox-fiókkal, folytassa a használatát.</span><span class="sxs-lookup"><span data-stu-id="a6760-116">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="a6760-117">Nem lesz szüksége új homokozóra.</span><span class="sxs-lookup"><span data-stu-id="a6760-117">You won't need a new sandbox.</span></span>

<span data-ttu-id="a6760-118">A [Microsoft Vezérlőpult gyártói szerződésének](https://go.microsoft.com/fwlink/?linkid=2055198) áttekintése</span><span class="sxs-lookup"><span data-stu-id="a6760-118">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="a6760-119">A partner Center használata</span><span class="sxs-lookup"><span data-stu-id="a6760-119">Working in Partner Center</span></span>
<span data-ttu-id="a6760-120">Miután regisztrált a partner Center-beli CPV-felületre, és elfogadta a CPV-szerződést, a következőket teheti:</span><span class="sxs-lookup"><span data-stu-id="a6760-120">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="a6760-121">Több-bérlős alkalmazások kezelése (alkalmazások hozzáadása a partner Centerben lévő alkalmazások Azure Portalához, regisztrálásához és regisztrációjának megszüntetéséhez).</span><span class="sxs-lookup"><span data-stu-id="a6760-121">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="a6760-122">A CPVs regisztrálnia kell az alkalmazásaikat a partner Centerben ahhoz, hogy engedélyt kapjon a partner Center API-k számára.</span><span class="sxs-lookup"><span data-stu-id="a6760-122">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="a6760-123">Az alkalmazások csak a Azure Portalhez való hozzáadása nem engedélyezi a CPV-alkalmazások számára a partner Center API-kat.</span><span class="sxs-lookup"><span data-stu-id="a6760-123">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="a6760-124">A CPV-Profil megtekintése és kezelése</span><span class="sxs-lookup"><span data-stu-id="a6760-124">View and manage your CPV profile</span></span> 

- <span data-ttu-id="a6760-125">Megtekintheti és kezelheti azokat a felhasználókat, akiknek hozzáférésre van szükségük a CPV-képességekhez.</span><span class="sxs-lookup"><span data-stu-id="a6760-125">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="a6760-126">A globális rendszergazda a CPV egyetlen szerepköre.</span><span class="sxs-lookup"><span data-stu-id="a6760-126">Global admin is the only role a CPV can have.</span></span>


