---
description: ClassifyResponse schema from Avalara API
layout: schema
name: ClassifyResponse
properties_list:
- description: ''
  name: itemCode
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: predictions
  type: array
- description: Recommended Avalara tax code
  name: avataxCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/hs-code-classification-classify-response-schema.json
slug: hs-code-classification-classify-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/hs-code-classification-classify-response-schema.json\",\n  \"title\": \"ClassifyResponse\",\n  \"description\": \"ClassifyResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"itemCode\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"predictions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ClassificationPrediction\"\n      }\n    },\n    \"avataxCode\": {\n      \"type\": \"string\",\n      \"description\": \"Recommended Avalara tax code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/hs-code-classification-classify-response-schema.json
tags:
- Taxes
title: ClassifyResponse
---
