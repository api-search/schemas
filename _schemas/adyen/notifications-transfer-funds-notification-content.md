---
description: TransferFundsNotificationContent schema from Adyen API
layout: schema
name: TransferFundsNotificationContent
properties_list:
- description: The amount transferred.
  name: amount
  type: object
- description: The code of the Account to which funds were credited.
  name: destinationAccountCode
  type: string
- description: Invalid fields list.
  name: invalidFields
  type: array
- description: The reference provided by the merchant.
  name: merchantReference
  type: string
- description: The code of the Account from which funds were debited.
  name: sourceAccountCode
  type: string
- description: The status of the fund transfer.
  name: status
  type: object
- description: The transfer code.
  name: transferCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-transfer-funds-notification-content-schema.json
slug: notifications-transfer-funds-notification-content
source_filename: notifications-transfer-funds-notification-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-transfer-funds-notification-content-schema.json\",\n  \"title\": \"TransferFundsNotificationContent\",\n  \"description\": \"TransferFundsNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount transferred.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"destinationAccountCode\": {\n      \"description\": \"The code of the Account to which funds were credited.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Invalid fields list.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantReference\": {\n      \"x-addedInVersion\": \"\
  2\",\n      \"description\": \"The reference provided by the merchant.\",\n      \"type\": \"string\"\n    },\n    \"sourceAccountCode\": {\n      \"description\": \"The code of the Account from which funds were debited.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the fund transfer.\",\n      \"$ref\": \"#/components/schemas/OperationStatus\"\n    },\n    \"transferCode\": {\n      \"description\": \"The transfer code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-transfer-funds-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferFundsNotificationContent
---
