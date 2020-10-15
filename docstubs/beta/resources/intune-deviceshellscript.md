---
title: "deviceShellScript resource type"
description: "Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices. The script can be run once or periodically."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceShellScript resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices. The script can be run once or periodically.

## Methods

| Method                                                                                | Return Type                                                                                           | Description                                                                                         |
| :------------------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------- |
| [List deviceShellScript](../api/intune-deviceshellscript-list.md)                     | [deviceShellScript](intune-deviceShellScript.md) collection                                           | List properties and relationships of a deviceShellScript object.                                    |
| [Create deviceShellScript](../api/intune-deviceshellscript-create.md)                 | [deviceShellScript](intune-deviceShellScript.md)                                                      | Create a new deviceShellScript object.                                                              |
| [Get deviceShellScript](../api/intune-deviceshellscript-get.md)                       | [deviceShellScript](intune-deviceShellScript.md)                                                      | Read properties and relationships of a deviceShellScript object.                                    |
| [Update deviceShellScript](../api/intune-deviceshellscript-update.md)                 | [deviceShellScript](intune-deviceShellScript.md)                                                      | Update the properties of a deviceShellScript object.                                                |
| [Delete deviceShellScript](../api/intune-deviceshellscript-delete.md)                 |                                                                                                       | Delete a deviceShellScript object.                                                                  |
| [assign](../api/intune-deviceshellscript-assign.md)                                   |                                                                                                       |                                                                                                     |
| [List assignments](../api/intune-deviceshellscript-list-assignments.md)               | [deviceManagementScriptAssignment](../resources/intune-devicemanagementscriptassignment.md)           | Get the deviceManagementScriptAssignment objects from an assignments navigation property.           |
| [Create assignments](../api/intune-deviceshellscript-post-assignments.md)             | [deviceManagementScriptAssignment](../resources/intune-devicemanagementscriptassignment.md)           | Create a new deviceManagementScriptAssignment object.                                               |
| [Get assignments](../api/intune-deviceshellscript-get-assignments.md)                 | [deviceManagementScriptAssignment](../resources/intune-devicemanagementscriptassignment.md)           | Read the properties and relationships of a deviceManagementScriptAssignment object.                 |
| [Update assignments](../api/intune-deviceshellscript-update-assignments.md)           | [deviceManagementScriptAssignment](../resources/intune-devicemanagementscriptassignment.md)           | Update the properties of a deviceManagementScriptAssignment object.                                 |
| [Delete assignments](../api/intune-deviceshellscript-delete-assignments.md)           |                                                                                                       | Delete a deviceManagementScriptAssignment object.                                                   |
| [List deviceRunStates](../api/intune-deviceshellscript-list-devicerunstates.md)       | [deviceManagementScriptDeviceState](../resources/intune-devicemanagementscriptdevicestate.md)         | Get the deviceManagementScriptDeviceState objects from a deviceRunStates navigation property.       |
| [Create deviceRunStates](../api/intune-deviceshellscript-post-devicerunstates.md)     | [deviceManagementScriptDeviceState](../resources/intune-devicemanagementscriptdevicestate.md)         | Create a new deviceManagementScriptDeviceState object.                                              |
| [Get deviceRunStates](../api/intune-deviceshellscript-get-devicerunstates.md)         | [deviceManagementScriptDeviceState](../resources/intune-devicemanagementscriptdevicestate.md)         | Read the properties and relationships of a deviceManagementScriptDeviceState object.                |
| [Update deviceRunStates](../api/intune-deviceshellscript-update-devicerunstates.md)   | [deviceManagementScriptDeviceState](../resources/intune-devicemanagementscriptdevicestate.md)         | Update the properties of a deviceManagementScriptDeviceState object.                                |
| [Delete deviceRunStates](../api/intune-deviceshellscript-delete-devicerunstates.md)   |                                                                                                       | Delete a deviceManagementScriptDeviceState object.                                                  |
| [List groupAssignments](../api/intune-deviceshellscript-list-groupassignments.md)     | [deviceManagementScriptGroupAssignment](../resources/intune-devicemanagementscriptgroupassignment.md) | Get the deviceManagementScriptGroupAssignment objects from a groupAssignments navigation property.  |
| [Create groupAssignments](../api/intune-deviceshellscript-post-groupassignments.md)   | [deviceManagementScriptGroupAssignment](../resources/intune-devicemanagementscriptgroupassignment.md) | Create a new deviceManagementScriptGroupAssignment object.                                          |
| [Get groupAssignments](../api/intune-deviceshellscript-get-groupassignments.md)       | [deviceManagementScriptGroupAssignment](../resources/intune-devicemanagementscriptgroupassignment.md) | Read the properties and relationships of a deviceManagementScriptGroupAssignment object.            |
| [Update groupAssignments](../api/intune-deviceshellscript-update-groupassignments.md) | [deviceManagementScriptGroupAssignment](../resources/intune-devicemanagementscriptgroupassignment.md) | Update the properties of a deviceManagementScriptGroupAssignment object.                            |
| [Delete groupAssignments](../api/intune-deviceshellscript-delete-groupassignments.md) |                                                                                                       | Delete a deviceManagementScriptGroupAssignment object.                                              |
| [List runSummary](../api/intune-deviceshellscript-list-runsummary.md)                 | [deviceManagementScriptRunSummary](../resources/intune-devicemanagementscriptrunsummary.md)           | Get the deviceManagementScriptRunSummary objects from a runSummary navigation property.             |
| [Add runSummary](../api/intune-deviceshellscript-post-runsummary.md)                  | [deviceManagementScriptRunSummary](../resources/intune-devicemanagementscriptrunsummary.md)           | Add deviceManagementScriptRunSummary by posting to the deviceManagementScriptRunSummary collection. |
| [Get runSummary](../api/intune-deviceshellscript-get-runsummary.md)                   | [deviceManagementScriptRunSummary](../resources/intune-devicemanagementscriptrunsummary.md)           | Read the properties and relationships of a deviceManagementScriptRunSummary object.                 |
| [Update runSummary](../api/intune-deviceshellscript-update-runsummary.md)             | [deviceManagementScriptRunSummary](../resources/intune-devicemanagementscriptrunsummary.md)           | Update the properties of a deviceManagementScriptRunSummary object.                                 |
| [Remove runSummary](../api/intune-deviceshellscript-delete-runsummary.md)             |                                                                                                       | Remove a deviceManagementScriptRunSummary object.                                                   |
| [List userRunStates](../api/intune-deviceshellscript-list-userrunstates.md)           | [deviceManagementScriptUserState](../resources/intune-devicemanagementscriptuserstate.md)             | Get the deviceManagementScriptUserState objects from an userRunStates navigation property.          |
| [Create userRunStates](../api/intune-deviceshellscript-post-userrunstates.md)         | [deviceManagementScriptUserState](../resources/intune-devicemanagementscriptuserstate.md)             | Create a new deviceManagementScriptUserState object.                                                |
| [Get userRunStates](../api/intune-deviceshellscript-get-userrunstates.md)             | [deviceManagementScriptUserState](../resources/intune-devicemanagementscriptuserstate.md)             | Read the properties and relationships of a deviceManagementScriptUserState object.                  |
| [Update userRunStates](../api/intune-deviceshellscript-update-userrunstates.md)       | [deviceManagementScriptUserState](../resources/intune-devicemanagementscriptuserstate.md)             | Update the properties of a deviceManagementScriptUserState object.                                  |
| [Delete userRunStates](../api/intune-deviceshellscript-delete-userrunstates.md)       |                                                                                                       | Delete a deviceManagementScriptUserState object.                                                    |

## Properties

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

## Relationships

| Relationship     | Type                                                                                                      | Description                                                     |
| :--------------- | :-------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------- |
| assignments      | [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) collection           | The list of group assignments for the device management script. |
| deviceRunStates  | [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection         | List of run states for this script across all devices.          |
| groupAssignments | [deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md) collection | The list of group assignments for the device management script. |
| runSummary       | [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md)                      | Run summary for device management script.                       |
| userRunStates    | [deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) collection             | List of run states for this script across all users.            |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceShellScript",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "blockExecutionNotifications": "Boolean",
  "createdDateTime": "DateTimeOffset",
  "description": "String",
  "displayName": "String",
  "executionFrequency": "Duration",
  "fileName": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "DateTimeOffset",
  "retryCount": "Int32",
  "roleScopeTagIds": ["String"],
  "runAsAccount": "system | user",
  "scriptContent": "Binary"
}
```