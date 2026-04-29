---
description: InternationalTransactionRestriction schema from Adyen API
layout: schema
name: InternationalTransactionRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: 'Boolean indicating whether transaction is an international transaction. Possible values: - **true**: The transaction is an international transaction. - **false**: The transaction is a domestic transac'
  name: value
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-international-transaction-restriction-schema.json
slug: configuration-international-transaction-restriction
source_filename: configuration-international-transaction-restriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-international-transaction-restriction-schema.json\",\n  \"title\": \"InternationalTransactionRestriction\",\n  \"description\": \"InternationalTransactionRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Boolean indicating whether transaction is an international transaction.\\n\\nPossible values:\\n\\n- **true**: The transaction is an international transaction.\\n\\n- **false**: The transaction is a domestic transaction.\\n\\n\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-international-transaction-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InternationalTransactionRestriction
---
