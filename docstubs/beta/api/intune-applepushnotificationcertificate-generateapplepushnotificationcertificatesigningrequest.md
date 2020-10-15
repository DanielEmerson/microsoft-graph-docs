---
title: "applepushnotificationcertificate : generateApplePushNotificationCertificateSigningRequest"
description: "Download Apple push notification certificate signing request"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# applepushnotificationcertificate : generateApplePushNotificationCertificateSigningRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Download Apple push notification certificate signing request

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

<!-- Actions and Functions -->

<!-- CRUD Methods -->

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 Ok` response code and a String object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "applepushnotificationcertificate_generateapplepushnotificationcertificatesigningrequest"
}
-->

```http
POST https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate/generateApplePushNotificationCertificateSigningRequest

Content-Type: application/json
Content-Length: 8

"String"

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.String"
}
-->

```http
HTTP 1.1 200 Ok

Content-Type: application/json
{
  "value": "String"
}

```