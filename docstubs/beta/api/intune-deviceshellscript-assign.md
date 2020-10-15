---
title: "deviceshellscript : assign"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# deviceshellscript : assign

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

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request Body

In the request body, supply JSON representation of the parameters.

<!-- Actions and Functions -->

The following table shows the parameters that can be used with this method.

| Parameter                              | Type                                                                                                      | Description |
| :------------------------------------- | :-------------------------------------------------------------------------------------------------------- | :---------- |
| deviceManagementScriptGroupAssignments | [deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md) collection |             |
| deviceManagementScriptAssignments      | [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) collection           |             |

<!-- CRUD Methods -->

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "deviceshellscript_assign"
}
-->

```http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{id}/assign

```

### Response

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "$(this.ReturnTypeFullName)"
}
-->

```http
HTTP 1.1 204 No Content

```