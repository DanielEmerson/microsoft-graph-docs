---
title: "Create deviceShellScripts"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create deviceShellScripts

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new deviceShellScript object.

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

In the request body, supply JSON representation of the [deviceShellScript](../resources/intune-deviceshellscript.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a deviceShellScript object.

| Property                    | Type              | Description                                                                                   |
| :-------------------------- | :---------------- | :-------------------------------------------------------------------------------------------- |
| blockExecutionNotifications | Boolean           | Does not notify the user a script is being executed                                           |
| createdDateTime             | DateTimeOffset    | The date and time the device management script was created. This property is read-only.       |
| description                 | String            | Optional description for the device management script.                                        |
| displayName                 | String            | Name of the device management script.                                                         |
| executionFrequency          | Duration          | The interval for script to run. If not defined the script will run once                       |
| fileName                    | String            | Script file name.                                                                             |
| id                          | String            | Unique Identifier for the device management script. Read-only.                                |
| lastModifiedDateTime        | DateTimeOffset    | The date and time the device management script was last modified. This property is read-only. |
| retryCount                  | Int32             | Number of times for the script to be retried if it fails                                      |
| roleScopeTagIds             | String collection | List of Scope Tag IDs for this PowerShellScript instance.                                     |
| runAsAccount                | String            | Indicates the type of execution context.                                                      |
| scriptContent               | Binary            | The script content.                                                                           |

## Response

If successful, this method returns a `201 Created` response code and a deviceShellScript object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_deviceshellscripts"
}
-->

```http
POST https://graph.microsoft.com/beta

Content-Type: application/json
Content-Length: 507

[
  {
    "@odata.type": "#microsoft.graph.deviceShellScript",
    "blockExecutionNotifications": "Boolean",
    "createdDateTime": "DateTimeOffset",
    "description": "String",
    "displayName": "String",
    "executionFrequency": "Duration",
    "fileName": "String",
    "id": "String(identifier)",
    "lastModifiedDateTime": "DateTimeOffset",
    "retryCount": "Int32",
    "roleScopeTagIds": [
      "String"
    ],
    "runAsAccount": "String",
    "scriptContent": "Binary"
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
    "@odata.type": "#microsoft.graph.deviceShellScript",
    "blockExecutionNotifications": "Boolean",
    "createdDateTime": "DateTimeOffset",
    "description": "String",
    "displayName": "String",
    "executionFrequency": "Duration",
    "fileName": "String",
    "id": "String(identifier)",
    "lastModifiedDateTime": "DateTimeOffset",
    "retryCount": "Int32",
    "roleScopeTagIds": [
      "String"
    ],
    "runAsAccount": "String",
    "scriptContent": "Binary"
  }
]
}

```