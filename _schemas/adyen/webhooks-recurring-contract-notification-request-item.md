---
description: RecurringContractNotificationRequestItem schema from Adyen API
layout: schema
name: RecurringContractNotificationRequestItem
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
- description: The `pspReference` of the initial payment.
  name: originalPsp
  type: string
- description: For modifications, this field corresponds to the payment request assigned to the original payment.
  name: originalReference
  type: string
- description: The payment method used in the transaction.
  name: paymentMethod
  type: string
- description: The [token for stored payment details](https://docs.adyen.com/online-payments/tokenization/create-and-use-tokens/) to make recurring payments. This is the same as the `recurringDetailReference`.
  name: pspReference
  type: string
- description: If `success` = `false`, then this includes a short message with an explanation for the refusal.
  name: reason
  type: string
- description: 'Informs about the outcome of the event (`eventCode`) the notification is for. If `true`: the event was executed successfully. If `false`: the event was not executed successfully.'
  name: success
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/webhooks-recurring-contract-notification-request-item-schema.json
slug: webhooks-recurring-contract-notification-request-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-recurring-contract-notification-request-item-schema.json\",\n  \"title\": \"RecurringContractNotificationRequestItem\",\n  \"description\": \"RecurringContractNotificationRequestItem schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"description\": \"This object is a generic container that can hold extra fields.\",\n      \"$ref\": \"#/components/schemas/RecurringContractNotificationAdditionalData\"\n    },\n    \"amount\": {\n      \"description\": \"The payment amount. For HTTP POST notifications, currency and value are returned as URL parameters.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"eventCode\": {\n      \"description\": \"The type of event the notification item is for.\",\n      \"enum\": [\n        \"RECURRING_CONTRACT\"\
  \n      ],\n      \"type\": \"string\"\n    },\n    \"eventDate\": {\n      \"description\": \"The time when the event was generated. Format: ISO 8601; yyyy-MM-DDThh:mm:ssTZD\",\n      \"example\": \"2021-07-17T13:42:40+01:00\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"merchantAccountCode\": {\n      \"description\": \"The merchant account identifier used in the transaction the notification item is for.\",\n      \"type\": \"string\"\n    },\n    \"merchantReference\": {\n      \"description\": \"Your reference to uniquely identify the payment.\",\n      \"type\": \"string\"\n    },\n    \"originalPsp\": {\n      \"description\": \"The `pspReference` of the initial payment.\",\n      \"type\": \"string\"\n    },\n    \"originalReference\": {\n      \"description\": \"For modifications, this field corresponds to the payment request assigned to the original payment.\",\n      \"type\": \"string\"\n    },\n    \"paymentMethod\": {\n      \"description\"\
  : \"The payment method used in the transaction.\",\n      \"example\": \"visa, mc, iDeal\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The [token for stored payment details](https://docs.adyen.com/online-payments/tokenization/create-and-use-tokens/) to make recurring payments. This is the same as the `recurringDetailReference`.\",\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"description\": \"If `success` = `false`, then this includes a short message with an explanation for the refusal.\",\n      \"type\": \"string\"\n    },\n    \"success\": {\n      \"description\": \"Informs about the outcome of the event (`eventCode`) the notification is for. \\nIf `true`: the event was executed successfully. \\nIf `false`: the event was not executed successfully.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantReference\",\n    \"merchantAccountCode\",\n    \"eventDate\",\n    \"amount\",\n    \"success\",\n\
  \    \"eventCode\",\n    \"originalPsp\",\n    \"pspReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-recurring-contract-notification-request-item-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RecurringContractNotificationRequestItem
---
