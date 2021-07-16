---
title: Az első API-hívás a partnerelemzési adatok eléréséhez
description: Példák arra, hogyan használható az API a partnerelemzési adatok eléréséhez.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d2252ccfb601ae22ce106d87fb06b67bf0927df5
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376670"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a>Az első API-hívás a partnerelemzési adatok eléréséhez

A partnerelemzési adatok eléréséhez szükséges API-k listáját lásd: API-k a partnerelemzési adatok [eléréséhez.](insights-programmatic-analytics-available-api.md) Az első API-hívás előtt győződjön meg [](insights-programmatic-prerequisites.md) arról, hogy teljesülnek a partneri és elemzési Elemzések előfeltételei.

## <a name="token-generation"></a>Jogkivonat létrehozása

A metódusok hívása előtt be kell szereznie egy Azure Active Directory (AAD) hozzáférési jogkivonatot. Át kell adni az Azure AD hozzáférési jogkivonatot az API minden metódusának Authorization fejlécéhez. A hozzáférési jogkivonat beszerzése után 60 perc alatt használhatja azt a lejárata előtt. A jogkivonat lejárata után frissítheti a jogkivonatot, és továbbra is használhatja az API-hoz való további hívásokhoz.

A jogkivonat létrehozásához tekintse meg az alábbi mintakérést. A jogkivonat létrehozásához szükséges három érték a `clientId` , a és a `clientSecret` `tenantId` . Az erőforrás-paramétert a következőre kell beállítani: `https://api.partnercenter.microsoft.com`

#### <a name="request-example"></a>Példa kérésre

```console
curl --location --request POST 'https://login.microsoftonline.com/<tenantId>/oauth2/token' \
--header 'return-client-request-id: true' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: fpc=Ar2GMei7JwdKg4Y4onHrMpvxqd4FAQAAAEhU_tcOAAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd' \
--data-urlencode 'resource= https://api.partnercenter.microsoft.com' \
--data-urlencode 'client_id= ' \
--data-urlencode 'client_secret= ' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username= ' \
--data-urlencode 'password= '
```

#### <a name="response-example"></a>Példa válaszra

```json
{
    "token_type": "Bearer",
    "expires_in": "3599",
    "ext_expires_in": "3599",
    "expires_on": "1612794445",
    "not_before": "1612790545",
    "resource": "https://api.partnercenter.microsoft.com",
    "access_token": {Token}
}
```

További információ az alkalmazás Azure AD-jogkivonatának beszerzéséről: Access analytics data using Store services (Elemzési adatok elérése [a Store-szolgáltatások használatával).](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)

## <a name="programmatic-api-call"></a>Programozott API-hívás

Miután beszerezte az AAD-jogkivonatot az előző szakaszban leírtak szerint, kövesse az alábbi lépéseket az első programozott hozzáférési jelentés létrehozásához.

Az adatok a következő adatkészletből tölthetők le (datasetName):

- CustomersAndTenants
- SeatsSubscriptionsAndRevenue
- AzureUsage
- MSLearn
- OfficeUsage
- Profil
- TrainingCompletions (Betanítás kiegészítések)
- DynamicsUsage
- KompetenciaSummaryHistory
- PowerBIUsage
- EMSUsage
- KompetenciaPeformanceRequirement
- ResellerPerformance
- CLASAgreementRenewalsPropensity
- CLASAzurePropensity
- CLASD365Propensity
- CLASM365Propensity
- TeamsUsage3PApps
- TeamsUsageWorkload
- TeamsUsageMeetingsAndCalls

A következő szakaszban példákat láthat arra, hogyan lehet programozott módon hozzáférni `SubscriptionId` a DynamicsUsage adatkészletből.

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a>1. lépés: REST-hívás a get datasets API használatával

Az API-válasz megszabadja az adatkészlet nevét, ahonnan letöltheti a jelentést. Az adott adatkészlethez az API-válasz az egyéni jelentéssablonhoz használható választható oszlopok listáját is tartalmazza. Az oszlopok nevét [](insights-data-definitions.md) az adatdefiníciókban is lekértük.

#### <a name="request-example"></a>Példa kérésre

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Példa válaszra

