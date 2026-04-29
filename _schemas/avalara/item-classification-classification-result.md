---
description: ClassificationResult schema from Avalara API
layout: schema
name: ClassificationResult
properties_list:
- description: ''
  name: itemCode
  type: string
- description: ''
  name: description
  type: string
- description: Classified HS Code
  name: hsCode
  type: string
- description: ''
  name: hsCodeDescription
  type: string
- description: Classification confidence score (0-1)
  name: confidence
  type: number
- description: ''
  name: country
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/item-classification-classification-result-schema.json
slug: item-classification-classification-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-result-schema.json\",\n  \"title\": \"ClassificationResult\",\n  \"description\": \"ClassificationResult schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"itemCode\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"hsCode\": {\n      \"type\": \"string\",\n      \"description\": \"Classified HS Code\"\n    },\n    \"hsCodeDescription\": {\n      \"type\": \"string\"\n    },\n    \"confidence\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Classification confidence score (0-1)\"\n    },\n    \"country\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-result-schema.json
tags:
- Taxes
title: ClassificationResult
---
