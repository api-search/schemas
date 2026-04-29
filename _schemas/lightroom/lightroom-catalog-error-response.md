---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: code
  type: integer
- description: ''
  name: description
  type: string
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-catalog-error-response-schema.json
slug: lightroom-catalog-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-catalog-error-response-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: ErrorResponse
---
