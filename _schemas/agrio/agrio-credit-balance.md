---
description: Current API credit balance for the authenticated account.
layout: schema
name: Credit Balance
properties_list:
- description: Number of available credits remaining.
  name: balance
  type: integer
- description: Credit unit type.
  name: currency
  type: string
- description: Unique identifier for the API account.
  name: account_id
  type: string
provider_name: agrio
provider_slug: agrio
schema_file: json-schema/agrio-credit-balance-schema.json
slug: agrio-credit-balance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-credit-balance-schema.json\",\n  \"title\": \"Credit Balance\",\n  \"description\": \"Current API credit balance for the authenticated account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balance\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of available credits remaining.\",\n      \"example\": 450\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Credit unit type.\",\n      \"example\": \"credits\"\n    },\n    \"account_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API account.\",\n      \"example\": \"acc-500123\"\n    }\n  },\n  \"required\": [\n    \"balance\",\n    \"currency\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-credit-balance-schema.json
tags:
- Agriculture
- Plant Disease
- Pest Detection
- AI
- Crop Advisory
title: Credit Balance
---
