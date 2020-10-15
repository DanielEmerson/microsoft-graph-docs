---
title: "Update applePushNotificationCertificate"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update applePushNotificationCertificate

Namespace: microsoft.graph

Update the properties of an applePushNotificationCertificate object.

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

In the request body, supply JSON representation of the [applePushNotificationCertificate](../resources/intune-applepushnotificationcertificate.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create an applePushNotificationCertificate object.

| Property             | Type           | Description                                                           |
| :------------------- | :------------- | :-------------------------------------------------------------------- |
| appleIdentifier      | String         | Apple Id of the account used to create the MDM push certificate.      |
| certificate          | String         |                                                                       |
| expirationDateTime   | DateTimeOffset | The expiration date and time for Apple push notification certificate. |
| id                   | String         | Unique Identifier for the certificate Read-only.                      |
| lastModifiedDateTime | DateTimeOffset | Last modified date and time for Apple push notification certificate.  |
| topicIdentifier      | String         | Topic Id.                                                             |

## Response

If successful, this method returns a `200 OK` response code and an applePushNotificationCertificate object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_applepushnotificationcertificate"
}
-->

```http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate

Content-Type: application/json
Content-Length: 254

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "String",
  "certificate": "String",
  "expirationDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset",
  "topicIdentifier": "String"
}

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
  "expirationDateTime": "DateTimeOffset",
  "id": "String(identifier)",
  "lastModifiedDateTime": "DateTimeOffset",
  "topicIdentifier": "String"
}
}

```