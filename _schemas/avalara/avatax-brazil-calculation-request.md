---
description: CalculationRequest schema from Avalara API
layout: schema
name: CalculationRequest
properties_list:
- description: ''
  name: header
  type: object
- description: ''
  name: lines
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-brazil-calculation-request-schema.json
slug: avatax-brazil-calculation-request
source_filename: avatax-brazil-calculation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-calculation-request-schema.json\",\n  \"title\": \"CalculationRequest\",\n  \"description\": \"CalculationRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"header\",\n    \"lines\"\n  ],\n  \"properties\": {\n    \"header\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"transactionType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Sale\",\n            \"Purchase\",\n            \"Return\",\n            \"Transfer\"\n          ]\n        },\n        \"companyLocation\": {\n          \"type\": \"string\",\n          \"description\": \"Company establishment code\"\n        },\n        \"documentCode\": {\n          \"type\": \"string\"\n        },\n        \"transactionDate\": {\n          \"type\": \"string\",\n\
  \          \"format\": \"date\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"default\": \"BRL\"\n        }\n      }\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CalculationLine\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-calculation-request-schema.json
tags:
- Taxes
title: CalculationRequest
---
