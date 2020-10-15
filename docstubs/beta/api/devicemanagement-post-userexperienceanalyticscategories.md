---
title: "Create userExperienceAnalyticsCategories"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create userExperienceAnalyticsCategories

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new userExperienceAnalyticsCategory object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request Body

In the request body, supply JSON representation of the [userExperienceAnalyticsCategory](../resources/intune-userexperienceanalyticscategory.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a userExperienceAnalyticsCategory object.

| Property     | Type                                                                                        | Description                                                                 |
| :----------- | :------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------- |
| id           | String                                                                                      | The unique identifier of the user experience analytics category. Read-only. |
| insights     | [userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection | The insights for the user experience analytics category.                    |
| overallScore | Int32                                                                                       | The overall score of the user experience analytics category.                |
| state        | String                                                                                      | The current health state of the user experience analytics category.         |

## Response

If successful, this method returns a `201 Created` response code and a userExperienceAnalyticsCategory object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticscategories"
}
-->

```http
POST https://graph.microsoft.com/beta

Content-Type: application/json
Content-Length: 565

[
  {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
    "id": "String(identifier)",
    "insights": [
      {
        "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
        "insightId": "String",
        "severity": "String",
        "userExperienceAnalyticsMetricId": "String",
        "values": [
          {
            "@odata.type": "#microsoft.graph.insightValueDouble",
            "value": "Double"
          }
        ]
      }
    ],
    "overallScore": "Int32",
    "state": "String"
  }
]

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "$(this.ReturnTypeFullName)"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": [
  {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
    "id": "String(identifier)",
    "insights": [
      {
        "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
        "insightId": "String",
        "severity": "String",
        "userExperienceAnalyticsMetricId": "String",
        "values": [
          {
            "@odata.type": "#microsoft.graph.insightValueDouble",
            "value": "Double"
          }
        ]
      }
    ],
    "overallScore": "Int32",
    "state": "String"
  }
]
}

```