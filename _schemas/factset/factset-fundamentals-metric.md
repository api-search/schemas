---
description: Metadata for a single available fundamental metric including its category, data type, and documentation reference.
layout: schema
name: Metric
properties_list:
- description: Metric identifier to be used as input in the metrics parameter.
  name: metric
  type: '[''string'', ''null'']'
- description: Plain text name of the metric.
  name: name
  type: '[''string'', ''null'']'
- description: Primary category such as INCOME_STATEMENT, BALANCE_SHEET, CASH_FLOW, or RATIOS.
  name: category
  type: '[''string'', ''null'']'
- description: Sub-category such as ASSETS, SUPPLEMENTAL, SHAREHOLDERS_EQUITY, VALUATION, PROFITABILITY, etc.
  name: subcategory
  type: '[''string'', ''null'']'
- description: Online Assistant Page ID in D***** format for methodology lookup.
  name: oaPageId
  type: '[''string'', ''null'']'
- description: Online Assistant URL for methodology definitions.
  name: oaUrl
  type: '[''string'', ''null'']'
- description: The factor for the metric (e.g. 1000000 = millions).
  name: factor
  type: '[''integer'', ''null'']'
- description: Standard Data Feed package availability. BASIC or ADVANCED. Null indicates API-only availability.
  name: sdfPackage
  type: '[''string'', ''null'']'
- description: The data type for the metric (date, doubleArray, float, floatArray, intArray, string, stringArray).
  name: dataType
  type: '[''string'', ''null'']'
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-metric-schema.json
slug: factset-fundamentals-metric
source_filename: factset-fundamentals-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Metric\",\n  \"type\": \"object\",\n  \"description\": \"Metadata for a single available fundamental metric including its category, data type, and documentation reference.\",\n  \"properties\": {\n    \"metric\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Metric identifier to be used as input in the metrics parameter.\"\n    },\n    \"name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Plain text name of the metric.\"\n    },\n    \"category\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Primary category such as INCOME_STATEMENT, BALANCE_SHEET, CASH_FLOW, or RATIOS.\"\n    },\n    \"subcategory\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Sub-category such as ASSETS, SUPPLEMENTAL, SHAREHOLDERS_EQUITY, VALUATION, PROFITABILITY, etc.\"\n    },\n    \"oaPageId\": {\n      \"type\": \"['string',\
  \ 'null']\",\n      \"description\": \"Online Assistant Page ID in D***** format for methodology lookup.\"\n    },\n    \"oaUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Online Assistant URL for methodology definitions.\"\n    },\n    \"factor\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"The factor for the metric (e.g. 1000000 = millions).\"\n    },\n    \"sdfPackage\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Standard Data Feed package availability. BASIC or ADVANCED. Null indicates API-only availability.\"\n    },\n    \"dataType\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The data type for the metric (date, doubleArray, float, floatArray, intArray, string, stringArray).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-metric-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Metric
---
