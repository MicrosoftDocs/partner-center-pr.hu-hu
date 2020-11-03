---
title: A. csv fájl mezői több felhasználó importálásához egy ügyfél-fiókhoz
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ha több felhasználót szeretne felvenni egy ügyfél-fiókba, hozzon létre egy vesszővel tagolt (. csv) fájlt a megfelelő mezőkkel.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/03/2020
ms.locfileid: "92528095"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="1f1ec-103">Egy. csv-fájl létrehozásával több felhasználót is hozzáadhat egy felhasználói fiókhoz</span><span class="sxs-lookup"><span data-stu-id="1f1ec-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="1f1ec-104">**A következőkre vonatkozik**</span><span class="sxs-lookup"><span data-stu-id="1f1ec-104">**Applies to**</span></span>

- <span data-ttu-id="1f1ec-105">Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="1f1ec-105">Partner Center</span></span>

<span data-ttu-id="1f1ec-106">**Megfelelő szerepkörök**</span><span class="sxs-lookup"><span data-stu-id="1f1ec-106">**Appropriate roles**</span></span>

- <span data-ttu-id="1f1ec-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="1f1ec-107">Global admin</span></span>

<span data-ttu-id="1f1ec-108">Egyszerre több felhasználót is hozzáadhat egy ügyfél fiókjához, ha a vesszővel tagolt fájlformátumban (. csv) egy adatfájlt tölt fel a partner központba.</span><span class="sxs-lookup"><span data-stu-id="1f1ec-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="1f1ec-109">Letölthet egy minta adatfájlt a partner központjából, és szerkesztheti a saját használatra, vagy létrehozhat egy új adatfájlt az alább meghatározott adatmodell használatával.</span><span class="sxs-lookup"><span data-stu-id="1f1ec-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="1f1ec-110">Az adatfájlra vonatkozó követelmények</span><span class="sxs-lookup"><span data-stu-id="1f1ec-110">Data file requirements</span></span>

<span data-ttu-id="1f1ec-111">Ha több felhasználót szeretne hozzáadni egy ügyfél fiókjához a tömeges feltöltési folyamat használatával, a következő követelményeknek kell megfelelnie:</span><span class="sxs-lookup"><span data-stu-id="1f1ec-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="1f1ec-112">Globális rendszergazdai engedélyekkel kell rendelkeznie az ügyfél fiókhoz;</span><span class="sxs-lookup"><span data-stu-id="1f1ec-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="1f1ec-113">Minden felhasználónak rendelkeznie kell egy egyedi e-mail-címmel, amely az ügyfél e-mail-tartományához van hozzáfűzve;</span><span class="sxs-lookup"><span data-stu-id="1f1ec-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="1f1ec-114">Egyszerre akár 100 rekordot is feltölthet.</span><span class="sxs-lookup"><span data-stu-id="1f1ec-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="1f1ec-115">Ha több mint 100 felhasználót kell felvennie, hozzon létre és töltsön fel további adatfájlokat.</span><span class="sxs-lookup"><span data-stu-id="1f1ec-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="1f1ec-116">Minden felhasználónak ugyanabban a földrajzi **helyen** kell lennie.</span><span class="sxs-lookup"><span data-stu-id="1f1ec-116">All users must be in the same geographic **Location** .</span></span>
- <span data-ttu-id="1f1ec-117">Csak az alábbiakban ismertetett adattípusokat adja meg.</span><span class="sxs-lookup"><span data-stu-id="1f1ec-117">Enter only the data described below.</span></span> <span data-ttu-id="1f1ec-118">A külső adatok miatt a feltöltés sikertelen lesz.</span><span class="sxs-lookup"><span data-stu-id="1f1ec-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="1f1ec-119">Adja meg az adatfájl következő értékeit:</span><span class="sxs-lookup"><span data-stu-id="1f1ec-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="1f1ec-120">**Oszlop neve**</span><span class="sxs-lookup"><span data-stu-id="1f1ec-120">**Column name**</span></span> | <span data-ttu-id="1f1ec-121">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="1f1ec-121">**Description**</span></span>  | <span data-ttu-id="1f1ec-122">**Korlátozás**</span><span class="sxs-lookup"><span data-stu-id="1f1ec-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="1f1ec-123">Utónév</span><span class="sxs-lookup"><span data-stu-id="1f1ec-123">First name</span></span>  | <span data-ttu-id="1f1ec-124">Felhasználó vezetékneve (nem kötelező mező)</span><span class="sxs-lookup"><span data-stu-id="1f1ec-124">User's first name (optional field)</span></span>  | <span data-ttu-id="1f1ec-125">50 – karakteres korlát</span><span class="sxs-lookup"><span data-stu-id="1f1ec-125">50-character limit</span></span>  |
| <span data-ttu-id="1f1ec-126">Vezetéknév</span><span class="sxs-lookup"><span data-stu-id="1f1ec-126">Last name</span></span>  | <span data-ttu-id="1f1ec-127">Felhasználó vezetékneve (nem kötelező mező)</span><span class="sxs-lookup"><span data-stu-id="1f1ec-127">User's last name (optional field)</span></span>  | <span data-ttu-id="1f1ec-128">50 – karakteres korlát</span><span class="sxs-lookup"><span data-stu-id="1f1ec-128">50-character limit</span></span>  |
| <span data-ttu-id="1f1ec-129">Megjelenített név</span><span class="sxs-lookup"><span data-stu-id="1f1ec-129">Display name</span></span>    | <span data-ttu-id="1f1ec-130">A partner Centerben megjelenő név (kötelező mező)</span><span class="sxs-lookup"><span data-stu-id="1f1ec-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="1f1ec-131">50 – karakteres korlát</span><span class="sxs-lookup"><span data-stu-id="1f1ec-131">50-character limit</span></span>                         |
| <span data-ttu-id="1f1ec-132">E-mail</span><span class="sxs-lookup"><span data-stu-id="1f1ec-132">Email</span></span>   | <span data-ttu-id="1f1ec-133">Felhasználó üzleti e-mail-címe az ügyfél cégnél (kötelező mező)</span><span class="sxs-lookup"><span data-stu-id="1f1ec-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="1f1ec-134">Minden felhasználónak egyedi e-mail-címmel kell rendelkeznie</span><span class="sxs-lookup"><span data-stu-id="1f1ec-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="1f1ec-135">Állapot frissítése</span><span class="sxs-lookup"><span data-stu-id="1f1ec-135">Status update</span></span>   | <span data-ttu-id="1f1ec-136">Annak jelzésére szolgál, hogy az új felhasználói rekord létrehozása sikerült-e</span><span class="sxs-lookup"><span data-stu-id="1f1ec-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="1f1ec-137">\*\*Hagyja üresen\*\*</span><span class="sxs-lookup"><span data-stu-id="1f1ec-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="1f1ec-138">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="1f1ec-138">Next steps</span></span>

- [<span data-ttu-id="1f1ec-139">Több felhasználó hozzáadása egy ügyfélhez</span><span class="sxs-lookup"><span data-stu-id="1f1ec-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)