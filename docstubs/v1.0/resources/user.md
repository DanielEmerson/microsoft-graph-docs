---
title: "user resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# user resource type

Namespace: microsoft.graph

## Methods

| Method                                                                          | Return Type                                           | Description                                                              |
| :------------------------------------------------------------------------------ | :---------------------------------------------------- | :----------------------------------------------------------------------- |
| [List user](../api/user-list.md)                                                | [user](user.md) collection                            | List properties and relationships of a user object.                      |
| [Create user](../api/user-create.md)                                            | [user](user.md)                                       | Create a new user object.                                                |
| [Get user](../api/user-get.md)                                                  | [user](user.md)                                       | Read properties and relationships of a user object.                      |
| [Update user](../api/user-update.md)                                            | [user](user.md)                                       | Update the properties of a user object.                                  |
| [Delete user](../api/user-delete.md)                                            |                                                       | Delete a user object.                                                    |
| [removeAllDevicesFromManagement](../api/user-removeAllDevicesFromManagement.md) |                                                       | Retire all devices from management for this user                         |
| [List managedDevices](../api/user-list-manageddevices.md)                       | [managedDevice](../resources/intune-manageddevice.md) | Get the managedDevice objects from a managedDevices navigation property. |
| [Create managedDevices](../api/user-post-manageddevices.md)                     | [managedDevice](../resources/intune-manageddevice.md) | Create a new managedDevice object.                                       |
| [Get managedDevices](../api/user-get-manageddevices.md)                         | [managedDevice](../resources/intune-manageddevice.md) | Read the properties and relationships of a managedDevice object.         |
| [Update managedDevices](../api/user-update-manageddevices.md)                   | [managedDevice](../resources/intune-manageddevice.md) | Update the properties of a managedDevice object.                         |
| [Delete managedDevices](../api/user-delete-manageddevices.md)                   |                                                       | Delete a managedDevice object.                                           |

## Properties

| Property | Type   | Description                               |
| :------- | :----- | :---------------------------------------- |
| id       | String | Unique identifier of the user. Read-only. |

## Relationships

| Relationship   | Type                                                      | Description                                   |
| :------------- | :-------------------------------------------------------- | :-------------------------------------------- |
| managedDevices | [managedDevice](../resources/manageddevice.md) collection | The managed devices associated with the user. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```