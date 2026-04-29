---
description: ''
layout: schema
name: CalculationsSummary
properties_list:
- description: Last poll status of the calculation.
  name: status
  type: string
- description: Number of calculation units in batch.
  name: units
  type: integer
- description: Request time of calculation.
  name: requestTime
  type: string
- description: Last poll time of calculation.
  name: lastPollTime
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-calculations-summary-schema.json
slug: factset-pa-engine-calculations-summary
source_filename: factset-pa-engine-calculations-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CalculationsSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Last poll status of the calculation.\"\n    },\n    \"units\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of calculation units in batch.\"\n    },\n    \"requestTime\": {\n      \"type\": \"string\",\n      \"description\": \"Request time of calculation.\"\n    },\n    \"lastPollTime\": {\n      \"type\": \"string\",\n      \"description\": \"Last poll time of calculation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-calculations-summary-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CalculationsSummary
---
