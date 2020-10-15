---
title: "devicemanagement : getComanagementEligibleDevicesSummary"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# devicemanagement : getComanagementEligibleDevicesSummary

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

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Function Parameters

<!-- Actions and Functions -->

<!-- CRUD Methods -->

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 Ok` response code and a comanagementEligibleDevicesSummary object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "devicemanagement_getcomanagementeligibledevicessummary"
}
-->

```http
GET https://graph.microsoft.com/beta/deviceManagement/getComanagementEligibleDevicesSummary

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.comanagementEligibleDevicesSummary"
}
-->

```http
HTTP 1.1 200 Ok

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.comanagementEligibleDevicesSummary",
  "comanagedCount": "Int32",
  "eligibleButNotAzureAdJoinedCount": "Int32",
  "eligibleCount": "Int32",
  "ineligibleCount": "Int32",
  "needsOsUpdateCount": "Int32"
}
}

```