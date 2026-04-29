---
description: CalcAdjRequest schema from Avalara API
layout: schema
name: CalcAdjRequest
properties_list:
- description: ''
  name: cmpn
  type: object
- description: ''
  name: inv
  type: array
- description: ''
  name: adj
  type: object
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-calc-adj-request-schema.json
slug: communications-calc-adj-request
source_filename: communications-calc-adj-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-calc-adj-request-schema.json\",\n  \"title\": \"CalcAdjRequest\",\n  \"description\": \"CalcAdjRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cmpn\": {\n      \"$ref\": \"#/components/schemas/CompanyData\"\n    },\n    \"inv\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Invoice\"\n      }\n    },\n    \"adj\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"disc\": {\n          \"type\": \"integer\",\n          \"description\": \"Discount type\"\n        },\n        \"adj\": {\n          \"type\": \"integer\",\n          \"description\": \"Adjustment method\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-calc-adj-request-schema.json
tags:
- Taxes
title: CalcAdjRequest
---
