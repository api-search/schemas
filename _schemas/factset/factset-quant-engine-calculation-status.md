---
description: ''
layout: schema
name: CalculationStatus
properties_list:
- description: Calculation's identifier
  name: calculationid
  type: string
- description: Calculation's status
  name: status
  type: string
- description: Number of calculation units in batch.
  name: units
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-quant-engine-calculation-status-schema.json
slug: factset-quant-engine-calculation-status
source_filename: factset-quant-engine-calculation-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CalculationStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"calculationid\": {\n      \"type\": \"string\",\n      \"description\": \"Calculation's identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Calculation's status\"\n    },\n    \"units\": {\n      \"type\": \"object\",\n      \"description\": \"Number of calculation units in batch.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-quant-engine-calculation-status-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CalculationStatus
---
