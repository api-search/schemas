---
description: ClassificationRequestList schema from Avalara API
layout: schema
name: ClassificationRequestList
properties_list:
- description: ''
  name: '@recordSetCount'
  type: integer
- description: ''
  name: value
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/item-classification-classification-request-list-schema.json
slug: item-classification-classification-request-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-request-list-schema.json\",\n  \"title\": \"ClassificationRequestList\",\n  \"description\": \"ClassificationRequestList schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@recordSetCount\": {\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ClassificationRequestSummary\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-request-list-schema.json
tags:
- Taxes
title: ClassificationRequestList
---
