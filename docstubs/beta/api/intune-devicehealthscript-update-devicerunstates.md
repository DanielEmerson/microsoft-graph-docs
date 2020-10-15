---
title: "Update deviceRunStates"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update deviceRunStates

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a deviceHealthScriptDeviceState object.

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

In the request body, supply JSON representation of the [deviceHealthScriptDeviceState](../resources/intune-devicehealthscriptdevicestate.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a deviceHealthScriptDeviceState object.

| Property                             | Type           | Description                                                                                 |
| :----------------------------------- | :------------- | :------------------------------------------------------------------------------------------ |
| detectionState                       | String         | Detection state from the lastest device health script execution                             |
| expectedStateUpdateDateTime          | DateTimeOffset | The next timestamp of when the device health script is expected to execute                  |
| id                                   | String         | Key of the device health script device state entity. This property is read-only. Read-only. |
| lastStateUpdateDateTime              | DateTimeOffset | The last timestamp of when the device health script executed                                |
| lastSyncDateTime                     | DateTimeOffset | The last time that Intune Managment Extension synced with Intune                            |
| postRemediationDetectionScriptError  | String         | Error from the detection script after remediation                                           |
| postRemediationDetectionScriptOutput | String         | Detection script output after remediation                                                   |
| preRemediationDetectionScriptError   | String         | Error from the detection script before remediation                                          |
| preRemediationDetectionScriptOutput  | String         | Output of the detection script before remediation                                           |
| remediationScriptError               | String         | Error output of the remediation script                                                      |
| remediationState                     | String         | Remediation state from the lastest device health script execution                           |

## Response

If successful, this method returns a `200 OK` response code and a deviceHealthScriptDeviceState object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_devicerunstates"
}
-->

```http
PATCH https://graph.microsoft.com/beta

Content-Type: application/json
Content-Length: 588

[
  {
    "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
    "detectionState": "String",
    "expectedStateUpdateDateTime": "DateTimeOffset",
    "id": "String(identifier)",
    "lastStateUpdateDateTime": "DateTimeOffset",
    "lastSyncDateTime": "DateTimeOffset",
    "postRemediationDetectionScriptError": "String",
    "postRemediationDetectionScriptOutput": "String",
    "preRemediationDetectionScriptError": "String",
    "preRemediationDetectionScriptOutput": "String",
    "remediationScriptError": "String",
    "remediationState": "String"
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
    "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
    "detectionState": "String",
    "expectedStateUpdateDateTime": "DateTimeOffset",
    "id": "String(identifier)",
    "lastStateUpdateDateTime": "DateTimeOffset",
    "lastSyncDateTime": "DateTimeOffset",
    "postRemediationDetectionScriptError": "String",
    "postRemediationDetectionScriptOutput": "String",
    "preRemediationDetectionScriptError": "String",
    "preRemediationDetectionScriptOutput": "String",
    "remediationScriptError": "String",
    "remediationState": "String"
  }
]
}

```