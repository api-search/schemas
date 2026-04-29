---
description: TotalAmountRestriction schema from Adyen API
layout: schema
name: TotalAmountRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: The amount value and currency.
  name: value
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-total-amount-restriction-schema.json
slug: configuration-total-amount-restriction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-total-amount-restriction-schema.json\",\n  \"title\": \"TotalAmountRestriction\",\n  \"description\": \"TotalAmountRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The amount value and currency.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-total-amount-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TotalAmountRestriction
---
