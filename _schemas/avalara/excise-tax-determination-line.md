---
description: TaxDeterminationLine schema from Avalara API
layout: schema
name: TaxDeterminationLine
properties_list:
- description: ''
  name: lineNumber
  type: string
- description: ''
  name: productCode
  type: string
- description: ''
  name: taxes
  type: array
- description: ''
  name: totalTax
  type: number
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-tax-determination-line-schema.json
slug: excise-tax-determination-line
source_filename: excise-tax-determination-line-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-tax-determination-line-schema.json\",\n  \"title\": \"TaxDeterminationLine\",\n  \"description\": \"TaxDeterminationLine schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineNumber\": {\n      \"type\": \"string\"\n    },\n    \"productCode\": {\n      \"type\": \"string\"\n    },\n    \"taxes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ExciseTaxDetail\"\n      }\n    },\n    \"totalTax\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-tax-determination-line-schema.json
tags:
- Taxes
title: TaxDeterminationLine
---
