---
description: List of accounts
layout: schema
name: AccountListResponse
properties_list:
- description: ''
  name: accounts
  type: array
- description: ''
  name: totalCount
  type: integer
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/accountlistresponse-schema.json
slug: accountlistresponse
source_filename: accountlistresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/accountlistresponse-schema.json\",\n  \"title\": \"AccountListResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of accounts\",\n  \"properties\": {\n    \"accounts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Account\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/accountlistresponse-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: AccountListResponse
---
