---
description: ''
layout: schema
name: CalculationStatus
properties_list:
- description: The unique ID for this calculation
  name: id
  type: string
- description: ''
  name: status
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-programmatic-environment-calculation-status-schema.json
slug: factset-programmatic-environment-calculation-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CalculationStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID for this calculation\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-programmatic-environment-calculation-status-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CalculationStatus
---
