---
title: "Create userExperienceAnalyticsAppHealthDevicePerformanceDetails"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create userExperienceAnalyticsAppHealthDevicePerformanceDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new userExperienceAnalyticsAppHealthDevicePerformanceDetails object.

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

In the request body, supply JSON representation of the userExperienceAnalyticsAppHealthDevicePerformanceDetails object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create an userExperienceAnalyticsAppHealthDevicePerformanceDetails object.

| Property          | Type           | Description                                                                                  |
| :---------------- | :------------- | :------------------------------------------------------------------------------------------- |
| appDisplayName    | String         | The friendly name of the application for which the event occurred.                           |
| deviceDisplayName | String         | The name of the device.                                                                      |
| deviceId          | String         | The id of the device.                                                                        |
| eventDateTime     | DateTimeOffset | The time the event occurred.                                                                 |
| eventType         | String         | The type of the event.                                                                       |
| id                | String         | The unique identifier of the user experience analytics device performance object. Read-only. |

## Response

If successful, this method returns a `201 Created` response code and an userExperienceAnalyticsAppHealthDevicePerformanceDetails object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsapphealthdeviceperformancedetails"
}
-->

```http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails/{id}

Content-Type: application/json
Content-Length: 252

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "appDisplayName": "String",
  "deviceDisplayName": "String",
  "deviceId": "String",
  "eventDateTime": "DateTimeOffset",
  "eventType": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsAppHealthDevicePerformanceDetails"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "appDisplayName": "String",
  "deviceDisplayName": "String",
  "deviceId": "String",
  "eventDateTime": "DateTimeOffset",
  "eventType": "String",
  "id": "String(identifier)"
}
}

```