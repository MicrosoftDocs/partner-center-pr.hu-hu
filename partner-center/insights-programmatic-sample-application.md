---
title: Mintaalkalmazás
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A mintaalkalmazással saját alkalmazást építhet a partnerelemzési adatok programozott módon való eléréséhez.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376662"
---
# <a name="sample-application"></a><span data-ttu-id="675b3-103">Mintaalkalmazás</span><span class="sxs-lookup"><span data-stu-id="675b3-103">Sample Application</span></span>

<span data-ttu-id="675b3-104">A mintaalkalmazások C# és JAVA nyelven vannak létrehozva, és elérhetők a [GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="675b3-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="675b3-105">C# mintaalkalmazás</span><span class="sxs-lookup"><span data-stu-id="675b3-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="675b3-106">JAVA-mintaalkalmazás</span><span class="sxs-lookup"><span data-stu-id="675b3-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="675b3-107">A mintaalkalmazásból ihletet meríthet, és bármilyen nyelven saját alkalmazást építhet.</span><span class="sxs-lookup"><span data-stu-id="675b3-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="675b3-108">A mintaalkalmazás a következő célokat éri el:</span><span class="sxs-lookup"><span data-stu-id="675b3-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="675b3-109">Létrehoz egy Azure Active Directory (Azure AD) jogkivonatot.</span><span class="sxs-lookup"><span data-stu-id="675b3-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="675b3-110">Lekérhetők az elérhető adatkészletek.</span><span class="sxs-lookup"><span data-stu-id="675b3-110">Gets available datasets.</span></span>
- <span data-ttu-id="675b3-111">Felhasználó által megadott lekérdezéseket hoz létre.</span><span class="sxs-lookup"><span data-stu-id="675b3-111">Creates user defined queries.</span></span>
- <span data-ttu-id="675b3-112">Lekérdezi a felhasználó által definiált és rendszerlekérdezések.</span><span class="sxs-lookup"><span data-stu-id="675b3-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="675b3-113">Ütemez egy jelentést.</span><span class="sxs-lookup"><span data-stu-id="675b3-113">Schedules a report.</span></span>

<span data-ttu-id="675b3-114">A mintaalkalmazás nem fedi le az API-k más funkciókhoz való meghívásának módját.</span><span class="sxs-lookup"><span data-stu-id="675b3-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="675b3-115">Az egyéb API-k meghívásának folyamata azonban ugyanaz marad, mint a fent vázolt.</span><span class="sxs-lookup"><span data-stu-id="675b3-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="675b3-116">Az alkalmazás futtatása</span><span class="sxs-lookup"><span data-stu-id="675b3-116">How to run the application</span></span>

- <span data-ttu-id="675b3-117">Klónozza az adattárat egy helyi rendszerbe a következő paranccsal:</span><span class="sxs-lookup"><span data-stu-id="675b3-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="675b3-118">További útmutatásért tekintse meg a ProgrammaticExportSampleAppMPN/README.md fájlt a GitHub [adattárban.](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)</span><span class="sxs-lookup"><span data-stu-id="675b3-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="675b3-119">Az alkalmazás gyors futtatásához frissítse az ügyfél-azonosítót és az ügyfél titkos **appsettings.Development.jsoldalon**</span><span class="sxs-lookup"><span data-stu-id="675b3-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Az appsetting fejlesztési JSON-ként való ábrázolása":::

<span data-ttu-id="675b3-121">Az alkalmazás futtatása elindít egy helyi webkiszolgálót, és megnyílik egy lap ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).</span><span class="sxs-lookup"><span data-stu-id="675b3-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Mintaalkalmazás felhasználói felületének ábrázolása":::

<span data-ttu-id="675b3-123">Ez az oldal API-hívásokat kezdeményez a helyi gépen futó webkiszolgálóhoz, amely pedig a tényleges programozott hozzáférési API-hívásokat fogja kezdeményezni.</span><span class="sxs-lookup"><span data-stu-id="675b3-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="675b3-124">Kódtöredékek</span><span class="sxs-lookup"><span data-stu-id="675b3-124">Code Snippets</span></span>

<span data-ttu-id="675b3-125">A programozott hozzáférési API-hívások C#-kódjának alapvető szerkezete a következő:</span><span class="sxs-lookup"><span data-stu-id="675b3-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Kódrészlet ábrázolása":::

## <a name="next-steps"></a><span data-ttu-id="675b3-127">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="675b3-127">Next steps</span></span>

[<span data-ttu-id="675b3-128">API-k a partnerelemzési adatok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="675b3-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
