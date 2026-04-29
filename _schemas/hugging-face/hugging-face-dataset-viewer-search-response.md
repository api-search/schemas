---
description: ''
layout: schema
name: SearchResponse
properties_list:
- description: ''
  name: features
  type: array
- description: ''
  name: rows
  type: array
- description: Total number of matching rows
  name: num_rows_total
  type: integer
- description: ''
  name: num_rows_per_page
  type: integer
- description: ''
  name: partial
  type: boolean
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-dataset-viewer-search-response-schema.json
slug: hugging-face-dataset-viewer-search-response
source_filename: hugging-face-dataset-viewer-search-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"features\": {\n      \"type\": \"array\"\n    },\n    \"rows\": {\n      \"type\": \"array\"\n    },\n    \"num_rows_total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching rows\"\n    },\n    \"num_rows_per_page\": {\n      \"type\": \"integer\"\n    },\n    \"partial\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-dataset-viewer-search-response-schema.json
tags: []
title: SearchResponse
---
