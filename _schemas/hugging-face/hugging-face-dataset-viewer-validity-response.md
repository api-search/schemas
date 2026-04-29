---
description: ''
layout: schema
name: ValidityResponse
properties_list:
- description: Whether preview (first rows) is available
  name: preview
  type: boolean
- description: Whether the full viewer is available
  name: viewer
  type: boolean
- description: Whether full-text search is available
  name: search
  type: boolean
- description: Whether filtering is available
  name: filter
  type: boolean
- description: Whether statistics are available
  name: statistics
  type: boolean
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-dataset-viewer-validity-response-schema.json
slug: hugging-face-dataset-viewer-validity-response
source_filename: hugging-face-dataset-viewer-validity-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ValidityResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"preview\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether preview (first rows) is available\"\n    },\n    \"viewer\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the full viewer is available\"\n    },\n    \"search\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether full-text search is available\"\n    },\n    \"filter\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether filtering is available\"\n    },\n    \"statistics\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether statistics are available\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-dataset-viewer-validity-response-schema.json
tags: []
title: ValidityResponse
---
