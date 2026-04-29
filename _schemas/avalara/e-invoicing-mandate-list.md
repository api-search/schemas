---
description: MandateList schema from Avalara API
layout: schema
name: MandateList
properties_list:
- description: ''
  name: '@recordSetCount'
  type: integer
- description: ''
  name: value
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-mandate-list-schema.json
slug: e-invoicing-mandate-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-mandate-list-schema.json\",\n  \"title\": \"MandateList\",\n  \"description\": \"MandateList schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@recordSetCount\": {\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Mandate\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-mandate-list-schema.json
tags:
- Taxes
title: MandateList
---
