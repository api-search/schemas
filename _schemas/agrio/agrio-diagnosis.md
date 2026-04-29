---
description: Complete plant diagnosis result including crop identification and ranked disease list.
layout: schema
name: Diagnosis
properties_list:
- description: Identified or confirmed crop type.
  name: crop
  type: string
- description: Confidence level for crop identification (high, medium, low).
  name: cropConfidence
  type: string
- description: Ranked list of disease/pest diagnoses sorted by confidence descending.
  name: idArray
  type: array
provider_name: agrio
provider_slug: agrio
schema_file: json-schema/agrio-diagnosis-schema.json
slug: agrio-diagnosis
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-diagnosis-schema.json\",\n  \"title\": \"Diagnosis\",\n  \"description\": \"Complete plant diagnosis result including crop identification and ranked disease list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"crop\": {\n      \"type\": \"string\",\n      \"description\": \"Identified or confirmed crop type.\",\n      \"example\": \"tomato\"\n    },\n    \"cropConfidence\": {\n      \"type\": \"string\",\n      \"description\": \"Confidence level for crop identification (high, medium, low).\",\n      \"example\": \"high\"\n    },\n    \"idArray\": {\n      \"type\": \"array\",\n      \"description\": \"Ranked list of disease/pest diagnoses sorted by confidence descending.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DiagnosisResult\"\n      }\n    }\n  },\n  \"required\": [\n \
  \   \"crop\",\n    \"cropConfidence\",\n    \"idArray\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-diagnosis-schema.json
tags:
- Agriculture
- Plant Disease
- Pest Detection
- AI
- Crop Advisory
title: Diagnosis
---
