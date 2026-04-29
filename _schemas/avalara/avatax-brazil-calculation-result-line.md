---
description: CalculationResultLine schema from Avalara API
layout: schema
name: CalculationResultLine
properties_list:
- description: ''
  name: lineCode
  type: string
- description: ''
  name: taxes
  type: array
- description: ''
  name: totalTax
  type: number
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-brazil-calculation-result-line-schema.json
slug: avatax-brazil-calculation-result-line
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-calculation-result-line-schema.json\",\n  \"title\": \"CalculationResultLine\",\n  \"description\": \"CalculationResultLine schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineCode\": {\n      \"type\": \"string\"\n    },\n    \"taxes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BrazilTaxDetail\"\n      }\n    },\n    \"totalTax\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-calculation-result-line-schema.json
tags:
- Taxes
title: CalculationResultLine
---
