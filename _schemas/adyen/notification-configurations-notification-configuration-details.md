---
description: NotificationConfigurationDetails schema from Adyen API
layout: schema
name: NotificationConfigurationDetails
properties_list:
- description: Indicates whether the notification subscription is active.
  name: active
  type: boolean
- description: The version of the notification to which you are subscribing. To make sure that your integration can properly process the notification, subscribe to the same version as the API that you're using.
  name: apiVersion
  type: integer
- description: A description of the notification subscription configuration.
  name: description
  type: string
- description: Contains objects that define event types and their subscription settings.
  name: eventConfigs
  type: array
- description: A string with which to salt the notification(s) before hashing. If this field is provided, a hash value will be included under the notification header `HmacSignature` and the hash protocol will be inc
  name: hmacSignatureKey
  type: string
- description: Adyen-generated ID for the entry, returned in the response when you create a notification configuration. Required when updating an existing configuration using [`/updateNotificationConfiguration`](htt
  name: notificationId
  type: integer
- description: The password to use when accessing the notifyURL with the specified username.
  name: notifyPassword
  type: string
- description: The URL to which the notifications are to be sent.
  name: notifyURL
  type: string
- description: The username to use when accessing the notifyURL.
  name: notifyUsername
  type: string
- description: 'The SSL protocol employed by the endpoint. >Permitted values: `TLSv12`, `TLSv13`.'
  name: sslProtocol
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-configurations-notification-configuration-details-schema.json
slug: notification-configurations-notification-configuration-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-notification-configuration-details-schema.json\",\n  \"title\": \"NotificationConfigurationDetails\",\n  \"description\": \"NotificationConfigurationDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"active\": {\n      \"description\": \"Indicates whether the notification subscription is active.\",\n      \"type\": \"boolean\"\n    },\n    \"apiVersion\": {\n      \"description\": \"The version of the notification to which you are subscribing. To make sure that your integration can properly process the notification, subscribe to the same version as the API that you're using.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"description\": {\n      \"description\": \"A description of the notification subscription configuration.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"eventConfigs\": {\n      \"description\": \"Contains objects that define event types and their subscription settings.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/NotificationEventConfiguration\"\n      },\n      \"type\": \"array\"\n    },\n    \"hmacSignatureKey\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"A string with which to salt the notification(s) before hashing. If this field is provided, a hash value will be included under the notification header `HmacSignature` and the hash protocol will be included under the notification header `Protocol`. A notification body along with its `hmacSignatureKey` and `Protocol` can be used to calculate a hash value; matching this hash value with the `HmacSignature` will ensure that the notification body has not been tampered with or corrupted.\\n\\n>Must be a 32-byte hex-encoded string (i.e. a string containing 64 hexadecimal characters; e.g. \\\"b0ea55c2fe60d4d1d605e9c385e0e7f7e6cafbb939ce07010f31a327a0871f27\\\
  \").\\n\\nThe omission of this field will preclude the provision of the `HmacSignature` and `Protocol` headers in notification(s).\",\n      \"type\": \"string\"\n    },\n    \"notificationId\": {\n      \"description\": \"Adyen-generated ID for the entry, returned in the response when you create a notification configuration. Required when updating an existing configuration using [`/updateNotificationConfiguration`](https://docs.adyen.com/api-explorer/#/NotificationConfigurationService/latest/post/updateNotificationConfiguration).\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"notifyPassword\": {\n      \"description\": \"The password to use when accessing the notifyURL with the specified username.\",\n      \"type\": \"string\"\n    },\n    \"notifyURL\": {\n      \"description\": \"The URL to which the notifications are to be sent.\",\n      \"type\": \"string\"\n    },\n    \"notifyUsername\": {\n      \"description\": \"The username to use when accessing\
  \ the notifyURL.\",\n      \"type\": \"string\"\n    },\n    \"sslProtocol\": {\n      \"description\": \"The SSL protocol employed by the endpoint.\\n>Permitted values: `TLSv12`, `TLSv13`.\",\n      \"enum\": [\n        \"TLSv12\",\n        \"TLSv13\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-notification-configuration-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NotificationConfigurationDetails
---
