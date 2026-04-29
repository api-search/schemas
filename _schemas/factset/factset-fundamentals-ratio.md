---
description: A single pre-calculated financial ratio for a security and fiscal period.
layout: schema
name: Ratio
properties_list:
- description: Identifier that was used for the request.
  name: requestId
  type: string
- description: FactSet Regional Security Identifier.
  name: fsymId
  type: '[''string'', ''null'']'
- description: The ratio metric identifier.
  name: metric
  type: '[''string'', ''null'']'
- description: Periodicity of the fiscal period.
  name: periodicity
  type: '[''string'', ''null'']'
- description: Fiscal period indicator.
  name: fiscalPeriod
  type: '[''integer'', ''null'']'
- description: Fiscal year in YYYY format.
  name: fiscalYear
  type: '[''integer'', ''null'']'
- description: The normalized date the fiscal period ended.
  name: fiscalEndDate
  type: '[''string'', ''null'']'
- description: ISO 4217 currency code.
  name: currency
  type: '[''string'', ''null'']'
- description: The calculated ratio value.
  name: value
  type: '[''number'', ''null'']'
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-ratio-schema.json
slug: factset-fundamentals-ratio
source_filename: factset-fundamentals-ratio-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Ratio\",\n  \"type\": \"object\",\n  \"description\": \"A single pre-calculated financial ratio for a security and fiscal period.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"FactSet Regional Security Identifier.\"\n    },\n    \"metric\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The ratio metric identifier.\"\n    },\n    \"periodicity\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Periodicity of the fiscal period.\"\n    },\n    \"fiscalPeriod\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Fiscal period indicator.\"\n    },\n    \"fiscalYear\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Fiscal year\
  \ in YYYY format.\"\n    },\n    \"fiscalEndDate\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The normalized date the fiscal period ended.\"\n    },\n    \"currency\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"ISO 4217 currency code.\"\n    },\n    \"value\": {\n      \"type\": \"['number', 'null']\",\n      \"description\": \"The calculated ratio value.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-ratio-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Ratio
---
