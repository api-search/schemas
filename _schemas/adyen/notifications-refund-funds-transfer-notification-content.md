---
description: RefundFundsTransferNotificationContent schema from Adyen API
layout: schema
name: RefundFundsTransferNotificationContent
properties_list:
- description: The amount to be refunded.
  name: amount
  type: object
- description: Invalid fields list.
  name: invalidFields
  type: array
- description: A value that can be supplied at the discretion of the executing user in order to link multiple transactions to one another.
  name: merchantReference
  type: string
- description: A PSP reference of the original fund transfer.
  name: originalReference
  type: string
- description: The status of the fund transfer refund.
  name: status
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-refund-funds-transfer-notification-content-schema.json
slug: notifications-refund-funds-transfer-notification-content
source_filename: notifications-refund-funds-transfer-notification-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-refund-funds-transfer-notification-content-schema.json\",\n  \"title\": \"RefundFundsTransferNotificationContent\",\n  \"description\": \"RefundFundsTransferNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount to be refunded.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Invalid fields list.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantReference\": {\n      \"description\": \"A value that can be supplied at the discretion of the executing user in order to link multiple transactions to one another.\",\n      \"\
  type\": \"string\"\n    },\n    \"originalReference\": {\n      \"description\": \"A PSP reference of the original fund transfer.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the fund transfer refund.\",\n      \"$ref\": \"#/components/schemas/OperationStatus\"\n    }\n  },\n  \"required\": [\n    \"originalReference\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-refund-funds-transfer-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RefundFundsTransferNotificationContent
---
