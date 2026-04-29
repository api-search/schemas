---
description: ''
layout: schema
name: ConfigurationAccount
properties_list:
- description: Benchmark code.
  name: benchmarkCode
  type: string
- description: Benchmark name.
  name: benchmarkName
  type: string
- description: Maximum end date.
  name: maxEndDate
  type: string
- description: Minimum start date.
  name: minStartDate
  type: string
- description: Locking date.
  name: lockingDate
  type: string
- description: Account name.
  name: name
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vault-configuration-account-schema.json
slug: factset-vault-configuration-account
source_filename: factset-vault-configuration-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConfigurationAccount\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"benchmarkCode\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark code.\"\n    },\n    \"benchmarkName\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark name.\"\n    },\n    \"maxEndDate\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum end date.\"\n    },\n    \"minStartDate\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum start date.\"\n    },\n    \"lockingDate\": {\n      \"type\": \"string\",\n      \"description\": \"Locking date.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Account name.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vault-configuration-account-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ConfigurationAccount
---
