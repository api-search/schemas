---
description: CalculationResponse schema from Avalara API
layout: schema
name: CalculationResponse
properties_list:
- description: ''
  name: header
  type: object
- description: ''
  name: lines
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-brazil-calculation-response-schema.json
slug: avatax-brazil-calculation-response
source_filename: avatax-brazil-calculation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-calculation-response-schema.json\",\n  \"title\": \"CalculationResponse\",\n  \"description\": \"CalculationResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"header\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"transactionId\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CalculationResultLine\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-calculation-response-schema.json
tags:
- Taxes
title: CalculationResponse
---
