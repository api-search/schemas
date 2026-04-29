---
description: ''
layout: schema
name: StatisticsResponse
properties_list:
- description: Total number of examples analyzed
  name: num_examples
  type: integer
- description: ''
  name: statistics
  type: array
- description: ''
  name: partial
  type: boolean
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-dataset-viewer-statistics-response-schema.json
slug: hugging-face-dataset-viewer-statistics-response
source_filename: hugging-face-dataset-viewer-statistics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatisticsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"num_examples\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of examples analyzed\"\n    },\n    \"statistics\": {\n      \"type\": \"array\"\n    },\n    \"partial\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-dataset-viewer-statistics-response-schema.json
tags: []
title: StatisticsResponse
---
