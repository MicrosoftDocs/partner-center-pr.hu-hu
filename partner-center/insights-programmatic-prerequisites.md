---
title: Az elemzési adatok programozott elérésének előfeltételei
description: Az elemzési adatok programozott elérésének előfeltételei
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376667"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Az elemzési adatok programozott elérésének előfeltételei

**Megfelelő szerepkörök:** Globális rendszergazdai | MPN-rendszergazda

Mielőtt programozott módon hozzáfér a partnerelemzési adatokhoz, teljesítenie kell az alábbi követelményeket.

## <a name="mpn-program-enrollment"></a>MPN-program regisztrálása

A partnerelemzési adatok programozott eléréséhez regisztrálni kell az MPN-programban, és létre kell Partnerközpont fiókkal. További információ: [MPN-fiók létrehozása a Partnerközpont](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Azure Active Directory (AAD) alkalmazás létrehozása

A partneradatok programozott eléréséhez nem használhatók normál felhasználói hitelesítő adatok Elemzések Analytics-adatokhoz. A Azure Active Directory hozzáférési API-k eléréséhez létre kell Azure Active Directory (AAD) alkalmazást és egy titkos elérésű (alkalmazás + felhasználói hozzáférés) alkalmazást. Az AAD-alkalmazások és titkos információk létrehozásáról lásd: Rövid útmutató: Alkalmazás regisztrálása [a Microsoft Identitásplatform.](/azure/active-directory/develop/quickstart-register-app)   A Microsoft-fiók eléréséhez engedély Partner API. Az engedélyek hozzáadásának elsajátításért lásd: Partner API [hitelesítés – Partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Vezetői jelentésmegjelenítő (ERV) szerepkör hozzárendelése a felhasználóhoz

A partnerelemzési adatok programozott módon való eléréséhez az Executive Report Viewer (ERV) alkalmazással kell rendelkezésre lennie. Az ERV szerepkör felhasználóhoz való hozzárendelésének elsajátításért lásd: Partnerközpont Elemzések hozzáférés hozzárendelése – [Partnerközpont](insights-roles.md)

## <a name="generate-an-aad-token"></a>AAD-jogkivonat létrehozása

Létre kell hoznia egy AAD-jogkivonatot az alkalmazás (ügyfél) azonosítójával, titkos ügyfél titkos kódjával, a felhasználói azonosítójával és jelszavával.   [Itt ellenőrizheti](insights-programmatic-first-api-call.md#token-generation) az AAD-jogkivonat létrehozásához szükséges lépéseket.

> [!Note]
> A jogkivonat egy óráig érvényes.

## <a name="next-steps"></a>Következő lépések
[Programozott hozzáférési paradigma](insights-programmatic-access-paradigm.md)