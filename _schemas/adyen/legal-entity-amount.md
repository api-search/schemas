---
description: Amount schema from Adyen API
layout: schema
name: Amount
properties_list:
- description: The type of currency. Must be EUR (or EUR equivalent)
  name: currency
  type: string
- description: Total value of amount. Must be >= 0
  name: value
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-amount-schema.json
slug: legal-entity-amount
source_filename: legal-entity-amount-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-amount-schema.json\",\n  \"title\": \"Amount\",\n  \"description\": \"Amount schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"description\": \"The type of currency. Must be EUR (or EUR equivalent)\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Total value of amount. Must be >= 0\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-amount-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Amount
---
