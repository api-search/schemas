---
description: Paginated list of accounts
layout: schema
name: AccountListResponse
properties_list:
- description: ''
  name: accounts
  type: array
- description: Total number of accounts
  name: totalCount
  type: integer
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: offset
  type: integer
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/accountlistresponse-schema.json
slug: accountlistresponse
source_filename: accountlistresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/accountlistresponse-schema.json\",\n  \"title\": \"AccountListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of accounts\",\n  \"properties\": {\n    \"accounts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Account\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of accounts\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/accountlistresponse-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: AccountListResponse
---
