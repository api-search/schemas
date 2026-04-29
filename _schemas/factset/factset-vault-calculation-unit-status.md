---
description: ''
layout: schema
name: CalculationUnitStatus
properties_list:
- description: The status of calculation unit.
  name: status
  type: string
- description: The error in a calculation unit.
  name: errors
  type: array
- description: The result URL of the calculation.
  name: result
  type: string
- description: The progress of the calculation unit.
  name: progress
  type: string
- description: The points for the calculation unit.
  name: points
  type: integer
- description: The warnings in a calculation unit.
  name: warnings
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vault-calculation-unit-status-schema.json
slug: factset-vault-calculation-unit-status
source_filename: factset-vault-calculation-unit-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CalculationUnitStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of calculation unit.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"The error in a calculation unit.\"\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"description\": \"The result URL of the calculation.\"\n    },\n    \"progress\": {\n      \"type\": \"string\",\n      \"description\": \"The progress of the calculation unit.\"\n    },\n    \"points\": {\n      \"type\": \"integer\",\n      \"description\": \"The points for the calculation unit.\"\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"description\": \"The warnings in a calculation unit.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vault-calculation-unit-status-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CalculationUnitStatus
---
