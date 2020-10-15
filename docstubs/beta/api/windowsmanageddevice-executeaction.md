---
title: "windowsmanageddevice : executeAction"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# windowsmanageddevice : executeAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

In the request body, supply JSON representation of the parameters.

<!-- Actions and Functions -->

The following table shows the parameters that can be used with this method.

| Parameter          | Type              | Description |
| :----------------- | :---------------- | :---------- |
| actionName         | String            |             |
| keepEnrollmentData | Boolean           |             |
| keepUserData       | Boolean           |             |
| deviceIds          | String collection |             |
| notificationTitle  | String            |             |
| notificationBody   | String            |             |
| deviceName         | String            |             |

<!-- CRUD Methods -->

## Response

If successful, this method returns a `200 Ok` response code and a bulkManagedDeviceActionResult object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "windowsmanageddevice_executeaction"
}
-->

```http
POST https://graph.microsoft.com/beta/users/{id}/managedDevices/{id}/executeAction

Content-Type: application/json
Content-Length: 259

{
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ],
  "successfulDeviceIds": [
    "String"
  ]
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.bulkManagedDeviceActionResult"
}
-->

```http
HTTP 1.1 200 Ok

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ],
  "successfulDeviceIds": [
    "String"
  ]
}
}

```