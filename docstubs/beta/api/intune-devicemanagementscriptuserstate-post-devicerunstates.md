---
title: "Create deviceRunStates"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create deviceRunStates

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new deviceManagementScriptDeviceState object.

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

In the request body, supply JSON representation of the [deviceManagementScriptDeviceState](../resources/intune-devicemanagementscriptdevicestate.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a deviceManagementScriptDeviceState object.

| Property                | Type           | Description                                                                                     |
| :---------------------- | :------------- | :---------------------------------------------------------------------------------------------- |
| errorCode               | Int32          | Error code corresponding to erroneous execution of the device management script.                |
| errorDescription        | String         | Error description corresponding to erroneous execution of the device management script.         |
| id                      | String         | Key of the device management script device state entity. This property is read-only. Read-only. |
| lastStateUpdateDateTime | DateTimeOffset | Latest time the device management script executes.                                              |
| resultMessage           | String         | Details of execution output.                                                                    |
| runState                | String         | State of latest run of the device management script.                                            |

## Response

If successful, this method returns a `201 Created` response code and a deviceManagementScriptDeviceState object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_devicerunstates"
}
-->

```http
POST https://graph.microsoft.com/beta

Content-Type: application/json
Content-Length: 291

[
  {
    "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
    "errorCode": "Int32",
    "errorDescription": "String",
    "id": "String(identifier)",
    "lastStateUpdateDateTime": "DateTimeOffset",
    "resultMessage": "String",
    "runState": "String"
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
    "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
    "errorCode": "Int32",
    "errorDescription": "String",
    "id": "String(identifier)",
    "lastStateUpdateDateTime": "DateTimeOffset",
    "resultMessage": "String",
    "runState": "String"
  }
]
}

```