---
description: ScheduleAccountUpdaterRequest schema from Adyen API
layout: schema
name: ScheduleAccountUpdaterRequest
properties_list:
- description: This field contains additional data, which may be required for a particular request.
  name: additionalData
  type: object
- description: Credit card data. Optional if `shopperReference` and `selectedRecurringDetailReference` are provided.
  name: card
  type: object
- description: Account of the merchant.
  name: merchantAccount
  type: string
- description: A reference that merchants can apply for the call.
  name: reference
  type: string
- description: The selected detail recurring reference. Optional if `card` is provided.
  name: selectedRecurringDetailReference
  type: string
- description: The reference of the shopper that owns the recurring contract. Optional if `card` is provided.
  name: shopperReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-schedule-account-updater-request-schema.json
slug: recurring-schedule-account-updater-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-schedule-account-updater-request-schema.json\",\n  \"title\": \"ScheduleAccountUpdaterRequest\",\n  \"description\": \"ScheduleAccountUpdaterRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"This field contains additional data, which may be required for a particular request.\",\n      \"type\": \"object\"\n    },\n    \"card\": {\n      \"description\": \"Credit card data.\\n\\nOptional if `shopperReference` and `selectedRecurringDetailReference` are provided.\",\n      \"$ref\": \"#/components/schemas/Card\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"Account of the merchant.\",\n      \"type\": \"string\"\n    },\n    \"reference\"\
  : {\n      \"description\": \"A reference that merchants can apply for the call.\",\n      \"type\": \"string\"\n    },\n    \"selectedRecurringDetailReference\": {\n      \"description\": \"The selected detail recurring reference.\\n\\nOptional if `card` is provided.\",\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"The reference of the shopper that owns the recurring contract.\\n\\nOptional if `card` is provided.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"reference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-schedule-account-updater-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ScheduleAccountUpdaterRequest
---
