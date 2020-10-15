---
title: "List managedDeviceOverview"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# List managedDeviceOverview

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the managedDeviceOverview objects and their properties.

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

If successful, this method returns a `200 Ok` response code and a managedDeviceOverview object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "list_manageddeviceoverview"
}
-->

```http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.managedDeviceOverview"
}
-->

```http
HTTP 1.1 200 Ok

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": "Int32",
    "blockedDeviceCount": "Int32",
    "quarantinedDeviceCount": "Int32",
    "unavailableDeviceCount": "Int32",
    "unknownDeviceCount": "Int32"
  },
  "deviceOperatingSystemSummary": {
    "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
    "androidCorporateWorkProfileCount": "Int32",
    "androidCount": "Int32",
    "androidDedicatedCount": "Int32",
    "androidDeviceAdminCount": "Int32",
    "androidFullyManagedCount": "Int32",
    "androidWorkProfileCount": "Int32",
    "aospUserlessCount": "Int32",
    "configMgrDeviceCount": "Int32",
    "iosCount": "Int32",
    "macOSCount": "Int32",
    "unknownCount": "Int32",
    "windowsCount": "Int32",
    "windowsMobileCount": "Int32"
  },
  "dualEnrolledDeviceCount": "Int32",
  "enrolledDeviceCount": "Int32",
  "id": "String(identifier)",
  "lastModifiedDateTime": "DateTimeOffset",
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceManufacturers": [
      "String"
    ],
    "deviceModels": [
      "String"
    ]
  },
  "mdmEnrolledCount": "Int32"
}
}

```