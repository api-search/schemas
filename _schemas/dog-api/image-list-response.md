---
description: Response envelope returning a list of dog image URLs.
layout: schema
name: ImageListResponse
properties_list:
- description: ''
  name: message
  type: array
- description: ''
  name: status
  type: string
provider_name: Dog API
provider_slug: dog-api
schema_file: json-schema/image-list-response.json
slug: image-list-response
source_filename: image-list-response.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dog-api/refs/heads/main/json-schema/image-list-response.json\",\n  \"title\": \"ImageListResponse\",\n  \"description\": \"Response envelope returning a list of dog image URLs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"success\", \"error\"]\n    }\n  },\n  \"required\": [\"message\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dog-api/refs/heads/main/json-schema/image-list-response.json
tags:
- Dogs
- Images
- Open Data
- Open Source
title: ImageListResponse
---
