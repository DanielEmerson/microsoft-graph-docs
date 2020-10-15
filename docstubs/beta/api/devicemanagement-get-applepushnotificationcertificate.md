---
title: "Get applePushNotificationCertificate"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Get applePushNotificationCertificate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an applePushNotificationCertificate object.

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

If successful, this method returns a `200 OK` response code and an applePushNotificationCertificate object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "get_applepushnotificationcertificate"
}
-->

```http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.applePushNotificationCertificate"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "String",
  "certificate": "String",
  "certificateSerialNumber": "String",
  "certificateUploadFailureReason": "String",
  "certificateUploadStatus": "String",
  "expirationDateTime": "DateTimeOffset",
  "id": "String(identifier)",
  "lastModifiedDateTime": "DateTimeOffset",
  "topicIdentifier": "String"
}
}

```