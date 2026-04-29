---
description: Store schema from Adyen API
layout: schema
name: Store
properties_list:
- description: The address of the store.
  name: address
  type: object
- description: The description of the store.
  name: description
  type: string
- description: The list of terminals assigned to the store.
  name: inStoreTerminals
  type: array
- description: The code of the merchant account.
  name: merchantAccountCode
  type: string
- description: 'The status of the store: - `PreActive`: the store has been created, but not yet activated. - `Active`: the store has been activated. This means you can process payments for this store. - `Inactive`: t'
  name: status
  type: string
- description: The code of the store.
  name: store
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/pos-terminal-store-schema.json
slug: pos-terminal-store
source_filename: pos-terminal-store-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-store-schema.json\",\n  \"title\": \"Store\",\n  \"description\": \"Store schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the store.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"description\": {\n      \"description\": \"The description of the store.\",\n      \"type\": \"string\"\n    },\n    \"inStoreTerminals\": {\n      \"description\": \"The list of terminals assigned to the store.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantAccountCode\": {\n      \"description\": \"The code of the merchant account.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the store:\\n\\n- `PreActive`:\
  \ the store has been created, but not yet activated. \\n\\n- `Active`: the store has been activated. This means you can process payments for this store. \\n\\n- `Inactive`: the store is currently not active. \\n\\n- `InactiveWithModifications`: the store is currently not active, but payment modifications such as refunds are possible. \\n\\n- `Closed`: the store has been closed. \",\n      \"type\": \"string\"\n    },\n    \"store\": {\n      \"description\": \"The code of the store.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"store\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-store-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Store
---
