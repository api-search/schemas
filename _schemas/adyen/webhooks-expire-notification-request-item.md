---
description: ExpireNotificationRequestItem schema from Adyen API
layout: schema
name: ExpireNotificationRequestItem
properties_list:
- description: A generic container for extra fields.
  name: additionalData
  type: object
- description: The amount that was originally authorised.
  name: amount
  type: object
- description: The type of event the notification item is for.
  name: eventCode
  type: string
- description: 'The time when the event was generated. Format: ISO 8601; yyyy-MM-DDThh:mm:ssTZD'
  name: eventDate
  type: string
- description: The merchant account identifier used in the transaction the notification item is for.
  name: merchantAccountCode
  type: string
- description: Your reference to uniquely identify the payment.
  name: merchantReference
  type: string
- description: For modifications, this field corresponds to the payment request assigned to the original payment.
  name: originalReference
  type: string
- description: The payment method used in the transaction.
  name: paymentMethod
  type: string
- description: Adyen's 16-character unique reference associated with the transaction or request. This value is globally unique. Use it when communicating with us about this request.
  name: pspReference
  type: string
- description: If `success` = `false`, then this includes a short message with an explanation for the refusal.
  name: reason
  type: string
- description: Always `true`.
  name: success
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/webhooks-expire-notification-request-item-schema.json
slug: webhooks-expire-notification-request-item
source_filename: webhooks-expire-notification-request-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-expire-notification-request-item-schema.json\",\n  \"title\": \"ExpireNotificationRequestItem\",\n  \"description\": \"ExpireNotificationRequestItem schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"description\": \"A generic container for extra fields.\",\n      \"$ref\": \"#/components/schemas/NotificationAdditionalData\"\n    },\n    \"amount\": {\n      \"description\": \"The amount that was originally authorised.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"eventCode\": {\n      \"description\": \"The type of event the notification item is for.\",\n      \"enum\": [\n        \"EXPIRE\"\n      ],\n      \"type\": \"string\"\n    },\n    \"eventDate\": {\n      \"description\": \"The time when the event was generated. Format:\
  \ ISO 8601; yyyy-MM-DDThh:mm:ssTZD\",\n      \"example\": \"2021-07-17T13:42:40+01:00\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"merchantAccountCode\": {\n      \"description\": \"The merchant account identifier used in the transaction the notification item is for.\",\n      \"type\": \"string\"\n    },\n    \"merchantReference\": {\n      \"description\": \"Your reference to uniquely identify the payment.\",\n      \"type\": \"string\"\n    },\n    \"originalReference\": {\n      \"description\": \"For modifications, this field corresponds to the payment request assigned to the original payment.\",\n      \"type\": \"string\"\n    },\n    \"paymentMethod\": {\n      \"description\": \"The payment method used in the transaction.\",\n      \"example\": \"visa, mc, iDeal\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character unique reference associated with the transaction or request. This value\
  \ is globally unique. Use it when communicating with us about this request.\",\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"description\": \"If `success` = `false`, then this includes a short message with an explanation for the refusal.\",\n      \"type\": \"string\"\n    },\n    \"success\": {\n      \"description\": \"Always `true`.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"pspReference\",\n    \"merchantReference\",\n    \"merchantAccountCode\",\n    \"eventDate\",\n    \"eventCode\",\n    \"amount\",\n    \"success\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-expire-notification-request-item-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ExpireNotificationRequestItem
---
