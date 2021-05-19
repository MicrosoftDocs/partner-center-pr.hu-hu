---
title: A .csv-fájl mezői több felhasználó importálása egy ügyfélfiókhoz
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ha több felhasználót szeretne hozzáadni egy ügyfélfiókhoz, hozzon létre egy vesszővel elválasztott értékfájlt (.csv) a megfelelő mezőkkel.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150981"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="fb925-103">Több felhasználó hozzáadása egy ügyfélfiókhoz egy .csv-fájl létrehozásával</span><span class="sxs-lookup"><span data-stu-id="fb925-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="fb925-104">**Megfelelő szerepkörök:** Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="fb925-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="fb925-105">Egyszerre több felhasználót is hozzáadhat egy ügyfél fiókjához úgy, hogy feltölt egy vesszővel elválasztott értékfájlformátumban (.csv) egy adatfájlt a Partnerközpont.</span><span class="sxs-lookup"><span data-stu-id="fb925-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="fb925-106">Letölthet egy mintaadatfájlt a Partnerközpont majd saját használatra szerkesztheti, vagy létrehozhat egy új adatfájlt az alább definiált adatmodellel.</span><span class="sxs-lookup"><span data-stu-id="fb925-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="fb925-107">Adatfájlokkal kapcsolatos követelmények</span><span class="sxs-lookup"><span data-stu-id="fb925-107">Data file requirements</span></span>

<span data-ttu-id="fb925-108">Ha több felhasználót szeretne hozzáadni egy ügyfél fiókjához a tömeges feltöltési folyamattal, meg kell felelnie a következő követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="fb925-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="fb925-109">Globális rendszergazdai engedélyekkel kell rendelkeznie az ügyfélfiókhoz;</span><span class="sxs-lookup"><span data-stu-id="fb925-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="fb925-110">Minden felhasználónak egyedi e-mail-címmel kell rendelkezik, amely az ügyfél e-mail-tartománya(i)hoz van hozzáfűzve;</span><span class="sxs-lookup"><span data-stu-id="fb925-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="fb925-111">Egyszerre legfeljebb 100 rekordot tölthet fel.</span><span class="sxs-lookup"><span data-stu-id="fb925-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="fb925-112">Ha több mint 100 felhasználót kell hozzáadnia, hozzon létre és töltsön fel további adatfájlokat.</span><span class="sxs-lookup"><span data-stu-id="fb925-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="fb925-113">Minden felhasználónak azonos földrajzi helyen kell **lennie.**</span><span class="sxs-lookup"><span data-stu-id="fb925-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="fb925-114">Csak az alább leírt adatokat adja meg.</span><span class="sxs-lookup"><span data-stu-id="fb925-114">Enter only the data described below.</span></span> <span data-ttu-id="fb925-115">A felesleges adatok miatt a feltöltés sikertelen lesz.</span><span class="sxs-lookup"><span data-stu-id="fb925-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="fb925-116">Adja meg a következő adatokat az adatfájlban:</span><span class="sxs-lookup"><span data-stu-id="fb925-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="fb925-117">**Oszlop neve**</span><span class="sxs-lookup"><span data-stu-id="fb925-117">**Column name**</span></span> | <span data-ttu-id="fb925-118">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="fb925-118">**Description**</span></span>  | <span data-ttu-id="fb925-119">**Korlátozás**</span><span class="sxs-lookup"><span data-stu-id="fb925-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="fb925-120">Utónév</span><span class="sxs-lookup"><span data-stu-id="fb925-120">First name</span></span>  | <span data-ttu-id="fb925-121">Felhasználó vezetékneve (nem kötelező mező)</span><span class="sxs-lookup"><span data-stu-id="fb925-121">User's first name (optional field)</span></span>  | <span data-ttu-id="fb925-122">50 karakteres korlát</span><span class="sxs-lookup"><span data-stu-id="fb925-122">50-character limit</span></span>  |
| <span data-ttu-id="fb925-123">Vezetéknév</span><span class="sxs-lookup"><span data-stu-id="fb925-123">Last name</span></span>  | <span data-ttu-id="fb925-124">Felhasználó vezetékneve (nem kötelező mező)</span><span class="sxs-lookup"><span data-stu-id="fb925-124">User's last name (optional field)</span></span>  | <span data-ttu-id="fb925-125">50 karakteres korlát</span><span class="sxs-lookup"><span data-stu-id="fb925-125">50-character limit</span></span>  |
| <span data-ttu-id="fb925-126">Megjelenített név</span><span class="sxs-lookup"><span data-stu-id="fb925-126">Display name</span></span>    | <span data-ttu-id="fb925-127">A név megjelenik a Partnerközpont (kötelező mező)</span><span class="sxs-lookup"><span data-stu-id="fb925-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="fb925-128">50 karakteres korlát</span><span class="sxs-lookup"><span data-stu-id="fb925-128">50-character limit</span></span>                         |
| <span data-ttu-id="fb925-129">E-mail</span><span class="sxs-lookup"><span data-stu-id="fb925-129">Email</span></span>   | <span data-ttu-id="fb925-130">A felhasználó vállalati e-mail-címe az ügyfél vállalatnál (kötelező mező)</span><span class="sxs-lookup"><span data-stu-id="fb925-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="fb925-131">Minden felhasználónak egyedi e-mail-címmel kell</span><span class="sxs-lookup"><span data-stu-id="fb925-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="fb925-132">Állapotfrissítés</span><span class="sxs-lookup"><span data-stu-id="fb925-132">Status update</span></span>   | <span data-ttu-id="fb925-133">Annak jelzésére használatos, hogy az új felhasználói rekord sikeresen létrejött-e</span><span class="sxs-lookup"><span data-stu-id="fb925-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="fb925-134">\*\*Hagyja üresen\*\*</span><span class="sxs-lookup"><span data-stu-id="fb925-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="fb925-135">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="fb925-135">Next steps</span></span>

- [<span data-ttu-id="fb925-136">Több felhasználó hozzáadása egy ügyfélhez</span><span class="sxs-lookup"><span data-stu-id="fb925-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)