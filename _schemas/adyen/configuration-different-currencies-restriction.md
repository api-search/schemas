---
description: DifferentCurrenciesRestriction schema from Adyen API
layout: schema
name: DifferentCurrenciesRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: 'Checks the currency of the payment against the currency of the payment instrument. Possible values: - **true**: The currency of the payment is different from the currency of the payment instrument. - '
  name: value
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-different-currencies-restriction-schema.json
slug: configuration-different-currencies-restriction
source_filename: configuration-different-currencies-restriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-different-currencies-restriction-schema.json\",\n  \"title\": \"DifferentCurrenciesRestriction\",\n  \"description\": \"DifferentCurrenciesRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Checks the currency of the payment against the currency of the payment instrument.\\n\\nPossible values:\\n\\n- **true**: The currency of the payment is different from the currency of the payment instrument.\\n\\n- **false**: The currencies are the same.\\n\\n\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-different-currencies-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DifferentCurrenciesRestriction
---
