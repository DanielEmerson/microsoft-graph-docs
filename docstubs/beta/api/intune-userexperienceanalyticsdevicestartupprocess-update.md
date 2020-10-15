---
title: "Update userExperienceAnalyticsDeviceStartupProcess"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update userExperienceAnalyticsDeviceStartupProcess

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a userExperienceAnalyticsDeviceStartupProcess object.

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

In the request body, supply JSON representation of the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-userexperienceanalyticsdevicestartupprocess.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a userExperienceAnalyticsDeviceStartupProcess object.

| Property          | Type   | Description                                                                               |
| :---------------- | :----- | :---------------------------------------------------------------------------------------- |
| id                | String | The unique identifier of the user experience analytics device startup process. Read-only. |
| managedDeviceId   | String | The user experience analytics device id.                                                  |
| processName       | String | User experience analytics device startup process name.                                    |
| productName       | String | The user experience analytics device startup process product name.                        |
| publisher         | String | The User experience analytics device startup process publisher.                           |
| startupImpactInMs | Int32  | User experience analytics device startup process impact in milliseconds.                  |

## Response

If successful, this method returns a `200 OK` response code and a userExperienceAnalyticsDeviceStartupProcess object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_userexperienceanalyticsdevicestartupprocess"
}
-->

```http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{id}

Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "managedDeviceId": "String",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "startupImpactInMs": "Int32"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsDeviceStartupProcess"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "id": "String(identifier)",
  "managedDeviceId": "String",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "startupImpactInMs": "Int32"
}
}

```