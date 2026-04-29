---
description: ''
layout: schema
name: SplitsResponse
properties_list:
- description: ''
  name: splits
  type: array
- description: ''
  name: pending
  type: array
- description: ''
  name: failed
  type: array
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-dataset-viewer-splits-response-schema.json
slug: hugging-face-dataset-viewer-splits-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SplitsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"splits\": {\n      \"type\": \"array\"\n    },\n    \"pending\": {\n      \"type\": \"array\"\n    },\n    \"failed\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-dataset-viewer-splits-response-schema.json
tags: []
title: SplitsResponse
---
