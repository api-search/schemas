---
description: Paginated list of accounts
layout: schema
name: AccountList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/banking-account-list-schema.json
slug: banking-account-list
source_filename: banking-account-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-account-list-schema.json\",\n  \"title\": \"AccountList\",\n  \"description\": \"Paginated list of accounts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Account\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 5\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-account-list-schema.json
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: AccountList
---
