---
description: AuthorisationNotificationRequestItem schema from Adyen API
layout: schema
name: AuthorisationNotificationRequestItem
properties_list:
- description: This object is a generic container that can hold extra fields.
  name: additionalData
  type: object
- description: The payment amount. For HTTP POST notifications, currency and value are returned as URL parameters.
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
- description: The operations indicate the supported follow-up actions concerning the payment. > This is an **experimental field**. Do not base your code on this field. Not all specific cases are covered yet. It's p
  name: operations
  type: array
- description: The payment method used in the transaction.
  name: paymentMethod
  type: string
- description: Adyen's 16-character unique reference associated with the transaction or request. This value is globally unique. Use it when communicating with us about this request.
  name: pspReference
  type: string
- description: 'If `success` = `true` and `paymentMethod` = `visa`, `mc`, or `amex` then this field contains the following details: Authorisation code, last 4 digits of the card, card expiry date. In case of failure,'
  name: reason
  type: string
- description: 'If `true`: The payment request was successful. If `false`: The payment request failed. Check the `reason` field for failure information.'
  name: success
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/webhooks-authorisation-notification-request-item-schema.json
slug: webhooks-authorisation-notification-request-item
source_filename: webhooks-authorisation-notification-request-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-authorisation-notification-request-item-schema.json\",\n  \"title\": \"AuthorisationNotificationRequestItem\",\n  \"description\": \"AuthorisationNotificationRequestItem schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"description\": \"This object is a generic container that can hold extra fields.\",\n      \"$ref\": \"#/components/schemas/AuthorisationNotificationAdditionalData\"\n    },\n    \"amount\": {\n      \"description\": \"The payment amount. For HTTP POST notifications, currency and value are returned as URL parameters.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"eventCode\": {\n      \"description\": \"The type of event the notification item is for.\",\n      \"enum\": [\n        \"AUTHORISATION\"\n      ],\n  \
  \    \"type\": \"string\"\n    },\n    \"eventDate\": {\n      \"description\": \"The time when the event was generated. Format: ISO 8601; yyyy-MM-DDThh:mm:ssTZD\",\n      \"example\": \"2021-07-17T13:42:40+01:00\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"merchantAccountCode\": {\n      \"description\": \"The merchant account identifier used in the transaction the notification item is for.\",\n      \"type\": \"string\"\n    },\n    \"merchantReference\": {\n      \"description\": \"Your reference to uniquely identify the payment.\",\n      \"type\": \"string\"\n    },\n    \"operations\": {\n      \"description\": \"The operations indicate the supported follow-up actions concerning the payment.\\n> This is an **experimental field**. Do not base your code on this field. Not all specific cases are covered yet. It's possible that the field is empty or contains generic information.\",\n      \"items\": {\n        \"enum\": [\n          \"CAPTURE\",\n \
  \         \"CANCEL\",\n          \"REFUND\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"paymentMethod\": {\n      \"description\": \"The payment method used in the transaction.\",\n      \"example\": \"visa, mc, iDeal\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character unique reference associated with the transaction or request. This value is globally unique. Use it when communicating with us about this request.\",\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"description\": \"If `success` = `true` and `paymentMethod` = `visa`, `mc`, or `amex` then this field contains the following details: \\nAuthorisation code, last 4 digits of the card, card expiry date. \\n In case of failure, this contains information about the authorisation failure\",\n      \"example\": \"874574:1935:11/2012\",\n      \"type\": \"string\"\n    },\n    \"success\": {\n      \"description\"\
  : \"If `true`: The payment request was successful. \\n If `false`: The payment request failed. \\n Check the `reason` field for failure information.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"pspReference\",\n    \"merchantReference\",\n    \"merchantAccountCode\",\n    \"eventDate\",\n    \"amount\",\n    \"eventCode\",\n    \"success\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-authorisation-notification-request-item-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AuthorisationNotificationRequestItem
---
