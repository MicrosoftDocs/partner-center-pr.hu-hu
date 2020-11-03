---
title: Több felhasználó hozzáadása egy ügyfél-fiókhoz
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ha több felhasználót szeretne felvenni egy ügyfél fiókjába, töltse fel az adatfájlt a partner központba a vesszővel tagolt (. csv) fájlformátum használatával.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0a9b2ed89b10e43c31d00777054839f3208e5c16
ms.sourcegitcommit: 32516c30e90ee78415e5537d2b8ccf467f56a82d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/03/2020
ms.locfileid: "92528107"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="e25cd-103">Felhasználók egy. csv-fájljának feltöltése egy ügyfél fiókjába</span><span class="sxs-lookup"><span data-stu-id="e25cd-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="e25cd-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="e25cd-104">**Applies to**</span></span>

- <span data-ttu-id="e25cd-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="e25cd-105">Partner Center</span></span>

<span data-ttu-id="e25cd-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="e25cd-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e25cd-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="e25cd-107">Global admin</span></span>

<span data-ttu-id="e25cd-108">Egyszerre több felhasználót is hozzáadhat egy ügyfél fiókjához, ha a vesszővel tagolt fájlformátumban (. csv) egy adatfájlt tölt fel a partner központba.</span><span class="sxs-lookup"><span data-stu-id="e25cd-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="e25cd-109">Az ügyfél-felhasználók fájljának létrehozása és az ügyfél-fiókba való feltöltés</span><span class="sxs-lookup"><span data-stu-id="e25cd-109">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="e25cd-110">Hozzon létre egy vesszővel tagolt (. csv) adatfájlt a fent ismertetett adatokkal.</span><span class="sxs-lookup"><span data-stu-id="e25cd-110">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="e25cd-111">Mentse a fájlt, hogy egy későbbi lépésben tallózással keresse meg.</span><span class="sxs-lookup"><span data-stu-id="e25cd-111">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="e25cd-112">A [. csv fájl mezőinek megtekintéséhez több felhasználó importálása egy ügyfél-fiókba](file-customer-users.md).</span><span class="sxs-lookup"><span data-stu-id="e25cd-112">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="e25cd-113">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="e25cd-113">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="e25cd-114">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="e25cd-114">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

4. <span data-ttu-id="e25cd-115">Válassza ki az ügyfél **felhasználóinak és licencek** lapját, majd válassza a **felhasználók feltöltése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e25cd-115">Select the customer's **Users and Licenses** tab, then select **Upload users** .</span></span>

5. <span data-ttu-id="e25cd-116">A **felhasználói adatok feltöltése** területen válassza a **Tallózás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e25cd-116">Under **Upload user info** , select **Browse** .</span></span>

6. <span data-ttu-id="e25cd-117">A fájl kiválasztása lapon válassza ki az adatfájlt, majd kattintson a **Megnyitás** gombra.</span><span class="sxs-lookup"><span data-stu-id="e25cd-117">In the file selector, select your data file and then select **Open** .</span></span>

7. <span data-ttu-id="e25cd-118">Válassza az **Érvényesítés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e25cd-118">Select **Validate** .</span></span>

    <span data-ttu-id="e25cd-119">**Megjegyzés**    A legtöbb fiók-létrehozási hibát az adatfájlok hibái okozzák, beleértve a hiányzó információkat, a formázott vagy duplikált e-mail-címeket, vagy túl sok rekordot a fájlban.</span><span class="sxs-lookup"><span data-stu-id="e25cd-119">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="e25cd-120">Miután a partner Center érvényesíti a fájlt, válassza ki az új felhasználók földrajzi **helyét** .</span><span class="sxs-lookup"><span data-stu-id="e25cd-120">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="e25cd-121">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="e25cd-121">Select **Save** .</span></span>
10. <span data-ttu-id="e25cd-122">Töltse le a felhasználók ideiglenes jelszavával kapcsolatos információkat.</span><span class="sxs-lookup"><span data-stu-id="e25cd-122">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="e25cd-123">Ügyeljen arra, hogy az ideiglenes jelszavakkal töltse le a fájlt, mivel ezt később nem fogja tudni elvégezni.</span><span class="sxs-lookup"><span data-stu-id="e25cd-123">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="e25cd-124">Az új felhasználóknak az új fiókok ideiglenes jelszavával be kell jelentkezniük az új fiókba.</span><span class="sxs-lookup"><span data-stu-id="e25cd-124">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="e25cd-125">Az új felhasználók automatikusan kapnak engedélyeket a **licencek és szolgáltatások használatára** .</span><span class="sxs-lookup"><span data-stu-id="e25cd-125">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="e25cd-126">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="e25cd-126">Next steps</span></span>

- [<span data-ttu-id="e25cd-127">A partner Centerben a saját termékeinek vagy szolgáltatásainak megvásárlására jogosult ügyfelek számára</span><span class="sxs-lookup"><span data-stu-id="e25cd-127">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
