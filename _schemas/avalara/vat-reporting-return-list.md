---
description: ReturnList schema from Avalara API
layout: schema
name: ReturnList
properties_list:
- description: ''
  name: '@recordSetCount'
  type: integer
- description: ''
  name: value
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/vat-reporting-return-list-schema.json
slug: vat-reporting-return-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-return-list-schema.json\",\n  \"title\": \"ReturnList\",\n  \"description\": \"ReturnList schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@recordSetCount\": {\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/VATReturn\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-return-list-schema.json
tags:
- Taxes
title: ReturnList
---
