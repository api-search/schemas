---
description: Response envelope returning a single dog image URL.
layout: schema
name: ImageResponse
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: status
  type: string
provider_name: Dog API
provider_slug: dog-api
schema_file: json-schema/image-response.json
slug: image-response
source_filename: image-response.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dog-api/refs/heads/main/json-schema/image-response.json\",\n  \"title\": \"ImageResponse\",\n  \"description\": \"Response envelope returning a single dog image URL.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"success\", \"error\"]\n    }\n  },\n  \"required\": [\"message\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dog-api/refs/heads/main/json-schema/image-response.json
tags:
- Dogs
- Images
- Open Data
- Open Source
title: ImageResponse
---
