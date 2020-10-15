---
title: "Update assignments"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update assignments

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a deviceHealthScriptAssignment object.

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

In the request body, supply JSON representation of the [deviceHealthScriptAssignment](../resources/intune-devicehealthscriptassignment.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a deviceHealthScriptAssignment object.

| Property             | Type                                                                                             | Description                                                                                                |
| :------------------- | :----------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| id                   | String                                                                                           | Key of the device health script assignment entity. This property is read-only. Read-only.                  |
| runRemediationScript | Boolean                                                                                          | Determine whether we want to run detection script only or run both detection script and remediation script |
| runSchedule          | [deviceHealthScriptRunSchedule](../resources/devicehealthscriptrunschedule.md)                   | Script run schedule for the target group                                                                   |
| target               | [deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md) | The Azure Active Directory group we are targeting the script to                                            |

## Response

If successful, this method returns a `200 OK` response code and a deviceHealthScriptAssignment object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_assignments"
}
-->

```http
PATCH https://graph.microsoft.com/beta

Content-Type: application/json
Content-Length: 504

[
  {
    "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
    "id": "String(identifier)",
    "runRemediationScript": "Boolean",
    "runSchedule": {
      "@odata.type": "#microsoft.graph.deviceHealthScriptHourlySchedule",
      "interval": "Int32"
    },
    "target": {
      "@odata.type": "#microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "String",
      "deviceAndAppManagementAssignmentFilterType": "String"
    }
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
    "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
    "id": "String(identifier)",
    "runRemediationScript": "Boolean",
    "runSchedule": {
      "@odata.type": "#microsoft.graph.deviceHealthScriptHourlySchedule",
      "interval": "Int32"
    },
    "target": {
      "@odata.type": "#microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "String",
      "deviceAndAppManagementAssignmentFilterType": "String"
    }
  }
]
}

```