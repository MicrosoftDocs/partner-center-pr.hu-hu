---
title: Számlázás – licencalapú SaaS-tranzakciók
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg a licencalapú Partnerközpont saaS-tranzakciókra vonatkozó gyakori számlázási forgatókönyveket.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 764d5a3cb0dc6f409e5272d4119424396caff53b
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148635"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Gyakori számlázási forgatókönyvek licencalapú SaaS-tranzakciókhoz a Partnerközpont

**Megfelelő szerepkörök:** Rendszergazdai ügynök | Számlázási rendszergazdai | Az | Értékesítési ügynök


Ezek a [gyakori számlázási forgatókönyvek](common-billing-scenarios.md) a licencalapú szolgáltatott szoftver (SaaS) előfizetésére vonatkoznak a Partnerközpont.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Ingyenes próba SaaS-előfizetés konvertálása fizetős előfizetésre

Ez a forgatókönyv a licencalapú ingyenes próba SaaS-előfizetés megújításának számlázását ismerteti. A megújítás az ingyenes próbaidőszak végén fizetős előfizetésre konvertálja az ingyenes próbaverziót.

Ebben a példában egy licencalapú SaaS- (szolgáltatott szoftver) előfizetés ingyenes próbaverzióját vásárolta meg június 10-én. Az ingyenes próbaidőszak végén az ingyenes próbaverzió automatikusan megújul fizetős előfizetésként.

A felderítési fájlok a következő díjakat tartalmazzák:

| Vásárlás dátuma | Díj kezdő dátuma | Díj záró dátuma | Egységár | Egységmennyiség | Teljes összeg | Díj típusa | Előfizetés leírása |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 1 | 0 USD | Új | Ingyenes próbaidőszak |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 USD | 1 | 2 USD | Frissítés | Fizetős előfizetés |

## <a name="cancel-a-free-trial-saas-subscription"></a>Ingyenes próba SaaS-előfizetés lemondása

> [!TIP]
> A licencalapú ingyenes SaaS-próbaverziós előfizetést bármikor lemondhatja, még az ingyenes próbaidőszak alatt is.

Ebben a forgatókönyvben július 1-én vásárolt egy licencalapú ingyenes Próba SaaS-előfizetést, majd azonnal megszakította azt a Partnerközpont.

A felderítési fájl a következő díjakat tartalmazza:

| Vásárlás dátuma | Díj kezdő dátuma | Díj záró dátuma | Egységár | Egységmennyiség | Teljes összeg | Díj típusa | Előfizetés leírása |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Új | Ingyenes próbaidőszak |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 USD | 11 | 0 USD | Mégse | Ingyenes próbaidőszak |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Egyéni fogyasztásmérő SaaS-előfizetésének konvertálása másik termékváltozatra

Ez a forgatókönyv azt ismerteti, hogyan alakítható át egy egyéni fogyasztásmérő SaaS-előfizetése egy készleten található egységről (SKU) egy másik termékváltozatra ugyanazon a terméken ugyanazon a napon.

Ebben a forgatókönyvben megvásárolt egy termékváltozatot (ezüstöt) egy termék alatt, és ugyanezen a napon konvertálta egy másik elérhető termékváltozatra (bronz).

A felderítési fájl a következő díjakat tartalmazza:

| Vásárlás dátuma | Termékváltozat | Díj kezdő dátuma | Díj záró dátuma | Egységár | Egységmennyiség | Teljes összeg | Díj típusa | Előfizetés leírása |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Ezüst | 06/10/2019 | 06/10/2019 | 20 USD | 1 | 20 USD | Új | Egyéni fogyasztásmérő SaaS-előfizetése |
| 06/10/2019 | Ezüst | 06/10/2019 | 06/10/2019 | 20 USD | 1 | -20 USD | Konvertálás | Egyéni fogyasztásmérő SaaS-előfizetésének újrabetöltési időszaka |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Konvertálás | Egyéni fogyasztásmérő SaaS-előfizetése |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Ügyfélmérő SaaS-előfizetés vásárlása és lemondása ugyanezen a napon

Ez a forgatókönyv azt írja le, hogy az ügyfélmérő SaaS-előfizetésének számlázása az ugyanazon a napon vásárolt és Azure Portal időpontban lett-e meg.

Ebben a forgatókönyvben egyéni mérő SaaS-előfizetést vásárolt a Azure Portal. Ezután ugyanezen a napon lemondta az előfizetést.

| Vásárlás dátuma | Termékváltozat | Díj kezdő dátuma | Díj záró dátuma | Egységár | Egységmennyiség | Teljes összeg | Díj típusa | Előfizetés leírása |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10 USD | 1 | 10 USD | Új | Egyéni fogyasztásmérő SaaS-előfizetése |
| 06/10/2019 | Bronz | 06/10/2019 | 06/10/2019 | 10 USD | 1 | -10 USD | CancelImmediate (Szerviz törlése) | Egyéni fogyasztásmérő SaaS-előfizetése |
