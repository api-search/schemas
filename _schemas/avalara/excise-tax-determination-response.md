---
description: TaxDeterminationResponse schema from Avalara API
layout: schema
name: TaxDeterminationResponse
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: transactionLines
  type: array
- description: ''
  name: totalTaxAmount
  type: number
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-tax-determination-response-schema.json
slug: excise-tax-determination-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-tax-determination-response-schema.json\",\n  \"title\": \"TaxDeterminationResponse\",\n  \"description\": \"TaxDeterminationResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Success\",\n        \"Error\",\n        \"Partial\"\n      ]\n    },\n    \"transactionLines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaxDeterminationLine\"\n      }\n    },\n    \"totalTaxAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-tax-determination-response-schema.json
tags:
- Taxes
title: TaxDeterminationResponse
---
