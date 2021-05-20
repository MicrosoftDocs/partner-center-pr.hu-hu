---
title: Több felhasználó hozzáadása egy ügyfélfiókhoz
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ha több felhasználót szeretne hozzáadni egy ügyfél fiókjához, töltsön fel egy adatfájlt a Partnerközpont vesszővel elválasztott (.csv) fájlformátumban.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150471"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="ed6fc-103">Felhasználók .csv-fájl feltöltése egy ügyfél fiókjába</span><span class="sxs-lookup"><span data-stu-id="ed6fc-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="ed6fc-104">**Megfelelő szerepkörök:** Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="ed6fc-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="ed6fc-105">Egyszerre több felhasználót is hozzáadhat egy ügyfél fiókjához, ha feltölt egy vesszővel elválasztott értékfájlformátumban (.csv) egy adatfájlt a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="ed6fc-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="ed6fc-106">Hozza létre az ügyfélfelhasználók fájlját, és töltse fel az ügyfélfiókba</span><span class="sxs-lookup"><span data-stu-id="ed6fc-106">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="ed6fc-107">Hozzon létre egy vesszővel elválasztott adatfájlt (.csv) a fent leírt adatokkal.</span><span class="sxs-lookup"><span data-stu-id="ed6fc-107">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="ed6fc-108">Mentse a fájlt, hogy egy későbbi lépésben tallózni tudja.</span><span class="sxs-lookup"><span data-stu-id="ed6fc-108">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="ed6fc-109">A [.csv-fájl mezőiben több felhasználót importálhat egy ügyfélfiókhoz.](file-customer-users.md)</span><span class="sxs-lookup"><span data-stu-id="ed6fc-109">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="ed6fc-110">Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="ed6fc-110">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="ed6fc-111">A Partnerközpont válassza az **Ügyfelek** lehetőséget, majd válasszon ki egy ügyfelet a listából.</span><span class="sxs-lookup"><span data-stu-id="ed6fc-111">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="ed6fc-112">Válassza az ügyfél Felhasználók és licencek **lapját,** majd válassza a **Felhasználók feltöltése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ed6fc-112">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="ed6fc-113">A **Felhasználói adatok feltöltése alatt válassza** a Tallózás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ed6fc-113">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="ed6fc-114">A fájlválasztóban válassza ki az adatfájlt, majd válassza a **Megnyitás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ed6fc-114">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="ed6fc-115">Válassza az **Érvényesítés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ed6fc-115">Select **Validate**.</span></span>

    <span data-ttu-id="ed6fc-116">**Megjegyzés**  A fiók létrehozásával kapcsolatos legtöbb hibát adatfájlhibák okják, beleértve a hiányzó információkat, a helytelenül formázott vagy duplikált e-mail-címeket, vagy a fájl túl sok rekordját.</span><span class="sxs-lookup"><span data-stu-id="ed6fc-116">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="ed6fc-117">Miután a Partnerközpont érvényesíti a fájlt, válassza ki az új felhasználók **földrajzi** helyét.</span><span class="sxs-lookup"><span data-stu-id="ed6fc-117">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="ed6fc-118">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="ed6fc-118">Select **Save**.</span></span>
10. <span data-ttu-id="ed6fc-119">Töltse le a felhasználók ideiglenes jelszóinformációját.</span><span class="sxs-lookup"><span data-stu-id="ed6fc-119">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="ed6fc-120">Ne aggódjon, most töltse le az ideiglenes jelszavakkal együtt a fájlt, mert később ezt nem fogja tudni megtenni.</span><span class="sxs-lookup"><span data-stu-id="ed6fc-120">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="ed6fc-121">Az új felhasználóknak az új fiókjuk ideiglenes jelszavával kell bejelentkezniük az új fiókjukba.</span><span class="sxs-lookup"><span data-stu-id="ed6fc-121">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="ed6fc-122">Az új felhasználókhoz automatikusan hozzárendelt engedélyek: **Használhat licenceket és szolgáltatásokat.**</span><span class="sxs-lookup"><span data-stu-id="ed6fc-122">New users are automatically assigned permissions of **Can use licenses and services**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="ed6fc-123">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="ed6fc-123">Next steps</span></span>

- [<span data-ttu-id="ed6fc-124">Engedélyt adhat az ügyfeleknek a Partnerközpont saját termékeik vagy szolgáltatásaik vásárlására</span><span class="sxs-lookup"><span data-stu-id="ed6fc-124">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
