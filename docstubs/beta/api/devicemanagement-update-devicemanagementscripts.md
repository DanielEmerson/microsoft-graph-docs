---
title: "Update deviceManagementScripts"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update deviceManagementScripts

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a deviceManagementScript object.

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

In the request body, supply JSON representation of the [deviceManagementScript](../resources/intune-devicemanagementscript.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a deviceManagementScript object.

| Property              | Type              | Description                                                                                   |
| :-------------------- | :---------------- | :-------------------------------------------------------------------------------------------- |
| createdDateTime       | DateTimeOffset    | The date and time the device management script was created. This property is read-only.       |
| description           | String            | Optional description for the device management script.                                        |
| displayName           | String            | Name of the device management script.                                                         |
| enforceSignatureCheck | Boolean           | Indicate whether the script signature needs be checked.                                       |
| fileName              | String            | Script file name.                                                                             |
| id                    | String            | Unique Identifier for the device management script. Read-only.                                |
| lastModifiedDateTime  | DateTimeOffset    | The date and time the device management script was last modified. This property is read-only. |
| roleScopeTagIds       | String collection | List of Scope Tag IDs for this PowerShellScript instance.                                     |
| runAs32Bit            | Boolean           | A value indicating whether the PowerShell script should run as 32-bit                         |
| runAsAccount          | String            | Indicates the type of execution context.                                                      |
| scriptContent         | Binary            | The script content.                                                                           |

## Response

If successful, this method returns a `200 OK` response code and a deviceManagementScript object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_devicemanagementscripts"
}
-->

```http
PATCH https://graph.microsoft.com/beta

Content-Type: application/json
Content-Length: 469

[
  {
    "@odata.type": "#microsoft.graph.deviceManagementScript",
    "createdDateTime": "DateTimeOffset",
    "description": "String",
    "displayName": "String",
    "enforceSignatureCheck": "Boolean",
    "fileName": "String",
    "id": "String(identifier)",
    "lastModifiedDateTime": "DateTimeOffset",
    "roleScopeTagIds": [
      "String"
    ],
    "runAs32Bit": "Boolean",
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
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": [
  {
    "@odata.type": "#microsoft.graph.deviceManagementScript",
    "createdDateTime": "DateTimeOffset",
    "description": "String",
    "displayName": "String",
    "enforceSignatureCheck": "Boolean",
    "fileName": "String",
    "id": "String(identifier)",
    "lastModifiedDateTime": "DateTimeOffset",
    "roleScopeTagIds": [
      "String"
    ],
    "runAs32Bit": "Boolean",
    "runAsAccount": "String",
    "scriptContent": "Binary"
  }
]
}

```