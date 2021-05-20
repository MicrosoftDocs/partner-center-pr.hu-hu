---
title: Azure-előfizetések hozzárendelése az ügyfelekhez
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Megtudhatja, hogyan rendelhet Azure-előfizetéseket az ügyfeleihez a Partnerközpont és hogyan engedélyezheti az ügyfeleknek a saját előfizetéseik kezelését.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aba4f97ad6a385c2a9e36c95354a9d53e38ba9e3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149978"
---
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a><span data-ttu-id="7b738-103">Azure-előfizetések hozzárendelése az ügyfelekhez Partnerközpont</span><span class="sxs-lookup"><span data-stu-id="7b738-103">Assigning Azure subscriptions to customers in Partner Center</span></span>

<span data-ttu-id="7b738-104">**Megfelelő szerepkörök:** Globális rendszergazdai | Értékesítési ügynök</span><span class="sxs-lookup"><span data-stu-id="7b738-104">**Appropriate roles**: Global admin | Sales agent</span></span>

## <a name="assign-azure-subscriptions-to-your-customers"></a><span data-ttu-id="7b738-105">Azure-előfizetések hozzárendelése az ügyfelekhez</span><span class="sxs-lookup"><span data-stu-id="7b738-105">Assign Azure subscriptions to your customers</span></span>

1. <span data-ttu-id="7b738-106">Válassza **az Ügyfelek** Partnerközpont menüben, és keresse meg a kezelni kívánt ügyfelet. </span><span class="sxs-lookup"><span data-stu-id="7b738-106">Select **Customers** from your **Partner Center** menu and locate the customer you want to manage.</span></span>

2. <span data-ttu-id="7b738-107">A sor végén lévő lefelé mutató nyílra kattintva bontsa ki az ügyfél rekordját, majd válassza a **a Microsoft Azure felügyeleti portálja.**</span><span class="sxs-lookup"><span data-stu-id="7b738-107">Select the down arrow at the end of the row to expand the customer's record and then select **Microsoft Azure Management Portal**.</span></span> <span data-ttu-id="7b738-108">A következő webhelyre [](https://portal.azure.com/) lesz irányítva Azure Portal ahol kezelheti az ügyfél előfizetését.</span><span class="sxs-lookup"><span data-stu-id="7b738-108">You will be directed to the [Azure portal](https://portal.azure.com/) where you can manage the customer's subscriptions.</span></span>

3. <span data-ttu-id="7b738-109">A Azure Portal válassza az **Előfizetések lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7b738-109">From the Azure portal, select **Subscriptions**.</span></span>

4. <span data-ttu-id="7b738-110">Válassza ki a hozzárendelni kívánt előfizetést, majd válassza **a** Access Control.</span><span class="sxs-lookup"><span data-stu-id="7b738-110">Select the subscription you would like to assign, then select **Access Control**.</span></span>

5. <span data-ttu-id="7b738-111">Válassza **a Hozzáadás** lehetőséget, hogy hozzáadja a felhasználót az előfizetéshez.</span><span class="sxs-lookup"><span data-stu-id="7b738-111">Select **Add** to add a user to the subscription.</span></span> 

6. <span data-ttu-id="7b738-112">Miután hozzáadta a felhasználót az előfizetéshez, hozzárendelhet egy szerepkört és azt a fiókot, amelyhez a felhasználónak hozzáférése lesz.</span><span class="sxs-lookup"><span data-stu-id="7b738-112">After you add the user to the subscription, you can assign the user a role and the specific account that user will have access to.</span></span>

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a><span data-ttu-id="7b738-113">Azure-előfizetések kezelése az ügyfelek számára</span><span class="sxs-lookup"><span data-stu-id="7b738-113">Enable customers to manage their Azure subscriptions</span></span>

<span data-ttu-id="7b738-114">Miután létrehozott egy Microsoft Azure számára, engedélyezheti számukra az előfizetés kezelését.</span><span class="sxs-lookup"><span data-stu-id="7b738-114">After you create a Microsoft Azure subscription for a customer, you can enable them to manage the subscription.</span></span> <span data-ttu-id="7b738-115">Ehhez be kell jelentkeznie az ügyfél felügyeleti Microsoft Azure portálra.</span><span class="sxs-lookup"><span data-stu-id="7b738-115">To do this, you'll need to log on to the customer's Microsoft Azure Management portal.</span></span> 

1. <span data-ttu-id="7b738-116">Az ügyfél nevének megnyitásához Azure Portal bontsa ki az ügyfél termékoldalát az ügyféllistában, vagy válassza ki az ügyfél nevét, majd válassza a **a Microsoft Azure felügyeleti portálja.**</span><span class="sxs-lookup"><span data-stu-id="7b738-116">To open the customer's Azure portal, either expand the customer's listing in your customer list or select the customer's name and then select **Microsoft Azure Management Portal**.</span></span>

   > [!NOTE]  
   > <span data-ttu-id="7b738-117">Ha a rendszer arra kéri, hogy jelentkezzen be a Azure Portal, előfordulhat, hogy nem rendelkezik delegált rendszergazdai jogosultságokkal.</span><span class="sxs-lookup"><span data-stu-id="7b738-117">If you are prompted to log onto the Azure portal, you may not have delegated administrative privileges.</span></span> <span data-ttu-id="7b738-118">Válassza **a Kapcsolat kérése lehetőséget,** hogy meghívja az ügyfelet, hogy azonosítsa Önt mint rekordpartnert.</span><span class="sxs-lookup"><span data-stu-id="7b738-118">Select **Request a relationship** to invite the customer to identify you as their Partner of Record.</span></span> <span data-ttu-id="7b738-119">Miután az ügyfél elfogadja a meghívást, Automatikusan delegált rendszergazdai jogosultságokat kap.</span><span class="sxs-lookup"><span data-stu-id="7b738-119">After the customer accepts your invitation, you are automatically granted delegated administrative privileges.</span></span>

2. <span data-ttu-id="7b738-120">A Azure Portal nyissa meg az ügyfél előfizetési listáját, és válassza ki az ügyfél Azure-előfizetését.</span><span class="sxs-lookup"><span data-stu-id="7b738-120">In the Azure portal, open the customer's subscriptions list and select the customer's Azure subscription.</span></span>

3. <span data-ttu-id="7b738-121">Rendeljen hozzá egy szerepkört az ügyfél bármely felhasználója számára, hogy az előfizetése alatt erőforrásokat hoz létre és kezelhet.</span><span class="sxs-lookup"><span data-stu-id="7b738-121">Assign a role to any of the customer's users so that they can create and manage resources under their subscription.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7b738-122">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="7b738-122">Next steps</span></span>

- [<span data-ttu-id="7b738-123">Hogyan értékesítik az előfizetéseket a CSP-partnerek az ügyfeleknek?</span><span class="sxs-lookup"><span data-stu-id="7b738-123">How CSP partners can sell subscriptions to customers</span></span>](customer-subscriptions.md)

- [<span data-ttu-id="7b738-124">Ügyfél szolgáltatásának vagy előfizetéseinek kezeléséhez szükséges engedélyek beszerzése</span><span class="sxs-lookup"><span data-stu-id="7b738-124">How to obtain permissions to manage a customer's service or subscriptions</span></span>](customers-revoke-admin-privileges.md)
