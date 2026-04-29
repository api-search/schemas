---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: HTTP status code
  name: code
  type: integer
- description: Error description
  name: description
  type: string
- description: ''
  name: errors
  type: array
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-services-error-response-schema.json
slug: lightroom-services-error-response
source_filename: lightroom-services-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Error description\"\n    },\n    \"errors\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-services-error-response-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: ErrorResponse
---
