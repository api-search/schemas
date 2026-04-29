---
description: ''
layout: schema
name: ParquetResponse
properties_list:
- description: ''
  name: parquet_files
  type: array
- description: Whether only partial data was converted
  name: partial
  type: boolean
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-dataset-viewer-parquet-response-schema.json
slug: hugging-face-dataset-viewer-parquet-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ParquetResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parquet_files\": {\n      \"type\": \"array\"\n    },\n    \"partial\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether only partial data was converted\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-dataset-viewer-parquet-response-schema.json
tags: []
title: ParquetResponse
---
