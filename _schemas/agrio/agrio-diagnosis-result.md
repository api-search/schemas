---
description: A single disease or pest identification result.
layout: schema
name: Diagnosis Result
properties_list:
- description: Unique identifier for the disease or pest.
  name: id
  type: string
- description: Confidence score for this diagnosis (0.0 to 1.0).
  name: confidence
  type: number
- description: Common name of the disease or pest.
  name: commonName
  type: string
- description: Scientific name of the disease or pest.
  name: scientificName
  type: string
provider_name: agrio
provider_slug: agrio
schema_file: json-schema/agrio-diagnosis-result-schema.json
slug: agrio-diagnosis-result
source_filename: agrio-diagnosis-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-diagnosis-result-schema.json\",\n  \"title\": \"Diagnosis Result\",\n  \"description\": \"A single disease or pest identification result.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the disease or pest.\",\n      \"example\": \"early_blight\"\n    },\n    \"confidence\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Confidence score for this diagnosis (0.0 to 1.0).\",\n      \"example\": 0.87\n    },\n    \"commonName\": {\n      \"type\": \"string\",\n      \"description\": \"Common name of the disease or pest.\",\n      \"example\": \"Early Blight\"\n    },\n    \"scientificName\": {\n      \"type\": \"string\",\n      \"description\": \"Scientific name of the disease\
  \ or pest.\",\n      \"example\": \"Alternaria solani\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"confidence\",\n    \"commonName\",\n    \"scientificName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-diagnosis-result-schema.json
tags:
- Agriculture
- Plant Disease
- Pest Detection
- AI
- Crop Advisory
title: Diagnosis Result
---
