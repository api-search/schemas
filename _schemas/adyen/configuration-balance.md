---
description: Balance schema from Adyen API
layout: schema
name: Balance
properties_list:
- description: The remaining amount available for spending.
  name: available
  type: integer
- description: The total amount in the balance.
  name: balance
  type: integer
- description: The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes) of the balance.
  name: currency
  type: string
- description: The amount pending to be paid out but not yet available in the balance.
  name: pending
  type: integer
- description: The amount reserved for payments that have been authorised, but have not been captured yet.
  name: reserved
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-balance-schema.json
slug: configuration-balance
source_filename: configuration-balance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-balance-schema.json\",\n  \"title\": \"Balance\",\n  \"description\": \"Balance schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"available\": {\n      \"description\": \"The remaining amount available for spending.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"balance\": {\n      \"description\": \"The total amount in the balance.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"currency\": {\n      \"description\": \"The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes) of the balance.\",\n      \"type\": \"string\"\n    },\n    \"pending\": {\n      \"description\": \"The amount pending to be paid out but not yet available in the balance.\",\n      \"format\": \"\
  int64\",\n      \"type\": \"integer\"\n    },\n    \"reserved\": {\n      \"description\": \"The amount reserved for payments that have been authorised, but have not been captured yet.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"currency\",\n    \"balance\",\n    \"reserved\",\n    \"available\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-balance-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Balance
---
