---
description: FetchResult_ItemModel schema from Avalara API
layout: schema
name: FetchResult_ItemModel
properties_list:
- description: ''
  name: '@recordsetCount'
  type: integer
- description: ''
  name: value
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-fetch-result_-item-model-schema.json
slug: avatax-rest-fetch-result_-item-model
source_filename: avatax-rest-fetch-result_-item-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-fetch-result_-item-model-schema.json\",\n  \"title\": \"FetchResult_ItemModel\",\n  \"description\": \"FetchResult_ItemModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@recordsetCount\": {\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ItemModel\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-fetch-result_-item-model-schema.json
tags:
- Taxes
title: FetchResult_ItemModel
---
