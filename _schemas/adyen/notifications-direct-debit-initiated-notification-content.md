---
description: DirectDebitInitiatedNotificationContent schema from Adyen API
layout: schema
name: DirectDebitInitiatedNotificationContent
properties_list:
- description: The code of the account.
  name: accountCode
  type: string
- description: The amount to be debited from the funding account.
  name: amount
  type: object
- description: The date of the debit initiation.
  name: debitInitiationDate
  type: object
- description: Invalid fields list.
  name: invalidFields
  type: array
- description: The code of the merchant account.
  name: merchantAccountCode
  type: string
- description: The split data for the debit request.
  name: splits
  type: array
- description: Direct debit status.
  name: status
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-direct-debit-initiated-notification-content-schema.json
slug: notifications-direct-debit-initiated-notification-content
source_filename: notifications-direct-debit-initiated-notification-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-direct-debit-initiated-notification-content-schema.json\",\n  \"title\": \"DirectDebitInitiatedNotificationContent\",\n  \"description\": \"DirectDebitInitiatedNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account.\",\n      \"type\": \"string\"\n    },\n    \"amount\": {\n      \"description\": \"The amount to be debited from the funding account.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"debitInitiationDate\": {\n      \"description\": \"The date of the debit initiation.\",\n      \"$ref\": \"#/components/schemas/LocalDate\"\n    },\n    \"invalidFields\": {\n      \"description\": \"Invalid fields list.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\
  \n      },\n      \"type\": \"array\"\n    },\n    \"merchantAccountCode\": {\n      \"description\": \"The code of the merchant account.\",\n      \"type\": \"string\"\n    },\n    \"splits\": {\n      \"description\": \"The split data for the debit request.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Split\"\n      },\n      \"type\": \"array\"\n    },\n    \"status\": {\n      \"description\": \"Direct debit status.\",\n      \"$ref\": \"#/components/schemas/OperationStatus\"\n    }\n  },\n  \"required\": [\n    \"amount\",\n    \"accountCode\",\n    \"merchantAccountCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-direct-debit-initiated-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DirectDebitInitiatedNotificationContent
---