```json
{
  "value": [
    {
      "datasetName": "DynamicsUsage",
      "selectableColumns": [
        "PGAMpnId",
        "SubscriptionId",
        "SubscriptionStartDate",
        "SubscriptionEndDate",
        "SubscriptionStatus",
        "Month",
        "RevSumDivisionName",
        "RevSumCategoryName",
        "SKU",
        "SKUId",
        "FreeVsPaidSKU",
        "SalesModel",
        "DetailedSalesModel",
        "CustomerName",
        "CustomerTenantId",
        "CustomerTpid",
        "CustomerSegment",
        "CustomerMarket",
        "MPNId",
        "PartnerName",
        "PartnerLocation",
        "PartnerAttachType",
        "AvailableSeats",
        "AssignedSeats",
        "ActiveSeats",
        "DeploymentOpportunity",
        "ActiveUsagePercent"
      ],
      "availableMetrics": [
        "SubscriptionCount",
        "TotalAssignedSeats",
        "TotalSoldSeats",
        "TotalActiveSeats",
        "TotalRevenueAndACR",
        "CustomerCount",
        "CustomerTenantCount"
      ],
      "availableDateRanges": [
        "LAST_MONTH",
        "LAST_3_MONTHS",
        "LAST_6_MONTHS",
        "LAST_1_YEAR",
        "LIFETIME"
      ],
      "minimumRecurrenceInterval": 24
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Dataset fetched successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-2-create-the-custom-query"></a>2. lépés: Az egyéni lekérdezés létrehozása

Ebben a lépésben a DynamicsUsage adatkészlet SubscriptionId (Előfizetés-azonosító) mezőivel hozunk létre egyéni lekérdezést a kívánt jelentéshez. Ha a lekérdezésben nincs megadva, az alapértelmezett időtartam 6 hónap.

#### <a name="request-example"></a>Példa kérésre

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries' \ 
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
{
  "Name": "SubscriptionId Dynamics ",
  "Description": "List of Subscription Id from DynamicsUsage",
  "Query": "SELECT SubscriptionId from DynamicsUsage "
            }"
```

#### <a name="response-example"></a>Példa válaszra

```json
{
  "value": [
    {
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "name": "SubscriptionId Dynamics",
      "description": "List of Subscription Id from DynamicsUsage",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T07:28:37Z"
    }
 ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

A lekérdezés sikeres végrehajtásakor egy jön létre, amely a jelentés létrehozásához `queryId` szükséges.

### <a name="step-3-execute-test-query-api"></a>3. lépés: Tesztlekérdezés VÉGREHAJTÁSA API

Ebben a lépésben a tesztlekérdezés API-val lekértjük a létrehozott lekérdezés első 100 sorát.

#### <a name="request-example"></a>Példa kérésre

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Példa válaszra

```json
{
  "value": [
    {
      "SubscriptionId": "251DE3D4-8868-4032-B518-F142DA50522F"
    },
    {
      "SubscriptionId": "758A0647-790C-435B-BEAA-652DF47E327C"
    },
    {
      "SubscriptionId": "ACE5A84B-9794-4480-82C5-AF9462DE2589"
    },
    {
      "SubscriptionId": "C75163EE-A0CA-4822-8275-E29E2490FF1C"
    },
    {
      "SubscriptionId": "082A8A18-0834-4376-A9A4-3AA4ECD02826"
    },
    .
    .
    .
    {
      "SubscriptionId": "5E10B817-7FCB-43CE-9F32-9CB60CF14658"
    },
    {
      "SubscriptionId": "7578872A-18C1-4E6B-8F51-469555337389"
    },
    {
      "SubscriptionId": "00601E10-4C05-4BA2-B977-6578F5C81D69"
    },
    {
      "SubscriptionId": "7EBFC3A9-D502-4EA2-87E7-C42971639E8C"
    },
    {
      "SubscriptionId": "2AC30AE1-5934-48FB-A0E5-EF6985761138"
    }
  ],
  "nextLink": null,
  "totalCount": 100,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-4-create-the-report"></a>4. lépés: A jelentés létrehozása

Ebben a lépésben a korábban létrehozott QueryId lekérdezésazonosítót használjuk a jelentés létrehozásához.

#### <a name="request-example"></a>Példa kérésre

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport'\
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
'{
  "ReportName": "DynamicsUsage Subscription ID Report",
  "Description": "Report for getting list of Subscription Id for Dynamics Usage",
  "QueryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
  "StartTime": "2021-04-01T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": "2021-03-31T18:41:00Z",
  "QueryEndTime": "2021-06-30T18:41:00Z",
  "RecurrenceInterval": 48,
  "RecurrenceCount": 20,
  "Format": "csv",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}'
```

#### <a name="response-example"></a>Példa válaszra

```json
{
  "value": [
    {
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "reportName": "DynamicsUsage Subscription ID Report",
      "description": "Report for getting list of Subscription Id for Dynamics Usage",
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T08:15:15Z",
      "modifiedTime": null,
      "executeNow": false,
      "startTime": "2021-04-01T18:41:00Z",
      "reportStatus": "Active",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": "https://<SampleCallbackUrl>",
      "CallbackMethod": "GET",
      "format": "csv"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Report created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Sikeres végrehajtás esetén létrejön egy , amely a jelentés letöltésének ütemezéséhez `reportId` szükséges.

### <a name="step-5-execute-report-executions-api"></a>5. lépés: A Report Executions API végrehajtása

Ebben a lépésben a Jelentésvégrehajtások API-val lekértjük a jelentés biztonságos helyét (URL-címét).

#### <a name="request-example"></a>Példa kérésre

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a>Példa válaszra

```json
{
  "value": [
    {
      "executionId": "315eb63e-e2b2-41a2-ad8e-790b040fdce3",
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": null,
      "CallbackMethod": null,
      "format": "csv",
      "executionStatus": "Pending",
      "reportLocation": null,
      "reportAccessSecureLink": null,
      "reportExpiryTime": null,
      "reportGeneratedTime": null
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

## <a name="next-steps"></a>Következő lépések

- Próbálja ki az API-kat a [swagger API URL-címével](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)