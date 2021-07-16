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
# <a name="sample-application"></a>Mintaalkalmazás

A mintaalkalmazások C# és JAVA nyelven vannak létrehozva, és elérhetők a [GitHub](https://github.com/partneranalytics)

- [C# mintaalkalmazás](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [JAVA-mintaalkalmazás](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

A mintaalkalmazásból ihletet meríthet, és bármilyen nyelven saját alkalmazást építhet.

A mintaalkalmazás a következő célokat éri el:

- Létrehoz egy Azure Active Directory (Azure AD) jogkivonatot.
- Lekérhetők az elérhető adatkészletek.
- Felhasználó által megadott lekérdezéseket hoz létre.
- Lekérdezi a felhasználó által definiált és rendszerlekérdezések.
- Ütemez egy jelentést.

A mintaalkalmazás nem fedi le az API-k más funkciókhoz való meghívásának módját. Az egyéb API-k meghívásának folyamata azonban ugyanaz marad, mint a fent vázolt.

## <a name="how-to-run-the-application"></a>Az alkalmazás futtatása

- Klónozza az adattárat egy helyi rendszerbe a következő paranccsal:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> További útmutatásért tekintse meg a ProgrammaticExportSampleAppMPN/README.md fájlt a GitHub [adattárban.](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

- Az alkalmazás gyors futtatásához frissítse az ügyfél-azonosítót és az ügyfél titkos **appsettings.Development.jsoldalon**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Az appsetting fejlesztési JSON-ként való ábrázolása":::

Az alkalmazás futtatása elindít egy helyi webkiszolgálót, és megnyílik egy lap ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Mintaalkalmazás felhasználói felületének ábrázolása":::

Ez az oldal API-hívásokat kezdeményez a helyi gépen futó webkiszolgálóhoz, amely pedig a tényleges programozott hozzáférési API-hívásokat fogja kezdeményezni.

## <a name="code-snippets"></a>Kódtöredékek

A programozott hozzáférési API-hívások C#-kódjának alapvető szerkezete a következő:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Kódrészlet ábrázolása":::

## <a name="next-steps"></a>Következő lépések

[API-k a partnerelemzési adatok eléréséhez](insights-programmatic-analytics-available-api.md)
