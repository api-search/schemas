---
description: BalanceMutation schema from Adyen API
layout: schema
name: BalanceMutation
properties_list:
- description: The amount in the payment's currency that is debited or credited on the balance accounting register.
  name: balance
  type: integer
- description: The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes).
  name: currency
  type: string
- description: The amount in the payment's currency that is debited or credited on the received accounting register.
  name: received
  type: integer
- description: The amount in the payment's currency that is debited or credited on the reserved accounting register.
  name: reserved
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounting-notifications-balance-mutation-schema.json
slug: accounting-notifications-balance-mutation
source_filename: accounting-notifications-balance-mutation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-balance-mutation-schema.json\",\n  \"title\": \"BalanceMutation\",\n  \"description\": \"BalanceMutation schema from Adyen API\",\n  \"properties\": {\n    \"balance\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The amount in the payment's currency that is debited or credited on the balance accounting register.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"currency\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"type\": \"string\"\n    },\n    \"received\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The amount in the payment's currency that is debited or credited on the received accounting\
  \ register.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"reserved\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The amount in the payment's currency that is debited or credited on the reserved accounting register.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-balance-mutation-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BalanceMutation
---
