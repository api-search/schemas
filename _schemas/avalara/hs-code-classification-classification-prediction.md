---
description: ClassificationPrediction schema from Avalara API
layout: schema
name: ClassificationPrediction
properties_list:
- description: Predicted HS Code
  name: hsCode
  type: string
- description: HS Code description
  name: description
  type: string
- description: Confidence score (0-1)
  name: confidence
  type: number
- description: ''
  name: parentCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/hs-code-classification-classification-prediction-schema.json
slug: hs-code-classification-classification-prediction
source_filename: hs-code-classification-classification-prediction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/hs-code-classification-classification-prediction-schema.json\",\n  \"title\": \"ClassificationPrediction\",\n  \"description\": \"ClassificationPrediction schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hsCode\": {\n      \"type\": \"string\",\n      \"description\": \"Predicted HS Code\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"HS Code description\"\n    },\n    \"confidence\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Confidence score (0-1)\"\n    },\n    \"parentCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/hs-code-classification-classification-prediction-schema.json
tags:
- Taxes
title: ClassificationPrediction
---
