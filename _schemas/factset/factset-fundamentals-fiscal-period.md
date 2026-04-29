---
description: Fiscal period date range specification. Calendar dates that will fall back to the most recently completed period during resolution.
layout: schema
name: FiscalPeriod
properties_list:
- description: The fiscal period start expressed as YYYY-MM-DD.
  name: start
  type: string
- description: The fiscal period end expressed as YYYY-MM-DD.
  name: end
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-fiscal-period-schema.json
slug: factset-fundamentals-fiscal-period
source_filename: factset-fundamentals-fiscal-period-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FiscalPeriod\",\n  \"type\": \"object\",\n  \"description\": \"Fiscal period date range specification. Calendar dates that will fall back to the most recently completed period during resolution.\",\n  \"properties\": {\n    \"start\": {\n      \"type\": \"string\",\n      \"description\": \"The fiscal period start expressed as YYYY-MM-DD.\"\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"description\": \"The fiscal period end expressed as YYYY-MM-DD.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-fiscal-period-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: FiscalPeriod
---
