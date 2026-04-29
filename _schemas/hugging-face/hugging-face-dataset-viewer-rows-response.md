---
description: ''
layout: schema
name: RowsResponse
properties_list:
- description: Column definitions and types
  name: features
  type: array
- description: Row data
  name: rows
  type: array
- description: Total number of rows in the split
  name: num_rows_total
  type: integer
- description: Number of rows per page
  name: num_rows_per_page
  type: integer
- description: Whether this is a partial result
  name: partial
  type: boolean
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-dataset-viewer-rows-response-schema.json
slug: hugging-face-dataset-viewer-rows-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RowsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"Column definitions and types\"\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"description\": \"Row data\"\n    },\n    \"num_rows_total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of rows in the split\"\n    },\n    \"num_rows_per_page\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows per page\"\n    },\n    \"partial\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a partial result\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-dataset-viewer-rows-response-schema.json
tags: []
title: RowsResponse
---
