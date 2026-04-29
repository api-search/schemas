---
description: ''
layout: schema
name: AccountListResponse
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: data
  type: array
- description: ''
  name: size
  type: integer
provider_name: Basiq
provider_slug: basiq
schema_file: json-schema/accountlistresponse.json
slug: accountlistresponse
source_filename: accountlistresponse.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/accountlistresponse.json\",\n  \"title\": \"AccountListResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"default\": \"list\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Account\"\n      }\n    },\n    \"size\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/accountlistresponse.json
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
title: AccountListResponse
---
