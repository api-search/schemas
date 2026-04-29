---
description: A single consensus estimate data point aggregating analyst projections for a security, metric, and fiscal period.
layout: schema
name: Estimate
properties_list:
- description: Identifier that was used for the request.
  name: requestId
  type: string
- description: FactSet Regional Security Identifier.
  name: fsymId
  type: '[''string'', ''null'']'
- description: The estimate metric identifier.
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
- description: The date the fiscal period ends.
  name: fiscalEndDate
  type: '[''string'', ''null'']'
- description: ISO 4217 currency code.
  name: currency
  type: '[''string'', ''null'']'
- description: Number of analyst estimates included in the consensus.
  name: estimateCount
  type: '[''integer'', ''null'']'
- description: Mean (average) of analyst estimates.
  name: mean
  type: '[''number'', ''null'']'
- description: Median of analyst estimates.
  name: median
  type: '[''number'', ''null'']'
- description: Highest analyst estimate.
  name: high
  type: '[''number'', ''null'']'
- description: Lowest analyst estimate.
  name: low
  type: '[''number'', ''null'']'
- description: Standard deviation of analyst estimates.
  name: standardDeviation
  type: '[''number'', ''null'']'
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-estimate-schema.json
slug: factset-fundamentals-estimate
source_filename: factset-fundamentals-estimate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Estimate\",\n  \"type\": \"object\",\n  \"description\": \"A single consensus estimate data point aggregating analyst projections for a security, metric, and fiscal period.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"FactSet Regional Security Identifier.\"\n    },\n    \"metric\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The estimate metric identifier.\"\n    },\n    \"periodicity\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Periodicity of the fiscal period.\"\n    },\n    \"fiscalPeriod\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Fiscal period indicator.\"\n    },\n    \"fiscalYear\": {\n      \"type\": \"['integer',\
  \ 'null']\",\n      \"description\": \"Fiscal year in YYYY format.\"\n    },\n    \"fiscalEndDate\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The date the fiscal period ends.\"\n    },\n    \"currency\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"ISO 4217 currency code.\"\n    },\n    \"estimateCount\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Number of analyst estimates included in the consensus.\"\n    },\n    \"mean\": {\n      \"type\": \"['number', 'null']\",\n      \"description\": \"Mean (average) of analyst estimates.\"\n    },\n    \"median\": {\n      \"type\": \"['number', 'null']\",\n      \"description\": \"Median of analyst estimates.\"\n    },\n    \"high\": {\n      \"type\": \"['number', 'null']\",\n      \"description\": \"Highest analyst estimate.\"\n    },\n    \"low\": {\n      \"type\": \"['number', 'null']\",\n      \"description\": \"Lowest analyst estimate.\"\n    },\n    \"standardDeviation\"\
  : {\n      \"type\": \"['number', 'null']\",\n      \"description\": \"Standard deviation of analyst estimates.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-estimate-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Estimate
---
