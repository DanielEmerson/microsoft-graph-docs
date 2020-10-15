---
title: "List comanagementEligibleDevices"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# List comanagementEligibleDevices

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the comanagementEligibleDevice objects from a comanagementEligibleDevices navigation property.

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

## Optional query parameters

This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Request Body

<!-- Actions and Functions -->

<!-- CRUD Methods -->

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 Ok` response code and a comanagementEligibleDevice object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "list_comanagementeligibledevices"
}
-->

```http
GET https://graph.microsoft.com/beta

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
HTTP 1.1 200 Ok

Content-Type: application/json
{
  "value": [
  {
    "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
    "clientRegistrationStatus": "String",
    "deviceName": "String",
    "deviceType": "String",
    "entitySource": "Int32",
    "id": "String(identifier)",
    "managementAgents": "String",
    "managementState": "String",
    "manufacturer": "String",
    "mdmStatus": "String",
    "model": "String",
    "osDescription": "String",
    "osVersion": "String",
    "ownerType": "String",
    "referenceId": "String",
    "serialNumber": "String",
    "status": "String",
    "upn": "String",
    "userEmail": "String",
    "userId": "String",
    "userName": "String"
  }
]
}

```