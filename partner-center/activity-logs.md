---
title: Elemzések az ügyfél tevékenységnaplóiból
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogyan lehet megtekinteni és exportálni a tevékenységnaplókat, hogy betekintést nyerjen az ügyfélfiók tranzakcióiba és az ügyfelekhez kapcsolódó egyéb partnerkezelési tevékenységekbe.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1bb98dd71c9e46914b90d5efbfe14404d08275f9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150590"
---
# <a name="view-or-export-customer-activity-logs-for-more-insight-into-customer-transactions"></a><span data-ttu-id="40da6-103">Ügyféltevékenység-naplók megtekintése vagy exportálása az ügyféltranzakciókra vonatkozó további információkért</span><span class="sxs-lookup"><span data-stu-id="40da6-103">View or export customer activity logs for more insight into customer transactions</span></span>

<span data-ttu-id="40da6-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Számlázási rendszergazdai | Felhasználókezelési rendszergazdai | Rendszergazdai ügynök | Értékesítési ügynök | Helpdesk agent</span><span class="sxs-lookup"><span data-stu-id="40da6-104">**Appropriate roles**: Global admin | Billing admin | User management admin | Admin agent | Sales agent | Helpdesk agent</span></span>

<span data-ttu-id="40da6-105">A tevékenységnaplók információkat nyújtanak az ügyfelek tranzakcióiról és partnerkezelési műveleteiről.</span><span class="sxs-lookup"><span data-stu-id="40da6-105">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="40da6-106">A tranzakciók naplói részletes információkat nyújtanak a tranzakcióról, beleértve a megvásárolt előfizetéseket is.</span><span class="sxs-lookup"><span data-stu-id="40da6-106">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="40da6-107">A tevékenységnaplókat Excel-kompatibilis, vesszővel elválasztott fájlformátumba (.csv) is exportálhatja.</span><span class="sxs-lookup"><span data-stu-id="40da6-107">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="40da6-108">A tevékenységnaplók az ügyfélfiókokkal és terméktranzakciókkal kapcsolatos partneri műveletek rekordjait biztosítják.</span><span class="sxs-lookup"><span data-stu-id="40da6-108">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="40da6-109">A tevékenységnaplókat .csv-fájlba is exportálhatja.</span><span class="sxs-lookup"><span data-stu-id="40da6-109">You can also export activity logs to a .csv file.</span></span>

## <a name="view-and-export-activity-logs"></a><span data-ttu-id="40da6-110">Tevékenységnaplók megtekintése és exportálása</span><span class="sxs-lookup"><span data-stu-id="40da6-110">View and export activity logs</span></span>

1. <span data-ttu-id="40da6-111">Jelentkezzen be a Partnerközpont [irányítópultjára.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="40da6-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="40da6-112">A **Fiókbeállítások menüben** válassza a **Tevékenységnapló lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="40da6-112">From the **Account settings** menu, select **Activity Log**.</span></span>

3. <span data-ttu-id="40da6-113">Válassza ki a Tevékenységnapló időszakát a **From** (Innen) és **a to (Vissza)** mezőkben.</span><span class="sxs-lookup"><span data-stu-id="40da6-113">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="40da6-114">A tevékenységnapló exportálása alapértelmezés szerint a legutóbbi hónapra van beállítva.</span><span class="sxs-lookup"><span data-stu-id="40da6-114">The activity log export defaults to the most recent month.</span></span>

   <span data-ttu-id="40da6-115">Minden tevékenységnapló tartalmaz egy hivatkozást a felsorolt ügyfél **Előfizetések oldalára.**</span><span class="sxs-lookup"><span data-stu-id="40da6-115">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

   <span data-ttu-id="40da6-116">A naplózott művelet részleteinek megtekintéséhez válasszon egy lefelé mutató nyilat bármely tevékenységnaplóhoz.</span><span class="sxs-lookup"><span data-stu-id="40da6-116">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="40da6-117">Egyetlen tevékenységnapló jelentős mennyiségű adatot mutathat, például több termék megrendelését.</span><span class="sxs-lookup"><span data-stu-id="40da6-117">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

4. <span data-ttu-id="40da6-118">A napló adatoszlopai a következők:</span><span class="sxs-lookup"><span data-stu-id="40da6-118">The data columns of the log include the following:</span></span>
   - <span data-ttu-id="40da6-119">**Dátum-idő**– a művelet dátuma és időpontja;</span><span class="sxs-lookup"><span data-stu-id="40da6-119">**Date-Time**-the date and time of the action;</span></span>
   - <span data-ttu-id="40da6-120">**Érintett ügyfél**– az ügyfél cégneve;</span><span class="sxs-lookup"><span data-stu-id="40da6-120">**Affected customer**—the customer's company name;</span></span>
   - <span data-ttu-id="40da6-121">**Művelet**– az ügyfél által tett művelet, például "létrehozta a ajánló";</span><span class="sxs-lookup"><span data-stu-id="40da6-121">**Action**—the action taken by the customer such as "created a referral";</span></span>
   - <span data-ttu-id="40da6-122">**Partnerfelhasználó**– a tevékenységhez társított partner.</span><span class="sxs-lookup"><span data-stu-id="40da6-122">**Partner user**—the partner associated with the activity.</span></span>

5. <span data-ttu-id="40da6-123">Válassza **a Napló exportálása** lehetőséget, hogy az ügyfél előfizetési adatait egy .csv-fájlba másolja, és töltse le a számítógép alapértelmezett letöltési mappájába.</span><span class="sxs-lookup"><span data-stu-id="40da6-123">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="40da6-124">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="40da6-124">Next steps</span></span>

- [<span data-ttu-id="40da6-125">Előfizetések és licencek elemzése az üzleti döntések meghozatala érdekében</span><span class="sxs-lookup"><span data-stu-id="40da6-125">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)
