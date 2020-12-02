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
ms.openlocfilehash: 9f1d6e2a59bd892b7b79a1e3aa532242cdd0e302
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474189"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="8dcca-103">Felhasználók egy. csv-fájljának feltöltése egy ügyfél fiókjába</span><span class="sxs-lookup"><span data-stu-id="8dcca-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="8dcca-104">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="8dcca-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8dcca-105">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="8dcca-105">Global admin</span></span>

<span data-ttu-id="8dcca-106">Egyszerre több felhasználót is hozzáadhat egy ügyfél fiókjához, ha a vesszővel tagolt fájlformátumban (. csv) egy adatfájlt tölt fel a partner központba.</span><span class="sxs-lookup"><span data-stu-id="8dcca-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="8dcca-107">Az ügyfél-felhasználók fájljának létrehozása és az ügyfél-fiókba való feltöltés</span><span class="sxs-lookup"><span data-stu-id="8dcca-107">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="8dcca-108">Hozzon létre egy vesszővel tagolt (. csv) adatfájlt a fent ismertetett adatokkal.</span><span class="sxs-lookup"><span data-stu-id="8dcca-108">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="8dcca-109">Mentse a fájlt, hogy egy későbbi lépésben tallózással keresse meg.</span><span class="sxs-lookup"><span data-stu-id="8dcca-109">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="8dcca-110">A [. csv fájl mezőinek megtekintéséhez több felhasználó importálása egy ügyfél-fiókba](file-customer-users.md).</span><span class="sxs-lookup"><span data-stu-id="8dcca-110">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="8dcca-111">Jelentkezzen be a partner Center [irányítópultra](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="8dcca-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="8dcca-112">A partner Center menüben válassza az **ügyfelek** lehetőséget, majd válasszon egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="8dcca-112">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="8dcca-113">Válassza ki az ügyfél **felhasználóinak és licencek** lapját, majd válassza a **felhasználók feltöltése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8dcca-113">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="8dcca-114">A **felhasználói adatok feltöltése** területen válassza a **Tallózás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8dcca-114">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="8dcca-115">A fájl kiválasztása lapon válassza ki az adatfájlt, majd kattintson a **Megnyitás** gombra.</span><span class="sxs-lookup"><span data-stu-id="8dcca-115">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="8dcca-116">Válassza az **Érvényesítés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8dcca-116">Select **Validate**.</span></span>

    <span data-ttu-id="8dcca-117">**Megjegyzés**  A legtöbb fiók-létrehozási hibát az adatfájlok hibái okozzák, beleértve a hiányzó információkat, a formázott vagy duplikált e-mail-címeket, vagy túl sok rekordot a fájlban.</span><span class="sxs-lookup"><span data-stu-id="8dcca-117">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="8dcca-118">Miután a partner Center érvényesíti a fájlt, válassza ki az új felhasználók földrajzi **helyét** .</span><span class="sxs-lookup"><span data-stu-id="8dcca-118">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="8dcca-119">Válassza a **Mentés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8dcca-119">Select **Save**.</span></span>
10. <span data-ttu-id="8dcca-120">Töltse le a felhasználók ideiglenes jelszavával kapcsolatos információkat.</span><span class="sxs-lookup"><span data-stu-id="8dcca-120">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="8dcca-121">Ügyeljen arra, hogy az ideiglenes jelszavakkal töltse le a fájlt, mivel ezt később nem fogja tudni elvégezni.</span><span class="sxs-lookup"><span data-stu-id="8dcca-121">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="8dcca-122">Az új felhasználóknak az új fiókok ideiglenes jelszavával be kell jelentkezniük az új fiókba.</span><span class="sxs-lookup"><span data-stu-id="8dcca-122">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="8dcca-123">Az új felhasználók automatikusan kapnak engedélyeket a **licencek és szolgáltatások használatára** .</span><span class="sxs-lookup"><span data-stu-id="8dcca-123">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="8dcca-124">További lépések</span><span class="sxs-lookup"><span data-stu-id="8dcca-124">Next steps</span></span>

- [<span data-ttu-id="8dcca-125">A partner Centerben a saját termékeinek vagy szolgáltatásainak megvásárlására jogosult ügyfelek számára</span><span class="sxs-lookup"><span data-stu-id="8dcca-125">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
